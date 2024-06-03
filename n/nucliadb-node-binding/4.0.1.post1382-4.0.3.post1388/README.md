# Comparing `tmp/nucliadb_node_binding-4.0.1.post1382.tar.gz` & `tmp/nucliadb_node_binding-4.0.3.post1388.tar.gz`

## Comparing `nucliadb_node_binding-4.0.1.post1382.tar` & `nucliadb_node_binding-4.0.3.post1388.tar`

### file list

```diff
@@ -1,352 +1,352 @@
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22721 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10092 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3435 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2152 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3523 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127     4424 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/config.rs
--rw-r--r--   0     1001      127    12340 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    29379 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11821 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    15068 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1741 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    11691 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2513 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127     8487 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2607 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    23029 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    25379 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     7189 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     2157 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127    10472 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2282 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127      940 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    18009 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15288 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     3267 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32.rs
--rw-r--r--   0     1001      127     4415 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32_unaligned.rs
--rw-r--r--   0     1001      127      903 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/vector_types/mod.rs
--rw-r--r--   0     1001      127     3877 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/tests/test_basic_search.rs
--rw-r--r--   0     1001      127     2895 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    43269 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17239 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17039 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     7990 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9523 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    43324 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18147 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    19055 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1496 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    11343 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13965 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2300 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12999 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3394 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2489 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      332 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1455 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8294 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3035 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11334 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     1111 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/errors.rs
--rw-r--r--   0     1001      127     2656 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18813 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    19577 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1553 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13111 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14260 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11563 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    15700 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    11202 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/indexes.rs
--rw-r--r--   0     1001      127    10055 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1168 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    28646 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    27248 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     7048 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/tests.rs
--rw-r--r--   0     1001      127     1890 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/versioning.rs
--rw-r--r--   0     1001      127    10199 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8386 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     9372 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     2508 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
--rw-r--r--   0     1001      127     6862 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5554 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0     1001      127     5337 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     3063 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     5462 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2944 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2023 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8450 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2557 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     5688 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2340 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127     8473 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/audit.rs
--rw-r--r--   0     1001      127    46350 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127    14122 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1271 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    95906 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    17860 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    62254 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    24308 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    50492 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127    10160 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/Cargo.toml
--rw-r--r--   0     1001      127     1017 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/.cargo/config.toml
--rw-r--r--   0     1001      127     1553 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/CHANGELOG.md
--rw-r--r--   0     1001      127      903 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/Makefile
--rw-r--r--   0     1001      127       52 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/README.md
--rwxr-xr-x   0     1001      127      978 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/cov.sh
--rw-r--r--   0     1001      127     1642 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/audit.proto
--rw-r--r--   0     1001      127     1938 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/dataset.proto
--rw-r--r--   0     1001      127     4911 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/knowledgebox.proto
--rw-r--r--   0     1001      127      129 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/migrations.proto
--rw-r--r--   0     1001      127    10792 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/nodereader.proto
--rw-r--r--   0     1001      127     4554 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/noderesources.proto
--rw-r--r--   0     1001      127     2907 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/nodewriter.proto
--rw-r--r--   0     1001      127       13 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/.gitignore
--rw-r--r--   0     1001      127      106 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/MANIFEST.in
--rw-r--r--   0     1001      127       93 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/README.rst
--rw-r--r--   0     1001      127        0 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/__init__.py
--rw-r--r--   0     1001      127     5729 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/audit_pb2.py
--rw-r--r--   0     1001      127    11478 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi
--rw-r--r--   0     1001      127     5708 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py
--rw-r--r--   0     1001      127    14374 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi
--rw-r--r--   0     1001      127    14324 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py
--rw-r--r--   0     1001      127    33126 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi
--rw-r--r--   0     1001      127     1152 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py
--rw-r--r--   0     1001      127      844 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi
--rw-r--r--   0     1001      127    22792 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py
--rw-r--r--   0     1001      127    60294 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi
--rw-r--r--   0     1001      127    27532 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py
--rw-r--r--   0     1001      127    12923 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi
--rw-r--r--   0     1001      127    14299 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py
--rw-r--r--   0     1001      127    35337 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi
--rw-r--r--   0     1001      127     7995 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py
--rw-r--r--   0     1001      127    13432 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi
--rw-r--r--   0     1001      127    20793 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py
--rw-r--r--   0     1001      127     9143 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi
--rw-r--r--   0     1001      127        0 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/py.typed
--rw-r--r--   0     1001      127     5175 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2.py
--rw-r--r--   0     1001      127     9274 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi
--rw-r--r--   0     1001      127     6379 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py
--rw-r--r--   0     1001      127     3969 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi
--rw-r--r--   0     1001      127    35561 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/resources_pb2.py
--rw-r--r--   0     1001      127    95697 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi
--rw-r--r--   0     1001      127     2192 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py
--rw-r--r--   0     1001      127     2533 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi
--rw-r--r--   0     1001      127     4407 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py
--rw-r--r--   0     1001      127     2145 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi
--rw-r--r--   0     1001      127    13931 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2.py
--rw-r--r--   0     1001      127    28248 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi
--rw-r--r--   0     1001      127    13970 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py
--rw-r--r--   0     1001      127    11918 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi
--rw-r--r--   0     1001      127     6683 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/utils_pb2.py
--rw-r--r--   0     1001      127    18303 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi
--rw-r--r--   0     1001      127    32771 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2.py
--rw-r--r--   0     1001      127    78350 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi
--rw-r--r--   0     1001      127    39118 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py
--rw-r--r--   0     1001      127    20964 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi
--rw-r--r--   0     1001      127       96 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/setup.cfg
--rw-r--r--   0     1001      127      761 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/setup.py
--rw-r--r--   0     1001      127      708 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/reader.proto
--rw-r--r--   0     1001      127     1863 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/replication.proto
--rw-r--r--   0     1001      127    12098 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/resources.proto
--rw-r--r--   0     1001      127      558 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/standalone.proto
--rw-r--r--   0     1001      127     3469 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/train.proto
--rw-r--r--   0     1001      127     2301 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/utils.proto
--rw-r--r--   0     1001      127    12100 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/writer.proto
--rw-r--r--   0     1001      127     1461 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1621 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/src/update.rs
--rw-r--r--   0     1001      127    12085 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-05-29 12:14:52.000000 nucliadb_node_binding-4.0.1.post1382/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.1.post1382/PKG-INFO
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     3063 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     5462 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2944 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2023 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8450 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2557 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     5665 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    19055 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1496 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    11343 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13965 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2300 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12999 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3394 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2489 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      332 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1455 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8294 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11334 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    19577 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1553 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13111 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14260 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11563 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    15700 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11202 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/indexes.rs
+-rw-r--r--   0     1001      127    10055 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1168 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    28646 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    27248 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     7048 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/tests.rs
+-rw-r--r--   0     1001      127     1890 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10199 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8386 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     9372 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     2508 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
+-rw-r--r--   0     1001      127     6862 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5554 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0     1001      127     5337 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    43269 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    18906 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17039 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     7990 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9523 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22721 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10092 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3435 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2152 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3523 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127     4424 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/config.rs
+-rw-r--r--   0     1001      127    12340 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    29379 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11821 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    15068 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1741 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    11691 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2513 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127     8487 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2607 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    23029 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    25379 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     7189 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     2157 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127    10472 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2282 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127      940 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    18009 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15288 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     3267 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32.rs
+-rw-r--r--   0     1001      127     4415 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32_unaligned.rs
+-rw-r--r--   0     1001      127      903 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/vector_types/mod.rs
+-rw-r--r--   0     1001      127     3877 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/tests/test_basic_search.rs
+-rw-r--r--   0     1001      127     2895 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43324 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18147 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2340 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127     8473 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/audit.rs
+-rw-r--r--   0     1001      127    46848 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127    14122 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1271 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    95906 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    17860 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    62254 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    24308 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    50492 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127    10160 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/Cargo.toml
+-rw-r--r--   0     1001      127     1017 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/.cargo/config.toml
+-rw-r--r--   0     1001      127     1553 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/CHANGELOG.md
+-rw-r--r--   0     1001      127      903 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/Makefile
+-rw-r--r--   0     1001      127       52 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/README.md
+-rwxr-xr-x   0     1001      127      978 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/cov.sh
+-rw-r--r--   0     1001      127     1642 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/audit.proto
+-rw-r--r--   0     1001      127     1938 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/dataset.proto
+-rw-r--r--   0     1001      127     4911 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/knowledgebox.proto
+-rw-r--r--   0     1001      127      129 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/migrations.proto
+-rw-r--r--   0     1001      127    10792 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/nodereader.proto
+-rw-r--r--   0     1001      127     4554 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/noderesources.proto
+-rw-r--r--   0     1001      127     2907 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/nodewriter.proto
+-rw-r--r--   0     1001      127       13 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/.gitignore
+-rw-r--r--   0     1001      127      106 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/MANIFEST.in
+-rw-r--r--   0     1001      127       93 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/README.rst
+-rw-r--r--   0     1001      127        0 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/__init__.py
+-rw-r--r--   0     1001      127     5729 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/audit_pb2.py
+-rw-r--r--   0     1001      127    11478 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi
+-rw-r--r--   0     1001      127     5708 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py
+-rw-r--r--   0     1001      127    14374 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi
+-rw-r--r--   0     1001      127    14324 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py
+-rw-r--r--   0     1001      127    33126 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi
+-rw-r--r--   0     1001      127     1152 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py
+-rw-r--r--   0     1001      127      844 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi
+-rw-r--r--   0     1001      127    22792 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py
+-rw-r--r--   0     1001      127    60294 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi
+-rw-r--r--   0     1001      127    27532 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py
+-rw-r--r--   0     1001      127    12923 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    14299 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py
+-rw-r--r--   0     1001      127    35337 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi
+-rw-r--r--   0     1001      127     7995 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py
+-rw-r--r--   0     1001      127    13432 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi
+-rw-r--r--   0     1001      127    20793 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py
+-rw-r--r--   0     1001      127     9143 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi
+-rw-r--r--   0     1001      127        0 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/py.typed
+-rw-r--r--   0     1001      127     5175 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2.py
+-rw-r--r--   0     1001      127     9274 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi
+-rw-r--r--   0     1001      127     6379 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py
+-rw-r--r--   0     1001      127     3969 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    35561 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/resources_pb2.py
+-rw-r--r--   0     1001      127    95697 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi
+-rw-r--r--   0     1001      127     2192 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py
+-rw-r--r--   0     1001      127     2533 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi
+-rw-r--r--   0     1001      127     4407 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py
+-rw-r--r--   0     1001      127     2145 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi
+-rw-r--r--   0     1001      127    13931 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2.py
+-rw-r--r--   0     1001      127    28170 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi
+-rw-r--r--   0     1001      127    13970 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py
+-rw-r--r--   0     1001      127    11840 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi
+-rw-r--r--   0     1001      127     6683 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/utils_pb2.py
+-rw-r--r--   0     1001      127    18303 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi
+-rw-r--r--   0     1001      127    32378 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2.py
+-rw-r--r--   0     1001      127    77514 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi
+-rw-r--r--   0     1001      127    35989 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py
+-rw-r--r--   0     1001      127    19731 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi
+-rw-r--r--   0     1001      127       96 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/setup.cfg
+-rw-r--r--   0     1001      127      761 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/setup.py
+-rw-r--r--   0     1001      127      708 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/reader.proto
+-rw-r--r--   0     1001      127     1863 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/replication.proto
+-rw-r--r--   0     1001      127    12098 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/resources.proto
+-rw-r--r--   0     1001      127      558 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/standalone.proto
+-rw-r--r--   0     1001      127     3469 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/train.proto
+-rw-r--r--   0     1001      127     2301 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/utils.proto
+-rw-r--r--   0     1001      127    11929 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/writer.proto
+-rw-r--r--   0     1001      127     1461 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1621 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/src/update.rs
+-rw-r--r--   0     1001      127    12085 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-06-03 13:21:07.000000 nucliadb_node_binding-4.0.3.post1388/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-4.0.3.post1388/PKG-INFO
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/config.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/config.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32_unaligned.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/vector_types/dense_f32_unaligned.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/src/vector_types/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/src/vector_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/tests/test_basic_search.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/tests/test_basic_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -79,33 +79,33 @@
 
     #[measure(actor = "paragraphs", metric = "set_resource")]
     #[tracing::instrument(skip_all)]
     fn set_resource(&mut self, resource: &Resource) -> NodeResult<()> {
         let time = Instant::now();
         let id = Some(&resource.shard_id);
 
-        if resource.status != ResourceStatus::Delete as i32 {
-            let v = time.elapsed().as_millis();
-            debug!("{id:?} - Indexing paragraphs: starts at {v} ms");
-
-            let _ = self.index_paragraph(resource);
-            let v = time.elapsed().as_millis();
-            debug!("{id:?} - Indexing paragraphs: ends at {v} ms");
-        }
-
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Processing paragraphs to delete: starts at {v} ms");
 
         for paragraph_id in &resource.paragraphs_to_delete {
             let uuid_term = Term::from_field_text(self.schema.paragraph, paragraph_id);
             self.writer.delete_term(uuid_term);
         }
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Processing paragraphs to delete: ends at {v} ms");
 
+        if resource.status != ResourceStatus::Delete as i32 {
+            let v = time.elapsed().as_millis();
+            debug!("{id:?} - Indexing paragraphs: starts at {v} ms");
+
+            let _ = self.index_paragraph(resource);
+            let v = time.elapsed().as_millis();
+            debug!("{id:?} - Indexing paragraphs: ends at {v} ms");
+        }
+
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Commit: starts at {v} ms");
 
         self.writer.commit()?;
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Commit: ends at {v} ms");
 
@@ -454,8 +454,50 @@
         let (_top_docs, count) = searcher.search(&query, &(TopDocs::with_limit(2), Count))?;
         assert_eq!(count, 1);
 
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
         Ok(())
     }
+
+    #[test]
+    fn test_set_resource_replaces_documents() -> NodeResult<()> {
+        let dir = TempDir::new().unwrap();
+        let psc = ParagraphConfig {
+            path: dir.path().join("paragraphs"),
+        };
+
+        // Create a resource
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
+        let resource1 = create_resource("shard1".to_string());
+        paragraph_writer_service.set_resource(&resource1)?;
+
+        // Check that it exists
+        let reader = paragraph_writer_service.index.reader()?;
+        let searcher = reader.searcher();
+        let query = TermQuery::new(
+            Term::from_field_text(paragraph_writer_service.schema.text, "document"),
+            IndexRecordOption::Basic,
+        );
+        let (_top_docs, count) = searcher.search(&query, &(TopDocs::with_limit(2), Count))?;
+        assert_eq!(count, 1);
+
+        // Edit the resource
+        let mut resource_update = create_resource("shard1".to_string());
+        resource_update.paragraphs_to_delete =
+            resource_update.paragraphs.values().flat_map(|p| p.paragraphs.keys().cloned()).collect();
+        paragraph_writer_service.set_resource(&resource_update)?;
+
+        // Check that it is updated
+        let reader = paragraph_writer_service.index.reader()?;
+        let searcher = reader.searcher();
+        let query = TermQuery::new(
+            Term::from_field_text(paragraph_writer_service.schema.text, "document"),
+            IndexRecordOption::Basic,
+        );
+
+        let (_top_docs, count) = searcher.search(&query, &(TopDocs::with_limit(2), Count))?;
+        assert_eq!(count, 1);
+
+        Ok(())
+    }
 }
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/errors.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/indexes.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/indexes.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/tests.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/shards/versioning.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/shards/versioning.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_node/tests/test_vectorsets.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_node/tests/test_vectorsets.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files 6% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 })
             });
             (field_id, sentences_iterator)
         })
     }
 
     pub fn sentences_to_delete(&self) -> impl Iterator<Item = &str> {
-        self.resource.paragraphs_to_delete.iter().map(|paragraph_id| paragraph_id.as_str())
+        self.resource.sentences_to_delete.iter().map(String::as_str)
     }
 }
 
 pub struct ParagraphVectors<'a> {
     pub vectors: &'a HashMap<String, noderesources::VectorSentence>,
     pub labels: &'a Vec<String>,
 }
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/audit.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/audit.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files 8% similar despite different names*

```diff
@@ -346,87 +346,14 @@
     pub msgid: ::std::collections::HashMap<::prost::alloc::string::String, i64>,
 }
 #[allow(clippy::derive_partial_eq_without_eq)]
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct WriterStatusRequest {}
 #[allow(clippy::derive_partial_eq_without_eq)]
 #[derive(Clone, PartialEq, ::prost::Message)]
-pub struct SetLabelsRequest {
-    #[prost(message, optional, tag = "1")]
-    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
-    #[prost(string, tag = "2")]
-    pub id: ::prost::alloc::string::String,
-    #[prost(message, optional, tag = "3")]
-    pub labelset: ::core::option::Option<super::knowledgebox::LabelSet>,
-}
-#[allow(clippy::derive_partial_eq_without_eq)]
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct DelLabelsRequest {
-    #[prost(message, optional, tag = "1")]
-    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
-    #[prost(string, tag = "2")]
-    pub id: ::prost::alloc::string::String,
-}
-#[allow(clippy::derive_partial_eq_without_eq)]
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct GetLabelsResponse {
-    #[prost(message, optional, tag = "1")]
-    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
-    #[prost(message, optional, tag = "2")]
-    pub labels: ::core::option::Option<super::knowledgebox::Labels>,
-    #[prost(enumeration = "get_labels_response::Status", tag = "3")]
-    pub status: i32,
-}
-/// Nested message and enum types in `GetLabelsResponse`.
-pub mod get_labels_response {
-    #[derive(
-        Clone,
-        Copy,
-        Debug,
-        PartialEq,
-        Eq,
-        Hash,
-        PartialOrd,
-        Ord,
-        ::prost::Enumeration
-    )]
-    #[repr(i32)]
-    pub enum Status {
-        Ok = 0,
-        Notfound = 1,
-    }
-    impl Status {
-        /// String value of the enum field names used in the ProtoBuf definition.
-        ///
-        /// The values are not transformed in any way and thus are considered stable
-        /// (if the ProtoBuf definition does not change) and safe for programmatic use.
-        pub fn as_str_name(&self) -> &'static str {
-            match self {
-                Status::Ok => "OK",
-                Status::Notfound => "NOTFOUND",
-            }
-        }
-        /// Creates an enum from field names used in the ProtoBuf definition.
-        pub fn from_str_name(value: &str) -> ::core::option::Option<Self> {
-            match value {
-                "OK" => Some(Self::Ok),
-                "NOTFOUND" => Some(Self::Notfound),
-                _ => None,
-            }
-        }
-    }
-}
-#[allow(clippy::derive_partial_eq_without_eq)]
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct GetLabelsRequest {
-    #[prost(message, optional, tag = "1")]
-    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
-}
-#[allow(clippy::derive_partial_eq_without_eq)]
-#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct NewEntitiesGroupRequest {
     #[prost(message, optional, tag = "1")]
     pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
     #[prost(string, tag = "2")]
     pub group: ::prost::alloc::string::String,
     #[prost(message, optional, tag = "3")]
     pub entities: ::core::option::Option<super::knowledgebox::EntitiesGroup>,
@@ -717,32 +644,24 @@
         pub group: ::prost::alloc::string::String,
         #[prost(string, tag = "2")]
         pub entity: ::prost::alloc::string::String,
     }
 }
 #[allow(clippy::derive_partial_eq_without_eq)]
 #[derive(Clone, PartialEq, ::prost::Message)]
-pub struct GetLabelSetRequest {
-    #[prost(message, optional, tag = "1")]
-    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
-    #[prost(string, tag = "2")]
-    pub labelset: ::prost::alloc::string::String,
-}
-#[allow(clippy::derive_partial_eq_without_eq)]
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct GetLabelSetResponse {
+pub struct GetLabelsResponse {
     #[prost(message, optional, tag = "1")]
     pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
     #[prost(message, optional, tag = "2")]
-    pub labelset: ::core::option::Option<super::knowledgebox::LabelSet>,
-    #[prost(enumeration = "get_label_set_response::Status", tag = "3")]
+    pub labels: ::core::option::Option<super::knowledgebox::Labels>,
+    #[prost(enumeration = "get_labels_response::Status", tag = "3")]
     pub status: i32,
 }
-/// Nested message and enum types in `GetLabelSetResponse`.
-pub mod get_label_set_response {
+/// Nested message and enum types in `GetLabelsResponse`.
+pub mod get_labels_response {
     #[derive(
         Clone,
         Copy,
         Debug,
         PartialEq,
         Eq,
         Hash,
@@ -774,14 +693,20 @@
                 _ => None,
             }
         }
     }
 }
 #[allow(clippy::derive_partial_eq_without_eq)]
 #[derive(Clone, PartialEq, ::prost::Message)]
+pub struct GetLabelsRequest {
+    #[prost(message, optional, tag = "1")]
+    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
+}
+#[allow(clippy::derive_partial_eq_without_eq)]
+#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct GetEntitiesGroupRequest {
     #[prost(message, optional, tag = "1")]
     pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
     #[prost(string, tag = "2")]
     pub group: ::prost::alloc::string::String,
 }
 #[allow(clippy::derive_partial_eq_without_eq)]
@@ -895,32 +820,14 @@
                 _ => None,
             }
         }
     }
 }
 #[allow(clippy::derive_partial_eq_without_eq)]
 #[derive(Clone, PartialEq, ::prost::Message)]
-pub struct DelVectorSetRequest {
-    #[prost(message, optional, tag = "1")]
-    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
-    #[prost(string, tag = "2")]
-    pub vectorset: ::prost::alloc::string::String,
-}
-#[allow(clippy::derive_partial_eq_without_eq)]
-#[derive(Clone, PartialEq, ::prost::Message)]
-pub struct SetVectorSetRequest {
-    #[prost(message, optional, tag = "1")]
-    pub kb: ::core::option::Option<super::knowledgebox::KnowledgeBoxId>,
-    #[prost(string, tag = "2")]
-    pub id: ::prost::alloc::string::String,
-    #[prost(message, optional, tag = "3")]
-    pub vectorset: ::core::option::Option<super::knowledgebox::VectorSet>,
-}
-#[allow(clippy::derive_partial_eq_without_eq)]
-#[derive(Clone, PartialEq, ::prost::Message)]
 pub struct OpStatusWriter {
     #[prost(enumeration = "op_status_writer::Status", tag = "1")]
     pub status: i32,
 }
 /// Nested message and enum types in `OpStatusWriter`.
 pub mod op_status_writer {
     #[derive(
@@ -1295,14 +1202,136 @@
 pub struct FileUploaded {}
 #[allow(clippy::derive_partial_eq_without_eq)]
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct SynonymsRequest {
     #[prost(string, tag = "1")]
     pub kbid: ::prost::alloc::string::String,
 }
+#[allow(clippy::derive_partial_eq_without_eq)]
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct NewVectorSetRequest {
+    #[prost(string, tag = "1")]
+    pub kbid: ::prost::alloc::string::String,
+    #[prost(string, tag = "2")]
+    pub vectorset_id: ::prost::alloc::string::String,
+    #[prost(enumeration = "super::nodewriter::VectorType", tag = "3")]
+    pub vector_type: i32,
+    #[prost(enumeration = "super::utils::VectorSimilarity", tag = "4")]
+    pub similarity: i32,
+    #[prost(uint32, tag = "5")]
+    pub vector_dimension: u32,
+    #[prost(bool, tag = "6")]
+    pub normalize_vectors: bool,
+    #[prost(uint32, repeated, tag = "7")]
+    pub matryoshka_dimensions: ::prost::alloc::vec::Vec<u32>,
+}
+#[allow(clippy::derive_partial_eq_without_eq)]
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct NewVectorSetResponse {
+    #[prost(enumeration = "new_vector_set_response::Status", tag = "1")]
+    pub status: i32,
+    #[prost(string, tag = "2")]
+    pub details: ::prost::alloc::string::String,
+}
+/// Nested message and enum types in `NewVectorSetResponse`.
+pub mod new_vector_set_response {
+    #[derive(
+        Clone,
+        Copy,
+        Debug,
+        PartialEq,
+        Eq,
+        Hash,
+        PartialOrd,
+        Ord,
+        ::prost::Enumeration
+    )]
+    #[repr(i32)]
+    pub enum Status {
+        Ok = 0,
+        /// generic error
+        Error = 1,
+    }
+    impl Status {
+        /// String value of the enum field names used in the ProtoBuf definition.
+        ///
+        /// The values are not transformed in any way and thus are considered stable
+        /// (if the ProtoBuf definition does not change) and safe for programmatic use.
+        pub fn as_str_name(&self) -> &'static str {
+            match self {
+                Status::Ok => "OK",
+                Status::Error => "ERROR",
+            }
+        }
+        /// Creates an enum from field names used in the ProtoBuf definition.
+        pub fn from_str_name(value: &str) -> ::core::option::Option<Self> {
+            match value {
+                "OK" => Some(Self::Ok),
+                "ERROR" => Some(Self::Error),
+                _ => None,
+            }
+        }
+    }
+}
+#[allow(clippy::derive_partial_eq_without_eq)]
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct DelVectorSetRequest {
+    #[prost(string, tag = "1")]
+    pub kbid: ::prost::alloc::string::String,
+    #[prost(string, tag = "2")]
+    pub vectorset_id: ::prost::alloc::string::String,
+}
+#[allow(clippy::derive_partial_eq_without_eq)]
+#[derive(Clone, PartialEq, ::prost::Message)]
+pub struct DelVectorSetResponse {
+    #[prost(enumeration = "del_vector_set_response::Status", tag = "1")]
+    pub status: i32,
+    #[prost(string, tag = "2")]
+    pub details: ::prost::alloc::string::String,
+}
+/// Nested message and enum types in `DelVectorSetResponse`.
+pub mod del_vector_set_response {
+    #[derive(
+        Clone,
+        Copy,
+        Debug,
+        PartialEq,
+        Eq,
+        Hash,
+        PartialOrd,
+        Ord,
+        ::prost::Enumeration
+    )]
+    #[repr(i32)]
+    pub enum Status {
+        Ok = 0,
+        /// generic error
+        Error = 1,
+    }
+    impl Status {
+        /// String value of the enum field names used in the ProtoBuf definition.
+        ///
+        /// The values are not transformed in any way and thus are considered stable
+        /// (if the ProtoBuf definition does not change) and safe for programmatic use.
+        pub fn as_str_name(&self) -> &'static str {
+            match self {
+                Status::Ok => "OK",
+                Status::Error => "ERROR",
+            }
+        }
+        /// Creates an enum from field names used in the ProtoBuf definition.
+        pub fn from_str_name(value: &str) -> ::core::option::Option<Self> {
+            match value {
+                "OK" => Some(Self::Ok),
+                "ERROR" => Some(Self::Error),
+                _ => None,
+            }
+        }
+    }
+}
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Hash, PartialOrd, Ord, ::prost::Enumeration)]
 #[repr(i32)]
 pub enum NotificationSource {
     Unset = 0,
     Writer = 1,
     Processor = 2,
 }
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-4.0.3.post1388/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/Cargo.toml` & `nucliadb_node_binding-4.0.3.post1388/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "4.0.1-post1382"
+version = "4.0.3-post1388"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/.cargo/config.toml` & `nucliadb_node_binding-4.0.3.post1388/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/CHANGELOG.md` & `nucliadb_node_binding-4.0.3.post1388/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/Makefile` & `nucliadb_node_binding-4.0.3.post1388/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/cov.sh` & `nucliadb_node_binding-4.0.3.post1388/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/audit.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/audit.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/dataset.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/dataset.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/knowledgebox.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/knowledgebox.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/nodereader.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/nodereader.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/noderesources.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/noderesources.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/nodewriter.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/nodewriter.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/audit_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/audit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/knowledgebox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/migrations_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/migrations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodereader_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/noderesources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/nodewriter_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/replication_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/resources_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/standalone_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -121,46 +121,44 @@
 from nucliadb_protos.writer_pb2 import (
     Audit as Audit,
     BinaryData as BinaryData,
     BinaryMetadata as BinaryMetadata,
     BrokerMessage as BrokerMessage,
     BrokerMessageBlobReference as BrokerMessageBlobReference,
     DelEntitiesRequest as DelEntitiesRequest,
-    DelLabelsRequest as DelLabelsRequest,
     DelVectorSetRequest as DelVectorSetRequest,
+    DelVectorSetResponse as DelVectorSetResponse,
     Error as Error,
     FileRequest as FileRequest,
     FileUploaded as FileUploaded,
     GetEntitiesGroupRequest as GetEntitiesGroupRequest,
     GetEntitiesGroupResponse as GetEntitiesGroupResponse,
     GetEntitiesRequest as GetEntitiesRequest,
     GetEntitiesResponse as GetEntitiesResponse,
-    GetLabelSetRequest as GetLabelSetRequest,
-    GetLabelSetResponse as GetLabelSetResponse,
     GetLabelsRequest as GetLabelsRequest,
     GetLabelsResponse as GetLabelsResponse,
     GetVectorSetsRequest as GetVectorSetsRequest,
     GetVectorSetsResponse as GetVectorSetsResponse,
     IndexResource as IndexResource,
     IndexStatus as IndexStatus,
     ListEntitiesGroupsRequest as ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse as ListEntitiesGroupsResponse,
     ListMembersRequest as ListMembersRequest,
     ListMembersResponse as ListMembersResponse,
     Member as Member,
     MergeEntitiesRequest as MergeEntitiesRequest,
     NewEntitiesGroupRequest as NewEntitiesGroupRequest,
     NewEntitiesGroupResponse as NewEntitiesGroupResponse,
+    NewVectorSetRequest as NewVectorSetRequest,
+    NewVectorSetResponse as NewVectorSetResponse,
     Notification as Notification,
     NotificationSource as NotificationSource,
     OpStatusWriter as OpStatusWriter,
     PROCESSOR as PROCESSOR,
     SetEntitiesRequest as SetEntitiesRequest,
-    SetLabelsRequest as SetLabelsRequest,
-    SetVectorSetRequest as SetVectorSetRequest,
     SetVectorsRequest as SetVectorsRequest,
     SetVectorsResponse as SetVectorsResponse,
     ShardObject as ShardObject,
     ShardReplica as ShardReplica,
     Shards as Shards,
     SynonymsRequest as SynonymsRequest,
     UNSET as UNSET,
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/train_pb2_grpc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -119,46 +119,44 @@
 from nucliadb_protos.writer_pb2 import (
     Audit as Audit,
     BinaryData as BinaryData,
     BinaryMetadata as BinaryMetadata,
     BrokerMessage as BrokerMessage,
     BrokerMessageBlobReference as BrokerMessageBlobReference,
     DelEntitiesRequest as DelEntitiesRequest,
-    DelLabelsRequest as DelLabelsRequest,
     DelVectorSetRequest as DelVectorSetRequest,
+    DelVectorSetResponse as DelVectorSetResponse,
     Error as Error,
     FileRequest as FileRequest,
     FileUploaded as FileUploaded,
     GetEntitiesGroupRequest as GetEntitiesGroupRequest,
     GetEntitiesGroupResponse as GetEntitiesGroupResponse,
     GetEntitiesRequest as GetEntitiesRequest,
     GetEntitiesResponse as GetEntitiesResponse,
-    GetLabelSetRequest as GetLabelSetRequest,
-    GetLabelSetResponse as GetLabelSetResponse,
     GetLabelsRequest as GetLabelsRequest,
     GetLabelsResponse as GetLabelsResponse,
     GetVectorSetsRequest as GetVectorSetsRequest,
     GetVectorSetsResponse as GetVectorSetsResponse,
     IndexResource as IndexResource,
     IndexStatus as IndexStatus,
     ListEntitiesGroupsRequest as ListEntitiesGroupsRequest,
     ListEntitiesGroupsResponse as ListEntitiesGroupsResponse,
     ListMembersRequest as ListMembersRequest,
     ListMembersResponse as ListMembersResponse,
     Member as Member,
     MergeEntitiesRequest as MergeEntitiesRequest,
     NewEntitiesGroupRequest as NewEntitiesGroupRequest,
     NewEntitiesGroupResponse as NewEntitiesGroupResponse,
+    NewVectorSetRequest as NewVectorSetRequest,
+    NewVectorSetResponse as NewVectorSetResponse,
     Notification as Notification,
     NotificationSource as NotificationSource,
     OpStatusWriter as OpStatusWriter,
     PROCESSOR as PROCESSOR,
     SetEntitiesRequest as SetEntitiesRequest,
-    SetLabelsRequest as SetLabelsRequest,
-    SetVectorSetRequest as SetVectorSetRequest,
     SetVectorsRequest as SetVectorsRequest,
     SetVectorsResponse as SetVectorsResponse,
     ShardObject as ShardObject,
     ShardReplica as ShardReplica,
     Shards as Shards,
     SynonymsRequest as SynonymsRequest,
     UNSET as UNSET,
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/utils_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/utils_pb2.pyi`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from nucliadb_protos import audit_pb2 as nucliadb__protos_dot_audit__pb2
 
 from nucliadb_protos.noderesources_pb2 import *
 from nucliadb_protos.resources_pb2 import *
 from nucliadb_protos.knowledgebox_pb2 import *
 from nucliadb_protos.audit_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnucliadb_protos/writer.proto\x12\tfdbwriter\x1a\x1fgoogle/protobuf/timestamp.proto\x1a#nucliadb_protos/noderesources.proto\x1a\x1fnucliadb_protos/resources.proto\x1a\"nucliadb_protos/knowledgebox.proto\x1a\x1bnucliadb_protos/audit.proto\"\xd9\x02\n\x05\x41udit\x12\x0c\n\x04user\x18\x01 \x01(\t\x12(\n\x04when\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x03 \x01(\t\x12\'\n\x06source\x18\x04 \x01(\x0e\x32\x17.fdbwriter.Audit.Source\x12\x0c\n\x04kbid\x18\x05 \x01(\t\x12\x0c\n\x04uuid\x18\x06 \x01(\t\x12>\n\x0emessage_source\x18\x07 \x01(\x0e\x32&.fdbwriter.BrokerMessage.MessageSource\x12*\n\x0e\x66ield_metadata\x18\x08 \x03(\x0b\x32\x12.resources.FieldID\x12\'\n\x0c\x61udit_fields\x18\t \x03(\x0b\x32\x11.audit.AuditField\".\n\x06Source\x12\x08\n\x04HTTP\x10\x00\x12\r\n\tDASHBOARD\x10\x01\x12\x0b\n\x07\x44\x45SKTOP\x10\x02\"\xad\x01\n\x05\x45rror\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12(\n\nfield_type\x18\x02 \x01(\x0e\x32\x14.resources.FieldType\x12\r\n\x05\x65rror\x18\x03 \x01(\t\x12(\n\x04\x63ode\x18\x04 \x01(\x0e\x32\x1a.fdbwriter.Error.ErrorCode\"2\n\tErrorCode\x12\x0b\n\x07GENERIC\x10\x00\x12\x0b\n\x07\x45XTRACT\x10\x01\x12\x0b\n\x07PROCESS\x10\x02\"\x97\x11\n\rBrokerMessage\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04slug\x18\x04 \x01(\t\x12\x1f\n\x05\x61udit\x18\x05 \x01(\x0b\x32\x10.fdbwriter.Audit\x12\x32\n\x04type\x18\x06 \x01(\x0e\x32$.fdbwriter.BrokerMessage.MessageType\x12\x0f\n\x07multiid\x18\x07 \x01(\t\x12\x1f\n\x05\x62\x61sic\x18\x08 \x01(\x0b\x32\x10.resources.Basic\x12!\n\x06origin\x18\t \x01(\x0b\x32\x11.resources.Origin\x12\"\n\trelations\x18\n \x03(\x0b\x32\x0f.utils.Relation\x12\x42\n\rconversations\x18\x0b \x03(\x0b\x32+.fdbwriter.BrokerMessage.ConversationsEntry\x12\x36\n\x07layouts\x18\x0c \x03(\x0b\x32%.fdbwriter.BrokerMessage.LayoutsEntry\x12\x32\n\x05texts\x18\r \x03(\x0b\x32#.fdbwriter.BrokerMessage.TextsEntry\x12>\n\x0bkeywordsets\x18\x0e \x03(\x0b\x32).fdbwriter.BrokerMessage.KeywordsetsEntry\x12:\n\tdatetimes\x18\x0f \x03(\x0b\x32\'.fdbwriter.BrokerMessage.DatetimesEntry\x12\x32\n\x05links\x18\x10 \x03(\x0b\x32#.fdbwriter.BrokerMessage.LinksEntry\x12\x32\n\x05\x66iles\x18\x11 \x03(\x0b\x32#.fdbwriter.BrokerMessage.FilesEntry\x12\x39\n\x13link_extracted_data\x18\x12 \x03(\x0b\x32\x1c.resources.LinkExtractedData\x12\x39\n\x13\x66ile_extracted_data\x18\x13 \x03(\x0b\x32\x1c.resources.FileExtractedData\x12\x37\n\x0e\x65xtracted_text\x18\x14 \x03(\x0b\x32\x1f.resources.ExtractedTextWrapper\x12?\n\x0e\x66ield_metadata\x18\x15 \x03(\x0b\x32\'.resources.FieldComputedMetadataWrapper\x12\x39\n\rfield_vectors\x18\x16 \x03(\x0b\x32\".resources.ExtractedVectorsWrapper\x12\x45\n\x14\x66ield_large_metadata\x18\x17 \x03(\x0b\x32\'.resources.LargeComputedMetadataWrapper\x12)\n\rdelete_fields\x18\x18 \x03(\x0b\x32\x12.resources.FieldID\x12\x12\n\norigin_seq\x18\x19 \x01(\x05\x12\x1c\n\x14slow_processing_time\x18\x1a \x01(\x02\x12\x1b\n\x13pre_processing_time\x18\x1c \x01(\x02\x12-\n\tdone_time\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07txseqid\x18\x1e \x01(\x03\x42\x02\x18\x01\x12 \n\x06\x65rrors\x18\x1f \x03(\x0b\x32\x10.fdbwriter.Error\x12\x15\n\rprocessing_id\x18  \x01(\t\x12\x36\n\x06source\x18! \x01(\x0e\x32&.fdbwriter.BrokerMessage.MessageSource\x12\x13\n\x0b\x61\x63\x63ount_seq\x18\" \x01(\x03\x12\x33\n\x0cuser_vectors\x18# \x03(\x0b\x32\x1d.resources.UserVectorsWrapper\x12\x0f\n\x07reindex\x18$ \x01(\x08\x12\x1f\n\x05\x65xtra\x18% \x01(\x0b\x32\x10.resources.Extra\x12?\n\x10question_answers\x18& \x03(\x0b\x32%.resources.FieldQuestionAnswerWrapper\x12!\n\x08security\x18\' \x01(\x0b\x32\x0f.utils.Security\x1aM\n\x12\x43onversationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.resources.Conversation:\x02\x38\x01\x1a\x46\n\x0cLayoutsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.resources.FieldLayout:\x02\x38\x01\x1a\x42\n\nTextsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.resources.FieldText:\x02\x38\x01\x1aN\n\x10KeywordsetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.resources.FieldKeywordset:\x02\x38\x01\x1aJ\n\x0e\x44\x61tetimesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.resources.FieldDatetime:\x02\x38\x01\x1a\x42\n\nLinksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.resources.FieldLink:\x02\x38\x01\x1a\x42\n\nFilesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.resources.FieldFile:\x02\x38\x01\"N\n\x0bMessageType\x12\x0e\n\nAUTOCOMMIT\x10\x00\x12\t\n\x05MULTI\x10\x01\x12\n\n\x06\x43OMMIT\x10\x02\x12\x0c\n\x08ROLLBACK\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\"*\n\rMessageSource\x12\n\n\x06WRITER\x10\x00\x12\r\n\tPROCESSOR\x10\x01\"M\n\x1a\x42rokerMessageBlobReference\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x13\n\x0bstorage_key\x18\x03 \x01(\t\"\x97\x01\n\x14WriterStatusResponse\x12\x16\n\x0eknowledgeboxes\x18\x01 \x03(\t\x12\x39\n\x05msgid\x18\x02 \x03(\x0b\x32*.fdbwriter.WriterStatusResponse.MsgidEntry\x1a,\n\nMsgidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"\x15\n\x13WriterStatusRequest\"r\n\x10SetLabelsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\n\n\x02id\x18\x02 \x01(\t\x12(\n\x08labelset\x18\x03 \x01(\x0b\x32\x16.knowledgebox.LabelSet\"H\n\x10\x44\x65lLabelsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\n\n\x02id\x18\x02 \x01(\t\"\xb8\x01\n\x11GetLabelsResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12$\n\x06labels\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Labels\x12\x33\n\x06status\x18\x03 \x01(\x0e\x32#.fdbwriter.GetLabelsResponse.Status\"\x1e\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\"<\n\x10GetLabelsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"\x81\x01\n\x17NewEntitiesGroupRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\x12-\n\x08\x65ntities\x18\x03 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup\"\x99\x01\n\x18NewEntitiesGroupResponse\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.fdbwriter.NewEntitiesGroupResponse.Status\"A\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x10\n\x0cKB_NOT_FOUND\x10\x02\x12\x12\n\x0e\x41LREADY_EXISTS\x10\x03\"|\n\x12SetEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\x12-\n\x08\x65ntities\x18\x03 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup\"\x8a\x03\n\x1aUpdateEntitiesGroupRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\x12;\n\x03\x61\x64\x64\x18\x03 \x03(\x0b\x32..fdbwriter.UpdateEntitiesGroupRequest.AddEntry\x12\x41\n\x06update\x18\x04 \x03(\x0b\x32\x31.fdbwriter.UpdateEntitiesGroupRequest.UpdateEntry\x12\x0e\n\x06\x64\x65lete\x18\x05 \x03(\t\x12\r\n\x05title\x18\x06 \x01(\t\x12\r\n\x05\x63olor\x18\x07 \x01(\t\x1a@\n\x08\x41\x64\x64\x45ntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Entity:\x02\x38\x01\x1a\x43\n\x0bUpdateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Entity:\x02\x38\x01\"\xa9\x01\n\x1bUpdateEntitiesGroupResponse\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.fdbwriter.UpdateEntitiesGroupResponse.Status\"K\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x10\n\x0cKB_NOT_FOUND\x10\x02\x12\x1c\n\x18\x45NTITIES_GROUP_NOT_FOUND\x10\x03\"E\n\x19ListEntitiesGroupsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"\x9b\x02\n\x1aListEntitiesGroupsResponse\x12\x41\n\x06groups\x18\x01 \x03(\x0b\x32\x31.fdbwriter.ListEntitiesGroupsResponse.GroupsEntry\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.fdbwriter.ListEntitiesGroupsResponse.Status\x1aQ\n\x0bGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".knowledgebox.EntitiesGroupSummary:\x02\x38\x01\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\x12\t\n\x05\x45RROR\x10\x02\">\n\x12GetEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"\xa9\x02\n\x13GetEntitiesResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12:\n\x06groups\x18\x02 \x03(\x0b\x32*.fdbwriter.GetEntitiesResponse.GroupsEntry\x12\x35\n\x06status\x18\x03 \x01(\x0e\x32%.fdbwriter.GetEntitiesResponse.Status\x1aJ\n\x0bGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup:\x02\x38\x01\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"M\n\x12\x44\x65lEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\"\xd9\x01\n\x14MergeEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\x36\n\x04\x66rom\x18\x02 \x01(\x0b\x32(.fdbwriter.MergeEntitiesRequest.EntityID\x12\x34\n\x02to\x18\x03 \x01(\x0b\x32(.fdbwriter.MergeEntitiesRequest.EntityID\x1a)\n\x08\x45ntityID\x12\r\n\x05group\x18\x01 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x02 \x01(\t\"P\n\x12GetLabelSetRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\x10\n\x08labelset\x18\x02 \x01(\t\"\xc0\x01\n\x13GetLabelSetResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12(\n\x08labelset\x18\x02 \x01(\x0b\x32\x16.knowledgebox.LabelSet\x12\x35\n\x06status\x18\x03 \x01(\x0e\x32%.fdbwriter.GetLabelSetResponse.Status\"\x1e\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\"R\n\x17GetEntitiesGroupRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\"\xf9\x01\n\x18GetEntitiesGroupResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12*\n\x05group\x18\x02 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup\x12:\n\x06status\x18\x03 \x01(\x0e\x32*.fdbwriter.GetEntitiesGroupResponse.Status\"K\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x10\n\x0cKB_NOT_FOUND\x10\x01\x12\x1c\n\x18\x45NTITIES_GROUP_NOT_FOUND\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"@\n\x14GetVectorSetsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"\xd3\x01\n\x15GetVectorSetsResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12,\n\nvectorsets\x18\x02 \x01(\x0b\x32\x18.knowledgebox.VectorSets\x12\x37\n\x06status\x18\x03 \x01(\x0e\x32\'.fdbwriter.GetVectorSetsResponse.Status\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"R\n\x13\x44\x65lVectorSetRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\x11\n\tvectorset\x18\x02 \x01(\t\"w\n\x13SetVectorSetRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\n\n\x02id\x18\x02 \x01(\t\x12*\n\tvectorset\x18\x03 \x01(\x0b\x32\x17.knowledgebox.VectorSet\"m\n\x0eOpStatusWriter\x12\x30\n\x06status\x18\x01 \x01(\x0e\x32 .fdbwriter.OpStatusWriter.Status\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x0c\n\x08NOTFOUND\x10\x02\"\xd2\x03\n\x0cNotification\x12\x11\n\tpartition\x18\x01 \x01(\x05\x12\r\n\x05multi\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04kbid\x18\x04 \x01(\t\x12\r\n\x05seqid\x18\x05 \x01(\x03\x12.\n\x06\x61\x63tion\x18\x06 \x01(\x0e\x32\x1e.fdbwriter.Notification.Action\x12\x35\n\nwrite_type\x18\x07 \x01(\x0e\x32!.fdbwriter.Notification.WriteType\x12-\n\x07message\x18\x08 \x01(\x0b\x32\x18.fdbwriter.BrokerMessageB\x02\x18\x01\x12-\n\x06source\x18\t \x01(\x0e\x32\x1d.fdbwriter.NotificationSource\x12\x19\n\x11processing_errors\x18\n \x01(\x08\x12\'\n\rmessage_audit\x18\x0b \x01(\x0b\x32\x10.fdbwriter.Audit\",\n\x06\x41\x63tion\x12\n\n\x06\x43OMMIT\x10\x00\x12\t\n\x05\x41\x42ORT\x10\x01\x12\x0b\n\x07INDEXED\x10\x02\">\n\tWriteType\x12\t\n\x05UNSET\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0c\n\x08MODIFIED\x10\x02\x12\x0b\n\x07\x44\x45LETED\x10\x03\"\xff\x01\n\x06Member\x12\n\n\x02id\x18\x01 \x01(\t\x12\x16\n\x0elisten_address\x18\x02 \x01(\t\x12\x13\n\x07is_self\x18\x03 \x01(\x08\x42\x02\x18\x01\x12(\n\x04type\x18\x04 \x01(\x0e\x32\x16.fdbwriter.Member.TypeB\x02\x18\x01\x12\x11\n\x05\x64ummy\x18\x05 \x01(\x08\x42\x02\x18\x01\x12\x16\n\nload_score\x18\x06 \x01(\x02\x42\x02\x18\x01\x12\x13\n\x0bshard_count\x18\x07 \x01(\r\x12\x12\n\nprimary_id\x18\x08 \x01(\t\">\n\x04Type\x12\x06\n\x02IO\x10\x00\x12\n\n\x06SEARCH\x10\x01\x12\n\n\x06INGEST\x10\x02\x12\t\n\x05TRAIN\x10\x03\x12\x0b\n\x07UNKNOWN\x10\x04\"\x14\n\x12ListMembersRequest\"9\n\x13ListMembersResponse\x12\"\n\x07members\x18\x01 \x03(\x0b\x32\x11.fdbwriter.Member\"H\n\x0cShardReplica\x12*\n\x05shard\x18\x01 \x01(\x0b\x32\x1b.noderesources.ShardCreated\x12\x0c\n\x04node\x18\x02 \x01(\t\"\x8d\x01\n\x0bShardObject\x12\r\n\x05shard\x18\x01 \x01(\t\x12)\n\x08replicas\x18\x03 \x03(\x0b\x32\x17.fdbwriter.ShardReplica\x12\x31\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x11\n\tread_only\x18\x05 \x01(\x08\"\xc2\x02\n\x06Shards\x12&\n\x06shards\x18\x01 \x03(\x0b\x32\x16.fdbwriter.ShardObject\x12\x0c\n\x04kbid\x18\x02 \x01(\t\x12\x12\n\x06\x61\x63tual\x18\x03 \x01(\x05\x42\x02\x18\x01\x12/\n\nsimilarity\x18\x04 \x01(\x0e\x32\x17.utils.VectorSimilarityB\x02\x18\x01\x12\x32\n\x05model\x18\x05 \x01(\x0b\x32#.knowledgebox.SemanticModelMetadata\x12.\n\x0frelease_channel\x18\x06 \x01(\x0e\x32\x15.utils.ReleaseChannel\x12+\n\x05\x65xtra\x18\x07 \x03(\x0b\x32\x1c.fdbwriter.Shards.ExtraEntry\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"C\n\rIndexResource\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x0b\n\x03rid\x18\x02 \x01(\t\x12\x17\n\x0freindex_vectors\x18\x03 \x01(\x08\"\r\n\x0bIndexStatus\"w\n\x11SetVectorsRequest\x12$\n\x07vectors\x18\x01 \x01(\x0b\x32\x13.utils.VectorObject\x12\x0c\n\x04kbid\x18\x02 \x01(\t\x12\x0b\n\x03rid\x18\x03 \x01(\t\x12!\n\x05\x66ield\x18\x04 \x01(\x0b\x32\x12.resources.FieldID\"#\n\x12SetVectorsResponse\x12\r\n\x05\x66ound\x18\x01 \x01(\x08\"*\n\x0b\x46ileRequest\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\"\x1a\n\nBinaryData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"a\n\x0e\x42inaryMetadata\x12\x0c\n\x04kbid\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x05 \x01(\t\x12\x14\n\x0c\x63ontent_type\x18\x06 \x01(\t\"k\n\x10UploadBinaryData\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x19.fdbwriter.BinaryMetadataH\x00\x12\x11\n\x07payload\x18\x03 \x01(\x0cH\x00\x42\x06\n\x04\x64\x61ta\"\x0e\n\x0c\x46ileUploaded\"\x1f\n\x0fSynonymsRequest\x12\x0c\n\x04kbid\x18\x01 \x01(\t*:\n\x12NotificationSource\x12\t\n\x05UNSET\x10\x00\x12\n\n\x06WRITER\x10\x01\x12\r\n\tPROCESSOR\x10\x02\x32\xd2\x0e\n\x06Writer\x12Y\n\x0fNewKnowledgeBox\x12\x1d.knowledgebox.KnowledgeBoxNew\x1a%.knowledgebox.NewKnowledgeBoxResponse\"\x00\x12^\n\x12\x44\x65leteKnowledgeBox\x12\x1c.knowledgebox.KnowledgeBoxID\x1a(.knowledgebox.DeleteKnowledgeBoxResponse\"\x00\x12\x62\n\x12UpdateKnowledgeBox\x12 .knowledgebox.KnowledgeBoxUpdate\x1a(.knowledgebox.UpdateKnowledgeBoxResponse\"\x00\x12V\n\x0eGCKnowledgeBox\x12\x1c.knowledgebox.KnowledgeBoxID\x1a$.knowledgebox.GCKnowledgeBoxResponse\"\x00\x12K\n\nSetVectors\x12\x1c.fdbwriter.SetVectorsRequest\x1a\x1d.fdbwriter.SetVectorsResponse\"\x00\x12I\n\x0eProcessMessage\x12\x18.fdbwriter.BrokerMessage\x1a\x19.fdbwriter.OpStatusWriter\"\x00(\x01\x12H\n\tGetLabels\x12\x1b.fdbwriter.GetLabelsRequest\x1a\x1c.fdbwriter.GetLabelsResponse\"\x00\x12N\n\x0bGetLabelSet\x12\x1d.fdbwriter.GetLabelSetRequest\x1a\x1e.fdbwriter.GetLabelSetResponse\"\x00\x12\x45\n\tSetLabels\x12\x1b.fdbwriter.SetLabelsRequest\x1a\x19.fdbwriter.OpStatusWriter\"\x00\x12\x45\n\tDelLabels\x12\x1b.fdbwriter.DelLabelsRequest\x1a\x19.fdbwriter.OpStatusWriter\"\x00\x12]\n\x10NewEntitiesGroup\x12\".fdbwriter.NewEntitiesGroupRequest\x1a#.fdbwriter.NewEntitiesGroupResponse\"\x00\x12N\n\x0bGetEntities\x12\x1d.fdbwriter.GetEntitiesRequest\x1a\x1e.fdbwriter.GetEntitiesResponse\"\x00\x12]\n\x10GetEntitiesGroup\x12\".fdbwriter.GetEntitiesGroupRequest\x1a#.fdbwriter.GetEntitiesGroupResponse\"\x00\x12\x63\n\x12ListEntitiesGroups\x12$.fdbwriter.ListEntitiesGroupsRequest\x1a%.fdbwriter.ListEntitiesGroupsResponse\"\x00\x12I\n\x0bSetEntities\x12\x1d.fdbwriter.SetEntitiesRequest\x1a\x19.fdbwriter.OpStatusWriter\"\x00\x12\x66\n\x13UpdateEntitiesGroup\x12%.fdbwriter.UpdateEntitiesGroupRequest\x1a&.fdbwriter.UpdateEntitiesGroupResponse\"\x00\x12I\n\x0b\x44\x65lEntities\x12\x1d.fdbwriter.DelEntitiesRequest\x1a\x19.fdbwriter.OpStatusWriter\"\x00\x12K\n\x06Status\x12\x1e.fdbwriter.WriterStatusRequest\x1a\x1f.fdbwriter.WriterStatusResponse\"\x00\x12L\n\x0bListMembers\x12\x1d.fdbwriter.ListMembersRequest\x1a\x1e.fdbwriter.ListMembersResponse\x12;\n\x05Index\x12\x18.fdbwriter.IndexResource\x1a\x16.fdbwriter.IndexStatus\"\x00\x12=\n\x07ReIndex\x12\x18.fdbwriter.IndexResource\x1a\x16.fdbwriter.IndexStatus\"\x00\x12\x41\n\x0c\x44ownloadFile\x12\x16.fdbwriter.FileRequest\x1a\x15.fdbwriter.BinaryData\"\x00\x30\x01\x12\x46\n\nUploadFile\x12\x1b.fdbwriter.UploadBinaryData\x1a\x17.fdbwriter.FileUploaded\"\x00(\x01P\x01P\x02P\x03P\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cnucliadb_protos/writer.proto\x12\tfdbwriter\x1a\x1fgoogle/protobuf/timestamp.proto\x1a#nucliadb_protos/noderesources.proto\x1a\x1fnucliadb_protos/resources.proto\x1a\"nucliadb_protos/knowledgebox.proto\x1a\x1bnucliadb_protos/audit.proto\"\xd9\x02\n\x05\x41udit\x12\x0c\n\x04user\x18\x01 \x01(\t\x12(\n\x04when\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x03 \x01(\t\x12\'\n\x06source\x18\x04 \x01(\x0e\x32\x17.fdbwriter.Audit.Source\x12\x0c\n\x04kbid\x18\x05 \x01(\t\x12\x0c\n\x04uuid\x18\x06 \x01(\t\x12>\n\x0emessage_source\x18\x07 \x01(\x0e\x32&.fdbwriter.BrokerMessage.MessageSource\x12*\n\x0e\x66ield_metadata\x18\x08 \x03(\x0b\x32\x12.resources.FieldID\x12\'\n\x0c\x61udit_fields\x18\t \x03(\x0b\x32\x11.audit.AuditField\".\n\x06Source\x12\x08\n\x04HTTP\x10\x00\x12\r\n\tDASHBOARD\x10\x01\x12\x0b\n\x07\x44\x45SKTOP\x10\x02\"\xad\x01\n\x05\x45rror\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12(\n\nfield_type\x18\x02 \x01(\x0e\x32\x14.resources.FieldType\x12\r\n\x05\x65rror\x18\x03 \x01(\t\x12(\n\x04\x63ode\x18\x04 \x01(\x0e\x32\x1a.fdbwriter.Error.ErrorCode\"2\n\tErrorCode\x12\x0b\n\x07GENERIC\x10\x00\x12\x0b\n\x07\x45XTRACT\x10\x01\x12\x0b\n\x07PROCESS\x10\x02\"\x97\x11\n\rBrokerMessage\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04slug\x18\x04 \x01(\t\x12\x1f\n\x05\x61udit\x18\x05 \x01(\x0b\x32\x10.fdbwriter.Audit\x12\x32\n\x04type\x18\x06 \x01(\x0e\x32$.fdbwriter.BrokerMessage.MessageType\x12\x0f\n\x07multiid\x18\x07 \x01(\t\x12\x1f\n\x05\x62\x61sic\x18\x08 \x01(\x0b\x32\x10.resources.Basic\x12!\n\x06origin\x18\t \x01(\x0b\x32\x11.resources.Origin\x12\"\n\trelations\x18\n \x03(\x0b\x32\x0f.utils.Relation\x12\x42\n\rconversations\x18\x0b \x03(\x0b\x32+.fdbwriter.BrokerMessage.ConversationsEntry\x12\x36\n\x07layouts\x18\x0c \x03(\x0b\x32%.fdbwriter.BrokerMessage.LayoutsEntry\x12\x32\n\x05texts\x18\r \x03(\x0b\x32#.fdbwriter.BrokerMessage.TextsEntry\x12>\n\x0bkeywordsets\x18\x0e \x03(\x0b\x32).fdbwriter.BrokerMessage.KeywordsetsEntry\x12:\n\tdatetimes\x18\x0f \x03(\x0b\x32\'.fdbwriter.BrokerMessage.DatetimesEntry\x12\x32\n\x05links\x18\x10 \x03(\x0b\x32#.fdbwriter.BrokerMessage.LinksEntry\x12\x32\n\x05\x66iles\x18\x11 \x03(\x0b\x32#.fdbwriter.BrokerMessage.FilesEntry\x12\x39\n\x13link_extracted_data\x18\x12 \x03(\x0b\x32\x1c.resources.LinkExtractedData\x12\x39\n\x13\x66ile_extracted_data\x18\x13 \x03(\x0b\x32\x1c.resources.FileExtractedData\x12\x37\n\x0e\x65xtracted_text\x18\x14 \x03(\x0b\x32\x1f.resources.ExtractedTextWrapper\x12?\n\x0e\x66ield_metadata\x18\x15 \x03(\x0b\x32\'.resources.FieldComputedMetadataWrapper\x12\x39\n\rfield_vectors\x18\x16 \x03(\x0b\x32\".resources.ExtractedVectorsWrapper\x12\x45\n\x14\x66ield_large_metadata\x18\x17 \x03(\x0b\x32\'.resources.LargeComputedMetadataWrapper\x12)\n\rdelete_fields\x18\x18 \x03(\x0b\x32\x12.resources.FieldID\x12\x12\n\norigin_seq\x18\x19 \x01(\x05\x12\x1c\n\x14slow_processing_time\x18\x1a \x01(\x02\x12\x1b\n\x13pre_processing_time\x18\x1c \x01(\x02\x12-\n\tdone_time\x18\x1d \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x07txseqid\x18\x1e \x01(\x03\x42\x02\x18\x01\x12 \n\x06\x65rrors\x18\x1f \x03(\x0b\x32\x10.fdbwriter.Error\x12\x15\n\rprocessing_id\x18  \x01(\t\x12\x36\n\x06source\x18! \x01(\x0e\x32&.fdbwriter.BrokerMessage.MessageSource\x12\x13\n\x0b\x61\x63\x63ount_seq\x18\" \x01(\x03\x12\x33\n\x0cuser_vectors\x18# \x03(\x0b\x32\x1d.resources.UserVectorsWrapper\x12\x0f\n\x07reindex\x18$ \x01(\x08\x12\x1f\n\x05\x65xtra\x18% \x01(\x0b\x32\x10.resources.Extra\x12?\n\x10question_answers\x18& \x03(\x0b\x32%.resources.FieldQuestionAnswerWrapper\x12!\n\x08security\x18\' \x01(\x0b\x32\x0f.utils.Security\x1aM\n\x12\x43onversationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.resources.Conversation:\x02\x38\x01\x1a\x46\n\x0cLayoutsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.resources.FieldLayout:\x02\x38\x01\x1a\x42\n\nTextsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.resources.FieldText:\x02\x38\x01\x1aN\n\x10KeywordsetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.resources.FieldKeywordset:\x02\x38\x01\x1aJ\n\x0e\x44\x61tetimesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.resources.FieldDatetime:\x02\x38\x01\x1a\x42\n\nLinksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.resources.FieldLink:\x02\x38\x01\x1a\x42\n\nFilesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.resources.FieldFile:\x02\x38\x01\"N\n\x0bMessageType\x12\x0e\n\nAUTOCOMMIT\x10\x00\x12\t\n\x05MULTI\x10\x01\x12\n\n\x06\x43OMMIT\x10\x02\x12\x0c\n\x08ROLLBACK\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\"*\n\rMessageSource\x12\n\n\x06WRITER\x10\x00\x12\r\n\tPROCESSOR\x10\x01\"M\n\x1a\x42rokerMessageBlobReference\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x13\n\x0bstorage_key\x18\x03 \x01(\t\"\x97\x01\n\x14WriterStatusResponse\x12\x16\n\x0eknowledgeboxes\x18\x01 \x03(\t\x12\x39\n\x05msgid\x18\x02 \x03(\x0b\x32*.fdbwriter.WriterStatusResponse.MsgidEntry\x1a,\n\nMsgidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"\x15\n\x13WriterStatusRequest\"\x81\x01\n\x17NewEntitiesGroupRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\x12-\n\x08\x65ntities\x18\x03 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup\"\x99\x01\n\x18NewEntitiesGroupResponse\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.fdbwriter.NewEntitiesGroupResponse.Status\"A\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x10\n\x0cKB_NOT_FOUND\x10\x02\x12\x12\n\x0e\x41LREADY_EXISTS\x10\x03\"|\n\x12SetEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\x12-\n\x08\x65ntities\x18\x03 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup\"\x8a\x03\n\x1aUpdateEntitiesGroupRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\x12;\n\x03\x61\x64\x64\x18\x03 \x03(\x0b\x32..fdbwriter.UpdateEntitiesGroupRequest.AddEntry\x12\x41\n\x06update\x18\x04 \x03(\x0b\x32\x31.fdbwriter.UpdateEntitiesGroupRequest.UpdateEntry\x12\x0e\n\x06\x64\x65lete\x18\x05 \x03(\t\x12\r\n\x05title\x18\x06 \x01(\t\x12\r\n\x05\x63olor\x18\x07 \x01(\t\x1a@\n\x08\x41\x64\x64\x45ntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Entity:\x02\x38\x01\x1a\x43\n\x0bUpdateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Entity:\x02\x38\x01\"\xa9\x01\n\x1bUpdateEntitiesGroupResponse\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.fdbwriter.UpdateEntitiesGroupResponse.Status\"K\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x10\n\x0cKB_NOT_FOUND\x10\x02\x12\x1c\n\x18\x45NTITIES_GROUP_NOT_FOUND\x10\x03\"E\n\x19ListEntitiesGroupsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"\x9b\x02\n\x1aListEntitiesGroupsResponse\x12\x41\n\x06groups\x18\x01 \x03(\x0b\x32\x31.fdbwriter.ListEntitiesGroupsResponse.GroupsEntry\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.fdbwriter.ListEntitiesGroupsResponse.Status\x1aQ\n\x0bGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".knowledgebox.EntitiesGroupSummary:\x02\x38\x01\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\x12\t\n\x05\x45RROR\x10\x02\">\n\x12GetEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"\xa9\x02\n\x13GetEntitiesResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12:\n\x06groups\x18\x02 \x03(\x0b\x32*.fdbwriter.GetEntitiesResponse.GroupsEntry\x12\x35\n\x06status\x18\x03 \x01(\x0e\x32%.fdbwriter.GetEntitiesResponse.Status\x1aJ\n\x0bGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup:\x02\x38\x01\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"M\n\x12\x44\x65lEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\"\xd9\x01\n\x14MergeEntitiesRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\x36\n\x04\x66rom\x18\x02 \x01(\x0b\x32(.fdbwriter.MergeEntitiesRequest.EntityID\x12\x34\n\x02to\x18\x03 \x01(\x0b\x32(.fdbwriter.MergeEntitiesRequest.EntityID\x1a)\n\x08\x45ntityID\x12\r\n\x05group\x18\x01 \x01(\t\x12\x0e\n\x06\x65ntity\x18\x02 \x01(\t\"\xb8\x01\n\x11GetLabelsResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12$\n\x06labels\x18\x02 \x01(\x0b\x32\x14.knowledgebox.Labels\x12\x33\n\x06status\x18\x03 \x01(\x0e\x32#.fdbwriter.GetLabelsResponse.Status\"\x1e\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\"<\n\x10GetLabelsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"R\n\x17GetEntitiesGroupRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12\r\n\x05group\x18\x02 \x01(\t\"\xf9\x01\n\x18GetEntitiesGroupResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12*\n\x05group\x18\x02 \x01(\x0b\x32\x1b.knowledgebox.EntitiesGroup\x12:\n\x06status\x18\x03 \x01(\x0e\x32*.fdbwriter.GetEntitiesGroupResponse.Status\"K\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x10\n\x0cKB_NOT_FOUND\x10\x01\x12\x1c\n\x18\x45NTITIES_GROUP_NOT_FOUND\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"@\n\x14GetVectorSetsRequest\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\"\xd3\x01\n\x15GetVectorSetsResponse\x12(\n\x02kb\x18\x01 \x01(\x0b\x32\x1c.knowledgebox.KnowledgeBoxID\x12,\n\nvectorsets\x18\x02 \x01(\x0b\x32\x18.knowledgebox.VectorSets\x12\x37\n\x06status\x18\x03 \x01(\x0e\x32\'.fdbwriter.GetVectorSetsResponse.Status\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\x0c\n\x08NOTFOUND\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"m\n\x0eOpStatusWriter\x12\x30\n\x06status\x18\x01 \x01(\x0e\x32 .fdbwriter.OpStatusWriter.Status\")\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\x12\x0c\n\x08NOTFOUND\x10\x02\"\xd2\x03\n\x0cNotification\x12\x11\n\tpartition\x18\x01 \x01(\x05\x12\r\n\x05multi\x18\x02 \x01(\t\x12\x0c\n\x04uuid\x18\x03 \x01(\t\x12\x0c\n\x04kbid\x18\x04 \x01(\t\x12\r\n\x05seqid\x18\x05 \x01(\x03\x12.\n\x06\x61\x63tion\x18\x06 \x01(\x0e\x32\x1e.fdbwriter.Notification.Action\x12\x35\n\nwrite_type\x18\x07 \x01(\x0e\x32!.fdbwriter.Notification.WriteType\x12-\n\x07message\x18\x08 \x01(\x0b\x32\x18.fdbwriter.BrokerMessageB\x02\x18\x01\x12-\n\x06source\x18\t \x01(\x0e\x32\x1d.fdbwriter.NotificationSource\x12\x19\n\x11processing_errors\x18\n \x01(\x08\x12\'\n\rmessage_audit\x18\x0b \x01(\x0b\x32\x10.fdbwriter.Audit\",\n\x06\x41\x63tion\x12\n\n\x06\x43OMMIT\x10\x00\x12\t\n\x05\x41\x42ORT\x10\x01\x12\x0b\n\x07INDEXED\x10\x02\">\n\tWriteType\x12\t\n\x05UNSET\x10\x00\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0c\n\x08MODIFIED\x10\x02\x12\x0b\n\x07\x44\x45LETED\x10\x03\"\xff\x01\n\x06Member\x12\n\n\x02id\x18\x01 \x01(\t\x12\x16\n\x0elisten_address\x18\x02 \x01(\t\x12\x13\n\x07is_self\x18\x03 \x01(\x08\x42\x02\x18\x01\x12(\n\x04type\x18\x04 \x01(\x0e\x32\x16.fdbwriter.Member.TypeB\x02\x18\x01\x12\x11\n\x05\x64ummy\x18\x05 \x01(\x08\x42\x02\x18\x01\x12\x16\n\nload_score\x18\x06 \x01(\x02\x42\x02\x18\x01\x12\x13\n\x0bshard_count\x18\x07 \x01(\r\x12\x12\n\nprimary_id\x18\x08 \x01(\t\">\n\x04Type\x12\x06\n\x02IO\x10\x00\x12\n\n\x06SEARCH\x10\x01\x12\n\n\x06INGEST\x10\x02\x12\t\n\x05TRAIN\x10\x03\x12\x0b\n\x07UNKNOWN\x10\x04\"\x14\n\x12ListMembersRequest\"9\n\x13ListMembersResponse\x12\"\n\x07members\x18\x01 \x03(\x0b\x32\x11.fdbwriter.Member\"H\n\x0cShardReplica\x12*\n\x05shard\x18\x01 \x01(\x0b\x32\x1b.noderesources.ShardCreated\x12\x0c\n\x04node\x18\x02 \x01(\t\"\x8d\x01\n\x0bShardObject\x12\r\n\x05shard\x18\x01 \x01(\t\x12)\n\x08replicas\x18\x03 \x03(\x0b\x32\x17.fdbwriter.ShardReplica\x12\x31\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x11\n\tread_only\x18\x05 \x01(\x08\"\xc2\x02\n\x06Shards\x12&\n\x06shards\x18\x01 \x03(\x0b\x32\x16.fdbwriter.ShardObject\x12\x0c\n\x04kbid\x18\x02 \x01(\t\x12\x12\n\x06\x61\x63tual\x18\x03 \x01(\x05\x42\x02\x18\x01\x12/\n\nsimilarity\x18\x04 \x01(\x0e\x32\x17.utils.VectorSimilarityB\x02\x18\x01\x12\x32\n\x05model\x18\x05 \x01(\x0b\x32#.knowledgebox.SemanticModelMetadata\x12.\n\x0frelease_channel\x18\x06 \x01(\x0e\x32\x15.utils.ReleaseChannel\x12+\n\x05\x65xtra\x18\x07 \x03(\x0b\x32\x1c.fdbwriter.Shards.ExtraEntry\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"C\n\rIndexResource\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x0b\n\x03rid\x18\x02 \x01(\t\x12\x17\n\x0freindex_vectors\x18\x03 \x01(\x08\"\r\n\x0bIndexStatus\"w\n\x11SetVectorsRequest\x12$\n\x07vectors\x18\x01 \x01(\x0b\x32\x13.utils.VectorObject\x12\x0c\n\x04kbid\x18\x02 \x01(\t\x12\x0b\n\x03rid\x18\x03 \x01(\t\x12!\n\x05\x66ield\x18\x04 \x01(\x0b\x32\x12.resources.FieldID\"#\n\x12SetVectorsResponse\x12\r\n\x05\x66ound\x18\x01 \x01(\x08\"*\n\x0b\x46ileRequest\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\"\x1a\n\nBinaryData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"a\n\x0e\x42inaryMetadata\x12\x0c\n\x04kbid\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x05 \x01(\t\x12\x14\n\x0c\x63ontent_type\x18\x06 \x01(\t\"k\n\x10UploadBinaryData\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x19.fdbwriter.BinaryMetadataH\x00\x12\x11\n\x07payload\x18\x03 \x01(\x0cH\x00\x42\x06\n\x04\x64\x61ta\"\x0e\n\x0c\x46ileUploaded\"\x1f\n\x0fSynonymsRequest\x12\x0c\n\x04kbid\x18\x01 \x01(\t\"\xe7\x01\n\x13NewVectorSetRequest\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x14\n\x0cvectorset_id\x18\x02 \x01(\t\x12+\n\x0bvector_type\x18\x03 \x01(\x0e\x32\x16.nodewriter.VectorType\x12+\n\nsimilarity\x18\x04 \x01(\x0e\x32\x17.utils.VectorSimilarity\x12\x18\n\x10vector_dimension\x18\x05 \x01(\r\x12\x19\n\x11normalize_vectors\x18\x06 \x01(\x08\x12\x1d\n\x15matryoshka_dimensions\x18\x07 \x03(\r\"|\n\x14NewVectorSetResponse\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.fdbwriter.NewVectorSetResponse.Status\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"9\n\x13\x44\x65lVectorSetRequest\x12\x0c\n\x04kbid\x18\x01 \x01(\t\x12\x14\n\x0cvectorset_id\x18\x02 \x01(\t\"|\n\x14\x44\x65lVectorSetResponse\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.fdbwriter.DelVectorSetResponse.Status\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\t\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01*:\n\x12NotificationSource\x12\t\n\x05UNSET\x10\x00\x12\n\n\x06WRITER\x10\x01\x12\r\n\tPROCESSOR\x10\x02\x32\xd0\r\n\x06Writer\x12Y\n\x0fNewKnowledgeBox\x12\x1d.knowledgebox.KnowledgeBoxNew\x1a%.knowledgebox.NewKnowledgeBoxResponse\"\x00\x12^\n\x12\x44\x65leteKnowledgeBox\x12\x1c.knowledgebox.KnowledgeBoxID\x1a(.knowledgebox.DeleteKnowledgeBoxResponse\"\x00\x12\x62\n\x12UpdateKnowledgeBox\x12 .knowledgebox.KnowledgeBoxUpdate\x1a(.knowledgebox.UpdateKnowledgeBoxResponse\"\x00\x12V\n\x0eGCKnowledgeBox\x12\x1c.knowledgebox.KnowledgeBoxID\x1a$.knowledgebox.GCKnowledgeBoxResponse\"\x00\x12K\n\nSetVectors\x12\x1c.fdbwriter.SetVectorsRequest\x1a\x1d.fdbwriter.SetVectorsResponse\"\x00\x12I\n\x0eProcessMessage\x12\x18.fdbwriter.BrokerMessage\x1a\x19.fdbwriter.OpStatusWriter\"\x00(\x01\x12]\n\x10NewEntitiesGroup\x12\".fdbwriter.NewEntitiesGroupRequest\x1a#.fdbwriter.NewEntitiesGroupResponse\"\x00\x12N\n\x0bGetEntities\x12\x1d.fdbwriter.GetEntitiesRequest\x1a\x1e.fdbwriter.GetEntitiesResponse\"\x00\x12]\n\x10GetEntitiesGroup\x12\".fdbwriter.GetEntitiesGroupRequest\x1a#.fdbwriter.GetEntitiesGroupResponse\"\x00\x12\x63\n\x12ListEntitiesGroups\x12$.fdbwriter.ListEntitiesGroupsRequest\x1a%.fdbwriter.ListEntitiesGroupsResponse\"\x00\x12I\n\x0bSetEntities\x12\x1d.fdbwriter.SetEntitiesRequest\x1a\x19.fdbwriter.OpStatusWriter\"\x00\x12\x66\n\x13UpdateEntitiesGroup\x12%.fdbwriter.UpdateEntitiesGroupRequest\x1a&.fdbwriter.UpdateEntitiesGroupResponse\"\x00\x12I\n\x0b\x44\x65lEntities\x12\x1d.fdbwriter.DelEntitiesRequest\x1a\x19.fdbwriter.OpStatusWriter\"\x00\x12K\n\x06Status\x12\x1e.fdbwriter.WriterStatusRequest\x1a\x1f.fdbwriter.WriterStatusResponse\"\x00\x12L\n\x0bListMembers\x12\x1d.fdbwriter.ListMembersRequest\x1a\x1e.fdbwriter.ListMembersResponse\x12;\n\x05Index\x12\x18.fdbwriter.IndexResource\x1a\x16.fdbwriter.IndexStatus\"\x00\x12=\n\x07ReIndex\x12\x18.fdbwriter.IndexResource\x1a\x16.fdbwriter.IndexStatus\"\x00\x12\x41\n\x0c\x44ownloadFile\x12\x16.fdbwriter.FileRequest\x1a\x15.fdbwriter.BinaryData\"\x00\x30\x01\x12\x46\n\nUploadFile\x12\x1b.fdbwriter.UploadBinaryData\x1a\x17.fdbwriter.FileUploaded\"\x00(\x01\x12Q\n\x0cNewVectorSet\x12\x1e.fdbwriter.NewVectorSetRequest\x1a\x1f.fdbwriter.NewVectorSetResponse\"\x00\x12Q\n\x0c\x44\x65lVectorSet\x12\x1e.fdbwriter.DelVectorSetRequest\x1a\x1f.fdbwriter.DelVectorSetResponse\"\x00P\x01P\x02P\x03P\x04\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'nucliadb_protos.writer_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_BROKERMESSAGE_CONVERSATIONSENTRY']._options = None
@@ -94,16 +94,16 @@
   _globals['_SHARDOBJECT'].fields_by_name['timestamp']._serialized_options = b'\030\001'
   _globals['_SHARDS_EXTRAENTRY']._options = None
   _globals['_SHARDS_EXTRAENTRY']._serialized_options = b'8\001'
   _globals['_SHARDS'].fields_by_name['actual']._options = None
   _globals['_SHARDS'].fields_by_name['actual']._serialized_options = b'\030\001'
   _globals['_SHARDS'].fields_by_name['similarity']._options = None
   _globals['_SHARDS'].fields_by_name['similarity']._serialized_options = b'\030\001'
-  _globals['_NOTIFICATIONSOURCE']._serialized_start=8766
-  _globals['_NOTIFICATIONSOURCE']._serialized_end=8824
+  _globals['_NOTIFICATIONSOURCE']._serialized_start=8639
+  _globals['_NOTIFICATIONSOURCE']._serialized_end=8697
   _globals['_AUDIT']._serialized_start=212
   _globals['_AUDIT']._serialized_end=557
   _globals['_AUDIT_SOURCE']._serialized_start=511
   _globals['_AUDIT_SOURCE']._serialized_end=557
   _globals['_ERROR']._serialized_start=560
   _globals['_ERROR']._serialized_end=733
   _globals['_ERROR_ERRORCODE']._serialized_start=683
@@ -132,128 +132,126 @@
   _globals['_BROKERMESSAGEBLOBREFERENCE']._serialized_end=3014
   _globals['_WRITERSTATUSRESPONSE']._serialized_start=3017
   _globals['_WRITERSTATUSRESPONSE']._serialized_end=3168
   _globals['_WRITERSTATUSRESPONSE_MSGIDENTRY']._serialized_start=3124
   _globals['_WRITERSTATUSRESPONSE_MSGIDENTRY']._serialized_end=3168
   _globals['_WRITERSTATUSREQUEST']._serialized_start=3170
   _globals['_WRITERSTATUSREQUEST']._serialized_end=3191
-  _globals['_SETLABELSREQUEST']._serialized_start=3193
-  _globals['_SETLABELSREQUEST']._serialized_end=3307
-  _globals['_DELLABELSREQUEST']._serialized_start=3309
-  _globals['_DELLABELSREQUEST']._serialized_end=3381
-  _globals['_GETLABELSRESPONSE']._serialized_start=3384
-  _globals['_GETLABELSRESPONSE']._serialized_end=3568
-  _globals['_GETLABELSRESPONSE_STATUS']._serialized_start=3538
-  _globals['_GETLABELSRESPONSE_STATUS']._serialized_end=3568
-  _globals['_GETLABELSREQUEST']._serialized_start=3570
-  _globals['_GETLABELSREQUEST']._serialized_end=3630
-  _globals['_NEWENTITIESGROUPREQUEST']._serialized_start=3633
-  _globals['_NEWENTITIESGROUPREQUEST']._serialized_end=3762
-  _globals['_NEWENTITIESGROUPRESPONSE']._serialized_start=3765
-  _globals['_NEWENTITIESGROUPRESPONSE']._serialized_end=3918
-  _globals['_NEWENTITIESGROUPRESPONSE_STATUS']._serialized_start=3853
-  _globals['_NEWENTITIESGROUPRESPONSE_STATUS']._serialized_end=3918
-  _globals['_SETENTITIESREQUEST']._serialized_start=3920
-  _globals['_SETENTITIESREQUEST']._serialized_end=4044
-  _globals['_UPDATEENTITIESGROUPREQUEST']._serialized_start=4047
-  _globals['_UPDATEENTITIESGROUPREQUEST']._serialized_end=4441
-  _globals['_UPDATEENTITIESGROUPREQUEST_ADDENTRY']._serialized_start=4308
-  _globals['_UPDATEENTITIESGROUPREQUEST_ADDENTRY']._serialized_end=4372
-  _globals['_UPDATEENTITIESGROUPREQUEST_UPDATEENTRY']._serialized_start=4374
-  _globals['_UPDATEENTITIESGROUPREQUEST_UPDATEENTRY']._serialized_end=4441
-  _globals['_UPDATEENTITIESGROUPRESPONSE']._serialized_start=4444
-  _globals['_UPDATEENTITIESGROUPRESPONSE']._serialized_end=4613
-  _globals['_UPDATEENTITIESGROUPRESPONSE_STATUS']._serialized_start=4538
-  _globals['_UPDATEENTITIESGROUPRESPONSE_STATUS']._serialized_end=4613
-  _globals['_LISTENTITIESGROUPSREQUEST']._serialized_start=4615
-  _globals['_LISTENTITIESGROUPSREQUEST']._serialized_end=4684
-  _globals['_LISTENTITIESGROUPSRESPONSE']._serialized_start=4687
-  _globals['_LISTENTITIESGROUPSRESPONSE']._serialized_end=4970
-  _globals['_LISTENTITIESGROUPSRESPONSE_GROUPSENTRY']._serialized_start=4846
-  _globals['_LISTENTITIESGROUPSRESPONSE_GROUPSENTRY']._serialized_end=4927
-  _globals['_LISTENTITIESGROUPSRESPONSE_STATUS']._serialized_start=4929
-  _globals['_LISTENTITIESGROUPSRESPONSE_STATUS']._serialized_end=4970
-  _globals['_GETENTITIESREQUEST']._serialized_start=4972
-  _globals['_GETENTITIESREQUEST']._serialized_end=5034
-  _globals['_GETENTITIESRESPONSE']._serialized_start=5037
-  _globals['_GETENTITIESRESPONSE']._serialized_end=5334
-  _globals['_GETENTITIESRESPONSE_GROUPSENTRY']._serialized_start=5217
-  _globals['_GETENTITIESRESPONSE_GROUPSENTRY']._serialized_end=5291
-  _globals['_GETENTITIESRESPONSE_STATUS']._serialized_start=4929
-  _globals['_GETENTITIESRESPONSE_STATUS']._serialized_end=4970
-  _globals['_DELENTITIESREQUEST']._serialized_start=5336
-  _globals['_DELENTITIESREQUEST']._serialized_end=5413
-  _globals['_MERGEENTITIESREQUEST']._serialized_start=5416
-  _globals['_MERGEENTITIESREQUEST']._serialized_end=5633
-  _globals['_MERGEENTITIESREQUEST_ENTITYID']._serialized_start=5592
-  _globals['_MERGEENTITIESREQUEST_ENTITYID']._serialized_end=5633
-  _globals['_GETLABELSETREQUEST']._serialized_start=5635
-  _globals['_GETLABELSETREQUEST']._serialized_end=5715
-  _globals['_GETLABELSETRESPONSE']._serialized_start=5718
-  _globals['_GETLABELSETRESPONSE']._serialized_end=5910
-  _globals['_GETLABELSETRESPONSE_STATUS']._serialized_start=3538
-  _globals['_GETLABELSETRESPONSE_STATUS']._serialized_end=3568
-  _globals['_GETENTITIESGROUPREQUEST']._serialized_start=5912
-  _globals['_GETENTITIESGROUPREQUEST']._serialized_end=5994
-  _globals['_GETENTITIESGROUPRESPONSE']._serialized_start=5997
-  _globals['_GETENTITIESGROUPRESPONSE']._serialized_end=6246
-  _globals['_GETENTITIESGROUPRESPONSE_STATUS']._serialized_start=6171
-  _globals['_GETENTITIESGROUPRESPONSE_STATUS']._serialized_end=6246
-  _globals['_GETVECTORSETSREQUEST']._serialized_start=6248
-  _globals['_GETVECTORSETSREQUEST']._serialized_end=6312
-  _globals['_GETVECTORSETSRESPONSE']._serialized_start=6315
-  _globals['_GETVECTORSETSRESPONSE']._serialized_end=6526
-  _globals['_GETVECTORSETSRESPONSE_STATUS']._serialized_start=4929
-  _globals['_GETVECTORSETSRESPONSE_STATUS']._serialized_end=4970
-  _globals['_DELVECTORSETREQUEST']._serialized_start=6528
-  _globals['_DELVECTORSETREQUEST']._serialized_end=6610
-  _globals['_SETVECTORSETREQUEST']._serialized_start=6612
-  _globals['_SETVECTORSETREQUEST']._serialized_end=6731
-  _globals['_OPSTATUSWRITER']._serialized_start=6733
-  _globals['_OPSTATUSWRITER']._serialized_end=6842
-  _globals['_OPSTATUSWRITER_STATUS']._serialized_start=6801
-  _globals['_OPSTATUSWRITER_STATUS']._serialized_end=6842
-  _globals['_NOTIFICATION']._serialized_start=6845
-  _globals['_NOTIFICATION']._serialized_end=7311
-  _globals['_NOTIFICATION_ACTION']._serialized_start=7203
-  _globals['_NOTIFICATION_ACTION']._serialized_end=7247
-  _globals['_NOTIFICATION_WRITETYPE']._serialized_start=7249
-  _globals['_NOTIFICATION_WRITETYPE']._serialized_end=7311
-  _globals['_MEMBER']._serialized_start=7314
-  _globals['_MEMBER']._serialized_end=7569
-  _globals['_MEMBER_TYPE']._serialized_start=7507
-  _globals['_MEMBER_TYPE']._serialized_end=7569
-  _globals['_LISTMEMBERSREQUEST']._serialized_start=7571
-  _globals['_LISTMEMBERSREQUEST']._serialized_end=7591
-  _globals['_LISTMEMBERSRESPONSE']._serialized_start=7593
-  _globals['_LISTMEMBERSRESPONSE']._serialized_end=7650
-  _globals['_SHARDREPLICA']._serialized_start=7652
-  _globals['_SHARDREPLICA']._serialized_end=7724
-  _globals['_SHARDOBJECT']._serialized_start=7727
-  _globals['_SHARDOBJECT']._serialized_end=7868
-  _globals['_SHARDS']._serialized_start=7871
-  _globals['_SHARDS']._serialized_end=8193
-  _globals['_SHARDS_EXTRAENTRY']._serialized_start=8149
-  _globals['_SHARDS_EXTRAENTRY']._serialized_end=8193
-  _globals['_INDEXRESOURCE']._serialized_start=8195
-  _globals['_INDEXRESOURCE']._serialized_end=8262
-  _globals['_INDEXSTATUS']._serialized_start=8264
-  _globals['_INDEXSTATUS']._serialized_end=8277
-  _globals['_SETVECTORSREQUEST']._serialized_start=8279
-  _globals['_SETVECTORSREQUEST']._serialized_end=8398
-  _globals['_SETVECTORSRESPONSE']._serialized_start=8400
-  _globals['_SETVECTORSRESPONSE']._serialized_end=8435
-  _globals['_FILEREQUEST']._serialized_start=8437
-  _globals['_FILEREQUEST']._serialized_end=8479
-  _globals['_BINARYDATA']._serialized_start=8481
-  _globals['_BINARYDATA']._serialized_end=8507
-  _globals['_BINARYMETADATA']._serialized_start=8509
-  _globals['_BINARYMETADATA']._serialized_end=8606
-  _globals['_UPLOADBINARYDATA']._serialized_start=8608
-  _globals['_UPLOADBINARYDATA']._serialized_end=8715
-  _globals['_FILEUPLOADED']._serialized_start=8717
-  _globals['_FILEUPLOADED']._serialized_end=8731
-  _globals['_SYNONYMSREQUEST']._serialized_start=8733
-  _globals['_SYNONYMSREQUEST']._serialized_end=8764
-  _globals['_WRITER']._serialized_start=8827
-  _globals['_WRITER']._serialized_end=10701
+  _globals['_NEWENTITIESGROUPREQUEST']._serialized_start=3194
+  _globals['_NEWENTITIESGROUPREQUEST']._serialized_end=3323
+  _globals['_NEWENTITIESGROUPRESPONSE']._serialized_start=3326
+  _globals['_NEWENTITIESGROUPRESPONSE']._serialized_end=3479
+  _globals['_NEWENTITIESGROUPRESPONSE_STATUS']._serialized_start=3414
+  _globals['_NEWENTITIESGROUPRESPONSE_STATUS']._serialized_end=3479
+  _globals['_SETENTITIESREQUEST']._serialized_start=3481
+  _globals['_SETENTITIESREQUEST']._serialized_end=3605
+  _globals['_UPDATEENTITIESGROUPREQUEST']._serialized_start=3608
+  _globals['_UPDATEENTITIESGROUPREQUEST']._serialized_end=4002
+  _globals['_UPDATEENTITIESGROUPREQUEST_ADDENTRY']._serialized_start=3869
+  _globals['_UPDATEENTITIESGROUPREQUEST_ADDENTRY']._serialized_end=3933
+  _globals['_UPDATEENTITIESGROUPREQUEST_UPDATEENTRY']._serialized_start=3935
+  _globals['_UPDATEENTITIESGROUPREQUEST_UPDATEENTRY']._serialized_end=4002
+  _globals['_UPDATEENTITIESGROUPRESPONSE']._serialized_start=4005
+  _globals['_UPDATEENTITIESGROUPRESPONSE']._serialized_end=4174
+  _globals['_UPDATEENTITIESGROUPRESPONSE_STATUS']._serialized_start=4099
+  _globals['_UPDATEENTITIESGROUPRESPONSE_STATUS']._serialized_end=4174
+  _globals['_LISTENTITIESGROUPSREQUEST']._serialized_start=4176
+  _globals['_LISTENTITIESGROUPSREQUEST']._serialized_end=4245
+  _globals['_LISTENTITIESGROUPSRESPONSE']._serialized_start=4248
+  _globals['_LISTENTITIESGROUPSRESPONSE']._serialized_end=4531
+  _globals['_LISTENTITIESGROUPSRESPONSE_GROUPSENTRY']._serialized_start=4407
+  _globals['_LISTENTITIESGROUPSRESPONSE_GROUPSENTRY']._serialized_end=4488
+  _globals['_LISTENTITIESGROUPSRESPONSE_STATUS']._serialized_start=4490
+  _globals['_LISTENTITIESGROUPSRESPONSE_STATUS']._serialized_end=4531
+  _globals['_GETENTITIESREQUEST']._serialized_start=4533
+  _globals['_GETENTITIESREQUEST']._serialized_end=4595
+  _globals['_GETENTITIESRESPONSE']._serialized_start=4598
+  _globals['_GETENTITIESRESPONSE']._serialized_end=4895
+  _globals['_GETENTITIESRESPONSE_GROUPSENTRY']._serialized_start=4778
+  _globals['_GETENTITIESRESPONSE_GROUPSENTRY']._serialized_end=4852
+  _globals['_GETENTITIESRESPONSE_STATUS']._serialized_start=4490
+  _globals['_GETENTITIESRESPONSE_STATUS']._serialized_end=4531
+  _globals['_DELENTITIESREQUEST']._serialized_start=4897
+  _globals['_DELENTITIESREQUEST']._serialized_end=4974
+  _globals['_MERGEENTITIESREQUEST']._serialized_start=4977
+  _globals['_MERGEENTITIESREQUEST']._serialized_end=5194
+  _globals['_MERGEENTITIESREQUEST_ENTITYID']._serialized_start=5153
+  _globals['_MERGEENTITIESREQUEST_ENTITYID']._serialized_end=5194
+  _globals['_GETLABELSRESPONSE']._serialized_start=5197
+  _globals['_GETLABELSRESPONSE']._serialized_end=5381
+  _globals['_GETLABELSRESPONSE_STATUS']._serialized_start=4490
+  _globals['_GETLABELSRESPONSE_STATUS']._serialized_end=4520
+  _globals['_GETLABELSREQUEST']._serialized_start=5383
+  _globals['_GETLABELSREQUEST']._serialized_end=5443
+  _globals['_GETENTITIESGROUPREQUEST']._serialized_start=5445
+  _globals['_GETENTITIESGROUPREQUEST']._serialized_end=5527
+  _globals['_GETENTITIESGROUPRESPONSE']._serialized_start=5530
+  _globals['_GETENTITIESGROUPRESPONSE']._serialized_end=5779
+  _globals['_GETENTITIESGROUPRESPONSE_STATUS']._serialized_start=5704
+  _globals['_GETENTITIESGROUPRESPONSE_STATUS']._serialized_end=5779
+  _globals['_GETVECTORSETSREQUEST']._serialized_start=5781
+  _globals['_GETVECTORSETSREQUEST']._serialized_end=5845
+  _globals['_GETVECTORSETSRESPONSE']._serialized_start=5848
+  _globals['_GETVECTORSETSRESPONSE']._serialized_end=6059
+  _globals['_GETVECTORSETSRESPONSE_STATUS']._serialized_start=4490
+  _globals['_GETVECTORSETSRESPONSE_STATUS']._serialized_end=4531
+  _globals['_OPSTATUSWRITER']._serialized_start=6061
+  _globals['_OPSTATUSWRITER']._serialized_end=6170
+  _globals['_OPSTATUSWRITER_STATUS']._serialized_start=6129
+  _globals['_OPSTATUSWRITER_STATUS']._serialized_end=6170
+  _globals['_NOTIFICATION']._serialized_start=6173
+  _globals['_NOTIFICATION']._serialized_end=6639
+  _globals['_NOTIFICATION_ACTION']._serialized_start=6531
+  _globals['_NOTIFICATION_ACTION']._serialized_end=6575
+  _globals['_NOTIFICATION_WRITETYPE']._serialized_start=6577
+  _globals['_NOTIFICATION_WRITETYPE']._serialized_end=6639
+  _globals['_MEMBER']._serialized_start=6642
+  _globals['_MEMBER']._serialized_end=6897
+  _globals['_MEMBER_TYPE']._serialized_start=6835
+  _globals['_MEMBER_TYPE']._serialized_end=6897
+  _globals['_LISTMEMBERSREQUEST']._serialized_start=6899
+  _globals['_LISTMEMBERSREQUEST']._serialized_end=6919
+  _globals['_LISTMEMBERSRESPONSE']._serialized_start=6921
+  _globals['_LISTMEMBERSRESPONSE']._serialized_end=6978
+  _globals['_SHARDREPLICA']._serialized_start=6980
+  _globals['_SHARDREPLICA']._serialized_end=7052
+  _globals['_SHARDOBJECT']._serialized_start=7055
+  _globals['_SHARDOBJECT']._serialized_end=7196
+  _globals['_SHARDS']._serialized_start=7199
+  _globals['_SHARDS']._serialized_end=7521
+  _globals['_SHARDS_EXTRAENTRY']._serialized_start=7477
+  _globals['_SHARDS_EXTRAENTRY']._serialized_end=7521
+  _globals['_INDEXRESOURCE']._serialized_start=7523
+  _globals['_INDEXRESOURCE']._serialized_end=7590
+  _globals['_INDEXSTATUS']._serialized_start=7592
+  _globals['_INDEXSTATUS']._serialized_end=7605
+  _globals['_SETVECTORSREQUEST']._serialized_start=7607
+  _globals['_SETVECTORSREQUEST']._serialized_end=7726
+  _globals['_SETVECTORSRESPONSE']._serialized_start=7728
+  _globals['_SETVECTORSRESPONSE']._serialized_end=7763
+  _globals['_FILEREQUEST']._serialized_start=7765
+  _globals['_FILEREQUEST']._serialized_end=7807
+  _globals['_BINARYDATA']._serialized_start=7809
+  _globals['_BINARYDATA']._serialized_end=7835
+  _globals['_BINARYMETADATA']._serialized_start=7837
+  _globals['_BINARYMETADATA']._serialized_end=7934
+  _globals['_UPLOADBINARYDATA']._serialized_start=7936
+  _globals['_UPLOADBINARYDATA']._serialized_end=8043
+  _globals['_FILEUPLOADED']._serialized_start=8045
+  _globals['_FILEUPLOADED']._serialized_end=8059
+  _globals['_SYNONYMSREQUEST']._serialized_start=8061
+  _globals['_SYNONYMSREQUEST']._serialized_end=8092
+  _globals['_NEWVECTORSETREQUEST']._serialized_start=8095
+  _globals['_NEWVECTORSETREQUEST']._serialized_end=8326
+  _globals['_NEWVECTORSETRESPONSE']._serialized_start=8328
+  _globals['_NEWVECTORSETRESPONSE']._serialized_end=8452
+  _globals['_NEWVECTORSETRESPONSE_STATUS']._serialized_start=3414
+  _globals['_NEWVECTORSETRESPONSE_STATUS']._serialized_end=3441
+  _globals['_DELVECTORSETREQUEST']._serialized_start=8454
+  _globals['_DELVECTORSETREQUEST']._serialized_end=8511
+  _globals['_DELVECTORSETRESPONSE']._serialized_start=8513
+  _globals['_DELVECTORSETRESPONSE']._serialized_end=8637
+  _globals['_DELVECTORSETRESPONSE_STATUS']._serialized_start=3414
+  _globals['_DELVECTORSETRESPONSE_STATUS']._serialized_end=3441
+  _globals['_WRITER']._serialized_start=8700
+  _globals['_WRITER']._serialized_end=10444
 # @@protoc_insertion_point(module_scope)
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -22,4876 +22,4824 @@
 00000150: 6469 745f 7062 320a 696d 706f 7274 206e  dit_pb2.import n
 00000160: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
 00000170: 6e6f 776c 6564 6765 626f 785f 7062 320a  nowledgebox_pb2.
 00000180: 696d 706f 7274 206e 7563 6c69 6164 625f  import nucliadb_
 00000190: 7072 6f74 6f73 2e6e 6f64 6572 6573 6f75  protos.noderesou
 000001a0: 7263 6573 5f70 6232 0a69 6d70 6f72 7420  rces_pb2.import 
 000001b0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-000001c0: 7265 736f 7572 6365 735f 7062 320a 696d  resources_pb2.im
-000001d0: 706f 7274 206e 7563 6c69 6164 625f 7072  port nucliadb_pr
-000001e0: 6f74 6f73 2e75 7469 6c73 5f70 6232 0a69  otos.utils_pb2.i
-000001f0: 6d70 6f72 7420 7379 730a 696d 706f 7274  mport sys.import
-00000200: 2074 7970 696e 670a 0a69 6620 7379 732e   typing..if sys.
-00000210: 7665 7273 696f 6e5f 696e 666f 203e 3d20  version_info >= 
-00000220: 2833 2c20 3130 293a 0a20 2020 2069 6d70  (3, 10):.    imp
-00000230: 6f72 7420 7479 7069 6e67 2061 7320 7479  ort typing as ty
-00000240: 7069 6e67 5f65 7874 656e 7369 6f6e 730a  ping_extensions.
-00000250: 656c 7365 3a0a 2020 2020 696d 706f 7274  else:.    import
-00000260: 2074 7970 696e 675f 6578 7465 6e73 696f   typing_extensio
-00000270: 6e73 0a66 726f 6d20 6e75 636c 6961 6462  ns.from nucliadb
-00000280: 5f70 726f 746f 732e 6175 6469 745f 7062  _protos.audit_pb
-00000290: 3220 696d 706f 7274 2028 0a20 2020 2041  2 import (.    A
-000002a0: 5049 2061 7320 4150 492c 0a20 2020 2041  PI as API,.    A
-000002b0: 7564 6974 4669 656c 6420 6173 2041 7564  uditField as Aud
-000002c0: 6974 4669 656c 642c 0a20 2020 2041 7564  itField,.    Aud
-000002d0: 6974 4b42 436f 756e 7465 7220 6173 2041  itKBCounter as A
-000002e0: 7564 6974 4b42 436f 756e 7465 722c 0a20  uditKBCounter,. 
-000002f0: 2020 2041 7564 6974 5265 7175 6573 7420     AuditRequest 
-00000300: 6173 2041 7564 6974 5265 7175 6573 742c  as AuditRequest,
-00000310: 0a20 2020 2043 4852 4f4d 455f 4558 5445  .    CHROME_EXTE
-00000320: 4e53 494f 4e20 6173 2043 4852 4f4d 455f  NSION as CHROME_
-00000330: 4558 5445 4e53 494f 4e2c 0a20 2020 2043  EXTENSION,.    C
-00000340: 6861 7441 7564 6974 2061 7320 4368 6174  hatAudit as Chat
-00000350: 4175 6469 742c 0a20 2020 2043 6861 7443  Audit,.    ChatC
-00000360: 6f6e 7465 7874 2061 7320 4368 6174 436f  ontext as ChatCo
-00000370: 6e74 6578 742c 0a20 2020 2043 6c69 656e  ntext,.    Clien
-00000380: 7454 7970 6520 6173 2043 6c69 656e 7454  tType as ClientT
-00000390: 7970 652c 0a20 2020 2044 4153 4842 4f41  ype,.    DASHBOA
-000003a0: 5244 2061 7320 4441 5348 424f 4152 442c  RD as DASHBOARD,
-000003b0: 0a20 2020 2044 4553 4b54 4f50 2061 7320  .    DESKTOP as 
-000003c0: 4445 534b 544f 502c 0a20 2020 2057 4542  DESKTOP,.    WEB
-000003d0: 2061 7320 5745 422c 0a20 2020 2057 4944   as WEB,.    WID
-000003e0: 4745 5420 6173 2057 4944 4745 542c 0a29  GET as WIDGET,.)
-000003f0: 0a66 726f 6d20 6e75 636c 6961 6462 5f70  .from nucliadb_p
-00000400: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
-00000410: 6f78 5f70 6232 2069 6d70 6f72 7420 280a  ox_pb2 import (.
-00000420: 2020 2020 434f 4e46 4c49 4354 2061 7320      CONFLICT as 
-00000430: 434f 4e46 4c49 4354 2c0a 2020 2020 4465  CONFLICT,.    De
-00000440: 6c65 7465 4b6e 6f77 6c65 6467 6542 6f78  leteKnowledgeBox
-00000450: 5265 7370 6f6e 7365 2061 7320 4465 6c65  Response as Dele
-00000460: 7465 4b6e 6f77 6c65 6467 6542 6f78 5265  teKnowledgeBoxRe
-00000470: 7370 6f6e 7365 2c0a 2020 2020 4465 6c65  sponse,.    Dele
-00000480: 7465 6445 6e74 6974 6965 7347 726f 7570  tedEntitiesGroup
-00000490: 7320 6173 2044 656c 6574 6564 456e 7469  s as DeletedEnti
-000004a0: 7469 6573 4772 6f75 7073 2c0a 2020 2020  tiesGroups,.    
-000004b0: 4552 524f 5220 6173 2045 5252 4f52 2c0a  ERROR as ERROR,.
-000004c0: 2020 2020 456e 7469 7469 6573 4772 6f75      EntitiesGrou
-000004d0: 7020 6173 2045 6e74 6974 6965 7347 726f  p as EntitiesGro
-000004e0: 7570 2c0a 2020 2020 456e 7469 7469 6573  up,.    Entities
-000004f0: 4772 6f75 7053 756d 6d61 7279 2061 7320  GroupSummary as 
-00000500: 456e 7469 7469 6573 4772 6f75 7053 756d  EntitiesGroupSum
-00000510: 6d61 7279 2c0a 2020 2020 456e 7469 7469  mary,.    Entiti
-00000520: 6573 4772 6f75 7073 2061 7320 456e 7469  esGroups as Enti
-00000530: 7469 6573 4772 6f75 7073 2c0a 2020 2020  tiesGroups,.    
-00000540: 456e 7469 7479 2061 7320 456e 7469 7479  Entity as Entity
-00000550: 2c0a 2020 2020 456e 7469 7479 4772 6f75  ,.    EntityGrou
-00000560: 7044 7570 6c69 6361 7465 496e 6465 7820  pDuplicateIndex 
-00000570: 6173 2045 6e74 6974 7947 726f 7570 4475  as EntityGroupDu
-00000580: 706c 6963 6174 6549 6e64 6578 2c0a 2020  plicateIndex,.  
-00000590: 2020 4743 4b6e 6f77 6c65 6467 6542 6f78    GCKnowledgeBox
-000005a0: 5265 7370 6f6e 7365 2061 7320 4743 4b6e  Response as GCKn
-000005b0: 6f77 6c65 6467 6542 6f78 5265 7370 6f6e  owledgeBoxRespon
-000005c0: 7365 2c0a 2020 2020 4b42 436f 6e66 6967  se,.    KBConfig
-000005d0: 7572 6174 696f 6e20 6173 204b 4243 6f6e  uration as KBCon
-000005e0: 6669 6775 7261 7469 6f6e 2c0a 2020 2020  figuration,.    
-000005f0: 4b6e 6f77 6c65 6467 6542 6f78 436f 6e66  KnowledgeBoxConf
-00000600: 6967 2061 7320 4b6e 6f77 6c65 6467 6542  ig as KnowledgeB
-00000610: 6f78 436f 6e66 6967 2c0a 2020 2020 4b6e  oxConfig,.    Kn
-00000620: 6f77 6c65 6467 6542 6f78 4944 2061 7320  owledgeBoxID as 
-00000630: 4b6e 6f77 6c65 6467 6542 6f78 4944 2c0a  KnowledgeBoxID,.
+000001c0: 6e6f 6465 7772 6974 6572 5f70 6232 0a69  nodewriter_pb2.i
+000001d0: 6d70 6f72 7420 6e75 636c 6961 6462 5f70  mport nucliadb_p
+000001e0: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
+000001f0: 7062 320a 696d 706f 7274 206e 7563 6c69  pb2.import nucli
+00000200: 6164 625f 7072 6f74 6f73 2e75 7469 6c73  adb_protos.utils
+00000210: 5f70 6232 0a69 6d70 6f72 7420 7379 730a  _pb2.import sys.
+00000220: 696d 706f 7274 2074 7970 696e 670a 0a69  import typing..i
+00000230: 6620 7379 732e 7665 7273 696f 6e5f 696e  f sys.version_in
+00000240: 666f 203e 3d20 2833 2c20 3130 293a 0a20  fo >= (3, 10):. 
+00000250: 2020 2069 6d70 6f72 7420 7479 7069 6e67     import typing
+00000260: 2061 7320 7479 7069 6e67 5f65 7874 656e   as typing_exten
+00000270: 7369 6f6e 730a 656c 7365 3a0a 2020 2020  sions.else:.    
+00000280: 696d 706f 7274 2074 7970 696e 675f 6578  import typing_ex
+00000290: 7465 6e73 696f 6e73 0a66 726f 6d20 6e75  tensions.from nu
+000002a0: 636c 6961 6462 5f70 726f 746f 732e 6175  cliadb_protos.au
+000002b0: 6469 745f 7062 3220 696d 706f 7274 2028  dit_pb2 import (
+000002c0: 0a20 2020 2041 5049 2061 7320 4150 492c  .    API as API,
+000002d0: 0a20 2020 2041 7564 6974 4669 656c 6420  .    AuditField 
+000002e0: 6173 2041 7564 6974 4669 656c 642c 0a20  as AuditField,. 
+000002f0: 2020 2041 7564 6974 4b42 436f 756e 7465     AuditKBCounte
+00000300: 7220 6173 2041 7564 6974 4b42 436f 756e  r as AuditKBCoun
+00000310: 7465 722c 0a20 2020 2041 7564 6974 5265  ter,.    AuditRe
+00000320: 7175 6573 7420 6173 2041 7564 6974 5265  quest as AuditRe
+00000330: 7175 6573 742c 0a20 2020 2043 4852 4f4d  quest,.    CHROM
+00000340: 455f 4558 5445 4e53 494f 4e20 6173 2043  E_EXTENSION as C
+00000350: 4852 4f4d 455f 4558 5445 4e53 494f 4e2c  HROME_EXTENSION,
+00000360: 0a20 2020 2043 6861 7441 7564 6974 2061  .    ChatAudit a
+00000370: 7320 4368 6174 4175 6469 742c 0a20 2020  s ChatAudit,.   
+00000380: 2043 6861 7443 6f6e 7465 7874 2061 7320   ChatContext as 
+00000390: 4368 6174 436f 6e74 6578 742c 0a20 2020  ChatContext,.   
+000003a0: 2043 6c69 656e 7454 7970 6520 6173 2043   ClientType as C
+000003b0: 6c69 656e 7454 7970 652c 0a20 2020 2044  lientType,.    D
+000003c0: 4153 4842 4f41 5244 2061 7320 4441 5348  ASHBOARD as DASH
+000003d0: 424f 4152 442c 0a20 2020 2044 4553 4b54  BOARD,.    DESKT
+000003e0: 4f50 2061 7320 4445 534b 544f 502c 0a20  OP as DESKTOP,. 
+000003f0: 2020 2057 4542 2061 7320 5745 422c 0a20     WEB as WEB,. 
+00000400: 2020 2057 4944 4745 5420 6173 2057 4944     WIDGET as WID
+00000410: 4745 542c 0a29 0a66 726f 6d20 6e75 636c  GET,.).from nucl
+00000420: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+00000430: 6c65 6467 6562 6f78 5f70 6232 2069 6d70  ledgebox_pb2 imp
+00000440: 6f72 7420 280a 2020 2020 434f 4e46 4c49  ort (.    CONFLI
+00000450: 4354 2061 7320 434f 4e46 4c49 4354 2c0a  CT as CONFLICT,.
+00000460: 2020 2020 4465 6c65 7465 4b6e 6f77 6c65      DeleteKnowle
+00000470: 6467 6542 6f78 5265 7370 6f6e 7365 2061  dgeBoxResponse a
+00000480: 7320 4465 6c65 7465 4b6e 6f77 6c65 6467  s DeleteKnowledg
+00000490: 6542 6f78 5265 7370 6f6e 7365 2c0a 2020  eBoxResponse,.  
+000004a0: 2020 4465 6c65 7465 6445 6e74 6974 6965    DeletedEntitie
+000004b0: 7347 726f 7570 7320 6173 2044 656c 6574  sGroups as Delet
+000004c0: 6564 456e 7469 7469 6573 4772 6f75 7073  edEntitiesGroups
+000004d0: 2c0a 2020 2020 4552 524f 5220 6173 2045  ,.    ERROR as E
+000004e0: 5252 4f52 2c0a 2020 2020 456e 7469 7469  RROR,.    Entiti
+000004f0: 6573 4772 6f75 7020 6173 2045 6e74 6974  esGroup as Entit
+00000500: 6965 7347 726f 7570 2c0a 2020 2020 456e  iesGroup,.    En
+00000510: 7469 7469 6573 4772 6f75 7053 756d 6d61  titiesGroupSumma
+00000520: 7279 2061 7320 456e 7469 7469 6573 4772  ry as EntitiesGr
+00000530: 6f75 7053 756d 6d61 7279 2c0a 2020 2020  oupSummary,.    
+00000540: 456e 7469 7469 6573 4772 6f75 7073 2061  EntitiesGroups a
+00000550: 7320 456e 7469 7469 6573 4772 6f75 7073  s EntitiesGroups
+00000560: 2c0a 2020 2020 456e 7469 7479 2061 7320  ,.    Entity as 
+00000570: 456e 7469 7479 2c0a 2020 2020 456e 7469  Entity,.    Enti
+00000580: 7479 4772 6f75 7044 7570 6c69 6361 7465  tyGroupDuplicate
+00000590: 496e 6465 7820 6173 2045 6e74 6974 7947  Index as EntityG
+000005a0: 726f 7570 4475 706c 6963 6174 6549 6e64  roupDuplicateInd
+000005b0: 6578 2c0a 2020 2020 4743 4b6e 6f77 6c65  ex,.    GCKnowle
+000005c0: 6467 6542 6f78 5265 7370 6f6e 7365 2061  dgeBoxResponse a
+000005d0: 7320 4743 4b6e 6f77 6c65 6467 6542 6f78  s GCKnowledgeBox
+000005e0: 5265 7370 6f6e 7365 2c0a 2020 2020 4b42  Response,.    KB
+000005f0: 436f 6e66 6967 7572 6174 696f 6e20 6173  Configuration as
+00000600: 204b 4243 6f6e 6669 6775 7261 7469 6f6e   KBConfiguration
+00000610: 2c0a 2020 2020 4b6e 6f77 6c65 6467 6542  ,.    KnowledgeB
+00000620: 6f78 436f 6e66 6967 2061 7320 4b6e 6f77  oxConfig as Know
+00000630: 6c65 6467 6542 6f78 436f 6e66 6967 2c0a  ledgeBoxConfig,.
 00000640: 2020 2020 4b6e 6f77 6c65 6467 6542 6f78      KnowledgeBox
-00000650: 4e65 7720 6173 204b 6e6f 776c 6564 6765  New as Knowledge
-00000660: 426f 784e 6577 2c0a 2020 2020 4b6e 6f77  BoxNew,.    Know
-00000670: 6c65 6467 6542 6f78 5265 7370 6f6e 7365  ledgeBoxResponse
-00000680: 5374 6174 7573 2061 7320 4b6e 6f77 6c65  Status as Knowle
-00000690: 6467 6542 6f78 5265 7370 6f6e 7365 5374  dgeBoxResponseSt
-000006a0: 6174 7573 2c0a 2020 2020 4b6e 6f77 6c65  atus,.    Knowle
-000006b0: 6467 6542 6f78 5570 6461 7465 2061 7320  dgeBoxUpdate as 
-000006c0: 4b6e 6f77 6c65 6467 6542 6f78 5570 6461  KnowledgeBoxUpda
-000006d0: 7465 2c0a 2020 2020 4b6e 6f77 6c65 6467  te,.    Knowledg
-000006e0: 6542 6f78 5665 6374 6f72 5365 7473 436f  eBoxVectorSetsCo
-000006f0: 6e66 6967 2061 7320 4b6e 6f77 6c65 6467  nfig as Knowledg
-00000700: 6542 6f78 5665 6374 6f72 5365 7473 436f  eBoxVectorSetsCo
-00000710: 6e66 6967 2c0a 2020 2020 4c61 6265 6c20  nfig,.    Label 
-00000720: 6173 204c 6162 656c 2c0a 2020 2020 4c61  as Label,.    La
-00000730: 6265 6c53 6574 2061 7320 4c61 6265 6c53  belSet as LabelS
-00000740: 6574 2c0a 2020 2020 4c61 6265 6c73 2061  et,.    Labels a
-00000750: 7320 4c61 6265 6c73 2c0a 2020 2020 4e4f  s Labels,.    NO
-00000760: 5446 4f55 4e44 2061 7320 4e4f 5446 4f55  TFOUND as NOTFOU
-00000770: 4e44 2c0a 2020 2020 4e65 774b 6e6f 776c  ND,.    NewKnowl
-00000780: 6564 6765 426f 7852 6573 706f 6e73 6520  edgeBoxResponse 
-00000790: 6173 204e 6577 4b6e 6f77 6c65 6467 6542  as NewKnowledgeB
-000007a0: 6f78 5265 7370 6f6e 7365 2c0a 2020 2020  oxResponse,.    
-000007b0: 4f4b 2061 7320 4f4b 2c0a 2020 2020 5365  OK as OK,.    Se
-000007c0: 6d61 6e74 6963 4d6f 6465 6c4d 6574 6164  manticModelMetad
-000007d0: 6174 6120 6173 2053 656d 616e 7469 634d  ata as SemanticM
-000007e0: 6f64 656c 4d65 7461 6461 7461 2c0a 2020  odelMetadata,.  
-000007f0: 2020 5379 6e6f 6e79 6d73 2061 7320 5379    Synonyms as Sy
-00000800: 6e6f 6e79 6d73 2c0a 2020 2020 5465 726d  nonyms,.    Term
-00000810: 5379 6e6f 6e79 6d73 2061 7320 5465 726d  Synonyms as Term
-00000820: 5379 6e6f 6e79 6d73 2c0a 2020 2020 5570  Synonyms,.    Up
-00000830: 6461 7465 4b6e 6f77 6c65 6467 6542 6f78  dateKnowledgeBox
-00000840: 5265 7370 6f6e 7365 2061 7320 5570 6461  Response as Upda
-00000850: 7465 4b6e 6f77 6c65 6467 6542 6f78 5265  teKnowledgeBoxRe
-00000860: 7370 6f6e 7365 2c0a 2020 2020 5665 6374  sponse,.    Vect
-00000870: 6f72 5365 7420 6173 2056 6563 746f 7253  orSet as VectorS
-00000880: 6574 2c0a 2020 2020 5665 6374 6f72 5365  et,.    VectorSe
-00000890: 7443 6f6e 6669 6720 6173 2056 6563 746f  tConfig as Vecto
-000008a0: 7253 6574 436f 6e66 6967 2c0a 2020 2020  rSetConfig,.    
-000008b0: 5665 6374 6f72 5365 7473 2061 7320 5665  VectorSets as Ve
-000008c0: 6374 6f72 5365 7473 2c0a 290a 6672 6f6d  ctorSets,.).from
-000008d0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-000008e0: 2e6e 6f64 6572 6573 6f75 7263 6573 5f70  .noderesources_p
-000008f0: 6232 2069 6d70 6f72 7420 280a 2020 2020  b2 import (.    
-00000900: 456d 7074 7951 7565 7279 2061 7320 456d  EmptyQuery as Em
-00000910: 7074 7951 7565 7279 2c0a 2020 2020 456d  ptyQuery,.    Em
-00000920: 7074 7952 6573 706f 6e73 6520 6173 2045  ptyResponse as E
-00000930: 6d70 7479 5265 7370 6f6e 7365 2c0a 2020  mptyResponse,.  
-00000940: 2020 496e 6465 784d 6574 6164 6174 6120    IndexMetadata 
-00000950: 6173 2049 6e64 6578 4d65 7461 6461 7461  as IndexMetadata
-00000960: 2c0a 2020 2020 496e 6465 7850 6172 6167  ,.    IndexParag
-00000970: 7261 7068 2061 7320 496e 6465 7850 6172  raph as IndexPar
-00000980: 6167 7261 7068 2c0a 2020 2020 496e 6465  agraph,.    Inde
-00000990: 7850 6172 6167 7261 7068 7320 6173 2049  xParagraphs as I
-000009a0: 6e64 6578 5061 7261 6772 6170 6873 2c0a  ndexParagraphs,.
-000009b0: 2020 2020 4e6f 6465 4d65 7461 6461 7461      NodeMetadata
-000009c0: 2061 7320 4e6f 6465 4d65 7461 6461 7461   as NodeMetadata
-000009d0: 2c0a 2020 2020 5061 7261 6772 6170 684d  ,.    ParagraphM
-000009e0: 6574 6164 6174 6120 6173 2050 6172 6167  etadata as Parag
-000009f0: 7261 7068 4d65 7461 6461 7461 2c0a 2020  raphMetadata,.  
-00000a00: 2020 506f 7369 7469 6f6e 2061 7320 506f    Position as Po
-00000a10: 7369 7469 6f6e 2c0a 2020 2020 5265 7072  sition,.    Repr
-00000a20: 6573 656e 7461 7469 6f6e 2061 7320 5265  esentation as Re
-00000a30: 7072 6573 656e 7461 7469 6f6e 2c0a 2020  presentation,.  
-00000a40: 2020 5265 736f 7572 6365 2061 7320 5265    Resource as Re
-00000a50: 736f 7572 6365 2c0a 2020 2020 5265 736f  source,.    Reso
-00000a60: 7572 6365 4944 2061 7320 5265 736f 7572  urceID as Resour
-00000a70: 6365 4944 2c0a 2020 2020 5365 6e74 656e  ceID,.    Senten
-00000a80: 6365 4d65 7461 6461 7461 2061 7320 5365  ceMetadata as Se
-00000a90: 6e74 656e 6365 4d65 7461 6461 7461 2c0a  ntenceMetadata,.
-00000aa0: 2020 2020 5368 6172 6420 6173 2053 6861      Shard as Sha
-00000ab0: 7264 2c0a 2020 2020 5368 6172 6443 7265  rd,.    ShardCre
-00000ac0: 6174 6564 2061 7320 5368 6172 6443 7265  ated as ShardCre
-00000ad0: 6174 6564 2c0a 2020 2020 5368 6172 6449  ated,.    ShardI
-00000ae0: 6420 6173 2053 6861 7264 4964 2c0a 2020  d as ShardId,.  
-00000af0: 2020 5368 6172 6449 6473 2061 7320 5368    ShardIds as Sh
-00000b00: 6172 6449 6473 2c0a 2020 2020 5368 6172  ardIds,.    Shar
-00000b10: 644d 6574 6164 6174 6120 6173 2053 6861  dMetadata as Sha
-00000b20: 7264 4d65 7461 6461 7461 2c0a 2020 2020  rdMetadata,.    
-00000b30: 5465 7874 496e 666f 726d 6174 696f 6e20  TextInformation 
-00000b40: 6173 2054 6578 7449 6e66 6f72 6d61 7469  as TextInformati
-00000b50: 6f6e 2c0a 2020 2020 5665 6374 6f72 5365  on,.    VectorSe
-00000b60: 6e74 656e 6365 2061 7320 5665 6374 6f72  ntence as Vector
-00000b70: 5365 6e74 656e 6365 2c0a 2020 2020 5665  Sentence,.    Ve
-00000b80: 6374 6f72 5365 7449 4420 6173 2056 6563  ctorSetID as Vec
-00000b90: 746f 7253 6574 4944 2c0a 2020 2020 5665  torSetID,.    Ve
-00000ba0: 6374 6f72 5365 744c 6973 7420 6173 2056  ctorSetList as V
-00000bb0: 6563 746f 7253 6574 4c69 7374 2c0a 2020  ectorSetList,.  
-00000bc0: 2020 5665 6374 6f72 7365 7453 656e 7465    VectorsetSente
-00000bd0: 6e63 6573 2061 7320 5665 6374 6f72 7365  nces as Vectorse
-00000be0: 7453 656e 7465 6e63 6573 2c0a 290a 6672  tSentences,.).fr
-00000bf0: 6f6d 206e 7563 6c69 6164 625f 7072 6f74  om nucliadb_prot
-00000c00: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
-00000c10: 2069 6d70 6f72 7420 280a 2020 2020 416c   import (.    Al
-00000c20: 6c46 6965 6c64 4944 7320 6173 2041 6c6c  lFieldIDs as All
-00000c30: 4669 656c 6449 4473 2c0a 2020 2020 416e  FieldIDs,.    An
-00000c40: 7377 6572 7320 6173 2041 6e73 7765 7273  swers as Answers
-00000c50: 2c0a 2020 2020 4261 7369 6320 6173 2042  ,.    Basic as B
-00000c60: 6173 6963 2c0a 2020 2020 426c 6f63 6b20  asic,.    Block 
-00000c70: 6173 2042 6c6f 636b 2c0a 2020 2020 434f  as Block,.    CO
-00000c80: 4e56 4552 5341 5449 4f4e 2061 7320 434f  NVERSATION as CO
-00000c90: 4e56 4552 5341 5449 4f4e 2c0a 2020 2020  NVERSATION,.    
-00000ca0: 436c 6173 7369 6669 6361 7469 6f6e 2061  Classification a
-00000cb0: 7320 436c 6173 7369 6669 6361 7469 6f6e  s Classification
-00000cc0: 2c0a 2020 2020 436c 6f75 6446 696c 6520  ,.    CloudFile 
-00000cd0: 6173 2043 6c6f 7564 4669 6c65 2c0a 2020  as CloudFile,.  
-00000ce0: 2020 436f 6d70 7574 6564 4d65 7461 6461    ComputedMetada
-00000cf0: 7461 2061 7320 436f 6d70 7574 6564 4d65  ta as ComputedMe
-00000d00: 7461 6461 7461 2c0a 2020 2020 436f 6e76  tadata,.    Conv
-00000d10: 6572 7361 7469 6f6e 2061 7320 436f 6e76  ersation as Conv
-00000d20: 6572 7361 7469 6f6e 2c0a 2020 2020 4441  ersation,.    DA
-00000d30: 5445 5449 4d45 2061 7320 4441 5445 5449  TETIME as DATETI
-00000d40: 4d45 2c0a 2020 2020 456e 7469 7479 2061  ME,.    Entity a
-00000d50: 7320 456e 7469 7479 2c0a 2020 2020 4578  s Entity,.    Ex
-00000d60: 7472 6120 6173 2045 7874 7261 2c0a 2020  tra as Extra,.  
-00000d70: 2020 4578 7472 6163 7465 6454 6578 7457    ExtractedTextW
-00000d80: 7261 7070 6572 2061 7320 4578 7472 6163  rapper as Extrac
-00000d90: 7465 6454 6578 7457 7261 7070 6572 2c0a  tedTextWrapper,.
-00000da0: 2020 2020 4578 7472 6163 7465 6456 6563      ExtractedVec
-00000db0: 746f 7273 5772 6170 7065 7220 6173 2045  torsWrapper as E
-00000dc0: 7874 7261 6374 6564 5665 6374 6f72 7357  xtractedVectorsW
-00000dd0: 7261 7070 6572 2c0a 2020 2020 4649 4c45  rapper,.    FILE
-00000de0: 2061 7320 4649 4c45 2c0a 2020 2020 4669   as FILE,.    Fi
-00000df0: 656c 6443 6c61 7373 6966 6963 6174 696f  eldClassificatio
-00000e00: 6e73 2061 7320 4669 656c 6443 6c61 7373  ns as FieldClass
-00000e10: 6966 6963 6174 696f 6e73 2c0a 2020 2020  ifications,.    
-00000e20: 4669 656c 6443 6f6d 7075 7465 644d 6574  FieldComputedMet
-00000e30: 6164 6174 6120 6173 2046 6965 6c64 436f  adata as FieldCo
-00000e40: 6d70 7574 6564 4d65 7461 6461 7461 2c0a  mputedMetadata,.
-00000e50: 2020 2020 4669 656c 6443 6f6d 7075 7465      FieldCompute
-00000e60: 644d 6574 6164 6174 6157 7261 7070 6572  dMetadataWrapper
-00000e70: 2061 7320 4669 656c 6443 6f6d 7075 7465   as FieldCompute
-00000e80: 644d 6574 6164 6174 6157 7261 7070 6572  dMetadataWrapper
-00000e90: 2c0a 2020 2020 4669 656c 6443 6f6e 7665  ,.    FieldConve
-00000ea0: 7273 6174 696f 6e20 6173 2046 6965 6c64  rsation as Field
-00000eb0: 436f 6e76 6572 7361 7469 6f6e 2c0a 2020  Conversation,.  
-00000ec0: 2020 4669 656c 6444 6174 6574 696d 6520    FieldDatetime 
-00000ed0: 6173 2046 6965 6c64 4461 7465 7469 6d65  as FieldDatetime
-00000ee0: 2c0a 2020 2020 4669 656c 6446 696c 6520  ,.    FieldFile 
-00000ef0: 6173 2046 6965 6c64 4669 6c65 2c0a 2020  as FieldFile,.  
-00000f00: 2020 4669 656c 6449 4420 6173 2046 6965    FieldID as Fie
-00000f10: 6c64 4944 2c0a 2020 2020 4669 656c 644b  ldID,.    FieldK
-00000f20: 6579 776f 7264 7365 7420 6173 2046 6965  eywordset as Fie
-00000f30: 6c64 4b65 7977 6f72 6473 6574 2c0a 2020  ldKeywordset,.  
-00000f40: 2020 4669 656c 644c 6172 6765 4d65 7461    FieldLargeMeta
-00000f50: 6461 7461 2061 7320 4669 656c 644c 6172  data as FieldLar
-00000f60: 6765 4d65 7461 6461 7461 2c0a 2020 2020  geMetadata,.    
-00000f70: 4669 656c 644c 6179 6f75 7420 6173 2046  FieldLayout as F
-00000f80: 6965 6c64 4c61 796f 7574 2c0a 2020 2020  ieldLayout,.    
-00000f90: 4669 656c 644c 696e 6b20 6173 2046 6965  FieldLink as Fie
-00000fa0: 6c64 4c69 6e6b 2c0a 2020 2020 4669 656c  ldLink,.    Fiel
-00000fb0: 644d 6574 6164 6174 6120 6173 2046 6965  dMetadata as Fie
-00000fc0: 6c64 4d65 7461 6461 7461 2c0a 2020 2020  ldMetadata,.    
-00000fd0: 4669 656c 6451 7565 7374 696f 6e41 6e73  FieldQuestionAns
-00000fe0: 7765 7257 7261 7070 6572 2061 7320 4669  werWrapper as Fi
-00000ff0: 656c 6451 7565 7374 696f 6e41 6e73 7765  eldQuestionAnswe
-00001000: 7257 7261 7070 6572 2c0a 2020 2020 4669  rWrapper,.    Fi
-00001010: 656c 6454 6578 7420 6173 2046 6965 6c64  eldText as Field
-00001020: 5465 7874 2c0a 2020 2020 4669 656c 6454  Text,.    FieldT
-00001030: 7970 6520 6173 2046 6965 6c64 5479 7065  ype as FieldType
-00001040: 2c0a 2020 2020 4669 6c65 4578 7472 6163  ,.    FileExtrac
-00001050: 7465 6444 6174 6120 6173 2046 696c 6545  tedData as FileE
-00001060: 7874 7261 6374 6564 4461 7461 2c0a 2020  xtractedData,.  
-00001070: 2020 4669 6c65 5061 6765 7320 6173 2046    FilePages as F
-00001080: 696c 6550 6167 6573 2c0a 2020 2020 4745  ilePages,.    GE
-00001090: 4e45 5249 4320 6173 2047 454e 4552 4943  NERIC as GENERIC
-000010a0: 2c0a 2020 2020 4b45 5957 4f52 4453 4554  ,.    KEYWORDSET
-000010b0: 2061 7320 4b45 5957 4f52 4453 4554 2c0a   as KEYWORDSET,.
-000010c0: 2020 2020 4b65 7977 6f72 6420 6173 204b      Keyword as K
-000010d0: 6579 776f 7264 2c0a 2020 2020 4c41 594f  eyword,.    LAYO
-000010e0: 5554 2061 7320 4c41 594f 5554 2c0a 2020  UT as LAYOUT,.  
-000010f0: 2020 4c49 4e4b 2061 7320 4c49 4e4b 2c0a    LINK as LINK,.
-00001100: 2020 2020 4c61 7267 6543 6f6d 7075 7465      LargeCompute
-00001110: 644d 6574 6164 6174 6120 6173 204c 6172  dMetadata as Lar
-00001120: 6765 436f 6d70 7574 6564 4d65 7461 6461  geComputedMetada
-00001130: 7461 2c0a 2020 2020 4c61 7267 6543 6f6d  ta,.    LargeCom
-00001140: 7075 7465 644d 6574 6164 6174 6157 7261  putedMetadataWra
-00001150: 7070 6572 2061 7320 4c61 7267 6543 6f6d  pper as LargeCom
-00001160: 7075 7465 644d 6574 6164 6174 6157 7261  putedMetadataWra
-00001170: 7070 6572 2c0a 2020 2020 4c61 796f 7574  pper,.    Layout
-00001180: 436f 6e74 656e 7420 6173 204c 6179 6f75  Content as Layou
-00001190: 7443 6f6e 7465 6e74 2c0a 2020 2020 4c69  tContent,.    Li
-000011a0: 6e6b 4578 7472 6163 7465 6444 6174 6120  nkExtractedData 
-000011b0: 6173 204c 696e 6b45 7874 7261 6374 6564  as LinkExtracted
-000011c0: 4461 7461 2c0a 2020 2020 4d65 7373 6167  Data,.    Messag
-000011d0: 6520 6173 204d 6573 7361 6765 2c0a 2020  e as Message,.  
-000011e0: 2020 4d65 7373 6167 6543 6f6e 7465 6e74    MessageContent
-000011f0: 2061 7320 4d65 7373 6167 6543 6f6e 7465   as MessageConte
-00001200: 6e74 2c0a 2020 2020 4d65 7461 6461 7461  nt,.    Metadata
-00001210: 2061 7320 4d65 7461 6461 7461 2c0a 2020   as Metadata,.  
-00001220: 2020 4e65 7374 6564 4c69 7374 506f 7369    NestedListPosi
-00001230: 7469 6f6e 2061 7320 4e65 7374 6564 4c69  tion as NestedLi
-00001240: 7374 506f 7369 7469 6f6e 2c0a 2020 2020  stPosition,.    
-00001250: 4e65 7374 6564 506f 7369 7469 6f6e 2061  NestedPosition a
-00001260: 7320 4e65 7374 6564 506f 7369 7469 6f6e  s NestedPosition
-00001270: 2c0a 2020 2020 4f72 6967 696e 2061 7320  ,.    Origin as 
-00001280: 4f72 6967 696e 2c0a 2020 2020 5061 6765  Origin,.    Page
-00001290: 496e 666f 726d 6174 696f 6e20 6173 2050  Information as P
-000012a0: 6167 6549 6e66 6f72 6d61 7469 6f6e 2c0a  ageInformation,.
-000012b0: 2020 2020 5061 6765 506f 7369 7469 6f6e      PagePosition
-000012c0: 7320 6173 2050 6167 6550 6f73 6974 696f  s as PagePositio
-000012d0: 6e73 2c0a 2020 2020 5061 6765 5365 6c65  ns,.    PageSele
-000012e0: 6374 696f 6e73 2061 7320 5061 6765 5365  ctions as PageSe
-000012f0: 6c65 6374 696f 6e73 2c0a 2020 2020 5061  lections,.    Pa
-00001300: 6765 5374 7275 6374 7572 6520 6173 2050  geStructure as P
-00001310: 6167 6553 7472 7563 7475 7265 2c0a 2020  ageStructure,.  
-00001320: 2020 5061 6765 5374 7275 6374 7572 6550    PageStructureP
-00001330: 6167 6520 6173 2050 6167 6553 7472 7563  age as PageStruc
-00001340: 7475 7265 5061 6765 2c0a 2020 2020 5061  turePage,.    Pa
-00001350: 6765 5374 7275 6374 7572 6554 6f6b 656e  geStructureToken
-00001360: 2061 7320 5061 6765 5374 7275 6374 7572   as PageStructur
-00001370: 6554 6f6b 656e 2c0a 2020 2020 5061 7261  eToken,.    Para
-00001380: 6772 6170 6820 6173 2050 6172 6167 7261  graph as Paragra
-00001390: 7068 2c0a 2020 2020 5061 7261 6772 6170  ph,.    Paragrap
-000013a0: 6841 6e6e 6f74 6174 696f 6e20 6173 2050  hAnnotation as P
-000013b0: 6172 6167 7261 7068 416e 6e6f 7461 7469  aragraphAnnotati
-000013c0: 6f6e 2c0a 2020 2020 5061 7261 6772 6170  on,.    Paragrap
-000013d0: 6852 656c 6174 696f 6e73 2061 7320 5061  hRelations as Pa
-000013e0: 7261 6772 6170 6852 656c 6174 696f 6e73  ragraphRelations
-000013f0: 2c0a 2020 2020 506f 7369 7469 6f6e 2061  ,.    Position a
-00001400: 7320 506f 7369 7469 6f6e 2c0a 2020 2020  s Position,.    
-00001410: 506f 7369 7469 6f6e 7320 6173 2050 6f73  Positions as Pos
-00001420: 6974 696f 6e73 2c0a 2020 2020 5175 6573  itions,.    Ques
-00001430: 7469 6f6e 2061 7320 5175 6573 7469 6f6e  tion as Question
-00001440: 2c0a 2020 2020 5175 6573 7469 6f6e 416e  ,.    QuestionAn
-00001450: 7377 6572 2061 7320 5175 6573 7469 6f6e  swer as Question
-00001460: 416e 7377 6572 2c0a 2020 2020 5175 6573  Answer,.    Ques
-00001470: 7469 6f6e 416e 7377 6572 416e 6e6f 7461  tionAnswerAnnota
-00001480: 7469 6f6e 2061 7320 5175 6573 7469 6f6e  tion as Question
-00001490: 416e 7377 6572 416e 6e6f 7461 7469 6f6e  AnswerAnnotation
-000014a0: 2c0a 2020 2020 5175 6573 7469 6f6e 416e  ,.    QuestionAn
-000014b0: 7377 6572 7320 6173 2051 7565 7374 696f  swers as Questio
-000014c0: 6e41 6e73 7765 7273 2c0a 2020 2020 5265  nAnswers,.    Re
-000014d0: 6c61 7469 6f6e 7320 6173 2052 656c 6174  lations as Relat
-000014e0: 696f 6e73 2c0a 2020 2020 5265 7072 6573  ions,.    Repres
-000014f0: 656e 7461 7469 6f6e 2061 7320 5265 7072  entation as Repr
-00001500: 6573 656e 7461 7469 6f6e 2c0a 2020 2020  esentation,.    
-00001510: 526f 7773 5072 6576 6965 7720 6173 2052  RowsPreview as R
-00001520: 6f77 7350 7265 7669 6577 2c0a 2020 2020  owsPreview,.    
-00001530: 5365 6e74 656e 6365 2061 7320 5365 6e74  Sentence as Sent
-00001540: 656e 6365 2c0a 2020 2020 5445 5854 2061  ence,.    TEXT a
-00001550: 7320 5445 5854 2c0a 2020 2020 546f 6b65  s TEXT,.    Toke
-00001560: 6e53 706c 6974 2061 7320 546f 6b65 6e53  nSplit as TokenS
-00001570: 706c 6974 2c0a 2020 2020 5573 6572 4669  plit,.    UserFi
-00001580: 656c 644d 6574 6164 6174 6120 6173 2055  eldMetadata as U
-00001590: 7365 7246 6965 6c64 4d65 7461 6461 7461  serFieldMetadata
-000015a0: 2c0a 2020 2020 5573 6572 4d65 7461 6461  ,.    UserMetada
-000015b0: 7461 2061 7320 5573 6572 4d65 7461 6461  ta as UserMetada
-000015c0: 7461 2c0a 2020 2020 5573 6572 5665 6374  ta,.    UserVect
-000015d0: 6f72 7357 7261 7070 6572 2061 7320 5573  orsWrapper as Us
-000015e0: 6572 5665 6374 6f72 7357 7261 7070 6572  erVectorsWrapper
-000015f0: 2c0a 2020 2020 5669 7375 616c 5365 6c65  ,.    VisualSele
-00001600: 6374 696f 6e20 6173 2056 6973 7561 6c53  ction as VisualS
-00001610: 656c 6563 7469 6f6e 2c0a 290a 0a44 4553  election,.)..DES
-00001620: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
-00001630: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
-00001640: 746f 722e 4669 6c65 4465 7363 7269 7074  tor.FileDescript
-00001650: 6f72 0a0a 636c 6173 7320 5f4e 6f74 6966  or..class _Notif
-00001660: 6963 6174 696f 6e53 6f75 7263 653a 0a20  icationSource:. 
-00001670: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
-00001680: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
-00001690: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
-000016a0: 696e 732e 696e 7429 0a20 2020 2056 3a20  ins.int).    V: 
-000016b0: 7479 7069 6e67 5f65 7874 656e 7369 6f6e  typing_extension
-000016c0: 732e 5479 7065 416c 6961 7320 3d20 5661  s.TypeAlias = Va
-000016d0: 6c75 6554 7970 650a 0a63 6c61 7373 205f  lueType..class _
-000016e0: 4e6f 7469 6669 6361 7469 6f6e 536f 7572  NotificationSour
-000016f0: 6365 456e 756d 5479 7065 5772 6170 7065  ceEnumTypeWrappe
-00001700: 7228 676f 6f67 6c65 2e70 726f 746f 6275  r(google.protobu
-00001710: 662e 696e 7465 726e 616c 2e65 6e75 6d5f  f.internal.enum_
-00001720: 7479 7065 5f77 7261 7070 6572 2e5f 456e  type_wrapper._En
-00001730: 756d 5479 7065 5772 6170 7065 725b 5f4e  umTypeWrapper[_N
-00001740: 6f74 6966 6963 6174 696f 6e53 6f75 7263  otificationSourc
-00001750: 652e 5661 6c75 6554 7970 655d 2c20 6275  e.ValueType], bu
-00001760: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
-00001770: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-00001780: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-00001790: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
-000017a0: 6372 6970 746f 720a 2020 2020 554e 5345  criptor.    UNSE
-000017b0: 543a 205f 4e6f 7469 6669 6361 7469 6f6e  T: _Notification
-000017c0: 536f 7572 6365 2e56 616c 7565 5479 7065  Source.ValueType
-000017d0: 2020 2320 300a 2020 2020 5752 4954 4552    # 0.    WRITER
-000017e0: 3a20 5f4e 6f74 6966 6963 6174 696f 6e53  : _NotificationS
-000017f0: 6f75 7263 652e 5661 6c75 6554 7970 6520  ource.ValueType 
-00001800: 2023 2031 0a20 2020 2050 524f 4345 5353   # 1.    PROCESS
-00001810: 4f52 3a20 5f4e 6f74 6966 6963 6174 696f  OR: _Notificatio
-00001820: 6e53 6f75 7263 652e 5661 6c75 6554 7970  nSource.ValueTyp
-00001830: 6520 2023 2032 0a0a 636c 6173 7320 4e6f  e  # 2..class No
-00001840: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
-00001850: 285f 4e6f 7469 6669 6361 7469 6f6e 536f  (_NotificationSo
-00001860: 7572 6365 2c20 6d65 7461 636c 6173 733d  urce, metaclass=
-00001870: 5f4e 6f74 6966 6963 6174 696f 6e53 6f75  _NotificationSou
-00001880: 7263 6545 6e75 6d54 7970 6557 7261 7070  rceEnumTypeWrapp
-00001890: 6572 293a 202e 2e2e 0a0a 554e 5345 543a  er): .....UNSET:
-000018a0: 204e 6f74 6966 6963 6174 696f 6e53 6f75   NotificationSou
-000018b0: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
-000018c0: 2030 0a57 5249 5445 523a 204e 6f74 6966   0.WRITER: Notif
-000018d0: 6963 6174 696f 6e53 6f75 7263 652e 5661  icationSource.Va
-000018e0: 6c75 6554 7970 6520 2023 2031 0a50 524f  lueType  # 1.PRO
-000018f0: 4345 5353 4f52 3a20 4e6f 7469 6669 6361  CESSOR: Notifica
-00001900: 7469 6f6e 536f 7572 6365 2e56 616c 7565  tionSource.Value
-00001910: 5479 7065 2020 2320 320a 676c 6f62 616c  Type  # 2.global
-00001920: 5f5f 5f4e 6f74 6966 6963 6174 696f 6e53  ___NotificationS
-00001930: 6f75 7263 6520 3d20 4e6f 7469 6669 6361  ource = Notifica
-00001940: 7469 6f6e 536f 7572 6365 0a0a 4074 7970  tionSource..@typ
-00001950: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-00001960: 4175 6469 7428 676f 6f67 6c65 2e70 726f  Audit(google.pro
-00001970: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
-00001980: 7373 6167 6529 3a0a 2020 2020 2222 2257  ssage):.    """W
-00001990: 6520 7265 6365 6976 6520 7468 6973 2069  e receive this i
-000019a0: 6e66 6f72 6d61 7469 6f6e 2074 6872 6f77  nformation throw
-000019b0: 2061 6e20 7374 7265 616d 2073 7973 7465   an stream syste
-000019c0: 6d22 2222 0a0a 2020 2020 4445 5343 5249  m"""..    DESCRI
-000019d0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-000019e0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-000019f0: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
-00001a00: 2063 6c61 7373 205f 536f 7572 6365 3a0a   class _Source:.
-00001a10: 2020 2020 2020 2020 5661 6c75 6554 7970          ValueTyp
-00001a20: 6520 3d20 7479 7069 6e67 2e4e 6577 5479  e = typing.NewTy
-00001a30: 7065 2822 5661 6c75 6554 7970 6522 2c20  pe("ValueType", 
-00001a40: 6275 696c 7469 6e73 2e69 6e74 290a 2020  builtins.int).  
-00001a50: 2020 2020 2020 563a 2074 7970 696e 675f        V: typing_
-00001a60: 6578 7465 6e73 696f 6e73 2e54 7970 6541  extensions.TypeA
-00001a70: 6c69 6173 203d 2056 616c 7565 5479 7065  lias = ValueType
-00001a80: 0a0a 2020 2020 636c 6173 7320 5f53 6f75  ..    class _Sou
-00001a90: 7263 6545 6e75 6d54 7970 6557 7261 7070  rceEnumTypeWrapp
-00001aa0: 6572 2867 6f6f 676c 652e 7072 6f74 6f62  er(google.protob
-00001ab0: 7566 2e69 6e74 6572 6e61 6c2e 656e 756d  uf.internal.enum
-00001ac0: 5f74 7970 655f 7772 6170 7065 722e 5f45  _type_wrapper._E
-00001ad0: 6e75 6d54 7970 6557 7261 7070 6572 5b41  numTypeWrapper[A
-00001ae0: 7564 6974 2e5f 536f 7572 6365 2e56 616c  udit._Source.Val
-00001af0: 7565 5479 7065 5d2c 2062 7569 6c74 696e  ueType], builtin
-00001b00: 732e 7479 7065 293a 0a20 2020 2020 2020  s.type):.       
-00001b10: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-00001b20: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-00001b30: 6372 6970 746f 722e 456e 756d 4465 7363  criptor.EnumDesc
-00001b40: 7269 7074 6f72 0a20 2020 2020 2020 2048  riptor.        H
-00001b50: 5454 503a 2041 7564 6974 2e5f 536f 7572  TTP: Audit._Sour
-00001b60: 6365 2e56 616c 7565 5479 7065 2020 2320  ce.ValueType  # 
-00001b70: 300a 2020 2020 2020 2020 4441 5348 424f  0.        DASHBO
-00001b80: 4152 443a 2041 7564 6974 2e5f 536f 7572  ARD: Audit._Sour
-00001b90: 6365 2e56 616c 7565 5479 7065 2020 2320  ce.ValueType  # 
-00001ba0: 310a 2020 2020 2020 2020 4445 534b 544f  1.        DESKTO
-00001bb0: 503a 2041 7564 6974 2e5f 536f 7572 6365  P: Audit._Source
-00001bc0: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
-00001bd0: 0a20 2020 2063 6c61 7373 2053 6f75 7263  .    class Sourc
-00001be0: 6528 5f53 6f75 7263 652c 206d 6574 6163  e(_Source, metac
-00001bf0: 6c61 7373 3d5f 536f 7572 6365 456e 756d  lass=_SourceEnum
-00001c00: 5479 7065 5772 6170 7065 7229 3a20 2e2e  TypeWrapper): ..
-00001c10: 2e0a 2020 2020 4854 5450 3a20 4175 6469  ..    HTTP: Audi
-00001c20: 742e 536f 7572 6365 2e56 616c 7565 5479  t.Source.ValueTy
-00001c30: 7065 2020 2320 300a 2020 2020 4441 5348  pe  # 0.    DASH
-00001c40: 424f 4152 443a 2041 7564 6974 2e53 6f75  BOARD: Audit.Sou
-00001c50: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
-00001c60: 2031 0a20 2020 2044 4553 4b54 4f50 3a20   1.    DESKTOP: 
-00001c70: 4175 6469 742e 536f 7572 6365 2e56 616c  Audit.Source.Val
-00001c80: 7565 5479 7065 2020 2320 320a 0a20 2020  ueType  # 2..   
-00001c90: 2055 5345 525f 4649 454c 445f 4e55 4d42   USER_FIELD_NUMB
-00001ca0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00001cb0: 0a20 2020 2057 4845 4e5f 4649 454c 445f  .    WHEN_FIELD_
-00001cc0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00001cd0: 2e69 6e74 0a20 2020 204f 5249 4749 4e5f  .int.    ORIGIN_
+00000650: 4944 2061 7320 4b6e 6f77 6c65 6467 6542  ID as KnowledgeB
+00000660: 6f78 4944 2c0a 2020 2020 4b6e 6f77 6c65  oxID,.    Knowle
+00000670: 6467 6542 6f78 4e65 7720 6173 204b 6e6f  dgeBoxNew as Kno
+00000680: 776c 6564 6765 426f 784e 6577 2c0a 2020  wledgeBoxNew,.  
+00000690: 2020 4b6e 6f77 6c65 6467 6542 6f78 5265    KnowledgeBoxRe
+000006a0: 7370 6f6e 7365 5374 6174 7573 2061 7320  sponseStatus as 
+000006b0: 4b6e 6f77 6c65 6467 6542 6f78 5265 7370  KnowledgeBoxResp
+000006c0: 6f6e 7365 5374 6174 7573 2c0a 2020 2020  onseStatus,.    
+000006d0: 4b6e 6f77 6c65 6467 6542 6f78 5570 6461  KnowledgeBoxUpda
+000006e0: 7465 2061 7320 4b6e 6f77 6c65 6467 6542  te as KnowledgeB
+000006f0: 6f78 5570 6461 7465 2c0a 2020 2020 4b6e  oxUpdate,.    Kn
+00000700: 6f77 6c65 6467 6542 6f78 5665 6374 6f72  owledgeBoxVector
+00000710: 5365 7473 436f 6e66 6967 2061 7320 4b6e  SetsConfig as Kn
+00000720: 6f77 6c65 6467 6542 6f78 5665 6374 6f72  owledgeBoxVector
+00000730: 5365 7473 436f 6e66 6967 2c0a 2020 2020  SetsConfig,.    
+00000740: 4c61 6265 6c20 6173 204c 6162 656c 2c0a  Label as Label,.
+00000750: 2020 2020 4c61 6265 6c53 6574 2061 7320      LabelSet as 
+00000760: 4c61 6265 6c53 6574 2c0a 2020 2020 4c61  LabelSet,.    La
+00000770: 6265 6c73 2061 7320 4c61 6265 6c73 2c0a  bels as Labels,.
+00000780: 2020 2020 4e4f 5446 4f55 4e44 2061 7320      NOTFOUND as 
+00000790: 4e4f 5446 4f55 4e44 2c0a 2020 2020 4e65  NOTFOUND,.    Ne
+000007a0: 774b 6e6f 776c 6564 6765 426f 7852 6573  wKnowledgeBoxRes
+000007b0: 706f 6e73 6520 6173 204e 6577 4b6e 6f77  ponse as NewKnow
+000007c0: 6c65 6467 6542 6f78 5265 7370 6f6e 7365  ledgeBoxResponse
+000007d0: 2c0a 2020 2020 4f4b 2061 7320 4f4b 2c0a  ,.    OK as OK,.
+000007e0: 2020 2020 5365 6d61 6e74 6963 4d6f 6465      SemanticMode
+000007f0: 6c4d 6574 6164 6174 6120 6173 2053 656d  lMetadata as Sem
+00000800: 616e 7469 634d 6f64 656c 4d65 7461 6461  anticModelMetada
+00000810: 7461 2c0a 2020 2020 5379 6e6f 6e79 6d73  ta,.    Synonyms
+00000820: 2061 7320 5379 6e6f 6e79 6d73 2c0a 2020   as Synonyms,.  
+00000830: 2020 5465 726d 5379 6e6f 6e79 6d73 2061    TermSynonyms a
+00000840: 7320 5465 726d 5379 6e6f 6e79 6d73 2c0a  s TermSynonyms,.
+00000850: 2020 2020 5570 6461 7465 4b6e 6f77 6c65      UpdateKnowle
+00000860: 6467 6542 6f78 5265 7370 6f6e 7365 2061  dgeBoxResponse a
+00000870: 7320 5570 6461 7465 4b6e 6f77 6c65 6467  s UpdateKnowledg
+00000880: 6542 6f78 5265 7370 6f6e 7365 2c0a 2020  eBoxResponse,.  
+00000890: 2020 5665 6374 6f72 5365 7420 6173 2056    VectorSet as V
+000008a0: 6563 746f 7253 6574 2c0a 2020 2020 5665  ectorSet,.    Ve
+000008b0: 6374 6f72 5365 7443 6f6e 6669 6720 6173  ctorSetConfig as
+000008c0: 2056 6563 746f 7253 6574 436f 6e66 6967   VectorSetConfig
+000008d0: 2c0a 2020 2020 5665 6374 6f72 5365 7473  ,.    VectorSets
+000008e0: 2061 7320 5665 6374 6f72 5365 7473 2c0a   as VectorSets,.
+000008f0: 290a 6672 6f6d 206e 7563 6c69 6164 625f  ).from nucliadb_
+00000900: 7072 6f74 6f73 2e6e 6f64 6572 6573 6f75  protos.noderesou
+00000910: 7263 6573 5f70 6232 2069 6d70 6f72 7420  rces_pb2 import 
+00000920: 280a 2020 2020 456d 7074 7951 7565 7279  (.    EmptyQuery
+00000930: 2061 7320 456d 7074 7951 7565 7279 2c0a   as EmptyQuery,.
+00000940: 2020 2020 456d 7074 7952 6573 706f 6e73      EmptyRespons
+00000950: 6520 6173 2045 6d70 7479 5265 7370 6f6e  e as EmptyRespon
+00000960: 7365 2c0a 2020 2020 496e 6465 784d 6574  se,.    IndexMet
+00000970: 6164 6174 6120 6173 2049 6e64 6578 4d65  adata as IndexMe
+00000980: 7461 6461 7461 2c0a 2020 2020 496e 6465  tadata,.    Inde
+00000990: 7850 6172 6167 7261 7068 2061 7320 496e  xParagraph as In
+000009a0: 6465 7850 6172 6167 7261 7068 2c0a 2020  dexParagraph,.  
+000009b0: 2020 496e 6465 7850 6172 6167 7261 7068    IndexParagraph
+000009c0: 7320 6173 2049 6e64 6578 5061 7261 6772  s as IndexParagr
+000009d0: 6170 6873 2c0a 2020 2020 4e6f 6465 4d65  aphs,.    NodeMe
+000009e0: 7461 6461 7461 2061 7320 4e6f 6465 4d65  tadata as NodeMe
+000009f0: 7461 6461 7461 2c0a 2020 2020 5061 7261  tadata,.    Para
+00000a00: 6772 6170 684d 6574 6164 6174 6120 6173  graphMetadata as
+00000a10: 2050 6172 6167 7261 7068 4d65 7461 6461   ParagraphMetada
+00000a20: 7461 2c0a 2020 2020 506f 7369 7469 6f6e  ta,.    Position
+00000a30: 2061 7320 506f 7369 7469 6f6e 2c0a 2020   as Position,.  
+00000a40: 2020 5265 7072 6573 656e 7461 7469 6f6e    Representation
+00000a50: 2061 7320 5265 7072 6573 656e 7461 7469   as Representati
+00000a60: 6f6e 2c0a 2020 2020 5265 736f 7572 6365  on,.    Resource
+00000a70: 2061 7320 5265 736f 7572 6365 2c0a 2020   as Resource,.  
+00000a80: 2020 5265 736f 7572 6365 4944 2061 7320    ResourceID as 
+00000a90: 5265 736f 7572 6365 4944 2c0a 2020 2020  ResourceID,.    
+00000aa0: 5365 6e74 656e 6365 4d65 7461 6461 7461  SentenceMetadata
+00000ab0: 2061 7320 5365 6e74 656e 6365 4d65 7461   as SentenceMeta
+00000ac0: 6461 7461 2c0a 2020 2020 5368 6172 6420  data,.    Shard 
+00000ad0: 6173 2053 6861 7264 2c0a 2020 2020 5368  as Shard,.    Sh
+00000ae0: 6172 6443 7265 6174 6564 2061 7320 5368  ardCreated as Sh
+00000af0: 6172 6443 7265 6174 6564 2c0a 2020 2020  ardCreated,.    
+00000b00: 5368 6172 6449 6420 6173 2053 6861 7264  ShardId as Shard
+00000b10: 4964 2c0a 2020 2020 5368 6172 6449 6473  Id,.    ShardIds
+00000b20: 2061 7320 5368 6172 6449 6473 2c0a 2020   as ShardIds,.  
+00000b30: 2020 5368 6172 644d 6574 6164 6174 6120    ShardMetadata 
+00000b40: 6173 2053 6861 7264 4d65 7461 6461 7461  as ShardMetadata
+00000b50: 2c0a 2020 2020 5465 7874 496e 666f 726d  ,.    TextInform
+00000b60: 6174 696f 6e20 6173 2054 6578 7449 6e66  ation as TextInf
+00000b70: 6f72 6d61 7469 6f6e 2c0a 2020 2020 5665  ormation,.    Ve
+00000b80: 6374 6f72 5365 6e74 656e 6365 2061 7320  ctorSentence as 
+00000b90: 5665 6374 6f72 5365 6e74 656e 6365 2c0a  VectorSentence,.
+00000ba0: 2020 2020 5665 6374 6f72 5365 7449 4420      VectorSetID 
+00000bb0: 6173 2056 6563 746f 7253 6574 4944 2c0a  as VectorSetID,.
+00000bc0: 2020 2020 5665 6374 6f72 5365 744c 6973      VectorSetLis
+00000bd0: 7420 6173 2056 6563 746f 7253 6574 4c69  t as VectorSetLi
+00000be0: 7374 2c0a 2020 2020 5665 6374 6f72 7365  st,.    Vectorse
+00000bf0: 7453 656e 7465 6e63 6573 2061 7320 5665  tSentences as Ve
+00000c00: 6374 6f72 7365 7453 656e 7465 6e63 6573  ctorsetSentences
+00000c10: 2c0a 290a 6672 6f6d 206e 7563 6c69 6164  ,.).from nucliad
+00000c20: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
+00000c30: 6573 5f70 6232 2069 6d70 6f72 7420 280a  es_pb2 import (.
+00000c40: 2020 2020 416c 6c46 6965 6c64 4944 7320      AllFieldIDs 
+00000c50: 6173 2041 6c6c 4669 656c 6449 4473 2c0a  as AllFieldIDs,.
+00000c60: 2020 2020 416e 7377 6572 7320 6173 2041      Answers as A
+00000c70: 6e73 7765 7273 2c0a 2020 2020 4261 7369  nswers,.    Basi
+00000c80: 6320 6173 2042 6173 6963 2c0a 2020 2020  c as Basic,.    
+00000c90: 426c 6f63 6b20 6173 2042 6c6f 636b 2c0a  Block as Block,.
+00000ca0: 2020 2020 434f 4e56 4552 5341 5449 4f4e      CONVERSATION
+00000cb0: 2061 7320 434f 4e56 4552 5341 5449 4f4e   as CONVERSATION
+00000cc0: 2c0a 2020 2020 436c 6173 7369 6669 6361  ,.    Classifica
+00000cd0: 7469 6f6e 2061 7320 436c 6173 7369 6669  tion as Classifi
+00000ce0: 6361 7469 6f6e 2c0a 2020 2020 436c 6f75  cation,.    Clou
+00000cf0: 6446 696c 6520 6173 2043 6c6f 7564 4669  dFile as CloudFi
+00000d00: 6c65 2c0a 2020 2020 436f 6d70 7574 6564  le,.    Computed
+00000d10: 4d65 7461 6461 7461 2061 7320 436f 6d70  Metadata as Comp
+00000d20: 7574 6564 4d65 7461 6461 7461 2c0a 2020  utedMetadata,.  
+00000d30: 2020 436f 6e76 6572 7361 7469 6f6e 2061    Conversation a
+00000d40: 7320 436f 6e76 6572 7361 7469 6f6e 2c0a  s Conversation,.
+00000d50: 2020 2020 4441 5445 5449 4d45 2061 7320      DATETIME as 
+00000d60: 4441 5445 5449 4d45 2c0a 2020 2020 456e  DATETIME,.    En
+00000d70: 7469 7479 2061 7320 456e 7469 7479 2c0a  tity as Entity,.
+00000d80: 2020 2020 4578 7472 6120 6173 2045 7874      Extra as Ext
+00000d90: 7261 2c0a 2020 2020 4578 7472 6163 7465  ra,.    Extracte
+00000da0: 6454 6578 7457 7261 7070 6572 2061 7320  dTextWrapper as 
+00000db0: 4578 7472 6163 7465 6454 6578 7457 7261  ExtractedTextWra
+00000dc0: 7070 6572 2c0a 2020 2020 4578 7472 6163  pper,.    Extrac
+00000dd0: 7465 6456 6563 746f 7273 5772 6170 7065  tedVectorsWrappe
+00000de0: 7220 6173 2045 7874 7261 6374 6564 5665  r as ExtractedVe
+00000df0: 6374 6f72 7357 7261 7070 6572 2c0a 2020  ctorsWrapper,.  
+00000e00: 2020 4649 4c45 2061 7320 4649 4c45 2c0a    FILE as FILE,.
+00000e10: 2020 2020 4669 656c 6443 6c61 7373 6966      FieldClassif
+00000e20: 6963 6174 696f 6e73 2061 7320 4669 656c  ications as Fiel
+00000e30: 6443 6c61 7373 6966 6963 6174 696f 6e73  dClassifications
+00000e40: 2c0a 2020 2020 4669 656c 6443 6f6d 7075  ,.    FieldCompu
+00000e50: 7465 644d 6574 6164 6174 6120 6173 2046  tedMetadata as F
+00000e60: 6965 6c64 436f 6d70 7574 6564 4d65 7461  ieldComputedMeta
+00000e70: 6461 7461 2c0a 2020 2020 4669 656c 6443  data,.    FieldC
+00000e80: 6f6d 7075 7465 644d 6574 6164 6174 6157  omputedMetadataW
+00000e90: 7261 7070 6572 2061 7320 4669 656c 6443  rapper as FieldC
+00000ea0: 6f6d 7075 7465 644d 6574 6164 6174 6157  omputedMetadataW
+00000eb0: 7261 7070 6572 2c0a 2020 2020 4669 656c  rapper,.    Fiel
+00000ec0: 6443 6f6e 7665 7273 6174 696f 6e20 6173  dConversation as
+00000ed0: 2046 6965 6c64 436f 6e76 6572 7361 7469   FieldConversati
+00000ee0: 6f6e 2c0a 2020 2020 4669 656c 6444 6174  on,.    FieldDat
+00000ef0: 6574 696d 6520 6173 2046 6965 6c64 4461  etime as FieldDa
+00000f00: 7465 7469 6d65 2c0a 2020 2020 4669 656c  tetime,.    Fiel
+00000f10: 6446 696c 6520 6173 2046 6965 6c64 4669  dFile as FieldFi
+00000f20: 6c65 2c0a 2020 2020 4669 656c 6449 4420  le,.    FieldID 
+00000f30: 6173 2046 6965 6c64 4944 2c0a 2020 2020  as FieldID,.    
+00000f40: 4669 656c 644b 6579 776f 7264 7365 7420  FieldKeywordset 
+00000f50: 6173 2046 6965 6c64 4b65 7977 6f72 6473  as FieldKeywords
+00000f60: 6574 2c0a 2020 2020 4669 656c 644c 6172  et,.    FieldLar
+00000f70: 6765 4d65 7461 6461 7461 2061 7320 4669  geMetadata as Fi
+00000f80: 656c 644c 6172 6765 4d65 7461 6461 7461  eldLargeMetadata
+00000f90: 2c0a 2020 2020 4669 656c 644c 6179 6f75  ,.    FieldLayou
+00000fa0: 7420 6173 2046 6965 6c64 4c61 796f 7574  t as FieldLayout
+00000fb0: 2c0a 2020 2020 4669 656c 644c 696e 6b20  ,.    FieldLink 
+00000fc0: 6173 2046 6965 6c64 4c69 6e6b 2c0a 2020  as FieldLink,.  
+00000fd0: 2020 4669 656c 644d 6574 6164 6174 6120    FieldMetadata 
+00000fe0: 6173 2046 6965 6c64 4d65 7461 6461 7461  as FieldMetadata
+00000ff0: 2c0a 2020 2020 4669 656c 6451 7565 7374  ,.    FieldQuest
+00001000: 696f 6e41 6e73 7765 7257 7261 7070 6572  ionAnswerWrapper
+00001010: 2061 7320 4669 656c 6451 7565 7374 696f   as FieldQuestio
+00001020: 6e41 6e73 7765 7257 7261 7070 6572 2c0a  nAnswerWrapper,.
+00001030: 2020 2020 4669 656c 6454 6578 7420 6173      FieldText as
+00001040: 2046 6965 6c64 5465 7874 2c0a 2020 2020   FieldText,.    
+00001050: 4669 656c 6454 7970 6520 6173 2046 6965  FieldType as Fie
+00001060: 6c64 5479 7065 2c0a 2020 2020 4669 6c65  ldType,.    File
+00001070: 4578 7472 6163 7465 6444 6174 6120 6173  ExtractedData as
+00001080: 2046 696c 6545 7874 7261 6374 6564 4461   FileExtractedDa
+00001090: 7461 2c0a 2020 2020 4669 6c65 5061 6765  ta,.    FilePage
+000010a0: 7320 6173 2046 696c 6550 6167 6573 2c0a  s as FilePages,.
+000010b0: 2020 2020 4745 4e45 5249 4320 6173 2047      GENERIC as G
+000010c0: 454e 4552 4943 2c0a 2020 2020 4b45 5957  ENERIC,.    KEYW
+000010d0: 4f52 4453 4554 2061 7320 4b45 5957 4f52  ORDSET as KEYWOR
+000010e0: 4453 4554 2c0a 2020 2020 4b65 7977 6f72  DSET,.    Keywor
+000010f0: 6420 6173 204b 6579 776f 7264 2c0a 2020  d as Keyword,.  
+00001100: 2020 4c41 594f 5554 2061 7320 4c41 594f    LAYOUT as LAYO
+00001110: 5554 2c0a 2020 2020 4c49 4e4b 2061 7320  UT,.    LINK as 
+00001120: 4c49 4e4b 2c0a 2020 2020 4c61 7267 6543  LINK,.    LargeC
+00001130: 6f6d 7075 7465 644d 6574 6164 6174 6120  omputedMetadata 
+00001140: 6173 204c 6172 6765 436f 6d70 7574 6564  as LargeComputed
+00001150: 4d65 7461 6461 7461 2c0a 2020 2020 4c61  Metadata,.    La
+00001160: 7267 6543 6f6d 7075 7465 644d 6574 6164  rgeComputedMetad
+00001170: 6174 6157 7261 7070 6572 2061 7320 4c61  ataWrapper as La
+00001180: 7267 6543 6f6d 7075 7465 644d 6574 6164  rgeComputedMetad
+00001190: 6174 6157 7261 7070 6572 2c0a 2020 2020  ataWrapper,.    
+000011a0: 4c61 796f 7574 436f 6e74 656e 7420 6173  LayoutContent as
+000011b0: 204c 6179 6f75 7443 6f6e 7465 6e74 2c0a   LayoutContent,.
+000011c0: 2020 2020 4c69 6e6b 4578 7472 6163 7465      LinkExtracte
+000011d0: 6444 6174 6120 6173 204c 696e 6b45 7874  dData as LinkExt
+000011e0: 7261 6374 6564 4461 7461 2c0a 2020 2020  ractedData,.    
+000011f0: 4d65 7373 6167 6520 6173 204d 6573 7361  Message as Messa
+00001200: 6765 2c0a 2020 2020 4d65 7373 6167 6543  ge,.    MessageC
+00001210: 6f6e 7465 6e74 2061 7320 4d65 7373 6167  ontent as Messag
+00001220: 6543 6f6e 7465 6e74 2c0a 2020 2020 4d65  eContent,.    Me
+00001230: 7461 6461 7461 2061 7320 4d65 7461 6461  tadata as Metada
+00001240: 7461 2c0a 2020 2020 4e65 7374 6564 4c69  ta,.    NestedLi
+00001250: 7374 506f 7369 7469 6f6e 2061 7320 4e65  stPosition as Ne
+00001260: 7374 6564 4c69 7374 506f 7369 7469 6f6e  stedListPosition
+00001270: 2c0a 2020 2020 4e65 7374 6564 506f 7369  ,.    NestedPosi
+00001280: 7469 6f6e 2061 7320 4e65 7374 6564 506f  tion as NestedPo
+00001290: 7369 7469 6f6e 2c0a 2020 2020 4f72 6967  sition,.    Orig
+000012a0: 696e 2061 7320 4f72 6967 696e 2c0a 2020  in as Origin,.  
+000012b0: 2020 5061 6765 496e 666f 726d 6174 696f    PageInformatio
+000012c0: 6e20 6173 2050 6167 6549 6e66 6f72 6d61  n as PageInforma
+000012d0: 7469 6f6e 2c0a 2020 2020 5061 6765 506f  tion,.    PagePo
+000012e0: 7369 7469 6f6e 7320 6173 2050 6167 6550  sitions as PageP
+000012f0: 6f73 6974 696f 6e73 2c0a 2020 2020 5061  ositions,.    Pa
+00001300: 6765 5365 6c65 6374 696f 6e73 2061 7320  geSelections as 
+00001310: 5061 6765 5365 6c65 6374 696f 6e73 2c0a  PageSelections,.
+00001320: 2020 2020 5061 6765 5374 7275 6374 7572      PageStructur
+00001330: 6520 6173 2050 6167 6553 7472 7563 7475  e as PageStructu
+00001340: 7265 2c0a 2020 2020 5061 6765 5374 7275  re,.    PageStru
+00001350: 6374 7572 6550 6167 6520 6173 2050 6167  cturePage as Pag
+00001360: 6553 7472 7563 7475 7265 5061 6765 2c0a  eStructurePage,.
+00001370: 2020 2020 5061 6765 5374 7275 6374 7572      PageStructur
+00001380: 6554 6f6b 656e 2061 7320 5061 6765 5374  eToken as PageSt
+00001390: 7275 6374 7572 6554 6f6b 656e 2c0a 2020  ructureToken,.  
+000013a0: 2020 5061 7261 6772 6170 6820 6173 2050    Paragraph as P
+000013b0: 6172 6167 7261 7068 2c0a 2020 2020 5061  aragraph,.    Pa
+000013c0: 7261 6772 6170 6841 6e6e 6f74 6174 696f  ragraphAnnotatio
+000013d0: 6e20 6173 2050 6172 6167 7261 7068 416e  n as ParagraphAn
+000013e0: 6e6f 7461 7469 6f6e 2c0a 2020 2020 5061  notation,.    Pa
+000013f0: 7261 6772 6170 6852 656c 6174 696f 6e73  ragraphRelations
+00001400: 2061 7320 5061 7261 6772 6170 6852 656c   as ParagraphRel
+00001410: 6174 696f 6e73 2c0a 2020 2020 506f 7369  ations,.    Posi
+00001420: 7469 6f6e 2061 7320 506f 7369 7469 6f6e  tion as Position
+00001430: 2c0a 2020 2020 506f 7369 7469 6f6e 7320  ,.    Positions 
+00001440: 6173 2050 6f73 6974 696f 6e73 2c0a 2020  as Positions,.  
+00001450: 2020 5175 6573 7469 6f6e 2061 7320 5175    Question as Qu
+00001460: 6573 7469 6f6e 2c0a 2020 2020 5175 6573  estion,.    Ques
+00001470: 7469 6f6e 416e 7377 6572 2061 7320 5175  tionAnswer as Qu
+00001480: 6573 7469 6f6e 416e 7377 6572 2c0a 2020  estionAnswer,.  
+00001490: 2020 5175 6573 7469 6f6e 416e 7377 6572    QuestionAnswer
+000014a0: 416e 6e6f 7461 7469 6f6e 2061 7320 5175  Annotation as Qu
+000014b0: 6573 7469 6f6e 416e 7377 6572 416e 6e6f  estionAnswerAnno
+000014c0: 7461 7469 6f6e 2c0a 2020 2020 5175 6573  tation,.    Ques
+000014d0: 7469 6f6e 416e 7377 6572 7320 6173 2051  tionAnswers as Q
+000014e0: 7565 7374 696f 6e41 6e73 7765 7273 2c0a  uestionAnswers,.
+000014f0: 2020 2020 5265 6c61 7469 6f6e 7320 6173      Relations as
+00001500: 2052 656c 6174 696f 6e73 2c0a 2020 2020   Relations,.    
+00001510: 5265 7072 6573 656e 7461 7469 6f6e 2061  Representation a
+00001520: 7320 5265 7072 6573 656e 7461 7469 6f6e  s Representation
+00001530: 2c0a 2020 2020 526f 7773 5072 6576 6965  ,.    RowsPrevie
+00001540: 7720 6173 2052 6f77 7350 7265 7669 6577  w as RowsPreview
+00001550: 2c0a 2020 2020 5365 6e74 656e 6365 2061  ,.    Sentence a
+00001560: 7320 5365 6e74 656e 6365 2c0a 2020 2020  s Sentence,.    
+00001570: 5445 5854 2061 7320 5445 5854 2c0a 2020  TEXT as TEXT,.  
+00001580: 2020 546f 6b65 6e53 706c 6974 2061 7320    TokenSplit as 
+00001590: 546f 6b65 6e53 706c 6974 2c0a 2020 2020  TokenSplit,.    
+000015a0: 5573 6572 4669 656c 644d 6574 6164 6174  UserFieldMetadat
+000015b0: 6120 6173 2055 7365 7246 6965 6c64 4d65  a as UserFieldMe
+000015c0: 7461 6461 7461 2c0a 2020 2020 5573 6572  tadata,.    User
+000015d0: 4d65 7461 6461 7461 2061 7320 5573 6572  Metadata as User
+000015e0: 4d65 7461 6461 7461 2c0a 2020 2020 5573  Metadata,.    Us
+000015f0: 6572 5665 6374 6f72 7357 7261 7070 6572  erVectorsWrapper
+00001600: 2061 7320 5573 6572 5665 6374 6f72 7357   as UserVectorsW
+00001610: 7261 7070 6572 2c0a 2020 2020 5669 7375  rapper,.    Visu
+00001620: 616c 5365 6c65 6374 696f 6e20 6173 2056  alSelection as V
+00001630: 6973 7561 6c53 656c 6563 7469 6f6e 2c0a  isualSelection,.
+00001640: 290a 0a44 4553 4352 4950 544f 523a 2067  )..DESCRIPTOR: g
+00001650: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00001660: 6573 6372 6970 746f 722e 4669 6c65 4465  escriptor.FileDe
+00001670: 7363 7269 7074 6f72 0a0a 636c 6173 7320  scriptor..class 
+00001680: 5f4e 6f74 6966 6963 6174 696f 6e53 6f75  _NotificationSou
+00001690: 7263 653a 0a20 2020 2056 616c 7565 5479  rce:.    ValueTy
+000016a0: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
+000016b0: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
+000016c0: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
+000016d0: 2020 2056 3a20 7479 7069 6e67 5f65 7874     V: typing_ext
+000016e0: 656e 7369 6f6e 732e 5479 7065 416c 6961  ensions.TypeAlia
+000016f0: 7320 3d20 5661 6c75 6554 7970 650a 0a63  s = ValueType..c
+00001700: 6c61 7373 205f 4e6f 7469 6669 6361 7469  lass _Notificati
+00001710: 6f6e 536f 7572 6365 456e 756d 5479 7065  onSourceEnumType
+00001720: 5772 6170 7065 7228 676f 6f67 6c65 2e70  Wrapper(google.p
+00001730: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
+00001740: 2e65 6e75 6d5f 7479 7065 5f77 7261 7070  .enum_type_wrapp
+00001750: 6572 2e5f 456e 756d 5479 7065 5772 6170  er._EnumTypeWrap
+00001760: 7065 725b 5f4e 6f74 6966 6963 6174 696f  per[_Notificatio
+00001770: 6e53 6f75 7263 652e 5661 6c75 6554 7970  nSource.ValueTyp
+00001780: 655d 2c20 6275 696c 7469 6e73 2e74 7970  e], builtins.typ
+00001790: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+000017a0: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+000017b0: 6275 662e 6465 7363 7269 7074 6f72 2e45  buf.descriptor.E
+000017c0: 6e75 6d44 6573 6372 6970 746f 720a 2020  numDescriptor.  
+000017d0: 2020 554e 5345 543a 205f 4e6f 7469 6669    UNSET: _Notifi
+000017e0: 6361 7469 6f6e 536f 7572 6365 2e56 616c  cationSource.Val
+000017f0: 7565 5479 7065 2020 2320 300a 2020 2020  ueType  # 0.    
+00001800: 5752 4954 4552 3a20 5f4e 6f74 6966 6963  WRITER: _Notific
+00001810: 6174 696f 6e53 6f75 7263 652e 5661 6c75  ationSource.Valu
+00001820: 6554 7970 6520 2023 2031 0a20 2020 2050  eType  # 1.    P
+00001830: 524f 4345 5353 4f52 3a20 5f4e 6f74 6966  ROCESSOR: _Notif
+00001840: 6963 6174 696f 6e53 6f75 7263 652e 5661  icationSource.Va
+00001850: 6c75 6554 7970 6520 2023 2032 0a0a 636c  lueType  # 2..cl
+00001860: 6173 7320 4e6f 7469 6669 6361 7469 6f6e  ass Notification
+00001870: 536f 7572 6365 285f 4e6f 7469 6669 6361  Source(_Notifica
+00001880: 7469 6f6e 536f 7572 6365 2c20 6d65 7461  tionSource, meta
+00001890: 636c 6173 733d 5f4e 6f74 6966 6963 6174  class=_Notificat
+000018a0: 696f 6e53 6f75 7263 6545 6e75 6d54 7970  ionSourceEnumTyp
+000018b0: 6557 7261 7070 6572 293a 202e 2e2e 0a0a  eWrapper): .....
+000018c0: 554e 5345 543a 204e 6f74 6966 6963 6174  UNSET: Notificat
+000018d0: 696f 6e53 6f75 7263 652e 5661 6c75 6554  ionSource.ValueT
+000018e0: 7970 6520 2023 2030 0a57 5249 5445 523a  ype  # 0.WRITER:
+000018f0: 204e 6f74 6966 6963 6174 696f 6e53 6f75   NotificationSou
+00001900: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
+00001910: 2031 0a50 524f 4345 5353 4f52 3a20 4e6f   1.PROCESSOR: No
+00001920: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
+00001930: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+00001940: 676c 6f62 616c 5f5f 5f4e 6f74 6966 6963  global___Notific
+00001950: 6174 696f 6e53 6f75 7263 6520 3d20 4e6f  ationSource = No
+00001960: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
+00001970: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
+00001980: 636c 6173 7320 4175 6469 7428 676f 6f67  class Audit(goog
+00001990: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+000019a0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+000019b0: 2020 2222 2257 6520 7265 6365 6976 6520    """We receive 
+000019c0: 7468 6973 2069 6e66 6f72 6d61 7469 6f6e  this information
+000019d0: 2074 6872 6f77 2061 6e20 7374 7265 616d   throw an stream
+000019e0: 2073 7973 7465 6d22 2222 0a0a 2020 2020   system"""..    
+000019f0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+00001a00: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+00001a10: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
+00001a20: 720a 0a20 2020 2063 6c61 7373 205f 536f  r..    class _So
+00001a30: 7572 6365 3a0a 2020 2020 2020 2020 5661  urce:.        Va
+00001a40: 6c75 6554 7970 6520 3d20 7479 7069 6e67  lueType = typing
+00001a50: 2e4e 6577 5479 7065 2822 5661 6c75 6554  .NewType("ValueT
+00001a60: 7970 6522 2c20 6275 696c 7469 6e73 2e69  ype", builtins.i
+00001a70: 6e74 290a 2020 2020 2020 2020 563a 2074  nt).        V: t
+00001a80: 7970 696e 675f 6578 7465 6e73 696f 6e73  yping_extensions
+00001a90: 2e54 7970 6541 6c69 6173 203d 2056 616c  .TypeAlias = Val
+00001aa0: 7565 5479 7065 0a0a 2020 2020 636c 6173  ueType..    clas
+00001ab0: 7320 5f53 6f75 7263 6545 6e75 6d54 7970  s _SourceEnumTyp
+00001ac0: 6557 7261 7070 6572 2867 6f6f 676c 652e  eWrapper(google.
+00001ad0: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
+00001ae0: 6c2e 656e 756d 5f74 7970 655f 7772 6170  l.enum_type_wrap
+00001af0: 7065 722e 5f45 6e75 6d54 7970 6557 7261  per._EnumTypeWra
+00001b00: 7070 6572 5b41 7564 6974 2e5f 536f 7572  pper[Audit._Sour
+00001b10: 6365 2e56 616c 7565 5479 7065 5d2c 2062  ce.ValueType], b
+00001b20: 7569 6c74 696e 732e 7479 7065 293a 0a20  uiltins.type):. 
+00001b30: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
+00001b40: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
+00001b50: 7566 2e64 6573 6372 6970 746f 722e 456e  uf.descriptor.En
+00001b60: 756d 4465 7363 7269 7074 6f72 0a20 2020  umDescriptor.   
+00001b70: 2020 2020 2048 5454 503a 2041 7564 6974       HTTP: Audit
+00001b80: 2e5f 536f 7572 6365 2e56 616c 7565 5479  ._Source.ValueTy
+00001b90: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
+00001ba0: 4441 5348 424f 4152 443a 2041 7564 6974  DASHBOARD: Audit
+00001bb0: 2e5f 536f 7572 6365 2e56 616c 7565 5479  ._Source.ValueTy
+00001bc0: 7065 2020 2320 310a 2020 2020 2020 2020  pe  # 1.        
+00001bd0: 4445 534b 544f 503a 2041 7564 6974 2e5f  DESKTOP: Audit._
+00001be0: 536f 7572 6365 2e56 616c 7565 5479 7065  Source.ValueType
+00001bf0: 2020 2320 320a 0a20 2020 2063 6c61 7373    # 2..    class
+00001c00: 2053 6f75 7263 6528 5f53 6f75 7263 652c   Source(_Source,
+00001c10: 206d 6574 6163 6c61 7373 3d5f 536f 7572   metaclass=_Sour
+00001c20: 6365 456e 756d 5479 7065 5772 6170 7065  ceEnumTypeWrappe
+00001c30: 7229 3a20 2e2e 2e0a 2020 2020 4854 5450  r): ....    HTTP
+00001c40: 3a20 4175 6469 742e 536f 7572 6365 2e56  : Audit.Source.V
+00001c50: 616c 7565 5479 7065 2020 2320 300a 2020  alueType  # 0.  
+00001c60: 2020 4441 5348 424f 4152 443a 2041 7564    DASHBOARD: Aud
+00001c70: 6974 2e53 6f75 7263 652e 5661 6c75 6554  it.Source.ValueT
+00001c80: 7970 6520 2023 2031 0a20 2020 2044 4553  ype  # 1.    DES
+00001c90: 4b54 4f50 3a20 4175 6469 742e 536f 7572  KTOP: Audit.Sour
+00001ca0: 6365 2e56 616c 7565 5479 7065 2020 2320  ce.ValueType  # 
+00001cb0: 320a 0a20 2020 2055 5345 525f 4649 454c  2..    USER_FIEL
+00001cc0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00001cd0: 6e73 2e69 6e74 0a20 2020 2057 4845 4e5f  ns.int.    WHEN_
 00001ce0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00001cf0: 696c 7469 6e73 2e69 6e74 0a20 2020 2053  iltins.int.    S
-00001d00: 4f55 5243 455f 4649 454c 445f 4e55 4d42  OURCE_FIELD_NUMB
+00001cf0: 696c 7469 6e73 2e69 6e74 0a20 2020 204f  iltins.int.    O
+00001d00: 5249 4749 4e5f 4649 454c 445f 4e55 4d42  RIGIN_FIELD_NUMB
 00001d10: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00001d20: 0a20 2020 204b 4249 445f 4649 454c 445f  .    KBID_FIELD_
-00001d30: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00001d40: 2e69 6e74 0a20 2020 2055 5549 445f 4649  .int.    UUID_FI
-00001d50: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-00001d60: 7469 6e73 2e69 6e74 0a20 2020 204d 4553  tins.int.    MES
-00001d70: 5341 4745 5f53 4f55 5243 455f 4649 454c  SAGE_SOURCE_FIEL
-00001d80: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00001d90: 6e73 2e69 6e74 0a20 2020 2046 4945 4c44  ns.int.    FIELD
-00001da0: 5f4d 4554 4144 4154 415f 4649 454c 445f  _METADATA_FIELD_
-00001db0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00001dc0: 2e69 6e74 0a20 2020 2041 5544 4954 5f46  .int.    AUDIT_F
-00001dd0: 4945 4c44 535f 4649 454c 445f 4e55 4d42  IELDS_FIELD_NUMB
-00001de0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00001df0: 0a20 2020 2075 7365 723a 2062 7569 6c74  .    user: built
-00001e00: 696e 732e 7374 720a 2020 2020 6f72 6967  ins.str.    orig
-00001e10: 696e 3a20 6275 696c 7469 6e73 2e73 7472  in: builtins.str
-00001e20: 0a20 2020 2073 6f75 7263 653a 2067 6c6f  .    source: glo
-00001e30: 6261 6c5f 5f5f 4175 6469 742e 536f 7572  bal___Audit.Sour
-00001e40: 6365 2e56 616c 7565 5479 7065 0a20 2020  ce.ValueType.   
-00001e50: 206b 6269 643a 2062 7569 6c74 696e 732e   kbid: builtins.
-00001e60: 7374 720a 2020 2020 7575 6964 3a20 6275  str.    uuid: bu
-00001e70: 696c 7469 6e73 2e73 7472 0a20 2020 206d  iltins.str.    m
-00001e80: 6573 7361 6765 5f73 6f75 7263 653a 2067  essage_source: g
-00001e90: 6c6f 6261 6c5f 5f5f 4272 6f6b 6572 4d65  lobal___BrokerMe
-00001ea0: 7373 6167 652e 4d65 7373 6167 6553 6f75  ssage.MessageSou
-00001eb0: 7263 652e 5661 6c75 6554 7970 650a 2020  rce.ValueType.  
-00001ec0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00001ed0: 6465 6620 7768 656e 2873 656c 6629 202d  def when(self) -
-00001ee0: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
-00001ef0: 662e 7469 6d65 7374 616d 705f 7062 322e  f.timestamp_pb2.
-00001f00: 5469 6d65 7374 616d 703a 202e 2e2e 0a20  Timestamp: .... 
-00001f10: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00001f20: 2064 6566 2066 6965 6c64 5f6d 6574 6164   def field_metad
-00001f30: 6174 6128 7365 6c66 2920 2d3e 2067 6f6f  ata(self) -> goo
-00001f40: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-00001f50: 6572 6e61 6c2e 636f 6e74 6169 6e65 7273  ernal.containers
-00001f60: 2e52 6570 6561 7465 6443 6f6d 706f 7369  .RepeatedComposi
-00001f70: 7465 4669 656c 6443 6f6e 7461 696e 6572  teFieldContainer
-00001f80: 5b6e 7563 6c69 6164 625f 7072 6f74 6f73  [nucliadb_protos
-00001f90: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00001fa0: 6965 6c64 4944 5d3a 202e 2e2e 0a20 2020  ieldID]: ....   
-00001fb0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00001fc0: 6566 2061 7564 6974 5f66 6965 6c64 7328  ef audit_fields(
-00001fd0: 7365 6c66 2920 2d3e 2067 6f6f 676c 652e  self) -> google.
-00001fe0: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
-00001ff0: 6c2e 636f 6e74 6169 6e65 7273 2e52 6570  l.containers.Rep
-00002000: 6561 7465 6443 6f6d 706f 7369 7465 4669  eatedCompositeFi
-00002010: 656c 6443 6f6e 7461 696e 6572 5b6e 7563  eldContainer[nuc
-00002020: 6c69 6164 625f 7072 6f74 6f73 2e61 7564  liadb_protos.aud
-00002030: 6974 5f70 6232 2e41 7564 6974 4669 656c  it_pb2.AuditFiel
-00002040: 645d 3a20 2e2e 2e0a 2020 2020 6465 6620  d]: ....    def 
-00002050: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00002060: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00002070: 2a2c 0a20 2020 2020 2020 2075 7365 723a  *,.        user:
-00002080: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-00002090: 2e2e 2e2c 0a20 2020 2020 2020 2077 6865  ...,.        whe
-000020a0: 6e3a 2067 6f6f 676c 652e 7072 6f74 6f62  n: google.protob
-000020b0: 7566 2e74 696d 6573 7461 6d70 5f70 6232  uf.timestamp_pb2
-000020c0: 2e54 696d 6573 7461 6d70 207c 204e 6f6e  .Timestamp | Non
-000020d0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-000020e0: 206f 7269 6769 6e3a 2062 7569 6c74 696e   origin: builtin
-000020f0: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-00002100: 2020 2020 2073 6f75 7263 653a 2067 6c6f       source: glo
-00002110: 6261 6c5f 5f5f 4175 6469 742e 536f 7572  bal___Audit.Sour
-00002120: 6365 2e56 616c 7565 5479 7065 203d 202e  ce.ValueType = .
-00002130: 2e2e 2c0a 2020 2020 2020 2020 6b62 6964  ..,.        kbid
-00002140: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00002150: 202e 2e2e 2c0a 2020 2020 2020 2020 7575   ...,.        uu
-00002160: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
-00002170: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00002180: 6d65 7373 6167 655f 736f 7572 6365 3a20  message_source: 
-00002190: 676c 6f62 616c 5f5f 5f42 726f 6b65 724d  global___BrokerM
-000021a0: 6573 7361 6765 2e4d 6573 7361 6765 536f  essage.MessageSo
-000021b0: 7572 6365 2e56 616c 7565 5479 7065 203d  urce.ValueType =
-000021c0: 202e 2e2e 2c0a 2020 2020 2020 2020 6669   ...,.        fi
-000021d0: 656c 645f 6d65 7461 6461 7461 3a20 636f  eld_metadata: co
-000021e0: 6c6c 6563 7469 6f6e 732e 6162 632e 4974  llections.abc.It
-000021f0: 6572 6162 6c65 5b6e 7563 6c69 6164 625f  erable[nucliadb_
-00002200: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
-00002210: 5f70 6232 2e46 6965 6c64 4944 5d20 7c20  _pb2.FieldID] | 
-00002220: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-00002230: 2020 2020 6175 6469 745f 6669 656c 6473      audit_fields
-00002240: 3a20 636f 6c6c 6563 7469 6f6e 732e 6162  : collections.ab
-00002250: 632e 4974 6572 6162 6c65 5b6e 7563 6c69  c.Iterable[nucli
-00002260: 6164 625f 7072 6f74 6f73 2e61 7564 6974  adb_protos.audit
-00002270: 5f70 6232 2e41 7564 6974 4669 656c 645d  _pb2.AuditField]
-00002280: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-00002290: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-000022a0: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
-000022b0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-000022c0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-000022d0: 7261 6c5b 2277 6865 6e22 2c20 6222 7768  ral["when", b"wh
-000022e0: 656e 225d 2920 2d3e 2062 7569 6c74 696e  en"]) -> builtin
-000022f0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
-00002300: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-00002310: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00002320: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00002330: 2261 7564 6974 5f66 6965 6c64 7322 2c20  "audit_fields", 
-00002340: 6222 6175 6469 745f 6669 656c 6473 222c  b"audit_fields",
-00002350: 2022 6669 656c 645f 6d65 7461 6461 7461   "field_metadata
-00002360: 222c 2062 2266 6965 6c64 5f6d 6574 6164  ", b"field_metad
-00002370: 6174 6122 2c20 226b 6269 6422 2c20 6222  ata", "kbid", b"
-00002380: 6b62 6964 222c 2022 6d65 7373 6167 655f  kbid", "message_
-00002390: 736f 7572 6365 222c 2062 226d 6573 7361  source", b"messa
-000023a0: 6765 5f73 6f75 7263 6522 2c20 226f 7269  ge_source", "ori
-000023b0: 6769 6e22 2c20 6222 6f72 6967 696e 222c  gin", b"origin",
-000023c0: 2022 736f 7572 6365 222c 2062 2273 6f75   "source", b"sou
-000023d0: 7263 6522 2c20 2275 7365 7222 2c20 6222  rce", "user", b"
-000023e0: 7573 6572 222c 2022 7575 6964 222c 2062  user", "uuid", b
-000023f0: 2275 7569 6422 2c20 2277 6865 6e22 2c20  "uuid", "when", 
-00002400: 6222 7768 656e 225d 2920 2d3e 204e 6f6e  b"when"]) -> Non
-00002410: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
-00002420: 5f41 7564 6974 203d 2041 7564 6974 0a0a  _Audit = Audit..
-00002430: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
-00002440: 6173 7320 4572 726f 7228 676f 6f67 6c65  ass Error(google
-00002450: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
-00002460: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
-00002470: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-00002480: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-00002490: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-000024a0: 720a 0a20 2020 2063 6c61 7373 205f 4572  r..    class _Er
-000024b0: 726f 7243 6f64 653a 0a20 2020 2020 2020  rorCode:.       
-000024c0: 2056 616c 7565 5479 7065 203d 2074 7970   ValueType = typ
-000024d0: 696e 672e 4e65 7754 7970 6528 2256 616c  ing.NewType("Val
-000024e0: 7565 5479 7065 222c 2062 7569 6c74 696e  ueType", builtin
-000024f0: 732e 696e 7429 0a20 2020 2020 2020 2056  s.int).        V
-00002500: 3a20 7479 7069 6e67 5f65 7874 656e 7369  : typing_extensi
-00002510: 6f6e 732e 5479 7065 416c 6961 7320 3d20  ons.TypeAlias = 
-00002520: 5661 6c75 6554 7970 650a 0a20 2020 2063  ValueType..    c
-00002530: 6c61 7373 205f 4572 726f 7243 6f64 6545  lass _ErrorCodeE
-00002540: 6e75 6d54 7970 6557 7261 7070 6572 2867  numTypeWrapper(g
-00002550: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
-00002560: 6e74 6572 6e61 6c2e 656e 756d 5f74 7970  nternal.enum_typ
-00002570: 655f 7772 6170 7065 722e 5f45 6e75 6d54  e_wrapper._EnumT
-00002580: 7970 6557 7261 7070 6572 5b45 7272 6f72  ypeWrapper[Error
-00002590: 2e5f 4572 726f 7243 6f64 652e 5661 6c75  ._ErrorCode.Valu
-000025a0: 6554 7970 655d 2c20 6275 696c 7469 6e73  eType], builtins
-000025b0: 2e74 7970 6529 3a0a 2020 2020 2020 2020  .type):.        
-000025c0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-000025d0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-000025e0: 7269 7074 6f72 2e45 6e75 6d44 6573 6372  riptor.EnumDescr
-000025f0: 6970 746f 720a 2020 2020 2020 2020 4745  iptor.        GE
-00002600: 4e45 5249 433a 2045 7272 6f72 2e5f 4572  NERIC: Error._Er
-00002610: 726f 7243 6f64 652e 5661 6c75 6554 7970  rorCode.ValueTyp
-00002620: 6520 2023 2030 0a20 2020 2020 2020 2045  e  # 0.        E
-00002630: 5854 5241 4354 3a20 4572 726f 722e 5f45  XTRACT: Error._E
-00002640: 7272 6f72 436f 6465 2e56 616c 7565 5479  rrorCode.ValueTy
-00002650: 7065 2020 2320 310a 2020 2020 2020 2020  pe  # 1.        
-00002660: 5052 4f43 4553 533a 2045 7272 6f72 2e5f  PROCESS: Error._
-00002670: 4572 726f 7243 6f64 652e 5661 6c75 6554  ErrorCode.ValueT
-00002680: 7970 6520 2023 2032 0a0a 2020 2020 636c  ype  # 2..    cl
-00002690: 6173 7320 4572 726f 7243 6f64 6528 5f45  ass ErrorCode(_E
-000026a0: 7272 6f72 436f 6465 2c20 6d65 7461 636c  rrorCode, metacl
-000026b0: 6173 733d 5f45 7272 6f72 436f 6465 456e  ass=_ErrorCodeEn
-000026c0: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
-000026d0: 2e2e 2e0a 2020 2020 4745 4e45 5249 433a  ....    GENERIC:
-000026e0: 2045 7272 6f72 2e45 7272 6f72 436f 6465   Error.ErrorCode
-000026f0: 2e56 616c 7565 5479 7065 2020 2320 300a  .ValueType  # 0.
-00002700: 2020 2020 4558 5452 4143 543a 2045 7272      EXTRACT: Err
-00002710: 6f72 2e45 7272 6f72 436f 6465 2e56 616c  or.ErrorCode.Val
-00002720: 7565 5479 7065 2020 2320 310a 2020 2020  ueType  # 1.    
-00002730: 5052 4f43 4553 533a 2045 7272 6f72 2e45  PROCESS: Error.E
-00002740: 7272 6f72 436f 6465 2e56 616c 7565 5479  rrorCode.ValueTy
-00002750: 7065 2020 2320 320a 0a20 2020 2046 4945  pe  # 2..    FIE
-00002760: 4c44 5f46 4945 4c44 5f4e 554d 4245 523a  LD_FIELD_NUMBER:
-00002770: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00002780: 2020 4649 454c 445f 5459 5045 5f46 4945    FIELD_TYPE_FIE
-00002790: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-000027a0: 696e 732e 696e 740a 2020 2020 4552 524f  ins.int.    ERRO
-000027b0: 525f 4649 454c 445f 4e55 4d42 4552 3a20  R_FIELD_NUMBER: 
-000027c0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-000027d0: 2043 4f44 455f 4649 454c 445f 4e55 4d42   CODE_FIELD_NUMB
-000027e0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-000027f0: 0a20 2020 2066 6965 6c64 3a20 6275 696c  .    field: buil
-00002800: 7469 6e73 2e73 7472 0a20 2020 2066 6965  tins.str.    fie
-00002810: 6c64 5f74 7970 653a 206e 7563 6c69 6164  ld_type: nucliad
-00002820: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
-00002830: 6573 5f70 6232 2e46 6965 6c64 5479 7065  es_pb2.FieldType
-00002840: 2e56 616c 7565 5479 7065 0a20 2020 2065  .ValueType.    e
-00002850: 7272 6f72 3a20 6275 696c 7469 6e73 2e73  rror: builtins.s
-00002860: 7472 0a20 2020 2063 6f64 653a 2067 6c6f  tr.    code: glo
-00002870: 6261 6c5f 5f5f 4572 726f 722e 4572 726f  bal___Error.Erro
-00002880: 7243 6f64 652e 5661 6c75 6554 7970 650a  rCode.ValueType.
-00002890: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000028a0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000028b0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-000028c0: 2020 2066 6965 6c64 3a20 6275 696c 7469     field: builti
-000028d0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-000028e0: 2020 2020 2020 6669 656c 645f 7479 7065        field_type
-000028f0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-00002900: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-00002910: 4669 656c 6454 7970 652e 5661 6c75 6554  FieldType.ValueT
-00002920: 7970 6520 3d20 2e2e 2e2c 0a20 2020 2020  ype = ...,.     
-00002930: 2020 2065 7272 6f72 3a20 6275 696c 7469     error: builti
-00002940: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00002950: 2020 2020 2020 636f 6465 3a20 676c 6f62        code: glob
-00002960: 616c 5f5f 5f45 7272 6f72 2e45 7272 6f72  al___Error.Error
-00002970: 436f 6465 2e56 616c 7565 5479 7065 203d  Code.ValueType =
-00002980: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-00002990: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-000029a0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-000029b0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-000029c0: 7069 6e67 2e4c 6974 6572 616c 5b22 636f  ping.Literal["co
-000029d0: 6465 222c 2062 2263 6f64 6522 2c20 2265  de", b"code", "e
-000029e0: 7272 6f72 222c 2062 2265 7272 6f72 222c  rror", b"error",
-000029f0: 2022 6669 656c 6422 2c20 6222 6669 656c   "field", b"fiel
-00002a00: 6422 2c20 2266 6965 6c64 5f74 7970 6522  d", "field_type"
-00002a10: 2c20 6222 6669 656c 645f 7479 7065 225d  , b"field_type"]
-00002a20: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
-00002a30: 676c 6f62 616c 5f5f 5f45 7272 6f72 203d  global___Error =
-00002a40: 2045 7272 6f72 0a0a 4074 7970 696e 672e   Error..@typing.
-00002a50: 6669 6e61 6c0a 636c 6173 7320 4272 6f6b  final.class Brok
-00002a60: 6572 4d65 7373 6167 6528 676f 6f67 6c65  erMessage(google
-00002a70: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
-00002a80: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
-00002a90: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-00002aa0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-00002ab0: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-00002ac0: 720a 0a20 2020 2063 6c61 7373 205f 4d65  r..    class _Me
-00002ad0: 7373 6167 6554 7970 653a 0a20 2020 2020  ssageType:.     
-00002ae0: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
-00002af0: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
-00002b00: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
-00002b10: 696e 732e 696e 7429 0a20 2020 2020 2020  ins.int).       
-00002b20: 2056 3a20 7479 7069 6e67 5f65 7874 656e   V: typing_exten
-00002b30: 7369 6f6e 732e 5479 7065 416c 6961 7320  sions.TypeAlias 
-00002b40: 3d20 5661 6c75 6554 7970 650a 0a20 2020  = ValueType..   
-00002b50: 2063 6c61 7373 205f 4d65 7373 6167 6554   class _MessageT
-00002b60: 7970 6545 6e75 6d54 7970 6557 7261 7070  ypeEnumTypeWrapp
-00002b70: 6572 2867 6f6f 676c 652e 7072 6f74 6f62  er(google.protob
-00002b80: 7566 2e69 6e74 6572 6e61 6c2e 656e 756d  uf.internal.enum
-00002b90: 5f74 7970 655f 7772 6170 7065 722e 5f45  _type_wrapper._E
-00002ba0: 6e75 6d54 7970 6557 7261 7070 6572 5b42  numTypeWrapper[B
-00002bb0: 726f 6b65 724d 6573 7361 6765 2e5f 4d65  rokerMessage._Me
-00002bc0: 7373 6167 6554 7970 652e 5661 6c75 6554  ssageType.ValueT
-00002bd0: 7970 655d 2c20 6275 696c 7469 6e73 2e74  ype], builtins.t
-00002be0: 7970 6529 3a0a 2020 2020 2020 2020 4445  ype):.        DE
-00002bf0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00002c00: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00002c10: 7074 6f72 2e45 6e75 6d44 6573 6372 6970  ptor.EnumDescrip
-00002c20: 746f 720a 2020 2020 2020 2020 4155 544f  tor.        AUTO
-00002c30: 434f 4d4d 4954 3a20 4272 6f6b 6572 4d65  COMMIT: BrokerMe
-00002c40: 7373 6167 652e 5f4d 6573 7361 6765 5479  ssage._MessageTy
-00002c50: 7065 2e56 616c 7565 5479 7065 2020 2320  pe.ValueType  # 
-00002c60: 300a 2020 2020 2020 2020 4d55 4c54 493a  0.        MULTI:
-00002c70: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
-00002c80: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
-00002c90: 6554 7970 6520 2023 2031 0a20 2020 2020  eType  # 1.     
-00002ca0: 2020 2043 4f4d 4d49 543a 2042 726f 6b65     COMMIT: Broke
-00002cb0: 724d 6573 7361 6765 2e5f 4d65 7373 6167  rMessage._Messag
-00002cc0: 6554 7970 652e 5661 6c75 6554 7970 6520  eType.ValueType 
-00002cd0: 2023 2032 0a20 2020 2020 2020 2052 4f4c   # 2.        ROL
-00002ce0: 4c42 4143 4b3a 2042 726f 6b65 724d 6573  LBACK: BrokerMes
-00002cf0: 7361 6765 2e5f 4d65 7373 6167 6554 7970  sage._MessageTyp
-00002d00: 652e 5661 6c75 6554 7970 6520 2023 2033  e.ValueType  # 3
-00002d10: 0a20 2020 2020 2020 2044 454c 4554 453a  .        DELETE:
-00002d20: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
-00002d30: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
-00002d40: 6554 7970 6520 2023 2034 0a0a 2020 2020  eType  # 4..    
-00002d50: 636c 6173 7320 4d65 7373 6167 6554 7970  class MessageTyp
-00002d60: 6528 5f4d 6573 7361 6765 5479 7065 2c20  e(_MessageType, 
-00002d70: 6d65 7461 636c 6173 733d 5f4d 6573 7361  metaclass=_Messa
-00002d80: 6765 5479 7065 456e 756d 5479 7065 5772  geTypeEnumTypeWr
-00002d90: 6170 7065 7229 3a20 2e2e 2e0a 2020 2020  apper): ....    
-00002da0: 4155 544f 434f 4d4d 4954 3a20 4272 6f6b  AUTOCOMMIT: Brok
-00002db0: 6572 4d65 7373 6167 652e 4d65 7373 6167  erMessage.Messag
-00002dc0: 6554 7970 652e 5661 6c75 6554 7970 6520  eType.ValueType 
-00002dd0: 2023 2030 0a20 2020 204d 554c 5449 3a20   # 0.    MULTI: 
-00002de0: 4272 6f6b 6572 4d65 7373 6167 652e 4d65  BrokerMessage.Me
-00002df0: 7373 6167 6554 7970 652e 5661 6c75 6554  ssageType.ValueT
-00002e00: 7970 6520 2023 2031 0a20 2020 2043 4f4d  ype  # 1.    COM
-00002e10: 4d49 543a 2042 726f 6b65 724d 6573 7361  MIT: BrokerMessa
-00002e20: 6765 2e4d 6573 7361 6765 5479 7065 2e56  ge.MessageType.V
-00002e30: 616c 7565 5479 7065 2020 2320 320a 2020  alueType  # 2.  
-00002e40: 2020 524f 4c4c 4241 434b 3a20 4272 6f6b    ROLLBACK: Brok
-00002e50: 6572 4d65 7373 6167 652e 4d65 7373 6167  erMessage.Messag
-00002e60: 6554 7970 652e 5661 6c75 6554 7970 6520  eType.ValueType 
-00002e70: 2023 2033 0a20 2020 2044 454c 4554 453a   # 3.    DELETE:
-00002e80: 2042 726f 6b65 724d 6573 7361 6765 2e4d   BrokerMessage.M
-00002e90: 6573 7361 6765 5479 7065 2e56 616c 7565  essageType.Value
-00002ea0: 5479 7065 2020 2320 340a 0a20 2020 2063  Type  # 4..    c
-00002eb0: 6c61 7373 205f 4d65 7373 6167 6553 6f75  lass _MessageSou
-00002ec0: 7263 653a 0a20 2020 2020 2020 2056 616c  rce:.        Val
-00002ed0: 7565 5479 7065 203d 2074 7970 696e 672e  ueType = typing.
-00002ee0: 4e65 7754 7970 6528 2256 616c 7565 5479  NewType("ValueTy
-00002ef0: 7065 222c 2062 7569 6c74 696e 732e 696e  pe", builtins.in
-00002f00: 7429 0a20 2020 2020 2020 2056 3a20 7479  t).        V: ty
-00002f10: 7069 6e67 5f65 7874 656e 7369 6f6e 732e  ping_extensions.
-00002f20: 5479 7065 416c 6961 7320 3d20 5661 6c75  TypeAlias = Valu
-00002f30: 6554 7970 650a 0a20 2020 2063 6c61 7373  eType..    class
-00002f40: 205f 4d65 7373 6167 6553 6f75 7263 6545   _MessageSourceE
-00002f50: 6e75 6d54 7970 6557 7261 7070 6572 2867  numTypeWrapper(g
-00002f60: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
-00002f70: 6e74 6572 6e61 6c2e 656e 756d 5f74 7970  nternal.enum_typ
-00002f80: 655f 7772 6170 7065 722e 5f45 6e75 6d54  e_wrapper._EnumT
-00002f90: 7970 6557 7261 7070 6572 5b42 726f 6b65  ypeWrapper[Broke
-00002fa0: 724d 6573 7361 6765 2e5f 4d65 7373 6167  rMessage._Messag
-00002fb0: 6553 6f75 7263 652e 5661 6c75 6554 7970  eSource.ValueTyp
-00002fc0: 655d 2c20 6275 696c 7469 6e73 2e74 7970  e], builtins.typ
-00002fd0: 6529 3a0a 2020 2020 2020 2020 4445 5343  e):.        DESC
-00002fe0: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
-00002ff0: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
-00003000: 6f72 2e45 6e75 6d44 6573 6372 6970 746f  or.EnumDescripto
-00003010: 720a 2020 2020 2020 2020 5752 4954 4552  r.        WRITER
-00003020: 3a20 4272 6f6b 6572 4d65 7373 6167 652e  : BrokerMessage.
-00003030: 5f4d 6573 7361 6765 536f 7572 6365 2e56  _MessageSource.V
-00003040: 616c 7565 5479 7065 2020 2320 300a 2020  alueType  # 0.  
-00003050: 2020 2020 2020 5052 4f43 4553 534f 523a        PROCESSOR:
-00003060: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
-00003070: 4d65 7373 6167 6553 6f75 7263 652e 5661  MessageSource.Va
-00003080: 6c75 6554 7970 6520 2023 2031 0a0a 2020  lueType  # 1..  
-00003090: 2020 636c 6173 7320 4d65 7373 6167 6553    class MessageS
-000030a0: 6f75 7263 6528 5f4d 6573 7361 6765 536f  ource(_MessageSo
-000030b0: 7572 6365 2c20 6d65 7461 636c 6173 733d  urce, metaclass=
-000030c0: 5f4d 6573 7361 6765 536f 7572 6365 456e  _MessageSourceEn
-000030d0: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
-000030e0: 2e2e 2e0a 2020 2020 5752 4954 4552 3a20  ....    WRITER: 
-000030f0: 4272 6f6b 6572 4d65 7373 6167 652e 4d65  BrokerMessage.Me
-00003100: 7373 6167 6553 6f75 7263 652e 5661 6c75  ssageSource.Valu
-00003110: 6554 7970 6520 2023 2030 0a20 2020 2050  eType  # 0.    P
-00003120: 524f 4345 5353 4f52 3a20 4272 6f6b 6572  ROCESSOR: Broker
-00003130: 4d65 7373 6167 652e 4d65 7373 6167 6553  Message.MessageS
-00003140: 6f75 7263 652e 5661 6c75 6554 7970 6520  ource.ValueType 
-00003150: 2023 2031 0a0a 2020 2020 4074 7970 696e   # 1..    @typin
-00003160: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
-00003170: 7320 436f 6e76 6572 7361 7469 6f6e 7345  s ConversationsE
-00003180: 6e74 7279 2867 6f6f 676c 652e 7072 6f74  ntry(google.prot
-00003190: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-000031a0: 7361 6765 293a 0a20 2020 2020 2020 2044  sage):.        D
-000031b0: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
-000031c0: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
-000031d0: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
-000031e0: 0a0a 2020 2020 2020 2020 4b45 595f 4649  ..        KEY_FI
-000031f0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-00003200: 7469 6e73 2e69 6e74 0a20 2020 2020 2020  tins.int.       
-00003210: 2056 414c 5545 5f46 4945 4c44 5f4e 554d   VALUE_FIELD_NUM
-00003220: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00003230: 740a 2020 2020 2020 2020 6b65 793a 2062  t.        key: b
-00003240: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
-00003250: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00003260: 2020 2020 2020 6465 6620 7661 6c75 6528        def value(
-00003270: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-00003280: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
-00003290: 6573 5f70 6232 2e43 6f6e 7665 7273 6174  es_pb2.Conversat
-000032a0: 696f 6e3a 202e 2e2e 0a20 2020 2020 2020  ion: ....       
-000032b0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-000032c0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-000032d0: 0a20 2020 2020 2020 2020 2020 202a 2c0a  .            *,.
-000032e0: 2020 2020 2020 2020 2020 2020 6b65 793a              key:
-000032f0: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-00003300: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
-00003310: 2076 616c 7565 3a20 6e75 636c 6961 6462   value: nucliadb
-00003320: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-00003330: 735f 7062 322e 436f 6e76 6572 7361 7469  s_pb2.Conversati
-00003340: 6f6e 207c 204e 6f6e 6520 3d20 2e2e 2e2c  on | None = ...,
-00003350: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
-00003360: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
-00003370: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-00003380: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00003390: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
-000033a0: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
-000033b0: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-000033c0: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
-000033d0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-000033e0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-000033f0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00003400: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
-00003410: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
-00003420: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-00003430: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
-00003440: 616c 0a20 2020 2063 6c61 7373 204c 6179  al.    class Lay
-00003450: 6f75 7473 456e 7472 7928 676f 6f67 6c65  outsEntry(google
-00003460: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
-00003470: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
-00003480: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-00003490: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-000034a0: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-000034b0: 6970 746f 720a 0a20 2020 2020 2020 204b  iptor..        K
-000034c0: 4559 5f46 4945 4c44 5f4e 554d 4245 523a  EY_FIELD_NUMBER:
-000034d0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-000034e0: 2020 2020 2020 5641 4c55 455f 4649 454c        VALUE_FIEL
-000034f0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00003500: 6e73 2e69 6e74 0a20 2020 2020 2020 206b  ns.int.        k
-00003510: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
-00003520: 0a20 2020 2020 2020 2040 7072 6f70 6572  .        @proper
-00003530: 7479 0a20 2020 2020 2020 2064 6566 2076  ty.        def v
-00003540: 616c 7565 2873 656c 6629 202d 3e20 6e75  alue(self) -> nu
-00003550: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-00003560: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
-00003570: 644c 6179 6f75 743a 202e 2e2e 0a20 2020  dLayout: ....   
-00003580: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
-00003590: 5f28 0a20 2020 2020 2020 2020 2020 2073  _(.            s
-000035a0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-000035b0: 202a 2c0a 2020 2020 2020 2020 2020 2020   *,.            
-000035c0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
-000035d0: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
-000035e0: 2020 2020 2076 616c 7565 3a20 6e75 636c       value: nucl
-000035f0: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
-00003600: 7572 6365 735f 7062 322e 4669 656c 644c  urces_pb2.FieldL
-00003610: 6179 6f75 7420 7c20 4e6f 6e65 203d 202e  ayout | None = .
-00003620: 2e2e 2c0a 2020 2020 2020 2020 2920 2d3e  ..,.        ) ->
-00003630: 204e 6f6e 653a 202e 2e2e 0a20 2020 2020   None: ....     
-00003640: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
-00003650: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-00003660: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-00003670: 5b22 7661 6c75 6522 2c20 6222 7661 6c75  ["value", b"valu
-00003680: 6522 5d29 202d 3e20 6275 696c 7469 6e73  e"]) -> builtins
-00003690: 2e62 6f6f 6c3a 202e 2e2e 0a20 2020 2020  .bool: ....     
-000036a0: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-000036b0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-000036c0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-000036d0: 616c 5b22 6b65 7922 2c20 6222 6b65 7922  al["key", b"key"
-000036e0: 2c20 2276 616c 7565 222c 2062 2276 616c  , "value", b"val
-000036f0: 7565 225d 2920 2d3e 204e 6f6e 653a 202e  ue"]) -> None: .
-00003700: 2e2e 0a0a 2020 2020 4074 7970 696e 672e  ....    @typing.
-00003710: 6669 6e61 6c0a 2020 2020 636c 6173 7320  final.    class 
-00003720: 5465 7874 7345 6e74 7279 2867 6f6f 676c  TextsEntry(googl
-00003730: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-00003740: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-00003750: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
-00003760: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00003770: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-00003780: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
-00003790: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
-000037a0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-000037b0: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
-000037c0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-000037d0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
-000037e0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
-000037f0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
-00003800: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
-00003810: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
-00003820: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00003830: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
-00003840: 6c64 5465 7874 3a20 2e2e 2e0a 2020 2020  ldText: ....    
-00003850: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00003860: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00003870: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00003880: 2a2c 0a20 2020 2020 2020 2020 2020 206b  *,.            k
-00003890: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
-000038a0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-000038b0: 2020 2020 7661 6c75 653a 206e 7563 6c69      value: nucli
-000038c0: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
-000038d0: 7263 6573 5f70 6232 2e46 6965 6c64 5465  rces_pb2.FieldTe
-000038e0: 7874 207c 204e 6f6e 6520 3d20 2e2e 2e2c  xt | None = ...,
-000038f0: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
-00003900: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
-00003910: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-00003920: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00003930: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
-00003940: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
-00003950: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-00003960: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
-00003970: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-00003980: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00003990: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-000039a0: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
-000039b0: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
-000039c0: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-000039d0: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
-000039e0: 616c 0a20 2020 2063 6c61 7373 204b 6579  al.    class Key
-000039f0: 776f 7264 7365 7473 456e 7472 7928 676f  wordsetsEntry(go
-00003a00: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-00003a10: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-00003a20: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
-00003a30: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-00003a40: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-00003a50: 6573 6372 6970 746f 720a 0a20 2020 2020  escriptor..     
-00003a60: 2020 204b 4559 5f46 4945 4c44 5f4e 554d     KEY_FIELD_NUM
-00003a70: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00003a80: 740a 2020 2020 2020 2020 5641 4c55 455f  t.        VALUE_
-00003a90: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00003aa0: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
-00003ab0: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
-00003ac0: 2e73 7472 0a20 2020 2020 2020 2040 7072  .str.        @pr
-00003ad0: 6f70 6572 7479 0a20 2020 2020 2020 2064  operty.        d
-00003ae0: 6566 2076 616c 7565 2873 656c 6629 202d  ef value(self) -
-00003af0: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
-00003b00: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-00003b10: 4669 656c 644b 6579 776f 7264 7365 743a  FieldKeywordset:
-00003b20: 202e 2e2e 0a20 2020 2020 2020 2064 6566   ....        def
-00003b30: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00003b40: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00003b50: 2020 2020 2020 2020 202a 2c0a 2020 2020           *,.    
-00003b60: 2020 2020 2020 2020 6b65 793a 2062 7569          key: bui
-00003b70: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
-00003b80: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00003b90: 7565 3a20 6e75 636c 6961 6462 5f70 726f  ue: nucliadb_pro
-00003ba0: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-00003bb0: 322e 4669 656c 644b 6579 776f 7264 7365  2.FieldKeywordse
-00003bc0: 7420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  t | None = ...,.
-00003bd0: 2020 2020 2020 2020 2920 2d3e 204e 6f6e          ) -> Non
-00003be0: 653a 202e 2e2e 0a20 2020 2020 2020 2064  e: ....        d
-00003bf0: 6566 2048 6173 4669 656c 6428 7365 6c66  ef HasField(self
-00003c00: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00003c10: 7069 6e67 2e4c 6974 6572 616c 5b22 7661  ping.Literal["va
-00003c20: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
-00003c30: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
-00003c40: 6c3a 202e 2e2e 0a20 2020 2020 2020 2064  l: ....        d
-00003c50: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
-00003c60: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
-00003c70: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
-00003c80: 6b65 7922 2c20 6222 6b65 7922 2c20 2276  key", b"key", "v
-00003c90: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
-00003ca0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
-00003cb0: 2020 2020 4074 7970 696e 672e 6669 6e61      @typing.fina
-00003cc0: 6c0a 2020 2020 636c 6173 7320 4461 7465  l.    class Date
-00003cd0: 7469 6d65 7345 6e74 7279 2867 6f6f 676c  timesEntry(googl
-00003ce0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-00003cf0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-00003d00: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
-00003d10: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00003d20: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-00003d30: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
-00003d40: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
-00003d50: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00003d60: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
-00003d70: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00003d80: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
-00003d90: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
-00003da0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
-00003db0: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
-00003dc0: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
-00003dd0: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00003de0: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
-00003df0: 6c64 4461 7465 7469 6d65 3a20 2e2e 2e0a  ldDatetime: ....
-00003e00: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
-00003e10: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
-00003e20: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00003e30: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
-00003e40: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
-00003e50: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-00003e60: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
-00003e70: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00003e80: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
-00003e90: 6c64 4461 7465 7469 6d65 207c 204e 6f6e  ldDatetime | Non
-00003ea0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-00003eb0: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
-00003ec0: 2020 2020 2020 2020 6465 6620 4861 7346          def HasF
-00003ed0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00003ee0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00003ef0: 7465 7261 6c5b 2276 616c 7565 222c 2062  teral["value", b
-00003f00: 2276 616c 7565 225d 2920 2d3e 2062 7569  "value"]) -> bui
-00003f10: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
-00003f20: 2020 2020 2020 2020 6465 6620 436c 6561          def Clea
-00003f30: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-00003f40: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-00003f50: 4c69 7465 7261 6c5b 226b 6579 222c 2062  Literal["key", b
-00003f60: 226b 6579 222c 2022 7661 6c75 6522 2c20  "key", "value", 
-00003f70: 6222 7661 6c75 6522 5d29 202d 3e20 4e6f  b"value"]) -> No
-00003f80: 6e65 3a20 2e2e 2e0a 0a20 2020 2040 7479  ne: .....    @ty
-00003f90: 7069 6e67 2e66 696e 616c 0a20 2020 2063  ping.final.    c
-00003fa0: 6c61 7373 204c 696e 6b73 456e 7472 7928  lass LinksEntry(
-00003fb0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00003fc0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
-00003fd0: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
-00003fe0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-00003ff0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-00004000: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
-00004010: 2020 2020 204b 4559 5f46 4945 4c44 5f4e       KEY_FIELD_N
-00004020: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00004030: 696e 740a 2020 2020 2020 2020 5641 4c55  int.        VALU
-00004040: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
-00004050: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00004060: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
-00004070: 6e73 2e73 7472 0a20 2020 2020 2020 2040  ns.str.        @
-00004080: 7072 6f70 6572 7479 0a20 2020 2020 2020  property.       
-00004090: 2064 6566 2076 616c 7565 2873 656c 6629   def value(self)
-000040a0: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
-000040b0: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-000040c0: 322e 4669 656c 644c 696e 6b3a 202e 2e2e  2.FieldLink: ...
-000040d0: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
-000040e0: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
-000040f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00004100: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00004110: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
-00004120: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-00004130: 2020 2020 2020 2020 2076 616c 7565 3a20           value: 
-00004140: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00004150: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
-00004160: 656c 644c 696e 6b20 7c20 4e6f 6e65 203d  eldLink | None =
-00004170: 202e 2e2e 2c0a 2020 2020 2020 2020 2920   ...,.        ) 
-00004180: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
-00004190: 2020 2020 2064 6566 2048 6173 4669 656c       def HasFiel
-000041a0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-000041b0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-000041c0: 616c 5b22 7661 6c75 6522 2c20 6222 7661  al["value", b"va
-000041d0: 6c75 6522 5d29 202d 3e20 6275 696c 7469  lue"]) -> builti
-000041e0: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
-000041f0: 2020 2020 2064 6566 2043 6c65 6172 4669       def ClearFi
-00004200: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
-00004210: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
-00004220: 6572 616c 5b22 6b65 7922 2c20 6222 6b65  eral["key", b"ke
-00004230: 7922 2c20 2276 616c 7565 222c 2062 2276  y", "value", b"v
-00004240: 616c 7565 225d 2920 2d3e 204e 6f6e 653a  alue"]) -> None:
-00004250: 202e 2e2e 0a0a 2020 2020 4074 7970 696e   .....    @typin
-00004260: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
-00004270: 7320 4669 6c65 7345 6e74 7279 2867 6f6f  s FilesEntry(goo
-00004280: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-00004290: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-000042a0: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
-000042b0: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-000042c0: 7566 2e64 6573 6372 6970 746f 722e 4465  uf.descriptor.De
-000042d0: 7363 7269 7074 6f72 0a0a 2020 2020 2020  scriptor..      
-000042e0: 2020 4b45 595f 4649 454c 445f 4e55 4d42    KEY_FIELD_NUMB
-000042f0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00004300: 0a20 2020 2020 2020 2056 414c 5545 5f46  .        VALUE_F
-00004310: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00004320: 6c74 696e 732e 696e 740a 2020 2020 2020  ltins.int.      
-00004330: 2020 6b65 793a 2062 7569 6c74 696e 732e    key: builtins.
-00004340: 7374 720a 2020 2020 2020 2020 4070 726f  str.        @pro
-00004350: 7065 7274 790a 2020 2020 2020 2020 6465  perty.        de
-00004360: 6620 7661 6c75 6528 7365 6c66 2920 2d3e  f value(self) ->
-00004370: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00004380: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00004390: 6965 6c64 4669 6c65 3a20 2e2e 2e0a 2020  ieldFile: ....  
-000043a0: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
-000043b0: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
-000043c0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-000043d0: 2020 2a2c 0a20 2020 2020 2020 2020 2020    *,.           
-000043e0: 206b 6579 3a20 6275 696c 7469 6e73 2e73   key: builtins.s
-000043f0: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
-00004400: 2020 2020 2020 7661 6c75 653a 206e 7563        value: nuc
-00004410: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
-00004420: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
-00004430: 4669 6c65 207c 204e 6f6e 6520 3d20 2e2e  File | None = ..
-00004440: 2e2c 0a20 2020 2020 2020 2029 202d 3e20  .,.        ) -> 
-00004450: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 2020  None: ....      
-00004460: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
-00004470: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00004480: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00004490: 2276 616c 7565 222c 2062 2276 616c 7565  "value", b"value
-000044a0: 225d 2920 2d3e 2062 7569 6c74 696e 732e  "]) -> builtins.
-000044b0: 626f 6f6c 3a20 2e2e 2e0a 2020 2020 2020  bool: ....      
-000044c0: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
-000044d0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-000044e0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-000044f0: 6c5b 226b 6579 222c 2062 226b 6579 222c  l["key", b"key",
-00004500: 2022 7661 6c75 6522 2c20 6222 7661 6c75   "value", b"valu
-00004510: 6522 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  e"]) -> None: ..
-00004520: 2e0a 0a20 2020 204b 4249 445f 4649 454c  ...    KBID_FIEL
-00004530: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00004540: 6e73 2e69 6e74 0a20 2020 2055 5549 445f  ns.int.    UUID_
-00004550: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00004560: 696c 7469 6e73 2e69 6e74 0a20 2020 2053  iltins.int.    S
-00004570: 4c55 475f 4649 454c 445f 4e55 4d42 4552  LUG_FIELD_NUMBER
-00004580: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00004590: 2020 2041 5544 4954 5f46 4945 4c44 5f4e     AUDIT_FIELD_N
-000045a0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-000045b0: 696e 740a 2020 2020 5459 5045 5f46 4945  int.    TYPE_FIE
-000045c0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-000045d0: 696e 732e 696e 740a 2020 2020 4d55 4c54  ins.int.    MULT
-000045e0: 4949 445f 4649 454c 445f 4e55 4d42 4552  IID_FIELD_NUMBER
-000045f0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00004600: 2020 2042 4153 4943 5f46 4945 4c44 5f4e     BASIC_FIELD_N
-00004610: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00004620: 696e 740a 2020 2020 4f52 4947 494e 5f46  int.    ORIGIN_F
+00001d20: 0a20 2020 2053 4f55 5243 455f 4649 454c  .    SOURCE_FIEL
+00001d30: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00001d40: 6e73 2e69 6e74 0a20 2020 204b 4249 445f  ns.int.    KBID_
+00001d50: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00001d60: 696c 7469 6e73 2e69 6e74 0a20 2020 2055  iltins.int.    U
+00001d70: 5549 445f 4649 454c 445f 4e55 4d42 4552  UID_FIELD_NUMBER
+00001d80: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00001d90: 2020 204d 4553 5341 4745 5f53 4f55 5243     MESSAGE_SOURC
+00001da0: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
+00001db0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00001dc0: 2046 4945 4c44 5f4d 4554 4144 4154 415f   FIELD_METADATA_
+00001dd0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00001de0: 696c 7469 6e73 2e69 6e74 0a20 2020 2041  iltins.int.    A
+00001df0: 5544 4954 5f46 4945 4c44 535f 4649 454c  UDIT_FIELDS_FIEL
+00001e00: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00001e10: 6e73 2e69 6e74 0a20 2020 2075 7365 723a  ns.int.    user:
+00001e20: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
+00001e30: 2020 6f72 6967 696e 3a20 6275 696c 7469    origin: builti
+00001e40: 6e73 2e73 7472 0a20 2020 2073 6f75 7263  ns.str.    sourc
+00001e50: 653a 2067 6c6f 6261 6c5f 5f5f 4175 6469  e: global___Audi
+00001e60: 742e 536f 7572 6365 2e56 616c 7565 5479  t.Source.ValueTy
+00001e70: 7065 0a20 2020 206b 6269 643a 2062 7569  pe.    kbid: bui
+00001e80: 6c74 696e 732e 7374 720a 2020 2020 7575  ltins.str.    uu
+00001e90: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
+00001ea0: 0a20 2020 206d 6573 7361 6765 5f73 6f75  .    message_sou
+00001eb0: 7263 653a 2067 6c6f 6261 6c5f 5f5f 4272  rce: global___Br
+00001ec0: 6f6b 6572 4d65 7373 6167 652e 4d65 7373  okerMessage.Mess
+00001ed0: 6167 6553 6f75 7263 652e 5661 6c75 6554  ageSource.ValueT
+00001ee0: 7970 650a 2020 2020 4070 726f 7065 7274  ype.    @propert
+00001ef0: 790a 2020 2020 6465 6620 7768 656e 2873  y.    def when(s
+00001f00: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
+00001f10: 726f 746f 6275 662e 7469 6d65 7374 616d  rotobuf.timestam
+00001f20: 705f 7062 322e 5469 6d65 7374 616d 703a  p_pb2.Timestamp:
+00001f30: 202e 2e2e 0a20 2020 2040 7072 6f70 6572   ....    @proper
+00001f40: 7479 0a20 2020 2064 6566 2066 6965 6c64  ty.    def field
+00001f50: 5f6d 6574 6164 6174 6128 7365 6c66 2920  _metadata(self) 
+00001f60: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
+00001f70: 7566 2e69 6e74 6572 6e61 6c2e 636f 6e74  uf.internal.cont
+00001f80: 6169 6e65 7273 2e52 6570 6561 7465 6443  ainers.RepeatedC
+00001f90: 6f6d 706f 7369 7465 4669 656c 6443 6f6e  ompositeFieldCon
+00001fa0: 7461 696e 6572 5b6e 7563 6c69 6164 625f  tainer[nucliadb_
+00001fb0: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
+00001fc0: 5f70 6232 2e46 6965 6c64 4944 5d3a 202e  _pb2.FieldID]: .
+00001fd0: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00001fe0: 0a20 2020 2064 6566 2061 7564 6974 5f66  .    def audit_f
+00001ff0: 6965 6c64 7328 7365 6c66 2920 2d3e 2067  ields(self) -> g
+00002000: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
+00002010: 6e74 6572 6e61 6c2e 636f 6e74 6169 6e65  nternal.containe
+00002020: 7273 2e52 6570 6561 7465 6443 6f6d 706f  rs.RepeatedCompo
+00002030: 7369 7465 4669 656c 6443 6f6e 7461 696e  siteFieldContain
+00002040: 6572 5b6e 7563 6c69 6164 625f 7072 6f74  er[nucliadb_prot
+00002050: 6f73 2e61 7564 6974 5f70 6232 2e41 7564  os.audit_pb2.Aud
+00002060: 6974 4669 656c 645d 3a20 2e2e 2e0a 2020  itField]: ....  
+00002070: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00002080: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00002090: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+000020a0: 2075 7365 723a 2062 7569 6c74 696e 732e   user: builtins.
+000020b0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
+000020c0: 2020 2077 6865 6e3a 2067 6f6f 676c 652e     when: google.
+000020d0: 7072 6f74 6f62 7566 2e74 696d 6573 7461  protobuf.timesta
+000020e0: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
+000020f0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00002100: 2020 2020 2020 206f 7269 6769 6e3a 2062         origin: b
+00002110: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+00002120: 2e2c 0a20 2020 2020 2020 2073 6f75 7263  .,.        sourc
+00002130: 653a 2067 6c6f 6261 6c5f 5f5f 4175 6469  e: global___Audi
+00002140: 742e 536f 7572 6365 2e56 616c 7565 5479  t.Source.ValueTy
+00002150: 7065 203d 202e 2e2e 2c0a 2020 2020 2020  pe = ...,.      
+00002160: 2020 6b62 6964 3a20 6275 696c 7469 6e73    kbid: builtins
+00002170: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+00002180: 2020 2020 7575 6964 3a20 6275 696c 7469      uuid: builti
+00002190: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+000021a0: 2020 2020 2020 6d65 7373 6167 655f 736f        message_so
+000021b0: 7572 6365 3a20 676c 6f62 616c 5f5f 5f42  urce: global___B
+000021c0: 726f 6b65 724d 6573 7361 6765 2e4d 6573  rokerMessage.Mes
+000021d0: 7361 6765 536f 7572 6365 2e56 616c 7565  sageSource.Value
+000021e0: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
+000021f0: 2020 2020 6669 656c 645f 6d65 7461 6461      field_metada
+00002200: 7461 3a20 636f 6c6c 6563 7469 6f6e 732e  ta: collections.
+00002210: 6162 632e 4974 6572 6162 6c65 5b6e 7563  abc.Iterable[nuc
+00002220: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
+00002230: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
+00002240: 4944 5d20 7c20 4e6f 6e65 203d 202e 2e2e  ID] | None = ...
+00002250: 2c0a 2020 2020 2020 2020 6175 6469 745f  ,.        audit_
+00002260: 6669 656c 6473 3a20 636f 6c6c 6563 7469  fields: collecti
+00002270: 6f6e 732e 6162 632e 4974 6572 6162 6c65  ons.abc.Iterable
+00002280: 5b6e 7563 6c69 6164 625f 7072 6f74 6f73  [nucliadb_protos
+00002290: 2e61 7564 6974 5f70 6232 2e41 7564 6974  .audit_pb2.Audit
+000022a0: 4669 656c 645d 207c 204e 6f6e 6520 3d20  Field] | None = 
+000022b0: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
+000022c0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
+000022d0: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
+000022e0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+000022f0: 672e 4c69 7465 7261 6c5b 2277 6865 6e22  g.Literal["when"
+00002300: 2c20 6222 7768 656e 225d 2920 2d3e 2062  , b"when"]) -> b
+00002310: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
+00002320: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+00002330: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+00002340: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+00002350: 7465 7261 6c5b 2261 7564 6974 5f66 6965  teral["audit_fie
+00002360: 6c64 7322 2c20 6222 6175 6469 745f 6669  lds", b"audit_fi
+00002370: 656c 6473 222c 2022 6669 656c 645f 6d65  elds", "field_me
+00002380: 7461 6461 7461 222c 2062 2266 6965 6c64  tadata", b"field
+00002390: 5f6d 6574 6164 6174 6122 2c20 226b 6269  _metadata", "kbi
+000023a0: 6422 2c20 6222 6b62 6964 222c 2022 6d65  d", b"kbid", "me
+000023b0: 7373 6167 655f 736f 7572 6365 222c 2062  ssage_source", b
+000023c0: 226d 6573 7361 6765 5f73 6f75 7263 6522  "message_source"
+000023d0: 2c20 226f 7269 6769 6e22 2c20 6222 6f72  , "origin", b"or
+000023e0: 6967 696e 222c 2022 736f 7572 6365 222c  igin", "source",
+000023f0: 2062 2273 6f75 7263 6522 2c20 2275 7365   b"source", "use
+00002400: 7222 2c20 6222 7573 6572 222c 2022 7575  r", b"user", "uu
+00002410: 6964 222c 2062 2275 7569 6422 2c20 2277  id", b"uuid", "w
+00002420: 6865 6e22 2c20 6222 7768 656e 225d 2920  hen", b"when"]) 
+00002430: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
+00002440: 6f62 616c 5f5f 5f41 7564 6974 203d 2041  obal___Audit = A
+00002450: 7564 6974 0a0a 4074 7970 696e 672e 6669  udit..@typing.fi
+00002460: 6e61 6c0a 636c 6173 7320 4572 726f 7228  nal.class Error(
+00002470: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00002480: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+00002490: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
+000024a0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+000024b0: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
+000024c0: 6372 6970 746f 720a 0a20 2020 2063 6c61  criptor..    cla
+000024d0: 7373 205f 4572 726f 7243 6f64 653a 0a20  ss _ErrorCode:. 
+000024e0: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
+000024f0: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
+00002500: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
+00002510: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
+00002520: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
+00002530: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
+00002540: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
+00002550: 0a20 2020 2063 6c61 7373 205f 4572 726f  .    class _Erro
+00002560: 7243 6f64 6545 6e75 6d54 7970 6557 7261  rCodeEnumTypeWra
+00002570: 7070 6572 2867 6f6f 676c 652e 7072 6f74  pper(google.prot
+00002580: 6f62 7566 2e69 6e74 6572 6e61 6c2e 656e  obuf.internal.en
+00002590: 756d 5f74 7970 655f 7772 6170 7065 722e  um_type_wrapper.
+000025a0: 5f45 6e75 6d54 7970 6557 7261 7070 6572  _EnumTypeWrapper
+000025b0: 5b45 7272 6f72 2e5f 4572 726f 7243 6f64  [Error._ErrorCod
+000025c0: 652e 5661 6c75 6554 7970 655d 2c20 6275  e.ValueType], bu
+000025d0: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
+000025e0: 2020 2020 2020 4445 5343 5249 5054 4f52        DESCRIPTOR
+000025f0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+00002600: 662e 6465 7363 7269 7074 6f72 2e45 6e75  f.descriptor.Enu
+00002610: 6d44 6573 6372 6970 746f 720a 2020 2020  mDescriptor.    
+00002620: 2020 2020 4745 4e45 5249 433a 2045 7272      GENERIC: Err
+00002630: 6f72 2e5f 4572 726f 7243 6f64 652e 5661  or._ErrorCode.Va
+00002640: 6c75 6554 7970 6520 2023 2030 0a20 2020  lueType  # 0.   
+00002650: 2020 2020 2045 5854 5241 4354 3a20 4572       EXTRACT: Er
+00002660: 726f 722e 5f45 7272 6f72 436f 6465 2e56  ror._ErrorCode.V
+00002670: 616c 7565 5479 7065 2020 2320 310a 2020  alueType  # 1.  
+00002680: 2020 2020 2020 5052 4f43 4553 533a 2045        PROCESS: E
+00002690: 7272 6f72 2e5f 4572 726f 7243 6f64 652e  rror._ErrorCode.
+000026a0: 5661 6c75 6554 7970 6520 2023 2032 0a0a  ValueType  # 2..
+000026b0: 2020 2020 636c 6173 7320 4572 726f 7243      class ErrorC
+000026c0: 6f64 6528 5f45 7272 6f72 436f 6465 2c20  ode(_ErrorCode, 
+000026d0: 6d65 7461 636c 6173 733d 5f45 7272 6f72  metaclass=_Error
+000026e0: 436f 6465 456e 756d 5479 7065 5772 6170  CodeEnumTypeWrap
+000026f0: 7065 7229 3a20 2e2e 2e0a 2020 2020 4745  per): ....    GE
+00002700: 4e45 5249 433a 2045 7272 6f72 2e45 7272  NERIC: Error.Err
+00002710: 6f72 436f 6465 2e56 616c 7565 5479 7065  orCode.ValueType
+00002720: 2020 2320 300a 2020 2020 4558 5452 4143    # 0.    EXTRAC
+00002730: 543a 2045 7272 6f72 2e45 7272 6f72 436f  T: Error.ErrorCo
+00002740: 6465 2e56 616c 7565 5479 7065 2020 2320  de.ValueType  # 
+00002750: 310a 2020 2020 5052 4f43 4553 533a 2045  1.    PROCESS: E
+00002760: 7272 6f72 2e45 7272 6f72 436f 6465 2e56  rror.ErrorCode.V
+00002770: 616c 7565 5479 7065 2020 2320 320a 0a20  alueType  # 2.. 
+00002780: 2020 2046 4945 4c44 5f46 4945 4c44 5f4e     FIELD_FIELD_N
+00002790: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+000027a0: 696e 740a 2020 2020 4649 454c 445f 5459  int.    FIELD_TY
+000027b0: 5045 5f46 4945 4c44 5f4e 554d 4245 523a  PE_FIELD_NUMBER:
+000027c0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+000027d0: 2020 4552 524f 525f 4649 454c 445f 4e55    ERROR_FIELD_NU
+000027e0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+000027f0: 6e74 0a20 2020 2043 4f44 455f 4649 454c  nt.    CODE_FIEL
+00002800: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00002810: 6e73 2e69 6e74 0a20 2020 2066 6965 6c64  ns.int.    field
+00002820: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+00002830: 2020 2066 6965 6c64 5f74 7970 653a 206e     field_type: n
+00002840: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00002850: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
+00002860: 6c64 5479 7065 2e56 616c 7565 5479 7065  ldType.ValueType
+00002870: 0a20 2020 2065 7272 6f72 3a20 6275 696c  .    error: buil
+00002880: 7469 6e73 2e73 7472 0a20 2020 2063 6f64  tins.str.    cod
+00002890: 653a 2067 6c6f 6261 6c5f 5f5f 4572 726f  e: global___Erro
+000028a0: 722e 4572 726f 7243 6f64 652e 5661 6c75  r.ErrorCode.Valu
+000028b0: 6554 7970 650a 2020 2020 6465 6620 5f5f  eType.    def __
+000028c0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000028d0: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
+000028e0: 0a20 2020 2020 2020 2066 6965 6c64 3a20  .        field: 
+000028f0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
+00002900: 2e2e 2c0a 2020 2020 2020 2020 6669 656c  ..,.        fiel
+00002910: 645f 7479 7065 3a20 6e75 636c 6961 6462  d_type: nucliadb
+00002920: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+00002930: 735f 7062 322e 4669 656c 6454 7970 652e  s_pb2.FieldType.
+00002940: 5661 6c75 6554 7970 6520 3d20 2e2e 2e2c  ValueType = ...,
+00002950: 0a20 2020 2020 2020 2065 7272 6f72 3a20  .        error: 
+00002960: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
+00002970: 2e2e 2c0a 2020 2020 2020 2020 636f 6465  ..,.        code
+00002980: 3a20 676c 6f62 616c 5f5f 5f45 7272 6f72  : global___Error
+00002990: 2e45 7272 6f72 436f 6465 2e56 616c 7565  .ErrorCode.Value
+000029a0: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
+000029b0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+000029c0: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
+000029d0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+000029e0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+000029f0: 616c 5b22 636f 6465 222c 2062 2263 6f64  al["code", b"cod
+00002a00: 6522 2c20 2265 7272 6f72 222c 2062 2265  e", "error", b"e
+00002a10: 7272 6f72 222c 2022 6669 656c 6422 2c20  rror", "field", 
+00002a20: 6222 6669 656c 6422 2c20 2266 6965 6c64  b"field", "field
+00002a30: 5f74 7970 6522 2c20 6222 6669 656c 645f  _type", b"field_
+00002a40: 7479 7065 225d 2920 2d3e 204e 6f6e 653a  type"]) -> None:
+00002a50: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f45   .....global___E
+00002a60: 7272 6f72 203d 2045 7272 6f72 0a0a 4074  rror = Error..@t
+00002a70: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
+00002a80: 7320 4272 6f6b 6572 4d65 7373 6167 6528  s BrokerMessage(
+00002a90: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00002aa0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+00002ab0: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
+00002ac0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+00002ad0: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
+00002ae0: 6372 6970 746f 720a 0a20 2020 2063 6c61  criptor..    cla
+00002af0: 7373 205f 4d65 7373 6167 6554 7970 653a  ss _MessageType:
+00002b00: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
+00002b10: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
+00002b20: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
+00002b30: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
+00002b40: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
+00002b50: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
+00002b60: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
+00002b70: 650a 0a20 2020 2063 6c61 7373 205f 4d65  e..    class _Me
+00002b80: 7373 6167 6554 7970 6545 6e75 6d54 7970  ssageTypeEnumTyp
+00002b90: 6557 7261 7070 6572 2867 6f6f 676c 652e  eWrapper(google.
+00002ba0: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
+00002bb0: 6c2e 656e 756d 5f74 7970 655f 7772 6170  l.enum_type_wrap
+00002bc0: 7065 722e 5f45 6e75 6d54 7970 6557 7261  per._EnumTypeWra
+00002bd0: 7070 6572 5b42 726f 6b65 724d 6573 7361  pper[BrokerMessa
+00002be0: 6765 2e5f 4d65 7373 6167 6554 7970 652e  ge._MessageType.
+00002bf0: 5661 6c75 6554 7970 655d 2c20 6275 696c  ValueType], buil
+00002c00: 7469 6e73 2e74 7970 6529 3a0a 2020 2020  tins.type):.    
+00002c10: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
+00002c20: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00002c30: 6465 7363 7269 7074 6f72 2e45 6e75 6d44  descriptor.EnumD
+00002c40: 6573 6372 6970 746f 720a 2020 2020 2020  escriptor.      
+00002c50: 2020 4155 544f 434f 4d4d 4954 3a20 4272    AUTOCOMMIT: Br
+00002c60: 6f6b 6572 4d65 7373 6167 652e 5f4d 6573  okerMessage._Mes
+00002c70: 7361 6765 5479 7065 2e56 616c 7565 5479  sageType.ValueTy
+00002c80: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
+00002c90: 4d55 4c54 493a 2042 726f 6b65 724d 6573  MULTI: BrokerMes
+00002ca0: 7361 6765 2e5f 4d65 7373 6167 6554 7970  sage._MessageTyp
+00002cb0: 652e 5661 6c75 6554 7970 6520 2023 2031  e.ValueType  # 1
+00002cc0: 0a20 2020 2020 2020 2043 4f4d 4d49 543a  .        COMMIT:
+00002cd0: 2042 726f 6b65 724d 6573 7361 6765 2e5f   BrokerMessage._
+00002ce0: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
+00002cf0: 6554 7970 6520 2023 2032 0a20 2020 2020  eType  # 2.     
+00002d00: 2020 2052 4f4c 4c42 4143 4b3a 2042 726f     ROLLBACK: Bro
+00002d10: 6b65 724d 6573 7361 6765 2e5f 4d65 7373  kerMessage._Mess
+00002d20: 6167 6554 7970 652e 5661 6c75 6554 7970  ageType.ValueTyp
+00002d30: 6520 2023 2033 0a20 2020 2020 2020 2044  e  # 3.        D
+00002d40: 454c 4554 453a 2042 726f 6b65 724d 6573  ELETE: BrokerMes
+00002d50: 7361 6765 2e5f 4d65 7373 6167 6554 7970  sage._MessageTyp
+00002d60: 652e 5661 6c75 6554 7970 6520 2023 2034  e.ValueType  # 4
+00002d70: 0a0a 2020 2020 636c 6173 7320 4d65 7373  ..    class Mess
+00002d80: 6167 6554 7970 6528 5f4d 6573 7361 6765  ageType(_Message
+00002d90: 5479 7065 2c20 6d65 7461 636c 6173 733d  Type, metaclass=
+00002da0: 5f4d 6573 7361 6765 5479 7065 456e 756d  _MessageTypeEnum
+00002db0: 5479 7065 5772 6170 7065 7229 3a20 2e2e  TypeWrapper): ..
+00002dc0: 2e0a 2020 2020 4155 544f 434f 4d4d 4954  ..    AUTOCOMMIT
+00002dd0: 3a20 4272 6f6b 6572 4d65 7373 6167 652e  : BrokerMessage.
+00002de0: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
+00002df0: 6554 7970 6520 2023 2030 0a20 2020 204d  eType  # 0.    M
+00002e00: 554c 5449 3a20 4272 6f6b 6572 4d65 7373  ULTI: BrokerMess
+00002e10: 6167 652e 4d65 7373 6167 6554 7970 652e  age.MessageType.
+00002e20: 5661 6c75 6554 7970 6520 2023 2031 0a20  ValueType  # 1. 
+00002e30: 2020 2043 4f4d 4d49 543a 2042 726f 6b65     COMMIT: Broke
+00002e40: 724d 6573 7361 6765 2e4d 6573 7361 6765  rMessage.Message
+00002e50: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
+00002e60: 2320 320a 2020 2020 524f 4c4c 4241 434b  # 2.    ROLLBACK
+00002e70: 3a20 4272 6f6b 6572 4d65 7373 6167 652e  : BrokerMessage.
+00002e80: 4d65 7373 6167 6554 7970 652e 5661 6c75  MessageType.Valu
+00002e90: 6554 7970 6520 2023 2033 0a20 2020 2044  eType  # 3.    D
+00002ea0: 454c 4554 453a 2042 726f 6b65 724d 6573  ELETE: BrokerMes
+00002eb0: 7361 6765 2e4d 6573 7361 6765 5479 7065  sage.MessageType
+00002ec0: 2e56 616c 7565 5479 7065 2020 2320 340a  .ValueType  # 4.
+00002ed0: 0a20 2020 2063 6c61 7373 205f 4d65 7373  .    class _Mess
+00002ee0: 6167 6553 6f75 7263 653a 0a20 2020 2020  ageSource:.     
+00002ef0: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
+00002f00: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
+00002f10: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
+00002f20: 696e 732e 696e 7429 0a20 2020 2020 2020  ins.int).       
+00002f30: 2056 3a20 7479 7069 6e67 5f65 7874 656e   V: typing_exten
+00002f40: 7369 6f6e 732e 5479 7065 416c 6961 7320  sions.TypeAlias 
+00002f50: 3d20 5661 6c75 6554 7970 650a 0a20 2020  = ValueType..   
+00002f60: 2063 6c61 7373 205f 4d65 7373 6167 6553   class _MessageS
+00002f70: 6f75 7263 6545 6e75 6d54 7970 6557 7261  ourceEnumTypeWra
+00002f80: 7070 6572 2867 6f6f 676c 652e 7072 6f74  pper(google.prot
+00002f90: 6f62 7566 2e69 6e74 6572 6e61 6c2e 656e  obuf.internal.en
+00002fa0: 756d 5f74 7970 655f 7772 6170 7065 722e  um_type_wrapper.
+00002fb0: 5f45 6e75 6d54 7970 6557 7261 7070 6572  _EnumTypeWrapper
+00002fc0: 5b42 726f 6b65 724d 6573 7361 6765 2e5f  [BrokerMessage._
+00002fd0: 4d65 7373 6167 6553 6f75 7263 652e 5661  MessageSource.Va
+00002fe0: 6c75 6554 7970 655d 2c20 6275 696c 7469  lueType], builti
+00002ff0: 6e73 2e74 7970 6529 3a0a 2020 2020 2020  ns.type):.      
+00003000: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00003010: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00003020: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
+00003030: 6372 6970 746f 720a 2020 2020 2020 2020  criptor.        
+00003040: 5752 4954 4552 3a20 4272 6f6b 6572 4d65  WRITER: BrokerMe
+00003050: 7373 6167 652e 5f4d 6573 7361 6765 536f  ssage._MessageSo
+00003060: 7572 6365 2e56 616c 7565 5479 7065 2020  urce.ValueType  
+00003070: 2320 300a 2020 2020 2020 2020 5052 4f43  # 0.        PROC
+00003080: 4553 534f 523a 2042 726f 6b65 724d 6573  ESSOR: BrokerMes
+00003090: 7361 6765 2e5f 4d65 7373 6167 6553 6f75  sage._MessageSou
+000030a0: 7263 652e 5661 6c75 6554 7970 6520 2023  rce.ValueType  #
+000030b0: 2031 0a0a 2020 2020 636c 6173 7320 4d65   1..    class Me
+000030c0: 7373 6167 6553 6f75 7263 6528 5f4d 6573  ssageSource(_Mes
+000030d0: 7361 6765 536f 7572 6365 2c20 6d65 7461  sageSource, meta
+000030e0: 636c 6173 733d 5f4d 6573 7361 6765 536f  class=_MessageSo
+000030f0: 7572 6365 456e 756d 5479 7065 5772 6170  urceEnumTypeWrap
+00003100: 7065 7229 3a20 2e2e 2e0a 2020 2020 5752  per): ....    WR
+00003110: 4954 4552 3a20 4272 6f6b 6572 4d65 7373  ITER: BrokerMess
+00003120: 6167 652e 4d65 7373 6167 6553 6f75 7263  age.MessageSourc
+00003130: 652e 5661 6c75 6554 7970 6520 2023 2030  e.ValueType  # 0
+00003140: 0a20 2020 2050 524f 4345 5353 4f52 3a20  .    PROCESSOR: 
+00003150: 4272 6f6b 6572 4d65 7373 6167 652e 4d65  BrokerMessage.Me
+00003160: 7373 6167 6553 6f75 7263 652e 5661 6c75  ssageSource.Valu
+00003170: 6554 7970 6520 2023 2031 0a0a 2020 2020  eType  # 1..    
+00003180: 4074 7970 696e 672e 6669 6e61 6c0a 2020  @typing.final.  
+00003190: 2020 636c 6173 7320 436f 6e76 6572 7361    class Conversa
+000031a0: 7469 6f6e 7345 6e74 7279 2867 6f6f 676c  tionsEntry(googl
+000031b0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+000031c0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+000031d0: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
+000031e0: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+000031f0: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
+00003200: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
+00003210: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
+00003220: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00003230: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
+00003240: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00003250: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
+00003260: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+00003270: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
+00003280: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
+00003290: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
+000032a0: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+000032b0: 6573 6f75 7263 6573 5f70 6232 2e43 6f6e  esources_pb2.Con
+000032c0: 7665 7273 6174 696f 6e3a 202e 2e2e 0a20  versation: .... 
+000032d0: 2020 2020 2020 2064 6566 205f 5f69 6e69         def __ini
+000032e0: 745f 5f28 0a20 2020 2020 2020 2020 2020  t__(.           
+000032f0: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00003300: 2020 202a 2c0a 2020 2020 2020 2020 2020     *,.          
+00003310: 2020 6b65 793a 2062 7569 6c74 696e 732e    key: builtins.
+00003320: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
+00003330: 2020 2020 2020 2076 616c 7565 3a20 6e75         value: nu
+00003340: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+00003350: 736f 7572 6365 735f 7062 322e 436f 6e76  sources_pb2.Conv
+00003360: 6572 7361 7469 6f6e 207c 204e 6f6e 6520  ersation | None 
+00003370: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
+00003380: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+00003390: 2020 2020 2020 6465 6620 4861 7346 6965        def HasFie
+000033a0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+000033b0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+000033c0: 7261 6c5b 2276 616c 7565 222c 2062 2276  ral["value", b"v
+000033d0: 616c 7565 225d 2920 2d3e 2062 7569 6c74  alue"]) -> built
+000033e0: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
+000033f0: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
+00003400: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+00003410: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+00003420: 7465 7261 6c5b 226b 6579 222c 2062 226b  teral["key", b"k
+00003430: 6579 222c 2022 7661 6c75 6522 2c20 6222  ey", "value", b"
+00003440: 7661 6c75 6522 5d29 202d 3e20 4e6f 6e65  value"]) -> None
+00003450: 3a20 2e2e 2e0a 0a20 2020 2040 7479 7069  : .....    @typi
+00003460: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
+00003470: 7373 204c 6179 6f75 7473 456e 7472 7928  ss LayoutsEntry(
+00003480: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00003490: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+000034a0: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
+000034b0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+000034c0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+000034d0: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
+000034e0: 2020 2020 204b 4559 5f46 4945 4c44 5f4e       KEY_FIELD_N
+000034f0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00003500: 696e 740a 2020 2020 2020 2020 5641 4c55  int.        VALU
+00003510: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
+00003520: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00003530: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
+00003540: 6e73 2e73 7472 0a20 2020 2020 2020 2040  ns.str.        @
+00003550: 7072 6f70 6572 7479 0a20 2020 2020 2020  property.       
+00003560: 2064 6566 2076 616c 7565 2873 656c 6629   def value(self)
+00003570: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
+00003580: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
+00003590: 322e 4669 656c 644c 6179 6f75 743a 202e  2.FieldLayout: .
+000035a0: 2e2e 0a20 2020 2020 2020 2064 6566 205f  ...        def _
+000035b0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000035c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000035d0: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+000035e0: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
+000035f0: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+00003600: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00003610: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+00003620: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+00003630: 4669 656c 644c 6179 6f75 7420 7c20 4e6f  FieldLayout | No
+00003640: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+00003650: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+00003660: 0a20 2020 2020 2020 2064 6566 2048 6173  .        def Has
+00003670: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+00003680: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+00003690: 6974 6572 616c 5b22 7661 6c75 6522 2c20  iteral["value", 
+000036a0: 6222 7661 6c75 6522 5d29 202d 3e20 6275  b"value"]) -> bu
+000036b0: 696c 7469 6e73 2e62 6f6f 6c3a 202e 2e2e  iltins.bool: ...
+000036c0: 0a20 2020 2020 2020 2064 6566 2043 6c65  .        def Cle
+000036d0: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
+000036e0: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+000036f0: 2e4c 6974 6572 616c 5b22 6b65 7922 2c20  .Literal["key", 
+00003700: 6222 6b65 7922 2c20 2276 616c 7565 222c  b"key", "value",
+00003710: 2062 2276 616c 7565 225d 2920 2d3e 204e   b"value"]) -> N
+00003720: 6f6e 653a 202e 2e2e 0a0a 2020 2020 4074  one: .....    @t
+00003730: 7970 696e 672e 6669 6e61 6c0a 2020 2020  yping.final.    
+00003740: 636c 6173 7320 5465 7874 7345 6e74 7279  class TextsEntry
+00003750: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
+00003760: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
+00003770: 293a 0a20 2020 2020 2020 2044 4553 4352  ):.        DESCR
+00003780: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+00003790: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+000037a0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+000037b0: 2020 2020 2020 4b45 595f 4649 454c 445f        KEY_FIELD_
+000037c0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+000037d0: 2e69 6e74 0a20 2020 2020 2020 2056 414c  .int.        VAL
+000037e0: 5545 5f46 4945 4c44 5f4e 554d 4245 523a  UE_FIELD_NUMBER:
+000037f0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+00003800: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
+00003810: 696e 732e 7374 720a 2020 2020 2020 2020  ins.str.        
+00003820: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
+00003830: 2020 6465 6620 7661 6c75 6528 7365 6c66    def value(self
+00003840: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
+00003850: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+00003860: 6232 2e46 6965 6c64 5465 7874 3a20 2e2e  b2.FieldText: ..
+00003870: 2e0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
+00003880: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00003890: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000038a0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+000038b0: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
+000038c0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+000038d0: 2020 2020 2020 2020 2020 7661 6c75 653a            value:
+000038e0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+000038f0: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00003900: 6965 6c64 5465 7874 207c 204e 6f6e 6520  ieldText | None 
+00003910: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
+00003920: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+00003930: 2020 2020 2020 6465 6620 4861 7346 6965        def HasFie
+00003940: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+00003950: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+00003960: 7261 6c5b 2276 616c 7565 222c 2062 2276  ral["value", b"v
+00003970: 616c 7565 225d 2920 2d3e 2062 7569 6c74  alue"]) -> built
+00003980: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
+00003990: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
+000039a0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+000039b0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+000039c0: 7465 7261 6c5b 226b 6579 222c 2062 226b  teral["key", b"k
+000039d0: 6579 222c 2022 7661 6c75 6522 2c20 6222  ey", "value", b"
+000039e0: 7661 6c75 6522 5d29 202d 3e20 4e6f 6e65  value"]) -> None
+000039f0: 3a20 2e2e 2e0a 0a20 2020 2040 7479 7069  : .....    @typi
+00003a00: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
+00003a10: 7373 204b 6579 776f 7264 7365 7473 456e  ss KeywordsetsEn
+00003a20: 7472 7928 676f 6f67 6c65 2e70 726f 746f  try(google.proto
+00003a30: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
+00003a40: 6167 6529 3a0a 2020 2020 2020 2020 4445  age):.        DE
+00003a50: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00003a60: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00003a70: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+00003a80: 0a20 2020 2020 2020 204b 4559 5f46 4945  .        KEY_FIE
+00003a90: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00003aa0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
+00003ab0: 5641 4c55 455f 4649 454c 445f 4e55 4d42  VALUE_FIELD_NUMB
+00003ac0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00003ad0: 0a20 2020 2020 2020 206b 6579 3a20 6275  .        key: bu
+00003ae0: 696c 7469 6e73 2e73 7472 0a20 2020 2020  iltins.str.     
+00003af0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00003b00: 2020 2020 2064 6566 2076 616c 7565 2873       def value(s
+00003b10: 656c 6629 202d 3e20 6e75 636c 6961 6462  elf) -> nucliadb
+00003b20: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+00003b30: 735f 7062 322e 4669 656c 644b 6579 776f  s_pb2.FieldKeywo
+00003b40: 7264 7365 743a 202e 2e2e 0a20 2020 2020  rdset: ....     
+00003b50: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00003b60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003b70: 662c 0a20 2020 2020 2020 2020 2020 202a  f,.            *
+00003b80: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
+00003b90: 793a 2062 7569 6c74 696e 732e 7374 7220  y: builtins.str 
+00003ba0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2020  = ...,.         
+00003bb0: 2020 2076 616c 7565 3a20 6e75 636c 6961     value: nuclia
+00003bc0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+00003bd0: 6365 735f 7062 322e 4669 656c 644b 6579  ces_pb2.FieldKey
+00003be0: 776f 7264 7365 7420 7c20 4e6f 6e65 203d  wordset | None =
+00003bf0: 202e 2e2e 2c0a 2020 2020 2020 2020 2920   ...,.        ) 
+00003c00: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+00003c10: 2020 2020 2064 6566 2048 6173 4669 656c       def HasFiel
+00003c20: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+00003c30: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+00003c40: 616c 5b22 7661 6c75 6522 2c20 6222 7661  al["value", b"va
+00003c50: 6c75 6522 5d29 202d 3e20 6275 696c 7469  lue"]) -> builti
+00003c60: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
+00003c70: 2020 2020 2064 6566 2043 6c65 6172 4669       def ClearFi
+00003c80: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
+00003c90: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
+00003ca0: 6572 616c 5b22 6b65 7922 2c20 6222 6b65  eral["key", b"ke
+00003cb0: 7922 2c20 2276 616c 7565 222c 2062 2276  y", "value", b"v
+00003cc0: 616c 7565 225d 2920 2d3e 204e 6f6e 653a  alue"]) -> None:
+00003cd0: 202e 2e2e 0a0a 2020 2020 4074 7970 696e   .....    @typin
+00003ce0: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
+00003cf0: 7320 4461 7465 7469 6d65 7345 6e74 7279  s DatetimesEntry
+00003d00: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
+00003d10: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
+00003d20: 293a 0a20 2020 2020 2020 2044 4553 4352  ):.        DESCR
+00003d30: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+00003d40: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+00003d50: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+00003d60: 2020 2020 2020 4b45 595f 4649 454c 445f        KEY_FIELD_
+00003d70: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00003d80: 2e69 6e74 0a20 2020 2020 2020 2056 414c  .int.        VAL
+00003d90: 5545 5f46 4945 4c44 5f4e 554d 4245 523a  UE_FIELD_NUMBER:
+00003da0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+00003db0: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
+00003dc0: 696e 732e 7374 720a 2020 2020 2020 2020  ins.str.        
+00003dd0: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
+00003de0: 2020 6465 6620 7661 6c75 6528 7365 6c66    def value(self
+00003df0: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
+00003e00: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+00003e10: 6232 2e46 6965 6c64 4461 7465 7469 6d65  b2.FieldDatetime
+00003e20: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
+00003e30: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00003e40: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00003e50: 2020 2020 2020 2020 2020 2a2c 0a20 2020            *,.   
+00003e60: 2020 2020 2020 2020 206b 6579 3a20 6275           key: bu
+00003e70: 696c 7469 6e73 2e73 7472 203d 202e 2e2e  iltins.str = ...
+00003e80: 2c0a 2020 2020 2020 2020 2020 2020 7661  ,.            va
+00003e90: 6c75 653a 206e 7563 6c69 6164 625f 7072  lue: nucliadb_pr
+00003ea0: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+00003eb0: 6232 2e46 6965 6c64 4461 7465 7469 6d65  b2.FieldDatetime
+00003ec0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00003ed0: 2020 2020 2020 2029 202d 3e20 4e6f 6e65         ) -> None
+00003ee0: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
+00003ef0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
+00003f00: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+00003f10: 696e 672e 4c69 7465 7261 6c5b 2276 616c  ing.Literal["val
+00003f20: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
+00003f30: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
+00003f40: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
+00003f50: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
+00003f60: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+00003f70: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
+00003f80: 6579 222c 2062 226b 6579 222c 2022 7661  ey", b"key", "va
+00003f90: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
+00003fa0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20   -> None: ..... 
+00003fb0: 2020 2040 7479 7069 6e67 2e66 696e 616c     @typing.final
+00003fc0: 0a20 2020 2063 6c61 7373 204c 696e 6b73  .    class Links
+00003fd0: 456e 7472 7928 676f 6f67 6c65 2e70 726f  Entry(google.pro
+00003fe0: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
+00003ff0: 7373 6167 6529 3a0a 2020 2020 2020 2020  ssage):.        
+00004000: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+00004010: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+00004020: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
+00004030: 720a 0a20 2020 2020 2020 204b 4559 5f46  r..        KEY_F
+00004040: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00004050: 6c74 696e 732e 696e 740a 2020 2020 2020  ltins.int.      
+00004060: 2020 5641 4c55 455f 4649 454c 445f 4e55    VALUE_FIELD_NU
+00004070: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00004080: 6e74 0a20 2020 2020 2020 206b 6579 3a20  nt.        key: 
+00004090: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
+000040a0: 2020 2020 2040 7072 6f70 6572 7479 0a20       @property. 
+000040b0: 2020 2020 2020 2064 6566 2076 616c 7565         def value
+000040c0: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
+000040d0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+000040e0: 6365 735f 7062 322e 4669 656c 644c 696e  ces_pb2.FieldLin
+000040f0: 6b3a 202e 2e2e 0a20 2020 2020 2020 2064  k: ....        d
+00004100: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00004110: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00004120: 2020 2020 2020 2020 2020 202a 2c0a 2020             *,.  
+00004130: 2020 2020 2020 2020 2020 6b65 793a 2062            key: b
+00004140: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+00004150: 2e2c 0a20 2020 2020 2020 2020 2020 2076  .,.            v
+00004160: 616c 7565 3a20 6e75 636c 6961 6462 5f70  alue: nucliadb_p
+00004170: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
+00004180: 7062 322e 4669 656c 644c 696e 6b20 7c20  pb2.FieldLink | 
+00004190: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+000041a0: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
+000041b0: 2e2e 0a20 2020 2020 2020 2064 6566 2048  ...        def H
+000041c0: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
+000041d0: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+000041e0: 2e4c 6974 6572 616c 5b22 7661 6c75 6522  .Literal["value"
+000041f0: 2c20 6222 7661 6c75 6522 5d29 202d 3e20  , b"value"]) -> 
+00004200: 6275 696c 7469 6e73 2e62 6f6f 6c3a 202e  builtins.bool: .
+00004210: 2e2e 0a20 2020 2020 2020 2064 6566 2043  ...        def C
+00004220: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
+00004230: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+00004240: 6e67 2e4c 6974 6572 616c 5b22 6b65 7922  ng.Literal["key"
+00004250: 2c20 6222 6b65 7922 2c20 2276 616c 7565  , b"key", "value
+00004260: 222c 2062 2276 616c 7565 225d 2920 2d3e  ", b"value"]) ->
+00004270: 204e 6f6e 653a 202e 2e2e 0a0a 2020 2020   None: .....    
+00004280: 4074 7970 696e 672e 6669 6e61 6c0a 2020  @typing.final.  
+00004290: 2020 636c 6173 7320 4669 6c65 7345 6e74    class FilesEnt
+000042a0: 7279 2867 6f6f 676c 652e 7072 6f74 6f62  ry(google.protob
+000042b0: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
+000042c0: 6765 293a 0a20 2020 2020 2020 2044 4553  ge):.        DES
+000042d0: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
+000042e0: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
+000042f0: 746f 722e 4465 7363 7269 7074 6f72 0a0a  tor.Descriptor..
+00004300: 2020 2020 2020 2020 4b45 595f 4649 454c          KEY_FIEL
+00004310: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00004320: 6e73 2e69 6e74 0a20 2020 2020 2020 2056  ns.int.        V
+00004330: 414c 5545 5f46 4945 4c44 5f4e 554d 4245  ALUE_FIELD_NUMBE
+00004340: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00004350: 2020 2020 2020 2020 6b65 793a 2062 7569          key: bui
+00004360: 6c74 696e 732e 7374 720a 2020 2020 2020  ltins.str.      
+00004370: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00004380: 2020 2020 6465 6620 7661 6c75 6528 7365      def value(se
+00004390: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
+000043a0: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
+000043b0: 5f70 6232 2e46 6965 6c64 4669 6c65 3a20  _pb2.FieldFile: 
+000043c0: 2e2e 2e0a 2020 2020 2020 2020 6465 6620  ....        def 
+000043d0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000043e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000043f0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+00004400: 2020 2020 2020 206b 6579 3a20 6275 696c         key: buil
+00004410: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
+00004420: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00004430: 653a 206e 7563 6c69 6164 625f 7072 6f74  e: nucliadb_prot
+00004440: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
+00004450: 2e46 6965 6c64 4669 6c65 207c 204e 6f6e  .FieldFile | Non
+00004460: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
+00004470: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+00004480: 2020 2020 2020 2020 6465 6620 4861 7346          def HasF
+00004490: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+000044a0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+000044b0: 7465 7261 6c5b 2276 616c 7565 222c 2062  teral["value", b
+000044c0: 2276 616c 7565 225d 2920 2d3e 2062 7569  "value"]) -> bui
+000044d0: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
+000044e0: 2020 2020 2020 2020 6465 6620 436c 6561          def Clea
+000044f0: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00004500: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00004510: 4c69 7465 7261 6c5b 226b 6579 222c 2062  Literal["key", b
+00004520: 226b 6579 222c 2022 7661 6c75 6522 2c20  "key", "value", 
+00004530: 6222 7661 6c75 6522 5d29 202d 3e20 4e6f  b"value"]) -> No
+00004540: 6e65 3a20 2e2e 2e0a 0a20 2020 204b 4249  ne: .....    KBI
+00004550: 445f 4649 454c 445f 4e55 4d42 4552 3a20  D_FIELD_NUMBER: 
+00004560: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00004570: 2055 5549 445f 4649 454c 445f 4e55 4d42   UUID_FIELD_NUMB
+00004580: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00004590: 0a20 2020 2053 4c55 475f 4649 454c 445f  .    SLUG_FIELD_
+000045a0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+000045b0: 2e69 6e74 0a20 2020 2041 5544 4954 5f46  .int.    AUDIT_F
+000045c0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+000045d0: 6c74 696e 732e 696e 740a 2020 2020 5459  ltins.int.    TY
+000045e0: 5045 5f46 4945 4c44 5f4e 554d 4245 523a  PE_FIELD_NUMBER:
+000045f0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+00004600: 2020 4d55 4c54 4949 445f 4649 454c 445f    MULTIID_FIELD_
+00004610: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00004620: 2e69 6e74 0a20 2020 2042 4153 4943 5f46  .int.    BASIC_F
 00004630: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00004640: 6c74 696e 732e 696e 740a 2020 2020 5245  ltins.int.    RE
-00004650: 4c41 5449 4f4e 535f 4649 454c 445f 4e55  LATIONS_FIELD_NU
-00004660: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00004670: 6e74 0a20 2020 2043 4f4e 5645 5253 4154  nt.    CONVERSAT
-00004680: 494f 4e53 5f46 4945 4c44 5f4e 554d 4245  IONS_FIELD_NUMBE
-00004690: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-000046a0: 2020 2020 4c41 594f 5554 535f 4649 454c      LAYOUTS_FIEL
-000046b0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-000046c0: 6e73 2e69 6e74 0a20 2020 2054 4558 5453  ns.int.    TEXTS
-000046d0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-000046e0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-000046f0: 4b45 5957 4f52 4453 4554 535f 4649 454c  KEYWORDSETS_FIEL
-00004700: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00004710: 6e73 2e69 6e74 0a20 2020 2044 4154 4554  ns.int.    DATET
-00004720: 494d 4553 5f46 4945 4c44 5f4e 554d 4245  IMES_FIELD_NUMBE
-00004730: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00004740: 2020 2020 4c49 4e4b 535f 4649 454c 445f      LINKS_FIELD_
-00004750: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00004760: 2e69 6e74 0a20 2020 2046 494c 4553 5f46  .int.    FILES_F
-00004770: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00004780: 6c74 696e 732e 696e 740a 2020 2020 4c49  ltins.int.    LI
-00004790: 4e4b 5f45 5854 5241 4354 4544 5f44 4154  NK_EXTRACTED_DAT
-000047a0: 415f 4649 454c 445f 4e55 4d42 4552 3a20  A_FIELD_NUMBER: 
-000047b0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-000047c0: 2046 494c 455f 4558 5452 4143 5445 445f   FILE_EXTRACTED_
-000047d0: 4441 5441 5f46 4945 4c44 5f4e 554d 4245  DATA_FIELD_NUMBE
-000047e0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-000047f0: 2020 2020 4558 5452 4143 5445 445f 5445      EXTRACTED_TE
-00004800: 5854 5f46 4945 4c44 5f4e 554d 4245 523a  XT_FIELD_NUMBER:
-00004810: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00004820: 2020 4649 454c 445f 4d45 5441 4441 5441    FIELD_METADATA
-00004830: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00004840: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00004850: 4649 454c 445f 5645 4354 4f52 535f 4649  FIELD_VECTORS_FI
-00004860: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-00004870: 7469 6e73 2e69 6e74 0a20 2020 2046 4945  tins.int.    FIE
-00004880: 4c44 5f4c 4152 4745 5f4d 4554 4144 4154  LD_LARGE_METADAT
-00004890: 415f 4649 454c 445f 4e55 4d42 4552 3a20  A_FIELD_NUMBER: 
-000048a0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-000048b0: 2044 454c 4554 455f 4649 454c 4453 5f46   DELETE_FIELDS_F
-000048c0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-000048d0: 6c74 696e 732e 696e 740a 2020 2020 4f52  ltins.int.    OR
-000048e0: 4947 494e 5f53 4551 5f46 4945 4c44 5f4e  IGIN_SEQ_FIELD_N
-000048f0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00004900: 696e 740a 2020 2020 534c 4f57 5f50 524f  int.    SLOW_PRO
-00004910: 4345 5353 494e 475f 5449 4d45 5f46 4945  CESSING_TIME_FIE
-00004920: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00004930: 696e 732e 696e 740a 2020 2020 5052 455f  ins.int.    PRE_
-00004940: 5052 4f43 4553 5349 4e47 5f54 494d 455f  PROCESSING_TIME_
-00004950: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00004960: 696c 7469 6e73 2e69 6e74 0a20 2020 2044  iltins.int.    D
-00004970: 4f4e 455f 5449 4d45 5f46 4945 4c44 5f4e  ONE_TIME_FIELD_N
-00004980: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00004990: 696e 740a 2020 2020 5458 5345 5149 445f  int.    TXSEQID_
-000049a0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-000049b0: 696c 7469 6e73 2e69 6e74 0a20 2020 2045  iltins.int.    E
-000049c0: 5252 4f52 535f 4649 454c 445f 4e55 4d42  RRORS_FIELD_NUMB
+00004640: 6c74 696e 732e 696e 740a 2020 2020 4f52  ltins.int.    OR
+00004650: 4947 494e 5f46 4945 4c44 5f4e 554d 4245  IGIN_FIELD_NUMBE
+00004660: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00004670: 2020 2020 5245 4c41 5449 4f4e 535f 4649      RELATIONS_FI
+00004680: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00004690: 7469 6e73 2e69 6e74 0a20 2020 2043 4f4e  tins.int.    CON
+000046a0: 5645 5253 4154 494f 4e53 5f46 4945 4c44  VERSATIONS_FIELD
+000046b0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+000046c0: 732e 696e 740a 2020 2020 4c41 594f 5554  s.int.    LAYOUT
+000046d0: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
+000046e0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+000046f0: 2054 4558 5453 5f46 4945 4c44 5f4e 554d   TEXTS_FIELD_NUM
+00004700: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00004710: 740a 2020 2020 4b45 5957 4f52 4453 4554  t.    KEYWORDSET
+00004720: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
+00004730: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00004740: 2044 4154 4554 494d 4553 5f46 4945 4c44   DATETIMES_FIELD
+00004750: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00004760: 732e 696e 740a 2020 2020 4c49 4e4b 535f  s.int.    LINKS_
+00004770: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00004780: 696c 7469 6e73 2e69 6e74 0a20 2020 2046  iltins.int.    F
+00004790: 494c 4553 5f46 4945 4c44 5f4e 554d 4245  ILES_FIELD_NUMBE
+000047a0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+000047b0: 2020 2020 4c49 4e4b 5f45 5854 5241 4354      LINK_EXTRACT
+000047c0: 4544 5f44 4154 415f 4649 454c 445f 4e55  ED_DATA_FIELD_NU
+000047d0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+000047e0: 6e74 0a20 2020 2046 494c 455f 4558 5452  nt.    FILE_EXTR
+000047f0: 4143 5445 445f 4441 5441 5f46 4945 4c44  ACTED_DATA_FIELD
+00004800: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00004810: 732e 696e 740a 2020 2020 4558 5452 4143  s.int.    EXTRAC
+00004820: 5445 445f 5445 5854 5f46 4945 4c44 5f4e  TED_TEXT_FIELD_N
+00004830: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00004840: 696e 740a 2020 2020 4649 454c 445f 4d45  int.    FIELD_ME
+00004850: 5441 4441 5441 5f46 4945 4c44 5f4e 554d  TADATA_FIELD_NUM
+00004860: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00004870: 740a 2020 2020 4649 454c 445f 5645 4354  t.    FIELD_VECT
+00004880: 4f52 535f 4649 454c 445f 4e55 4d42 4552  ORS_FIELD_NUMBER
+00004890: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+000048a0: 2020 2046 4945 4c44 5f4c 4152 4745 5f4d     FIELD_LARGE_M
+000048b0: 4554 4144 4154 415f 4649 454c 445f 4e55  ETADATA_FIELD_NU
+000048c0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+000048d0: 6e74 0a20 2020 2044 454c 4554 455f 4649  nt.    DELETE_FI
+000048e0: 454c 4453 5f46 4945 4c44 5f4e 554d 4245  ELDS_FIELD_NUMBE
+000048f0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00004900: 2020 2020 4f52 4947 494e 5f53 4551 5f46      ORIGIN_SEQ_F
+00004910: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00004920: 6c74 696e 732e 696e 740a 2020 2020 534c  ltins.int.    SL
+00004930: 4f57 5f50 524f 4345 5353 494e 475f 5449  OW_PROCESSING_TI
+00004940: 4d45 5f46 4945 4c44 5f4e 554d 4245 523a  ME_FIELD_NUMBER:
+00004950: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+00004960: 2020 5052 455f 5052 4f43 4553 5349 4e47    PRE_PROCESSING
+00004970: 5f54 494d 455f 4649 454c 445f 4e55 4d42  _TIME_FIELD_NUMB
+00004980: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00004990: 0a20 2020 2044 4f4e 455f 5449 4d45 5f46  .    DONE_TIME_F
+000049a0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+000049b0: 6c74 696e 732e 696e 740a 2020 2020 5458  ltins.int.    TX
+000049c0: 5345 5149 445f 4649 454c 445f 4e55 4d42  SEQID_FIELD_NUMB
 000049d0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-000049e0: 0a20 2020 2050 524f 4345 5353 494e 475f  .    PROCESSING_
-000049f0: 4944 5f46 4945 4c44 5f4e 554d 4245 523a  ID_FIELD_NUMBER:
-00004a00: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-00004a10: 2020 534f 5552 4345 5f46 4945 4c44 5f4e    SOURCE_FIELD_N
+000049e0: 0a20 2020 2045 5252 4f52 535f 4649 454c  .    ERRORS_FIEL
+000049f0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00004a00: 6e73 2e69 6e74 0a20 2020 2050 524f 4345  ns.int.    PROCE
+00004a10: 5353 494e 475f 4944 5f46 4945 4c44 5f4e  SSING_ID_FIELD_N
 00004a20: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00004a30: 696e 740a 2020 2020 4143 434f 554e 545f  int.    ACCOUNT_
-00004a40: 5345 515f 4649 454c 445f 4e55 4d42 4552  SEQ_FIELD_NUMBER
-00004a50: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00004a60: 2020 2055 5345 525f 5645 4354 4f52 535f     USER_VECTORS_
-00004a70: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00004a80: 696c 7469 6e73 2e69 6e74 0a20 2020 2052  iltins.int.    R
-00004a90: 4549 4e44 4558 5f46 4945 4c44 5f4e 554d  EINDEX_FIELD_NUM
-00004aa0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00004ab0: 740a 2020 2020 4558 5452 415f 4649 454c  t.    EXTRA_FIEL
-00004ac0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00004ad0: 6e73 2e69 6e74 0a20 2020 2051 5545 5354  ns.int.    QUEST
-00004ae0: 494f 4e5f 414e 5357 4552 535f 4649 454c  ION_ANSWERS_FIEL
-00004af0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00004b00: 6e73 2e69 6e74 0a20 2020 2053 4543 5552  ns.int.    SECUR
-00004b10: 4954 595f 4649 454c 445f 4e55 4d42 4552  ITY_FIELD_NUMBER
-00004b20: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00004b30: 2020 206b 6269 643a 2062 7569 6c74 696e     kbid: builtin
-00004b40: 732e 7374 720a 2020 2020 7575 6964 3a20  s.str.    uuid: 
-00004b50: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
-00004b60: 2073 6c75 673a 2062 7569 6c74 696e 732e   slug: builtins.
-00004b70: 7374 720a 2020 2020 7479 7065 3a20 676c  str.    type: gl
-00004b80: 6f62 616c 5f5f 5f42 726f 6b65 724d 6573  obal___BrokerMes
-00004b90: 7361 6765 2e4d 6573 7361 6765 5479 7065  sage.MessageType
-00004ba0: 2e56 616c 7565 5479 7065 0a20 2020 206d  .ValueType.    m
-00004bb0: 756c 7469 6964 3a20 6275 696c 7469 6e73  ultiid: builtins
-00004bc0: 2e73 7472 0a20 2020 206f 7269 6769 6e5f  .str.    origin_
-00004bd0: 7365 713a 2062 7569 6c74 696e 732e 696e  seq: builtins.in
-00004be0: 740a 2020 2020 736c 6f77 5f70 726f 6365  t.    slow_proce
-00004bf0: 7373 696e 675f 7469 6d65 3a20 6275 696c  ssing_time: buil
-00004c00: 7469 6e73 2e66 6c6f 6174 0a20 2020 2070  tins.float.    p
-00004c10: 7265 5f70 726f 6365 7373 696e 675f 7469  re_processing_ti
-00004c20: 6d65 3a20 6275 696c 7469 6e73 2e66 6c6f  me: builtins.flo
-00004c30: 6174 0a20 2020 2074 7873 6571 6964 3a20  at.    txseqid: 
-00004c40: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00004c50: 2022 2222 4e6f 7420 6e65 6564 6564 2061   """Not needed a
-00004c60: 6e79 6d6f 7265 2222 220a 2020 2020 7072  nymore""".    pr
-00004c70: 6f63 6573 7369 6e67 5f69 643a 2062 7569  ocessing_id: bui
-00004c80: 6c74 696e 732e 7374 720a 2020 2020 736f  ltins.str.    so
-00004c90: 7572 6365 3a20 676c 6f62 616c 5f5f 5f42  urce: global___B
-00004ca0: 726f 6b65 724d 6573 7361 6765 2e4d 6573  rokerMessage.Mes
-00004cb0: 7361 6765 536f 7572 6365 2e56 616c 7565  sageSource.Value
-00004cc0: 5479 7065 0a20 2020 2061 6363 6f75 6e74  Type.    account
-00004cd0: 5f73 6571 3a20 6275 696c 7469 6e73 2e69  _seq: builtins.i
-00004ce0: 6e74 0a20 2020 2072 6569 6e64 6578 3a20  nt.    reindex: 
-00004cf0: 6275 696c 7469 6e73 2e62 6f6f 6c0a 2020  builtins.bool.  
-00004d00: 2020 2222 2249 6620 7472 7565 2c20 666f    """If true, fo
-00004d10: 7263 6520 7265 696e 6465 7820 616c 6c20  rce reindex all 
-00004d20: 7061 7261 6772 6170 6873 2069 6e20 6120  paragraphs in a 
-00004d30: 7265 736f 7572 6365 2222 220a 2020 2020  resource""".    
-00004d40: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00004d50: 6620 6175 6469 7428 7365 6c66 2920 2d3e  f audit(self) ->
-00004d60: 2067 6c6f 6261 6c5f 5f5f 4175 6469 743a   global___Audit:
-00004d70: 202e 2e2e 0a20 2020 2040 7072 6f70 6572   ....    @proper
-00004d80: 7479 0a20 2020 2064 6566 2062 6173 6963  ty.    def basic
-00004d90: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
-00004da0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-00004db0: 6365 735f 7062 322e 4261 7369 633a 202e  ces_pb2.Basic: .
-00004dc0: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00004dd0: 0a20 2020 2064 6566 206f 7269 6769 6e28  .    def origin(
-00004de0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-00004df0: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
-00004e00: 6573 5f70 6232 2e4f 7269 6769 6e3a 202e  es_pb2.Origin: .
-00004e10: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00004e20: 0a20 2020 2064 6566 2072 656c 6174 696f  .    def relatio
-00004e30: 6e73 2873 656c 6629 202d 3e20 676f 6f67  ns(self) -> goog
-00004e40: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
-00004e50: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
-00004e60: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
-00004e70: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
-00004e80: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00004e90: 7574 696c 735f 7062 322e 5265 6c61 7469  utils_pb2.Relati
-00004ea0: 6f6e 5d3a 202e 2e2e 0a20 2020 2040 7072  on]: ....    @pr
-00004eb0: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
-00004ec0: 6f6e 7665 7273 6174 696f 6e73 2873 656c  onversations(sel
-00004ed0: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
-00004ee0: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
-00004ef0: 6f6e 7461 696e 6572 732e 4d65 7373 6167  ontainers.Messag
-00004f00: 654d 6170 5b62 7569 6c74 696e 732e 7374  eMap[builtins.st
-00004f10: 722c 206e 7563 6c69 6164 625f 7072 6f74  r, nucliadb_prot
-00004f20: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
-00004f30: 2e43 6f6e 7665 7273 6174 696f 6e5d 3a0a  .Conversation]:.
-00004f40: 2020 2020 2020 2020 2222 2246 6965 6c64          """Field
-00004f50: 2043 6f6e 7665 7273 6174 696f 6e73 2222   Conversations""
-00004f60: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
-00004f70: 0a20 2020 2064 6566 206c 6179 6f75 7473  .    def layouts
-00004f80: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
-00004f90: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
-00004fa0: 616c 2e63 6f6e 7461 696e 6572 732e 4d65  al.containers.Me
-00004fb0: 7373 6167 654d 6170 5b62 7569 6c74 696e  ssageMap[builtin
-00004fc0: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
-00004fd0: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
-00004fe0: 5f70 6232 2e46 6965 6c64 4c61 796f 7574  _pb2.FieldLayout
-00004ff0: 5d3a 0a20 2020 2020 2020 2022 2222 4669  ]:.        """Fi
-00005000: 656c 6420 4c61 796f 7574 2222 220a 0a20  eld Layout""".. 
-00005010: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00005020: 2064 6566 2074 6578 7473 2873 656c 6629   def texts(self)
-00005030: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
-00005040: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
-00005050: 7461 696e 6572 732e 4d65 7373 6167 654d  tainers.MessageM
-00005060: 6170 5b62 7569 6c74 696e 732e 7374 722c  ap[builtins.str,
-00005070: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00005080: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00005090: 6965 6c64 5465 7874 5d3a 0a20 2020 2020  ieldText]:.     
-000050a0: 2020 2022 2222 4669 656c 6420 5465 7874     """Field Text
-000050b0: 2222 220a 0a20 2020 2040 7072 6f70 6572  """..    @proper
-000050c0: 7479 0a20 2020 2064 6566 206b 6579 776f  ty.    def keywo
-000050d0: 7264 7365 7473 2873 656c 6629 202d 3e20  rdsets(self) -> 
-000050e0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-000050f0: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
-00005100: 6572 732e 4d65 7373 6167 654d 6170 5b62  ers.MessageMap[b
-00005110: 7569 6c74 696e 732e 7374 722c 206e 7563  uiltins.str, nuc
-00005120: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
-00005130: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
-00005140: 4b65 7977 6f72 6473 6574 5d3a 0a20 2020  Keywordset]:.   
-00005150: 2020 2020 2022 2222 4669 656c 6420 6b65       """Field ke
-00005160: 7977 6f72 6422 2222 0a0a 2020 2020 4070  yword"""..    @p
-00005170: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00005180: 6461 7465 7469 6d65 7328 7365 6c66 2920  datetimes(self) 
-00005190: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
-000051a0: 7566 2e69 6e74 6572 6e61 6c2e 636f 6e74  uf.internal.cont
-000051b0: 6169 6e65 7273 2e4d 6573 7361 6765 4d61  ainers.MessageMa
-000051c0: 705b 6275 696c 7469 6e73 2e73 7472 2c20  p[builtins.str, 
-000051d0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-000051e0: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
-000051f0: 656c 6444 6174 6574 696d 655d 3a0a 2020  eldDatetime]:.  
-00005200: 2020 2020 2020 2222 2246 6965 6c64 2044        """Field D
-00005210: 6174 6574 696d 6522 2222 0a0a 2020 2020  atetime"""..    
-00005220: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00005230: 6620 6c69 6e6b 7328 7365 6c66 2920 2d3e  f links(self) ->
-00005240: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00005250: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
-00005260: 6e65 7273 2e4d 6573 7361 6765 4d61 705b  ners.MessageMap[
-00005270: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
-00005280: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-00005290: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
-000052a0: 644c 696e 6b5d 3a0a 2020 2020 2020 2020  dLink]:.        
-000052b0: 2222 2246 6965 6c64 204c 696e 6b73 2222  """Field Links""
-000052c0: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
-000052d0: 0a20 2020 2064 6566 2066 696c 6573 2873  .    def files(s
-000052e0: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
-000052f0: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
-00005300: 2e63 6f6e 7461 696e 6572 732e 4d65 7373  .containers.Mess
-00005310: 6167 654d 6170 5b62 7569 6c74 696e 732e  ageMap[builtins.
-00005320: 7374 722c 206e 7563 6c69 6164 625f 7072  str, nucliadb_pr
-00005330: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
-00005340: 6232 2e46 6965 6c64 4669 6c65 5d3a 0a20  b2.FieldFile]:. 
-00005350: 2020 2020 2020 2022 2222 4669 656c 6420         """Field 
-00005360: 4669 6c65 2222 220a 0a20 2020 2040 7072  File"""..    @pr
-00005370: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
-00005380: 696e 6b5f 6578 7472 6163 7465 645f 6461  ink_extracted_da
-00005390: 7461 2873 656c 6629 202d 3e20 676f 6f67  ta(self) -> goog
-000053a0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
-000053b0: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
-000053c0: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
-000053d0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
-000053e0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-000053f0: 7265 736f 7572 6365 735f 7062 322e 4c69  resources_pb2.Li
-00005400: 6e6b 4578 7472 6163 7465 6444 6174 615d  nkExtractedData]
-00005410: 3a0a 2020 2020 2020 2020 2222 224c 696e  :.        """Lin
-00005420: 6b20 6578 7472 6163 7465 6420 6578 7472  k extracted extr
-00005430: 6120 696e 666f 2222 220a 0a20 2020 2040  a info"""..    @
-00005440: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00005450: 2066 696c 655f 6578 7472 6163 7465 645f   file_extracted_
-00005460: 6461 7461 2873 656c 6629 202d 3e20 676f  data(self) -> go
-00005470: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
-00005480: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
-00005490: 732e 5265 7065 6174 6564 436f 6d70 6f73  s.RepeatedCompos
-000054a0: 6974 6546 6965 6c64 436f 6e74 6169 6e65  iteFieldContaine
-000054b0: 725b 6e75 636c 6961 6462 5f70 726f 746f  r[nucliadb_proto
-000054c0: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-000054d0: 4669 6c65 4578 7472 6163 7465 6444 6174  FileExtractedDat
-000054e0: 615d 3a0a 2020 2020 2020 2020 2222 2246  a]:.        """F
-000054f0: 696c 6520 6578 7472 6163 7465 6420 6578  ile extracted ex
-00005500: 7472 6120 696e 666f 2222 220a 0a20 2020  tra info"""..   
-00005510: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00005520: 6566 2065 7874 7261 6374 6564 5f74 6578  ef extracted_tex
-00005530: 7428 7365 6c66 2920 2d3e 2067 6f6f 676c  t(self) -> googl
-00005540: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
-00005550: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
-00005560: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
-00005570: 4669 656c 6443 6f6e 7461 696e 6572 5b6e  FieldContainer[n
-00005580: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00005590: 6573 6f75 7263 6573 5f70 6232 2e45 7874  esources_pb2.Ext
-000055a0: 7261 6374 6564 5465 7874 5772 6170 7065  ractedTextWrappe
-000055b0: 725d 3a0a 2020 2020 2020 2020 2222 2246  r]:.        """F
-000055c0: 6965 6c64 2045 7874 7261 6374 6564 2f43  ield Extracted/C
-000055d0: 6f6d 7075 7465 6420 696e 666f 726d 6174  omputed informat
-000055e0: 696f 6e22 2222 0a0a 2020 2020 4070 726f  ion"""..    @pro
-000055f0: 7065 7274 790a 2020 2020 6465 6620 6669  perty.    def fi
-00005600: 656c 645f 6d65 7461 6461 7461 2873 656c  eld_metadata(sel
-00005610: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
-00005620: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
-00005630: 6f6e 7461 696e 6572 732e 5265 7065 6174  ontainers.Repeat
-00005640: 6564 436f 6d70 6f73 6974 6546 6965 6c64  edCompositeField
-00005650: 436f 6e74 6169 6e65 725b 6e75 636c 6961  Container[nuclia
-00005660: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-00005670: 6365 735f 7062 322e 4669 656c 6443 6f6d  ces_pb2.FieldCom
-00005680: 7075 7465 644d 6574 6164 6174 6157 7261  putedMetadataWra
-00005690: 7070 6572 5d3a 202e 2e2e 0a20 2020 2040  pper]: ....    @
-000056a0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-000056b0: 2066 6965 6c64 5f76 6563 746f 7273 2873   field_vectors(s
-000056c0: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
-000056d0: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
-000056e0: 2e63 6f6e 7461 696e 6572 732e 5265 7065  .containers.Repe
-000056f0: 6174 6564 436f 6d70 6f73 6974 6546 6965  atedCompositeFie
-00005700: 6c64 436f 6e74 6169 6e65 725b 6e75 636c  ldContainer[nucl
-00005710: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
-00005720: 7572 6365 735f 7062 322e 4578 7472 6163  urces_pb2.Extrac
-00005730: 7465 6456 6563 746f 7273 5772 6170 7065  tedVectorsWrappe
-00005740: 725d 3a20 2e2e 2e0a 2020 2020 4070 726f  r]: ....    @pro
-00005750: 7065 7274 790a 2020 2020 6465 6620 6669  perty.    def fi
-00005760: 656c 645f 6c61 7267 655f 6d65 7461 6461  eld_large_metada
-00005770: 7461 2873 656c 6629 202d 3e20 676f 6f67  ta(self) -> goog
-00005780: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
-00005790: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
-000057a0: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
-000057b0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
-000057c0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-000057d0: 7265 736f 7572 6365 735f 7062 322e 4c61  resources_pb2.La
-000057e0: 7267 6543 6f6d 7075 7465 644d 6574 6164  rgeComputedMetad
-000057f0: 6174 6157 7261 7070 6572 5d3a 0a20 2020  ataWrapper]:.   
-00005800: 2020 2020 2022 2222 5265 736f 7572 6365       """Resource
-00005810: 204c 6172 6765 2043 6f6d 7075 7465 6420   Large Computed 
-00005820: 4d65 7461 6461 7461 2222 220a 0a20 2020  Metadata"""..   
-00005830: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00005840: 6566 2064 656c 6574 655f 6669 656c 6473  ef delete_fields
-00005850: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
-00005860: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
-00005870: 616c 2e63 6f6e 7461 696e 6572 732e 5265  al.containers.Re
-00005880: 7065 6174 6564 436f 6d70 6f73 6974 6546  peatedCompositeF
-00005890: 6965 6c64 436f 6e74 6169 6e65 725b 6e75  ieldContainer[nu
-000058a0: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-000058b0: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
-000058c0: 6449 445d 3a20 2e2e 2e0a 2020 2020 4070  dID]: ....    @p
-000058d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000058e0: 646f 6e65 5f74 696d 6528 7365 6c66 2920  done_time(self) 
-000058f0: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
-00005900: 7566 2e74 696d 6573 7461 6d70 5f70 6232  uf.timestamp_pb2
-00005910: 2e54 696d 6573 7461 6d70 3a20 2e2e 2e0a  .Timestamp: ....
-00005920: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00005930: 2020 6465 6620 6572 726f 7273 2873 656c    def errors(sel
-00005940: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
-00005950: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
-00005960: 6f6e 7461 696e 6572 732e 5265 7065 6174  ontainers.Repeat
-00005970: 6564 436f 6d70 6f73 6974 6546 6965 6c64  edCompositeField
-00005980: 436f 6e74 6169 6e65 725b 676c 6f62 616c  Container[global
-00005990: 5f5f 5f45 7272 6f72 5d3a 202e 2e2e 0a20  ___Error]: .... 
-000059a0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000059b0: 2064 6566 2075 7365 725f 7665 6374 6f72   def user_vector
-000059c0: 7328 7365 6c66 2920 2d3e 2067 6f6f 676c  s(self) -> googl
-000059d0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
-000059e0: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
-000059f0: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
-00005a00: 4669 656c 6443 6f6e 7461 696e 6572 5b6e  FieldContainer[n
-00005a10: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00005a20: 6573 6f75 7263 6573 5f70 6232 2e55 7365  esources_pb2.Use
-00005a30: 7256 6563 746f 7273 5772 6170 7065 725d  rVectorsWrapper]
-00005a40: 3a20 2e2e 2e0a 2020 2020 4070 726f 7065  : ....    @prope
-00005a50: 7274 790a 2020 2020 6465 6620 6578 7472  rty.    def extr
-00005a60: 6128 7365 6c66 2920 2d3e 206e 7563 6c69  a(self) -> nucli
-00005a70: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
-00005a80: 7263 6573 5f70 6232 2e45 7874 7261 3a20  rces_pb2.Extra: 
-00005a90: 2e2e 2e0a 2020 2020 4070 726f 7065 7274  ....    @propert
-00005aa0: 790a 2020 2020 6465 6620 7175 6573 7469  y.    def questi
-00005ab0: 6f6e 5f61 6e73 7765 7273 2873 656c 6629  on_answers(self)
-00005ac0: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
-00005ad0: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
-00005ae0: 7461 696e 6572 732e 5265 7065 6174 6564  tainers.Repeated
-00005af0: 436f 6d70 6f73 6974 6546 6965 6c64 436f  CompositeFieldCo
-00005b00: 6e74 6169 6e65 725b 6e75 636c 6961 6462  ntainer[nucliadb
-00005b10: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-00005b20: 735f 7062 322e 4669 656c 6451 7565 7374  s_pb2.FieldQuest
-00005b30: 696f 6e41 6e73 7765 7257 7261 7070 6572  ionAnswerWrapper
-00005b40: 5d3a 202e 2e2e 0a20 2020 2040 7072 6f70  ]: ....    @prop
-00005b50: 6572 7479 0a20 2020 2064 6566 2073 6563  erty.    def sec
-00005b60: 7572 6974 7928 7365 6c66 2920 2d3e 206e  urity(self) -> n
-00005b70: 7563 6c69 6164 625f 7072 6f74 6f73 2e75  ucliadb_protos.u
-00005b80: 7469 6c73 5f70 6232 2e53 6563 7572 6974  tils_pb2.Securit
-00005b90: 793a 202e 2e2e 0a20 2020 2064 6566 205f  y: ....    def _
-00005ba0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00005bb0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-00005bc0: 2c0a 2020 2020 2020 2020 6b62 6964 3a20  ,.        kbid: 
-00005bd0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-00005be0: 2e2e 2c0a 2020 2020 2020 2020 7575 6964  ..,.        uuid
-00005bf0: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00005c00: 202e 2e2e 2c0a 2020 2020 2020 2020 736c   ...,.        sl
-00005c10: 7567 3a20 6275 696c 7469 6e73 2e73 7472  ug: builtins.str
-00005c20: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00005c30: 6175 6469 743a 2067 6c6f 6261 6c5f 5f5f  audit: global___
-00005c40: 4175 6469 7420 7c20 4e6f 6e65 203d 202e  Audit | None = .
-00005c50: 2e2e 2c0a 2020 2020 2020 2020 7479 7065  ..,.        type
-00005c60: 3a20 676c 6f62 616c 5f5f 5f42 726f 6b65  : global___Broke
-00005c70: 724d 6573 7361 6765 2e4d 6573 7361 6765  rMessage.Message
-00005c80: 5479 7065 2e56 616c 7565 5479 7065 203d  Type.ValueType =
-00005c90: 202e 2e2e 2c0a 2020 2020 2020 2020 6d75   ...,.        mu
-00005ca0: 6c74 6969 643a 2062 7569 6c74 696e 732e  ltiid: builtins.
-00005cb0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-00005cc0: 2020 2062 6173 6963 3a20 6e75 636c 6961     basic: nuclia
-00005cd0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-00005ce0: 6365 735f 7062 322e 4261 7369 6320 7c20  ces_pb2.Basic | 
-00005cf0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-00005d00: 2020 2020 6f72 6967 696e 3a20 6e75 636c      origin: nucl
-00005d10: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
-00005d20: 7572 6365 735f 7062 322e 4f72 6967 696e  urces_pb2.Origin
-00005d30: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-00005d40: 2020 2020 2020 2072 656c 6174 696f 6e73         relations
-00005d50: 3a20 636f 6c6c 6563 7469 6f6e 732e 6162  : collections.ab
-00005d60: 632e 4974 6572 6162 6c65 5b6e 7563 6c69  c.Iterable[nucli
-00005d70: 6164 625f 7072 6f74 6f73 2e75 7469 6c73  adb_protos.utils
-00005d80: 5f70 6232 2e52 656c 6174 696f 6e5d 207c  _pb2.Relation] |
-00005d90: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-00005da0: 2020 2020 2063 6f6e 7665 7273 6174 696f       conversatio
-00005db0: 6e73 3a20 636f 6c6c 6563 7469 6f6e 732e  ns: collections.
-00005dc0: 6162 632e 4d61 7070 696e 675b 6275 696c  abc.Mapping[buil
-00005dd0: 7469 6e73 2e73 7472 2c20 6e75 636c 6961  tins.str, nuclia
-00005de0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-00005df0: 6365 735f 7062 322e 436f 6e76 6572 7361  ces_pb2.Conversa
-00005e00: 7469 6f6e 5d20 7c20 4e6f 6e65 203d 202e  tion] | None = .
-00005e10: 2e2e 2c0a 2020 2020 2020 2020 6c61 796f  ..,.        layo
-00005e20: 7574 733a 2063 6f6c 6c65 6374 696f 6e73  uts: collections
-00005e30: 2e61 6263 2e4d 6170 7069 6e67 5b62 7569  .abc.Mapping[bui
-00005e40: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
-00005e50: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
-00005e60: 7263 6573 5f70 6232 2e46 6965 6c64 4c61  rces_pb2.FieldLa
-00005e70: 796f 7574 5d20 7c20 4e6f 6e65 203d 202e  yout] | None = .
-00005e80: 2e2e 2c0a 2020 2020 2020 2020 7465 7874  ..,.        text
-00005e90: 733a 2063 6f6c 6c65 6374 696f 6e73 2e61  s: collections.a
-00005ea0: 6263 2e4d 6170 7069 6e67 5b62 7569 6c74  bc.Mapping[built
-00005eb0: 696e 732e 7374 722c 206e 7563 6c69 6164  ins.str, nucliad
-00005ec0: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
-00005ed0: 6573 5f70 6232 2e46 6965 6c64 5465 7874  es_pb2.FieldText
-00005ee0: 5d20 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  ] | None = ...,.
-00005ef0: 2020 2020 2020 2020 6b65 7977 6f72 6473          keywords
-00005f00: 6574 733a 2063 6f6c 6c65 6374 696f 6e73  ets: collections
-00005f10: 2e61 6263 2e4d 6170 7069 6e67 5b62 7569  .abc.Mapping[bui
-00005f20: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
-00005f30: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
-00005f40: 7263 6573 5f70 6232 2e46 6965 6c64 4b65  rces_pb2.FieldKe
-00005f50: 7977 6f72 6473 6574 5d20 7c20 4e6f 6e65  ywordset] | None
-00005f60: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00005f70: 6461 7465 7469 6d65 733a 2063 6f6c 6c65  datetimes: colle
-00005f80: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
-00005f90: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
-00005fa0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00005fb0: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00005fc0: 6965 6c64 4461 7465 7469 6d65 5d20 7c20  ieldDatetime] | 
-00005fd0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-00005fe0: 2020 2020 6c69 6e6b 733a 2063 6f6c 6c65      links: colle
-00005ff0: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
-00006000: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
-00006010: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00006020: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
-00006030: 6965 6c64 4c69 6e6b 5d20 7c20 4e6f 6e65  ieldLink] | None
-00006040: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00006050: 6669 6c65 733a 2063 6f6c 6c65 6374 696f  files: collectio
-00006060: 6e73 2e61 6263 2e4d 6170 7069 6e67 5b62  ns.abc.Mapping[b
-00006070: 7569 6c74 696e 732e 7374 722c 206e 7563  uiltins.str, nuc
-00006080: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
-00006090: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
-000060a0: 4669 6c65 5d20 7c20 4e6f 6e65 203d 202e  File] | None = .
-000060b0: 2e2e 2c0a 2020 2020 2020 2020 6c69 6e6b  ..,.        link
-000060c0: 5f65 7874 7261 6374 6564 5f64 6174 613a  _extracted_data:
-000060d0: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-000060e0: 2e49 7465 7261 626c 655b 6e75 636c 6961  .Iterable[nuclia
-000060f0: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
-00006100: 6365 735f 7062 322e 4c69 6e6b 4578 7472  ces_pb2.LinkExtr
-00006110: 6163 7465 6444 6174 615d 207c 204e 6f6e  actedData] | Non
-00006120: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-00006130: 2066 696c 655f 6578 7472 6163 7465 645f   file_extracted_
-00006140: 6461 7461 3a20 636f 6c6c 6563 7469 6f6e  data: collection
-00006150: 732e 6162 632e 4974 6572 6162 6c65 5b6e  s.abc.Iterable[n
-00006160: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-00006170: 6573 6f75 7263 6573 5f70 6232 2e46 696c  esources_pb2.Fil
-00006180: 6545 7874 7261 6374 6564 4461 7461 5d20  eExtractedData] 
-00006190: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-000061a0: 2020 2020 2020 6578 7472 6163 7465 645f        extracted_
-000061b0: 7465 7874 3a20 636f 6c6c 6563 7469 6f6e  text: collection
-000061c0: 732e 6162 632e 4974 6572 6162 6c65 5b6e  s.abc.Iterable[n
-000061d0: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
-000061e0: 6573 6f75 7263 6573 5f70 6232 2e45 7874  esources_pb2.Ext
-000061f0: 7261 6374 6564 5465 7874 5772 6170 7065  ractedTextWrappe
-00006200: 725d 207c 204e 6f6e 6520 3d20 2e2e 2e2c  r] | None = ...,
-00006210: 0a20 2020 2020 2020 2066 6965 6c64 5f6d  .        field_m
-00006220: 6574 6164 6174 613a 2063 6f6c 6c65 6374  etadata: collect
-00006230: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
-00006240: 655b 6e75 636c 6961 6462 5f70 726f 746f  e[nucliadb_proto
-00006250: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-00006260: 4669 656c 6443 6f6d 7075 7465 644d 6574  FieldComputedMet
-00006270: 6164 6174 6157 7261 7070 6572 5d20 7c20  adataWrapper] | 
-00006280: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-00006290: 2020 2020 6669 656c 645f 7665 6374 6f72      field_vector
-000062a0: 733a 2063 6f6c 6c65 6374 696f 6e73 2e61  s: collections.a
-000062b0: 6263 2e49 7465 7261 626c 655b 6e75 636c  bc.Iterable[nucl
-000062c0: 6961 6462 5f70 726f 746f 732e 7265 736f  iadb_protos.reso
-000062d0: 7572 6365 735f 7062 322e 4578 7472 6163  urces_pb2.Extrac
-000062e0: 7465 6456 6563 746f 7273 5772 6170 7065  tedVectorsWrappe
-000062f0: 725d 207c 204e 6f6e 6520 3d20 2e2e 2e2c  r] | None = ...,
-00006300: 0a20 2020 2020 2020 2066 6965 6c64 5f6c  .        field_l
-00006310: 6172 6765 5f6d 6574 6164 6174 613a 2063  arge_metadata: c
-00006320: 6f6c 6c65 6374 696f 6e73 2e61 6263 2e49  ollections.abc.I
-00006330: 7465 7261 626c 655b 6e75 636c 6961 6462  terable[nucliadb
-00006340: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
-00006350: 735f 7062 322e 4c61 7267 6543 6f6d 7075  s_pb2.LargeCompu
-00006360: 7465 644d 6574 6164 6174 6157 7261 7070  tedMetadataWrapp
-00006370: 6572 5d20 7c20 4e6f 6e65 203d 202e 2e2e  er] | None = ...
-00006380: 2c0a 2020 2020 2020 2020 6465 6c65 7465  ,.        delete
-00006390: 5f66 6965 6c64 733a 2063 6f6c 6c65 6374  _fields: collect
-000063a0: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
-000063b0: 655b 6e75 636c 6961 6462 5f70 726f 746f  e[nucliadb_proto
-000063c0: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
-000063d0: 4669 656c 6449 445d 207c 204e 6f6e 6520  FieldID] | None 
-000063e0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 206f  = ...,.        o
-000063f0: 7269 6769 6e5f 7365 713a 2062 7569 6c74  rigin_seq: built
-00006400: 696e 732e 696e 7420 3d20 2e2e 2e2c 0a20  ins.int = ...,. 
-00006410: 2020 2020 2020 2073 6c6f 775f 7072 6f63         slow_proc
-00006420: 6573 7369 6e67 5f74 696d 653a 2062 7569  essing_time: bui
-00006430: 6c74 696e 732e 666c 6f61 7420 3d20 2e2e  ltins.float = ..
-00006440: 2e2c 0a20 2020 2020 2020 2070 7265 5f70  .,.        pre_p
-00006450: 726f 6365 7373 696e 675f 7469 6d65 3a20  rocessing_time: 
-00006460: 6275 696c 7469 6e73 2e66 6c6f 6174 203d  builtins.float =
-00006470: 202e 2e2e 2c0a 2020 2020 2020 2020 646f   ...,.        do
-00006480: 6e65 5f74 696d 653a 2067 6f6f 676c 652e  ne_time: google.
-00006490: 7072 6f74 6f62 7566 2e74 696d 6573 7461  protobuf.timesta
-000064a0: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
-000064b0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-000064c0: 2020 2020 2020 2074 7873 6571 6964 3a20         txseqid: 
-000064d0: 6275 696c 7469 6e73 2e69 6e74 203d 202e  builtins.int = .
-000064e0: 2e2e 2c0a 2020 2020 2020 2020 6572 726f  ..,.        erro
-000064f0: 7273 3a20 636f 6c6c 6563 7469 6f6e 732e  rs: collections.
-00006500: 6162 632e 4974 6572 6162 6c65 5b67 6c6f  abc.Iterable[glo
-00006510: 6261 6c5f 5f5f 4572 726f 725d 207c 204e  bal___Error] | N
-00006520: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-00006530: 2020 2070 726f 6365 7373 696e 675f 6964     processing_id
-00006540: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00006550: 202e 2e2e 2c0a 2020 2020 2020 2020 736f   ...,.        so
-00006560: 7572 6365 3a20 676c 6f62 616c 5f5f 5f42  urce: global___B
-00006570: 726f 6b65 724d 6573 7361 6765 2e4d 6573  rokerMessage.Mes
-00006580: 7361 6765 536f 7572 6365 2e56 616c 7565  sageSource.Value
-00006590: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
-000065a0: 2020 2020 6163 636f 756e 745f 7365 713a      account_seq:
-000065b0: 2062 7569 6c74 696e 732e 696e 7420 3d20   builtins.int = 
-000065c0: 2e2e 2e2c 0a20 2020 2020 2020 2075 7365  ...,.        use
-000065d0: 725f 7665 6374 6f72 733a 2063 6f6c 6c65  r_vectors: colle
-000065e0: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
-000065f0: 626c 655b 6e75 636c 6961 6462 5f70 726f  ble[nucliadb_pro
-00006600: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
-00006610: 322e 5573 6572 5665 6374 6f72 7357 7261  2.UserVectorsWra
-00006620: 7070 6572 5d20 7c20 4e6f 6e65 203d 202e  pper] | None = .
-00006630: 2e2e 2c0a 2020 2020 2020 2020 7265 696e  ..,.        rein
-00006640: 6465 783a 2062 7569 6c74 696e 732e 626f  dex: builtins.bo
-00006650: 6f6c 203d 202e 2e2e 2c0a 2020 2020 2020  ol = ...,.      
-00006660: 2020 6578 7472 613a 206e 7563 6c69 6164    extra: nucliad
-00006670: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
-00006680: 6573 5f70 6232 2e45 7874 7261 207c 204e  es_pb2.Extra | N
-00006690: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-000066a0: 2020 2071 7565 7374 696f 6e5f 616e 7377     question_answ
-000066b0: 6572 733a 2063 6f6c 6c65 6374 696f 6e73  ers: collections
-000066c0: 2e61 6263 2e49 7465 7261 626c 655b 6e75  .abc.Iterable[nu
-000066d0: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-000066e0: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
-000066f0: 6451 7565 7374 696f 6e41 6e73 7765 7257  dQuestionAnswerW
-00006700: 7261 7070 6572 5d20 7c20 4e6f 6e65 203d  rapper] | None =
-00006710: 202e 2e2e 2c0a 2020 2020 2020 2020 7365   ...,.        se
-00006720: 6375 7269 7479 3a20 6e75 636c 6961 6462  curity: nucliadb
-00006730: 5f70 726f 746f 732e 7574 696c 735f 7062  _protos.utils_pb
-00006740: 322e 5365 6375 7269 7479 207c 204e 6f6e  2.Security | Non
-00006750: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
-00006760: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-00006770: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-00006780: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00006790: 7970 696e 672e 4c69 7465 7261 6c5b 2261  yping.Literal["a
-000067a0: 7564 6974 222c 2062 2261 7564 6974 222c  udit", b"audit",
-000067b0: 2022 6261 7369 6322 2c20 6222 6261 7369   "basic", b"basi
-000067c0: 6322 2c20 2264 6f6e 655f 7469 6d65 222c  c", "done_time",
-000067d0: 2062 2264 6f6e 655f 7469 6d65 222c 2022   b"done_time", "
-000067e0: 6578 7472 6122 2c20 6222 6578 7472 6122  extra", b"extra"
-000067f0: 2c20 226f 7269 6769 6e22 2c20 6222 6f72  , "origin", b"or
-00006800: 6967 696e 222c 2022 7365 6375 7269 7479  igin", "security
-00006810: 222c 2062 2273 6563 7572 6974 7922 5d29  ", b"security"])
-00006820: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
-00006830: 6c3a 202e 2e2e 0a20 2020 2064 6566 2043  l: ....    def C
-00006840: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
-00006850: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-00006860: 6e67 2e4c 6974 6572 616c 5b22 6163 636f  ng.Literal["acco
-00006870: 756e 745f 7365 7122 2c20 6222 6163 636f  unt_seq", b"acco
-00006880: 756e 745f 7365 7122 2c20 2261 7564 6974  unt_seq", "audit
-00006890: 222c 2062 2261 7564 6974 222c 2022 6261  ", b"audit", "ba
-000068a0: 7369 6322 2c20 6222 6261 7369 6322 2c20  sic", b"basic", 
-000068b0: 2263 6f6e 7665 7273 6174 696f 6e73 222c  "conversations",
-000068c0: 2062 2263 6f6e 7665 7273 6174 696f 6e73   b"conversations
-000068d0: 222c 2022 6461 7465 7469 6d65 7322 2c20  ", "datetimes", 
-000068e0: 6222 6461 7465 7469 6d65 7322 2c20 2264  b"datetimes", "d
-000068f0: 656c 6574 655f 6669 656c 6473 222c 2062  elete_fields", b
-00006900: 2264 656c 6574 655f 6669 656c 6473 222c  "delete_fields",
-00006910: 2022 646f 6e65 5f74 696d 6522 2c20 6222   "done_time", b"
-00006920: 646f 6e65 5f74 696d 6522 2c20 2265 7272  done_time", "err
-00006930: 6f72 7322 2c20 6222 6572 726f 7273 222c  ors", b"errors",
-00006940: 2022 6578 7472 6122 2c20 6222 6578 7472   "extra", b"extr
-00006950: 6122 2c20 2265 7874 7261 6374 6564 5f74  a", "extracted_t
-00006960: 6578 7422 2c20 6222 6578 7472 6163 7465  ext", b"extracte
-00006970: 645f 7465 7874 222c 2022 6669 656c 645f  d_text", "field_
-00006980: 6c61 7267 655f 6d65 7461 6461 7461 222c  large_metadata",
-00006990: 2062 2266 6965 6c64 5f6c 6172 6765 5f6d   b"field_large_m
-000069a0: 6574 6164 6174 6122 2c20 2266 6965 6c64  etadata", "field
-000069b0: 5f6d 6574 6164 6174 6122 2c20 6222 6669  _metadata", b"fi
-000069c0: 656c 645f 6d65 7461 6461 7461 222c 2022  eld_metadata", "
-000069d0: 6669 656c 645f 7665 6374 6f72 7322 2c20  field_vectors", 
-000069e0: 6222 6669 656c 645f 7665 6374 6f72 7322  b"field_vectors"
-000069f0: 2c20 2266 696c 655f 6578 7472 6163 7465  , "file_extracte
-00006a00: 645f 6461 7461 222c 2062 2266 696c 655f  d_data", b"file_
-00006a10: 6578 7472 6163 7465 645f 6461 7461 222c  extracted_data",
-00006a20: 2022 6669 6c65 7322 2c20 6222 6669 6c65   "files", b"file
-00006a30: 7322 2c20 226b 6269 6422 2c20 6222 6b62  s", "kbid", b"kb
-00006a40: 6964 222c 2022 6b65 7977 6f72 6473 6574  id", "keywordset
-00006a50: 7322 2c20 6222 6b65 7977 6f72 6473 6574  s", b"keywordset
-00006a60: 7322 2c20 226c 6179 6f75 7473 222c 2062  s", "layouts", b
-00006a70: 226c 6179 6f75 7473 222c 2022 6c69 6e6b  "layouts", "link
-00006a80: 5f65 7874 7261 6374 6564 5f64 6174 6122  _extracted_data"
-00006a90: 2c20 6222 6c69 6e6b 5f65 7874 7261 6374  , b"link_extract
-00006aa0: 6564 5f64 6174 6122 2c20 226c 696e 6b73  ed_data", "links
-00006ab0: 222c 2062 226c 696e 6b73 222c 2022 6d75  ", b"links", "mu
-00006ac0: 6c74 6969 6422 2c20 6222 6d75 6c74 6969  ltiid", b"multii
-00006ad0: 6422 2c20 226f 7269 6769 6e22 2c20 6222  d", "origin", b"
-00006ae0: 6f72 6967 696e 222c 2022 6f72 6967 696e  origin", "origin
-00006af0: 5f73 6571 222c 2062 226f 7269 6769 6e5f  _seq", b"origin_
-00006b00: 7365 7122 2c20 2270 7265 5f70 726f 6365  seq", "pre_proce
-00006b10: 7373 696e 675f 7469 6d65 222c 2062 2270  ssing_time", b"p
-00006b20: 7265 5f70 726f 6365 7373 696e 675f 7469  re_processing_ti
-00006b30: 6d65 222c 2022 7072 6f63 6573 7369 6e67  me", "processing
-00006b40: 5f69 6422 2c20 6222 7072 6f63 6573 7369  _id", b"processi
-00006b50: 6e67 5f69 6422 2c20 2271 7565 7374 696f  ng_id", "questio
-00006b60: 6e5f 616e 7377 6572 7322 2c20 6222 7175  n_answers", b"qu
-00006b70: 6573 7469 6f6e 5f61 6e73 7765 7273 222c  estion_answers",
-00006b80: 2022 7265 696e 6465 7822 2c20 6222 7265   "reindex", b"re
-00006b90: 696e 6465 7822 2c20 2272 656c 6174 696f  index", "relatio
-00006ba0: 6e73 222c 2062 2272 656c 6174 696f 6e73  ns", b"relations
-00006bb0: 222c 2022 7365 6375 7269 7479 222c 2062  ", "security", b
-00006bc0: 2273 6563 7572 6974 7922 2c20 2273 6c6f  "security", "slo
-00006bd0: 775f 7072 6f63 6573 7369 6e67 5f74 696d  w_processing_tim
-00006be0: 6522 2c20 6222 736c 6f77 5f70 726f 6365  e", b"slow_proce
-00006bf0: 7373 696e 675f 7469 6d65 222c 2022 736c  ssing_time", "sl
-00006c00: 7567 222c 2062 2273 6c75 6722 2c20 2273  ug", b"slug", "s
-00006c10: 6f75 7263 6522 2c20 6222 736f 7572 6365  ource", b"source
-00006c20: 222c 2022 7465 7874 7322 2c20 6222 7465  ", "texts", b"te
-00006c30: 7874 7322 2c20 2274 7873 6571 6964 222c  xts", "txseqid",
-00006c40: 2062 2274 7873 6571 6964 222c 2022 7479   b"txseqid", "ty
-00006c50: 7065 222c 2062 2274 7970 6522 2c20 2275  pe", b"type", "u
-00006c60: 7365 725f 7665 6374 6f72 7322 2c20 6222  ser_vectors", b"
-00006c70: 7573 6572 5f76 6563 746f 7273 222c 2022  user_vectors", "
-00006c80: 7575 6964 222c 2062 2275 7569 6422 5d29  uuid", b"uuid"])
-00006c90: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
-00006ca0: 6c6f 6261 6c5f 5f5f 4272 6f6b 6572 4d65  lobal___BrokerMe
-00006cb0: 7373 6167 6520 3d20 4272 6f6b 6572 4d65  ssage = BrokerMe
-00006cc0: 7373 6167 650a 0a40 7479 7069 6e67 2e66  ssage..@typing.f
-00006cd0: 696e 616c 0a63 6c61 7373 2042 726f 6b65  inal.class Broke
-00006ce0: 724d 6573 7361 6765 426c 6f62 5265 6665  rMessageBlobRefe
-00006cf0: 7265 6e63 6528 676f 6f67 6c65 2e70 726f  rence(google.pro
-00006d00: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
-00006d10: 7373 6167 6529 3a0a 2020 2020 4445 5343  ssage):.    DESC
-00006d20: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
-00006d30: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
-00006d40: 6f72 2e44 6573 6372 6970 746f 720a 0a20  or.Descriptor.. 
-00006d50: 2020 204b 4249 445f 4649 454c 445f 4e55     KBID_FIELD_NU
-00006d60: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00006d70: 6e74 0a20 2020 2055 5549 445f 4649 454c  nt.    UUID_FIEL
-00006d80: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00006d90: 6e73 2e69 6e74 0a20 2020 2053 544f 5241  ns.int.    STORA
-00006da0: 4745 5f4b 4559 5f46 4945 4c44 5f4e 554d  GE_KEY_FIELD_NUM
-00006db0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-00006dc0: 740a 2020 2020 6b62 6964 3a20 6275 696c  t.    kbid: buil
-00006dd0: 7469 6e73 2e73 7472 0a20 2020 2075 7569  tins.str.    uui
-00006de0: 643a 2062 7569 6c74 696e 732e 7374 720a  d: builtins.str.
-00006df0: 2020 2020 7374 6f72 6167 655f 6b65 793a      storage_key:
-00006e00: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00006e10: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00006e20: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00006e30: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00006e40: 206b 6269 643a 2062 7569 6c74 696e 732e   kbid: builtins.
-00006e50: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-00006e60: 2020 2075 7569 643a 2062 7569 6c74 696e     uuid: builtin
-00006e70: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-00006e80: 2020 2020 2073 746f 7261 6765 5f6b 6579       storage_key
-00006e90: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00006ea0: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-00006eb0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-00006ec0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-00006ed0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00006ee0: 7069 6e67 2e4c 6974 6572 616c 5b22 6b62  ping.Literal["kb
-00006ef0: 6964 222c 2062 226b 6269 6422 2c20 2273  id", b"kbid", "s
-00006f00: 746f 7261 6765 5f6b 6579 222c 2062 2273  torage_key", b"s
-00006f10: 746f 7261 6765 5f6b 6579 222c 2022 7575  torage_key", "uu
-00006f20: 6964 222c 2062 2275 7569 6422 5d29 202d  id", b"uuid"]) -
-00006f30: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
-00006f40: 6261 6c5f 5f5f 4272 6f6b 6572 4d65 7373  bal___BrokerMess
-00006f50: 6167 6542 6c6f 6252 6566 6572 656e 6365  ageBlobReference
-00006f60: 203d 2042 726f 6b65 724d 6573 7361 6765   = BrokerMessage
-00006f70: 426c 6f62 5265 6665 7265 6e63 650a 0a40  BlobReference..@
-00006f80: 7479 7069 6e67 2e66 696e 616c 0a63 6c61  typing.final.cla
-00006f90: 7373 2057 7269 7465 7253 7461 7475 7352  ss WriterStatusR
-00006fa0: 6573 706f 6e73 6528 676f 6f67 6c65 2e70  esponse(google.p
-00006fb0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-00006fc0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-00006fd0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00006fe0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00006ff0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-00007000: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
-00007010: 616c 0a20 2020 2063 6c61 7373 204d 7367  al.    class Msg
-00007020: 6964 456e 7472 7928 676f 6f67 6c65 2e70  idEntry(google.p
-00007030: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-00007040: 4d65 7373 6167 6529 3a0a 2020 2020 2020  Message):.      
-00007050: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-00007060: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-00007070: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-00007080: 746f 720a 0a20 2020 2020 2020 204b 4559  tor..        KEY
-00007090: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-000070a0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-000070b0: 2020 2020 5641 4c55 455f 4649 454c 445f      VALUE_FIELD_
-000070c0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-000070d0: 2e69 6e74 0a20 2020 2020 2020 206b 6579  .int.        key
-000070e0: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
-000070f0: 2020 2020 2020 2076 616c 7565 3a20 6275         value: bu
-00007100: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
-00007110: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00007120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007130: 662c 0a20 2020 2020 2020 2020 2020 202a  f,.            *
-00007140: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
-00007150: 793a 2062 7569 6c74 696e 732e 7374 7220  y: builtins.str 
-00007160: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2020  = ...,.         
-00007170: 2020 2076 616c 7565 3a20 6275 696c 7469     value: builti
-00007180: 6e73 2e69 6e74 203d 202e 2e2e 2c0a 2020  ns.int = ...,.  
-00007190: 2020 2020 2020 2920 2d3e 204e 6f6e 653a        ) -> None:
-000071a0: 202e 2e2e 0a20 2020 2020 2020 2064 6566   ....        def
-000071b0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-000071c0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-000071d0: 7069 6e67 2e4c 6974 6572 616c 5b22 6b65  ping.Literal["ke
-000071e0: 7922 2c20 6222 6b65 7922 2c20 2276 616c  y", b"key", "val
-000071f0: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
-00007200: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 2020  -> None: .....  
-00007210: 2020 4b4e 4f57 4c45 4447 4542 4f58 4553    KNOWLEDGEBOXES
-00007220: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00007230: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00007240: 4d53 4749 445f 4649 454c 445f 4e55 4d42  MSGID_FIELD_NUMB
-00007250: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00007260: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00007270: 2020 2064 6566 206b 6e6f 776c 6564 6765     def knowledge
-00007280: 626f 7865 7328 7365 6c66 2920 2d3e 2067  boxes(self) -> g
-00007290: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
-000072a0: 6e74 6572 6e61 6c2e 636f 6e74 6169 6e65  nternal.containe
-000072b0: 7273 2e52 6570 6561 7465 6453 6361 6c61  rs.RepeatedScala
-000072c0: 7246 6965 6c64 436f 6e74 6169 6e65 725b  rFieldContainer[
-000072d0: 6275 696c 7469 6e73 2e73 7472 5d3a 202e  builtins.str]: .
-000072e0: 2e2e 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-000072f0: 0a20 2020 2064 6566 206d 7367 6964 2873  .    def msgid(s
-00007300: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
-00007310: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
-00007320: 2e63 6f6e 7461 696e 6572 732e 5363 616c  .containers.Scal
-00007330: 6172 4d61 705b 6275 696c 7469 6e73 2e73  arMap[builtins.s
-00007340: 7472 2c20 6275 696c 7469 6e73 2e69 6e74  tr, builtins.int
-00007350: 5d3a 0a20 2020 2020 2020 2022 2222 6d61  ]:.        """ma
-00007360: 7020 6f66 206c 6173 7420 6d65 7373 6167  p of last messag
-00007370: 6520 7072 6f63 6573 7365 6422 2222 0a0a  e processed"""..
-00007380: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00007390: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000073a0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-000073b0: 2020 206b 6e6f 776c 6564 6765 626f 7865     knowledgeboxe
-000073c0: 733a 2063 6f6c 6c65 6374 696f 6e73 2e61  s: collections.a
-000073d0: 6263 2e49 7465 7261 626c 655b 6275 696c  bc.Iterable[buil
-000073e0: 7469 6e73 2e73 7472 5d20 7c20 4e6f 6e65  tins.str] | None
-000073f0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00007400: 6d73 6769 643a 2063 6f6c 6c65 6374 696f  msgid: collectio
-00007410: 6e73 2e61 6263 2e4d 6170 7069 6e67 5b62  ns.abc.Mapping[b
-00007420: 7569 6c74 696e 732e 7374 722c 2062 7569  uiltins.str, bui
-00007430: 6c74 696e 732e 696e 745d 207c 204e 6f6e  ltins.int] | Non
-00007440: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
-00007450: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-00007460: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-00007470: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00007480: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00007490: 226b 6e6f 776c 6564 6765 626f 7865 7322  "knowledgeboxes"
-000074a0: 2c20 6222 6b6e 6f77 6c65 6467 6562 6f78  , b"knowledgebox
-000074b0: 6573 222c 2022 6d73 6769 6422 2c20 6222  es", "msgid", b"
-000074c0: 6d73 6769 6422 5d29 202d 3e20 4e6f 6e65  msgid"]) -> None
-000074d0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
-000074e0: 5772 6974 6572 5374 6174 7573 5265 7370  WriterStatusResp
-000074f0: 6f6e 7365 203d 2057 7269 7465 7253 7461  onse = WriterSta
-00007500: 7475 7352 6573 706f 6e73 650a 0a40 7479  tusResponse..@ty
-00007510: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
-00007520: 2057 7269 7465 7253 7461 7475 7352 6571   WriterStatusReq
-00007530: 7565 7374 2867 6f6f 676c 652e 7072 6f74  uest(google.prot
-00007540: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-00007550: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
-00007560: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-00007570: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-00007580: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-00007590: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000075a0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000075b0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
-000075c0: 0a0a 676c 6f62 616c 5f5f 5f57 7269 7465  ..global___Write
-000075d0: 7253 7461 7475 7352 6571 7565 7374 203d  rStatusRequest =
-000075e0: 2057 7269 7465 7253 7461 7475 7352 6571   WriterStatusReq
-000075f0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
-00007600: 6e61 6c0a 636c 6173 7320 5365 744c 6162  nal.class SetLab
-00007610: 656c 7352 6571 7565 7374 2867 6f6f 676c  elsRequest(googl
-00007620: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-00007630: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-00007640: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-00007650: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-00007660: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-00007670: 6f72 0a0a 2020 2020 4b42 5f46 4945 4c44  or..    KB_FIELD
-00007680: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00007690: 732e 696e 740a 2020 2020 4944 5f46 4945  s.int.    ID_FIE
-000076a0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-000076b0: 696e 732e 696e 740a 2020 2020 4c41 4245  ins.int.    LABE
-000076c0: 4c53 4554 5f46 4945 4c44 5f4e 554d 4245  LSET_FIELD_NUMBE
-000076d0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-000076e0: 2020 2020 6964 3a20 6275 696c 7469 6e73      id: builtins
-000076f0: 2e73 7472 0a20 2020 2040 7072 6f70 6572  .str.    @proper
-00007700: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
-00007710: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
-00007720: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-00007730: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
-00007740: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
-00007750: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00007760: 6620 6c61 6265 6c73 6574 2873 656c 6629  f labelset(self)
-00007770: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
-00007780: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-00007790: 5f70 6232 2e4c 6162 656c 5365 743a 202e  _pb2.LabelSet: .
-000077a0: 2e2e 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-000077b0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000077c0: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-000077d0: 2020 2020 2020 6b62 3a20 6e75 636c 6961        kb: nuclia
-000077e0: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-000077f0: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
-00007800: 6564 6765 426f 7849 4420 7c20 4e6f 6e65  edgeBoxID | None
-00007810: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00007820: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
-00007830: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00007840: 6c61 6265 6c73 6574 3a20 6e75 636c 6961  labelset: nuclia
-00007850: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
-00007860: 6467 6562 6f78 5f70 6232 2e4c 6162 656c  dgebox_pb2.Label
-00007870: 5365 7420 7c20 4e6f 6e65 203d 202e 2e2e  Set | None = ...
-00007880: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00007890: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
-000078a0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-000078b0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-000078c0: 6974 6572 616c 5b22 6b62 222c 2062 226b  iteral["kb", b"k
-000078d0: 6222 2c20 226c 6162 656c 7365 7422 2c20  b", "labelset", 
-000078e0: 6222 6c61 6265 6c73 6574 225d 2920 2d3e  b"labelset"]) ->
-000078f0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
-00007900: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
-00007910: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-00007920: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-00007930: 4c69 7465 7261 6c5b 2269 6422 2c20 6222  Literal["id", b"
-00007940: 6964 222c 2022 6b62 222c 2062 226b 6222  id", "kb", b"kb"
-00007950: 2c20 226c 6162 656c 7365 7422 2c20 6222  , "labelset", b"
-00007960: 6c61 6265 6c73 6574 225d 2920 2d3e 204e  labelset"]) -> N
-00007970: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
-00007980: 5f5f 5f53 6574 4c61 6265 6c73 5265 7175  ___SetLabelsRequ
-00007990: 6573 7420 3d20 5365 744c 6162 656c 7352  est = SetLabelsR
-000079a0: 6571 7565 7374 0a0a 4074 7970 696e 672e  equest..@typing.
-000079b0: 6669 6e61 6c0a 636c 6173 7320 4465 6c4c  final.class DelL
-000079c0: 6162 656c 7352 6571 7565 7374 2867 6f6f  abelsRequest(goo
-000079d0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-000079e0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-000079f0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-00007a00: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-00007a10: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-00007a20: 7074 6f72 0a0a 2020 2020 4b42 5f46 4945  ptor..    KB_FIE
-00007a30: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00007a40: 696e 732e 696e 740a 2020 2020 4944 5f46  ins.int.    ID_F
-00007a50: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00007a60: 6c74 696e 732e 696e 740a 2020 2020 6964  ltins.int.    id
-00007a70: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
-00007a80: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00007a90: 2064 6566 206b 6228 7365 6c66 2920 2d3e   def kb(self) ->
-00007aa0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00007ab0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-00007ac0: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
-00007ad0: 3a20 2e2e 2e0a 2020 2020 6465 6620 5f5f  : ....    def __
-00007ae0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00007af0: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-00007b00: 0a20 2020 2020 2020 206b 623a 206e 7563  .        kb: nuc
-00007b10: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-00007b20: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
-00007b30: 6f77 6c65 6467 6542 6f78 4944 207c 204e  owledgeBoxID | N
-00007b40: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-00007b50: 2020 2069 643a 2062 7569 6c74 696e 732e     id: builtins.
-00007b60: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2029  str = ...,.    )
-00007b70: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-00007b80: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
-00007b90: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00007ba0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00007bb0: 226b 6222 2c20 6222 6b62 225d 2920 2d3e  "kb", b"kb"]) ->
-00007bc0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
-00007bd0: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
-00007be0: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-00007bf0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-00007c00: 4c69 7465 7261 6c5b 2269 6422 2c20 6222  Literal["id", b"
-00007c10: 6964 222c 2022 6b62 222c 2062 226b 6222  id", "kb", b"kb"
-00007c20: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-00007c30: 0a67 6c6f 6261 6c5f 5f5f 4465 6c4c 6162  .global___DelLab
-00007c40: 656c 7352 6571 7565 7374 203d 2044 656c  elsRequest = Del
-00007c50: 4c61 6265 6c73 5265 7175 6573 740a 0a40  LabelsRequest..@
-00007c60: 7479 7069 6e67 2e66 696e 616c 0a63 6c61  typing.final.cla
-00007c70: 7373 2047 6574 4c61 6265 6c73 5265 7370  ss GetLabelsResp
-00007c80: 6f6e 7365 2867 6f6f 676c 652e 7072 6f74  onse(google.prot
-00007c90: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-00007ca0: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
-00007cb0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-00007cc0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-00007cd0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-00007ce0: 2020 636c 6173 7320 5f53 7461 7475 733a    class _Status:
-00007cf0: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
-00007d00: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
-00007d10: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
-00007d20: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
-00007d30: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
-00007d40: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
-00007d50: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
-00007d60: 650a 0a20 2020 2063 6c61 7373 205f 5374  e..    class _St
-00007d70: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
-00007d80: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
-00007d90: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
-00007da0: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
-00007db0: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
-00007dc0: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
-00007dd0: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
-00007de0: 7970 655d 2c20 6275 696c 7469 6e73 2e74  ype], builtins.t
-00007df0: 7970 6529 3a0a 2020 2020 2020 2020 4445  ype):.        DE
-00007e00: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00007e10: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00007e20: 7074 6f72 2e45 6e75 6d44 6573 6372 6970  ptor.EnumDescrip
-00007e30: 746f 720a 2020 2020 2020 2020 4f4b 3a20  tor.        OK: 
-00007e40: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
-00007e50: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
-00007e60: 7970 6520 2023 2030 0a20 2020 2020 2020  ype  # 0.       
-00007e70: 204e 4f54 464f 554e 443a 2047 6574 4c61   NOTFOUND: GetLa
-00007e80: 6265 6c73 5265 7370 6f6e 7365 2e5f 5374  belsResponse._St
-00007e90: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
-00007ea0: 2320 310a 0a20 2020 2063 6c61 7373 2053  # 1..    class S
-00007eb0: 7461 7475 7328 5f53 7461 7475 732c 206d  tatus(_Status, m
-00007ec0: 6574 6163 6c61 7373 3d5f 5374 6174 7573  etaclass=_Status
-00007ed0: 456e 756d 5479 7065 5772 6170 7065 7229  EnumTypeWrapper)
-00007ee0: 3a20 2e2e 2e0a 2020 2020 4f4b 3a20 4765  : ....    OK: Ge
-00007ef0: 744c 6162 656c 7352 6573 706f 6e73 652e  tLabelsResponse.
-00007f00: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-00007f10: 2020 2320 300a 2020 2020 4e4f 5446 4f55    # 0.    NOTFOU
-00007f20: 4e44 3a20 4765 744c 6162 656c 7352 6573  ND: GetLabelsRes
-00007f30: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-00007f40: 7565 5479 7065 2020 2320 310a 0a20 2020  ueType  # 1..   
-00007f50: 204b 425f 4649 454c 445f 4e55 4d42 4552   KB_FIELD_NUMBER
-00007f60: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00007f70: 2020 204c 4142 454c 535f 4649 454c 445f     LABELS_FIELD_
-00007f80: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00007f90: 2e69 6e74 0a20 2020 2053 5441 5455 535f  .int.    STATUS_
-00007fa0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00007fb0: 696c 7469 6e73 2e69 6e74 0a20 2020 2073  iltins.int.    s
-00007fc0: 7461 7475 733a 2067 6c6f 6261 6c5f 5f5f  tatus: global___
-00007fd0: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
-00007fe0: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-00007ff0: 7065 0a20 2020 2040 7072 6f70 6572 7479  pe.    @property
-00008000: 0a20 2020 2064 6566 206b 6228 7365 6c66  .    def kb(self
-00008010: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-00008020: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-00008030: 785f 7062 322e 4b6e 6f77 6c65 6467 6542  x_pb2.KnowledgeB
-00008040: 6f78 4944 3a20 2e2e 2e0a 2020 2020 4070  oxID: ....    @p
-00008050: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00008060: 6c61 6265 6c73 2873 656c 6629 202d 3e20  labels(self) -> 
-00008070: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-00008080: 6b6e 6f77 6c65 6467 6562 6f78 5f70 6232  knowledgebox_pb2
-00008090: 2e4c 6162 656c 733a 202e 2e2e 0a20 2020  .Labels: ....   
-000080a0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-000080b0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000080c0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-000080d0: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
-000080e0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-000080f0: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
-00008100: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
-00008110: 2c0a 2020 2020 2020 2020 6c61 6265 6c73  ,.        labels
-00008120: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-00008130: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-00008140: 6232 2e4c 6162 656c 7320 7c20 4e6f 6e65  b2.Labels | None
-00008150: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00008160: 7374 6174 7573 3a20 676c 6f62 616c 5f5f  status: global__
-00008170: 5f47 6574 4c61 6265 6c73 5265 7370 6f6e  _GetLabelsRespon
-00008180: 7365 2e53 7461 7475 732e 5661 6c75 6554  se.Status.ValueT
-00008190: 7970 6520 3d20 2e2e 2e2c 0a20 2020 2029  ype = ...,.    )
-000081a0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-000081b0: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
-000081c0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-000081d0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-000081e0: 226b 6222 2c20 6222 6b62 222c 2022 6c61  "kb", b"kb", "la
-000081f0: 6265 6c73 222c 2062 226c 6162 656c 7322  bels", b"labels"
-00008200: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
-00008210: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
-00008220: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-00008230: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00008240: 7069 6e67 2e4c 6974 6572 616c 5b22 6b62  ping.Literal["kb
-00008250: 222c 2062 226b 6222 2c20 226c 6162 656c  ", b"kb", "label
-00008260: 7322 2c20 6222 6c61 6265 6c73 222c 2022  s", b"labels", "
-00008270: 7374 6174 7573 222c 2062 2273 7461 7475  status", b"statu
-00008280: 7322 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  s"]) -> None: ..
-00008290: 2e0a 0a67 6c6f 6261 6c5f 5f5f 4765 744c  ...global___GetL
-000082a0: 6162 656c 7352 6573 706f 6e73 6520 3d20  abelsResponse = 
-000082b0: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
-000082c0: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
-000082d0: 0a63 6c61 7373 2047 6574 4c61 6265 6c73  .class GetLabels
-000082e0: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
-000082f0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-00008300: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-00008310: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00008320: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00008330: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-00008340: 0a20 2020 204b 425f 4649 454c 445f 4e55  .    KB_FIELD_NU
-00008350: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00008360: 6e74 0a20 2020 2040 7072 6f70 6572 7479  nt.    @property
-00008370: 0a20 2020 2064 6566 206b 6228 7365 6c66  .    def kb(self
-00008380: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
-00008390: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
-000083a0: 785f 7062 322e 4b6e 6f77 6c65 6467 6542  x_pb2.KnowledgeB
-000083b0: 6f78 4944 3a20 2e2e 2e0a 2020 2020 6465  oxID: ....    de
-000083c0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-000083d0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000083e0: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
-000083f0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00008400: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-00008410: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
-00008420: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-00008430: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-00008440: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
-00008450: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-00008460: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-00008470: 7261 6c5b 226b 6222 2c20 6222 6b62 225d  ral["kb", b"kb"]
-00008480: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-00008490: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
-000084a0: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
-000084b0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-000084c0: 696e 672e 4c69 7465 7261 6c5b 226b 6222  ing.Literal["kb"
-000084d0: 2c20 6222 6b62 225d 2920 2d3e 204e 6f6e  , b"kb"]) -> Non
-000084e0: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
-000084f0: 5f47 6574 4c61 6265 6c73 5265 7175 6573  _GetLabelsReques
-00008500: 7420 3d20 4765 744c 6162 656c 7352 6571  t = GetLabelsReq
-00008510: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
-00008520: 6e61 6c0a 636c 6173 7320 4e65 7745 6e74  nal.class NewEnt
-00008530: 6974 6965 7347 726f 7570 5265 7175 6573  itiesGroupReques
-00008540: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
-00008550: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-00008560: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-00008570: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-00008580: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-00008590: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
-000085a0: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
-000085b0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-000085c0: 2047 524f 5550 5f46 4945 4c44 5f4e 554d   GROUP_FIELD_NUM
-000085d0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-000085e0: 740a 2020 2020 454e 5449 5449 4553 5f46  t.    ENTITIES_F
-000085f0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00008600: 6c74 696e 732e 696e 740a 2020 2020 6772  ltins.int.    gr
-00008610: 6f75 703a 2062 7569 6c74 696e 732e 7374  oup: builtins.st
-00008620: 720a 2020 2020 4070 726f 7065 7274 790a  r.    @property.
-00008630: 2020 2020 6465 6620 6b62 2873 656c 6629      def kb(self)
-00008640: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
-00008650: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-00008660: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
-00008670: 7849 443a 202e 2e2e 0a20 2020 2040 7072  xID: ....    @pr
-00008680: 6f70 6572 7479 0a20 2020 2064 6566 2065  operty.    def e
-00008690: 6e74 6974 6965 7328 7365 6c66 2920 2d3e  ntities(self) ->
-000086a0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-000086b0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-000086c0: 322e 456e 7469 7469 6573 4772 6f75 703a  2.EntitiesGroup:
-000086d0: 202e 2e2e 0a20 2020 2064 6566 205f 5f69   ....    def __i
-000086e0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-000086f0: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
-00008700: 2020 2020 2020 2020 6b62 3a20 6e75 636c          kb: nucl
-00008710: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-00008720: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
-00008730: 776c 6564 6765 426f 7849 4420 7c20 4e6f  wledgeBoxID | No
-00008740: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00008750: 2020 6772 6f75 703a 2062 7569 6c74 696e    group: builtin
-00008760: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-00008770: 2020 2020 2065 6e74 6974 6965 733a 206e       entities: n
-00008780: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-00008790: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-000087a0: 456e 7469 7469 6573 4772 6f75 7020 7c20  EntitiesGroup | 
-000087b0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-000087c0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-000087d0: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
-000087e0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-000087f0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-00008800: 5b22 656e 7469 7469 6573 222c 2062 2265  ["entities", b"e
-00008810: 6e74 6974 6965 7322 2c20 226b 6222 2c20  ntities", "kb", 
-00008820: 6222 6b62 225d 2920 2d3e 2062 7569 6c74  b"kb"]) -> built
-00008830: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
-00008840: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
-00008850: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-00008860: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-00008870: 6c5b 2265 6e74 6974 6965 7322 2c20 6222  l["entities", b"
-00008880: 656e 7469 7469 6573 222c 2022 6772 6f75  entities", "grou
-00008890: 7022 2c20 6222 6772 6f75 7022 2c20 226b  p", b"group", "k
-000088a0: 6222 2c20 6222 6b62 225d 2920 2d3e 204e  b", b"kb"]) -> N
-000088b0: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
-000088c0: 5f5f 5f4e 6577 456e 7469 7469 6573 4772  ___NewEntitiesGr
-000088d0: 6f75 7052 6571 7565 7374 203d 204e 6577  oupRequest = New
-000088e0: 456e 7469 7469 6573 4772 6f75 7052 6571  EntitiesGroupReq
-000088f0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
-00008900: 6e61 6c0a 636c 6173 7320 4e65 7745 6e74  nal.class NewEnt
-00008910: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
-00008920: 7365 2867 6f6f 676c 652e 7072 6f74 6f62  se(google.protob
-00008930: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
-00008940: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
-00008950: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-00008960: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-00008970: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
-00008980: 636c 6173 7320 5f53 7461 7475 733a 0a20  class _Status:. 
-00008990: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
-000089a0: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
-000089b0: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
-000089c0: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
-000089d0: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
-000089e0: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
-000089f0: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
-00008a00: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
-00008a10: 7573 456e 756d 5479 7065 5772 6170 7065  usEnumTypeWrappe
-00008a20: 7228 676f 6f67 6c65 2e70 726f 746f 6275  r(google.protobu
-00008a30: 662e 696e 7465 726e 616c 2e65 6e75 6d5f  f.internal.enum_
-00008a40: 7479 7065 5f77 7261 7070 6572 2e5f 456e  type_wrapper._En
-00008a50: 756d 5479 7065 5772 6170 7065 725b 4e65  umTypeWrapper[Ne
-00008a60: 7745 6e74 6974 6965 7347 726f 7570 5265  wEntitiesGroupRe
-00008a70: 7370 6f6e 7365 2e5f 5374 6174 7573 2e56  sponse._Status.V
-00008a80: 616c 7565 5479 7065 5d2c 2062 7569 6c74  alueType], built
-00008a90: 696e 732e 7479 7065 293a 0a20 2020 2020  ins.type):.     
-00008aa0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-00008ab0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-00008ac0: 6573 6372 6970 746f 722e 456e 756d 4465  escriptor.EnumDe
-00008ad0: 7363 7269 7074 6f72 0a20 2020 2020 2020  scriptor.       
-00008ae0: 204f 4b3a 204e 6577 456e 7469 7469 6573   OK: NewEntities
-00008af0: 4772 6f75 7052 6573 706f 6e73 652e 5f53  GroupResponse._S
-00008b00: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-00008b10: 2023 2030 0a20 2020 2020 2020 2045 5252   # 0.        ERR
-00008b20: 4f52 3a20 4e65 7745 6e74 6974 6965 7347  OR: NewEntitiesG
-00008b30: 726f 7570 5265 7370 6f6e 7365 2e5f 5374  roupResponse._St
-00008b40: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
-00008b50: 2320 310a 2020 2020 2020 2020 4b42 5f4e  # 1.        KB_N
-00008b60: 4f54 5f46 4f55 4e44 3a20 4e65 7745 6e74  OT_FOUND: NewEnt
-00008b70: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
-00008b80: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
-00008b90: 5479 7065 2020 2320 320a 2020 2020 2020  Type  # 2.      
-00008ba0: 2020 414c 5245 4144 595f 4558 4953 5453    ALREADY_EXISTS
-00008bb0: 3a20 4e65 7745 6e74 6974 6965 7347 726f  : NewEntitiesGro
-00008bc0: 7570 5265 7370 6f6e 7365 2e5f 5374 6174  upResponse._Stat
-00008bd0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-00008be0: 330a 0a20 2020 2063 6c61 7373 2053 7461  3..    class Sta
-00008bf0: 7475 7328 5f53 7461 7475 732c 206d 6574  tus(_Status, met
-00008c00: 6163 6c61 7373 3d5f 5374 6174 7573 456e  aclass=_StatusEn
-00008c10: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
-00008c20: 2e2e 2e0a 2020 2020 4f4b 3a20 4e65 7745  ....    OK: NewE
-00008c30: 6e74 6974 6965 7347 726f 7570 5265 7370  ntitiesGroupResp
-00008c40: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
-00008c50: 6554 7970 6520 2023 2030 0a20 2020 2045  eType  # 0.    E
-00008c60: 5252 4f52 3a20 4e65 7745 6e74 6974 6965  RROR: NewEntitie
-00008c70: 7347 726f 7570 5265 7370 6f6e 7365 2e53  sGroupResponse.S
-00008c80: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-00008c90: 2023 2031 0a20 2020 204b 425f 4e4f 545f   # 1.    KB_NOT_
-00008ca0: 464f 554e 443a 204e 6577 456e 7469 7469  FOUND: NewEntiti
-00008cb0: 6573 4772 6f75 7052 6573 706f 6e73 652e  esGroupResponse.
-00008cc0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-00008cd0: 2020 2320 320a 2020 2020 414c 5245 4144    # 2.    ALREAD
-00008ce0: 595f 4558 4953 5453 3a20 4e65 7745 6e74  Y_EXISTS: NewEnt
-00008cf0: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
-00008d00: 7365 2e53 7461 7475 732e 5661 6c75 6554  se.Status.ValueT
-00008d10: 7970 6520 2023 2033 0a0a 2020 2020 5354  ype  # 3..    ST
-00008d20: 4154 5553 5f46 4945 4c44 5f4e 554d 4245  ATUS_FIELD_NUMBE
-00008d30: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00008d40: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
-00008d50: 616c 5f5f 5f4e 6577 456e 7469 7469 6573  al___NewEntities
-00008d60: 4772 6f75 7052 6573 706f 6e73 652e 5374  GroupResponse.St
-00008d70: 6174 7573 2e56 616c 7565 5479 7065 0a20  atus.ValueType. 
-00008d80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00008d90: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00008da0: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00008db0: 2020 7374 6174 7573 3a20 676c 6f62 616c    status: global
-00008dc0: 5f5f 5f4e 6577 456e 7469 7469 6573 4772  ___NewEntitiesGr
-00008dd0: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
-00008de0: 7573 2e56 616c 7565 5479 7065 203d 202e  us.ValueType = .
-00008df0: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
-00008e00: 653a 202e 2e2e 0a20 2020 2064 6566 2043  e: ....    def C
-00008e10: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
-00008e20: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-00008e30: 6e67 2e4c 6974 6572 616c 5b22 7374 6174  ng.Literal["stat
-00008e40: 7573 222c 2062 2273 7461 7475 7322 5d29  us", b"status"])
-00008e50: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
-00008e60: 6c6f 6261 6c5f 5f5f 4e65 7745 6e74 6974  lobal___NewEntit
-00008e70: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
-00008e80: 203d 204e 6577 456e 7469 7469 6573 4772   = NewEntitiesGr
-00008e90: 6f75 7052 6573 706f 6e73 650a 0a40 7479  oupResponse..@ty
-00008ea0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
-00008eb0: 2053 6574 456e 7469 7469 6573 5265 7175   SetEntitiesRequ
-00008ec0: 6573 7428 676f 6f67 6c65 2e70 726f 746f  est(google.proto
-00008ed0: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
-00008ee0: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
-00008ef0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-00008f00: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-00008f10: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
-00008f20: 204b 425f 4649 454c 445f 4e55 4d42 4552   KB_FIELD_NUMBER
-00008f30: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00008f40: 2020 2047 524f 5550 5f46 4945 4c44 5f4e     GROUP_FIELD_N
-00008f50: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00008f60: 696e 740a 2020 2020 454e 5449 5449 4553  int.    ENTITIES
-00008f70: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00008f80: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00008f90: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
-00008fa0: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
-00008fb0: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
-00008fc0: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
-00008fd0: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
-00008fe0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
-00008ff0: 426f 7849 443a 202e 2e2e 0a20 2020 2040  BoxID: ....    @
-00009000: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00009010: 2065 6e74 6974 6965 7328 7365 6c66 2920   entities(self) 
-00009020: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
-00009030: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-00009040: 7062 322e 456e 7469 7469 6573 4772 6f75  pb2.EntitiesGrou
-00009050: 703a 202e 2e2e 0a20 2020 2064 6566 205f  p: ....    def _
-00009060: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00009070: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-00009080: 2c0a 2020 2020 2020 2020 6b62 3a20 6e75  ,.        kb: nu
-00009090: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
-000090a0: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
-000090b0: 6e6f 776c 6564 6765 426f 7849 4420 7c20  nowledgeBoxID | 
-000090c0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-000090d0: 2020 2020 6772 6f75 703a 2062 7569 6c74      group: built
-000090e0: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-000090f0: 2020 2020 2020 2065 6e74 6974 6965 733a         entities:
-00009100: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00009110: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-00009120: 322e 456e 7469 7469 6573 4772 6f75 7020  2.EntitiesGroup 
-00009130: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-00009140: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
-00009150: 0a20 2020 2064 6566 2048 6173 4669 656c  .    def HasFiel
-00009160: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-00009170: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-00009180: 616c 5b22 656e 7469 7469 6573 222c 2062  al["entities", b
-00009190: 2265 6e74 6974 6965 7322 2c20 226b 6222  "entities", "kb"
-000091a0: 2c20 6222 6b62 225d 2920 2d3e 2062 7569  , b"kb"]) -> bui
-000091b0: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
-000091c0: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
-000091d0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-000091e0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-000091f0: 7261 6c5b 2265 6e74 6974 6965 7322 2c20  ral["entities", 
-00009200: 6222 656e 7469 7469 6573 222c 2022 6772  b"entities", "gr
-00009210: 6f75 7022 2c20 6222 6772 6f75 7022 2c20  oup", b"group", 
-00009220: 226b 6222 2c20 6222 6b62 225d 2920 2d3e  "kb", b"kb"]) ->
-00009230: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
-00009240: 616c 5f5f 5f53 6574 456e 7469 7469 6573  al___SetEntities
-00009250: 5265 7175 6573 7420 3d20 5365 7445 6e74  Request = SetEnt
-00009260: 6974 6965 7352 6571 7565 7374 0a0a 4074  itiesRequest..@t
-00009270: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
-00009280: 7320 5570 6461 7465 456e 7469 7469 6573  s UpdateEntities
-00009290: 4772 6f75 7052 6571 7565 7374 2867 6f6f  GroupRequest(goo
-000092a0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-000092b0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-000092c0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-000092d0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-000092e0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-000092f0: 7074 6f72 0a0a 2020 2020 4074 7970 696e  ptor..    @typin
-00009300: 672e 6669 6e61 6c0a 2020 2020 636c 6173  g.final.    clas
-00009310: 7320 4164 6445 6e74 7279 2867 6f6f 676c  s AddEntry(googl
-00009320: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-00009330: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-00009340: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
-00009350: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00009360: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-00009370: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
-00009380: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
-00009390: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-000093a0: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
-000093b0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-000093c0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
-000093d0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
-000093e0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
-000093f0: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
-00009400: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
-00009410: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-00009420: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-00009430: 456e 7469 7479 3a20 2e2e 2e0a 2020 2020  Entity: ....    
-00009440: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00009450: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00009460: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00009470: 2a2c 0a20 2020 2020 2020 2020 2020 206b  *,.            k
-00009480: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
-00009490: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-000094a0: 2020 2020 7661 6c75 653a 206e 7563 6c69      value: nucli
-000094b0: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-000094c0: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
-000094d0: 7479 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ty | None = ...,
-000094e0: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
-000094f0: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
-00009500: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-00009510: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00009520: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
-00009530: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
-00009540: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-00009550: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
-00009560: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-00009570: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-00009580: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00009590: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
-000095a0: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
-000095b0: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-000095c0: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
-000095d0: 616c 0a20 2020 2063 6c61 7373 2055 7064  al.    class Upd
-000095e0: 6174 6545 6e74 7279 2867 6f6f 676c 652e  ateEntry(google.
-000095f0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
-00009600: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
-00009610: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-00009620: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-00009630: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-00009640: 7074 6f72 0a0a 2020 2020 2020 2020 4b45  ptor..        KE
-00009650: 595f 4649 454c 445f 4e55 4d42 4552 3a20  Y_FIELD_NUMBER: 
-00009660: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00009670: 2020 2020 2056 414c 5545 5f46 4945 4c44       VALUE_FIELD
-00009680: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00009690: 732e 696e 740a 2020 2020 2020 2020 6b65  s.int.        ke
-000096a0: 793a 2062 7569 6c74 696e 732e 7374 720a  y: builtins.str.
-000096b0: 2020 2020 2020 2020 4070 726f 7065 7274          @propert
-000096c0: 790a 2020 2020 2020 2020 6465 6620 7661  y.        def va
-000096d0: 6c75 6528 7365 6c66 2920 2d3e 206e 7563  lue(self) -> nuc
-000096e0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-000096f0: 776c 6564 6765 626f 785f 7062 322e 456e  wledgebox_pb2.En
-00009700: 7469 7479 3a20 2e2e 2e0a 2020 2020 2020  tity: ....      
-00009710: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00009720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009730: 2c0a 2020 2020 2020 2020 2020 2020 2a2c  ,.            *,
-00009740: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
-00009750: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00009760: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-00009770: 2020 7661 6c75 653a 206e 7563 6c69 6164    value: nucliad
-00009780: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-00009790: 6765 626f 785f 7062 322e 456e 7469 7479  gebox_pb2.Entity
-000097a0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-000097b0: 2020 2020 2020 2029 202d 3e20 4e6f 6e65         ) -> None
-000097c0: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
-000097d0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
-000097e0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-000097f0: 696e 672e 4c69 7465 7261 6c5b 2276 616c  ing.Literal["val
-00009800: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
-00009810: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
-00009820: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
-00009830: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
-00009840: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-00009850: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-00009860: 6579 222c 2062 226b 6579 222c 2022 7661  ey", b"key", "va
-00009870: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
-00009880: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20   -> None: ..... 
-00009890: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
-000098a0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-000098b0: 0a20 2020 2047 524f 5550 5f46 4945 4c44  .    GROUP_FIELD
-000098c0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-000098d0: 732e 696e 740a 2020 2020 4144 445f 4649  s.int.    ADD_FI
-000098e0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-000098f0: 7469 6e73 2e69 6e74 0a20 2020 2055 5044  tins.int.    UPD
-00009900: 4154 455f 4649 454c 445f 4e55 4d42 4552  ATE_FIELD_NUMBER
-00009910: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00009920: 2020 2044 454c 4554 455f 4649 454c 445f     DELETE_FIELD_
-00009930: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00009940: 2e69 6e74 0a20 2020 2054 4954 4c45 5f46  .int.    TITLE_F
-00009950: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00009960: 6c74 696e 732e 696e 740a 2020 2020 434f  ltins.int.    CO
-00009970: 4c4f 525f 4649 454c 445f 4e55 4d42 4552  LOR_FIELD_NUMBER
-00009980: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00009990: 2020 2067 726f 7570 3a20 6275 696c 7469     group: builti
-000099a0: 6e73 2e73 7472 0a20 2020 2074 6974 6c65  ns.str.    title
-000099b0: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
-000099c0: 2020 2063 6f6c 6f72 3a20 6275 696c 7469     color: builti
-000099d0: 6e73 2e73 7472 0a20 2020 2040 7072 6f70  ns.str.    @prop
-000099e0: 6572 7479 0a20 2020 2064 6566 206b 6228  erty.    def kb(
-000099f0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-00009a00: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-00009a10: 6765 626f 785f 7062 322e 4b6e 6f77 6c65  gebox_pb2.Knowle
-00009a20: 6467 6542 6f78 4944 3a20 2e2e 2e0a 2020  dgeBoxID: ....  
-00009a30: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00009a40: 6465 6620 6164 6428 7365 6c66 2920 2d3e  def add(self) ->
-00009a50: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00009a60: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
-00009a70: 6e65 7273 2e4d 6573 7361 6765 4d61 705b  ners.MessageMap[
-00009a80: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
-00009a90: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
-00009aa0: 6f77 6c65 6467 6562 6f78 5f70 6232 2e45  owledgebox_pb2.E
-00009ab0: 6e74 6974 795d 3a0a 2020 2020 2020 2020  ntity]:.        
-00009ac0: 2222 2265 6e74 6974 795f 6964 3a20 456e  """entity_id: En
-00009ad0: 7469 7479 2222 220a 0a20 2020 2040 7072  tity"""..    @pr
-00009ae0: 6f70 6572 7479 0a20 2020 2064 6566 2075  operty.    def u
-00009af0: 7064 6174 6528 7365 6c66 2920 2d3e 2067  pdate(self) -> g
-00009b00: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
-00009b10: 6e74 6572 6e61 6c2e 636f 6e74 6169 6e65  nternal.containe
-00009b20: 7273 2e4d 6573 7361 6765 4d61 705b 6275  rs.MessageMap[bu
-00009b30: 696c 7469 6e73 2e73 7472 2c20 6e75 636c  iltins.str, nucl
-00009b40: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-00009b50: 6c65 6467 6562 6f78 5f70 6232 2e45 6e74  ledgebox_pb2.Ent
-00009b60: 6974 795d 3a0a 2020 2020 2020 2020 2222  ity]:.        ""
-00009b70: 2265 6e74 6974 795f 6964 3a20 456e 7469  "entity_id: Enti
-00009b80: 7479 2222 220a 0a20 2020 2040 7072 6f70  ty"""..    @prop
-00009b90: 6572 7479 0a20 2020 2064 6566 2064 656c  erty.    def del
-00009ba0: 6574 6528 7365 6c66 2920 2d3e 2067 6f6f  ete(self) -> goo
-00009bb0: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-00009bc0: 6572 6e61 6c2e 636f 6e74 6169 6e65 7273  ernal.containers
-00009bd0: 2e52 6570 6561 7465 6453 6361 6c61 7246  .RepeatedScalarF
-00009be0: 6965 6c64 436f 6e74 6169 6e65 725b 6275  ieldContainer[bu
-00009bf0: 696c 7469 6e73 2e73 7472 5d3a 0a20 2020  iltins.str]:.   
-00009c00: 2020 2020 2022 2222 656e 7469 7479 5f69       """entity_i
-00009c10: 6422 2222 0a0a 2020 2020 6465 6620 5f5f  d"""..    def __
-00009c20: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00009c30: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-00009c40: 0a20 2020 2020 2020 206b 623a 206e 7563  .        kb: nuc
-00009c50: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-00009c60: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
-00009c70: 6f77 6c65 6467 6542 6f78 4944 207c 204e  owledgeBoxID | N
-00009c80: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-00009c90: 2020 2067 726f 7570 3a20 6275 696c 7469     group: builti
-00009ca0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00009cb0: 2020 2020 2020 6164 643a 2063 6f6c 6c65        add: colle
-00009cc0: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
-00009cd0: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
-00009ce0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-00009cf0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-00009d00: 322e 456e 7469 7479 5d20 7c20 4e6f 6e65  2.Entity] | None
-00009d10: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00009d20: 7570 6461 7465 3a20 636f 6c6c 6563 7469  update: collecti
-00009d30: 6f6e 732e 6162 632e 4d61 7070 696e 675b  ons.abc.Mapping[
-00009d40: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
-00009d50: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
-00009d60: 6f77 6c65 6467 6562 6f78 5f70 6232 2e45  owledgebox_pb2.E
-00009d70: 6e74 6974 795d 207c 204e 6f6e 6520 3d20  ntity] | None = 
-00009d80: 2e2e 2e2c 0a20 2020 2020 2020 2064 656c  ...,.        del
-00009d90: 6574 653a 2063 6f6c 6c65 6374 696f 6e73  ete: collections
-00009da0: 2e61 6263 2e49 7465 7261 626c 655b 6275  .abc.Iterable[bu
-00009db0: 696c 7469 6e73 2e73 7472 5d20 7c20 4e6f  iltins.str] | No
-00009dc0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
-00009dd0: 2020 7469 746c 653a 2062 7569 6c74 696e    title: builtin
-00009de0: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-00009df0: 2020 2020 2063 6f6c 6f72 3a20 6275 696c       color: buil
-00009e00: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
-00009e10: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
-00009e20: 2e2e 0a20 2020 2064 6566 2048 6173 4669  ...    def HasFi
-00009e30: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
-00009e40: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
-00009e50: 6572 616c 5b22 6b62 222c 2062 226b 6222  eral["kb", b"kb"
-00009e60: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
-00009e70: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
-00009e80: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-00009e90: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-00009ea0: 7069 6e67 2e4c 6974 6572 616c 5b22 6164  ping.Literal["ad
-00009eb0: 6422 2c20 6222 6164 6422 2c20 2263 6f6c  d", b"add", "col
-00009ec0: 6f72 222c 2062 2263 6f6c 6f72 222c 2022  or", b"color", "
-00009ed0: 6465 6c65 7465 222c 2062 2264 656c 6574  delete", b"delet
-00009ee0: 6522 2c20 2267 726f 7570 222c 2062 2267  e", "group", b"g
-00009ef0: 726f 7570 222c 2022 6b62 222c 2062 226b  roup", "kb", b"k
-00009f00: 6222 2c20 2274 6974 6c65 222c 2062 2274  b", "title", b"t
-00009f10: 6974 6c65 222c 2022 7570 6461 7465 222c  itle", "update",
-00009f20: 2062 2275 7064 6174 6522 5d29 202d 3e20   b"update"]) -> 
-00009f30: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
-00009f40: 6c5f 5f5f 5570 6461 7465 456e 7469 7469  l___UpdateEntiti
-00009f50: 6573 4772 6f75 7052 6571 7565 7374 203d  esGroupRequest =
-00009f60: 2055 7064 6174 6545 6e74 6974 6965 7347   UpdateEntitiesG
-00009f70: 726f 7570 5265 7175 6573 740a 0a40 7479  roupRequest..@ty
-00009f80: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
-00009f90: 2055 7064 6174 6545 6e74 6974 6965 7347   UpdateEntitiesG
-00009fa0: 726f 7570 5265 7370 6f6e 7365 2867 6f6f  roupResponse(goo
-00009fb0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-00009fc0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-00009fd0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-00009fe0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-00009ff0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-0000a000: 7074 6f72 0a0a 2020 2020 636c 6173 7320  ptor..    class 
-0000a010: 5f53 7461 7475 733a 0a20 2020 2020 2020  _Status:.       
-0000a020: 2056 616c 7565 5479 7065 203d 2074 7970   ValueType = typ
-0000a030: 696e 672e 4e65 7754 7970 6528 2256 616c  ing.NewType("Val
-0000a040: 7565 5479 7065 222c 2062 7569 6c74 696e  ueType", builtin
-0000a050: 732e 696e 7429 0a20 2020 2020 2020 2056  s.int).        V
-0000a060: 3a20 7479 7069 6e67 5f65 7874 656e 7369  : typing_extensi
-0000a070: 6f6e 732e 5479 7065 416c 6961 7320 3d20  ons.TypeAlias = 
-0000a080: 5661 6c75 6554 7970 650a 0a20 2020 2063  ValueType..    c
-0000a090: 6c61 7373 205f 5374 6174 7573 456e 756d  lass _StatusEnum
-0000a0a0: 5479 7065 5772 6170 7065 7228 676f 6f67  TypeWrapper(goog
-0000a0b0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
-0000a0c0: 726e 616c 2e65 6e75 6d5f 7479 7065 5f77  rnal.enum_type_w
-0000a0d0: 7261 7070 6572 2e5f 456e 756d 5479 7065  rapper._EnumType
-0000a0e0: 5772 6170 7065 725b 5570 6461 7465 456e  Wrapper[UpdateEn
-0000a0f0: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
-0000a100: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
-0000a110: 6554 7970 655d 2c20 6275 696c 7469 6e73  eType], builtins
-0000a120: 2e74 7970 6529 3a0a 2020 2020 2020 2020  .type):.        
-0000a130: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-0000a140: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-0000a150: 7269 7074 6f72 2e45 6e75 6d44 6573 6372  riptor.EnumDescr
-0000a160: 6970 746f 720a 2020 2020 2020 2020 4f4b  iptor.        OK
-0000a170: 3a20 5570 6461 7465 456e 7469 7469 6573  : UpdateEntities
-0000a180: 4772 6f75 7052 6573 706f 6e73 652e 5f53  GroupResponse._S
-0000a190: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-0000a1a0: 2023 2030 0a20 2020 2020 2020 2045 5252   # 0.        ERR
-0000a1b0: 4f52 3a20 5570 6461 7465 456e 7469 7469  OR: UpdateEntiti
-0000a1c0: 6573 4772 6f75 7052 6573 706f 6e73 652e  esGroupResponse.
-0000a1d0: 5f53 7461 7475 732e 5661 6c75 6554 7970  _Status.ValueTyp
-0000a1e0: 6520 2023 2031 0a20 2020 2020 2020 204b  e  # 1.        K
-0000a1f0: 425f 4e4f 545f 464f 554e 443a 2055 7064  B_NOT_FOUND: Upd
-0000a200: 6174 6545 6e74 6974 6965 7347 726f 7570  ateEntitiesGroup
-0000a210: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
-0000a220: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
-0000a230: 2020 2020 2020 2020 454e 5449 5449 4553          ENTITIES
-0000a240: 5f47 524f 5550 5f4e 4f54 5f46 4f55 4e44  _GROUP_NOT_FOUND
-0000a250: 3a20 5570 6461 7465 456e 7469 7469 6573  : UpdateEntities
-0000a260: 4772 6f75 7052 6573 706f 6e73 652e 5f53  GroupResponse._S
-0000a270: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-0000a280: 2023 2033 0a0a 2020 2020 636c 6173 7320   # 3..    class 
-0000a290: 5374 6174 7573 285f 5374 6174 7573 2c20  Status(_Status, 
-0000a2a0: 6d65 7461 636c 6173 733d 5f53 7461 7475  metaclass=_Statu
-0000a2b0: 7345 6e75 6d54 7970 6557 7261 7070 6572  sEnumTypeWrapper
-0000a2c0: 293a 202e 2e2e 0a20 2020 204f 4b3a 2055  ): ....    OK: U
-0000a2d0: 7064 6174 6545 6e74 6974 6965 7347 726f  pdateEntitiesGro
-0000a2e0: 7570 5265 7370 6f6e 7365 2e53 7461 7475  upResponse.Statu
-0000a2f0: 732e 5661 6c75 6554 7970 6520 2023 2030  s.ValueType  # 0
-0000a300: 0a20 2020 2045 5252 4f52 3a20 5570 6461  .    ERROR: Upda
-0000a310: 7465 456e 7469 7469 6573 4772 6f75 7052  teEntitiesGroupR
-0000a320: 6573 706f 6e73 652e 5374 6174 7573 2e56  esponse.Status.V
-0000a330: 616c 7565 5479 7065 2020 2320 310a 2020  alueType  # 1.  
-0000a340: 2020 4b42 5f4e 4f54 5f46 4f55 4e44 3a20    KB_NOT_FOUND: 
-0000a350: 5570 6461 7465 456e 7469 7469 6573 4772  UpdateEntitiesGr
-0000a360: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
-0000a370: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000a380: 320a 2020 2020 454e 5449 5449 4553 5f47  2.    ENTITIES_G
-0000a390: 524f 5550 5f4e 4f54 5f46 4f55 4e44 3a20  ROUP_NOT_FOUND: 
-0000a3a0: 5570 6461 7465 456e 7469 7469 6573 4772  UpdateEntitiesGr
-0000a3b0: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
-0000a3c0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000a3d0: 330a 0a20 2020 2053 5441 5455 535f 4649  3..    STATUS_FI
-0000a3e0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-0000a3f0: 7469 6e73 2e69 6e74 0a20 2020 2073 7461  tins.int.    sta
-0000a400: 7475 733a 2067 6c6f 6261 6c5f 5f5f 5570  tus: global___Up
-0000a410: 6461 7465 456e 7469 7469 6573 4772 6f75  dateEntitiesGrou
-0000a420: 7052 6573 706f 6e73 652e 5374 6174 7573  pResponse.Status
-0000a430: 2e56 616c 7565 5479 7065 0a20 2020 2064  .ValueType.    d
-0000a440: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0000a450: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000a460: 2020 202a 2c0a 2020 2020 2020 2020 7374     *,.        st
-0000a470: 6174 7573 3a20 676c 6f62 616c 5f5f 5f55  atus: global___U
-0000a480: 7064 6174 6545 6e74 6974 6965 7347 726f  pdateEntitiesGro
-0000a490: 7570 5265 7370 6f6e 7365 2e53 7461 7475  upResponse.Statu
-0000a4a0: 732e 5661 6c75 6554 7970 6520 3d20 2e2e  s.ValueType = ..
-0000a4b0: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
-0000a4c0: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
-0000a4d0: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
-0000a4e0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-0000a4f0: 672e 4c69 7465 7261 6c5b 2273 7461 7475  g.Literal["statu
-0000a500: 7322 2c20 6222 7374 6174 7573 225d 2920  s", b"status"]) 
-0000a510: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
-0000a520: 6f62 616c 5f5f 5f55 7064 6174 6545 6e74  obal___UpdateEnt
-0000a530: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
-0000a540: 7365 203d 2055 7064 6174 6545 6e74 6974  se = UpdateEntit
-0000a550: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
-0000a560: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
-0000a570: 636c 6173 7320 4c69 7374 456e 7469 7469  class ListEntiti
-0000a580: 6573 4772 6f75 7073 5265 7175 6573 7428  esGroupsRequest(
-0000a590: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-0000a5a0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
-0000a5b0: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
-0000a5c0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
-0000a5d0: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
-0000a5e0: 6372 6970 746f 720a 0a20 2020 204b 425f  criptor..    KB_
-0000a5f0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-0000a600: 696c 7469 6e73 2e69 6e74 0a20 2020 2040  iltins.int.    @
-0000a610: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000a620: 206b 6228 7365 6c66 2920 2d3e 206e 7563   kb(self) -> nuc
-0000a630: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-0000a640: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
-0000a650: 6f77 6c65 6467 6542 6f78 4944 3a20 2e2e  owledgeBoxID: ..
-0000a660: 2e0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0000a670: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0000a680: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
-0000a690: 2020 2020 206b 623a 206e 7563 6c69 6164       kb: nucliad
-0000a6a0: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-0000a6b0: 6765 626f 785f 7062 322e 4b6e 6f77 6c65  gebox_pb2.Knowle
-0000a6c0: 6467 6542 6f78 4944 207c 204e 6f6e 6520  dgeBoxID | None 
-0000a6d0: 3d20 2e2e 2e2c 0a20 2020 2029 202d 3e20  = ...,.    ) -> 
-0000a6e0: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
-0000a6f0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
-0000a700: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-0000a710: 696e 672e 4c69 7465 7261 6c5b 226b 6222  ing.Literal["kb"
-0000a720: 2c20 6222 6b62 225d 2920 2d3e 2062 7569  , b"kb"]) -> bui
-0000a730: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
-0000a740: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
-0000a750: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
-0000a760: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
-0000a770: 7261 6c5b 226b 6222 2c20 6222 6b62 225d  ral["kb", b"kb"]
-0000a780: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
-0000a790: 676c 6f62 616c 5f5f 5f4c 6973 7445 6e74  global___ListEnt
-0000a7a0: 6974 6965 7347 726f 7570 7352 6571 7565  itiesGroupsReque
-0000a7b0: 7374 203d 204c 6973 7445 6e74 6974 6965  st = ListEntitie
-0000a7c0: 7347 726f 7570 7352 6571 7565 7374 0a0a  sGroupsRequest..
-0000a7d0: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
-0000a7e0: 6173 7320 4c69 7374 456e 7469 7469 6573  ass ListEntities
-0000a7f0: 4772 6f75 7073 5265 7370 6f6e 7365 2867  GroupsResponse(g
-0000a800: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
-0000a810: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
-0000a820: 0a20 2020 2044 4553 4352 4950 544f 523a  .    DESCRIPTOR:
-0000a830: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-0000a840: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-0000a850: 7269 7074 6f72 0a0a 2020 2020 636c 6173  riptor..    clas
-0000a860: 7320 5f53 7461 7475 733a 0a20 2020 2020  s _Status:.     
-0000a870: 2020 2056 616c 7565 5479 7065 203d 2074     ValueType = t
-0000a880: 7970 696e 672e 4e65 7754 7970 6528 2256  yping.NewType("V
-0000a890: 616c 7565 5479 7065 222c 2062 7569 6c74  alueType", built
-0000a8a0: 696e 732e 696e 7429 0a20 2020 2020 2020  ins.int).       
-0000a8b0: 2056 3a20 7479 7069 6e67 5f65 7874 656e   V: typing_exten
-0000a8c0: 7369 6f6e 732e 5479 7065 416c 6961 7320  sions.TypeAlias 
-0000a8d0: 3d20 5661 6c75 6554 7970 650a 0a20 2020  = ValueType..   
-0000a8e0: 2063 6c61 7373 205f 5374 6174 7573 456e   class _StatusEn
-0000a8f0: 756d 5479 7065 5772 6170 7065 7228 676f  umTypeWrapper(go
-0000a900: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
-0000a910: 7465 726e 616c 2e65 6e75 6d5f 7479 7065  ternal.enum_type
-0000a920: 5f77 7261 7070 6572 2e5f 456e 756d 5479  _wrapper._EnumTy
-0000a930: 7065 5772 6170 7065 725b 4c69 7374 456e  peWrapper[ListEn
-0000a940: 7469 7469 6573 4772 6f75 7073 5265 7370  titiesGroupsResp
-0000a950: 6f6e 7365 2e5f 5374 6174 7573 2e56 616c  onse._Status.Val
-0000a960: 7565 5479 7065 5d2c 2062 7569 6c74 696e  ueType], builtin
-0000a970: 732e 7479 7065 293a 0a20 2020 2020 2020  s.type):.       
-0000a980: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-0000a990: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-0000a9a0: 6372 6970 746f 722e 456e 756d 4465 7363  criptor.EnumDesc
-0000a9b0: 7269 7074 6f72 0a20 2020 2020 2020 204f  riptor.        O
-0000a9c0: 4b3a 204c 6973 7445 6e74 6974 6965 7347  K: ListEntitiesG
-0000a9d0: 726f 7570 7352 6573 706f 6e73 652e 5f53  roupsResponse._S
-0000a9e0: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-0000a9f0: 2023 2030 0a20 2020 2020 2020 204e 4f54   # 0.        NOT
-0000aa00: 464f 554e 443a 204c 6973 7445 6e74 6974  FOUND: ListEntit
-0000aa10: 6965 7347 726f 7570 7352 6573 706f 6e73  iesGroupsRespons
-0000aa20: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
-0000aa30: 7970 6520 2023 2031 0a20 2020 2020 2020  ype  # 1.       
-0000aa40: 2045 5252 4f52 3a20 4c69 7374 456e 7469   ERROR: ListEnti
-0000aa50: 7469 6573 4772 6f75 7073 5265 7370 6f6e  tiesGroupsRespon
-0000aa60: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
-0000aa70: 5479 7065 2020 2320 320a 0a20 2020 2063  Type  # 2..    c
-0000aa80: 6c61 7373 2053 7461 7475 7328 5f53 7461  lass Status(_Sta
-0000aa90: 7475 732c 206d 6574 6163 6c61 7373 3d5f  tus, metaclass=_
-0000aaa0: 5374 6174 7573 456e 756d 5479 7065 5772  StatusEnumTypeWr
-0000aab0: 6170 7065 7229 3a20 2e2e 2e0a 2020 2020  apper): ....    
-0000aac0: 4f4b 3a20 4c69 7374 456e 7469 7469 6573  OK: ListEntities
-0000aad0: 4772 6f75 7073 5265 7370 6f6e 7365 2e53  GroupsResponse.S
-0000aae0: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-0000aaf0: 2023 2030 0a20 2020 204e 4f54 464f 554e   # 0.    NOTFOUN
-0000ab00: 443a 204c 6973 7445 6e74 6974 6965 7347  D: ListEntitiesG
-0000ab10: 726f 7570 7352 6573 706f 6e73 652e 5374  roupsResponse.St
-0000ab20: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
-0000ab30: 2320 310a 2020 2020 4552 524f 523a 204c  # 1.    ERROR: L
-0000ab40: 6973 7445 6e74 6974 6965 7347 726f 7570  istEntitiesGroup
-0000ab50: 7352 6573 706f 6e73 652e 5374 6174 7573  sResponse.Status
-0000ab60: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
-0000ab70: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
-0000ab80: 616c 0a20 2020 2063 6c61 7373 2047 726f  al.    class Gro
-0000ab90: 7570 7345 6e74 7279 2867 6f6f 676c 652e  upsEntry(google.
-0000aba0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
-0000abb0: 2e4d 6573 7361 6765 293a 0a20 2020 2020  .Message):.     
-0000abc0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-0000abd0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-0000abe0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-0000abf0: 7074 6f72 0a0a 2020 2020 2020 2020 4b45  ptor..        KE
-0000ac00: 595f 4649 454c 445f 4e55 4d42 4552 3a20  Y_FIELD_NUMBER: 
-0000ac10: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-0000ac20: 2020 2020 2056 414c 5545 5f46 4945 4c44       VALUE_FIELD
-0000ac30: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000ac40: 732e 696e 740a 2020 2020 2020 2020 6b65  s.int.        ke
-0000ac50: 793a 2062 7569 6c74 696e 732e 7374 720a  y: builtins.str.
-0000ac60: 2020 2020 2020 2020 4070 726f 7065 7274          @propert
-0000ac70: 790a 2020 2020 2020 2020 6465 6620 7661  y.        def va
-0000ac80: 6c75 6528 7365 6c66 2920 2d3e 206e 7563  lue(self) -> nuc
-0000ac90: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-0000aca0: 776c 6564 6765 626f 785f 7062 322e 456e  wledgebox_pb2.En
-0000acb0: 7469 7469 6573 4772 6f75 7053 756d 6d61  titiesGroupSumma
-0000acc0: 7279 3a20 2e2e 2e0a 2020 2020 2020 2020  ry: ....        
-0000acd0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0000ace0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
-0000acf0: 2020 2020 2020 2020 2020 2020 2a2c 0a20              *,. 
-0000ad00: 2020 2020 2020 2020 2020 206b 6579 3a20             key: 
-0000ad10: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-0000ad20: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
-0000ad30: 7661 6c75 653a 206e 7563 6c69 6164 625f  value: nucliadb_
-0000ad40: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-0000ad50: 626f 785f 7062 322e 456e 7469 7469 6573  box_pb2.Entities
-0000ad60: 4772 6f75 7053 756d 6d61 7279 207c 204e  GroupSummary | N
-0000ad70: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-0000ad80: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
-0000ad90: 2e0a 2020 2020 2020 2020 6465 6620 4861  ..        def Ha
-0000ada0: 7346 6965 6c64 2873 656c 662c 2066 6965  sField(self, fie
-0000adb0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-0000adc0: 4c69 7465 7261 6c5b 2276 616c 7565 222c  Literal["value",
-0000add0: 2062 2276 616c 7565 225d 2920 2d3e 2062   b"value"]) -> b
-0000ade0: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-0000adf0: 2e0a 2020 2020 2020 2020 6465 6620 436c  ..        def Cl
-0000ae00: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
-0000ae10: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-0000ae20: 672e 4c69 7465 7261 6c5b 226b 6579 222c  g.Literal["key",
-0000ae30: 2062 226b 6579 222c 2022 7661 6c75 6522   b"key", "value"
-0000ae40: 2c20 6222 7661 6c75 6522 5d29 202d 3e20  , b"value"]) -> 
-0000ae50: 4e6f 6e65 3a20 2e2e 2e0a 0a20 2020 2047  None: .....    G
-0000ae60: 524f 5550 535f 4649 454c 445f 4e55 4d42  ROUPS_FIELD_NUMB
-0000ae70: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-0000ae80: 0a20 2020 2053 5441 5455 535f 4649 454c  .    STATUS_FIEL
-0000ae90: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000aea0: 6e73 2e69 6e74 0a20 2020 2073 7461 7475  ns.int.    statu
-0000aeb0: 733a 2067 6c6f 6261 6c5f 5f5f 4c69 7374  s: global___List
-0000aec0: 456e 7469 7469 6573 4772 6f75 7073 5265  EntitiesGroupsRe
-0000aed0: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
-0000aee0: 6c75 6554 7970 650a 2020 2020 4070 726f  lueType.    @pro
-0000aef0: 7065 7274 790a 2020 2020 6465 6620 6772  perty.    def gr
-0000af00: 6f75 7073 2873 656c 6629 202d 3e20 676f  oups(self) -> go
-0000af10: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
-0000af20: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
-0000af30: 732e 4d65 7373 6167 654d 6170 5b62 7569  s.MessageMap[bui
-0000af40: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
-0000af50: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-0000af60: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
-0000af70: 7469 6573 4772 6f75 7053 756d 6d61 7279  tiesGroupSummary
-0000af80: 5d3a 202e 2e2e 0a20 2020 2064 6566 205f  ]: ....    def _
-0000af90: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000afa0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-0000afb0: 2c0a 2020 2020 2020 2020 6772 6f75 7073  ,.        groups
-0000afc0: 3a20 636f 6c6c 6563 7469 6f6e 732e 6162  : collections.ab
-0000afd0: 632e 4d61 7070 696e 675b 6275 696c 7469  c.Mapping[builti
-0000afe0: 6e73 2e73 7472 2c20 6e75 636c 6961 6462  ns.str, nucliadb
-0000aff0: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
-0000b000: 6562 6f78 5f70 6232 2e45 6e74 6974 6965  ebox_pb2.Entitie
-0000b010: 7347 726f 7570 5375 6d6d 6172 795d 207c  sGroupSummary] |
-0000b020: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-0000b030: 2020 2020 2073 7461 7475 733a 2067 6c6f       status: glo
-0000b040: 6261 6c5f 5f5f 4c69 7374 456e 7469 7469  bal___ListEntiti
-0000b050: 6573 4772 6f75 7073 5265 7370 6f6e 7365  esGroupsResponse
-0000b060: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
-0000b070: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
-0000b080: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-0000b090: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-0000b0a0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000b0b0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000b0c0: 2267 726f 7570 7322 2c20 6222 6772 6f75  "groups", b"grou
-0000b0d0: 7073 222c 2022 7374 6174 7573 222c 2062  ps", "status", b
-0000b0e0: 2273 7461 7475 7322 5d29 202d 3e20 4e6f  "status"]) -> No
-0000b0f0: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
-0000b100: 5f5f 4c69 7374 456e 7469 7469 6573 4772  __ListEntitiesGr
-0000b110: 6f75 7073 5265 7370 6f6e 7365 203d 204c  oupsResponse = L
-0000b120: 6973 7445 6e74 6974 6965 7347 726f 7570  istEntitiesGroup
-0000b130: 7352 6573 706f 6e73 650a 0a40 7479 7069  sResponse..@typi
-0000b140: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
-0000b150: 6574 456e 7469 7469 6573 5265 7175 6573  etEntitiesReques
-0000b160: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
-0000b170: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-0000b180: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-0000b190: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000b1a0: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000b1b0: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
-0000b1c0: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
-0000b1d0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-0000b1e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0000b1f0: 6566 206b 6228 7365 6c66 2920 2d3e 206e  ef kb(self) -> n
-0000b200: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-0000b210: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-0000b220: 4b6e 6f77 6c65 6467 6542 6f78 4944 3a20  KnowledgeBoxID: 
-0000b230: 2e2e 2e0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-0000b240: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0000b250: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
-0000b260: 2020 2020 2020 206b 623a 206e 7563 6c69         kb: nucli
-0000b270: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-0000b280: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
-0000b290: 6c65 6467 6542 6f78 4944 207c 204e 6f6e  ledgeBoxID | Non
-0000b2a0: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
-0000b2b0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-0000b2c0: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-0000b2d0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-0000b2e0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-0000b2f0: 6222 2c20 6222 6b62 225d 2920 2d3e 2062  b", b"kb"]) -> b
-0000b300: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-0000b310: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-0000b320: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000b330: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000b340: 7465 7261 6c5b 226b 6222 2c20 6222 6b62  teral["kb", b"kb
-0000b350: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
-0000b360: 0a0a 676c 6f62 616c 5f5f 5f47 6574 456e  ..global___GetEn
-0000b370: 7469 7469 6573 5265 7175 6573 7420 3d20  titiesRequest = 
-0000b380: 4765 7445 6e74 6974 6965 7352 6571 7565  GetEntitiesReque
-0000b390: 7374 0a0a 4074 7970 696e 672e 6669 6e61  st..@typing.fina
-0000b3a0: 6c0a 636c 6173 7320 4765 7445 6e74 6974  l.class GetEntit
-0000b3b0: 6965 7352 6573 706f 6e73 6528 676f 6f67  iesResponse(goog
-0000b3c0: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-0000b3d0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-0000b3e0: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-0000b3f0: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-0000b400: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-0000b410: 746f 720a 0a20 2020 2063 6c61 7373 205f  tor..    class _
-0000b420: 5374 6174 7573 3a0a 2020 2020 2020 2020  Status:.        
-0000b430: 5661 6c75 6554 7970 6520 3d20 7479 7069  ValueType = typi
-0000b440: 6e67 2e4e 6577 5479 7065 2822 5661 6c75  ng.NewType("Valu
-0000b450: 6554 7970 6522 2c20 6275 696c 7469 6e73  eType", builtins
-0000b460: 2e69 6e74 290a 2020 2020 2020 2020 563a  .int).        V:
-0000b470: 2074 7970 696e 675f 6578 7465 6e73 696f   typing_extensio
-0000b480: 6e73 2e54 7970 6541 6c69 6173 203d 2056  ns.TypeAlias = V
-0000b490: 616c 7565 5479 7065 0a0a 2020 2020 636c  alueType..    cl
-0000b4a0: 6173 7320 5f53 7461 7475 7345 6e75 6d54  ass _StatusEnumT
-0000b4b0: 7970 6557 7261 7070 6572 2867 6f6f 676c  ypeWrapper(googl
-0000b4c0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
-0000b4d0: 6e61 6c2e 656e 756d 5f74 7970 655f 7772  nal.enum_type_wr
-0000b4e0: 6170 7065 722e 5f45 6e75 6d54 7970 6557  apper._EnumTypeW
-0000b4f0: 7261 7070 6572 5b47 6574 456e 7469 7469  rapper[GetEntiti
-0000b500: 6573 5265 7370 6f6e 7365 2e5f 5374 6174  esResponse._Stat
-0000b510: 7573 2e56 616c 7565 5479 7065 5d2c 2062  us.ValueType], b
-0000b520: 7569 6c74 696e 732e 7479 7065 293a 0a20  uiltins.type):. 
-0000b530: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
-0000b540: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
-0000b550: 7566 2e64 6573 6372 6970 746f 722e 456e  uf.descriptor.En
-0000b560: 756d 4465 7363 7269 7074 6f72 0a20 2020  umDescriptor.   
-0000b570: 2020 2020 204f 4b3a 2047 6574 456e 7469       OK: GetEnti
-0000b580: 7469 6573 5265 7370 6f6e 7365 2e5f 5374  tiesResponse._St
-0000b590: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
-0000b5a0: 2320 300a 2020 2020 2020 2020 4e4f 5446  # 0.        NOTF
-0000b5b0: 4f55 4e44 3a20 4765 7445 6e74 6974 6965  OUND: GetEntitie
-0000b5c0: 7352 6573 706f 6e73 652e 5f53 7461 7475  sResponse._Statu
-0000b5d0: 732e 5661 6c75 6554 7970 6520 2023 2031  s.ValueType  # 1
-0000b5e0: 0a20 2020 2020 2020 2045 5252 4f52 3a20  .        ERROR: 
-0000b5f0: 4765 7445 6e74 6974 6965 7352 6573 706f  GetEntitiesRespo
-0000b600: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
-0000b610: 6554 7970 6520 2023 2032 0a0a 2020 2020  eType  # 2..    
-0000b620: 636c 6173 7320 5374 6174 7573 285f 5374  class Status(_St
-0000b630: 6174 7573 2c20 6d65 7461 636c 6173 733d  atus, metaclass=
-0000b640: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
-0000b650: 7261 7070 6572 293a 202e 2e2e 0a20 2020  rapper): ....   
-0000b660: 204f 4b3a 2047 6574 456e 7469 7469 6573   OK: GetEntities
-0000b670: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
-0000b680: 5661 6c75 6554 7970 6520 2023 2030 0a20  ValueType  # 0. 
-0000b690: 2020 204e 4f54 464f 554e 443a 2047 6574     NOTFOUND: Get
-0000b6a0: 456e 7469 7469 6573 5265 7370 6f6e 7365  EntitiesResponse
-0000b6b0: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
-0000b6c0: 6520 2023 2031 0a20 2020 2045 5252 4f52  e  # 1.    ERROR
-0000b6d0: 3a20 4765 7445 6e74 6974 6965 7352 6573  : GetEntitiesRes
-0000b6e0: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-0000b6f0: 7565 5479 7065 2020 2320 320a 0a20 2020  ueType  # 2..   
-0000b700: 2040 7479 7069 6e67 2e66 696e 616c 0a20   @typing.final. 
-0000b710: 2020 2063 6c61 7373 2047 726f 7570 7345     class GroupsE
-0000b720: 6e74 7279 2867 6f6f 676c 652e 7072 6f74  ntry(google.prot
-0000b730: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-0000b740: 7361 6765 293a 0a20 2020 2020 2020 2044  sage):.        D
-0000b750: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
-0000b760: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
-0000b770: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
-0000b780: 0a0a 2020 2020 2020 2020 4b45 595f 4649  ..        KEY_FI
-0000b790: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-0000b7a0: 7469 6e73 2e69 6e74 0a20 2020 2020 2020  tins.int.       
-0000b7b0: 2056 414c 5545 5f46 4945 4c44 5f4e 554d   VALUE_FIELD_NUM
-0000b7c0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-0000b7d0: 740a 2020 2020 2020 2020 6b65 793a 2062  t.        key: b
-0000b7e0: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
-0000b7f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000b800: 2020 2020 2020 6465 6620 7661 6c75 6528        def value(
-0000b810: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-0000b820: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-0000b830: 6765 626f 785f 7062 322e 456e 7469 7469  gebox_pb2.Entiti
-0000b840: 6573 4772 6f75 703a 202e 2e2e 0a20 2020  esGroup: ....   
-0000b850: 2020 2020 2064 6566 205f 5f69 6e69 745f       def __init_
-0000b860: 5f28 0a20 2020 2020 2020 2020 2020 2073  _(.            s
-0000b870: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000b880: 202a 2c0a 2020 2020 2020 2020 2020 2020   *,.            
-0000b890: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
-0000b8a0: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
-0000b8b0: 2020 2020 2076 616c 7565 3a20 6e75 636c       value: nucl
-0000b8c0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-0000b8d0: 6c65 6467 6562 6f78 5f70 6232 2e45 6e74  ledgebox_pb2.Ent
-0000b8e0: 6974 6965 7347 726f 7570 207c 204e 6f6e  itiesGroup | Non
-0000b8f0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-0000b900: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
-0000b910: 2020 2020 2020 2020 6465 6620 4861 7346          def HasF
-0000b920: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000b930: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000b940: 7465 7261 6c5b 2276 616c 7565 222c 2062  teral["value", b
-0000b950: 2276 616c 7565 225d 2920 2d3e 2062 7569  "value"]) -> bui
-0000b960: 6c74 696e 732e 626f 6f6c 3a20 2e2e 2e0a  ltins.bool: ....
-0000b970: 2020 2020 2020 2020 6465 6620 436c 6561          def Clea
-0000b980: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-0000b990: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-0000b9a0: 4c69 7465 7261 6c5b 226b 6579 222c 2062  Literal["key", b
-0000b9b0: 226b 6579 222c 2022 7661 6c75 6522 2c20  "key", "value", 
-0000b9c0: 6222 7661 6c75 6522 5d29 202d 3e20 4e6f  b"value"]) -> No
-0000b9d0: 6e65 3a20 2e2e 2e0a 0a20 2020 204b 425f  ne: .....    KB_
-0000b9e0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-0000b9f0: 696c 7469 6e73 2e69 6e74 0a20 2020 2047  iltins.int.    G
-0000ba00: 524f 5550 535f 4649 454c 445f 4e55 4d42  ROUPS_FIELD_NUMB
+00004a30: 696e 740a 2020 2020 534f 5552 4345 5f46  int.    SOURCE_F
+00004a40: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00004a50: 6c74 696e 732e 696e 740a 2020 2020 4143  ltins.int.    AC
+00004a60: 434f 554e 545f 5345 515f 4649 454c 445f  COUNT_SEQ_FIELD_
+00004a70: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00004a80: 2e69 6e74 0a20 2020 2055 5345 525f 5645  .int.    USER_VE
+00004a90: 4354 4f52 535f 4649 454c 445f 4e55 4d42  CTORS_FIELD_NUMB
+00004aa0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00004ab0: 0a20 2020 2052 4549 4e44 4558 5f46 4945  .    REINDEX_FIE
+00004ac0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00004ad0: 696e 732e 696e 740a 2020 2020 4558 5452  ins.int.    EXTR
+00004ae0: 415f 4649 454c 445f 4e55 4d42 4552 3a20  A_FIELD_NUMBER: 
+00004af0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00004b00: 2051 5545 5354 494f 4e5f 414e 5357 4552   QUESTION_ANSWER
+00004b10: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
+00004b20: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00004b30: 2053 4543 5552 4954 595f 4649 454c 445f   SECURITY_FIELD_
+00004b40: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00004b50: 2e69 6e74 0a20 2020 206b 6269 643a 2062  .int.    kbid: b
+00004b60: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
+00004b70: 7575 6964 3a20 6275 696c 7469 6e73 2e73  uuid: builtins.s
+00004b80: 7472 0a20 2020 2073 6c75 673a 2062 7569  tr.    slug: bui
+00004b90: 6c74 696e 732e 7374 720a 2020 2020 7479  ltins.str.    ty
+00004ba0: 7065 3a20 676c 6f62 616c 5f5f 5f42 726f  pe: global___Bro
+00004bb0: 6b65 724d 6573 7361 6765 2e4d 6573 7361  kerMessage.Messa
+00004bc0: 6765 5479 7065 2e56 616c 7565 5479 7065  geType.ValueType
+00004bd0: 0a20 2020 206d 756c 7469 6964 3a20 6275  .    multiid: bu
+00004be0: 696c 7469 6e73 2e73 7472 0a20 2020 206f  iltins.str.    o
+00004bf0: 7269 6769 6e5f 7365 713a 2062 7569 6c74  rigin_seq: built
+00004c00: 696e 732e 696e 740a 2020 2020 736c 6f77  ins.int.    slow
+00004c10: 5f70 726f 6365 7373 696e 675f 7469 6d65  _processing_time
+00004c20: 3a20 6275 696c 7469 6e73 2e66 6c6f 6174  : builtins.float
+00004c30: 0a20 2020 2070 7265 5f70 726f 6365 7373  .    pre_process
+00004c40: 696e 675f 7469 6d65 3a20 6275 696c 7469  ing_time: builti
+00004c50: 6e73 2e66 6c6f 6174 0a20 2020 2074 7873  ns.float.    txs
+00004c60: 6571 6964 3a20 6275 696c 7469 6e73 2e69  eqid: builtins.i
+00004c70: 6e74 0a20 2020 2022 2222 4e6f 7420 6e65  nt.    """Not ne
+00004c80: 6564 6564 2061 6e79 6d6f 7265 2222 220a  eded anymore""".
+00004c90: 2020 2020 7072 6f63 6573 7369 6e67 5f69      processing_i
+00004ca0: 643a 2062 7569 6c74 696e 732e 7374 720a  d: builtins.str.
+00004cb0: 2020 2020 736f 7572 6365 3a20 676c 6f62      source: glob
+00004cc0: 616c 5f5f 5f42 726f 6b65 724d 6573 7361  al___BrokerMessa
+00004cd0: 6765 2e4d 6573 7361 6765 536f 7572 6365  ge.MessageSource
+00004ce0: 2e56 616c 7565 5479 7065 0a20 2020 2061  .ValueType.    a
+00004cf0: 6363 6f75 6e74 5f73 6571 3a20 6275 696c  ccount_seq: buil
+00004d00: 7469 6e73 2e69 6e74 0a20 2020 2072 6569  tins.int.    rei
+00004d10: 6e64 6578 3a20 6275 696c 7469 6e73 2e62  ndex: builtins.b
+00004d20: 6f6f 6c0a 2020 2020 2222 2249 6620 7472  ool.    """If tr
+00004d30: 7565 2c20 666f 7263 6520 7265 696e 6465  ue, force reinde
+00004d40: 7820 616c 6c20 7061 7261 6772 6170 6873  x all paragraphs
+00004d50: 2069 6e20 6120 7265 736f 7572 6365 2222   in a resource""
+00004d60: 220a 2020 2020 4070 726f 7065 7274 790a  ".    @property.
+00004d70: 2020 2020 6465 6620 6175 6469 7428 7365      def audit(se
+00004d80: 6c66 2920 2d3e 2067 6c6f 6261 6c5f 5f5f  lf) -> global___
+00004d90: 4175 6469 743a 202e 2e2e 0a20 2020 2040  Audit: ....    @
+00004da0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00004db0: 2062 6173 6963 2873 656c 6629 202d 3e20   basic(self) -> 
+00004dc0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00004dd0: 7265 736f 7572 6365 735f 7062 322e 4261  resources_pb2.Ba
+00004de0: 7369 633a 202e 2e2e 0a20 2020 2040 7072  sic: ....    @pr
+00004df0: 6f70 6572 7479 0a20 2020 2064 6566 206f  operty.    def o
+00004e00: 7269 6769 6e28 7365 6c66 2920 2d3e 206e  rigin(self) -> n
+00004e10: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00004e20: 6573 6f75 7263 6573 5f70 6232 2e4f 7269  esources_pb2.Ori
+00004e30: 6769 6e3a 202e 2e2e 0a20 2020 2040 7072  gin: ....    @pr
+00004e40: 6f70 6572 7479 0a20 2020 2064 6566 2072  operty.    def r
+00004e50: 656c 6174 696f 6e73 2873 656c 6629 202d  elations(self) -
+00004e60: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
+00004e70: 662e 696e 7465 726e 616c 2e63 6f6e 7461  f.internal.conta
+00004e80: 696e 6572 732e 5265 7065 6174 6564 436f  iners.RepeatedCo
+00004e90: 6d70 6f73 6974 6546 6965 6c64 436f 6e74  mpositeFieldCont
+00004ea0: 6169 6e65 725b 6e75 636c 6961 6462 5f70  ainer[nucliadb_p
+00004eb0: 726f 746f 732e 7574 696c 735f 7062 322e  rotos.utils_pb2.
+00004ec0: 5265 6c61 7469 6f6e 5d3a 202e 2e2e 0a20  Relation]: .... 
+00004ed0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00004ee0: 2064 6566 2063 6f6e 7665 7273 6174 696f   def conversatio
+00004ef0: 6e73 2873 656c 6629 202d 3e20 676f 6f67  ns(self) -> goog
+00004f00: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+00004f10: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+00004f20: 4d65 7373 6167 654d 6170 5b62 7569 6c74  MessageMap[built
+00004f30: 696e 732e 7374 722c 206e 7563 6c69 6164  ins.str, nucliad
+00004f40: 625f 7072 6f74 6f73 2e72 6573 6f75 7263  b_protos.resourc
+00004f50: 6573 5f70 6232 2e43 6f6e 7665 7273 6174  es_pb2.Conversat
+00004f60: 696f 6e5d 3a0a 2020 2020 2020 2020 2222  ion]:.        ""
+00004f70: 2246 6965 6c64 2043 6f6e 7665 7273 6174  "Field Conversat
+00004f80: 696f 6e73 2222 220a 0a20 2020 2040 7072  ions"""..    @pr
+00004f90: 6f70 6572 7479 0a20 2020 2064 6566 206c  operty.    def l
+00004fa0: 6179 6f75 7473 2873 656c 6629 202d 3e20  ayouts(self) -> 
+00004fb0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00004fc0: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
+00004fd0: 6572 732e 4d65 7373 6167 654d 6170 5b62  ers.MessageMap[b
+00004fe0: 7569 6c74 696e 732e 7374 722c 206e 7563  uiltins.str, nuc
+00004ff0: 6c69 6164 625f 7072 6f74 6f73 2e72 6573  liadb_protos.res
+00005000: 6f75 7263 6573 5f70 6232 2e46 6965 6c64  ources_pb2.Field
+00005010: 4c61 796f 7574 5d3a 0a20 2020 2020 2020  Layout]:.       
+00005020: 2022 2222 4669 656c 6420 4c61 796f 7574   """Field Layout
+00005030: 2222 220a 0a20 2020 2040 7072 6f70 6572  """..    @proper
+00005040: 7479 0a20 2020 2064 6566 2074 6578 7473  ty.    def texts
+00005050: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
+00005060: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
+00005070: 616c 2e63 6f6e 7461 696e 6572 732e 4d65  al.containers.Me
+00005080: 7373 6167 654d 6170 5b62 7569 6c74 696e  ssageMap[builtin
+00005090: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
+000050a0: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
+000050b0: 5f70 6232 2e46 6965 6c64 5465 7874 5d3a  _pb2.FieldText]:
+000050c0: 0a20 2020 2020 2020 2022 2222 4669 656c  .        """Fiel
+000050d0: 6420 5465 7874 2222 220a 0a20 2020 2040  d Text"""..    @
+000050e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000050f0: 206b 6579 776f 7264 7365 7473 2873 656c   keywordsets(sel
+00005100: 6629 202d 3e20 676f 6f67 6c65 2e70 726f  f) -> google.pro
+00005110: 746f 6275 662e 696e 7465 726e 616c 2e63  tobuf.internal.c
+00005120: 6f6e 7461 696e 6572 732e 4d65 7373 6167  ontainers.Messag
+00005130: 654d 6170 5b62 7569 6c74 696e 732e 7374  eMap[builtins.st
+00005140: 722c 206e 7563 6c69 6164 625f 7072 6f74  r, nucliadb_prot
+00005150: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
+00005160: 2e46 6965 6c64 4b65 7977 6f72 6473 6574  .FieldKeywordset
+00005170: 5d3a 0a20 2020 2020 2020 2022 2222 4669  ]:.        """Fi
+00005180: 656c 6420 6b65 7977 6f72 6422 2222 0a0a  eld keyword"""..
+00005190: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+000051a0: 2020 6465 6620 6461 7465 7469 6d65 7328    def datetimes(
+000051b0: 7365 6c66 2920 2d3e 2067 6f6f 676c 652e  self) -> google.
+000051c0: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
+000051d0: 6c2e 636f 6e74 6169 6e65 7273 2e4d 6573  l.containers.Mes
+000051e0: 7361 6765 4d61 705b 6275 696c 7469 6e73  sageMap[builtins
+000051f0: 2e73 7472 2c20 6e75 636c 6961 6462 5f70  .str, nucliadb_p
+00005200: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
+00005210: 7062 322e 4669 656c 6444 6174 6574 696d  pb2.FieldDatetim
+00005220: 655d 3a0a 2020 2020 2020 2020 2222 2246  e]:.        """F
+00005230: 6965 6c64 2044 6174 6574 696d 6522 2222  ield Datetime"""
+00005240: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00005250: 2020 2020 6465 6620 6c69 6e6b 7328 7365      def links(se
+00005260: 6c66 2920 2d3e 2067 6f6f 676c 652e 7072  lf) -> google.pr
+00005270: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
+00005280: 636f 6e74 6169 6e65 7273 2e4d 6573 7361  containers.Messa
+00005290: 6765 4d61 705b 6275 696c 7469 6e73 2e73  geMap[builtins.s
+000052a0: 7472 2c20 6e75 636c 6961 6462 5f70 726f  tr, nucliadb_pro
+000052b0: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
+000052c0: 322e 4669 656c 644c 696e 6b5d 3a0a 2020  2.FieldLink]:.  
+000052d0: 2020 2020 2020 2222 2246 6965 6c64 204c        """Field L
+000052e0: 696e 6b73 2222 220a 0a20 2020 2040 7072  inks"""..    @pr
+000052f0: 6f70 6572 7479 0a20 2020 2064 6566 2066  operty.    def f
+00005300: 696c 6573 2873 656c 6629 202d 3e20 676f  iles(self) -> go
+00005310: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+00005320: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
+00005330: 732e 4d65 7373 6167 654d 6170 5b62 7569  s.MessageMap[bui
+00005340: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
+00005350: 6164 625f 7072 6f74 6f73 2e72 6573 6f75  adb_protos.resou
+00005360: 7263 6573 5f70 6232 2e46 6965 6c64 4669  rces_pb2.FieldFi
+00005370: 6c65 5d3a 0a20 2020 2020 2020 2022 2222  le]:.        """
+00005380: 4669 656c 6420 4669 6c65 2222 220a 0a20  Field File""".. 
+00005390: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000053a0: 2064 6566 206c 696e 6b5f 6578 7472 6163   def link_extrac
+000053b0: 7465 645f 6461 7461 2873 656c 6629 202d  ted_data(self) -
+000053c0: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
+000053d0: 662e 696e 7465 726e 616c 2e63 6f6e 7461  f.internal.conta
+000053e0: 696e 6572 732e 5265 7065 6174 6564 436f  iners.RepeatedCo
+000053f0: 6d70 6f73 6974 6546 6965 6c64 436f 6e74  mpositeFieldCont
+00005400: 6169 6e65 725b 6e75 636c 6961 6462 5f70  ainer[nucliadb_p
+00005410: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
+00005420: 7062 322e 4c69 6e6b 4578 7472 6163 7465  pb2.LinkExtracte
+00005430: 6444 6174 615d 3a0a 2020 2020 2020 2020  dData]:.        
+00005440: 2222 224c 696e 6b20 6578 7472 6163 7465  """Link extracte
+00005450: 6420 6578 7472 6120 696e 666f 2222 220a  d extra info""".
+00005460: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00005470: 2020 2064 6566 2066 696c 655f 6578 7472     def file_extr
+00005480: 6163 7465 645f 6461 7461 2873 656c 6629  acted_data(self)
+00005490: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
+000054a0: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
+000054b0: 7461 696e 6572 732e 5265 7065 6174 6564  tainers.Repeated
+000054c0: 436f 6d70 6f73 6974 6546 6965 6c64 436f  CompositeFieldCo
+000054d0: 6e74 6169 6e65 725b 6e75 636c 6961 6462  ntainer[nucliadb
+000054e0: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+000054f0: 735f 7062 322e 4669 6c65 4578 7472 6163  s_pb2.FileExtrac
+00005500: 7465 6444 6174 615d 3a0a 2020 2020 2020  tedData]:.      
+00005510: 2020 2222 2246 696c 6520 6578 7472 6163    """File extrac
+00005520: 7465 6420 6578 7472 6120 696e 666f 2222  ted extra info""
+00005530: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
+00005540: 0a20 2020 2064 6566 2065 7874 7261 6374  .    def extract
+00005550: 6564 5f74 6578 7428 7365 6c66 2920 2d3e  ed_text(self) ->
+00005560: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00005570: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
+00005580: 6e65 7273 2e52 6570 6561 7465 6443 6f6d  ners.RepeatedCom
+00005590: 706f 7369 7465 4669 656c 6443 6f6e 7461  positeFieldConta
+000055a0: 696e 6572 5b6e 7563 6c69 6164 625f 7072  iner[nucliadb_pr
+000055b0: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+000055c0: 6232 2e45 7874 7261 6374 6564 5465 7874  b2.ExtractedText
+000055d0: 5772 6170 7065 725d 3a0a 2020 2020 2020  Wrapper]:.      
+000055e0: 2020 2222 2246 6965 6c64 2045 7874 7261    """Field Extra
+000055f0: 6374 6564 2f43 6f6d 7075 7465 6420 696e  cted/Computed in
+00005600: 666f 726d 6174 696f 6e22 2222 0a0a 2020  formation"""..  
+00005610: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00005620: 6465 6620 6669 656c 645f 6d65 7461 6461  def field_metada
+00005630: 7461 2873 656c 6629 202d 3e20 676f 6f67  ta(self) -> goog
+00005640: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+00005650: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+00005660: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
+00005670: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
+00005680: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00005690: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
+000056a0: 656c 6443 6f6d 7075 7465 644d 6574 6164  eldComputedMetad
+000056b0: 6174 6157 7261 7070 6572 5d3a 202e 2e2e  ataWrapper]: ...
+000056c0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000056d0: 2020 2064 6566 2066 6965 6c64 5f76 6563     def field_vec
+000056e0: 746f 7273 2873 656c 6629 202d 3e20 676f  tors(self) -> go
+000056f0: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+00005700: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
+00005710: 732e 5265 7065 6174 6564 436f 6d70 6f73  s.RepeatedCompos
+00005720: 6974 6546 6965 6c64 436f 6e74 6169 6e65  iteFieldContaine
+00005730: 725b 6e75 636c 6961 6462 5f70 726f 746f  r[nucliadb_proto
+00005740: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+00005750: 4578 7472 6163 7465 6456 6563 746f 7273  ExtractedVectors
+00005760: 5772 6170 7065 725d 3a20 2e2e 2e0a 2020  Wrapper]: ....  
+00005770: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00005780: 6465 6620 6669 656c 645f 6c61 7267 655f  def field_large_
+00005790: 6d65 7461 6461 7461 2873 656c 6629 202d  metadata(self) -
+000057a0: 3e20 676f 6f67 6c65 2e70 726f 746f 6275  > google.protobu
+000057b0: 662e 696e 7465 726e 616c 2e63 6f6e 7461  f.internal.conta
+000057c0: 696e 6572 732e 5265 7065 6174 6564 436f  iners.RepeatedCo
+000057d0: 6d70 6f73 6974 6546 6965 6c64 436f 6e74  mpositeFieldCont
+000057e0: 6169 6e65 725b 6e75 636c 6961 6462 5f70  ainer[nucliadb_p
+000057f0: 726f 746f 732e 7265 736f 7572 6365 735f  rotos.resources_
+00005800: 7062 322e 4c61 7267 6543 6f6d 7075 7465  pb2.LargeCompute
+00005810: 644d 6574 6164 6174 6157 7261 7070 6572  dMetadataWrapper
+00005820: 5d3a 0a20 2020 2020 2020 2022 2222 5265  ]:.        """Re
+00005830: 736f 7572 6365 204c 6172 6765 2043 6f6d  source Large Com
+00005840: 7075 7465 6420 4d65 7461 6461 7461 2222  puted Metadata""
+00005850: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
+00005860: 0a20 2020 2064 6566 2064 656c 6574 655f  .    def delete_
+00005870: 6669 656c 6473 2873 656c 6629 202d 3e20  fields(self) -> 
+00005880: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00005890: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
+000058a0: 6572 732e 5265 7065 6174 6564 436f 6d70  ers.RepeatedComp
+000058b0: 6f73 6974 6546 6965 6c64 436f 6e74 6169  ositeFieldContai
+000058c0: 6e65 725b 6e75 636c 6961 6462 5f70 726f  ner[nucliadb_pro
+000058d0: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
+000058e0: 322e 4669 656c 6449 445d 3a20 2e2e 2e0a  2.FieldID]: ....
+000058f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00005900: 2020 6465 6620 646f 6e65 5f74 696d 6528    def done_time(
+00005910: 7365 6c66 2920 2d3e 2067 6f6f 676c 652e  self) -> google.
+00005920: 7072 6f74 6f62 7566 2e74 696d 6573 7461  protobuf.timesta
+00005930: 6d70 5f70 6232 2e54 696d 6573 7461 6d70  mp_pb2.Timestamp
+00005940: 3a20 2e2e 2e0a 2020 2020 4070 726f 7065  : ....    @prope
+00005950: 7274 790a 2020 2020 6465 6620 6572 726f  rty.    def erro
+00005960: 7273 2873 656c 6629 202d 3e20 676f 6f67  rs(self) -> goog
+00005970: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+00005980: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+00005990: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
+000059a0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
+000059b0: 676c 6f62 616c 5f5f 5f45 7272 6f72 5d3a  global___Error]:
+000059c0: 202e 2e2e 0a20 2020 2040 7072 6f70 6572   ....    @proper
+000059d0: 7479 0a20 2020 2064 6566 2075 7365 725f  ty.    def user_
+000059e0: 7665 6374 6f72 7328 7365 6c66 2920 2d3e  vectors(self) ->
+000059f0: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00005a00: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
+00005a10: 6e65 7273 2e52 6570 6561 7465 6443 6f6d  ners.RepeatedCom
+00005a20: 706f 7369 7465 4669 656c 6443 6f6e 7461  positeFieldConta
+00005a30: 696e 6572 5b6e 7563 6c69 6164 625f 7072  iner[nucliadb_pr
+00005a40: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+00005a50: 6232 2e55 7365 7256 6563 746f 7273 5772  b2.UserVectorsWr
+00005a60: 6170 7065 725d 3a20 2e2e 2e0a 2020 2020  apper]: ....    
+00005a70: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00005a80: 6620 6578 7472 6128 7365 6c66 2920 2d3e  f extra(self) ->
+00005a90: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00005aa0: 2e72 6573 6f75 7263 6573 5f70 6232 2e45  .resources_pb2.E
+00005ab0: 7874 7261 3a20 2e2e 2e0a 2020 2020 4070  xtra: ....    @p
+00005ac0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00005ad0: 7175 6573 7469 6f6e 5f61 6e73 7765 7273  question_answers
+00005ae0: 2873 656c 6629 202d 3e20 676f 6f67 6c65  (self) -> google
+00005af0: 2e70 726f 746f 6275 662e 696e 7465 726e  .protobuf.intern
+00005b00: 616c 2e63 6f6e 7461 696e 6572 732e 5265  al.containers.Re
+00005b10: 7065 6174 6564 436f 6d70 6f73 6974 6546  peatedCompositeF
+00005b20: 6965 6c64 436f 6e74 6169 6e65 725b 6e75  ieldContainer[nu
+00005b30: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+00005b40: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
+00005b50: 6451 7565 7374 696f 6e41 6e73 7765 7257  dQuestionAnswerW
+00005b60: 7261 7070 6572 5d3a 202e 2e2e 0a20 2020  rapper]: ....   
+00005b70: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00005b80: 6566 2073 6563 7572 6974 7928 7365 6c66  ef security(self
+00005b90: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
+00005ba0: 6f74 6f73 2e75 7469 6c73 5f70 6232 2e53  otos.utils_pb2.S
+00005bb0: 6563 7572 6974 793a 202e 2e2e 0a20 2020  ecurity: ....   
+00005bc0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00005bd0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00005be0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00005bf0: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
+00005c00: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
+00005c10: 2020 7575 6964 3a20 6275 696c 7469 6e73    uuid: builtins
+00005c20: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+00005c30: 2020 2020 736c 7567 3a20 6275 696c 7469      slug: builti
+00005c40: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+00005c50: 2020 2020 2020 6175 6469 743a 2067 6c6f        audit: glo
+00005c60: 6261 6c5f 5f5f 4175 6469 7420 7c20 4e6f  bal___Audit | No
+00005c70: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+00005c80: 2020 7479 7065 3a20 676c 6f62 616c 5f5f    type: global__
+00005c90: 5f42 726f 6b65 724d 6573 7361 6765 2e4d  _BrokerMessage.M
+00005ca0: 6573 7361 6765 5479 7065 2e56 616c 7565  essageType.Value
+00005cb0: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
+00005cc0: 2020 2020 6d75 6c74 6969 643a 2062 7569      multiid: bui
+00005cd0: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
+00005ce0: 0a20 2020 2020 2020 2062 6173 6963 3a20  .        basic: 
+00005cf0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00005d00: 7265 736f 7572 6365 735f 7062 322e 4261  resources_pb2.Ba
+00005d10: 7369 6320 7c20 4e6f 6e65 203d 202e 2e2e  sic | None = ...
+00005d20: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
+00005d30: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+00005d40: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+00005d50: 4f72 6967 696e 207c 204e 6f6e 6520 3d20  Origin | None = 
+00005d60: 2e2e 2e2c 0a20 2020 2020 2020 2072 656c  ...,.        rel
+00005d70: 6174 696f 6e73 3a20 636f 6c6c 6563 7469  ations: collecti
+00005d80: 6f6e 732e 6162 632e 4974 6572 6162 6c65  ons.abc.Iterable
+00005d90: 5b6e 7563 6c69 6164 625f 7072 6f74 6f73  [nucliadb_protos
+00005da0: 2e75 7469 6c73 5f70 6232 2e52 656c 6174  .utils_pb2.Relat
+00005db0: 696f 6e5d 207c 204e 6f6e 6520 3d20 2e2e  ion] | None = ..
+00005dc0: 2e2c 0a20 2020 2020 2020 2063 6f6e 7665  .,.        conve
+00005dd0: 7273 6174 696f 6e73 3a20 636f 6c6c 6563  rsations: collec
+00005de0: 7469 6f6e 732e 6162 632e 4d61 7070 696e  tions.abc.Mappin
+00005df0: 675b 6275 696c 7469 6e73 2e73 7472 2c20  g[builtins.str, 
+00005e00: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00005e10: 7265 736f 7572 6365 735f 7062 322e 436f  resources_pb2.Co
+00005e20: 6e76 6572 7361 7469 6f6e 5d20 7c20 4e6f  nversation] | No
+00005e30: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+00005e40: 2020 6c61 796f 7574 733a 2063 6f6c 6c65    layouts: colle
+00005e50: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
+00005e60: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
+00005e70: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00005e80: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00005e90: 6965 6c64 4c61 796f 7574 5d20 7c20 4e6f  ieldLayout] | No
+00005ea0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+00005eb0: 2020 7465 7874 733a 2063 6f6c 6c65 6374    texts: collect
+00005ec0: 696f 6e73 2e61 6263 2e4d 6170 7069 6e67  ions.abc.Mapping
+00005ed0: 5b62 7569 6c74 696e 732e 7374 722c 206e  [builtins.str, n
+00005ee0: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00005ef0: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
+00005f00: 6c64 5465 7874 5d20 7c20 4e6f 6e65 203d  ldText] | None =
+00005f10: 202e 2e2e 2c0a 2020 2020 2020 2020 6b65   ...,.        ke
+00005f20: 7977 6f72 6473 6574 733a 2063 6f6c 6c65  ywordsets: colle
+00005f30: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
+00005f40: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
+00005f50: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00005f60: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00005f70: 6965 6c64 4b65 7977 6f72 6473 6574 5d20  ieldKeywordset] 
+00005f80: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
+00005f90: 2020 2020 2020 6461 7465 7469 6d65 733a        datetimes:
+00005fa0: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+00005fb0: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
+00005fc0: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
+00005fd0: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
+00005fe0: 5f70 6232 2e46 6965 6c64 4461 7465 7469  _pb2.FieldDateti
+00005ff0: 6d65 5d20 7c20 4e6f 6e65 203d 202e 2e2e  me] | None = ...
+00006000: 2c0a 2020 2020 2020 2020 6c69 6e6b 733a  ,.        links:
+00006010: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+00006020: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
+00006030: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
+00006040: 7072 6f74 6f73 2e72 6573 6f75 7263 6573  protos.resources
+00006050: 5f70 6232 2e46 6965 6c64 4c69 6e6b 5d20  _pb2.FieldLink] 
+00006060: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
+00006070: 2020 2020 2020 6669 6c65 733a 2063 6f6c        files: col
+00006080: 6c65 6374 696f 6e73 2e61 6263 2e4d 6170  lections.abc.Map
+00006090: 7069 6e67 5b62 7569 6c74 696e 732e 7374  ping[builtins.st
+000060a0: 722c 206e 7563 6c69 6164 625f 7072 6f74  r, nucliadb_prot
+000060b0: 6f73 2e72 6573 6f75 7263 6573 5f70 6232  os.resources_pb2
+000060c0: 2e46 6965 6c64 4669 6c65 5d20 7c20 4e6f  .FieldFile] | No
+000060d0: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+000060e0: 2020 6c69 6e6b 5f65 7874 7261 6374 6564    link_extracted
+000060f0: 5f64 6174 613a 2063 6f6c 6c65 6374 696f  _data: collectio
+00006100: 6e73 2e61 6263 2e49 7465 7261 626c 655b  ns.abc.Iterable[
+00006110: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00006120: 7265 736f 7572 6365 735f 7062 322e 4c69  resources_pb2.Li
+00006130: 6e6b 4578 7472 6163 7465 6444 6174 615d  nkExtractedData]
+00006140: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00006150: 2020 2020 2020 2066 696c 655f 6578 7472         file_extr
+00006160: 6163 7465 645f 6461 7461 3a20 636f 6c6c  acted_data: coll
+00006170: 6563 7469 6f6e 732e 6162 632e 4974 6572  ections.abc.Iter
+00006180: 6162 6c65 5b6e 7563 6c69 6164 625f 7072  able[nucliadb_pr
+00006190: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+000061a0: 6232 2e46 696c 6545 7874 7261 6374 6564  b2.FileExtracted
+000061b0: 4461 7461 5d20 7c20 4e6f 6e65 203d 202e  Data] | None = .
+000061c0: 2e2e 2c0a 2020 2020 2020 2020 6578 7472  ..,.        extr
+000061d0: 6163 7465 645f 7465 7874 3a20 636f 6c6c  acted_text: coll
+000061e0: 6563 7469 6f6e 732e 6162 632e 4974 6572  ections.abc.Iter
+000061f0: 6162 6c65 5b6e 7563 6c69 6164 625f 7072  able[nucliadb_pr
+00006200: 6f74 6f73 2e72 6573 6f75 7263 6573 5f70  otos.resources_p
+00006210: 6232 2e45 7874 7261 6374 6564 5465 7874  b2.ExtractedText
+00006220: 5772 6170 7065 725d 207c 204e 6f6e 6520  Wrapper] | None 
+00006230: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2066  = ...,.        f
+00006240: 6965 6c64 5f6d 6574 6164 6174 613a 2063  ield_metadata: c
+00006250: 6f6c 6c65 6374 696f 6e73 2e61 6263 2e49  ollections.abc.I
+00006260: 7465 7261 626c 655b 6e75 636c 6961 6462  terable[nucliadb
+00006270: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+00006280: 735f 7062 322e 4669 656c 6443 6f6d 7075  s_pb2.FieldCompu
+00006290: 7465 644d 6574 6164 6174 6157 7261 7070  tedMetadataWrapp
+000062a0: 6572 5d20 7c20 4e6f 6e65 203d 202e 2e2e  er] | None = ...
+000062b0: 2c0a 2020 2020 2020 2020 6669 656c 645f  ,.        field_
+000062c0: 7665 6374 6f72 733a 2063 6f6c 6c65 6374  vectors: collect
+000062d0: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
+000062e0: 655b 6e75 636c 6961 6462 5f70 726f 746f  e[nucliadb_proto
+000062f0: 732e 7265 736f 7572 6365 735f 7062 322e  s.resources_pb2.
+00006300: 4578 7472 6163 7465 6456 6563 746f 7273  ExtractedVectors
+00006310: 5772 6170 7065 725d 207c 204e 6f6e 6520  Wrapper] | None 
+00006320: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2066  = ...,.        f
+00006330: 6965 6c64 5f6c 6172 6765 5f6d 6574 6164  ield_large_metad
+00006340: 6174 613a 2063 6f6c 6c65 6374 696f 6e73  ata: collections
+00006350: 2e61 6263 2e49 7465 7261 626c 655b 6e75  .abc.Iterable[nu
+00006360: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
+00006370: 736f 7572 6365 735f 7062 322e 4c61 7267  sources_pb2.Larg
+00006380: 6543 6f6d 7075 7465 644d 6574 6164 6174  eComputedMetadat
+00006390: 6157 7261 7070 6572 5d20 7c20 4e6f 6e65  aWrapper] | None
+000063a0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+000063b0: 6465 6c65 7465 5f66 6965 6c64 733a 2063  delete_fields: c
+000063c0: 6f6c 6c65 6374 696f 6e73 2e61 6263 2e49  ollections.abc.I
+000063d0: 7465 7261 626c 655b 6e75 636c 6961 6462  terable[nucliadb
+000063e0: 5f70 726f 746f 732e 7265 736f 7572 6365  _protos.resource
+000063f0: 735f 7062 322e 4669 656c 6449 445d 207c  s_pb2.FieldID] |
+00006400: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
+00006410: 2020 2020 206f 7269 6769 6e5f 7365 713a       origin_seq:
+00006420: 2062 7569 6c74 696e 732e 696e 7420 3d20   builtins.int = 
+00006430: 2e2e 2e2c 0a20 2020 2020 2020 2073 6c6f  ...,.        slo
+00006440: 775f 7072 6f63 6573 7369 6e67 5f74 696d  w_processing_tim
+00006450: 653a 2062 7569 6c74 696e 732e 666c 6f61  e: builtins.floa
+00006460: 7420 3d20 2e2e 2e2c 0a20 2020 2020 2020  t = ...,.       
+00006470: 2070 7265 5f70 726f 6365 7373 696e 675f   pre_processing_
+00006480: 7469 6d65 3a20 6275 696c 7469 6e73 2e66  time: builtins.f
+00006490: 6c6f 6174 203d 202e 2e2e 2c0a 2020 2020  loat = ...,.    
+000064a0: 2020 2020 646f 6e65 5f74 696d 653a 2067      done_time: g
+000064b0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e74  oogle.protobuf.t
+000064c0: 696d 6573 7461 6d70 5f70 6232 2e54 696d  imestamp_pb2.Tim
+000064d0: 6573 7461 6d70 207c 204e 6f6e 6520 3d20  estamp | None = 
+000064e0: 2e2e 2e2c 0a20 2020 2020 2020 2074 7873  ...,.        txs
+000064f0: 6571 6964 3a20 6275 696c 7469 6e73 2e69  eqid: builtins.i
+00006500: 6e74 203d 202e 2e2e 2c0a 2020 2020 2020  nt = ...,.      
+00006510: 2020 6572 726f 7273 3a20 636f 6c6c 6563    errors: collec
+00006520: 7469 6f6e 732e 6162 632e 4974 6572 6162  tions.abc.Iterab
+00006530: 6c65 5b67 6c6f 6261 6c5f 5f5f 4572 726f  le[global___Erro
+00006540: 725d 207c 204e 6f6e 6520 3d20 2e2e 2e2c  r] | None = ...,
+00006550: 0a20 2020 2020 2020 2070 726f 6365 7373  .        process
+00006560: 696e 675f 6964 3a20 6275 696c 7469 6e73  ing_id: builtins
+00006570: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+00006580: 2020 2020 736f 7572 6365 3a20 676c 6f62      source: glob
+00006590: 616c 5f5f 5f42 726f 6b65 724d 6573 7361  al___BrokerMessa
+000065a0: 6765 2e4d 6573 7361 6765 536f 7572 6365  ge.MessageSource
+000065b0: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
+000065c0: 2c0a 2020 2020 2020 2020 6163 636f 756e  ,.        accoun
+000065d0: 745f 7365 713a 2062 7569 6c74 696e 732e  t_seq: builtins.
+000065e0: 696e 7420 3d20 2e2e 2e2c 0a20 2020 2020  int = ...,.     
+000065f0: 2020 2075 7365 725f 7665 6374 6f72 733a     user_vectors:
+00006600: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+00006610: 2e49 7465 7261 626c 655b 6e75 636c 6961  .Iterable[nuclia
+00006620: 6462 5f70 726f 746f 732e 7265 736f 7572  db_protos.resour
+00006630: 6365 735f 7062 322e 5573 6572 5665 6374  ces_pb2.UserVect
+00006640: 6f72 7357 7261 7070 6572 5d20 7c20 4e6f  orsWrapper] | No
+00006650: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+00006660: 2020 7265 696e 6465 783a 2062 7569 6c74    reindex: built
+00006670: 696e 732e 626f 6f6c 203d 202e 2e2e 2c0a  ins.bool = ...,.
+00006680: 2020 2020 2020 2020 6578 7472 613a 206e          extra: n
+00006690: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+000066a0: 6573 6f75 7263 6573 5f70 6232 2e45 7874  esources_pb2.Ext
+000066b0: 7261 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ra | None = ...,
+000066c0: 0a20 2020 2020 2020 2071 7565 7374 696f  .        questio
+000066d0: 6e5f 616e 7377 6572 733a 2063 6f6c 6c65  n_answers: colle
+000066e0: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
+000066f0: 626c 655b 6e75 636c 6961 6462 5f70 726f  ble[nucliadb_pro
+00006700: 746f 732e 7265 736f 7572 6365 735f 7062  tos.resources_pb
+00006710: 322e 4669 656c 6451 7565 7374 696f 6e41  2.FieldQuestionA
+00006720: 6e73 7765 7257 7261 7070 6572 5d20 7c20  nswerWrapper] | 
+00006730: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+00006740: 2020 2020 7365 6375 7269 7479 3a20 6e75      security: nu
+00006750: 636c 6961 6462 5f70 726f 746f 732e 7574  cliadb_protos.ut
+00006760: 696c 735f 7062 322e 5365 6375 7269 7479  ils_pb2.Security
+00006770: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00006780: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+00006790: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
+000067a0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+000067b0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+000067c0: 7261 6c5b 2261 7564 6974 222c 2062 2261  ral["audit", b"a
+000067d0: 7564 6974 222c 2022 6261 7369 6322 2c20  udit", "basic", 
+000067e0: 6222 6261 7369 6322 2c20 2264 6f6e 655f  b"basic", "done_
+000067f0: 7469 6d65 222c 2062 2264 6f6e 655f 7469  time", b"done_ti
+00006800: 6d65 222c 2022 6578 7472 6122 2c20 6222  me", "extra", b"
+00006810: 6578 7472 6122 2c20 226f 7269 6769 6e22  extra", "origin"
+00006820: 2c20 6222 6f72 6967 696e 222c 2022 7365  , b"origin", "se
+00006830: 6375 7269 7479 222c 2062 2273 6563 7572  curity", b"secur
+00006840: 6974 7922 5d29 202d 3e20 6275 696c 7469  ity"]) -> builti
+00006850: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
+00006860: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
+00006870: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+00006880: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+00006890: 5b22 6163 636f 756e 745f 7365 7122 2c20  ["account_seq", 
+000068a0: 6222 6163 636f 756e 745f 7365 7122 2c20  b"account_seq", 
+000068b0: 2261 7564 6974 222c 2062 2261 7564 6974  "audit", b"audit
+000068c0: 222c 2022 6261 7369 6322 2c20 6222 6261  ", "basic", b"ba
+000068d0: 7369 6322 2c20 2263 6f6e 7665 7273 6174  sic", "conversat
+000068e0: 696f 6e73 222c 2062 2263 6f6e 7665 7273  ions", b"convers
+000068f0: 6174 696f 6e73 222c 2022 6461 7465 7469  ations", "dateti
+00006900: 6d65 7322 2c20 6222 6461 7465 7469 6d65  mes", b"datetime
+00006910: 7322 2c20 2264 656c 6574 655f 6669 656c  s", "delete_fiel
+00006920: 6473 222c 2062 2264 656c 6574 655f 6669  ds", b"delete_fi
+00006930: 656c 6473 222c 2022 646f 6e65 5f74 696d  elds", "done_tim
+00006940: 6522 2c20 6222 646f 6e65 5f74 696d 6522  e", b"done_time"
+00006950: 2c20 2265 7272 6f72 7322 2c20 6222 6572  , "errors", b"er
+00006960: 726f 7273 222c 2022 6578 7472 6122 2c20  rors", "extra", 
+00006970: 6222 6578 7472 6122 2c20 2265 7874 7261  b"extra", "extra
+00006980: 6374 6564 5f74 6578 7422 2c20 6222 6578  cted_text", b"ex
+00006990: 7472 6163 7465 645f 7465 7874 222c 2022  tracted_text", "
+000069a0: 6669 656c 645f 6c61 7267 655f 6d65 7461  field_large_meta
+000069b0: 6461 7461 222c 2062 2266 6965 6c64 5f6c  data", b"field_l
+000069c0: 6172 6765 5f6d 6574 6164 6174 6122 2c20  arge_metadata", 
+000069d0: 2266 6965 6c64 5f6d 6574 6164 6174 6122  "field_metadata"
+000069e0: 2c20 6222 6669 656c 645f 6d65 7461 6461  , b"field_metada
+000069f0: 7461 222c 2022 6669 656c 645f 7665 6374  ta", "field_vect
+00006a00: 6f72 7322 2c20 6222 6669 656c 645f 7665  ors", b"field_ve
+00006a10: 6374 6f72 7322 2c20 2266 696c 655f 6578  ctors", "file_ex
+00006a20: 7472 6163 7465 645f 6461 7461 222c 2062  tracted_data", b
+00006a30: 2266 696c 655f 6578 7472 6163 7465 645f  "file_extracted_
+00006a40: 6461 7461 222c 2022 6669 6c65 7322 2c20  data", "files", 
+00006a50: 6222 6669 6c65 7322 2c20 226b 6269 6422  b"files", "kbid"
+00006a60: 2c20 6222 6b62 6964 222c 2022 6b65 7977  , b"kbid", "keyw
+00006a70: 6f72 6473 6574 7322 2c20 6222 6b65 7977  ordsets", b"keyw
+00006a80: 6f72 6473 6574 7322 2c20 226c 6179 6f75  ordsets", "layou
+00006a90: 7473 222c 2062 226c 6179 6f75 7473 222c  ts", b"layouts",
+00006aa0: 2022 6c69 6e6b 5f65 7874 7261 6374 6564   "link_extracted
+00006ab0: 5f64 6174 6122 2c20 6222 6c69 6e6b 5f65  _data", b"link_e
+00006ac0: 7874 7261 6374 6564 5f64 6174 6122 2c20  xtracted_data", 
+00006ad0: 226c 696e 6b73 222c 2062 226c 696e 6b73  "links", b"links
+00006ae0: 222c 2022 6d75 6c74 6969 6422 2c20 6222  ", "multiid", b"
+00006af0: 6d75 6c74 6969 6422 2c20 226f 7269 6769  multiid", "origi
+00006b00: 6e22 2c20 6222 6f72 6967 696e 222c 2022  n", b"origin", "
+00006b10: 6f72 6967 696e 5f73 6571 222c 2062 226f  origin_seq", b"o
+00006b20: 7269 6769 6e5f 7365 7122 2c20 2270 7265  rigin_seq", "pre
+00006b30: 5f70 726f 6365 7373 696e 675f 7469 6d65  _processing_time
+00006b40: 222c 2062 2270 7265 5f70 726f 6365 7373  ", b"pre_process
+00006b50: 696e 675f 7469 6d65 222c 2022 7072 6f63  ing_time", "proc
+00006b60: 6573 7369 6e67 5f69 6422 2c20 6222 7072  essing_id", b"pr
+00006b70: 6f63 6573 7369 6e67 5f69 6422 2c20 2271  ocessing_id", "q
+00006b80: 7565 7374 696f 6e5f 616e 7377 6572 7322  uestion_answers"
+00006b90: 2c20 6222 7175 6573 7469 6f6e 5f61 6e73  , b"question_ans
+00006ba0: 7765 7273 222c 2022 7265 696e 6465 7822  wers", "reindex"
+00006bb0: 2c20 6222 7265 696e 6465 7822 2c20 2272  , b"reindex", "r
+00006bc0: 656c 6174 696f 6e73 222c 2062 2272 656c  elations", b"rel
+00006bd0: 6174 696f 6e73 222c 2022 7365 6375 7269  ations", "securi
+00006be0: 7479 222c 2062 2273 6563 7572 6974 7922  ty", b"security"
+00006bf0: 2c20 2273 6c6f 775f 7072 6f63 6573 7369  , "slow_processi
+00006c00: 6e67 5f74 696d 6522 2c20 6222 736c 6f77  ng_time", b"slow
+00006c10: 5f70 726f 6365 7373 696e 675f 7469 6d65  _processing_time
+00006c20: 222c 2022 736c 7567 222c 2062 2273 6c75  ", "slug", b"slu
+00006c30: 6722 2c20 2273 6f75 7263 6522 2c20 6222  g", "source", b"
+00006c40: 736f 7572 6365 222c 2022 7465 7874 7322  source", "texts"
+00006c50: 2c20 6222 7465 7874 7322 2c20 2274 7873  , b"texts", "txs
+00006c60: 6571 6964 222c 2062 2274 7873 6571 6964  eqid", b"txseqid
+00006c70: 222c 2022 7479 7065 222c 2062 2274 7970  ", "type", b"typ
+00006c80: 6522 2c20 2275 7365 725f 7665 6374 6f72  e", "user_vector
+00006c90: 7322 2c20 6222 7573 6572 5f76 6563 746f  s", b"user_vecto
+00006ca0: 7273 222c 2022 7575 6964 222c 2062 2275  rs", "uuid", b"u
+00006cb0: 7569 6422 5d29 202d 3e20 4e6f 6e65 3a20  uid"]) -> None: 
+00006cc0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4272  .....global___Br
+00006cd0: 6f6b 6572 4d65 7373 6167 6520 3d20 4272  okerMessage = Br
+00006ce0: 6f6b 6572 4d65 7373 6167 650a 0a40 7479  okerMessage..@ty
+00006cf0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+00006d00: 2042 726f 6b65 724d 6573 7361 6765 426c   BrokerMessageBl
+00006d10: 6f62 5265 6665 7265 6e63 6528 676f 6f67  obReference(goog
+00006d20: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+00006d30: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+00006d40: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00006d50: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00006d60: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+00006d70: 746f 720a 0a20 2020 204b 4249 445f 4649  tor..    KBID_FI
+00006d80: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00006d90: 7469 6e73 2e69 6e74 0a20 2020 2055 5549  tins.int.    UUI
+00006da0: 445f 4649 454c 445f 4e55 4d42 4552 3a20  D_FIELD_NUMBER: 
+00006db0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00006dc0: 2053 544f 5241 4745 5f4b 4559 5f46 4945   STORAGE_KEY_FIE
+00006dd0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00006de0: 696e 732e 696e 740a 2020 2020 6b62 6964  ins.int.    kbid
+00006df0: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+00006e00: 2020 2075 7569 643a 2062 7569 6c74 696e     uuid: builtin
+00006e10: 732e 7374 720a 2020 2020 7374 6f72 6167  s.str.    storag
+00006e20: 655f 6b65 793a 2062 7569 6c74 696e 732e  e_key: builtins.
+00006e30: 7374 720a 2020 2020 6465 6620 5f5f 696e  str.    def __in
+00006e40: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00006e50: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
+00006e60: 2020 2020 2020 206b 6269 643a 2062 7569         kbid: bui
+00006e70: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
+00006e80: 0a20 2020 2020 2020 2075 7569 643a 2062  .        uuid: b
+00006e90: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+00006ea0: 2e2c 0a20 2020 2020 2020 2073 746f 7261  .,.        stora
+00006eb0: 6765 5f6b 6579 3a20 6275 696c 7469 6e73  ge_key: builtins
+00006ec0: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+00006ed0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
+00006ee0: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
+00006ef0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+00006f00: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+00006f10: 616c 5b22 6b62 6964 222c 2062 226b 6269  al["kbid", b"kbi
+00006f20: 6422 2c20 2273 746f 7261 6765 5f6b 6579  d", "storage_key
+00006f30: 222c 2062 2273 746f 7261 6765 5f6b 6579  ", b"storage_key
+00006f40: 222c 2022 7575 6964 222c 2062 2275 7569  ", "uuid", b"uui
+00006f50: 6422 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  d"]) -> None: ..
+00006f60: 2e0a 0a67 6c6f 6261 6c5f 5f5f 4272 6f6b  ...global___Brok
+00006f70: 6572 4d65 7373 6167 6542 6c6f 6252 6566  erMessageBlobRef
+00006f80: 6572 656e 6365 203d 2042 726f 6b65 724d  erence = BrokerM
+00006f90: 6573 7361 6765 426c 6f62 5265 6665 7265  essageBlobRefere
+00006fa0: 6e63 650a 0a40 7479 7069 6e67 2e66 696e  nce..@typing.fin
+00006fb0: 616c 0a63 6c61 7373 2057 7269 7465 7253  al.class WriterS
+00006fc0: 7461 7475 7352 6573 706f 6e73 6528 676f  tatusResponse(go
+00006fd0: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+00006fe0: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+00006ff0: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
+00007000: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00007010: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
+00007020: 6970 746f 720a 0a20 2020 2040 7479 7069  iptor..    @typi
+00007030: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
+00007040: 7373 204d 7367 6964 456e 7472 7928 676f  ss MsgidEntry(go
+00007050: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+00007060: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+00007070: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
+00007080: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+00007090: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+000070a0: 6573 6372 6970 746f 720a 0a20 2020 2020  escriptor..     
+000070b0: 2020 204b 4559 5f46 4945 4c44 5f4e 554d     KEY_FIELD_NUM
+000070c0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+000070d0: 740a 2020 2020 2020 2020 5641 4c55 455f  t.        VALUE_
+000070e0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+000070f0: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
+00007100: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
+00007110: 2e73 7472 0a20 2020 2020 2020 2076 616c  .str.        val
+00007120: 7565 3a20 6275 696c 7469 6e73 2e69 6e74  ue: builtins.int
+00007130: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
+00007140: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
+00007150: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00007160: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00007170: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
+00007180: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+00007190: 2020 2020 2020 2020 2076 616c 7565 3a20           value: 
+000071a0: 6275 696c 7469 6e73 2e69 6e74 203d 202e  builtins.int = .
+000071b0: 2e2e 2c0a 2020 2020 2020 2020 2920 2d3e  ..,.        ) ->
+000071c0: 204e 6f6e 653a 202e 2e2e 0a20 2020 2020   None: ....     
+000071d0: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
+000071e0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+000071f0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+00007200: 616c 5b22 6b65 7922 2c20 6222 6b65 7922  al["key", b"key"
+00007210: 2c20 2276 616c 7565 222c 2062 2276 616c  , "value", b"val
+00007220: 7565 225d 2920 2d3e 204e 6f6e 653a 202e  ue"]) -> None: .
+00007230: 2e2e 0a0a 2020 2020 4b4e 4f57 4c45 4447  ....    KNOWLEDG
+00007240: 4542 4f58 4553 5f46 4945 4c44 5f4e 554d  EBOXES_FIELD_NUM
+00007250: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00007260: 740a 2020 2020 4d53 4749 445f 4649 454c  t.    MSGID_FIEL
+00007270: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00007280: 6e73 2e69 6e74 0a20 2020 2040 7072 6f70  ns.int.    @prop
+00007290: 6572 7479 0a20 2020 2064 6566 206b 6e6f  erty.    def kno
+000072a0: 776c 6564 6765 626f 7865 7328 7365 6c66  wledgeboxes(self
+000072b0: 2920 2d3e 2067 6f6f 676c 652e 7072 6f74  ) -> google.prot
+000072c0: 6f62 7566 2e69 6e74 6572 6e61 6c2e 636f  obuf.internal.co
+000072d0: 6e74 6169 6e65 7273 2e52 6570 6561 7465  ntainers.Repeate
+000072e0: 6453 6361 6c61 7246 6965 6c64 436f 6e74  dScalarFieldCont
+000072f0: 6169 6e65 725b 6275 696c 7469 6e73 2e73  ainer[builtins.s
+00007300: 7472 5d3a 202e 2e2e 0a20 2020 2040 7072  tr]: ....    @pr
+00007310: 6f70 6572 7479 0a20 2020 2064 6566 206d  operty.    def m
+00007320: 7367 6964 2873 656c 6629 202d 3e20 676f  sgid(self) -> go
+00007330: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+00007340: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
+00007350: 732e 5363 616c 6172 4d61 705b 6275 696c  s.ScalarMap[buil
+00007360: 7469 6e73 2e73 7472 2c20 6275 696c 7469  tins.str, builti
+00007370: 6e73 2e69 6e74 5d3a 0a20 2020 2020 2020  ns.int]:.       
+00007380: 2022 2222 6d61 7020 6f66 206c 6173 7420   """map of last 
+00007390: 6d65 7373 6167 6520 7072 6f63 6573 7365  message processe
+000073a0: 6422 2222 0a0a 2020 2020 6465 6620 5f5f  d"""..    def __
+000073b0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000073c0: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
+000073d0: 0a20 2020 2020 2020 206b 6e6f 776c 6564  .        knowled
+000073e0: 6765 626f 7865 733a 2063 6f6c 6c65 6374  geboxes: collect
+000073f0: 696f 6e73 2e61 6263 2e49 7465 7261 626c  ions.abc.Iterabl
+00007400: 655b 6275 696c 7469 6e73 2e73 7472 5d20  e[builtins.str] 
+00007410: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
+00007420: 2020 2020 2020 6d73 6769 643a 2063 6f6c        msgid: col
+00007430: 6c65 6374 696f 6e73 2e61 6263 2e4d 6170  lections.abc.Map
+00007440: 7069 6e67 5b62 7569 6c74 696e 732e 7374  ping[builtins.st
+00007450: 722c 2062 7569 6c74 696e 732e 696e 745d  r, builtins.int]
+00007460: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00007470: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+00007480: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+00007490: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+000074a0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+000074b0: 7465 7261 6c5b 226b 6e6f 776c 6564 6765  teral["knowledge
+000074c0: 626f 7865 7322 2c20 6222 6b6e 6f77 6c65  boxes", b"knowle
+000074d0: 6467 6562 6f78 6573 222c 2022 6d73 6769  dgeboxes", "msgi
+000074e0: 6422 2c20 6222 6d73 6769 6422 5d29 202d  d", b"msgid"]) -
+000074f0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+00007500: 6261 6c5f 5f5f 5772 6974 6572 5374 6174  bal___WriterStat
+00007510: 7573 5265 7370 6f6e 7365 203d 2057 7269  usResponse = Wri
+00007520: 7465 7253 7461 7475 7352 6573 706f 6e73  terStatusRespons
+00007530: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
+00007540: 0a63 6c61 7373 2057 7269 7465 7253 7461  .class WriterSta
+00007550: 7475 7352 6571 7565 7374 2867 6f6f 676c  tusRequest(googl
+00007560: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+00007570: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+00007580: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+00007590: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+000075a0: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
+000075b0: 6f72 0a0a 2020 2020 6465 6620 5f5f 696e  or..    def __in
+000075c0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000075d0: 6c66 2c0a 2020 2020 2920 2d3e 204e 6f6e  lf,.    ) -> Non
+000075e0: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+000075f0: 5f57 7269 7465 7253 7461 7475 7352 6571  _WriterStatusReq
+00007600: 7565 7374 203d 2057 7269 7465 7253 7461  uest = WriterSta
+00007610: 7475 7352 6571 7565 7374 0a0a 4074 7970  tusRequest..@typ
+00007620: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
+00007630: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
+00007640: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
+00007650: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+00007660: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+00007670: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00007680: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00007690: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+000076a0: 0a20 2020 204b 425f 4649 454c 445f 4e55  .    KB_FIELD_NU
+000076b0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+000076c0: 6e74 0a20 2020 2047 524f 5550 5f46 4945  nt.    GROUP_FIE
+000076d0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+000076e0: 696e 732e 696e 740a 2020 2020 454e 5449  ins.int.    ENTI
+000076f0: 5449 4553 5f46 4945 4c44 5f4e 554d 4245  TIES_FIELD_NUMBE
+00007700: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00007710: 2020 2020 6772 6f75 703a 2062 7569 6c74      group: built
+00007720: 696e 732e 7374 720a 2020 2020 4070 726f  ins.str.    @pro
+00007730: 7065 7274 790a 2020 2020 6465 6620 6b62  perty.    def kb
+00007740: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
+00007750: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
+00007760: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
+00007770: 6564 6765 426f 7849 443a 202e 2e2e 0a20  edgeBoxID: .... 
+00007780: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00007790: 2064 6566 2065 6e74 6974 6965 7328 7365   def entities(se
+000077a0: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
+000077b0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+000077c0: 626f 785f 7062 322e 456e 7469 7469 6573  box_pb2.Entities
+000077d0: 4772 6f75 703a 202e 2e2e 0a20 2020 2064  Group: ....    d
+000077e0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+000077f0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00007800: 2020 202a 2c0a 2020 2020 2020 2020 6b62     *,.        kb
+00007810: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+00007820: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+00007830: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
+00007840: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
+00007850: 2020 2020 2020 2020 6772 6f75 703a 2062          group: b
+00007860: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+00007870: 2e2c 0a20 2020 2020 2020 2065 6e74 6974  .,.        entit
+00007880: 6965 733a 206e 7563 6c69 6164 625f 7072  ies: nucliadb_pr
+00007890: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
+000078a0: 785f 7062 322e 456e 7469 7469 6573 4772  x_pb2.EntitiesGr
+000078b0: 6f75 7020 7c20 4e6f 6e65 203d 202e 2e2e  oup | None = ...
+000078c0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+000078d0: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
+000078e0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+000078f0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+00007900: 6974 6572 616c 5b22 656e 7469 7469 6573  iteral["entities
+00007910: 222c 2062 2265 6e74 6974 6965 7322 2c20  ", b"entities", 
+00007920: 226b 6222 2c20 6222 6b62 225d 2920 2d3e  "kb", b"kb"]) ->
+00007930: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
+00007940: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+00007950: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00007960: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00007970: 4c69 7465 7261 6c5b 2265 6e74 6974 6965  Literal["entitie
+00007980: 7322 2c20 6222 656e 7469 7469 6573 222c  s", b"entities",
+00007990: 2022 6772 6f75 7022 2c20 6222 6772 6f75   "group", b"grou
+000079a0: 7022 2c20 226b 6222 2c20 6222 6b62 225d  p", "kb", b"kb"]
+000079b0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
+000079c0: 676c 6f62 616c 5f5f 5f4e 6577 456e 7469  global___NewEnti
+000079d0: 7469 6573 4772 6f75 7052 6571 7565 7374  tiesGroupRequest
+000079e0: 203d 204e 6577 456e 7469 7469 6573 4772   = NewEntitiesGr
+000079f0: 6f75 7052 6571 7565 7374 0a0a 4074 7970  oupRequest..@typ
+00007a00: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
+00007a10: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
+00007a20: 5265 7370 6f6e 7365 2867 6f6f 676c 652e  Response(google.
+00007a30: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
+00007a40: 2e4d 6573 7361 6765 293a 0a20 2020 2044  .Message):.    D
+00007a50: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+00007a60: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+00007a70: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
+00007a80: 0a0a 2020 2020 636c 6173 7320 5f53 7461  ..    class _Sta
+00007a90: 7475 733a 0a20 2020 2020 2020 2056 616c  tus:.        Val
+00007aa0: 7565 5479 7065 203d 2074 7970 696e 672e  ueType = typing.
+00007ab0: 4e65 7754 7970 6528 2256 616c 7565 5479  NewType("ValueTy
+00007ac0: 7065 222c 2062 7569 6c74 696e 732e 696e  pe", builtins.in
+00007ad0: 7429 0a20 2020 2020 2020 2056 3a20 7479  t).        V: ty
+00007ae0: 7069 6e67 5f65 7874 656e 7369 6f6e 732e  ping_extensions.
+00007af0: 5479 7065 416c 6961 7320 3d20 5661 6c75  TypeAlias = Valu
+00007b00: 6554 7970 650a 0a20 2020 2063 6c61 7373  eType..    class
+00007b10: 205f 5374 6174 7573 456e 756d 5479 7065   _StatusEnumType
+00007b20: 5772 6170 7065 7228 676f 6f67 6c65 2e70  Wrapper(google.p
+00007b30: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
+00007b40: 2e65 6e75 6d5f 7479 7065 5f77 7261 7070  .enum_type_wrapp
+00007b50: 6572 2e5f 456e 756d 5479 7065 5772 6170  er._EnumTypeWrap
+00007b60: 7065 725b 4e65 7745 6e74 6974 6965 7347  per[NewEntitiesG
+00007b70: 726f 7570 5265 7370 6f6e 7365 2e5f 5374  roupResponse._St
+00007b80: 6174 7573 2e56 616c 7565 5479 7065 5d2c  atus.ValueType],
+00007b90: 2062 7569 6c74 696e 732e 7479 7065 293a   builtins.type):
+00007ba0: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
+00007bb0: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+00007bc0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+00007bd0: 456e 756d 4465 7363 7269 7074 6f72 0a20  EnumDescriptor. 
+00007be0: 2020 2020 2020 204f 4b3a 204e 6577 456e         OK: NewEn
+00007bf0: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+00007c00: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+00007c10: 6554 7970 6520 2023 2030 0a20 2020 2020  eType  # 0.     
+00007c20: 2020 2045 5252 4f52 3a20 4e65 7745 6e74     ERROR: NewEnt
+00007c30: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+00007c40: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
+00007c50: 5479 7065 2020 2320 310a 2020 2020 2020  Type  # 1.      
+00007c60: 2020 4b42 5f4e 4f54 5f46 4f55 4e44 3a20    KB_NOT_FOUND: 
+00007c70: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
+00007c80: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
+00007c90: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+00007ca0: 2020 2020 2020 2020 414c 5245 4144 595f          ALREADY_
+00007cb0: 4558 4953 5453 3a20 4e65 7745 6e74 6974  EXISTS: NewEntit
+00007cc0: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
+00007cd0: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
+00007ce0: 7065 2020 2320 330a 0a20 2020 2063 6c61  pe  # 3..    cla
+00007cf0: 7373 2053 7461 7475 7328 5f53 7461 7475  ss Status(_Statu
+00007d00: 732c 206d 6574 6163 6c61 7373 3d5f 5374  s, metaclass=_St
+00007d10: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
+00007d20: 7065 7229 3a20 2e2e 2e0a 2020 2020 4f4b  per): ....    OK
+00007d30: 3a20 4e65 7745 6e74 6974 6965 7347 726f  : NewEntitiesGro
+00007d40: 7570 5265 7370 6f6e 7365 2e53 7461 7475  upResponse.Statu
+00007d50: 732e 5661 6c75 6554 7970 6520 2023 2030  s.ValueType  # 0
+00007d60: 0a20 2020 2045 5252 4f52 3a20 4e65 7745  .    ERROR: NewE
+00007d70: 6e74 6974 6965 7347 726f 7570 5265 7370  ntitiesGroupResp
+00007d80: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
+00007d90: 6554 7970 6520 2023 2031 0a20 2020 204b  eType  # 1.    K
+00007da0: 425f 4e4f 545f 464f 554e 443a 204e 6577  B_NOT_FOUND: New
+00007db0: 456e 7469 7469 6573 4772 6f75 7052 6573  EntitiesGroupRes
+00007dc0: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+00007dd0: 7565 5479 7065 2020 2320 320a 2020 2020  ueType  # 2.    
+00007de0: 414c 5245 4144 595f 4558 4953 5453 3a20  ALREADY_EXISTS: 
+00007df0: 4e65 7745 6e74 6974 6965 7347 726f 7570  NewEntitiesGroup
+00007e00: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
+00007e10: 5661 6c75 6554 7970 6520 2023 2033 0a0a  ValueType  # 3..
+00007e20: 2020 2020 5354 4154 5553 5f46 4945 4c44      STATUS_FIELD
+00007e30: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00007e40: 732e 696e 740a 2020 2020 7374 6174 7573  s.int.    status
+00007e50: 3a20 676c 6f62 616c 5f5f 5f4e 6577 456e  : global___NewEn
+00007e60: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+00007e70: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+00007e80: 5479 7065 0a20 2020 2064 6566 205f 5f69  Type.    def __i
+00007e90: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00007ea0: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
+00007eb0: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
+00007ec0: 676c 6f62 616c 5f5f 5f4e 6577 456e 7469  global___NewEnti
+00007ed0: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
+00007ee0: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+00007ef0: 7065 203d 202e 2e2e 2c0a 2020 2020 2920  pe = ...,.    ) 
+00007f00: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+00007f10: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
+00007f20: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+00007f30: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+00007f40: 5b22 7374 6174 7573 222c 2062 2273 7461  ["status", b"sta
+00007f50: 7475 7322 5d29 202d 3e20 4e6f 6e65 3a20  tus"]) -> None: 
+00007f60: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4e65  .....global___Ne
+00007f70: 7745 6e74 6974 6965 7347 726f 7570 5265  wEntitiesGroupRe
+00007f80: 7370 6f6e 7365 203d 204e 6577 456e 7469  sponse = NewEnti
+00007f90: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
+00007fa0: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
+00007fb0: 0a63 6c61 7373 2053 6574 456e 7469 7469  .class SetEntiti
+00007fc0: 6573 5265 7175 6573 7428 676f 6f67 6c65  esRequest(google
+00007fd0: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
+00007fe0: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
+00007ff0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+00008000: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+00008010: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
+00008020: 720a 0a20 2020 204b 425f 4649 454c 445f  r..    KB_FIELD_
+00008030: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00008040: 2e69 6e74 0a20 2020 2047 524f 5550 5f46  .int.    GROUP_F
+00008050: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00008060: 6c74 696e 732e 696e 740a 2020 2020 454e  ltins.int.    EN
+00008070: 5449 5449 4553 5f46 4945 4c44 5f4e 554d  TITIES_FIELD_NUM
+00008080: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+00008090: 740a 2020 2020 6772 6f75 703a 2062 7569  t.    group: bui
+000080a0: 6c74 696e 732e 7374 720a 2020 2020 4070  ltins.str.    @p
+000080b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+000080c0: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
+000080d0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+000080e0: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
+000080f0: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
+00008100: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00008110: 2020 2064 6566 2065 6e74 6974 6965 7328     def entities(
+00008120: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+00008130: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+00008140: 6765 626f 785f 7062 322e 456e 7469 7469  gebox_pb2.Entiti
+00008150: 6573 4772 6f75 703a 202e 2e2e 0a20 2020  esGroup: ....   
+00008160: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00008170: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00008180: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00008190: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
+000081a0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+000081b0: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
+000081c0: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
+000081d0: 2c0a 2020 2020 2020 2020 6772 6f75 703a  ,.        group:
+000081e0: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
+000081f0: 2e2e 2e2c 0a20 2020 2020 2020 2065 6e74  ...,.        ent
+00008200: 6974 6965 733a 206e 7563 6c69 6164 625f  ities: nucliadb_
+00008210: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+00008220: 626f 785f 7062 322e 456e 7469 7469 6573  box_pb2.Entities
+00008230: 4772 6f75 7020 7c20 4e6f 6e65 203d 202e  Group | None = .
+00008240: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
+00008250: 653a 202e 2e2e 0a20 2020 2064 6566 2048  e: ....    def H
+00008260: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
+00008270: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+00008280: 2e4c 6974 6572 616c 5b22 656e 7469 7469  .Literal["entiti
+00008290: 6573 222c 2062 2265 6e74 6974 6965 7322  es", b"entities"
+000082a0: 2c20 226b 6222 2c20 6222 6b62 225d 2920  , "kb", b"kb"]) 
+000082b0: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
+000082c0: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+000082d0: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+000082e0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+000082f0: 672e 4c69 7465 7261 6c5b 2265 6e74 6974  g.Literal["entit
+00008300: 6965 7322 2c20 6222 656e 7469 7469 6573  ies", b"entities
+00008310: 222c 2022 6772 6f75 7022 2c20 6222 6772  ", "group", b"gr
+00008320: 6f75 7022 2c20 226b 6222 2c20 6222 6b62  oup", "kb", b"kb
+00008330: 225d 2920 2d3e 204e 6f6e 653a 202e 2e2e  "]) -> None: ...
+00008340: 0a0a 676c 6f62 616c 5f5f 5f53 6574 456e  ..global___SetEn
+00008350: 7469 7469 6573 5265 7175 6573 7420 3d20  titiesRequest = 
+00008360: 5365 7445 6e74 6974 6965 7352 6571 7565  SetEntitiesReque
+00008370: 7374 0a0a 4074 7970 696e 672e 6669 6e61  st..@typing.fina
+00008380: 6c0a 636c 6173 7320 5570 6461 7465 456e  l.class UpdateEn
+00008390: 7469 7469 6573 4772 6f75 7052 6571 7565  titiesGroupReque
+000083a0: 7374 2867 6f6f 676c 652e 7072 6f74 6f62  st(google.protob
+000083b0: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
+000083c0: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
+000083d0: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+000083e0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+000083f0: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+00008400: 4074 7970 696e 672e 6669 6e61 6c0a 2020  @typing.final.  
+00008410: 2020 636c 6173 7320 4164 6445 6e74 7279    class AddEntry
+00008420: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
+00008430: 2e6d 6573 7361 6765 2e4d 6573 7361 6765  .message.Message
+00008440: 293a 0a20 2020 2020 2020 2044 4553 4352  ):.        DESCR
+00008450: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+00008460: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+00008470: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+00008480: 2020 2020 2020 4b45 595f 4649 454c 445f        KEY_FIELD_
+00008490: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+000084a0: 2e69 6e74 0a20 2020 2020 2020 2056 414c  .int.        VAL
+000084b0: 5545 5f46 4945 4c44 5f4e 554d 4245 523a  UE_FIELD_NUMBER:
+000084c0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+000084d0: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
+000084e0: 696e 732e 7374 720a 2020 2020 2020 2020  ins.str.        
+000084f0: 4070 726f 7065 7274 790a 2020 2020 2020  @property.      
+00008500: 2020 6465 6620 7661 6c75 6528 7365 6c66    def value(self
+00008510: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
+00008520: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
+00008530: 785f 7062 322e 456e 7469 7479 3a20 2e2e  x_pb2.Entity: ..
+00008540: 2e0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
+00008550: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00008560: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00008570: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+00008580: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
+00008590: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+000085a0: 2020 2020 2020 2020 2020 7661 6c75 653a            value:
+000085b0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+000085c0: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+000085d0: 322e 456e 7469 7479 207c 204e 6f6e 6520  2.Entity | None 
+000085e0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
+000085f0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+00008600: 2020 2020 2020 6465 6620 4861 7346 6965        def HasFie
+00008610: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+00008620: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+00008630: 7261 6c5b 2276 616c 7565 222c 2062 2276  ral["value", b"v
+00008640: 616c 7565 225d 2920 2d3e 2062 7569 6c74  alue"]) -> built
+00008650: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
+00008660: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
+00008670: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+00008680: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+00008690: 7465 7261 6c5b 226b 6579 222c 2062 226b  teral["key", b"k
+000086a0: 6579 222c 2022 7661 6c75 6522 2c20 6222  ey", "value", b"
+000086b0: 7661 6c75 6522 5d29 202d 3e20 4e6f 6e65  value"]) -> None
+000086c0: 3a20 2e2e 2e0a 0a20 2020 2040 7479 7069  : .....    @typi
+000086d0: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
+000086e0: 7373 2055 7064 6174 6545 6e74 7279 2867  ss UpdateEntry(g
+000086f0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
+00008700: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
+00008710: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
+00008720: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+00008730: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+00008740: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+00008750: 2020 2020 4b45 595f 4649 454c 445f 4e55      KEY_FIELD_NU
+00008760: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00008770: 6e74 0a20 2020 2020 2020 2056 414c 5545  nt.        VALUE
+00008780: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00008790: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+000087a0: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
+000087b0: 732e 7374 720a 2020 2020 2020 2020 4070  s.str.        @p
+000087c0: 726f 7065 7274 790a 2020 2020 2020 2020  roperty.        
+000087d0: 6465 6620 7661 6c75 6528 7365 6c66 2920  def value(self) 
+000087e0: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
+000087f0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+00008800: 7062 322e 456e 7469 7479 3a20 2e2e 2e0a  pb2.Entity: ....
+00008810: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
+00008820: 6974 5f5f 280a 2020 2020 2020 2020 2020  it__(.          
+00008830: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00008840: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
+00008850: 2020 206b 6579 3a20 6275 696c 7469 6e73     key: builtins
+00008860: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+00008870: 2020 2020 2020 2020 7661 6c75 653a 206e          value: n
+00008880: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+00008890: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+000088a0: 456e 7469 7479 207c 204e 6f6e 6520 3d20  Entity | None = 
+000088b0: 2e2e 2e2c 0a20 2020 2020 2020 2029 202d  ...,.        ) -
+000088c0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+000088d0: 2020 2020 6465 6620 4861 7346 6965 6c64      def HasField
+000088e0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+000088f0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+00008900: 6c5b 2276 616c 7565 222c 2062 2276 616c  l["value", b"val
+00008910: 7565 225d 2920 2d3e 2062 7569 6c74 696e  ue"]) -> builtin
+00008920: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
+00008930: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
+00008940: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+00008950: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+00008960: 7261 6c5b 226b 6579 222c 2062 226b 6579  ral["key", b"key
+00008970: 222c 2022 7661 6c75 6522 2c20 6222 7661  ", "value", b"va
+00008980: 6c75 6522 5d29 202d 3e20 4e6f 6e65 3a20  lue"]) -> None: 
+00008990: 2e2e 2e0a 0a20 2020 204b 425f 4649 454c  .....    KB_FIEL
+000089a0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+000089b0: 6e73 2e69 6e74 0a20 2020 2047 524f 5550  ns.int.    GROUP
+000089c0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+000089d0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+000089e0: 4144 445f 4649 454c 445f 4e55 4d42 4552  ADD_FIELD_NUMBER
+000089f0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00008a00: 2020 2055 5044 4154 455f 4649 454c 445f     UPDATE_FIELD_
+00008a10: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00008a20: 2e69 6e74 0a20 2020 2044 454c 4554 455f  .int.    DELETE_
+00008a30: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00008a40: 696c 7469 6e73 2e69 6e74 0a20 2020 2054  iltins.int.    T
+00008a50: 4954 4c45 5f46 4945 4c44 5f4e 554d 4245  ITLE_FIELD_NUMBE
+00008a60: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00008a70: 2020 2020 434f 4c4f 525f 4649 454c 445f      COLOR_FIELD_
+00008a80: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00008a90: 2e69 6e74 0a20 2020 2067 726f 7570 3a20  .int.    group: 
+00008aa0: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
+00008ab0: 2074 6974 6c65 3a20 6275 696c 7469 6e73   title: builtins
+00008ac0: 2e73 7472 0a20 2020 2063 6f6c 6f72 3a20  .str.    color: 
+00008ad0: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
+00008ae0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00008af0: 6566 206b 6228 7365 6c66 2920 2d3e 206e  ef kb(self) -> n
+00008b00: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+00008b10: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+00008b20: 4b6e 6f77 6c65 6467 6542 6f78 4944 3a20  KnowledgeBoxID: 
+00008b30: 2e2e 2e0a 2020 2020 4070 726f 7065 7274  ....    @propert
+00008b40: 790a 2020 2020 6465 6620 6164 6428 7365  y.    def add(se
+00008b50: 6c66 2920 2d3e 2067 6f6f 676c 652e 7072  lf) -> google.pr
+00008b60: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
+00008b70: 636f 6e74 6169 6e65 7273 2e4d 6573 7361  containers.Messa
+00008b80: 6765 4d61 705b 6275 696c 7469 6e73 2e73  geMap[builtins.s
+00008b90: 7472 2c20 6e75 636c 6961 6462 5f70 726f  tr, nucliadb_pro
+00008ba0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+00008bb0: 5f70 6232 2e45 6e74 6974 795d 3a0a 2020  _pb2.Entity]:.  
+00008bc0: 2020 2020 2020 2222 2265 6e74 6974 795f        """entity_
+00008bd0: 6964 3a20 456e 7469 7479 2222 220a 0a20  id: Entity""".. 
+00008be0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00008bf0: 2064 6566 2075 7064 6174 6528 7365 6c66   def update(self
+00008c00: 2920 2d3e 2067 6f6f 676c 652e 7072 6f74  ) -> google.prot
+00008c10: 6f62 7566 2e69 6e74 6572 6e61 6c2e 636f  obuf.internal.co
+00008c20: 6e74 6169 6e65 7273 2e4d 6573 7361 6765  ntainers.Message
+00008c30: 4d61 705b 6275 696c 7469 6e73 2e73 7472  Map[builtins.str
+00008c40: 2c20 6e75 636c 6961 6462 5f70 726f 746f  , nucliadb_proto
+00008c50: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+00008c60: 6232 2e45 6e74 6974 795d 3a0a 2020 2020  b2.Entity]:.    
+00008c70: 2020 2020 2222 2265 6e74 6974 795f 6964      """entity_id
+00008c80: 3a20 456e 7469 7479 2222 220a 0a20 2020  : Entity"""..   
+00008c90: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00008ca0: 6566 2064 656c 6574 6528 7365 6c66 2920  ef delete(self) 
+00008cb0: 2d3e 2067 6f6f 676c 652e 7072 6f74 6f62  -> google.protob
+00008cc0: 7566 2e69 6e74 6572 6e61 6c2e 636f 6e74  uf.internal.cont
+00008cd0: 6169 6e65 7273 2e52 6570 6561 7465 6453  ainers.RepeatedS
+00008ce0: 6361 6c61 7246 6965 6c64 436f 6e74 6169  calarFieldContai
+00008cf0: 6e65 725b 6275 696c 7469 6e73 2e73 7472  ner[builtins.str
+00008d00: 5d3a 0a20 2020 2020 2020 2022 2222 656e  ]:.        """en
+00008d10: 7469 7479 5f69 6422 2222 0a0a 2020 2020  tity_id"""..    
+00008d20: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00008d30: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00008d40: 2020 2020 2a2c 0a20 2020 2020 2020 206b      *,.        k
+00008d50: 623a 206e 7563 6c69 6164 625f 7072 6f74  b: nucliadb_prot
+00008d60: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+00008d70: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
+00008d80: 4944 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ID | None = ...,
+00008d90: 0a20 2020 2020 2020 2067 726f 7570 3a20  .        group: 
+00008da0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
+00008db0: 2e2e 2c0a 2020 2020 2020 2020 6164 643a  ..,.        add:
+00008dc0: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+00008dd0: 2e4d 6170 7069 6e67 5b62 7569 6c74 696e  .Mapping[builtin
+00008de0: 732e 7374 722c 206e 7563 6c69 6164 625f  s.str, nucliadb_
+00008df0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+00008e00: 626f 785f 7062 322e 456e 7469 7479 5d20  box_pb2.Entity] 
+00008e10: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
+00008e20: 2020 2020 2020 7570 6461 7465 3a20 636f        update: co
+00008e30: 6c6c 6563 7469 6f6e 732e 6162 632e 4d61  llections.abc.Ma
+00008e40: 7070 696e 675b 6275 696c 7469 6e73 2e73  pping[builtins.s
+00008e50: 7472 2c20 6e75 636c 6961 6462 5f70 726f  tr, nucliadb_pro
+00008e60: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+00008e70: 5f70 6232 2e45 6e74 6974 795d 207c 204e  _pb2.Entity] | N
+00008e80: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+00008e90: 2020 2064 656c 6574 653a 2063 6f6c 6c65     delete: colle
+00008ea0: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
+00008eb0: 626c 655b 6275 696c 7469 6e73 2e73 7472  ble[builtins.str
+00008ec0: 5d20 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  ] | None = ...,.
+00008ed0: 2020 2020 2020 2020 7469 746c 653a 2062          title: b
+00008ee0: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+00008ef0: 2e2c 0a20 2020 2020 2020 2063 6f6c 6f72  .,.        color
+00008f00: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+00008f10: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+00008f20: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+00008f30: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
+00008f40: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+00008f50: 6e67 2e4c 6974 6572 616c 5b22 6b62 222c  ng.Literal["kb",
+00008f60: 2062 226b 6222 5d29 202d 3e20 6275 696c   b"kb"]) -> buil
+00008f70: 7469 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20  tins.bool: .... 
+00008f80: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
+00008f90: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
+00008fa0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
+00008fb0: 616c 5b22 6164 6422 2c20 6222 6164 6422  al["add", b"add"
+00008fc0: 2c20 2263 6f6c 6f72 222c 2062 2263 6f6c  , "color", b"col
+00008fd0: 6f72 222c 2022 6465 6c65 7465 222c 2062  or", "delete", b
+00008fe0: 2264 656c 6574 6522 2c20 2267 726f 7570  "delete", "group
+00008ff0: 222c 2062 2267 726f 7570 222c 2022 6b62  ", b"group", "kb
+00009000: 222c 2062 226b 6222 2c20 2274 6974 6c65  ", b"kb", "title
+00009010: 222c 2062 2274 6974 6c65 222c 2022 7570  ", b"title", "up
+00009020: 6461 7465 222c 2062 2275 7064 6174 6522  date", b"update"
+00009030: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+00009040: 0a67 6c6f 6261 6c5f 5f5f 5570 6461 7465  .global___Update
+00009050: 456e 7469 7469 6573 4772 6f75 7052 6571  EntitiesGroupReq
+00009060: 7565 7374 203d 2055 7064 6174 6545 6e74  uest = UpdateEnt
+00009070: 6974 6965 7347 726f 7570 5265 7175 6573  itiesGroupReques
+00009080: 740a 0a40 7479 7069 6e67 2e66 696e 616c  t..@typing.final
+00009090: 0a63 6c61 7373 2055 7064 6174 6545 6e74  .class UpdateEnt
+000090a0: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+000090b0: 7365 2867 6f6f 676c 652e 7072 6f74 6f62  se(google.protob
+000090c0: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
+000090d0: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
+000090e0: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+000090f0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+00009100: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+00009110: 636c 6173 7320 5f53 7461 7475 733a 0a20  class _Status:. 
+00009120: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
+00009130: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
+00009140: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
+00009150: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
+00009160: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
+00009170: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
+00009180: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
+00009190: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
+000091a0: 7573 456e 756d 5479 7065 5772 6170 7065  usEnumTypeWrappe
+000091b0: 7228 676f 6f67 6c65 2e70 726f 746f 6275  r(google.protobu
+000091c0: 662e 696e 7465 726e 616c 2e65 6e75 6d5f  f.internal.enum_
+000091d0: 7479 7065 5f77 7261 7070 6572 2e5f 456e  type_wrapper._En
+000091e0: 756d 5479 7065 5772 6170 7065 725b 5570  umTypeWrapper[Up
+000091f0: 6461 7465 456e 7469 7469 6573 4772 6f75  dateEntitiesGrou
+00009200: 7052 6573 706f 6e73 652e 5f53 7461 7475  pResponse._Statu
+00009210: 732e 5661 6c75 6554 7970 655d 2c20 6275  s.ValueType], bu
+00009220: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
+00009230: 2020 2020 2020 4445 5343 5249 5054 4f52        DESCRIPTOR
+00009240: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+00009250: 662e 6465 7363 7269 7074 6f72 2e45 6e75  f.descriptor.Enu
+00009260: 6d44 6573 6372 6970 746f 720a 2020 2020  mDescriptor.    
+00009270: 2020 2020 4f4b 3a20 5570 6461 7465 456e      OK: UpdateEn
+00009280: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+00009290: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+000092a0: 6554 7970 6520 2023 2030 0a20 2020 2020  eType  # 0.     
+000092b0: 2020 2045 5252 4f52 3a20 5570 6461 7465     ERROR: Update
+000092c0: 456e 7469 7469 6573 4772 6f75 7052 6573  EntitiesGroupRes
+000092d0: 706f 6e73 652e 5f53 7461 7475 732e 5661  ponse._Status.Va
+000092e0: 6c75 6554 7970 6520 2023 2031 0a20 2020  lueType  # 1.   
+000092f0: 2020 2020 204b 425f 4e4f 545f 464f 554e       KB_NOT_FOUN
+00009300: 443a 2055 7064 6174 6545 6e74 6974 6965  D: UpdateEntitie
+00009310: 7347 726f 7570 5265 7370 6f6e 7365 2e5f  sGroupResponse._
+00009320: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+00009330: 2020 2320 320a 2020 2020 2020 2020 454e    # 2.        EN
+00009340: 5449 5449 4553 5f47 524f 5550 5f4e 4f54  TITIES_GROUP_NOT
+00009350: 5f46 4f55 4e44 3a20 5570 6461 7465 456e  _FOUND: UpdateEn
+00009360: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+00009370: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+00009380: 6554 7970 6520 2023 2033 0a0a 2020 2020  eType  # 3..    
+00009390: 636c 6173 7320 5374 6174 7573 285f 5374  class Status(_St
+000093a0: 6174 7573 2c20 6d65 7461 636c 6173 733d  atus, metaclass=
+000093b0: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
+000093c0: 7261 7070 6572 293a 202e 2e2e 0a20 2020  rapper): ....   
+000093d0: 204f 4b3a 2055 7064 6174 6545 6e74 6974   OK: UpdateEntit
+000093e0: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
+000093f0: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
+00009400: 6520 2023 2030 0a20 2020 2045 5252 4f52  e  # 0.    ERROR
+00009410: 3a20 5570 6461 7465 456e 7469 7469 6573  : UpdateEntities
+00009420: 4772 6f75 7052 6573 706f 6e73 652e 5374  GroupResponse.St
+00009430: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+00009440: 2320 310a 2020 2020 4b42 5f4e 4f54 5f46  # 1.    KB_NOT_F
+00009450: 4f55 4e44 3a20 5570 6461 7465 456e 7469  OUND: UpdateEnti
+00009460: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
+00009470: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+00009480: 7065 2020 2320 320a 2020 2020 454e 5449  pe  # 2.    ENTI
+00009490: 5449 4553 5f47 524f 5550 5f4e 4f54 5f46  TIES_GROUP_NOT_F
+000094a0: 4f55 4e44 3a20 5570 6461 7465 456e 7469  OUND: UpdateEnti
+000094b0: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
+000094c0: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+000094d0: 7065 2020 2320 330a 0a20 2020 2053 5441  pe  # 3..    STA
+000094e0: 5455 535f 4649 454c 445f 4e55 4d42 4552  TUS_FIELD_NUMBER
+000094f0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00009500: 2020 2073 7461 7475 733a 2067 6c6f 6261     status: globa
+00009510: 6c5f 5f5f 5570 6461 7465 456e 7469 7469  l___UpdateEntiti
+00009520: 6573 4772 6f75 7052 6573 706f 6e73 652e  esGroupResponse.
+00009530: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+00009540: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00009550: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00009560: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+00009570: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
+00009580: 616c 5f5f 5f55 7064 6174 6545 6e74 6974  al___UpdateEntit
+00009590: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
+000095a0: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
+000095b0: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
+000095c0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+000095d0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+000095e0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+000095f0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00009600: 2273 7461 7475 7322 2c20 6222 7374 6174  "status", b"stat
+00009610: 7573 225d 2920 2d3e 204e 6f6e 653a 202e  us"]) -> None: .
+00009620: 2e2e 0a0a 676c 6f62 616c 5f5f 5f55 7064  ....global___Upd
+00009630: 6174 6545 6e74 6974 6965 7347 726f 7570  ateEntitiesGroup
+00009640: 5265 7370 6f6e 7365 203d 2055 7064 6174  Response = Updat
+00009650: 6545 6e74 6974 6965 7347 726f 7570 5265  eEntitiesGroupRe
+00009660: 7370 6f6e 7365 0a0a 4074 7970 696e 672e  sponse..@typing.
+00009670: 6669 6e61 6c0a 636c 6173 7320 4c69 7374  final.class List
+00009680: 456e 7469 7469 6573 4772 6f75 7073 5265  EntitiesGroupsRe
+00009690: 7175 6573 7428 676f 6f67 6c65 2e70 726f  quest(google.pro
+000096a0: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
+000096b0: 7373 6167 6529 3a0a 2020 2020 4445 5343  ssage):.    DESC
+000096c0: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
+000096d0: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
+000096e0: 6f72 2e44 6573 6372 6970 746f 720a 0a20  or.Descriptor.. 
+000096f0: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
+00009700: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00009710: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00009720: 2020 2064 6566 206b 6228 7365 6c66 2920     def kb(self) 
+00009730: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
+00009740: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+00009750: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
+00009760: 4944 3a20 2e2e 2e0a 2020 2020 6465 6620  ID: ....    def 
+00009770: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00009780: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00009790: 2a2c 0a20 2020 2020 2020 206b 623a 206e  *,.        kb: n
+000097a0: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+000097b0: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+000097c0: 4b6e 6f77 6c65 6467 6542 6f78 4944 207c  KnowledgeBoxID |
+000097d0: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
+000097e0: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+000097f0: 2020 2020 6465 6620 4861 7346 6965 6c64      def HasField
+00009800: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+00009810: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+00009820: 6c5b 226b 6222 2c20 6222 6b62 225d 2920  l["kb", b"kb"]) 
+00009830: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
+00009840: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+00009850: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+00009860: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+00009870: 672e 4c69 7465 7261 6c5b 226b 6222 2c20  g.Literal["kb", 
+00009880: 6222 6b62 225d 2920 2d3e 204e 6f6e 653a  b"kb"]) -> None:
+00009890: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f4c   .....global___L
+000098a0: 6973 7445 6e74 6974 6965 7347 726f 7570  istEntitiesGroup
+000098b0: 7352 6571 7565 7374 203d 204c 6973 7445  sRequest = ListE
+000098c0: 6e74 6974 6965 7347 726f 7570 7352 6571  ntitiesGroupsReq
+000098d0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
+000098e0: 6e61 6c0a 636c 6173 7320 4c69 7374 456e  nal.class ListEn
+000098f0: 7469 7469 6573 4772 6f75 7073 5265 7370  titiesGroupsResp
+00009900: 6f6e 7365 2867 6f6f 676c 652e 7072 6f74  onse(google.prot
+00009910: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+00009920: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
+00009930: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+00009940: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+00009950: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+00009960: 2020 636c 6173 7320 5f53 7461 7475 733a    class _Status:
+00009970: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
+00009980: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
+00009990: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
+000099a0: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
+000099b0: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
+000099c0: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
+000099d0: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
+000099e0: 650a 0a20 2020 2063 6c61 7373 205f 5374  e..    class _St
+000099f0: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
+00009a00: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
+00009a10: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
+00009a20: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
+00009a30: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
+00009a40: 4c69 7374 456e 7469 7469 6573 4772 6f75  ListEntitiesGrou
+00009a50: 7073 5265 7370 6f6e 7365 2e5f 5374 6174  psResponse._Stat
+00009a60: 7573 2e56 616c 7565 5479 7065 5d2c 2062  us.ValueType], b
+00009a70: 7569 6c74 696e 732e 7479 7065 293a 0a20  uiltins.type):. 
+00009a80: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
+00009a90: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
+00009aa0: 7566 2e64 6573 6372 6970 746f 722e 456e  uf.descriptor.En
+00009ab0: 756d 4465 7363 7269 7074 6f72 0a20 2020  umDescriptor.   
+00009ac0: 2020 2020 204f 4b3a 204c 6973 7445 6e74       OK: ListEnt
+00009ad0: 6974 6965 7347 726f 7570 7352 6573 706f  itiesGroupsRespo
+00009ae0: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+00009af0: 6554 7970 6520 2023 2030 0a20 2020 2020  eType  # 0.     
+00009b00: 2020 204e 4f54 464f 554e 443a 204c 6973     NOTFOUND: Lis
+00009b10: 7445 6e74 6974 6965 7347 726f 7570 7352  tEntitiesGroupsR
+00009b20: 6573 706f 6e73 652e 5f53 7461 7475 732e  esponse._Status.
+00009b30: 5661 6c75 6554 7970 6520 2023 2031 0a20  ValueType  # 1. 
+00009b40: 2020 2020 2020 2045 5252 4f52 3a20 4c69         ERROR: Li
+00009b50: 7374 456e 7469 7469 6573 4772 6f75 7073  stEntitiesGroups
+00009b60: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
+00009b70: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+00009b80: 0a20 2020 2063 6c61 7373 2053 7461 7475  .    class Statu
+00009b90: 7328 5f53 7461 7475 732c 206d 6574 6163  s(_Status, metac
+00009ba0: 6c61 7373 3d5f 5374 6174 7573 456e 756d  lass=_StatusEnum
+00009bb0: 5479 7065 5772 6170 7065 7229 3a20 2e2e  TypeWrapper): ..
+00009bc0: 2e0a 2020 2020 4f4b 3a20 4c69 7374 456e  ..    OK: ListEn
+00009bd0: 7469 7469 6573 4772 6f75 7073 5265 7370  titiesGroupsResp
+00009be0: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
+00009bf0: 6554 7970 6520 2023 2030 0a20 2020 204e  eType  # 0.    N
+00009c00: 4f54 464f 554e 443a 204c 6973 7445 6e74  OTFOUND: ListEnt
+00009c10: 6974 6965 7347 726f 7570 7352 6573 706f  itiesGroupsRespo
+00009c20: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+00009c30: 5479 7065 2020 2320 310a 2020 2020 4552  Type  # 1.    ER
+00009c40: 524f 523a 204c 6973 7445 6e74 6974 6965  ROR: ListEntitie
+00009c50: 7347 726f 7570 7352 6573 706f 6e73 652e  sGroupsResponse.
+00009c60: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+00009c70: 2020 2320 320a 0a20 2020 2040 7479 7069    # 2..    @typi
+00009c80: 6e67 2e66 696e 616c 0a20 2020 2063 6c61  ng.final.    cla
+00009c90: 7373 2047 726f 7570 7345 6e74 7279 2867  ss GroupsEntry(g
+00009ca0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
+00009cb0: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
+00009cc0: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
+00009cd0: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+00009ce0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+00009cf0: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+00009d00: 2020 2020 4b45 595f 4649 454c 445f 4e55      KEY_FIELD_NU
+00009d10: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+00009d20: 6e74 0a20 2020 2020 2020 2056 414c 5545  nt.        VALUE
+00009d30: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00009d40: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+00009d50: 2020 2020 6b65 793a 2062 7569 6c74 696e      key: builtin
+00009d60: 732e 7374 720a 2020 2020 2020 2020 4070  s.str.        @p
+00009d70: 726f 7065 7274 790a 2020 2020 2020 2020  roperty.        
+00009d80: 6465 6620 7661 6c75 6528 7365 6c66 2920  def value(self) 
+00009d90: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
+00009da0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+00009db0: 7062 322e 456e 7469 7469 6573 4772 6f75  pb2.EntitiesGrou
+00009dc0: 7053 756d 6d61 7279 3a20 2e2e 2e0a 2020  pSummary: ....  
+00009dd0: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
+00009de0: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
+00009df0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00009e00: 2020 2a2c 0a20 2020 2020 2020 2020 2020    *,.           
+00009e10: 206b 6579 3a20 6275 696c 7469 6e73 2e73   key: builtins.s
+00009e20: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
+00009e30: 2020 2020 2020 7661 6c75 653a 206e 7563        value: nuc
+00009e40: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+00009e50: 776c 6564 6765 626f 785f 7062 322e 456e  wledgebox_pb2.En
+00009e60: 7469 7469 6573 4772 6f75 7053 756d 6d61  titiesGroupSumma
+00009e70: 7279 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ry | None = ...,
+00009e80: 0a20 2020 2020 2020 2029 202d 3e20 4e6f  .        ) -> No
+00009e90: 6e65 3a20 2e2e 2e0a 2020 2020 2020 2020  ne: ....        
+00009ea0: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+00009eb0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+00009ec0: 7970 696e 672e 4c69 7465 7261 6c5b 2276  yping.Literal["v
+00009ed0: 616c 7565 222c 2062 2276 616c 7565 225d  alue", b"value"]
+00009ee0: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
+00009ef0: 6f6c 3a20 2e2e 2e0a 2020 2020 2020 2020  ol: ....        
+00009f00: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+00009f10: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+00009f20: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+00009f30: 226b 6579 222c 2062 226b 6579 222c 2022  "key", b"key", "
+00009f40: 7661 6c75 6522 2c20 6222 7661 6c75 6522  value", b"value"
+00009f50: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+00009f60: 0a20 2020 2047 524f 5550 535f 4649 454c  .    GROUPS_FIEL
+00009f70: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00009f80: 6e73 2e69 6e74 0a20 2020 2053 5441 5455  ns.int.    STATU
+00009f90: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
+00009fa0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00009fb0: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
+00009fc0: 5f5f 4c69 7374 456e 7469 7469 6573 4772  __ListEntitiesGr
+00009fd0: 6f75 7073 5265 7370 6f6e 7365 2e53 7461  oupsResponse.Sta
+00009fe0: 7475 732e 5661 6c75 6554 7970 650a 2020  tus.ValueType.  
+00009ff0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000a000: 6465 6620 6772 6f75 7073 2873 656c 6629  def groups(self)
+0000a010: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
+0000a020: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
+0000a030: 7461 696e 6572 732e 4d65 7373 6167 654d  tainers.MessageM
+0000a040: 6170 5b62 7569 6c74 696e 732e 7374 722c  ap[builtins.str,
+0000a050: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+0000a060: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+0000a070: 322e 456e 7469 7469 6573 4772 6f75 7053  2.EntitiesGroupS
+0000a080: 756d 6d61 7279 5d3a 202e 2e2e 0a20 2020  ummary]: ....   
+0000a090: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0000a0a0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000a0b0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+0000a0c0: 6772 6f75 7073 3a20 636f 6c6c 6563 7469  groups: collecti
+0000a0d0: 6f6e 732e 6162 632e 4d61 7070 696e 675b  ons.abc.Mapping[
+0000a0e0: 6275 696c 7469 6e73 2e73 7472 2c20 6e75  builtins.str, nu
+0000a0f0: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+0000a100: 6f77 6c65 6467 6562 6f78 5f70 6232 2e45  owledgebox_pb2.E
+0000a110: 6e74 6974 6965 7347 726f 7570 5375 6d6d  ntitiesGroupSumm
+0000a120: 6172 795d 207c 204e 6f6e 6520 3d20 2e2e  ary] | None = ..
+0000a130: 2e2c 0a20 2020 2020 2020 2073 7461 7475  .,.        statu
+0000a140: 733a 2067 6c6f 6261 6c5f 5f5f 4c69 7374  s: global___List
+0000a150: 456e 7469 7469 6573 4772 6f75 7073 5265  EntitiesGroupsRe
+0000a160: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
+0000a170: 6c75 6554 7970 6520 3d20 2e2e 2e2c 0a20  lueType = ...,. 
+0000a180: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+0000a190: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+0000a1a0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+0000a1b0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+0000a1c0: 7465 7261 6c5b 2267 726f 7570 7322 2c20  teral["groups", 
+0000a1d0: 6222 6772 6f75 7073 222c 2022 7374 6174  b"groups", "stat
+0000a1e0: 7573 222c 2062 2273 7461 7475 7322 5d29  us", b"status"])
+0000a1f0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
+0000a200: 6c6f 6261 6c5f 5f5f 4c69 7374 456e 7469  lobal___ListEnti
+0000a210: 7469 6573 4772 6f75 7073 5265 7370 6f6e  tiesGroupsRespon
+0000a220: 7365 203d 204c 6973 7445 6e74 6974 6965  se = ListEntitie
+0000a230: 7347 726f 7570 7352 6573 706f 6e73 650a  sGroupsResponse.
+0000a240: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
+0000a250: 6c61 7373 2047 6574 456e 7469 7469 6573  lass GetEntities
+0000a260: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
+0000a270: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+0000a280: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+0000a290: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+0000a2a0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+0000a2b0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+0000a2c0: 0a20 2020 204b 425f 4649 454c 445f 4e55  .    KB_FIELD_NU
+0000a2d0: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
+0000a2e0: 6e74 0a20 2020 2040 7072 6f70 6572 7479  nt.    @property
+0000a2f0: 0a20 2020 2064 6566 206b 6228 7365 6c66  .    def kb(self
+0000a300: 2920 2d3e 206e 7563 6c69 6164 625f 7072  ) -> nucliadb_pr
+0000a310: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
+0000a320: 785f 7062 322e 4b6e 6f77 6c65 6467 6542  x_pb2.KnowledgeB
+0000a330: 6f78 4944 3a20 2e2e 2e0a 2020 2020 6465  oxID: ....    de
+0000a340: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0000a350: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000a360: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
+0000a370: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+0000a380: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+0000a390: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
+0000a3a0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+0000a3b0: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+0000a3c0: 2e0a 2020 2020 6465 6620 4861 7346 6965  ..    def HasFie
+0000a3d0: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+0000a3e0: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+0000a3f0: 7261 6c5b 226b 6222 2c20 6222 6b62 225d  ral["kb", b"kb"]
+0000a400: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
+0000a410: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
+0000a420: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
+0000a430: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+0000a440: 696e 672e 4c69 7465 7261 6c5b 226b 6222  ing.Literal["kb"
+0000a450: 2c20 6222 6b62 225d 2920 2d3e 204e 6f6e  , b"kb"]) -> Non
+0000a460: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+0000a470: 5f47 6574 456e 7469 7469 6573 5265 7175  _GetEntitiesRequ
+0000a480: 6573 7420 3d20 4765 7445 6e74 6974 6965  est = GetEntitie
+0000a490: 7352 6571 7565 7374 0a0a 4074 7970 696e  sRequest..@typin
+0000a4a0: 672e 6669 6e61 6c0a 636c 6173 7320 4765  g.final.class Ge
+0000a4b0: 7445 6e74 6974 6965 7352 6573 706f 6e73  tEntitiesRespons
+0000a4c0: 6528 676f 6f67 6c65 2e70 726f 746f 6275  e(google.protobu
+0000a4d0: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+0000a4e0: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+0000a4f0: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000a500: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+0000a510: 6573 6372 6970 746f 720a 0a20 2020 2063  escriptor..    c
+0000a520: 6c61 7373 205f 5374 6174 7573 3a0a 2020  lass _Status:.  
+0000a530: 2020 2020 2020 5661 6c75 6554 7970 6520        ValueType 
+0000a540: 3d20 7479 7069 6e67 2e4e 6577 5479 7065  = typing.NewType
+0000a550: 2822 5661 6c75 6554 7970 6522 2c20 6275  ("ValueType", bu
+0000a560: 696c 7469 6e73 2e69 6e74 290a 2020 2020  iltins.int).    
+0000a570: 2020 2020 563a 2074 7970 696e 675f 6578      V: typing_ex
+0000a580: 7465 6e73 696f 6e73 2e54 7970 6541 6c69  tensions.TypeAli
+0000a590: 6173 203d 2056 616c 7565 5479 7065 0a0a  as = ValueType..
+0000a5a0: 2020 2020 636c 6173 7320 5f53 7461 7475      class _Statu
+0000a5b0: 7345 6e75 6d54 7970 6557 7261 7070 6572  sEnumTypeWrapper
+0000a5c0: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
+0000a5d0: 2e69 6e74 6572 6e61 6c2e 656e 756d 5f74  .internal.enum_t
+0000a5e0: 7970 655f 7772 6170 7065 722e 5f45 6e75  ype_wrapper._Enu
+0000a5f0: 6d54 7970 6557 7261 7070 6572 5b47 6574  mTypeWrapper[Get
+0000a600: 456e 7469 7469 6573 5265 7370 6f6e 7365  EntitiesResponse
+0000a610: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
+0000a620: 7065 5d2c 2062 7569 6c74 696e 732e 7479  pe], builtins.ty
+0000a630: 7065 293a 0a20 2020 2020 2020 2044 4553  pe):.        DES
+0000a640: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
+0000a650: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
+0000a660: 746f 722e 456e 756d 4465 7363 7269 7074  tor.EnumDescript
+0000a670: 6f72 0a20 2020 2020 2020 204f 4b3a 2047  or.        OK: G
+0000a680: 6574 456e 7469 7469 6573 5265 7370 6f6e  etEntitiesRespon
+0000a690: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
+0000a6a0: 5479 7065 2020 2320 300a 2020 2020 2020  Type  # 0.      
+0000a6b0: 2020 4e4f 5446 4f55 4e44 3a20 4765 7445    NOTFOUND: GetE
+0000a6c0: 6e74 6974 6965 7352 6573 706f 6e73 652e  ntitiesResponse.
+0000a6d0: 5f53 7461 7475 732e 5661 6c75 6554 7970  _Status.ValueTyp
+0000a6e0: 6520 2023 2031 0a20 2020 2020 2020 2045  e  # 1.        E
+0000a6f0: 5252 4f52 3a20 4765 7445 6e74 6974 6965  RROR: GetEntitie
+0000a700: 7352 6573 706f 6e73 652e 5f53 7461 7475  sResponse._Statu
+0000a710: 732e 5661 6c75 6554 7970 6520 2023 2032  s.ValueType  # 2
+0000a720: 0a0a 2020 2020 636c 6173 7320 5374 6174  ..    class Stat
+0000a730: 7573 285f 5374 6174 7573 2c20 6d65 7461  us(_Status, meta
+0000a740: 636c 6173 733d 5f53 7461 7475 7345 6e75  class=_StatusEnu
+0000a750: 6d54 7970 6557 7261 7070 6572 293a 202e  mTypeWrapper): .
+0000a760: 2e2e 0a20 2020 204f 4b3a 2047 6574 456e  ...    OK: GetEn
+0000a770: 7469 7469 6573 5265 7370 6f6e 7365 2e53  titiesResponse.S
+0000a780: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
+0000a790: 2023 2030 0a20 2020 204e 4f54 464f 554e   # 0.    NOTFOUN
+0000a7a0: 443a 2047 6574 456e 7469 7469 6573 5265  D: GetEntitiesRe
+0000a7b0: 7370 6f6e 7365 2e53 7461 7475 732e 5661  sponse.Status.Va
+0000a7c0: 6c75 6554 7970 6520 2023 2031 0a20 2020  lueType  # 1.   
+0000a7d0: 2045 5252 4f52 3a20 4765 7445 6e74 6974   ERROR: GetEntit
+0000a7e0: 6965 7352 6573 706f 6e73 652e 5374 6174  iesResponse.Stat
+0000a7f0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000a800: 320a 0a20 2020 2040 7479 7069 6e67 2e66  2..    @typing.f
+0000a810: 696e 616c 0a20 2020 2063 6c61 7373 2047  inal.    class G
+0000a820: 726f 7570 7345 6e74 7279 2867 6f6f 676c  roupsEntry(googl
+0000a830: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+0000a840: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+0000a850: 2020 2020 2044 4553 4352 4950 544f 523a       DESCRIPTOR:
+0000a860: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+0000a870: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
+0000a880: 7269 7074 6f72 0a0a 2020 2020 2020 2020  riptor..        
+0000a890: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
+0000a8a0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+0000a8b0: 2020 2020 2020 2056 414c 5545 5f46 4945         VALUE_FIE
+0000a8c0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+0000a8d0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
+0000a8e0: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+0000a8f0: 720a 2020 2020 2020 2020 4070 726f 7065  r.        @prope
+0000a900: 7274 790a 2020 2020 2020 2020 6465 6620  rty.        def 
+0000a910: 7661 6c75 6528 7365 6c66 2920 2d3e 206e  value(self) -> n
+0000a920: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
+0000a930: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
+0000a940: 456e 7469 7469 6573 4772 6f75 703a 202e  EntitiesGroup: .
+0000a950: 2e2e 0a20 2020 2020 2020 2064 6566 205f  ...        def _
+0000a960: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000a970: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000a980: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+0000a990: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
+0000a9a0: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+0000a9b0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0000a9c0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+0000a9d0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+0000a9e0: 6232 2e45 6e74 6974 6965 7347 726f 7570  b2.EntitiesGroup
+0000a9f0: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+0000aa00: 2020 2020 2020 2029 202d 3e20 4e6f 6e65         ) -> None
+0000aa10: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
+0000aa20: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
+0000aa30: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+0000aa40: 696e 672e 4c69 7465 7261 6c5b 2276 616c  ing.Literal["val
+0000aa50: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
+0000aa60: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
+0000aa70: 3a20 2e2e 2e0a 2020 2020 2020 2020 6465  : ....        de
+0000aa80: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
+0000aa90: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+0000aaa0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
+0000aab0: 6579 222c 2062 226b 6579 222c 2022 7661  ey", b"key", "va
+0000aac0: 6c75 6522 2c20 6222 7661 6c75 6522 5d29  lue", b"value"])
+0000aad0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20   -> None: ..... 
+0000aae0: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
+0000aaf0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000ab00: 0a20 2020 2047 524f 5550 535f 4649 454c  .    GROUPS_FIEL
+0000ab10: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+0000ab20: 6e73 2e69 6e74 0a20 2020 2053 5441 5455  ns.int.    STATU
+0000ab30: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
+0000ab40: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000ab50: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
+0000ab60: 5f5f 4765 7445 6e74 6974 6965 7352 6573  __GetEntitiesRes
+0000ab70: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+0000ab80: 7565 5479 7065 0a20 2020 2040 7072 6f70  ueType.    @prop
+0000ab90: 6572 7479 0a20 2020 2064 6566 206b 6228  erty.    def kb(
+0000aba0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+0000abb0: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+0000abc0: 6765 626f 785f 7062 322e 4b6e 6f77 6c65  gebox_pb2.Knowle
+0000abd0: 6467 6542 6f78 4944 3a20 2e2e 2e0a 2020  dgeBoxID: ....  
+0000abe0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000abf0: 6465 6620 6772 6f75 7073 2873 656c 6629  def groups(self)
+0000ac00: 202d 3e20 676f 6f67 6c65 2e70 726f 746f   -> google.proto
+0000ac10: 6275 662e 696e 7465 726e 616c 2e63 6f6e  buf.internal.con
+0000ac20: 7461 696e 6572 732e 4d65 7373 6167 654d  tainers.MessageM
+0000ac30: 6170 5b62 7569 6c74 696e 732e 7374 722c  ap[builtins.str,
+0000ac40: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+0000ac50: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+0000ac60: 322e 456e 7469 7469 6573 4772 6f75 705d  2.EntitiesGroup]
+0000ac70: 3a20 2e2e 2e0a 2020 2020 6465 6620 5f5f  : ....    def __
+0000ac80: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0000ac90: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
+0000aca0: 0a20 2020 2020 2020 206b 623a 206e 7563  .        kb: nuc
+0000acb0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+0000acc0: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
+0000acd0: 6f77 6c65 6467 6542 6f78 4944 207c 204e  owledgeBoxID | N
+0000ace0: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
+0000acf0: 2020 2067 726f 7570 733a 2063 6f6c 6c65     groups: colle
+0000ad00: 6374 696f 6e73 2e61 6263 2e4d 6170 7069  ctions.abc.Mappi
+0000ad10: 6e67 5b62 7569 6c74 696e 732e 7374 722c  ng[builtins.str,
+0000ad20: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+0000ad30: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
+0000ad40: 322e 456e 7469 7469 6573 4772 6f75 705d  2.EntitiesGroup]
+0000ad50: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+0000ad60: 2020 2020 2020 2073 7461 7475 733a 2067         status: g
+0000ad70: 6c6f 6261 6c5f 5f5f 4765 7445 6e74 6974  lobal___GetEntit
+0000ad80: 6965 7352 6573 706f 6e73 652e 5374 6174  iesResponse.Stat
+0000ad90: 7573 2e56 616c 7565 5479 7065 203d 202e  us.ValueType = .
+0000ada0: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
+0000adb0: 653a 202e 2e2e 0a20 2020 2064 6566 2048  e: ....    def H
+0000adc0: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
+0000add0: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+0000ade0: 2e4c 6974 6572 616c 5b22 6b62 222c 2062  .Literal["kb", b
+0000adf0: 226b 6222 5d29 202d 3e20 6275 696c 7469  "kb"]) -> builti
+0000ae00: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
+0000ae10: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
+0000ae20: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+0000ae30: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+0000ae40: 5b22 6772 6f75 7073 222c 2062 2267 726f  ["groups", b"gro
+0000ae50: 7570 7322 2c20 226b 6222 2c20 6222 6b62  ups", "kb", b"kb
+0000ae60: 222c 2022 7374 6174 7573 222c 2062 2273  ", "status", b"s
+0000ae70: 7461 7475 7322 5d29 202d 3e20 4e6f 6e65  tatus"]) -> None
+0000ae80: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
+0000ae90: 4765 7445 6e74 6974 6965 7352 6573 706f  GetEntitiesRespo
+0000aea0: 6e73 6520 3d20 4765 7445 6e74 6974 6965  nse = GetEntitie
+0000aeb0: 7352 6573 706f 6e73 650a 0a40 7479 7069  sResponse..@typi
+0000aec0: 6e67 2e66 696e 616c 0a63 6c61 7373 2044  ng.final.class D
+0000aed0: 656c 456e 7469 7469 6573 5265 7175 6573  elEntitiesReques
+0000aee0: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
+0000aef0: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
+0000af00: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
+0000af10: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000af20: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+0000af30: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
+0000af40: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
+0000af50: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000af60: 2047 524f 5550 5f46 4945 4c44 5f4e 554d   GROUP_FIELD_NUM
+0000af70: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+0000af80: 740a 2020 2020 6772 6f75 703a 2062 7569  t.    group: bui
+0000af90: 6c74 696e 732e 7374 720a 2020 2020 4070  ltins.str.    @p
+0000afa0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000afb0: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
+0000afc0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+0000afd0: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
+0000afe0: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
+0000aff0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000b000: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0000b010: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+0000b020: 2020 2020 6b62 3a20 6e75 636c 6961 6462      kb: nucliadb
+0000b030: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
+0000b040: 6562 6f78 5f70 6232 2e4b 6e6f 776c 6564  ebox_pb2.Knowled
+0000b050: 6765 426f 7849 4420 7c20 4e6f 6e65 203d  geBoxID | None =
+0000b060: 202e 2e2e 2c0a 2020 2020 2020 2020 6772   ...,.        gr
+0000b070: 6f75 703a 2062 7569 6c74 696e 732e 7374  oup: builtins.st
+0000b080: 7220 3d20 2e2e 2e2c 0a20 2020 2029 202d  r = ...,.    ) -
+0000b090: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
+0000b0a0: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
+0000b0b0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+0000b0c0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
+0000b0d0: 6222 2c20 6222 6b62 225d 2920 2d3e 2062  b", b"kb"]) -> b
+0000b0e0: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
+0000b0f0: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+0000b100: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+0000b110: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+0000b120: 7465 7261 6c5b 2267 726f 7570 222c 2062  teral["group", b
+0000b130: 2267 726f 7570 222c 2022 6b62 222c 2062  "group", "kb", b
+0000b140: 226b 6222 5d29 202d 3e20 4e6f 6e65 3a20  "kb"]) -> None: 
+0000b150: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4465  .....global___De
+0000b160: 6c45 6e74 6974 6965 7352 6571 7565 7374  lEntitiesRequest
+0000b170: 203d 2044 656c 456e 7469 7469 6573 5265   = DelEntitiesRe
+0000b180: 7175 6573 740a 0a40 7479 7069 6e67 2e66  quest..@typing.f
+0000b190: 696e 616c 0a63 6c61 7373 204d 6572 6765  inal.class Merge
+0000b1a0: 456e 7469 7469 6573 5265 7175 6573 7428  EntitiesRequest(
+0000b1b0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+0000b1c0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+0000b1d0: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
+0000b1e0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+0000b1f0: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
+0000b200: 6372 6970 746f 720a 0a20 2020 2040 7479  criptor..    @ty
+0000b210: 7069 6e67 2e66 696e 616c 0a20 2020 2063  ping.final.    c
+0000b220: 6c61 7373 2045 6e74 6974 7949 4428 676f  lass EntityID(go
+0000b230: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+0000b240: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+0000b250: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
+0000b260: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
+0000b270: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
+0000b280: 6573 6372 6970 746f 720a 0a20 2020 2020  escriptor..     
+0000b290: 2020 2047 524f 5550 5f46 4945 4c44 5f4e     GROUP_FIELD_N
+0000b2a0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+0000b2b0: 696e 740a 2020 2020 2020 2020 454e 5449  int.        ENTI
+0000b2c0: 5459 5f46 4945 4c44 5f4e 554d 4245 523a  TY_FIELD_NUMBER:
+0000b2d0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000b2e0: 2020 2020 2020 6772 6f75 703a 2062 7569        group: bui
+0000b2f0: 6c74 696e 732e 7374 720a 2020 2020 2020  ltins.str.      
+0000b300: 2020 656e 7469 7479 3a20 6275 696c 7469    entity: builti
+0000b310: 6e73 2e73 7472 0a20 2020 2020 2020 2064  ns.str.        d
+0000b320: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0000b330: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+0000b340: 2020 2020 2020 2020 2020 202a 2c0a 2020             *,.  
+0000b350: 2020 2020 2020 2020 2020 6772 6f75 703a            group:
+0000b360: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
+0000b370: 2e2e 2e2c 0a20 2020 2020 2020 2020 2020  ...,.           
+0000b380: 2065 6e74 6974 793a 2062 7569 6c74 696e   entity: builtin
+0000b390: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+0000b3a0: 2020 2020 2029 202d 3e20 4e6f 6e65 3a20       ) -> None: 
+0000b3b0: 2e2e 2e0a 2020 2020 2020 2020 6465 6620  ....        def 
+0000b3c0: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
+0000b3d0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+0000b3e0: 696e 672e 4c69 7465 7261 6c5b 2265 6e74  ing.Literal["ent
+0000b3f0: 6974 7922 2c20 6222 656e 7469 7479 222c  ity", b"entity",
+0000b400: 2022 6772 6f75 7022 2c20 6222 6772 6f75   "group", b"grou
+0000b410: 7022 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  p"]) -> None: ..
+0000b420: 2e0a 0a20 2020 204b 425f 4649 454c 445f  ...    KB_FIELD_
+0000b430: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000b440: 2e69 6e74 0a20 2020 2046 524f 4d5f 4649  .int.    FROM_FI
+0000b450: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+0000b460: 7469 6e73 2e69 6e74 0a20 2020 2054 4f5f  tins.int.    TO_
+0000b470: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+0000b480: 696c 7469 6e73 2e69 6e74 0a20 2020 2040  iltins.int.    @
+0000b490: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0000b4a0: 206b 6228 7365 6c66 2920 2d3e 206e 7563   kb(self) -> nuc
+0000b4b0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+0000b4c0: 776c 6564 6765 626f 785f 7062 322e 4b6e  wledgebox_pb2.Kn
+0000b4d0: 6f77 6c65 6467 6542 6f78 4944 3a20 2e2e  owledgeBoxID: ..
+0000b4e0: 2e0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000b4f0: 2020 2020 6465 6620 746f 2873 656c 6629      def to(self)
+0000b500: 202d 3e20 676c 6f62 616c 5f5f 5f4d 6572   -> global___Mer
+0000b510: 6765 456e 7469 7469 6573 5265 7175 6573  geEntitiesReques
+0000b520: 742e 456e 7469 7479 4944 3a20 2e2e 2e0a  t.EntityID: ....
+0000b530: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000b540: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000b550: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0000b560: 2020 206b 623a 206e 7563 6c69 6164 625f     kb: nucliadb_
+0000b570: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+0000b580: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
+0000b590: 6542 6f78 4944 207c 204e 6f6e 6520 3d20  eBoxID | None = 
+0000b5a0: 2e2e 2e2c 0a20 2020 2020 2020 2074 6f3a  ...,.        to:
+0000b5b0: 2067 6c6f 6261 6c5f 5f5f 4d65 7267 6545   global___MergeE
+0000b5c0: 6e74 6974 6965 7352 6571 7565 7374 2e45  ntitiesRequest.E
+0000b5d0: 6e74 6974 7949 4420 7c20 4e6f 6e65 203d  ntityID | None =
+0000b5e0: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+0000b5f0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+0000b600: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
+0000b610: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+0000b620: 6e67 2e4c 6974 6572 616c 5b22 6672 6f6d  ng.Literal["from
+0000b630: 222c 2062 2266 726f 6d22 2c20 226b 6222  ", b"from", "kb"
+0000b640: 2c20 6222 6b62 222c 2022 746f 222c 2062  , b"kb", "to", b
+0000b650: 2274 6f22 5d29 202d 3e20 6275 696c 7469  "to"]) -> builti
+0000b660: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
+0000b670: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
+0000b680: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+0000b690: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+0000b6a0: 5b22 6672 6f6d 222c 2062 2266 726f 6d22  ["from", b"from"
+0000b6b0: 2c20 226b 6222 2c20 6222 6b62 222c 2022  , "kb", b"kb", "
+0000b6c0: 746f 222c 2062 2274 6f22 5d29 202d 3e20  to", b"to"]) -> 
+0000b6d0: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
+0000b6e0: 6c5f 5f5f 4d65 7267 6545 6e74 6974 6965  l___MergeEntitie
+0000b6f0: 7352 6571 7565 7374 203d 204d 6572 6765  sRequest = Merge
+0000b700: 456e 7469 7469 6573 5265 7175 6573 740a  EntitiesRequest.
+0000b710: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
+0000b720: 6c61 7373 2047 6574 4c61 6265 6c73 5265  lass GetLabelsRe
+0000b730: 7370 6f6e 7365 2867 6f6f 676c 652e 7072  sponse(google.pr
+0000b740: 6f74 6f62 7566 2e6d 6573 7361 6765 2e4d  otobuf.message.M
+0000b750: 6573 7361 6765 293a 0a20 2020 2044 4553  essage):.    DES
+0000b760: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
+0000b770: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
+0000b780: 746f 722e 4465 7363 7269 7074 6f72 0a0a  tor.Descriptor..
+0000b790: 2020 2020 636c 6173 7320 5f53 7461 7475      class _Statu
+0000b7a0: 733a 0a20 2020 2020 2020 2056 616c 7565  s:.        Value
+0000b7b0: 5479 7065 203d 2074 7970 696e 672e 4e65  Type = typing.Ne
+0000b7c0: 7754 7970 6528 2256 616c 7565 5479 7065  wType("ValueType
+0000b7d0: 222c 2062 7569 6c74 696e 732e 696e 7429  ", builtins.int)
+0000b7e0: 0a20 2020 2020 2020 2056 3a20 7479 7069  .        V: typi
+0000b7f0: 6e67 5f65 7874 656e 7369 6f6e 732e 5479  ng_extensions.Ty
+0000b800: 7065 416c 6961 7320 3d20 5661 6c75 6554  peAlias = ValueT
+0000b810: 7970 650a 0a20 2020 2063 6c61 7373 205f  ype..    class _
+0000b820: 5374 6174 7573 456e 756d 5479 7065 5772  StatusEnumTypeWr
+0000b830: 6170 7065 7228 676f 6f67 6c65 2e70 726f  apper(google.pro
+0000b840: 746f 6275 662e 696e 7465 726e 616c 2e65  tobuf.internal.e
+0000b850: 6e75 6d5f 7479 7065 5f77 7261 7070 6572  num_type_wrapper
+0000b860: 2e5f 456e 756d 5479 7065 5772 6170 7065  ._EnumTypeWrappe
+0000b870: 725b 4765 744c 6162 656c 7352 6573 706f  r[GetLabelsRespo
+0000b880: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+0000b890: 6554 7970 655d 2c20 6275 696c 7469 6e73  eType], builtins
+0000b8a0: 2e74 7970 6529 3a0a 2020 2020 2020 2020  .type):.        
+0000b8b0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+0000b8c0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+0000b8d0: 7269 7074 6f72 2e45 6e75 6d44 6573 6372  riptor.EnumDescr
+0000b8e0: 6970 746f 720a 2020 2020 2020 2020 4f4b  iptor.        OK
+0000b8f0: 3a20 4765 744c 6162 656c 7352 6573 706f  : GetLabelsRespo
+0000b900: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+0000b910: 6554 7970 6520 2023 2030 0a20 2020 2020  eType  # 0.     
+0000b920: 2020 204e 4f54 464f 554e 443a 2047 6574     NOTFOUND: Get
+0000b930: 4c61 6265 6c73 5265 7370 6f6e 7365 2e5f  LabelsResponse._
+0000b940: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+0000b950: 2020 2320 310a 0a20 2020 2063 6c61 7373    # 1..    class
+0000b960: 2053 7461 7475 7328 5f53 7461 7475 732c   Status(_Status,
+0000b970: 206d 6574 6163 6c61 7373 3d5f 5374 6174   metaclass=_Stat
+0000b980: 7573 456e 756d 5479 7065 5772 6170 7065  usEnumTypeWrappe
+0000b990: 7229 3a20 2e2e 2e0a 2020 2020 4f4b 3a20  r): ....    OK: 
+0000b9a0: 4765 744c 6162 656c 7352 6573 706f 6e73  GetLabelsRespons
+0000b9b0: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+0000b9c0: 7065 2020 2320 300a 2020 2020 4e4f 5446  pe  # 0.    NOTF
+0000b9d0: 4f55 4e44 3a20 4765 744c 6162 656c 7352  OUND: GetLabelsR
+0000b9e0: 6573 706f 6e73 652e 5374 6174 7573 2e56  esponse.Status.V
+0000b9f0: 616c 7565 5479 7065 2020 2320 310a 0a20  alueType  # 1.. 
+0000ba00: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
 0000ba10: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-0000ba20: 0a20 2020 2053 5441 5455 535f 4649 454c  .    STATUS_FIEL
+0000ba20: 0a20 2020 204c 4142 454c 535f 4649 454c  .    LABELS_FIEL
 0000ba30: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000ba40: 6e73 2e69 6e74 0a20 2020 2073 7461 7475  ns.int.    statu
-0000ba50: 733a 2067 6c6f 6261 6c5f 5f5f 4765 7445  s: global___GetE
-0000ba60: 6e74 6974 6965 7352 6573 706f 6e73 652e  ntitiesResponse.
-0000ba70: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000ba80: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000ba90: 2020 2064 6566 206b 6228 7365 6c66 2920     def kb(self) 
-0000baa0: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
-0000bab0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-0000bac0: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
-0000bad0: 4944 3a20 2e2e 2e0a 2020 2020 4070 726f  ID: ....    @pro
-0000bae0: 7065 7274 790a 2020 2020 6465 6620 6772  perty.    def gr
-0000baf0: 6f75 7073 2873 656c 6629 202d 3e20 676f  oups(self) -> go
-0000bb00: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
-0000bb10: 7465 726e 616c 2e63 6f6e 7461 696e 6572  ternal.container
-0000bb20: 732e 4d65 7373 6167 654d 6170 5b62 7569  s.MessageMap[bui
-0000bb30: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
-0000bb40: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-0000bb50: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
-0000bb60: 7469 6573 4772 6f75 705d 3a20 2e2e 2e0a  tiesGroup]: ....
-0000bb70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000bb80: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000bb90: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-0000bba0: 2020 206b 623a 206e 7563 6c69 6164 625f     kb: nucliadb_
-0000bbb0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-0000bbc0: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
-0000bbd0: 6542 6f78 4944 207c 204e 6f6e 6520 3d20  eBoxID | None = 
-0000bbe0: 2e2e 2e2c 0a20 2020 2020 2020 2067 726f  ...,.        gro
-0000bbf0: 7570 733a 2063 6f6c 6c65 6374 696f 6e73  ups: collections
-0000bc00: 2e61 6263 2e4d 6170 7069 6e67 5b62 7569  .abc.Mapping[bui
-0000bc10: 6c74 696e 732e 7374 722c 206e 7563 6c69  ltins.str, nucli
-0000bc20: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-0000bc30: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
-0000bc40: 7469 6573 4772 6f75 705d 207c 204e 6f6e  tiesGroup] | Non
-0000bc50: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-0000bc60: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
-0000bc70: 5f5f 4765 7445 6e74 6974 6965 7352 6573  __GetEntitiesRes
-0000bc80: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-0000bc90: 7565 5479 7065 203d 202e 2e2e 2c0a 2020  ueType = ...,.  
-0000bca0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
-0000bcb0: 0a20 2020 2064 6566 2048 6173 4669 656c  .    def HasFiel
-0000bcc0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-0000bcd0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-0000bce0: 616c 5b22 6b62 222c 2062 226b 6222 5d29  al["kb", b"kb"])
-0000bcf0: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
-0000bd00: 6c3a 202e 2e2e 0a20 2020 2064 6566 2043  l: ....    def C
-0000bd10: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
-0000bd20: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-0000bd30: 6e67 2e4c 6974 6572 616c 5b22 6772 6f75  ng.Literal["grou
-0000bd40: 7073 222c 2062 2267 726f 7570 7322 2c20  ps", b"groups", 
-0000bd50: 226b 6222 2c20 6222 6b62 222c 2022 7374  "kb", b"kb", "st
-0000bd60: 6174 7573 222c 2062 2273 7461 7475 7322  atus", b"status"
-0000bd70: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-0000bd80: 0a67 6c6f 6261 6c5f 5f5f 4765 7445 6e74  .global___GetEnt
-0000bd90: 6974 6965 7352 6573 706f 6e73 6520 3d20  itiesResponse = 
-0000bda0: 4765 7445 6e74 6974 6965 7352 6573 706f  GetEntitiesRespo
-0000bdb0: 6e73 650a 0a40 7479 7069 6e67 2e66 696e  nse..@typing.fin
-0000bdc0: 616c 0a63 6c61 7373 2044 656c 456e 7469  al.class DelEnti
-0000bdd0: 7469 6573 5265 7175 6573 7428 676f 6f67  tiesRequest(goog
-0000bde0: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-0000bdf0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-0000be00: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-0000be10: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-0000be20: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-0000be30: 746f 720a 0a20 2020 204b 425f 4649 454c  tor..    KB_FIEL
-0000be40: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000be50: 6e73 2e69 6e74 0a20 2020 2047 524f 5550  ns.int.    GROUP
-0000be60: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000be70: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000be80: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
-0000be90: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
-0000bea0: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
-0000beb0: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
-0000bec0: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
-0000bed0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
-0000bee0: 426f 7849 443a 202e 2e2e 0a20 2020 2064  BoxID: ....    d
-0000bef0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0000bf00: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000bf10: 2020 202a 2c0a 2020 2020 2020 2020 6b62     *,.        kb
-0000bf20: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-0000bf30: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-0000bf40: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
-0000bf50: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
-0000bf60: 2020 2020 2020 2020 6772 6f75 703a 2062          group: b
-0000bf70: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-0000bf80: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
-0000bf90: 3a20 2e2e 2e0a 2020 2020 6465 6620 4861  : ....    def Ha
-0000bfa0: 7346 6965 6c64 2873 656c 662c 2066 6965  sField(self, fie
-0000bfb0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-0000bfc0: 4c69 7465 7261 6c5b 226b 6222 2c20 6222  Literal["kb", b"
-0000bfd0: 6b62 225d 2920 2d3e 2062 7569 6c74 696e  kb"]) -> builtin
-0000bfe0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
-0000bff0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-0000c000: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000c010: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000c020: 2267 726f 7570 222c 2062 2267 726f 7570  "group", b"group
-0000c030: 222c 2022 6b62 222c 2062 226b 6222 5d29  ", "kb", b"kb"])
-0000c040: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
-0000c050: 6c6f 6261 6c5f 5f5f 4465 6c45 6e74 6974  lobal___DelEntit
-0000c060: 6965 7352 6571 7565 7374 203d 2044 656c  iesRequest = Del
-0000c070: 456e 7469 7469 6573 5265 7175 6573 740a  EntitiesRequest.
-0000c080: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
-0000c090: 6c61 7373 204d 6572 6765 456e 7469 7469  lass MergeEntiti
-0000c0a0: 6573 5265 7175 6573 7428 676f 6f67 6c65  esRequest(google
-0000c0b0: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
-0000c0c0: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
-0000c0d0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
-0000c0e0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
-0000c0f0: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
-0000c100: 720a 0a20 2020 2040 7479 7069 6e67 2e66  r..    @typing.f
-0000c110: 696e 616c 0a20 2020 2063 6c61 7373 2045  inal.    class E
-0000c120: 6e74 6974 7949 4428 676f 6f67 6c65 2e70  ntityID(google.p
-0000c130: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-0000c140: 4d65 7373 6167 6529 3a0a 2020 2020 2020  Message):.      
-0000c150: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-0000c160: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-0000c170: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-0000c180: 746f 720a 0a20 2020 2020 2020 2047 524f  tor..        GRO
-0000c190: 5550 5f46 4945 4c44 5f4e 554d 4245 523a  UP_FIELD_NUMBER:
-0000c1a0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-0000c1b0: 2020 2020 2020 454e 5449 5459 5f46 4945        ENTITY_FIE
-0000c1c0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-0000c1d0: 696e 732e 696e 740a 2020 2020 2020 2020  ins.int.        
-0000c1e0: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
-0000c1f0: 7374 720a 2020 2020 2020 2020 656e 7469  str.        enti
-0000c200: 7479 3a20 6275 696c 7469 6e73 2e73 7472  ty: builtins.str
-0000c210: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
-0000c220: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
-0000c230: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000c240: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-0000c250: 2020 2020 6772 6f75 703a 2062 7569 6c74      group: built
-0000c260: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-0000c270: 2020 2020 2020 2020 2020 2065 6e74 6974             entit
-0000c280: 793a 2062 7569 6c74 696e 732e 7374 7220  y: builtins.str 
-0000c290: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2029  = ...,.        )
-0000c2a0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
-0000c2b0: 2020 2020 2020 6465 6620 436c 6561 7246        def ClearF
-0000c2c0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000c2d0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000c2e0: 7465 7261 6c5b 2265 6e74 6974 7922 2c20  teral["entity", 
-0000c2f0: 6222 656e 7469 7479 222c 2022 6772 6f75  b"entity", "grou
-0000c300: 7022 2c20 6222 6772 6f75 7022 5d29 202d  p", b"group"]) -
-0000c310: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20 2020  > None: .....   
-0000c320: 204b 425f 4649 454c 445f 4e55 4d42 4552   KB_FIELD_NUMBER
-0000c330: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-0000c340: 2020 2046 524f 4d5f 4649 454c 445f 4e55     FROM_FIELD_NU
-0000c350: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-0000c360: 6e74 0a20 2020 2054 4f5f 4649 454c 445f  nt.    TO_FIELD_
-0000c370: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-0000c380: 2e69 6e74 0a20 2020 2040 7072 6f70 6572  .int.    @proper
-0000c390: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
-0000c3a0: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
-0000c3b0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
-0000c3c0: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
-0000c3d0: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
-0000c3e0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000c3f0: 6620 746f 2873 656c 6629 202d 3e20 676c  f to(self) -> gl
-0000c400: 6f62 616c 5f5f 5f4d 6572 6765 456e 7469  obal___MergeEnti
-0000c410: 7469 6573 5265 7175 6573 742e 456e 7469  tiesRequest.Enti
-0000c420: 7479 4944 3a20 2e2e 2e0a 2020 2020 6465  tyID: ....    de
-0000c430: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0000c440: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000c450: 2020 2a2c 0a20 2020 2020 2020 206b 623a    *,.        kb:
-0000c460: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000c470: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000c480: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
-0000c490: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
-0000c4a0: 2020 2020 2020 2074 6f3a 2067 6c6f 6261         to: globa
-0000c4b0: 6c5f 5f5f 4d65 7267 6545 6e74 6974 6965  l___MergeEntitie
-0000c4c0: 7352 6571 7565 7374 2e45 6e74 6974 7949  sRequest.EntityI
-0000c4d0: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
-0000c4e0: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
-0000c4f0: 2e2e 0a20 2020 2064 6566 2048 6173 4669  ...    def HasFi
-0000c500: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
-0000c510: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
-0000c520: 6572 616c 5b22 6672 6f6d 222c 2062 2266  eral["from", b"f
-0000c530: 726f 6d22 2c20 226b 6222 2c20 6222 6b62  rom", "kb", b"kb
-0000c540: 222c 2022 746f 222c 2062 2274 6f22 5d29  ", "to", b"to"])
-0000c550: 202d 3e20 6275 696c 7469 6e73 2e62 6f6f   -> builtins.boo
-0000c560: 6c3a 202e 2e2e 0a20 2020 2064 6566 2043  l: ....    def C
-0000c570: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
-0000c580: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-0000c590: 6e67 2e4c 6974 6572 616c 5b22 6672 6f6d  ng.Literal["from
-0000c5a0: 222c 2062 2266 726f 6d22 2c20 226b 6222  ", b"from", "kb"
-0000c5b0: 2c20 6222 6b62 222c 2022 746f 222c 2062  , b"kb", "to", b
-0000c5c0: 2274 6f22 5d29 202d 3e20 4e6f 6e65 3a20  "to"]) -> None: 
-0000c5d0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4d65  .....global___Me
-0000c5e0: 7267 6545 6e74 6974 6965 7352 6571 7565  rgeEntitiesReque
-0000c5f0: 7374 203d 204d 6572 6765 456e 7469 7469  st = MergeEntiti
-0000c600: 6573 5265 7175 6573 740a 0a40 7479 7069  esRequest..@typi
-0000c610: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
-0000c620: 6574 4c61 6265 6c53 6574 5265 7175 6573  etLabelSetReques
-0000c630: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
-0000c640: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-0000c650: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-0000c660: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000c670: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000c680: 6573 6372 6970 746f 720a 0a20 2020 204b  escriptor..    K
-0000c690: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
-0000c6a0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-0000c6b0: 204c 4142 454c 5345 545f 4649 454c 445f   LABELSET_FIELD_
-0000c6c0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-0000c6d0: 2e69 6e74 0a20 2020 206c 6162 656c 7365  .int.    labelse
-0000c6e0: 743a 2062 7569 6c74 696e 732e 7374 720a  t: builtins.str.
-0000c6f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000c700: 2020 6465 6620 6b62 2873 656c 6629 202d    def kb(self) -
-0000c710: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
-0000c720: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-0000c730: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
-0000c740: 443a 202e 2e2e 0a20 2020 2064 6566 205f  D: ....    def _
-0000c750: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000c760: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-0000c770: 2c0a 2020 2020 2020 2020 6b62 3a20 6e75  ,.        kb: nu
-0000c780: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
-0000c790: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
-0000c7a0: 6e6f 776c 6564 6765 426f 7849 4420 7c20  nowledgeBoxID | 
-0000c7b0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-0000c7c0: 2020 2020 6c61 6265 6c73 6574 3a20 6275      labelset: bu
-0000c7d0: 696c 7469 6e73 2e73 7472 203d 202e 2e2e  iltins.str = ...
-0000c7e0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-0000c7f0: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
-0000c800: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-0000c810: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-0000c820: 6974 6572 616c 5b22 6b62 222c 2062 226b  iteral["kb", b"k
-0000c830: 6222 5d29 202d 3e20 6275 696c 7469 6e73  b"]) -> builtins
-0000c840: 2e62 6f6f 6c3a 202e 2e2e 0a20 2020 2064  .bool: ....    d
-0000c850: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
-0000c860: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
-0000c870: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
-0000c880: 6b62 222c 2062 226b 6222 2c20 226c 6162  kb", b"kb", "lab
-0000c890: 656c 7365 7422 2c20 6222 6c61 6265 6c73  elset", b"labels
-0000c8a0: 6574 225d 2920 2d3e 204e 6f6e 653a 202e  et"]) -> None: .
-0000c8b0: 2e2e 0a0a 676c 6f62 616c 5f5f 5f47 6574  ....global___Get
-0000c8c0: 4c61 6265 6c53 6574 5265 7175 6573 7420  LabelSetRequest 
-0000c8d0: 3d20 4765 744c 6162 656c 5365 7452 6571  = GetLabelSetReq
-0000c8e0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
-0000c8f0: 6e61 6c0a 636c 6173 7320 4765 744c 6162  nal.class GetLab
-0000c900: 656c 5365 7452 6573 706f 6e73 6528 676f  elSetResponse(go
-0000c910: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
-0000c920: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
-0000c930: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
-0000c940: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-0000c950: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
-0000c960: 6970 746f 720a 0a20 2020 2063 6c61 7373  iptor..    class
-0000c970: 205f 5374 6174 7573 3a0a 2020 2020 2020   _Status:.      
-0000c980: 2020 5661 6c75 6554 7970 6520 3d20 7479    ValueType = ty
-0000c990: 7069 6e67 2e4e 6577 5479 7065 2822 5661  ping.NewType("Va
-0000c9a0: 6c75 6554 7970 6522 2c20 6275 696c 7469  lueType", builti
-0000c9b0: 6e73 2e69 6e74 290a 2020 2020 2020 2020  ns.int).        
-0000c9c0: 563a 2074 7970 696e 675f 6578 7465 6e73  V: typing_extens
-0000c9d0: 696f 6e73 2e54 7970 6541 6c69 6173 203d  ions.TypeAlias =
-0000c9e0: 2056 616c 7565 5479 7065 0a0a 2020 2020   ValueType..    
-0000c9f0: 636c 6173 7320 5f53 7461 7475 7345 6e75  class _StatusEnu
-0000ca00: 6d54 7970 6557 7261 7070 6572 2867 6f6f  mTypeWrapper(goo
-0000ca10: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-0000ca20: 6572 6e61 6c2e 656e 756d 5f74 7970 655f  ernal.enum_type_
-0000ca30: 7772 6170 7065 722e 5f45 6e75 6d54 7970  wrapper._EnumTyp
-0000ca40: 6557 7261 7070 6572 5b47 6574 4c61 6265  eWrapper[GetLabe
-0000ca50: 6c53 6574 5265 7370 6f6e 7365 2e5f 5374  lSetResponse._St
-0000ca60: 6174 7573 2e56 616c 7565 5479 7065 5d2c  atus.ValueType],
-0000ca70: 2062 7569 6c74 696e 732e 7479 7065 293a   builtins.type):
-0000ca80: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
-0000ca90: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
-0000caa0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
-0000cab0: 456e 756d 4465 7363 7269 7074 6f72 0a20  EnumDescriptor. 
-0000cac0: 2020 2020 2020 204f 4b3a 2047 6574 4c61         OK: GetLa
-0000cad0: 6265 6c53 6574 5265 7370 6f6e 7365 2e5f  belSetResponse._
-0000cae0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000caf0: 2020 2320 300a 2020 2020 2020 2020 4e4f    # 0.        NO
-0000cb00: 5446 4f55 4e44 3a20 4765 744c 6162 656c  TFOUND: GetLabel
-0000cb10: 5365 7452 6573 706f 6e73 652e 5f53 7461  SetResponse._Sta
-0000cb20: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
-0000cb30: 2031 0a0a 2020 2020 636c 6173 7320 5374   1..    class St
-0000cb40: 6174 7573 285f 5374 6174 7573 2c20 6d65  atus(_Status, me
-0000cb50: 7461 636c 6173 733d 5f53 7461 7475 7345  taclass=_StatusE
-0000cb60: 6e75 6d54 7970 6557 7261 7070 6572 293a  numTypeWrapper):
-0000cb70: 202e 2e2e 0a20 2020 204f 4b3a 2047 6574   ....    OK: Get
-0000cb80: 4c61 6265 6c53 6574 5265 7370 6f6e 7365  LabelSetResponse
-0000cb90: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
-0000cba0: 6520 2023 2030 0a20 2020 204e 4f54 464f  e  # 0.    NOTFO
-0000cbb0: 554e 443a 2047 6574 4c61 6265 6c53 6574  UND: GetLabelSet
-0000cbc0: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
-0000cbd0: 5661 6c75 6554 7970 6520 2023 2031 0a0a  ValueType  # 1..
-0000cbe0: 2020 2020 4b42 5f46 4945 4c44 5f4e 554d      KB_FIELD_NUM
-0000cbf0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
-0000cc00: 740a 2020 2020 4c41 4245 4c53 4554 5f46  t.    LABELSET_F
-0000cc10: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-0000cc20: 6c74 696e 732e 696e 740a 2020 2020 5354  ltins.int.    ST
-0000cc30: 4154 5553 5f46 4945 4c44 5f4e 554d 4245  ATUS_FIELD_NUMBE
-0000cc40: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000cc50: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
-0000cc60: 616c 5f5f 5f47 6574 4c61 6265 6c53 6574  al___GetLabelSet
-0000cc70: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
-0000cc80: 5661 6c75 6554 7970 650a 2020 2020 4070  ValueType.    @p
-0000cc90: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000cca0: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
-0000ccb0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-0000ccc0: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
-0000ccd0: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
-0000cce0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000ccf0: 2020 2064 6566 206c 6162 656c 7365 7428     def labelset(
-0000cd00: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-0000cd10: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
-0000cd20: 6765 626f 785f 7062 322e 4c61 6265 6c53  gebox_pb2.LabelS
-0000cd30: 6574 3a20 2e2e 2e0a 2020 2020 6465 6620  et: ....    def 
-0000cd40: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0000cd50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000cd60: 2a2c 0a20 2020 2020 2020 206b 623a 206e  *,.        kb: n
-0000cd70: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-0000cd80: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-0000cd90: 4b6e 6f77 6c65 6467 6542 6f78 4944 207c  KnowledgeBoxID |
-0000cda0: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
-0000cdb0: 2020 2020 206c 6162 656c 7365 743a 206e       labelset: n
-0000cdc0: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-0000cdd0: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-0000cde0: 4c61 6265 6c53 6574 207c 204e 6f6e 6520  LabelSet | None 
-0000cdf0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2073  = ...,.        s
-0000ce00: 7461 7475 733a 2067 6c6f 6261 6c5f 5f5f  tatus: global___
-0000ce10: 4765 744c 6162 656c 5365 7452 6573 706f  GetLabelSetRespo
-0000ce20: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
-0000ce30: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
-0000ce40: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-0000ce50: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
-0000ce60: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-0000ce70: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-0000ce80: 5b22 6b62 222c 2062 226b 6222 2c20 226c  ["kb", b"kb", "l
-0000ce90: 6162 656c 7365 7422 2c20 6222 6c61 6265  abelset", b"labe
-0000cea0: 6c73 6574 225d 2920 2d3e 2062 7569 6c74  lset"]) -> built
-0000ceb0: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
-0000cec0: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
-0000ced0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
-0000cee0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
-0000cef0: 6c5b 226b 6222 2c20 6222 6b62 222c 2022  l["kb", b"kb", "
-0000cf00: 6c61 6265 6c73 6574 222c 2062 226c 6162  labelset", b"lab
-0000cf10: 656c 7365 7422 2c20 2273 7461 7475 7322  elset", "status"
-0000cf20: 2c20 6222 7374 6174 7573 225d 2920 2d3e  , b"status"]) ->
-0000cf30: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
-0000cf40: 616c 5f5f 5f47 6574 4c61 6265 6c53 6574  al___GetLabelSet
-0000cf50: 5265 7370 6f6e 7365 203d 2047 6574 4c61  Response = GetLa
-0000cf60: 6265 6c53 6574 5265 7370 6f6e 7365 0a0a  belSetResponse..
-0000cf70: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
-0000cf80: 6173 7320 4765 7445 6e74 6974 6965 7347  ass GetEntitiesG
-0000cf90: 726f 7570 5265 7175 6573 7428 676f 6f67  roupRequest(goog
-0000cfa0: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-0000cfb0: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-0000cfc0: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-0000cfd0: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-0000cfe0: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-0000cff0: 746f 720a 0a20 2020 204b 425f 4649 454c  tor..    KB_FIEL
-0000d000: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-0000d010: 6e73 2e69 6e74 0a20 2020 2047 524f 5550  ns.int.    GROUP
-0000d020: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000d030: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000d040: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
-0000d050: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
-0000d060: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
-0000d070: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
-0000d080: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
-0000d090: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
-0000d0a0: 426f 7849 443a 202e 2e2e 0a20 2020 2064  BoxID: ....    d
-0000d0b0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0000d0c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000d0d0: 2020 202a 2c0a 2020 2020 2020 2020 6b62     *,.        kb
-0000d0e0: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-0000d0f0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-0000d100: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
-0000d110: 4420 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  D | None = ...,.
-0000d120: 2020 2020 2020 2020 6772 6f75 703a 2062          group: b
-0000d130: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
-0000d140: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
-0000d150: 3a20 2e2e 2e0a 2020 2020 6465 6620 4861  : ....    def Ha
-0000d160: 7346 6965 6c64 2873 656c 662c 2066 6965  sField(self, fie
-0000d170: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-0000d180: 4c69 7465 7261 6c5b 226b 6222 2c20 6222  Literal["kb", b"
-0000d190: 6b62 225d 2920 2d3e 2062 7569 6c74 696e  kb"]) -> builtin
-0000d1a0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
-0000d1b0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-0000d1c0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000d1d0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000d1e0: 2267 726f 7570 222c 2062 2267 726f 7570  "group", b"group
-0000d1f0: 222c 2022 6b62 222c 2062 226b 6222 5d29  ", "kb", b"kb"])
-0000d200: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
-0000d210: 6c6f 6261 6c5f 5f5f 4765 7445 6e74 6974  lobal___GetEntit
-0000d220: 6965 7347 726f 7570 5265 7175 6573 7420  iesGroupRequest 
-0000d230: 3d20 4765 7445 6e74 6974 6965 7347 726f  = GetEntitiesGro
-0000d240: 7570 5265 7175 6573 740a 0a40 7479 7069  upRequest..@typi
-0000d250: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
-0000d260: 6574 456e 7469 7469 6573 4772 6f75 7052  etEntitiesGroupR
-0000d270: 6573 706f 6e73 6528 676f 6f67 6c65 2e70  esponse(google.p
-0000d280: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-0000d290: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-0000d2a0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000d2b0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000d2c0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-0000d2d0: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
-0000d2e0: 7573 3a0a 2020 2020 2020 2020 5661 6c75  us:.        Valu
-0000d2f0: 6554 7970 6520 3d20 7479 7069 6e67 2e4e  eType = typing.N
-0000d300: 6577 5479 7065 2822 5661 6c75 6554 7970  ewType("ValueTyp
-0000d310: 6522 2c20 6275 696c 7469 6e73 2e69 6e74  e", builtins.int
-0000d320: 290a 2020 2020 2020 2020 563a 2074 7970  ).        V: typ
-0000d330: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
-0000d340: 7970 6541 6c69 6173 203d 2056 616c 7565  ypeAlias = Value
-0000d350: 5479 7065 0a0a 2020 2020 636c 6173 7320  Type..    class 
-0000d360: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
-0000d370: 7261 7070 6572 2867 6f6f 676c 652e 7072  rapper(google.pr
-0000d380: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
-0000d390: 656e 756d 5f74 7970 655f 7772 6170 7065  enum_type_wrappe
-0000d3a0: 722e 5f45 6e75 6d54 7970 6557 7261 7070  r._EnumTypeWrapp
-0000d3b0: 6572 5b47 6574 456e 7469 7469 6573 4772  er[GetEntitiesGr
-0000d3c0: 6f75 7052 6573 706f 6e73 652e 5f53 7461  oupResponse._Sta
-0000d3d0: 7475 732e 5661 6c75 6554 7970 655d 2c20  tus.ValueType], 
-0000d3e0: 6275 696c 7469 6e73 2e74 7970 6529 3a0a  builtins.type):.
-0000d3f0: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
-0000d400: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000d410: 6275 662e 6465 7363 7269 7074 6f72 2e45  buf.descriptor.E
-0000d420: 6e75 6d44 6573 6372 6970 746f 720a 2020  numDescriptor.  
-0000d430: 2020 2020 2020 4f4b 3a20 4765 7445 6e74        OK: GetEnt
-0000d440: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
-0000d450: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
-0000d460: 5479 7065 2020 2320 300a 2020 2020 2020  Type  # 0.      
-0000d470: 2020 4b42 5f4e 4f54 5f46 4f55 4e44 3a20    KB_NOT_FOUND: 
-0000d480: 4765 7445 6e74 6974 6965 7347 726f 7570  GetEntitiesGroup
-0000d490: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
-0000d4a0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
-0000d4b0: 2020 2020 2020 2020 454e 5449 5449 4553          ENTITIES
-0000d4c0: 5f47 524f 5550 5f4e 4f54 5f46 4f55 4e44  _GROUP_NOT_FOUND
-0000d4d0: 3a20 4765 7445 6e74 6974 6965 7347 726f  : GetEntitiesGro
-0000d4e0: 7570 5265 7370 6f6e 7365 2e5f 5374 6174  upResponse._Stat
-0000d4f0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000d500: 320a 2020 2020 2020 2020 4552 524f 523a  2.        ERROR:
-0000d510: 2047 6574 456e 7469 7469 6573 4772 6f75   GetEntitiesGrou
-0000d520: 7052 6573 706f 6e73 652e 5f53 7461 7475  pResponse._Statu
-0000d530: 732e 5661 6c75 6554 7970 6520 2023 2033  s.ValueType  # 3
-0000d540: 0a0a 2020 2020 636c 6173 7320 5374 6174  ..    class Stat
-0000d550: 7573 285f 5374 6174 7573 2c20 6d65 7461  us(_Status, meta
-0000d560: 636c 6173 733d 5f53 7461 7475 7345 6e75  class=_StatusEnu
-0000d570: 6d54 7970 6557 7261 7070 6572 293a 202e  mTypeWrapper): .
-0000d580: 2e2e 0a20 2020 204f 4b3a 2047 6574 456e  ...    OK: GetEn
-0000d590: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
-0000d5a0: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
-0000d5b0: 5479 7065 2020 2320 300a 2020 2020 4b42  Type  # 0.    KB
-0000d5c0: 5f4e 4f54 5f46 4f55 4e44 3a20 4765 7445  _NOT_FOUND: GetE
-0000d5d0: 6e74 6974 6965 7347 726f 7570 5265 7370  ntitiesGroupResp
-0000d5e0: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
-0000d5f0: 6554 7970 6520 2023 2031 0a20 2020 2045  eType  # 1.    E
-0000d600: 4e54 4954 4945 535f 4752 4f55 505f 4e4f  NTITIES_GROUP_NO
-0000d610: 545f 464f 554e 443a 2047 6574 456e 7469  T_FOUND: GetEnti
-0000d620: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-0000d630: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-0000d640: 7065 2020 2320 320a 2020 2020 4552 524f  pe  # 2.    ERRO
-0000d650: 523a 2047 6574 456e 7469 7469 6573 4772  R: GetEntitiesGr
-0000d660: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
-0000d670: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000d680: 330a 0a20 2020 204b 425f 4649 454c 445f  3..    KB_FIELD_
-0000d690: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-0000d6a0: 2e69 6e74 0a20 2020 2047 524f 5550 5f46  .int.    GROUP_F
-0000d6b0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-0000d6c0: 6c74 696e 732e 696e 740a 2020 2020 5354  ltins.int.    ST
-0000d6d0: 4154 5553 5f46 4945 4c44 5f4e 554d 4245  ATUS_FIELD_NUMBE
-0000d6e0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000d6f0: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
-0000d700: 616c 5f5f 5f47 6574 456e 7469 7469 6573  al___GetEntities
-0000d710: 4772 6f75 7052 6573 706f 6e73 652e 5374  GroupResponse.St
-0000d720: 6174 7573 2e56 616c 7565 5479 7065 0a20  atus.ValueType. 
-0000d730: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000d740: 2064 6566 206b 6228 7365 6c66 2920 2d3e   def kb(self) ->
-0000d750: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-0000d760: 2e6b 6e6f 776c 6564 6765 626f 785f 7062  .knowledgebox_pb
-0000d770: 322e 4b6e 6f77 6c65 6467 6542 6f78 4944  2.KnowledgeBoxID
-0000d780: 3a20 2e2e 2e0a 2020 2020 4070 726f 7065  : ....    @prope
-0000d790: 7274 790a 2020 2020 6465 6620 6772 6f75  rty.    def grou
-0000d7a0: 7028 7365 6c66 2920 2d3e 206e 7563 6c69  p(self) -> nucli
-0000d7b0: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-0000d7c0: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
-0000d7d0: 7469 6573 4772 6f75 703a 202e 2e2e 0a20  tiesGroup: .... 
-0000d7e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000d7f0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000d800: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-0000d810: 2020 6b62 3a20 6e75 636c 6961 6462 5f70    kb: nucliadb_p
-0000d820: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
-0000d830: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
-0000d840: 426f 7849 4420 7c20 4e6f 6e65 203d 202e  BoxID | None = .
-0000d850: 2e2e 2c0a 2020 2020 2020 2020 6772 6f75  ..,.        grou
-0000d860: 703a 206e 7563 6c69 6164 625f 7072 6f74  p: nucliadb_prot
-0000d870: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-0000d880: 7062 322e 456e 7469 7469 6573 4772 6f75  pb2.EntitiesGrou
-0000d890: 7020 7c20 4e6f 6e65 203d 202e 2e2e 2c0a  p | None = ...,.
-0000d8a0: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
-0000d8b0: 676c 6f62 616c 5f5f 5f47 6574 456e 7469  global___GetEnti
-0000d8c0: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
-0000d8d0: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
-0000d8e0: 7065 203d 202e 2e2e 2c0a 2020 2020 2920  pe = ...,.    ) 
-0000d8f0: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
-0000d900: 2064 6566 2048 6173 4669 656c 6428 7365   def HasField(se
-0000d910: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
-0000d920: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
-0000d930: 6772 6f75 7022 2c20 6222 6772 6f75 7022  group", b"group"
-0000d940: 2c20 226b 6222 2c20 6222 6b62 225d 2920  , "kb", b"kb"]) 
-0000d950: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
-0000d960: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
-0000d970: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
-0000d980: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-0000d990: 672e 4c69 7465 7261 6c5b 2267 726f 7570  g.Literal["group
-0000d9a0: 222c 2062 2267 726f 7570 222c 2022 6b62  ", b"group", "kb
-0000d9b0: 222c 2062 226b 6222 2c20 2273 7461 7475  ", b"kb", "statu
-0000d9c0: 7322 2c20 6222 7374 6174 7573 225d 2920  s", b"status"]) 
-0000d9d0: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
-0000d9e0: 6f62 616c 5f5f 5f47 6574 456e 7469 7469  obal___GetEntiti
-0000d9f0: 6573 4772 6f75 7052 6573 706f 6e73 6520  esGroupResponse 
-0000da00: 3d20 4765 7445 6e74 6974 6965 7347 726f  = GetEntitiesGro
-0000da10: 7570 5265 7370 6f6e 7365 0a0a 4074 7970  upResponse..@typ
-0000da20: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-0000da30: 4765 7456 6563 746f 7253 6574 7352 6571  GetVectorSetsReq
-0000da40: 7565 7374 2867 6f6f 676c 652e 7072 6f74  uest(google.prot
-0000da50: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-0000da60: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
-0000da70: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-0000da80: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-0000da90: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-0000daa0: 2020 4b42 5f46 4945 4c44 5f4e 554d 4245    KB_FIELD_NUMBE
-0000dab0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000dac0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0000dad0: 2020 6465 6620 6b62 2873 656c 6629 202d    def kb(self) -
-0000dae0: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
-0000daf0: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
-0000db00: 6232 2e4b 6e6f 776c 6564 6765 426f 7849  b2.KnowledgeBoxI
-0000db10: 443a 202e 2e2e 0a20 2020 2064 6566 205f  D: ....    def _
-0000db20: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000db30: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-0000db40: 2c0a 2020 2020 2020 2020 6b62 3a20 6e75  ,.        kb: nu
-0000db50: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
-0000db60: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
-0000db70: 6e6f 776c 6564 6765 426f 7849 4420 7c20  nowledgeBoxID | 
-0000db80: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-0000db90: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-0000dba0: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
-0000dbb0: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-0000dbc0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-0000dbd0: 5b22 6b62 222c 2062 226b 6222 5d29 202d  ["kb", b"kb"]) -
-0000dbe0: 3e20 6275 696c 7469 6e73 2e62 6f6f 6c3a  > builtins.bool:
-0000dbf0: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
-0000dc00: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
-0000dc10: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-0000dc20: 2e4c 6974 6572 616c 5b22 6b62 222c 2062  .Literal["kb", b
-0000dc30: 226b 6222 5d29 202d 3e20 4e6f 6e65 3a20  "kb"]) -> None: 
-0000dc40: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4765  .....global___Ge
-0000dc50: 7456 6563 746f 7253 6574 7352 6571 7565  tVectorSetsReque
-0000dc60: 7374 203d 2047 6574 5665 6374 6f72 5365  st = GetVectorSe
-0000dc70: 7473 5265 7175 6573 740a 0a40 7479 7069  tsRequest..@typi
-0000dc80: 6e67 2e66 696e 616c 0a63 6c61 7373 2047  ng.final.class G
-0000dc90: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
-0000dca0: 6f6e 7365 2867 6f6f 676c 652e 7072 6f74  onse(google.prot
-0000dcb0: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
-0000dcc0: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
-0000dcd0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
-0000dce0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
-0000dcf0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
-0000dd00: 2020 636c 6173 7320 5f53 7461 7475 733a    class _Status:
-0000dd10: 0a20 2020 2020 2020 2056 616c 7565 5479  .        ValueTy
-0000dd20: 7065 203d 2074 7970 696e 672e 4e65 7754  pe = typing.NewT
-0000dd30: 7970 6528 2256 616c 7565 5479 7065 222c  ype("ValueType",
-0000dd40: 2062 7569 6c74 696e 732e 696e 7429 0a20   builtins.int). 
-0000dd50: 2020 2020 2020 2056 3a20 7479 7069 6e67         V: typing
-0000dd60: 5f65 7874 656e 7369 6f6e 732e 5479 7065  _extensions.Type
-0000dd70: 416c 6961 7320 3d20 5661 6c75 6554 7970  Alias = ValueTyp
-0000dd80: 650a 0a20 2020 2063 6c61 7373 205f 5374  e..    class _St
-0000dd90: 6174 7573 456e 756d 5479 7065 5772 6170  atusEnumTypeWrap
-0000dda0: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
-0000ddb0: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
-0000ddc0: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
-0000ddd0: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
-0000dde0: 4765 7456 6563 746f 7253 6574 7352 6573  GetVectorSetsRes
-0000ddf0: 706f 6e73 652e 5f53 7461 7475 732e 5661  ponse._Status.Va
-0000de00: 6c75 6554 7970 655d 2c20 6275 696c 7469  lueType], builti
-0000de10: 6e73 2e74 7970 6529 3a0a 2020 2020 2020  ns.type):.      
-0000de20: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-0000de30: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-0000de40: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
-0000de50: 6372 6970 746f 720a 2020 2020 2020 2020  criptor.        
-0000de60: 4f4b 3a20 4765 7456 6563 746f 7253 6574  OK: GetVectorSet
-0000de70: 7352 6573 706f 6e73 652e 5f53 7461 7475  sResponse._Statu
-0000de80: 732e 5661 6c75 6554 7970 6520 2023 2030  s.ValueType  # 0
-0000de90: 0a20 2020 2020 2020 204e 4f54 464f 554e  .        NOTFOUN
-0000dea0: 443a 2047 6574 5665 6374 6f72 5365 7473  D: GetVectorSets
-0000deb0: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
-0000dec0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
-0000ded0: 2020 2020 2020 2020 4552 524f 523a 2047          ERROR: G
-0000dee0: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
-0000def0: 6f6e 7365 2e5f 5374 6174 7573 2e56 616c  onse._Status.Val
-0000df00: 7565 5479 7065 2020 2320 320a 0a20 2020  ueType  # 2..   
-0000df10: 2063 6c61 7373 2053 7461 7475 7328 5f53   class Status(_S
-0000df20: 7461 7475 732c 206d 6574 6163 6c61 7373  tatus, metaclass
-0000df30: 3d5f 5374 6174 7573 456e 756d 5479 7065  =_StatusEnumType
-0000df40: 5772 6170 7065 7229 3a20 2e2e 2e0a 2020  Wrapper): ....  
-0000df50: 2020 4f4b 3a20 4765 7456 6563 746f 7253    OK: GetVectorS
-0000df60: 6574 7352 6573 706f 6e73 652e 5374 6174  etsResponse.Stat
-0000df70: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000df80: 300a 2020 2020 4e4f 5446 4f55 4e44 3a20  0.    NOTFOUND: 
-0000df90: 4765 7456 6563 746f 7253 6574 7352 6573  GetVectorSetsRes
-0000dfa0: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-0000dfb0: 7565 5479 7065 2020 2320 310a 2020 2020  ueType  # 1.    
-0000dfc0: 4552 524f 523a 2047 6574 5665 6374 6f72  ERROR: GetVector
-0000dfd0: 5365 7473 5265 7370 6f6e 7365 2e53 7461  SetsResponse.Sta
-0000dfe0: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
-0000dff0: 2032 0a0a 2020 2020 4b42 5f46 4945 4c44   2..    KB_FIELD
-0000e000: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000e010: 732e 696e 740a 2020 2020 5645 4354 4f52  s.int.    VECTOR
-0000e020: 5345 5453 5f46 4945 4c44 5f4e 554d 4245  SETS_FIELD_NUMBE
-0000e030: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000e040: 2020 2020 5354 4154 5553 5f46 4945 4c44      STATUS_FIELD
-0000e050: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000e060: 732e 696e 740a 2020 2020 7374 6174 7573  s.int.    status
-0000e070: 3a20 676c 6f62 616c 5f5f 5f47 6574 5665  : global___GetVe
-0000e080: 6374 6f72 5365 7473 5265 7370 6f6e 7365  ctorSetsResponse
-0000e090: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
-0000e0a0: 650a 2020 2020 4070 726f 7065 7274 790a  e.    @property.
-0000e0b0: 2020 2020 6465 6620 6b62 2873 656c 6629      def kb(self)
-0000e0c0: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
-0000e0d0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-0000e0e0: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
-0000e0f0: 7849 443a 202e 2e2e 0a20 2020 2040 7072  xID: ....    @pr
-0000e100: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
-0000e110: 6563 746f 7273 6574 7328 7365 6c66 2920  ectorsets(self) 
-0000e120: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
-0000e130: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
-0000e140: 7062 322e 5665 6374 6f72 5365 7473 3a20  pb2.VectorSets: 
-0000e150: 2e2e 2e0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-0000e160: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0000e170: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
-0000e180: 2020 2020 2020 206b 623a 206e 7563 6c69         kb: nucli
-0000e190: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-0000e1a0: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
-0000e1b0: 6c65 6467 6542 6f78 4944 207c 204e 6f6e  ledgeBoxID | Non
-0000e1c0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-0000e1d0: 2076 6563 746f 7273 6574 733a 206e 7563   vectorsets: nuc
-0000e1e0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
-0000e1f0: 776c 6564 6765 626f 785f 7062 322e 5665  wledgebox_pb2.Ve
-0000e200: 6374 6f72 5365 7473 207c 204e 6f6e 6520  ctorSets | None 
-0000e210: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2073  = ...,.        s
-0000e220: 7461 7475 733a 2067 6c6f 6261 6c5f 5f5f  tatus: global___
-0000e230: 4765 7456 6563 746f 7253 6574 7352 6573  GetVectorSetsRes
-0000e240: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
-0000e250: 7565 5479 7065 203d 202e 2e2e 2c0a 2020  ueType = ...,.  
-0000e260: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
-0000e270: 0a20 2020 2064 6566 2048 6173 4669 656c  .    def HasFiel
-0000e280: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-0000e290: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-0000e2a0: 616c 5b22 6b62 222c 2062 226b 6222 2c20  al["kb", b"kb", 
-0000e2b0: 2276 6563 746f 7273 6574 7322 2c20 6222  "vectorsets", b"
-0000e2c0: 7665 6374 6f72 7365 7473 225d 2920 2d3e  vectorsets"]) ->
-0000e2d0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
-0000e2e0: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
-0000e2f0: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-0000e300: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-0000e310: 4c69 7465 7261 6c5b 226b 6222 2c20 6222  Literal["kb", b"
-0000e320: 6b62 222c 2022 7374 6174 7573 222c 2062  kb", "status", b
-0000e330: 2273 7461 7475 7322 2c20 2276 6563 746f  "status", "vecto
-0000e340: 7273 6574 7322 2c20 6222 7665 6374 6f72  rsets", b"vector
-0000e350: 7365 7473 225d 2920 2d3e 204e 6f6e 653a  sets"]) -> None:
-0000e360: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f47   .....global___G
-0000e370: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
-0000e380: 6f6e 7365 203d 2047 6574 5665 6374 6f72  onse = GetVector
-0000e390: 5365 7473 5265 7370 6f6e 7365 0a0a 4074  SetsResponse..@t
-0000e3a0: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
-0000e3b0: 7320 4465 6c56 6563 746f 7253 6574 5265  s DelVectorSetRe
-0000e3c0: 7175 6573 7428 676f 6f67 6c65 2e70 726f  quest(google.pro
-0000e3d0: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
-0000e3e0: 7373 6167 6529 3a0a 2020 2020 4445 5343  ssage):.    DESC
-0000e3f0: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
-0000e400: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
-0000e410: 6f72 2e44 6573 6372 6970 746f 720a 0a20  or.Descriptor.. 
-0000e420: 2020 204b 425f 4649 454c 445f 4e55 4d42     KB_FIELD_NUMB
-0000e430: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-0000e440: 0a20 2020 2056 4543 544f 5253 4554 5f46  .    VECTORSET_F
-0000e450: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-0000e460: 6c74 696e 732e 696e 740a 2020 2020 7665  ltins.int.    ve
-0000e470: 6374 6f72 7365 743a 2062 7569 6c74 696e  ctorset: builtin
-0000e480: 732e 7374 720a 2020 2020 4070 726f 7065  s.str.    @prope
-0000e490: 7274 790a 2020 2020 6465 6620 6b62 2873  rty.    def kb(s
-0000e4a0: 656c 6629 202d 3e20 6e75 636c 6961 6462  elf) -> nucliadb
-0000e4b0: 5f70 726f 746f 732e 6b6e 6f77 6c65 6467  _protos.knowledg
-0000e4c0: 6562 6f78 5f70 6232 2e4b 6e6f 776c 6564  ebox_pb2.Knowled
-0000e4d0: 6765 426f 7849 443a 202e 2e2e 0a20 2020  geBoxID: ....   
-0000e4e0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0000e4f0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000e500: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-0000e510: 6b62 3a20 6e75 636c 6961 6462 5f70 726f  kb: nucliadb_pro
-0000e520: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-0000e530: 5f70 6232 2e4b 6e6f 776c 6564 6765 426f  _pb2.KnowledgeBo
-0000e540: 7849 4420 7c20 4e6f 6e65 203d 202e 2e2e  xID | None = ...
-0000e550: 2c0a 2020 2020 2020 2020 7665 6374 6f72  ,.        vector
-0000e560: 7365 743a 2062 7569 6c74 696e 732e 7374  set: builtins.st
-0000e570: 7220 3d20 2e2e 2e2c 0a20 2020 2029 202d  r = ...,.    ) -
-0000e580: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-0000e590: 6465 6620 4861 7346 6965 6c64 2873 656c  def HasField(sel
-0000e5a0: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
-0000e5b0: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
-0000e5c0: 6222 2c20 6222 6b62 225d 2920 2d3e 2062  b", b"kb"]) -> b
-0000e5d0: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-0000e5e0: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-0000e5f0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-0000e600: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-0000e610: 7465 7261 6c5b 226b 6222 2c20 6222 6b62  teral["kb", b"kb
-0000e620: 222c 2022 7665 6374 6f72 7365 7422 2c20  ", "vectorset", 
-0000e630: 6222 7665 6374 6f72 7365 7422 5d29 202d  b"vectorset"]) -
-0000e640: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
-0000e650: 6261 6c5f 5f5f 4465 6c56 6563 746f 7253  bal___DelVectorS
-0000e660: 6574 5265 7175 6573 7420 3d20 4465 6c56  etRequest = DelV
-0000e670: 6563 746f 7253 6574 5265 7175 6573 740a  ectorSetRequest.
-0000e680: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
-0000e690: 6c61 7373 2053 6574 5665 6374 6f72 5365  lass SetVectorSe
-0000e6a0: 7452 6571 7565 7374 2867 6f6f 676c 652e  tRequest(google.
-0000e6b0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
-0000e6c0: 2e4d 6573 7361 6765 293a 0a20 2020 2044  .Message):.    D
-0000e6d0: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
-0000e6e0: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
-0000e6f0: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
-0000e700: 0a0a 2020 2020 4b42 5f46 4945 4c44 5f4e  ..    KB_FIELD_N
-0000e710: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-0000e720: 696e 740a 2020 2020 4944 5f46 4945 4c44  int.    ID_FIELD
-0000e730: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000e740: 732e 696e 740a 2020 2020 5645 4354 4f52  s.int.    VECTOR
-0000e750: 5345 545f 4649 454c 445f 4e55 4d42 4552  SET_FIELD_NUMBER
-0000e760: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-0000e770: 2020 2069 643a 2062 7569 6c74 696e 732e     id: builtins.
-0000e780: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
-0000e790: 790a 2020 2020 6465 6620 6b62 2873 656c  y.    def kb(sel
-0000e7a0: 6629 202d 3e20 6e75 636c 6961 6462 5f70  f) -> nucliadb_p
-0000e7b0: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
-0000e7c0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
-0000e7d0: 426f 7849 443a 202e 2e2e 0a20 2020 2040  BoxID: ....    @
-0000e7e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0000e7f0: 2076 6563 746f 7273 6574 2873 656c 6629   vectorset(self)
-0000e800: 202d 3e20 6e75 636c 6961 6462 5f70 726f   -> nucliadb_pro
-0000e810: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
-0000e820: 5f70 6232 2e56 6563 746f 7253 6574 3a20  _pb2.VectorSet: 
-0000e830: 2e2e 2e0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-0000e840: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0000e850: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
-0000e860: 2020 2020 2020 206b 623a 206e 7563 6c69         kb: nucli
-0000e870: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
-0000e880: 6564 6765 626f 785f 7062 322e 4b6e 6f77  edgebox_pb2.Know
-0000e890: 6c65 6467 6542 6f78 4944 207c 204e 6f6e  ledgeBoxID | Non
-0000e8a0: 6520 3d20 2e2e 2e2c 0a20 2020 2020 2020  e = ...,.       
-0000e8b0: 2069 643a 2062 7569 6c74 696e 732e 7374   id: builtins.st
-0000e8c0: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
-0000e8d0: 2076 6563 746f 7273 6574 3a20 6e75 636c   vectorset: nucl
-0000e8e0: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-0000e8f0: 6c65 6467 6562 6f78 5f70 6232 2e56 6563  ledgebox_pb2.Vec
-0000e900: 746f 7253 6574 207c 204e 6f6e 6520 3d20  torSet | None = 
-0000e910: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
-0000e920: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-0000e930: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
-0000e940: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-0000e950: 672e 4c69 7465 7261 6c5b 226b 6222 2c20  g.Literal["kb", 
-0000e960: 6222 6b62 222c 2022 7665 6374 6f72 7365  b"kb", "vectorse
-0000e970: 7422 2c20 6222 7665 6374 6f72 7365 7422  t", b"vectorset"
-0000e980: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
-0000e990: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
-0000e9a0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
-0000e9b0: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
-0000e9c0: 7069 6e67 2e4c 6974 6572 616c 5b22 6964  ping.Literal["id
-0000e9d0: 222c 2062 2269 6422 2c20 226b 6222 2c20  ", b"id", "kb", 
-0000e9e0: 6222 6b62 222c 2022 7665 6374 6f72 7365  b"kb", "vectorse
-0000e9f0: 7422 2c20 6222 7665 6374 6f72 7365 7422  t", b"vectorset"
-0000ea00: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
-0000ea10: 0a67 6c6f 6261 6c5f 5f5f 5365 7456 6563  .global___SetVec
-0000ea20: 746f 7253 6574 5265 7175 6573 7420 3d20  torSetRequest = 
-0000ea30: 5365 7456 6563 746f 7253 6574 5265 7175  SetVectorSetRequ
-0000ea40: 6573 740a 0a40 7479 7069 6e67 2e66 696e  est..@typing.fin
-0000ea50: 616c 0a63 6c61 7373 204f 7053 7461 7475  al.class OpStatu
-0000ea60: 7357 7269 7465 7228 676f 6f67 6c65 2e70  sWriter(google.p
-0000ea70: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-0000ea80: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-0000ea90: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000eaa0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000eab0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-0000eac0: 0a20 2020 2063 6c61 7373 205f 5374 6174  .    class _Stat
-0000ead0: 7573 3a0a 2020 2020 2020 2020 5661 6c75  us:.        Valu
-0000eae0: 6554 7970 6520 3d20 7479 7069 6e67 2e4e  eType = typing.N
-0000eaf0: 6577 5479 7065 2822 5661 6c75 6554 7970  ewType("ValueTyp
-0000eb00: 6522 2c20 6275 696c 7469 6e73 2e69 6e74  e", builtins.int
-0000eb10: 290a 2020 2020 2020 2020 563a 2074 7970  ).        V: typ
-0000eb20: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
-0000eb30: 7970 6541 6c69 6173 203d 2056 616c 7565  ypeAlias = Value
-0000eb40: 5479 7065 0a0a 2020 2020 636c 6173 7320  Type..    class 
-0000eb50: 5f53 7461 7475 7345 6e75 6d54 7970 6557  _StatusEnumTypeW
-0000eb60: 7261 7070 6572 2867 6f6f 676c 652e 7072  rapper(google.pr
-0000eb70: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
-0000eb80: 656e 756d 5f74 7970 655f 7772 6170 7065  enum_type_wrappe
-0000eb90: 722e 5f45 6e75 6d54 7970 6557 7261 7070  r._EnumTypeWrapp
-0000eba0: 6572 5b4f 7053 7461 7475 7357 7269 7465  er[OpStatusWrite
-0000ebb0: 722e 5f53 7461 7475 732e 5661 6c75 6554  r._Status.ValueT
-0000ebc0: 7970 655d 2c20 6275 696c 7469 6e73 2e74  ype], builtins.t
-0000ebd0: 7970 6529 3a0a 2020 2020 2020 2020 4445  ype):.        DE
-0000ebe0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-0000ebf0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-0000ec00: 7074 6f72 2e45 6e75 6d44 6573 6372 6970  ptor.EnumDescrip
-0000ec10: 746f 720a 2020 2020 2020 2020 4f4b 3a20  tor.        OK: 
-0000ec20: 4f70 5374 6174 7573 5772 6974 6572 2e5f  OpStatusWriter._
-0000ec30: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000ec40: 2020 2320 300a 2020 2020 2020 2020 4552    # 0.        ER
-0000ec50: 524f 523a 204f 7053 7461 7475 7357 7269  ROR: OpStatusWri
-0000ec60: 7465 722e 5f53 7461 7475 732e 5661 6c75  ter._Status.Valu
-0000ec70: 6554 7970 6520 2023 2031 0a20 2020 2020  eType  # 1.     
-0000ec80: 2020 204e 4f54 464f 554e 443a 204f 7053     NOTFOUND: OpS
-0000ec90: 7461 7475 7357 7269 7465 722e 5f53 7461  tatusWriter._Sta
-0000eca0: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
-0000ecb0: 2032 0a0a 2020 2020 636c 6173 7320 5374   2..    class St
-0000ecc0: 6174 7573 285f 5374 6174 7573 2c20 6d65  atus(_Status, me
-0000ecd0: 7461 636c 6173 733d 5f53 7461 7475 7345  taclass=_StatusE
-0000ece0: 6e75 6d54 7970 6557 7261 7070 6572 293a  numTypeWrapper):
-0000ecf0: 202e 2e2e 0a20 2020 204f 4b3a 204f 7053   ....    OK: OpS
-0000ed00: 7461 7475 7357 7269 7465 722e 5374 6174  tatusWriter.Stat
-0000ed10: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000ed20: 300a 2020 2020 4552 524f 523a 204f 7053  0.    ERROR: OpS
-0000ed30: 7461 7475 7357 7269 7465 722e 5374 6174  tatusWriter.Stat
-0000ed40: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
-0000ed50: 310a 2020 2020 4e4f 5446 4f55 4e44 3a20  1.    NOTFOUND: 
-0000ed60: 4f70 5374 6174 7573 5772 6974 6572 2e53  OpStatusWriter.S
-0000ed70: 7461 7475 732e 5661 6c75 6554 7970 6520  tatus.ValueType 
-0000ed80: 2023 2032 0a0a 2020 2020 5354 4154 5553   # 2..    STATUS
-0000ed90: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-0000eda0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-0000edb0: 7374 6174 7573 3a20 676c 6f62 616c 5f5f  status: global__
-0000edc0: 5f4f 7053 7461 7475 7357 7269 7465 722e  _OpStatusWriter.
-0000edd0: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
-0000ede0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000edf0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0000ee00: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000ee10: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
-0000ee20: 616c 5f5f 5f4f 7053 7461 7475 7357 7269  al___OpStatusWri
-0000ee30: 7465 722e 5374 6174 7573 2e56 616c 7565  ter.Status.Value
-0000ee40: 5479 7065 203d 202e 2e2e 2c0a 2020 2020  Type = ...,.    
-0000ee50: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-0000ee60: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-0000ee70: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-0000ee80: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-0000ee90: 616c 5b22 7374 6174 7573 222c 2062 2273  al["status", b"s
-0000eea0: 7461 7475 7322 5d29 202d 3e20 4e6f 6e65  tatus"]) -> None
-0000eeb0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
-0000eec0: 4f70 5374 6174 7573 5772 6974 6572 203d  OpStatusWriter =
-0000eed0: 204f 7053 7461 7475 7357 7269 7465 720a   OpStatusWriter.
-0000eee0: 0a40 7479 7069 6e67 2e66 696e 616c 0a63  .@typing.final.c
-0000eef0: 6c61 7373 204e 6f74 6966 6963 6174 696f  lass Notificatio
-0000ef00: 6e28 676f 6f67 6c65 2e70 726f 746f 6275  n(google.protobu
-0000ef10: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-0000ef20: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-0000ef30: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000ef40: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000ef50: 6573 6372 6970 746f 720a 0a20 2020 2063  escriptor..    c
-0000ef60: 6c61 7373 205f 4163 7469 6f6e 3a0a 2020  lass _Action:.  
-0000ef70: 2020 2020 2020 5661 6c75 6554 7970 6520        ValueType 
-0000ef80: 3d20 7479 7069 6e67 2e4e 6577 5479 7065  = typing.NewType
-0000ef90: 2822 5661 6c75 6554 7970 6522 2c20 6275  ("ValueType", bu
-0000efa0: 696c 7469 6e73 2e69 6e74 290a 2020 2020  iltins.int).    
-0000efb0: 2020 2020 563a 2074 7970 696e 675f 6578      V: typing_ex
-0000efc0: 7465 6e73 696f 6e73 2e54 7970 6541 6c69  tensions.TypeAli
-0000efd0: 6173 203d 2056 616c 7565 5479 7065 0a0a  as = ValueType..
-0000efe0: 2020 2020 636c 6173 7320 5f41 6374 696f      class _Actio
-0000eff0: 6e45 6e75 6d54 7970 6557 7261 7070 6572  nEnumTypeWrapper
-0000f000: 2867 6f6f 676c 652e 7072 6f74 6f62 7566  (google.protobuf
-0000f010: 2e69 6e74 6572 6e61 6c2e 656e 756d 5f74  .internal.enum_t
-0000f020: 7970 655f 7772 6170 7065 722e 5f45 6e75  ype_wrapper._Enu
-0000f030: 6d54 7970 6557 7261 7070 6572 5b4e 6f74  mTypeWrapper[Not
-0000f040: 6966 6963 6174 696f 6e2e 5f41 6374 696f  ification._Actio
-0000f050: 6e2e 5661 6c75 6554 7970 655d 2c20 6275  n.ValueType], bu
-0000f060: 696c 7469 6e73 2e74 7970 6529 3a0a 2020  iltins.type):.  
-0000f070: 2020 2020 2020 4445 5343 5249 5054 4f52        DESCRIPTOR
-0000f080: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
-0000f090: 662e 6465 7363 7269 7074 6f72 2e45 6e75  f.descriptor.Enu
-0000f0a0: 6d44 6573 6372 6970 746f 720a 2020 2020  mDescriptor.    
-0000f0b0: 2020 2020 434f 4d4d 4954 3a20 4e6f 7469      COMMIT: Noti
-0000f0c0: 6669 6361 7469 6f6e 2e5f 4163 7469 6f6e  fication._Action
-0000f0d0: 2e56 616c 7565 5479 7065 2020 2320 300a  .ValueType  # 0.
-0000f0e0: 2020 2020 2020 2020 4142 4f52 543a 204e          ABORT: N
-0000f0f0: 6f74 6966 6963 6174 696f 6e2e 5f41 6374  otification._Act
-0000f100: 696f 6e2e 5661 6c75 6554 7970 6520 2023  ion.ValueType  #
-0000f110: 2031 0a20 2020 2020 2020 2049 4e44 4558   1.        INDEX
-0000f120: 4544 3a20 4e6f 7469 6669 6361 7469 6f6e  ED: Notification
-0000f130: 2e5f 4163 7469 6f6e 2e56 616c 7565 5479  ._Action.ValueTy
-0000f140: 7065 2020 2320 320a 0a20 2020 2063 6c61  pe  # 2..    cla
-0000f150: 7373 2041 6374 696f 6e28 5f41 6374 696f  ss Action(_Actio
-0000f160: 6e2c 206d 6574 6163 6c61 7373 3d5f 4163  n, metaclass=_Ac
-0000f170: 7469 6f6e 456e 756d 5479 7065 5772 6170  tionEnumTypeWrap
-0000f180: 7065 7229 3a20 2e2e 2e0a 2020 2020 434f  per): ....    CO
-0000f190: 4d4d 4954 3a20 4e6f 7469 6669 6361 7469  MMIT: Notificati
-0000f1a0: 6f6e 2e41 6374 696f 6e2e 5661 6c75 6554  on.Action.ValueT
-0000f1b0: 7970 6520 2023 2030 0a20 2020 2041 424f  ype  # 0.    ABO
-0000f1c0: 5254 3a20 4e6f 7469 6669 6361 7469 6f6e  RT: Notification
-0000f1d0: 2e41 6374 696f 6e2e 5661 6c75 6554 7970  .Action.ValueTyp
-0000f1e0: 6520 2023 2031 0a20 2020 2049 4e44 4558  e  # 1.    INDEX
-0000f1f0: 4544 3a20 4e6f 7469 6669 6361 7469 6f6e  ED: Notification
-0000f200: 2e41 6374 696f 6e2e 5661 6c75 6554 7970  .Action.ValueTyp
-0000f210: 6520 2023 2032 0a0a 2020 2020 636c 6173  e  # 2..    clas
-0000f220: 7320 5f57 7269 7465 5479 7065 3a0a 2020  s _WriteType:.  
-0000f230: 2020 2020 2020 5661 6c75 6554 7970 6520        ValueType 
-0000f240: 3d20 7479 7069 6e67 2e4e 6577 5479 7065  = typing.NewType
-0000f250: 2822 5661 6c75 6554 7970 6522 2c20 6275  ("ValueType", bu
-0000f260: 696c 7469 6e73 2e69 6e74 290a 2020 2020  iltins.int).    
-0000f270: 2020 2020 563a 2074 7970 696e 675f 6578      V: typing_ex
-0000f280: 7465 6e73 696f 6e73 2e54 7970 6541 6c69  tensions.TypeAli
-0000f290: 6173 203d 2056 616c 7565 5479 7065 0a0a  as = ValueType..
-0000f2a0: 2020 2020 636c 6173 7320 5f57 7269 7465      class _Write
-0000f2b0: 5479 7065 456e 756d 5479 7065 5772 6170  TypeEnumTypeWrap
-0000f2c0: 7065 7228 676f 6f67 6c65 2e70 726f 746f  per(google.proto
-0000f2d0: 6275 662e 696e 7465 726e 616c 2e65 6e75  buf.internal.enu
-0000f2e0: 6d5f 7479 7065 5f77 7261 7070 6572 2e5f  m_type_wrapper._
-0000f2f0: 456e 756d 5479 7065 5772 6170 7065 725b  EnumTypeWrapper[
-0000f300: 4e6f 7469 6669 6361 7469 6f6e 2e5f 5772  Notification._Wr
-0000f310: 6974 6554 7970 652e 5661 6c75 6554 7970  iteType.ValueTyp
-0000f320: 655d 2c20 6275 696c 7469 6e73 2e74 7970  e], builtins.typ
-0000f330: 6529 3a0a 2020 2020 2020 2020 4445 5343  e):.        DESC
-0000f340: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
-0000f350: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
-0000f360: 6f72 2e45 6e75 6d44 6573 6372 6970 746f  or.EnumDescripto
-0000f370: 720a 2020 2020 2020 2020 554e 5345 543a  r.        UNSET:
-0000f380: 204e 6f74 6966 6963 6174 696f 6e2e 5f57   Notification._W
-0000f390: 7269 7465 5479 7065 2e56 616c 7565 5479  riteType.ValueTy
-0000f3a0: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
-0000f3b0: 4352 4541 5445 443a 204e 6f74 6966 6963  CREATED: Notific
-0000f3c0: 6174 696f 6e2e 5f57 7269 7465 5479 7065  ation._WriteType
-0000f3d0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
-0000f3e0: 2020 2020 2020 2020 4d4f 4449 4649 4544          MODIFIED
-0000f3f0: 3a20 4e6f 7469 6669 6361 7469 6f6e 2e5f  : Notification._
-0000f400: 5772 6974 6554 7970 652e 5661 6c75 6554  WriteType.ValueT
-0000f410: 7970 6520 2023 2032 0a20 2020 2020 2020  ype  # 2.       
-0000f420: 2044 454c 4554 4544 3a20 4e6f 7469 6669   DELETED: Notifi
-0000f430: 6361 7469 6f6e 2e5f 5772 6974 6554 7970  cation._WriteTyp
-0000f440: 652e 5661 6c75 6554 7970 6520 2023 2033  e.ValueType  # 3
-0000f450: 0a0a 2020 2020 636c 6173 7320 5772 6974  ..    class Writ
-0000f460: 6554 7970 6528 5f57 7269 7465 5479 7065  eType(_WriteType
-0000f470: 2c20 6d65 7461 636c 6173 733d 5f57 7269  , metaclass=_Wri
-0000f480: 7465 5479 7065 456e 756d 5479 7065 5772  teTypeEnumTypeWr
-0000f490: 6170 7065 7229 3a20 2e2e 2e0a 2020 2020  apper): ....    
-0000f4a0: 554e 5345 543a 204e 6f74 6966 6963 6174  UNSET: Notificat
-0000f4b0: 696f 6e2e 5772 6974 6554 7970 652e 5661  ion.WriteType.Va
-0000f4c0: 6c75 6554 7970 6520 2023 2030 0a20 2020  lueType  # 0.   
-0000f4d0: 2043 5245 4154 4544 3a20 4e6f 7469 6669   CREATED: Notifi
-0000f4e0: 6361 7469 6f6e 2e57 7269 7465 5479 7065  cation.WriteType
-0000f4f0: 2e56 616c 7565 5479 7065 2020 2320 310a  .ValueType  # 1.
-0000f500: 2020 2020 4d4f 4449 4649 4544 3a20 4e6f      MODIFIED: No
-0000f510: 7469 6669 6361 7469 6f6e 2e57 7269 7465  tification.Write
-0000f520: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
-0000f530: 2320 320a 2020 2020 4445 4c45 5445 443a  # 2.    DELETED:
-0000f540: 204e 6f74 6966 6963 6174 696f 6e2e 5772   Notification.Wr
-0000f550: 6974 6554 7970 652e 5661 6c75 6554 7970  iteType.ValueTyp
-0000f560: 6520 2023 2033 0a0a 2020 2020 5041 5254  e  # 3..    PART
-0000f570: 4954 494f 4e5f 4649 454c 445f 4e55 4d42  ITION_FIELD_NUMB
-0000f580: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-0000f590: 0a20 2020 204d 554c 5449 5f46 4945 4c44  .    MULTI_FIELD
-0000f5a0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-0000f5b0: 732e 696e 740a 2020 2020 5555 4944 5f46  s.int.    UUID_F
-0000f5c0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-0000f5d0: 6c74 696e 732e 696e 740a 2020 2020 4b42  ltins.int.    KB
-0000f5e0: 4944 5f46 4945 4c44 5f4e 554d 4245 523a  ID_FIELD_NUMBER:
-0000f5f0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-0000f600: 2020 5345 5149 445f 4649 454c 445f 4e55    SEQID_FIELD_NU
-0000f610: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-0000f620: 6e74 0a20 2020 2041 4354 494f 4e5f 4649  nt.    ACTION_FI
-0000f630: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-0000f640: 7469 6e73 2e69 6e74 0a20 2020 2057 5249  tins.int.    WRI
-0000f650: 5445 5f54 5950 455f 4649 454c 445f 4e55  TE_TYPE_FIELD_NU
-0000f660: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-0000f670: 6e74 0a20 2020 204d 4553 5341 4745 5f46  nt.    MESSAGE_F
-0000f680: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-0000f690: 6c74 696e 732e 696e 740a 2020 2020 534f  ltins.int.    SO
-0000f6a0: 5552 4345 5f46 4945 4c44 5f4e 554d 4245  URCE_FIELD_NUMBE
-0000f6b0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-0000f6c0: 2020 2020 5052 4f43 4553 5349 4e47 5f45      PROCESSING_E
-0000f6d0: 5252 4f52 535f 4649 454c 445f 4e55 4d42  RRORS_FIELD_NUMB
-0000f6e0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-0000f6f0: 0a20 2020 204d 4553 5341 4745 5f41 5544  .    MESSAGE_AUD
-0000f700: 4954 5f46 4945 4c44 5f4e 554d 4245 523a  IT_FIELD_NUMBER:
-0000f710: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-0000f720: 2020 7061 7274 6974 696f 6e3a 2062 7569    partition: bui
-0000f730: 6c74 696e 732e 696e 740a 2020 2020 6d75  ltins.int.    mu
-0000f740: 6c74 693a 2062 7569 6c74 696e 732e 7374  lti: builtins.st
-0000f750: 720a 2020 2020 7575 6964 3a20 6275 696c  r.    uuid: buil
-0000f760: 7469 6e73 2e73 7472 0a20 2020 206b 6269  tins.str.    kbi
-0000f770: 643a 2062 7569 6c74 696e 732e 7374 720a  d: builtins.str.
-0000f780: 2020 2020 7365 7169 643a 2062 7569 6c74      seqid: built
-0000f790: 696e 732e 696e 740a 2020 2020 6163 7469  ins.int.    acti
-0000f7a0: 6f6e 3a20 676c 6f62 616c 5f5f 5f4e 6f74  on: global___Not
-0000f7b0: 6966 6963 6174 696f 6e2e 4163 7469 6f6e  ification.Action
-0000f7c0: 2e56 616c 7565 5479 7065 0a20 2020 2077  .ValueType.    w
-0000f7d0: 7269 7465 5f74 7970 653a 2067 6c6f 6261  rite_type: globa
-0000f7e0: 6c5f 5f5f 4e6f 7469 6669 6361 7469 6f6e  l___Notification
-0000f7f0: 2e57 7269 7465 5479 7065 2e56 616c 7565  .WriteType.Value
-0000f800: 5479 7065 0a20 2020 2073 6f75 7263 653a  Type.    source:
-0000f810: 2067 6c6f 6261 6c5f 5f5f 4e6f 7469 6669   global___Notifi
-0000f820: 6361 7469 6f6e 536f 7572 6365 2e56 616c  cationSource.Val
-0000f830: 7565 5479 7065 0a20 2020 2070 726f 6365  ueType.    proce
-0000f840: 7373 696e 675f 6572 726f 7273 3a20 6275  ssing_errors: bu
-0000f850: 696c 7469 6e73 2e62 6f6f 6c0a 2020 2020  iltins.bool.    
-0000f860: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000f870: 6620 6d65 7373 6167 6528 7365 6c66 2920  f message(self) 
-0000f880: 2d3e 2067 6c6f 6261 6c5f 5f5f 4272 6f6b  -> global___Brok
-0000f890: 6572 4d65 7373 6167 653a 202e 2e2e 0a20  erMessage: .... 
-0000f8a0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000f8b0: 2064 6566 206d 6573 7361 6765 5f61 7564   def message_aud
-0000f8c0: 6974 2873 656c 6629 202d 3e20 676c 6f62  it(self) -> glob
-0000f8d0: 616c 5f5f 5f41 7564 6974 3a20 2e2e 2e0a  al___Audit: ....
-0000f8e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000f8f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000f900: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-0000f910: 2020 2070 6172 7469 7469 6f6e 3a20 6275     partition: bu
-0000f920: 696c 7469 6e73 2e69 6e74 203d 202e 2e2e  iltins.int = ...
-0000f930: 2c0a 2020 2020 2020 2020 6d75 6c74 693a  ,.        multi:
-0000f940: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-0000f950: 2e2e 2e2c 0a20 2020 2020 2020 2075 7569  ...,.        uui
-0000f960: 643a 2062 7569 6c74 696e 732e 7374 7220  d: builtins.str 
-0000f970: 3d20 2e2e 2e2c 0a20 2020 2020 2020 206b  = ...,.        k
-0000f980: 6269 643a 2062 7569 6c74 696e 732e 7374  bid: builtins.st
-0000f990: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
-0000f9a0: 2073 6571 6964 3a20 6275 696c 7469 6e73   seqid: builtins
-0000f9b0: 2e69 6e74 203d 202e 2e2e 2c0a 2020 2020  .int = ...,.    
-0000f9c0: 2020 2020 6163 7469 6f6e 3a20 676c 6f62      action: glob
-0000f9d0: 616c 5f5f 5f4e 6f74 6966 6963 6174 696f  al___Notificatio
-0000f9e0: 6e2e 4163 7469 6f6e 2e56 616c 7565 5479  n.Action.ValueTy
-0000f9f0: 7065 203d 202e 2e2e 2c0a 2020 2020 2020  pe = ...,.      
-0000fa00: 2020 7772 6974 655f 7479 7065 3a20 676c    write_type: gl
-0000fa10: 6f62 616c 5f5f 5f4e 6f74 6966 6963 6174  obal___Notificat
-0000fa20: 696f 6e2e 5772 6974 6554 7970 652e 5661  ion.WriteType.Va
-0000fa30: 6c75 6554 7970 6520 3d20 2e2e 2e2c 0a20  lueType = ...,. 
-0000fa40: 2020 2020 2020 206d 6573 7361 6765 3a20         message: 
-0000fa50: 676c 6f62 616c 5f5f 5f42 726f 6b65 724d  global___BrokerM
-0000fa60: 6573 7361 6765 207c 204e 6f6e 6520 3d20  essage | None = 
-0000fa70: 2e2e 2e2c 0a20 2020 2020 2020 2073 6f75  ...,.        sou
-0000fa80: 7263 653a 2067 6c6f 6261 6c5f 5f5f 4e6f  rce: global___No
-0000fa90: 7469 6669 6361 7469 6f6e 536f 7572 6365  tificationSource
-0000faa0: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
-0000fab0: 2c0a 2020 2020 2020 2020 7072 6f63 6573  ,.        proces
-0000fac0: 7369 6e67 5f65 7272 6f72 733a 2062 7569  sing_errors: bui
-0000fad0: 6c74 696e 732e 626f 6f6c 203d 202e 2e2e  ltins.bool = ...
-0000fae0: 2c0a 2020 2020 2020 2020 6d65 7373 6167  ,.        messag
-0000faf0: 655f 6175 6469 743a 2067 6c6f 6261 6c5f  e_audit: global_
-0000fb00: 5f5f 4175 6469 7420 7c20 4e6f 6e65 203d  __Audit | None =
-0000fb10: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-0000fb20: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-0000fb30: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
-0000fb40: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-0000fb50: 6e67 2e4c 6974 6572 616c 5b22 6d65 7373  ng.Literal["mess
-0000fb60: 6167 6522 2c20 6222 6d65 7373 6167 6522  age", b"message"
-0000fb70: 2c20 226d 6573 7361 6765 5f61 7564 6974  , "message_audit
-0000fb80: 222c 2062 226d 6573 7361 6765 5f61 7564  ", b"message_aud
-0000fb90: 6974 225d 2920 2d3e 2062 7569 6c74 696e  it"]) -> builtin
-0000fba0: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
-0000fbb0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-0000fbc0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-0000fbd0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-0000fbe0: 2261 6374 696f 6e22 2c20 6222 6163 7469  "action", b"acti
-0000fbf0: 6f6e 222c 2022 6b62 6964 222c 2062 226b  on", "kbid", b"k
-0000fc00: 6269 6422 2c20 226d 6573 7361 6765 222c  bid", "message",
-0000fc10: 2062 226d 6573 7361 6765 222c 2022 6d65   b"message", "me
-0000fc20: 7373 6167 655f 6175 6469 7422 2c20 6222  ssage_audit", b"
-0000fc30: 6d65 7373 6167 655f 6175 6469 7422 2c20  message_audit", 
-0000fc40: 226d 756c 7469 222c 2062 226d 756c 7469  "multi", b"multi
-0000fc50: 222c 2022 7061 7274 6974 696f 6e22 2c20  ", "partition", 
-0000fc60: 6222 7061 7274 6974 696f 6e22 2c20 2270  b"partition", "p
-0000fc70: 726f 6365 7373 696e 675f 6572 726f 7273  rocessing_errors
-0000fc80: 222c 2062 2270 726f 6365 7373 696e 675f  ", b"processing_
-0000fc90: 6572 726f 7273 222c 2022 7365 7169 6422  errors", "seqid"
-0000fca0: 2c20 6222 7365 7169 6422 2c20 2273 6f75  , b"seqid", "sou
-0000fcb0: 7263 6522 2c20 6222 736f 7572 6365 222c  rce", b"source",
-0000fcc0: 2022 7575 6964 222c 2062 2275 7569 6422   "uuid", b"uuid"
-0000fcd0: 2c20 2277 7269 7465 5f74 7970 6522 2c20  , "write_type", 
-0000fce0: 6222 7772 6974 655f 7479 7065 225d 2920  b"write_type"]) 
-0000fcf0: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
-0000fd00: 6f62 616c 5f5f 5f4e 6f74 6966 6963 6174  obal___Notificat
-0000fd10: 696f 6e20 3d20 4e6f 7469 6669 6361 7469  ion = Notificati
-0000fd20: 6f6e 0a0a 4074 7970 696e 672e 6669 6e61  on..@typing.fina
-0000fd30: 6c0a 636c 6173 7320 4d65 6d62 6572 2867  l.class Member(g
-0000fd40: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
-0000fd50: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
-0000fd60: 0a20 2020 2022 2222 5468 6520 6d65 6d62  .    """The memb
-0000fd70: 6572 2069 6e66 6f72 6d61 7469 6f6e 2e22  er information."
-0000fd80: 2222 0a0a 2020 2020 4445 5343 5249 5054  ""..    DESCRIPT
-0000fd90: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-0000fda0: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-0000fdb0: 6573 6372 6970 746f 720a 0a20 2020 2063  escriptor..    c
-0000fdc0: 6c61 7373 205f 5479 7065 3a0a 2020 2020  lass _Type:.    
-0000fdd0: 2020 2020 5661 6c75 6554 7970 6520 3d20      ValueType = 
-0000fde0: 7479 7069 6e67 2e4e 6577 5479 7065 2822  typing.NewType("
-0000fdf0: 5661 6c75 6554 7970 6522 2c20 6275 696c  ValueType", buil
-0000fe00: 7469 6e73 2e69 6e74 290a 2020 2020 2020  tins.int).      
-0000fe10: 2020 563a 2074 7970 696e 675f 6578 7465    V: typing_exte
-0000fe20: 6e73 696f 6e73 2e54 7970 6541 6c69 6173  nsions.TypeAlias
-0000fe30: 203d 2056 616c 7565 5479 7065 0a0a 2020   = ValueType..  
-0000fe40: 2020 636c 6173 7320 5f54 7970 6545 6e75    class _TypeEnu
-0000fe50: 6d54 7970 6557 7261 7070 6572 2867 6f6f  mTypeWrapper(goo
-0000fe60: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
-0000fe70: 6572 6e61 6c2e 656e 756d 5f74 7970 655f  ernal.enum_type_
-0000fe80: 7772 6170 7065 722e 5f45 6e75 6d54 7970  wrapper._EnumTyp
-0000fe90: 6557 7261 7070 6572 5b4d 656d 6265 722e  eWrapper[Member.
-0000fea0: 5f54 7970 652e 5661 6c75 6554 7970 655d  _Type.ValueType]
-0000feb0: 2c20 6275 696c 7469 6e73 2e74 7970 6529  , builtins.type)
-0000fec0: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
-0000fed0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-0000fee0: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-0000fef0: 2e45 6e75 6d44 6573 6372 6970 746f 720a  .EnumDescriptor.
-0000ff00: 2020 2020 2020 2020 494f 3a20 4d65 6d62          IO: Memb
-0000ff10: 6572 2e5f 5479 7065 2e56 616c 7565 5479  er._Type.ValueTy
-0000ff20: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
-0000ff30: 5345 4152 4348 3a20 4d65 6d62 6572 2e5f  SEARCH: Member._
-0000ff40: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
-0000ff50: 2320 310a 2020 2020 2020 2020 494e 4745  # 1.        INGE
-0000ff60: 5354 3a20 4d65 6d62 6572 2e5f 5479 7065  ST: Member._Type
-0000ff70: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
-0000ff80: 2020 2020 2020 2020 5452 4149 4e3a 204d          TRAIN: M
-0000ff90: 656d 6265 722e 5f54 7970 652e 5661 6c75  ember._Type.Valu
-0000ffa0: 6554 7970 6520 2023 2033 0a20 2020 2020  eType  # 3.     
-0000ffb0: 2020 2055 4e4b 4e4f 574e 3a20 4d65 6d62     UNKNOWN: Memb
-0000ffc0: 6572 2e5f 5479 7065 2e56 616c 7565 5479  er._Type.ValueTy
-0000ffd0: 7065 2020 2320 340a 0a20 2020 2063 6c61  pe  # 4..    cla
-0000ffe0: 7373 2054 7970 6528 5f54 7970 652c 206d  ss Type(_Type, m
-0000fff0: 6574 6163 6c61 7373 3d5f 5479 7065 456e  etaclass=_TypeEn
-00010000: 756d 5479 7065 5772 6170 7065 7229 3a20  umTypeWrapper): 
-00010010: 2e2e 2e0a 2020 2020 494f 3a20 4d65 6d62  ....    IO: Memb
-00010020: 6572 2e54 7970 652e 5661 6c75 6554 7970  er.Type.ValueTyp
-00010030: 6520 2023 2030 0a20 2020 2053 4541 5243  e  # 0.    SEARC
-00010040: 483a 204d 656d 6265 722e 5479 7065 2e56  H: Member.Type.V
-00010050: 616c 7565 5479 7065 2020 2320 310a 2020  alueType  # 1.  
-00010060: 2020 494e 4745 5354 3a20 4d65 6d62 6572    INGEST: Member
-00010070: 2e54 7970 652e 5661 6c75 6554 7970 6520  .Type.ValueType 
-00010080: 2023 2032 0a20 2020 2054 5241 494e 3a20   # 2.    TRAIN: 
-00010090: 4d65 6d62 6572 2e54 7970 652e 5661 6c75  Member.Type.Valu
-000100a0: 6554 7970 6520 2023 2033 0a20 2020 2055  eType  # 3.    U
-000100b0: 4e4b 4e4f 574e 3a20 4d65 6d62 6572 2e54  NKNOWN: Member.T
-000100c0: 7970 652e 5661 6c75 6554 7970 6520 2023  ype.ValueType  #
-000100d0: 2034 0a0a 2020 2020 4944 5f46 4945 4c44   4..    ID_FIELD
-000100e0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-000100f0: 732e 696e 740a 2020 2020 4c49 5354 454e  s.int.    LISTEN
-00010100: 5f41 4444 5245 5353 5f46 4945 4c44 5f4e  _ADDRESS_FIELD_N
-00010110: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00010120: 696e 740a 2020 2020 4953 5f53 454c 465f  int.    IS_SELF_
-00010130: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00010140: 696c 7469 6e73 2e69 6e74 0a20 2020 2054  iltins.int.    T
-00010150: 5950 455f 4649 454c 445f 4e55 4d42 4552  YPE_FIELD_NUMBER
-00010160: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00010170: 2020 2044 554d 4d59 5f46 4945 4c44 5f4e     DUMMY_FIELD_N
-00010180: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00010190: 696e 740a 2020 2020 4c4f 4144 5f53 434f  int.    LOAD_SCO
-000101a0: 5245 5f46 4945 4c44 5f4e 554d 4245 523a  RE_FIELD_NUMBER:
-000101b0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
-000101c0: 2020 5348 4152 445f 434f 554e 545f 4649    SHARD_COUNT_FI
-000101d0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-000101e0: 7469 6e73 2e69 6e74 0a20 2020 2050 5249  tins.int.    PRI
-000101f0: 4d41 5259 5f49 445f 4649 454c 445f 4e55  MARY_ID_FIELD_NU
-00010200: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00010210: 6e74 0a20 2020 2069 643a 2062 7569 6c74  nt.    id: built
-00010220: 696e 732e 7374 720a 2020 2020 2222 222f  ins.str.    """/
-00010230: 204d 656d 6265 7220 4944 2ee3 8080 4120   Member ID....A 
-00010240: 7374 7269 6e67 206f 6620 7468 6520 5555  string of the UU
-00010250: 4944 2e22 2222 0a20 2020 206c 6973 7465  ID.""".    liste
-00010260: 6e5f 6164 6472 6573 733a 2062 7569 6c74  n_address: built
-00010270: 696e 732e 7374 720a 2020 2020 2222 222f  ins.str.    """/
-00010280: 2043 6c75 7374 6572 206c 6973 7465 6e20   Cluster listen 
-00010290: 6164 6472 6573 732e 2073 7472 696e 6720  address. string 
-000102a0: 6f66 2049 5020 616e 6420 706f 7274 206e  of IP and port n
-000102b0: 756d 6265 722e 0a20 2020 202f 2045 2e67  umber..    / E.g
-000102c0: 2e20 3132 372e 302e 302e 313a 3530 3030  . 127.0.0.1:5000
-000102d0: 0a20 2020 2022 2222 0a20 2020 2069 735f  .    """.    is_
-000102e0: 7365 6c66 3a20 6275 696c 7469 6e73 2e62  self: builtins.b
-000102f0: 6f6f 6c0a 2020 2020 2222 222f 2049 6620  ool.    """/ If 
-00010300: 7472 7565 2c20 6974 206d 6561 6e73 2073  true, it means s
-00010310: 656c 662e 2222 220a 2020 2020 7479 7065  elf.""".    type
-00010320: 3a20 676c 6f62 616c 5f5f 5f4d 656d 6265  : global___Membe
-00010330: 722e 5479 7065 2e56 616c 7565 5479 7065  r.Type.ValueType
-00010340: 0a20 2020 2022 2222 2f20 496f 2c20 496e  .    """/ Io, In
-00010350: 6765 7374 2c20 5365 6172 6368 2c20 5472  gest, Search, Tr
-00010360: 6169 6e2e 2222 220a 2020 2020 6475 6d6d  ain.""".    dumm
-00010370: 793a 2062 7569 6c74 696e 732e 626f 6f6c  y: builtins.bool
-00010380: 0a20 2020 2022 2222 2f20 4475 6d6d 7920  .    """/ Dummy 
-00010390: 4d65 6d62 6572 2222 220a 2020 2020 6c6f  Member""".    lo
-000103a0: 6164 5f73 636f 7265 3a20 6275 696c 7469  ad_score: builti
-000103b0: 6e73 2e66 6c6f 6174 0a20 2020 2022 2222  ns.float.    """
-000103c0: 2f20 5468 6520 6c6f 6164 2073 636f 7265  / The load score
-000103d0: 206f 6620 7468 6520 6d65 6d62 6572 2e22   of the member."
-000103e0: 2222 0a20 2020 2073 6861 7264 5f63 6f75  "".    shard_cou
-000103f0: 6e74 3a20 6275 696c 7469 6e73 2e69 6e74  nt: builtins.int
-00010400: 0a20 2020 2022 2222 2f20 5468 6520 6e75  .    """/ The nu
-00010410: 6d62 6572 206f 6620 7368 6172 6473 2069  mber of shards i
-00010420: 6e20 7468 6520 6e6f 6465 2e22 2222 0a20  n the node.""". 
-00010430: 2020 2070 7269 6d61 7279 5f69 643a 2062     primary_id: b
-00010440: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
-00010450: 2222 222f 2054 6865 2069 6420 6f66 2074  """/ The id of t
-00010460: 6865 2070 7269 6d61 7279 206e 6f64 6520  he primary node 
-00010470: 2869 6620 6974 2069 7320 6120 7365 636f  (if it is a seco
-00010480: 6e64 6172 7920 6e6f 6465 292e 2222 220a  ndary node).""".
-00010490: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000104a0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000104b0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-000104c0: 2020 2069 643a 2062 7569 6c74 696e 732e     id: builtins.
-000104d0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-000104e0: 2020 206c 6973 7465 6e5f 6164 6472 6573     listen_addres
-000104f0: 733a 2062 7569 6c74 696e 732e 7374 7220  s: builtins.str 
-00010500: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2069  = ...,.        i
-00010510: 735f 7365 6c66 3a20 6275 696c 7469 6e73  s_self: builtins
-00010520: 2e62 6f6f 6c20 3d20 2e2e 2e2c 0a20 2020  .bool = ...,.   
-00010530: 2020 2020 2074 7970 653a 2067 6c6f 6261       type: globa
-00010540: 6c5f 5f5f 4d65 6d62 6572 2e54 7970 652e  l___Member.Type.
-00010550: 5661 6c75 6554 7970 6520 3d20 2e2e 2e2c  ValueType = ...,
-00010560: 0a20 2020 2020 2020 2064 756d 6d79 3a20  .        dummy: 
-00010570: 6275 696c 7469 6e73 2e62 6f6f 6c20 3d20  builtins.bool = 
-00010580: 2e2e 2e2c 0a20 2020 2020 2020 206c 6f61  ...,.        loa
-00010590: 645f 7363 6f72 653a 2062 7569 6c74 696e  d_score: builtin
-000105a0: 732e 666c 6f61 7420 3d20 2e2e 2e2c 0a20  s.float = ...,. 
-000105b0: 2020 2020 2020 2073 6861 7264 5f63 6f75         shard_cou
-000105c0: 6e74 3a20 6275 696c 7469 6e73 2e69 6e74  nt: builtins.int
-000105d0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-000105e0: 7072 696d 6172 795f 6964 3a20 6275 696c  primary_id: buil
-000105f0: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
-00010600: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
-00010610: 2e2e 0a20 2020 2064 6566 2043 6c65 6172  ...    def Clear
-00010620: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-00010630: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-00010640: 6974 6572 616c 5b22 6475 6d6d 7922 2c20  iteral["dummy", 
-00010650: 6222 6475 6d6d 7922 2c20 2269 6422 2c20  b"dummy", "id", 
-00010660: 6222 6964 222c 2022 6973 5f73 656c 6622  b"id", "is_self"
-00010670: 2c20 6222 6973 5f73 656c 6622 2c20 226c  , b"is_self", "l
-00010680: 6973 7465 6e5f 6164 6472 6573 7322 2c20  isten_address", 
-00010690: 6222 6c69 7374 656e 5f61 6464 7265 7373  b"listen_address
-000106a0: 222c 2022 6c6f 6164 5f73 636f 7265 222c  ", "load_score",
-000106b0: 2062 226c 6f61 645f 7363 6f72 6522 2c20   b"load_score", 
-000106c0: 2270 7269 6d61 7279 5f69 6422 2c20 6222  "primary_id", b"
-000106d0: 7072 696d 6172 795f 6964 222c 2022 7368  primary_id", "sh
-000106e0: 6172 645f 636f 756e 7422 2c20 6222 7368  ard_count", b"sh
-000106f0: 6172 645f 636f 756e 7422 2c20 2274 7970  ard_count", "typ
-00010700: 6522 2c20 6222 7479 7065 225d 2920 2d3e  e", b"type"]) ->
-00010710: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
-00010720: 616c 5f5f 5f4d 656d 6265 7220 3d20 4d65  al___Member = Me
-00010730: 6d62 6572 0a0a 4074 7970 696e 672e 6669  mber..@typing.fi
-00010740: 6e61 6c0a 636c 6173 7320 4c69 7374 4d65  nal.class ListMe
-00010750: 6d62 6572 7352 6571 7565 7374 2867 6f6f  mbersRequest(goo
-00010760: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-00010770: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-00010780: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-00010790: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-000107a0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-000107b0: 7074 6f72 0a0a 2020 2020 6465 6620 5f5f  ptor..    def __
-000107c0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000107d0: 7365 6c66 2c0a 2020 2020 2920 2d3e 204e  self,.    ) -> N
-000107e0: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
-000107f0: 5f5f 5f4c 6973 744d 656d 6265 7273 5265  ___ListMembersRe
-00010800: 7175 6573 7420 3d20 4c69 7374 4d65 6d62  quest = ListMemb
-00010810: 6572 7352 6571 7565 7374 0a0a 4074 7970  ersRequest..@typ
-00010820: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-00010830: 4c69 7374 4d65 6d62 6572 7352 6573 706f  ListMembersRespo
-00010840: 6e73 6528 676f 6f67 6c65 2e70 726f 746f  nse(google.proto
-00010850: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
-00010860: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
-00010870: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-00010880: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-00010890: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
-000108a0: 204d 454d 4245 5253 5f46 4945 4c44 5f4e   MEMBERS_FIELD_N
-000108b0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-000108c0: 696e 740a 2020 2020 4070 726f 7065 7274  int.    @propert
-000108d0: 790a 2020 2020 6465 6620 6d65 6d62 6572  y.    def member
-000108e0: 7328 7365 6c66 2920 2d3e 2067 6f6f 676c  s(self) -> googl
-000108f0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
-00010900: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
-00010910: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
-00010920: 4669 656c 6443 6f6e 7461 696e 6572 5b67  FieldContainer[g
-00010930: 6c6f 6261 6c5f 5f5f 4d65 6d62 6572 5d3a  lobal___Member]:
-00010940: 202e 2e2e 0a20 2020 2064 6566 205f 5f69   ....    def __i
-00010950: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00010960: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
-00010970: 2020 2020 2020 2020 6d65 6d62 6572 733a          members:
-00010980: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
-00010990: 2e49 7465 7261 626c 655b 676c 6f62 616c  .Iterable[global
-000109a0: 5f5f 5f4d 656d 6265 725d 207c 204e 6f6e  ___Member] | Non
-000109b0: 6520 3d20 2e2e 2e2c 0a20 2020 2029 202d  e = ...,.    ) -
-000109c0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020 2020  > None: ....    
-000109d0: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
-000109e0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
-000109f0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
-00010a00: 226d 656d 6265 7273 222c 2062 226d 656d  "members", b"mem
-00010a10: 6265 7273 225d 2920 2d3e 204e 6f6e 653a  bers"]) -> None:
-00010a20: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f4c   .....global___L
-00010a30: 6973 744d 656d 6265 7273 5265 7370 6f6e  istMembersRespon
-00010a40: 7365 203d 204c 6973 744d 656d 6265 7273  se = ListMembers
-00010a50: 5265 7370 6f6e 7365 0a0a 4074 7970 696e  Response..@typin
-00010a60: 672e 6669 6e61 6c0a 636c 6173 7320 5368  g.final.class Sh
-00010a70: 6172 6452 6570 6c69 6361 2867 6f6f 676c  ardReplica(googl
-00010a80: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-00010a90: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-00010aa0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-00010ab0: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-00010ac0: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-00010ad0: 6f72 0a0a 2020 2020 5348 4152 445f 4649  or..    SHARD_FI
-00010ae0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-00010af0: 7469 6e73 2e69 6e74 0a20 2020 204e 4f44  tins.int.    NOD
-00010b00: 455f 4649 454c 445f 4e55 4d42 4552 3a20  E_FIELD_NUMBER: 
-00010b10: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00010b20: 206e 6f64 653a 2062 7569 6c74 696e 732e   node: builtins.
-00010b30: 7374 720a 2020 2020 4070 726f 7065 7274  str.    @propert
-00010b40: 790a 2020 2020 6465 6620 7368 6172 6428  y.    def shard(
-00010b50: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
-00010b60: 625f 7072 6f74 6f73 2e6e 6f64 6572 6573  b_protos.noderes
-00010b70: 6f75 7263 6573 5f70 6232 2e53 6861 7264  ources_pb2.Shard
-00010b80: 4372 6561 7465 643a 202e 2e2e 0a20 2020  Created: ....   
-00010b90: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00010ba0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00010bb0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00010bc0: 7368 6172 643a 206e 7563 6c69 6164 625f  shard: nucliadb_
-00010bd0: 7072 6f74 6f73 2e6e 6f64 6572 6573 6f75  protos.noderesou
-00010be0: 7263 6573 5f70 6232 2e53 6861 7264 4372  rces_pb2.ShardCr
-00010bf0: 6561 7465 6420 7c20 4e6f 6e65 203d 202e  eated | None = .
-00010c00: 2e2e 2c0a 2020 2020 2020 2020 6e6f 6465  ..,.        node
-00010c10: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00010c20: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
-00010c30: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
-00010c40: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
-00010c50: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
-00010c60: 6e67 2e4c 6974 6572 616c 5b22 7368 6172  ng.Literal["shar
-00010c70: 6422 2c20 6222 7368 6172 6422 5d29 202d  d", b"shard"]) -
-00010c80: 3e20 6275 696c 7469 6e73 2e62 6f6f 6c3a  > builtins.bool:
-00010c90: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
-00010ca0: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
-00010cb0: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-00010cc0: 2e4c 6974 6572 616c 5b22 6e6f 6465 222c  .Literal["node",
-00010cd0: 2062 226e 6f64 6522 2c20 2273 6861 7264   b"node", "shard
-00010ce0: 222c 2062 2273 6861 7264 225d 2920 2d3e  ", b"shard"]) ->
-00010cf0: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
-00010d00: 616c 5f5f 5f53 6861 7264 5265 706c 6963  al___ShardReplic
-00010d10: 6120 3d20 5368 6172 6452 6570 6c69 6361  a = ShardReplica
-00010d20: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
-00010d30: 636c 6173 7320 5368 6172 644f 626a 6563  class ShardObjec
-00010d40: 7428 676f 6f67 6c65 2e70 726f 746f 6275  t(google.protobu
-00010d50: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-00010d60: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-00010d70: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-00010d80: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-00010d90: 6573 6372 6970 746f 720a 0a20 2020 2053  escriptor..    S
-00010da0: 4841 5244 5f46 4945 4c44 5f4e 554d 4245  HARD_FIELD_NUMBE
-00010db0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00010dc0: 2020 2020 5245 504c 4943 4153 5f46 4945      REPLICAS_FIE
-00010dd0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00010de0: 696e 732e 696e 740a 2020 2020 5449 4d45  ins.int.    TIME
-00010df0: 5354 414d 505f 4649 454c 445f 4e55 4d42  STAMP_FIELD_NUMB
-00010e00: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
-00010e10: 0a20 2020 2052 4541 445f 4f4e 4c59 5f46  .    READ_ONLY_F
-00010e20: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00010e30: 6c74 696e 732e 696e 740a 2020 2020 7368  ltins.int.    sh
-00010e40: 6172 643a 2062 7569 6c74 696e 732e 7374  ard: builtins.st
-00010e50: 720a 2020 2020 7265 6164 5f6f 6e6c 793a  r.    read_only:
-00010e60: 2062 7569 6c74 696e 732e 626f 6f6c 0a20   builtins.bool. 
-00010e70: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00010e80: 2064 6566 2072 6570 6c69 6361 7328 7365   def replicas(se
-00010e90: 6c66 2920 2d3e 2067 6f6f 676c 652e 7072  lf) -> google.pr
-00010ea0: 6f74 6f62 7566 2e69 6e74 6572 6e61 6c2e  otobuf.internal.
-00010eb0: 636f 6e74 6169 6e65 7273 2e52 6570 6561  containers.Repea
-00010ec0: 7465 6443 6f6d 706f 7369 7465 4669 656c  tedCompositeFiel
-00010ed0: 6443 6f6e 7461 696e 6572 5b67 6c6f 6261  dContainer[globa
-00010ee0: 6c5f 5f5f 5368 6172 6452 6570 6c69 6361  l___ShardReplica
-00010ef0: 5d3a 202e 2e2e 0a20 2020 2040 7072 6f70  ]: ....    @prop
-00010f00: 6572 7479 0a20 2020 2064 6566 2074 696d  erty.    def tim
-00010f10: 6573 7461 6d70 2873 656c 6629 202d 3e20  estamp(self) -> 
-00010f20: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-00010f30: 7469 6d65 7374 616d 705f 7062 322e 5469  timestamp_pb2.Ti
-00010f40: 6d65 7374 616d 703a 202e 2e2e 0a20 2020  mestamp: ....   
-00010f50: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00010f60: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00010f70: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00010f80: 7368 6172 643a 2062 7569 6c74 696e 732e  shard: builtins.
-00010f90: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2020  str = ...,.     
-00010fa0: 2020 2072 6570 6c69 6361 733a 2063 6f6c     replicas: col
-00010fb0: 6c65 6374 696f 6e73 2e61 6263 2e49 7465  lections.abc.Ite
-00010fc0: 7261 626c 655b 676c 6f62 616c 5f5f 5f53  rable[global___S
-00010fd0: 6861 7264 5265 706c 6963 615d 207c 204e  hardReplica] | N
-00010fe0: 6f6e 6520 3d20 2e2e 2e2c 0a20 2020 2020  one = ...,.     
-00010ff0: 2020 2074 696d 6573 7461 6d70 3a20 676f     timestamp: go
-00011000: 6f67 6c65 2e70 726f 746f 6275 662e 7469  ogle.protobuf.ti
-00011010: 6d65 7374 616d 705f 7062 322e 5469 6d65  mestamp_pb2.Time
-00011020: 7374 616d 7020 7c20 4e6f 6e65 203d 202e  stamp | None = .
-00011030: 2e2e 2c0a 2020 2020 2020 2020 7265 6164  ..,.        read
-00011040: 5f6f 6e6c 793a 2062 7569 6c74 696e 732e  _only: builtins.
-00011050: 626f 6f6c 203d 202e 2e2e 2c0a 2020 2020  bool = ...,.    
-00011060: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-00011070: 2020 2064 6566 2048 6173 4669 656c 6428     def HasField(
-00011080: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
-00011090: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
-000110a0: 5b22 7469 6d65 7374 616d 7022 2c20 6222  ["timestamp", b"
-000110b0: 7469 6d65 7374 616d 7022 5d29 202d 3e20  timestamp"]) -> 
-000110c0: 6275 696c 7469 6e73 2e62 6f6f 6c3a 202e  builtins.bool: .
-000110d0: 2e2e 0a20 2020 2064 6566 2043 6c65 6172  ...    def Clear
-000110e0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-000110f0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-00011100: 6974 6572 616c 5b22 7265 6164 5f6f 6e6c  iteral["read_onl
-00011110: 7922 2c20 6222 7265 6164 5f6f 6e6c 7922  y", b"read_only"
-00011120: 2c20 2272 6570 6c69 6361 7322 2c20 6222  , "replicas", b"
-00011130: 7265 706c 6963 6173 222c 2022 7368 6172  replicas", "shar
-00011140: 6422 2c20 6222 7368 6172 6422 2c20 2274  d", b"shard", "t
-00011150: 696d 6573 7461 6d70 222c 2062 2274 696d  imestamp", b"tim
-00011160: 6573 7461 6d70 225d 2920 2d3e 204e 6f6e  estamp"]) -> Non
-00011170: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
-00011180: 5f53 6861 7264 4f62 6a65 6374 203d 2053  _ShardObject = S
-00011190: 6861 7264 4f62 6a65 6374 0a0a 4074 7970  hardObject..@typ
-000111a0: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-000111b0: 5368 6172 6473 2867 6f6f 676c 652e 7072  Shards(google.pr
-000111c0: 6f74 6f62 7566 2e6d 6573 7361 6765 2e4d  otobuf.message.M
-000111d0: 6573 7361 6765 293a 0a20 2020 2044 4553  essage):.    DES
-000111e0: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
-000111f0: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
-00011200: 746f 722e 4465 7363 7269 7074 6f72 0a0a  tor.Descriptor..
-00011210: 2020 2020 4074 7970 696e 672e 6669 6e61      @typing.fina
-00011220: 6c0a 2020 2020 636c 6173 7320 4578 7472  l.    class Extr
-00011230: 6145 6e74 7279 2867 6f6f 676c 652e 7072  aEntry(google.pr
-00011240: 6f74 6f62 7566 2e6d 6573 7361 6765 2e4d  otobuf.message.M
-00011250: 6573 7361 6765 293a 0a20 2020 2020 2020  essage):.       
-00011260: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-00011270: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-00011280: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-00011290: 6f72 0a0a 2020 2020 2020 2020 4b45 595f  or..        KEY_
-000112a0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-000112b0: 696c 7469 6e73 2e69 6e74 0a20 2020 2020  iltins.int.     
-000112c0: 2020 2056 414c 5545 5f46 4945 4c44 5f4e     VALUE_FIELD_N
-000112d0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-000112e0: 696e 740a 2020 2020 2020 2020 6b65 793a  int.        key:
-000112f0: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00011300: 2020 2020 2020 7661 6c75 653a 2062 7569        value: bui
-00011310: 6c74 696e 732e 7374 720a 2020 2020 2020  ltins.str.      
-00011320: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00011330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011340: 2c0a 2020 2020 2020 2020 2020 2020 2a2c  ,.            *,
-00011350: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
-00011360: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
-00011370: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-00011380: 2020 7661 6c75 653a 2062 7569 6c74 696e    value: builtin
-00011390: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-000113a0: 2020 2020 2029 202d 3e20 4e6f 6e65 3a20       ) -> None: 
-000113b0: 2e2e 2e0a 2020 2020 2020 2020 6465 6620  ....        def 
-000113c0: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
-000113d0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-000113e0: 696e 672e 4c69 7465 7261 6c5b 226b 6579  ing.Literal["key
-000113f0: 222c 2062 226b 6579 222c 2022 7661 6c75  ", b"key", "valu
-00011400: 6522 2c20 6222 7661 6c75 6522 5d29 202d  e", b"value"]) -
-00011410: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a20 2020  > None: .....   
-00011420: 2053 4841 5244 535f 4649 454c 445f 4e55   SHARDS_FIELD_NU
-00011430: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00011440: 6e74 0a20 2020 204b 4249 445f 4649 454c  nt.    KBID_FIEL
-00011450: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00011460: 6e73 2e69 6e74 0a20 2020 2041 4354 5541  ns.int.    ACTUA
-00011470: 4c5f 4649 454c 445f 4e55 4d42 4552 3a20  L_FIELD_NUMBER: 
-00011480: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
-00011490: 2053 494d 494c 4152 4954 595f 4649 454c   SIMILARITY_FIEL
-000114a0: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-000114b0: 6e73 2e69 6e74 0a20 2020 204d 4f44 454c  ns.int.    MODEL
-000114c0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-000114d0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-000114e0: 5245 4c45 4153 455f 4348 414e 4e45 4c5f  RELEASE_CHANNEL_
-000114f0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00011500: 696c 7469 6e73 2e69 6e74 0a20 2020 2045  iltins.int.    E
-00011510: 5854 5241 5f46 4945 4c44 5f4e 554d 4245  XTRA_FIELD_NUMBE
-00011520: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00011530: 2020 2020 6b62 6964 3a20 6275 696c 7469      kbid: builti
-00011540: 6e73 2e73 7472 0a20 2020 2061 6374 7561  ns.str.    actua
-00011550: 6c3a 2062 7569 6c74 696e 732e 696e 740a  l: builtins.int.
-00011560: 2020 2020 2222 2244 4550 5245 4341 5445      """DEPRECATE
-00011570: 4420 6120 4b42 206b 6e6f 7720 6361 6e20  D a KB know can 
-00011580: 6861 7665 206d 756c 7469 706c 6520 616c  have multiple al
-00011590: 6976 6520 7368 6172 6473 2061 6e64 2069  ive shards and i
-000115a0: 7320 7472 6163 6b65 6420 696e 0a20 2020  s tracked in.   
-000115b0: 2065 6163 6820 5368 6172 644f 626a 6563   each ShardObjec
-000115c0: 740a 2020 2020 2222 220a 2020 2020 7369  t.    """.    si
-000115d0: 6d69 6c61 7269 7479 3a20 6e75 636c 6961  milarity: nuclia
-000115e0: 6462 5f70 726f 746f 732e 7574 696c 735f  db_protos.utils_
-000115f0: 7062 322e 5665 6374 6f72 5369 6d69 6c61  pb2.VectorSimila
-00011600: 7269 7479 2e56 616c 7565 5479 7065 0a20  rity.ValueType. 
-00011610: 2020 2022 2222 4445 5052 4543 4154 4544     """DEPRECATED
-00011620: 2069 6e20 6661 766f 7220 6f66 2060 6d6f   in favor of `mo
-00011630: 6465 6c60 2074 6f20 696e 636c 7564 6520  del` to include 
-00011640: 6d6f 7265 2064 6174 6122 2222 0a20 2020  more data""".   
-00011650: 2072 656c 6561 7365 5f63 6861 6e6e 656c   release_channel
-00011660: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
-00011670: 732e 7574 696c 735f 7062 322e 5265 6c65  s.utils_pb2.Rele
-00011680: 6173 6543 6861 6e6e 656c 2e56 616c 7565  aseChannel.Value
-00011690: 5479 7065 0a20 2020 2040 7072 6f70 6572  Type.    @proper
-000116a0: 7479 0a20 2020 2064 6566 2073 6861 7264  ty.    def shard
-000116b0: 7328 7365 6c66 2920 2d3e 2067 6f6f 676c  s(self) -> googl
-000116c0: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
-000116d0: 6e61 6c2e 636f 6e74 6169 6e65 7273 2e52  nal.containers.R
-000116e0: 6570 6561 7465 6443 6f6d 706f 7369 7465  epeatedComposite
-000116f0: 4669 656c 6443 6f6e 7461 696e 6572 5b67  FieldContainer[g
-00011700: 6c6f 6261 6c5f 5f5f 5368 6172 644f 626a  lobal___ShardObj
-00011710: 6563 745d 3a20 2e2e 2e0a 2020 2020 4070  ect]: ....    @p
-00011720: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00011730: 6d6f 6465 6c28 7365 6c66 2920 2d3e 206e  model(self) -> n
-00011740: 7563 6c69 6164 625f 7072 6f74 6f73 2e6b  ucliadb_protos.k
-00011750: 6e6f 776c 6564 6765 626f 785f 7062 322e  nowledgebox_pb2.
-00011760: 5365 6d61 6e74 6963 4d6f 6465 6c4d 6574  SemanticModelMet
-00011770: 6164 6174 613a 202e 2e2e 0a20 2020 2040  adata: ....    @
-00011780: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00011790: 2065 7874 7261 2873 656c 6629 202d 3e20   extra(self) -> 
-000117a0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
-000117b0: 696e 7465 726e 616c 2e63 6f6e 7461 696e  internal.contain
-000117c0: 6572 732e 5363 616c 6172 4d61 705b 6275  ers.ScalarMap[bu
-000117d0: 696c 7469 6e73 2e73 7472 2c20 6275 696c  iltins.str, buil
-000117e0: 7469 6e73 2e73 7472 5d3a 202e 2e2e 0a20  tins.str]: .... 
-000117f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00011800: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00011810: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00011820: 2020 7368 6172 6473 3a20 636f 6c6c 6563    shards: collec
-00011830: 7469 6f6e 732e 6162 632e 4974 6572 6162  tions.abc.Iterab
-00011840: 6c65 5b67 6c6f 6261 6c5f 5f5f 5368 6172  le[global___Shar
-00011850: 644f 626a 6563 745d 207c 204e 6f6e 6520  dObject] | None 
-00011860: 3d20 2e2e 2e2c 0a20 2020 2020 2020 206b  = ...,.        k
-00011870: 6269 643a 2062 7569 6c74 696e 732e 7374  bid: builtins.st
-00011880: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
-00011890: 2061 6374 7561 6c3a 2062 7569 6c74 696e   actual: builtin
-000118a0: 732e 696e 7420 3d20 2e2e 2e2c 0a20 2020  s.int = ...,.   
-000118b0: 2020 2020 2073 696d 696c 6172 6974 793a       similarity:
-000118c0: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
-000118d0: 2e75 7469 6c73 5f70 6232 2e56 6563 746f  .utils_pb2.Vecto
-000118e0: 7253 696d 696c 6172 6974 792e 5661 6c75  rSimilarity.Valu
-000118f0: 6554 7970 6520 3d20 2e2e 2e2c 0a20 2020  eType = ...,.   
-00011900: 2020 2020 206d 6f64 656c 3a20 6e75 636c       model: nucl
-00011910: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
-00011920: 6c65 6467 6562 6f78 5f70 6232 2e53 656d  ledgebox_pb2.Sem
-00011930: 616e 7469 634d 6f64 656c 4d65 7461 6461  anticModelMetada
-00011940: 7461 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ta | None = ...,
-00011950: 0a20 2020 2020 2020 2072 656c 6561 7365  .        release
-00011960: 5f63 6861 6e6e 656c 3a20 6e75 636c 6961  _channel: nuclia
-00011970: 6462 5f70 726f 746f 732e 7574 696c 735f  db_protos.utils_
-00011980: 7062 322e 5265 6c65 6173 6543 6861 6e6e  pb2.ReleaseChann
-00011990: 656c 2e56 616c 7565 5479 7065 203d 202e  el.ValueType = .
-000119a0: 2e2e 2c0a 2020 2020 2020 2020 6578 7472  ..,.        extr
-000119b0: 613a 2063 6f6c 6c65 6374 696f 6e73 2e61  a: collections.a
-000119c0: 6263 2e4d 6170 7069 6e67 5b62 7569 6c74  bc.Mapping[built
-000119d0: 696e 732e 7374 722c 2062 7569 6c74 696e  ins.str, builtin
-000119e0: 732e 7374 725d 207c 204e 6f6e 6520 3d20  s.str] | None = 
-000119f0: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
-00011a00: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00011a10: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
-00011a20: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-00011a30: 672e 4c69 7465 7261 6c5b 226d 6f64 656c  g.Literal["model
-00011a40: 222c 2062 226d 6f64 656c 225d 2920 2d3e  ", b"model"]) ->
-00011a50: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
-00011a60: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
-00011a70: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
-00011a80: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
-00011a90: 4c69 7465 7261 6c5b 2261 6374 7561 6c22  Literal["actual"
-00011aa0: 2c20 6222 6163 7475 616c 222c 2022 6578  , b"actual", "ex
-00011ab0: 7472 6122 2c20 6222 6578 7472 6122 2c20  tra", b"extra", 
-00011ac0: 226b 6269 6422 2c20 6222 6b62 6964 222c  "kbid", b"kbid",
-00011ad0: 2022 6d6f 6465 6c22 2c20 6222 6d6f 6465   "model", b"mode
-00011ae0: 6c22 2c20 2272 656c 6561 7365 5f63 6861  l", "release_cha
-00011af0: 6e6e 656c 222c 2062 2272 656c 6561 7365  nnel", b"release
-00011b00: 5f63 6861 6e6e 656c 222c 2022 7368 6172  _channel", "shar
-00011b10: 6473 222c 2062 2273 6861 7264 7322 2c20  ds", b"shards", 
-00011b20: 2273 696d 696c 6172 6974 7922 2c20 6222  "similarity", b"
-00011b30: 7369 6d69 6c61 7269 7479 225d 2920 2d3e  similarity"]) ->
-00011b40: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
-00011b50: 616c 5f5f 5f53 6861 7264 7320 3d20 5368  al___Shards = Sh
-00011b60: 6172 6473 0a0a 4074 7970 696e 672e 6669  ards..@typing.fi
-00011b70: 6e61 6c0a 636c 6173 7320 496e 6465 7852  nal.class IndexR
-00011b80: 6573 6f75 7263 6528 676f 6f67 6c65 2e70  esource(google.p
-00011b90: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-00011ba0: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-00011bb0: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00011bc0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00011bd0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-00011be0: 0a20 2020 204b 4249 445f 4649 454c 445f  .    KBID_FIELD_
-00011bf0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
-00011c00: 2e69 6e74 0a20 2020 2052 4944 5f46 4945  .int.    RID_FIE
-00011c10: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00011c20: 696e 732e 696e 740a 2020 2020 5245 494e  ins.int.    REIN
-00011c30: 4445 585f 5645 4354 4f52 535f 4649 454c  DEX_VECTORS_FIEL
-00011c40: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
-00011c50: 6e73 2e69 6e74 0a20 2020 206b 6269 643a  ns.int.    kbid:
-00011c60: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00011c70: 2020 7269 643a 2062 7569 6c74 696e 732e    rid: builtins.
-00011c80: 7374 720a 2020 2020 7265 696e 6465 785f  str.    reindex_
-00011c90: 7665 6374 6f72 733a 2062 7569 6c74 696e  vectors: builtin
-00011ca0: 732e 626f 6f6c 0a20 2020 2064 6566 205f  s.bool.    def _
-00011cb0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00011cc0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-00011cd0: 2c0a 2020 2020 2020 2020 6b62 6964 3a20  ,.        kbid: 
-00011ce0: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
-00011cf0: 2e2e 2c0a 2020 2020 2020 2020 7269 643a  ..,.        rid:
-00011d00: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
-00011d10: 2e2e 2e2c 0a20 2020 2020 2020 2072 6569  ...,.        rei
-00011d20: 6e64 6578 5f76 6563 746f 7273 3a20 6275  ndex_vectors: bu
-00011d30: 696c 7469 6e73 2e62 6f6f 6c20 3d20 2e2e  iltins.bool = ..
-00011d40: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
-00011d50: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
-00011d60: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
-00011d70: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-00011d80: 672e 4c69 7465 7261 6c5b 226b 6269 6422  g.Literal["kbid"
-00011d90: 2c20 6222 6b62 6964 222c 2022 7265 696e  , b"kbid", "rein
-00011da0: 6465 785f 7665 6374 6f72 7322 2c20 6222  dex_vectors", b"
-00011db0: 7265 696e 6465 785f 7665 6374 6f72 7322  reindex_vectors"
-00011dc0: 2c20 2272 6964 222c 2062 2272 6964 225d  , "rid", b"rid"]
-00011dd0: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a0a  ) -> None: .....
-00011de0: 676c 6f62 616c 5f5f 5f49 6e64 6578 5265  global___IndexRe
-00011df0: 736f 7572 6365 203d 2049 6e64 6578 5265  source = IndexRe
-00011e00: 736f 7572 6365 0a0a 4074 7970 696e 672e  source..@typing.
-00011e10: 6669 6e61 6c0a 636c 6173 7320 496e 6465  final.class Inde
-00011e20: 7853 7461 7475 7328 676f 6f67 6c65 2e70  xStatus(google.p
-00011e30: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
-00011e40: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
-00011e50: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
-00011e60: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
-00011e70: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
-00011e80: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00011e90: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00011ea0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
-00011eb0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 496e  .....global___In
-00011ec0: 6465 7853 7461 7475 7320 3d20 496e 6465  dexStatus = Inde
-00011ed0: 7853 7461 7475 730a 0a40 7479 7069 6e67  xStatus..@typing
-00011ee0: 2e66 696e 616c 0a63 6c61 7373 2053 6574  .final.class Set
-00011ef0: 5665 6374 6f72 7352 6571 7565 7374 2867  VectorsRequest(g
-00011f00: 6f6f 676c 652e 7072 6f74 6f62 7566 2e6d  oogle.protobuf.m
-00011f10: 6573 7361 6765 2e4d 6573 7361 6765 293a  essage.Message):
-00011f20: 0a20 2020 2044 4553 4352 4950 544f 523a  .    DESCRIPTOR:
-00011f30: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
-00011f40: 2e64 6573 6372 6970 746f 722e 4465 7363  .descriptor.Desc
-00011f50: 7269 7074 6f72 0a0a 2020 2020 5645 4354  riptor..    VECT
-00011f60: 4f52 535f 4649 454c 445f 4e55 4d42 4552  ORS_FIELD_NUMBER
-00011f70: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00011f80: 2020 204b 4249 445f 4649 454c 445f 4e55     KBID_FIELD_NU
-00011f90: 4d42 4552 3a20 6275 696c 7469 6e73 2e69  MBER: builtins.i
-00011fa0: 6e74 0a20 2020 2052 4944 5f46 4945 4c44  nt.    RID_FIELD
-00011fb0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
-00011fc0: 732e 696e 740a 2020 2020 4649 454c 445f  s.int.    FIELD_
-00011fd0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
-00011fe0: 696c 7469 6e73 2e69 6e74 0a20 2020 206b  iltins.int.    k
-00011ff0: 6269 643a 2062 7569 6c74 696e 732e 7374  bid: builtins.st
-00012000: 720a 2020 2020 7269 643a 2062 7569 6c74  r.    rid: built
-00012010: 696e 732e 7374 720a 2020 2020 4070 726f  ins.str.    @pro
-00012020: 7065 7274 790a 2020 2020 6465 6620 7665  perty.    def ve
-00012030: 6374 6f72 7328 7365 6c66 2920 2d3e 206e  ctors(self) -> n
-00012040: 7563 6c69 6164 625f 7072 6f74 6f73 2e75  ucliadb_protos.u
-00012050: 7469 6c73 5f70 6232 2e56 6563 746f 724f  tils_pb2.VectorO
-00012060: 626a 6563 743a 202e 2e2e 0a20 2020 2040  bject: ....    @
-00012070: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00012080: 2066 6965 6c64 2873 656c 6629 202d 3e20   field(self) -> 
-00012090: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
-000120a0: 7265 736f 7572 6365 735f 7062 322e 4669  resources_pb2.Fi
-000120b0: 656c 6449 443a 202e 2e2e 0a20 2020 2064  eldID: ....    d
-000120c0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-000120d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000120e0: 2020 202a 2c0a 2020 2020 2020 2020 7665     *,.        ve
-000120f0: 6374 6f72 733a 206e 7563 6c69 6164 625f  ctors: nucliadb_
-00012100: 7072 6f74 6f73 2e75 7469 6c73 5f70 6232  protos.utils_pb2
-00012110: 2e56 6563 746f 724f 626a 6563 7420 7c20  .VectorObject | 
-00012120: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
-00012130: 2020 2020 6b62 6964 3a20 6275 696c 7469      kbid: builti
-00012140: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00012150: 2020 2020 2020 7269 643a 2062 7569 6c74        rid: built
-00012160: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-00012170: 2020 2020 2020 2066 6965 6c64 3a20 6e75         field: nu
-00012180: 636c 6961 6462 5f70 726f 746f 732e 7265  cliadb_protos.re
-00012190: 736f 7572 6365 735f 7062 322e 4669 656c  sources_pb2.Fiel
-000121a0: 6449 4420 7c20 4e6f 6e65 203d 202e 2e2e  dID | None = ...
-000121b0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-000121c0: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
-000121d0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-000121e0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-000121f0: 6974 6572 616c 5b22 6669 656c 6422 2c20  iteral["field", 
-00012200: 6222 6669 656c 6422 2c20 2276 6563 746f  b"field", "vecto
-00012210: 7273 222c 2062 2276 6563 746f 7273 225d  rs", b"vectors"]
-00012220: 2920 2d3e 2062 7569 6c74 696e 732e 626f  ) -> builtins.bo
-00012230: 6f6c 3a20 2e2e 2e0a 2020 2020 6465 6620  ol: ....    def 
-00012240: 436c 6561 7246 6965 6c64 2873 656c 662c  ClearField(self,
-00012250: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
-00012260: 696e 672e 4c69 7465 7261 6c5b 2266 6965  ing.Literal["fie
-00012270: 6c64 222c 2062 2266 6965 6c64 222c 2022  ld", b"field", "
-00012280: 6b62 6964 222c 2062 226b 6269 6422 2c20  kbid", b"kbid", 
-00012290: 2272 6964 222c 2062 2272 6964 222c 2022  "rid", b"rid", "
-000122a0: 7665 6374 6f72 7322 2c20 6222 7665 6374  vectors", b"vect
-000122b0: 6f72 7322 5d29 202d 3e20 4e6f 6e65 3a20  ors"]) -> None: 
-000122c0: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 5365  .....global___Se
-000122d0: 7456 6563 746f 7273 5265 7175 6573 7420  tVectorsRequest 
-000122e0: 3d20 5365 7456 6563 746f 7273 5265 7175  = SetVectorsRequ
-000122f0: 6573 740a 0a40 7479 7069 6e67 2e66 696e  est..@typing.fin
-00012300: 616c 0a63 6c61 7373 2053 6574 5665 6374  al.class SetVect
-00012310: 6f72 7352 6573 706f 6e73 6528 676f 6f67  orsResponse(goog
-00012320: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-00012330: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-00012340: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-00012350: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-00012360: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-00012370: 746f 720a 0a20 2020 2046 4f55 4e44 5f46  tor..    FOUND_F
-00012380: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
-00012390: 6c74 696e 732e 696e 740a 2020 2020 666f  ltins.int.    fo
-000123a0: 756e 643a 2062 7569 6c74 696e 732e 626f  und: builtins.bo
-000123b0: 6f6c 0a20 2020 2064 6566 205f 5f69 6e69  ol.    def __ini
-000123c0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000123d0: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-000123e0: 2020 2020 2020 666f 756e 643a 2062 7569        found: bui
-000123f0: 6c74 696e 732e 626f 6f6c 203d 202e 2e2e  ltins.bool = ...
-00012400: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00012410: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
-00012420: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
-00012430: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-00012440: 2e4c 6974 6572 616c 5b22 666f 756e 6422  .Literal["found"
-00012450: 2c20 6222 666f 756e 6422 5d29 202d 3e20  , b"found"]) -> 
-00012460: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
-00012470: 6c5f 5f5f 5365 7456 6563 746f 7273 5265  l___SetVectorsRe
-00012480: 7370 6f6e 7365 203d 2053 6574 5665 6374  sponse = SetVect
-00012490: 6f72 7352 6573 706f 6e73 650a 0a40 7479  orsResponse..@ty
-000124a0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
-000124b0: 2046 696c 6552 6571 7565 7374 2867 6f6f   FileRequest(goo
-000124c0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
-000124d0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
-000124e0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
-000124f0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
-00012500: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
-00012510: 7074 6f72 0a0a 2020 2020 4255 434b 4554  ptor..    BUCKET
-00012520: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-00012530: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-00012540: 4b45 595f 4649 454c 445f 4e55 4d42 4552  KEY_FIELD_NUMBER
-00012550: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00012560: 2020 2062 7563 6b65 743a 2062 7569 6c74     bucket: built
-00012570: 696e 732e 7374 720a 2020 2020 6b65 793a  ins.str.    key:
-00012580: 2062 7569 6c74 696e 732e 7374 720a 2020   builtins.str.  
-00012590: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000125a0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000125b0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-000125c0: 2062 7563 6b65 743a 2062 7569 6c74 696e   bucket: builtin
-000125d0: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
-000125e0: 2020 2020 206b 6579 3a20 6275 696c 7469       key: builti
-000125f0: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
-00012600: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
-00012610: 0a20 2020 2064 6566 2043 6c65 6172 4669  .    def ClearFi
-00012620: 656c 6428 7365 6c66 2c20 6669 656c 645f  eld(self, field_
-00012630: 6e61 6d65 3a20 7479 7069 6e67 2e4c 6974  name: typing.Lit
-00012640: 6572 616c 5b22 6275 636b 6574 222c 2062  eral["bucket", b
-00012650: 2262 7563 6b65 7422 2c20 226b 6579 222c  "bucket", "key",
-00012660: 2062 226b 6579 225d 2920 2d3e 204e 6f6e   b"key"]) -> Non
-00012670: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
-00012680: 5f46 696c 6552 6571 7565 7374 203d 2046  _FileRequest = F
-00012690: 696c 6552 6571 7565 7374 0a0a 4074 7970  ileRequest..@typ
-000126a0: 696e 672e 6669 6e61 6c0a 636c 6173 7320  ing.final.class 
-000126b0: 4269 6e61 7279 4461 7461 2867 6f6f 676c  BinaryData(googl
-000126c0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-000126d0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-000126e0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-000126f0: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-00012700: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-00012710: 6f72 0a0a 2020 2020 4441 5441 5f46 4945  or..    DATA_FIE
-00012720: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00012730: 696e 732e 696e 740a 2020 2020 6461 7461  ins.int.    data
-00012740: 3a20 6275 696c 7469 6e73 2e62 7974 6573  : builtins.bytes
-00012750: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00012760: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00012770: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-00012780: 2020 2020 6461 7461 3a20 6275 696c 7469      data: builti
-00012790: 6e73 2e62 7974 6573 203d 202e 2e2e 2c0a  ns.bytes = ...,.
-000127a0: 2020 2020 2920 2d3e 204e 6f6e 653a 202e      ) -> None: .
-000127b0: 2e2e 0a20 2020 2064 6566 2043 6c65 6172  ...    def Clear
-000127c0: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
-000127d0: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
-000127e0: 6974 6572 616c 5b22 6461 7461 222c 2062  iteral["data", b
-000127f0: 2264 6174 6122 5d29 202d 3e20 4e6f 6e65  "data"]) -> None
-00012800: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
-00012810: 4269 6e61 7279 4461 7461 203d 2042 696e  BinaryData = Bin
-00012820: 6172 7944 6174 610a 0a40 7479 7069 6e67  aryData..@typing
-00012830: 2e66 696e 616c 0a63 6c61 7373 2042 696e  .final.class Bin
-00012840: 6172 794d 6574 6164 6174 6128 676f 6f67  aryMetadata(goog
-00012850: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
-00012860: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
-00012870: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
-00012880: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
-00012890: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
-000128a0: 746f 720a 0a20 2020 204b 4249 445f 4649  tor..    KBID_FI
-000128b0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
-000128c0: 7469 6e73 2e69 6e74 0a20 2020 204b 4559  tins.int.    KEY
-000128d0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
-000128e0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
-000128f0: 5349 5a45 5f46 4945 4c44 5f4e 554d 4245  SIZE_FIELD_NUMBE
-00012900: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00012910: 2020 2020 4649 4c45 4e41 4d45 5f46 4945      FILENAME_FIE
-00012920: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00012930: 696e 732e 696e 740a 2020 2020 434f 4e54  ins.int.    CONT
-00012940: 454e 545f 5459 5045 5f46 4945 4c44 5f4e  ENT_TYPE_FIELD_N
-00012950: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
-00012960: 696e 740a 2020 2020 6b62 6964 3a20 6275  int.    kbid: bu
-00012970: 696c 7469 6e73 2e73 7472 0a20 2020 206b  iltins.str.    k
-00012980: 6579 3a20 6275 696c 7469 6e73 2e73 7472  ey: builtins.str
-00012990: 0a20 2020 2073 697a 653a 2062 7569 6c74  .    size: built
-000129a0: 696e 732e 696e 740a 2020 2020 6669 6c65  ins.int.    file
-000129b0: 6e61 6d65 3a20 6275 696c 7469 6e73 2e73  name: builtins.s
-000129c0: 7472 0a20 2020 2063 6f6e 7465 6e74 5f74  tr.    content_t
-000129d0: 7970 653a 2062 7569 6c74 696e 732e 7374  ype: builtins.st
-000129e0: 720a 2020 2020 6465 6620 5f5f 696e 6974  r.    def __init
-000129f0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00012a00: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
-00012a10: 2020 2020 206b 6269 643a 2062 7569 6c74       kbid: built
-00012a20: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
-00012a30: 2020 2020 2020 206b 6579 3a20 6275 696c         key: buil
-00012a40: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
-00012a50: 2020 2020 2020 2020 7369 7a65 3a20 6275          size: bu
-00012a60: 696c 7469 6e73 2e69 6e74 203d 202e 2e2e  iltins.int = ...
-00012a70: 2c0a 2020 2020 2020 2020 6669 6c65 6e61  ,.        filena
-00012a80: 6d65 3a20 6275 696c 7469 6e73 2e73 7472  me: builtins.str
-00012a90: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
-00012aa0: 636f 6e74 656e 745f 7479 7065 3a20 6275  content_type: bu
-00012ab0: 696c 7469 6e73 2e73 7472 203d 202e 2e2e  iltins.str = ...
-00012ac0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-00012ad0: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
-00012ae0: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
-00012af0: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
-00012b00: 2e4c 6974 6572 616c 5b22 636f 6e74 656e  .Literal["conten
-00012b10: 745f 7479 7065 222c 2062 2263 6f6e 7465  t_type", b"conte
-00012b20: 6e74 5f74 7970 6522 2c20 2266 696c 656e  nt_type", "filen
-00012b30: 616d 6522 2c20 6222 6669 6c65 6e61 6d65  ame", b"filename
-00012b40: 222c 2022 6b62 6964 222c 2062 226b 6269  ", "kbid", b"kbi
-00012b50: 6422 2c20 226b 6579 222c 2062 226b 6579  d", "key", b"key
-00012b60: 222c 2022 7369 7a65 222c 2062 2273 697a  ", "size", b"siz
-00012b70: 6522 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  e"]) -> None: ..
-00012b80: 2e0a 0a67 6c6f 6261 6c5f 5f5f 4269 6e61  ...global___Bina
-00012b90: 7279 4d65 7461 6461 7461 203d 2042 696e  ryMetadata = Bin
-00012ba0: 6172 794d 6574 6164 6174 610a 0a40 7479  aryMetadata..@ty
-00012bb0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
-00012bc0: 2055 706c 6f61 6442 696e 6172 7944 6174   UploadBinaryDat
-00012bd0: 6128 676f 6f67 6c65 2e70 726f 746f 6275  a(google.protobu
-00012be0: 662e 6d65 7373 6167 652e 4d65 7373 6167  f.message.Messag
-00012bf0: 6529 3a0a 2020 2020 4445 5343 5249 5054  e):.    DESCRIPT
-00012c00: 4f52 3a20 676f 6f67 6c65 2e70 726f 746f  OR: google.proto
-00012c10: 6275 662e 6465 7363 7269 7074 6f72 2e44  buf.descriptor.D
-00012c20: 6573 6372 6970 746f 720a 0a20 2020 2043  escriptor..    C
-00012c30: 4f55 4e54 5f46 4945 4c44 5f4e 554d 4245  OUNT_FIELD_NUMBE
-00012c40: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
-00012c50: 2020 2020 4d45 5441 4441 5441 5f46 4945      METADATA_FIE
-00012c60: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00012c70: 696e 732e 696e 740a 2020 2020 5041 594c  ins.int.    PAYL
-00012c80: 4f41 445f 4649 454c 445f 4e55 4d42 4552  OAD_FIELD_NUMBER
-00012c90: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
-00012ca0: 2020 2063 6f75 6e74 3a20 6275 696c 7469     count: builti
-00012cb0: 6e73 2e69 6e74 0a20 2020 2070 6179 6c6f  ns.int.    paylo
-00012cc0: 6164 3a20 6275 696c 7469 6e73 2e62 7974  ad: builtins.byt
-00012cd0: 6573 0a20 2020 2040 7072 6f70 6572 7479  es.    @property
-00012ce0: 0a20 2020 2064 6566 206d 6574 6164 6174  .    def metadat
-00012cf0: 6128 7365 6c66 2920 2d3e 2067 6c6f 6261  a(self) -> globa
-00012d00: 6c5f 5f5f 4269 6e61 7279 4d65 7461 6461  l___BinaryMetada
-00012d10: 7461 3a20 2e2e 2e0a 2020 2020 6465 6620  ta: ....    def 
-00012d20: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00012d30: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00012d40: 2a2c 0a20 2020 2020 2020 2063 6f75 6e74  *,.        count
-00012d50: 3a20 6275 696c 7469 6e73 2e69 6e74 203d  : builtins.int =
-00012d60: 202e 2e2e 2c0a 2020 2020 2020 2020 6d65   ...,.        me
-00012d70: 7461 6461 7461 3a20 676c 6f62 616c 5f5f  tadata: global__
-00012d80: 5f42 696e 6172 794d 6574 6164 6174 6120  _BinaryMetadata 
-00012d90: 7c20 4e6f 6e65 203d 202e 2e2e 2c0a 2020  | None = ...,.  
-00012da0: 2020 2020 2020 7061 796c 6f61 643a 2062        payload: b
-00012db0: 7569 6c74 696e 732e 6279 7465 7320 3d20  uiltins.bytes = 
-00012dc0: 2e2e 2e2c 0a20 2020 2029 202d 3e20 4e6f  ...,.    ) -> No
-00012dd0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00012de0: 4861 7346 6965 6c64 2873 656c 662c 2066  HasField(self, f
-00012df0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
-00012e00: 672e 4c69 7465 7261 6c5b 2264 6174 6122  g.Literal["data"
-00012e10: 2c20 6222 6461 7461 222c 2022 6d65 7461  , b"data", "meta
-00012e20: 6461 7461 222c 2062 226d 6574 6164 6174  data", b"metadat
-00012e30: 6122 2c20 2270 6179 6c6f 6164 222c 2062  a", "payload", b
-00012e40: 2270 6179 6c6f 6164 225d 2920 2d3e 2062  "payload"]) -> b
-00012e50: 7569 6c74 696e 732e 626f 6f6c 3a20 2e2e  uiltins.bool: ..
-00012e60: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
-00012e70: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
-00012e80: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
-00012e90: 7465 7261 6c5b 2263 6f75 6e74 222c 2062  teral["count", b
-00012ea0: 2263 6f75 6e74 222c 2022 6461 7461 222c  "count", "data",
-00012eb0: 2062 2264 6174 6122 2c20 226d 6574 6164   b"data", "metad
-00012ec0: 6174 6122 2c20 6222 6d65 7461 6461 7461  ata", b"metadata
-00012ed0: 222c 2022 7061 796c 6f61 6422 2c20 6222  ", "payload", b"
-00012ee0: 7061 796c 6f61 6422 5d29 202d 3e20 4e6f  payload"]) -> No
-00012ef0: 6e65 3a20 2e2e 2e0a 2020 2020 6465 6620  ne: ....    def 
-00012f00: 5768 6963 684f 6e65 6f66 2873 656c 662c  WhichOneof(self,
-00012f10: 206f 6e65 6f66 5f67 726f 7570 3a20 7479   oneof_group: ty
-00012f20: 7069 6e67 2e4c 6974 6572 616c 5b22 6461  ping.Literal["da
-00012f30: 7461 222c 2062 2264 6174 6122 5d29 202d  ta", b"data"]) -
-00012f40: 3e20 7479 7069 6e67 2e4c 6974 6572 616c  > typing.Literal
-00012f50: 5b22 6d65 7461 6461 7461 222c 2022 7061  ["metadata", "pa
-00012f60: 796c 6f61 6422 5d20 7c20 4e6f 6e65 3a20  yload"] | None: 
-00012f70: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 5570  .....global___Up
-00012f80: 6c6f 6164 4269 6e61 7279 4461 7461 203d  loadBinaryData =
-00012f90: 2055 706c 6f61 6442 696e 6172 7944 6174   UploadBinaryDat
-00012fa0: 610a 0a40 7479 7069 6e67 2e66 696e 616c  a..@typing.final
-00012fb0: 0a63 6c61 7373 2046 696c 6555 706c 6f61  .class FileUploa
-00012fc0: 6465 6428 676f 6f67 6c65 2e70 726f 746f  ded(google.proto
-00012fd0: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
-00012fe0: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
-00012ff0: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
-00013000: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
-00013010: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
-00013020: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00013030: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00013040: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
-00013050: 0a67 6c6f 6261 6c5f 5f5f 4669 6c65 5570  .global___FileUp
-00013060: 6c6f 6164 6564 203d 2046 696c 6555 706c  loaded = FileUpl
-00013070: 6f61 6465 640a 0a40 7479 7069 6e67 2e66  oaded..@typing.f
-00013080: 696e 616c 0a63 6c61 7373 2053 796e 6f6e  inal.class Synon
-00013090: 796d 7352 6571 7565 7374 2867 6f6f 676c  ymsRequest(googl
-000130a0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
-000130b0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
-000130c0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
-000130d0: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
-000130e0: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
-000130f0: 6f72 0a0a 2020 2020 4b42 4944 5f46 4945  or..    KBID_FIE
-00013100: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
-00013110: 696e 732e 696e 740a 2020 2020 6b62 6964  ins.int.    kbid
-00013120: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
-00013130: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00013140: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00013150: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00013160: 2020 6b62 6964 3a20 6275 696c 7469 6e73    kbid: builtins
-00013170: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
-00013180: 2920 2d3e 204e 6f6e 653a 202e 2e2e 0a20  ) -> None: .... 
-00013190: 2020 2064 6566 2043 6c65 6172 4669 656c     def ClearFiel
-000131a0: 6428 7365 6c66 2c20 6669 656c 645f 6e61  d(self, field_na
-000131b0: 6d65 3a20 7479 7069 6e67 2e4c 6974 6572  me: typing.Liter
-000131c0: 616c 5b22 6b62 6964 222c 2062 226b 6269  al["kbid", b"kbi
-000131d0: 6422 5d29 202d 3e20 4e6f 6e65 3a20 2e2e  d"]) -> None: ..
-000131e0: 2e0a 0a67 6c6f 6261 6c5f 5f5f 5379 6e6f  ...global___Syno
-000131f0: 6e79 6d73 5265 7175 6573 7420 3d20 5379  nymsRequest = Sy
-00013200: 6e6f 6e79 6d73 5265 7175 6573 740a       nonymsRequest.
+0000ba40: 6e73 2e69 6e74 0a20 2020 2053 5441 5455  ns.int.    STATU
+0000ba50: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
+0000ba60: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000ba70: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
+0000ba80: 5f5f 4765 744c 6162 656c 7352 6573 706f  __GetLabelsRespo
+0000ba90: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+0000baa0: 5479 7065 0a20 2020 2040 7072 6f70 6572  Type.    @proper
+0000bab0: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
+0000bac0: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
+0000bad0: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+0000bae0: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
+0000baf0: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
+0000bb00: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000bb10: 6620 6c61 6265 6c73 2873 656c 6629 202d  f labels(self) -
+0000bb20: 3e20 6e75 636c 6961 6462 5f70 726f 746f  > nucliadb_proto
+0000bb30: 732e 6b6e 6f77 6c65 6467 6562 6f78 5f70  s.knowledgebox_p
+0000bb40: 6232 2e4c 6162 656c 733a 202e 2e2e 0a20  b2.Labels: .... 
+0000bb50: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000bb60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000bb70: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+0000bb80: 2020 6b62 3a20 6e75 636c 6961 6462 5f70    kb: nucliadb_p
+0000bb90: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
+0000bba0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
+0000bbb0: 426f 7849 4420 7c20 4e6f 6e65 203d 202e  BoxID | None = .
+0000bbc0: 2e2e 2c0a 2020 2020 2020 2020 6c61 6265  ..,.        labe
+0000bbd0: 6c73 3a20 6e75 636c 6961 6462 5f70 726f  ls: nucliadb_pro
+0000bbe0: 746f 732e 6b6e 6f77 6c65 6467 6562 6f78  tos.knowledgebox
+0000bbf0: 5f70 6232 2e4c 6162 656c 7320 7c20 4e6f  _pb2.Labels | No
+0000bc00: 6e65 203d 202e 2e2e 2c0a 2020 2020 2020  ne = ...,.      
+0000bc10: 2020 7374 6174 7573 3a20 676c 6f62 616c    status: global
+0000bc20: 5f5f 5f47 6574 4c61 6265 6c73 5265 7370  ___GetLabelsResp
+0000bc30: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
+0000bc40: 6554 7970 6520 3d20 2e2e 2e2c 0a20 2020  eType = ...,.   
+0000bc50: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+0000bc60: 2020 2020 6465 6620 4861 7346 6965 6c64      def HasField
+0000bc70: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+0000bc80: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+0000bc90: 6c5b 226b 6222 2c20 6222 6b62 222c 2022  l["kb", b"kb", "
+0000bca0: 6c61 6265 6c73 222c 2062 226c 6162 656c  labels", b"label
+0000bcb0: 7322 5d29 202d 3e20 6275 696c 7469 6e73  s"]) -> builtins
+0000bcc0: 2e62 6f6f 6c3a 202e 2e2e 0a20 2020 2064  .bool: ....    d
+0000bcd0: 6566 2043 6c65 6172 4669 656c 6428 7365  ef ClearField(se
+0000bce0: 6c66 2c20 6669 656c 645f 6e61 6d65 3a20  lf, field_name: 
+0000bcf0: 7479 7069 6e67 2e4c 6974 6572 616c 5b22  typing.Literal["
+0000bd00: 6b62 222c 2062 226b 6222 2c20 226c 6162  kb", b"kb", "lab
+0000bd10: 656c 7322 2c20 6222 6c61 6265 6c73 222c  els", b"labels",
+0000bd20: 2022 7374 6174 7573 222c 2062 2273 7461   "status", b"sta
+0000bd30: 7475 7322 5d29 202d 3e20 4e6f 6e65 3a20  tus"]) -> None: 
+0000bd40: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4765  .....global___Ge
+0000bd50: 744c 6162 656c 7352 6573 706f 6e73 6520  tLabelsResponse 
+0000bd60: 3d20 4765 744c 6162 656c 7352 6573 706f  = GetLabelsRespo
+0000bd70: 6e73 650a 0a40 7479 7069 6e67 2e66 696e  nse..@typing.fin
+0000bd80: 616c 0a63 6c61 7373 2047 6574 4c61 6265  al.class GetLabe
+0000bd90: 6c73 5265 7175 6573 7428 676f 6f67 6c65  lsRequest(google
+0000bda0: 2e70 726f 746f 6275 662e 6d65 7373 6167  .protobuf.messag
+0000bdb0: 652e 4d65 7373 6167 6529 3a0a 2020 2020  e.Message):.    
+0000bdc0: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+0000bdd0: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+0000bde0: 7269 7074 6f72 2e44 6573 6372 6970 746f  riptor.Descripto
+0000bdf0: 720a 0a20 2020 204b 425f 4649 454c 445f  r..    KB_FIELD_
+0000be00: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000be10: 2e69 6e74 0a20 2020 2040 7072 6f70 6572  .int.    @proper
+0000be20: 7479 0a20 2020 2064 6566 206b 6228 7365  ty.    def kb(se
+0000be30: 6c66 2920 2d3e 206e 7563 6c69 6164 625f  lf) -> nucliadb_
+0000be40: 7072 6f74 6f73 2e6b 6e6f 776c 6564 6765  protos.knowledge
+0000be50: 626f 785f 7062 322e 4b6e 6f77 6c65 6467  box_pb2.Knowledg
+0000be60: 6542 6f78 4944 3a20 2e2e 2e0a 2020 2020  eBoxID: ....    
+0000be70: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0000be80: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000be90: 2020 2020 2a2c 0a20 2020 2020 2020 206b      *,.        k
+0000bea0: 623a 206e 7563 6c69 6164 625f 7072 6f74  b: nucliadb_prot
+0000beb0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+0000bec0: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
+0000bed0: 4944 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ID | None = ...,
+0000bee0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
+0000bef0: 2e2e 2e0a 2020 2020 6465 6620 4861 7346  ....    def HasF
+0000bf00: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+0000bf10: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+0000bf20: 7465 7261 6c5b 226b 6222 2c20 6222 6b62  teral["kb", b"kb
+0000bf30: 225d 2920 2d3e 2062 7569 6c74 696e 732e  "]) -> builtins.
+0000bf40: 626f 6f6c 3a20 2e2e 2e0a 2020 2020 6465  bool: ....    de
+0000bf50: 6620 436c 6561 7246 6965 6c64 2873 656c  f ClearField(sel
+0000bf60: 662c 2066 6965 6c64 5f6e 616d 653a 2074  f, field_name: t
+0000bf70: 7970 696e 672e 4c69 7465 7261 6c5b 226b  yping.Literal["k
+0000bf80: 6222 2c20 6222 6b62 225d 2920 2d3e 204e  b", b"kb"]) -> N
+0000bf90: 6f6e 653a 202e 2e2e 0a0a 676c 6f62 616c  one: .....global
+0000bfa0: 5f5f 5f47 6574 4c61 6265 6c73 5265 7175  ___GetLabelsRequ
+0000bfb0: 6573 7420 3d20 4765 744c 6162 656c 7352  est = GetLabelsR
+0000bfc0: 6571 7565 7374 0a0a 4074 7970 696e 672e  equest..@typing.
+0000bfd0: 6669 6e61 6c0a 636c 6173 7320 4765 7445  final.class GetE
+0000bfe0: 6e74 6974 6965 7347 726f 7570 5265 7175  ntitiesGroupRequ
+0000bff0: 6573 7428 676f 6f67 6c65 2e70 726f 746f  est(google.proto
+0000c000: 6275 662e 6d65 7373 6167 652e 4d65 7373  buf.message.Mess
+0000c010: 6167 6529 3a0a 2020 2020 4445 5343 5249  age):.    DESCRI
+0000c020: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+0000c030: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+0000c040: 2e44 6573 6372 6970 746f 720a 0a20 2020  .Descriptor..   
+0000c050: 204b 425f 4649 454c 445f 4e55 4d42 4552   KB_FIELD_NUMBER
+0000c060: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+0000c070: 2020 2047 524f 5550 5f46 4945 4c44 5f4e     GROUP_FIELD_N
+0000c080: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+0000c090: 696e 740a 2020 2020 6772 6f75 703a 2062  int.    group: b
+0000c0a0: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
+0000c0b0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000c0c0: 6620 6b62 2873 656c 6629 202d 3e20 6e75  f kb(self) -> nu
+0000c0d0: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+0000c0e0: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
+0000c0f0: 6e6f 776c 6564 6765 426f 7849 443a 202e  nowledgeBoxID: .
+0000c100: 2e2e 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
+0000c110: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0000c120: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
+0000c130: 2020 2020 2020 6b62 3a20 6e75 636c 6961        kb: nuclia
+0000c140: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
+0000c150: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
+0000c160: 6564 6765 426f 7849 4420 7c20 4e6f 6e65  edgeBoxID | None
+0000c170: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+0000c180: 6772 6f75 703a 2062 7569 6c74 696e 732e  group: builtins.
+0000c190: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2029  str = ...,.    )
+0000c1a0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+0000c1b0: 2020 6465 6620 4861 7346 6965 6c64 2873    def HasField(s
+0000c1c0: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+0000c1d0: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+0000c1e0: 226b 6222 2c20 6222 6b62 225d 2920 2d3e  "kb", b"kb"]) ->
+0000c1f0: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
+0000c200: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+0000c210: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+0000c220: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000c230: 4c69 7465 7261 6c5b 2267 726f 7570 222c  Literal["group",
+0000c240: 2062 2267 726f 7570 222c 2022 6b62 222c   b"group", "kb",
+0000c250: 2062 226b 6222 5d29 202d 3e20 4e6f 6e65   b"kb"]) -> None
+0000c260: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
+0000c270: 4765 7445 6e74 6974 6965 7347 726f 7570  GetEntitiesGroup
+0000c280: 5265 7175 6573 7420 3d20 4765 7445 6e74  Request = GetEnt
+0000c290: 6974 6965 7347 726f 7570 5265 7175 6573  itiesGroupReques
+0000c2a0: 740a 0a40 7479 7069 6e67 2e66 696e 616c  t..@typing.final
+0000c2b0: 0a63 6c61 7373 2047 6574 456e 7469 7469  .class GetEntiti
+0000c2c0: 6573 4772 6f75 7052 6573 706f 6e73 6528  esGroupResponse(
+0000c2d0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+0000c2e0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+0000c2f0: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
+0000c300: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+0000c310: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
+0000c320: 6372 6970 746f 720a 0a20 2020 2063 6c61  criptor..    cla
+0000c330: 7373 205f 5374 6174 7573 3a0a 2020 2020  ss _Status:.    
+0000c340: 2020 2020 5661 6c75 6554 7970 6520 3d20      ValueType = 
+0000c350: 7479 7069 6e67 2e4e 6577 5479 7065 2822  typing.NewType("
+0000c360: 5661 6c75 6554 7970 6522 2c20 6275 696c  ValueType", buil
+0000c370: 7469 6e73 2e69 6e74 290a 2020 2020 2020  tins.int).      
+0000c380: 2020 563a 2074 7970 696e 675f 6578 7465    V: typing_exte
+0000c390: 6e73 696f 6e73 2e54 7970 6541 6c69 6173  nsions.TypeAlias
+0000c3a0: 203d 2056 616c 7565 5479 7065 0a0a 2020   = ValueType..  
+0000c3b0: 2020 636c 6173 7320 5f53 7461 7475 7345    class _StatusE
+0000c3c0: 6e75 6d54 7970 6557 7261 7070 6572 2867  numTypeWrapper(g
+0000c3d0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
+0000c3e0: 6e74 6572 6e61 6c2e 656e 756d 5f74 7970  nternal.enum_typ
+0000c3f0: 655f 7772 6170 7065 722e 5f45 6e75 6d54  e_wrapper._EnumT
+0000c400: 7970 6557 7261 7070 6572 5b47 6574 456e  ypeWrapper[GetEn
+0000c410: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+0000c420: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+0000c430: 6554 7970 655d 2c20 6275 696c 7469 6e73  eType], builtins
+0000c440: 2e74 7970 6529 3a0a 2020 2020 2020 2020  .type):.        
+0000c450: 4445 5343 5249 5054 4f52 3a20 676f 6f67  DESCRIPTOR: goog
+0000c460: 6c65 2e70 726f 746f 6275 662e 6465 7363  le.protobuf.desc
+0000c470: 7269 7074 6f72 2e45 6e75 6d44 6573 6372  riptor.EnumDescr
+0000c480: 6970 746f 720a 2020 2020 2020 2020 4f4b  iptor.        OK
+0000c490: 3a20 4765 7445 6e74 6974 6965 7347 726f  : GetEntitiesGro
+0000c4a0: 7570 5265 7370 6f6e 7365 2e5f 5374 6174  upResponse._Stat
+0000c4b0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000c4c0: 300a 2020 2020 2020 2020 4b42 5f4e 4f54  0.        KB_NOT
+0000c4d0: 5f46 4f55 4e44 3a20 4765 7445 6e74 6974  _FOUND: GetEntit
+0000c4e0: 6965 7347 726f 7570 5265 7370 6f6e 7365  iesGroupResponse
+0000c4f0: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
+0000c500: 7065 2020 2320 310a 2020 2020 2020 2020  pe  # 1.        
+0000c510: 454e 5449 5449 4553 5f47 524f 5550 5f4e  ENTITIES_GROUP_N
+0000c520: 4f54 5f46 4f55 4e44 3a20 4765 7445 6e74  OT_FOUND: GetEnt
+0000c530: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+0000c540: 7365 2e5f 5374 6174 7573 2e56 616c 7565  se._Status.Value
+0000c550: 5479 7065 2020 2320 320a 2020 2020 2020  Type  # 2.      
+0000c560: 2020 4552 524f 523a 2047 6574 456e 7469    ERROR: GetEnti
+0000c570: 7469 6573 4772 6f75 7052 6573 706f 6e73  tiesGroupRespons
+0000c580: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
+0000c590: 7970 6520 2023 2033 0a0a 2020 2020 636c  ype  # 3..    cl
+0000c5a0: 6173 7320 5374 6174 7573 285f 5374 6174  ass Status(_Stat
+0000c5b0: 7573 2c20 6d65 7461 636c 6173 733d 5f53  us, metaclass=_S
+0000c5c0: 7461 7475 7345 6e75 6d54 7970 6557 7261  tatusEnumTypeWra
+0000c5d0: 7070 6572 293a 202e 2e2e 0a20 2020 204f  pper): ....    O
+0000c5e0: 4b3a 2047 6574 456e 7469 7469 6573 4772  K: GetEntitiesGr
+0000c5f0: 6f75 7052 6573 706f 6e73 652e 5374 6174  oupResponse.Stat
+0000c600: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+0000c610: 300a 2020 2020 4b42 5f4e 4f54 5f46 4f55  0.    KB_NOT_FOU
+0000c620: 4e44 3a20 4765 7445 6e74 6974 6965 7347  ND: GetEntitiesG
+0000c630: 726f 7570 5265 7370 6f6e 7365 2e53 7461  roupResponse.Sta
+0000c640: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
+0000c650: 2031 0a20 2020 2045 4e54 4954 4945 535f   1.    ENTITIES_
+0000c660: 4752 4f55 505f 4e4f 545f 464f 554e 443a  GROUP_NOT_FOUND:
+0000c670: 2047 6574 456e 7469 7469 6573 4772 6f75   GetEntitiesGrou
+0000c680: 7052 6573 706f 6e73 652e 5374 6174 7573  pResponse.Status
+0000c690: 2e56 616c 7565 5479 7065 2020 2320 320a  .ValueType  # 2.
+0000c6a0: 2020 2020 4552 524f 523a 2047 6574 456e      ERROR: GetEn
+0000c6b0: 7469 7469 6573 4772 6f75 7052 6573 706f  titiesGroupRespo
+0000c6c0: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+0000c6d0: 5479 7065 2020 2320 330a 0a20 2020 204b  Type  # 3..    K
+0000c6e0: 425f 4649 454c 445f 4e55 4d42 4552 3a20  B_FIELD_NUMBER: 
+0000c6f0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000c700: 2047 524f 5550 5f46 4945 4c44 5f4e 554d   GROUP_FIELD_NUM
+0000c710: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+0000c720: 740a 2020 2020 5354 4154 5553 5f46 4945  t.    STATUS_FIE
+0000c730: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+0000c740: 696e 732e 696e 740a 2020 2020 7374 6174  ins.int.    stat
+0000c750: 7573 3a20 676c 6f62 616c 5f5f 5f47 6574  us: global___Get
+0000c760: 456e 7469 7469 6573 4772 6f75 7052 6573  EntitiesGroupRes
+0000c770: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+0000c780: 7565 5479 7065 0a20 2020 2040 7072 6f70  ueType.    @prop
+0000c790: 6572 7479 0a20 2020 2064 6566 206b 6228  erty.    def kb(
+0000c7a0: 7365 6c66 2920 2d3e 206e 7563 6c69 6164  self) -> nucliad
+0000c7b0: 625f 7072 6f74 6f73 2e6b 6e6f 776c 6564  b_protos.knowled
+0000c7c0: 6765 626f 785f 7062 322e 4b6e 6f77 6c65  gebox_pb2.Knowle
+0000c7d0: 6467 6542 6f78 4944 3a20 2e2e 2e0a 2020  dgeBoxID: ....  
+0000c7e0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000c7f0: 6465 6620 6772 6f75 7028 7365 6c66 2920  def group(self) 
+0000c800: 2d3e 206e 7563 6c69 6164 625f 7072 6f74  -> nucliadb_prot
+0000c810: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+0000c820: 7062 322e 456e 7469 7469 6573 4772 6f75  pb2.EntitiesGrou
+0000c830: 703a 202e 2e2e 0a20 2020 2064 6566 205f  p: ....    def _
+0000c840: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000c850: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
+0000c860: 2c0a 2020 2020 2020 2020 6b62 3a20 6e75  ,.        kb: nu
+0000c870: 636c 6961 6462 5f70 726f 746f 732e 6b6e  cliadb_protos.kn
+0000c880: 6f77 6c65 6467 6562 6f78 5f70 6232 2e4b  owledgebox_pb2.K
+0000c890: 6e6f 776c 6564 6765 426f 7849 4420 7c20  nowledgeBoxID | 
+0000c8a0: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+0000c8b0: 2020 2020 6772 6f75 703a 206e 7563 6c69      group: nucli
+0000c8c0: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000c8d0: 6564 6765 626f 785f 7062 322e 456e 7469  edgebox_pb2.Enti
+0000c8e0: 7469 6573 4772 6f75 7020 7c20 4e6f 6e65  tiesGroup | None
+0000c8f0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+0000c900: 7374 6174 7573 3a20 676c 6f62 616c 5f5f  status: global__
+0000c910: 5f47 6574 456e 7469 7469 6573 4772 6f75  _GetEntitiesGrou
+0000c920: 7052 6573 706f 6e73 652e 5374 6174 7573  pResponse.Status
+0000c930: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
+0000c940: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+0000c950: 202e 2e2e 0a20 2020 2064 6566 2048 6173   ....    def Has
+0000c960: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+0000c970: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+0000c980: 6974 6572 616c 5b22 6772 6f75 7022 2c20  iteral["group", 
+0000c990: 6222 6772 6f75 7022 2c20 226b 6222 2c20  b"group", "kb", 
+0000c9a0: 6222 6b62 225d 2920 2d3e 2062 7569 6c74  b"kb"]) -> built
+0000c9b0: 696e 732e 626f 6f6c 3a20 2e2e 2e0a 2020  ins.bool: ....  
+0000c9c0: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
+0000c9d0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+0000c9e0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+0000c9f0: 6c5b 2267 726f 7570 222c 2062 2267 726f  l["group", b"gro
+0000ca00: 7570 222c 2022 6b62 222c 2062 226b 6222  up", "kb", b"kb"
+0000ca10: 2c20 2273 7461 7475 7322 2c20 6222 7374  , "status", b"st
+0000ca20: 6174 7573 225d 2920 2d3e 204e 6f6e 653a  atus"]) -> None:
+0000ca30: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f47   .....global___G
+0000ca40: 6574 456e 7469 7469 6573 4772 6f75 7052  etEntitiesGroupR
+0000ca50: 6573 706f 6e73 6520 3d20 4765 7445 6e74  esponse = GetEnt
+0000ca60: 6974 6965 7347 726f 7570 5265 7370 6f6e  itiesGroupRespon
+0000ca70: 7365 0a0a 4074 7970 696e 672e 6669 6e61  se..@typing.fina
+0000ca80: 6c0a 636c 6173 7320 4765 7456 6563 746f  l.class GetVecto
+0000ca90: 7253 6574 7352 6571 7565 7374 2867 6f6f  rSetsRequest(goo
+0000caa0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+0000cab0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+0000cac0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+0000cad0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+0000cae0: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+0000caf0: 7074 6f72 0a0a 2020 2020 4b42 5f46 4945  ptor..    KB_FIE
+0000cb00: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+0000cb10: 696e 732e 696e 740a 2020 2020 4070 726f  ins.int.    @pro
+0000cb20: 7065 7274 790a 2020 2020 6465 6620 6b62  perty.    def kb
+0000cb30: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
+0000cb40: 6462 5f70 726f 746f 732e 6b6e 6f77 6c65  db_protos.knowle
+0000cb50: 6467 6562 6f78 5f70 6232 2e4b 6e6f 776c  dgebox_pb2.Knowl
+0000cb60: 6564 6765 426f 7849 443a 202e 2e2e 0a20  edgeBoxID: .... 
+0000cb70: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000cb80: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000cb90: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+0000cba0: 2020 6b62 3a20 6e75 636c 6961 6462 5f70    kb: nucliadb_p
+0000cbb0: 726f 746f 732e 6b6e 6f77 6c65 6467 6562  rotos.knowledgeb
+0000cbc0: 6f78 5f70 6232 2e4b 6e6f 776c 6564 6765  ox_pb2.Knowledge
+0000cbd0: 426f 7849 4420 7c20 4e6f 6e65 203d 202e  BoxID | None = .
+0000cbe0: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
+0000cbf0: 653a 202e 2e2e 0a20 2020 2064 6566 2048  e: ....    def H
+0000cc00: 6173 4669 656c 6428 7365 6c66 2c20 6669  asField(self, fi
+0000cc10: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+0000cc20: 2e4c 6974 6572 616c 5b22 6b62 222c 2062  .Literal["kb", b
+0000cc30: 226b 6222 5d29 202d 3e20 6275 696c 7469  "kb"]) -> builti
+0000cc40: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
+0000cc50: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
+0000cc60: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+0000cc70: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+0000cc80: 5b22 6b62 222c 2062 226b 6222 5d29 202d  ["kb", b"kb"]) -
+0000cc90: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+0000cca0: 6261 6c5f 5f5f 4765 7456 6563 746f 7253  bal___GetVectorS
+0000ccb0: 6574 7352 6571 7565 7374 203d 2047 6574  etsRequest = Get
+0000ccc0: 5665 6374 6f72 5365 7473 5265 7175 6573  VectorSetsReques
+0000ccd0: 740a 0a40 7479 7069 6e67 2e66 696e 616c  t..@typing.final
+0000cce0: 0a63 6c61 7373 2047 6574 5665 6374 6f72  .class GetVector
+0000ccf0: 5365 7473 5265 7370 6f6e 7365 2867 6f6f  SetsResponse(goo
+0000cd00: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+0000cd10: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+0000cd20: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+0000cd30: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+0000cd40: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+0000cd50: 7074 6f72 0a0a 2020 2020 636c 6173 7320  ptor..    class 
+0000cd60: 5f53 7461 7475 733a 0a20 2020 2020 2020  _Status:.       
+0000cd70: 2056 616c 7565 5479 7065 203d 2074 7970   ValueType = typ
+0000cd80: 696e 672e 4e65 7754 7970 6528 2256 616c  ing.NewType("Val
+0000cd90: 7565 5479 7065 222c 2062 7569 6c74 696e  ueType", builtin
+0000cda0: 732e 696e 7429 0a20 2020 2020 2020 2056  s.int).        V
+0000cdb0: 3a20 7479 7069 6e67 5f65 7874 656e 7369  : typing_extensi
+0000cdc0: 6f6e 732e 5479 7065 416c 6961 7320 3d20  ons.TypeAlias = 
+0000cdd0: 5661 6c75 6554 7970 650a 0a20 2020 2063  ValueType..    c
+0000cde0: 6c61 7373 205f 5374 6174 7573 456e 756d  lass _StatusEnum
+0000cdf0: 5479 7065 5772 6170 7065 7228 676f 6f67  TypeWrapper(goog
+0000ce00: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+0000ce10: 726e 616c 2e65 6e75 6d5f 7479 7065 5f77  rnal.enum_type_w
+0000ce20: 7261 7070 6572 2e5f 456e 756d 5479 7065  rapper._EnumType
+0000ce30: 5772 6170 7065 725b 4765 7456 6563 746f  Wrapper[GetVecto
+0000ce40: 7253 6574 7352 6573 706f 6e73 652e 5f53  rSetsResponse._S
+0000ce50: 7461 7475 732e 5661 6c75 6554 7970 655d  tatus.ValueType]
+0000ce60: 2c20 6275 696c 7469 6e73 2e74 7970 6529  , builtins.type)
+0000ce70: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
+0000ce80: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+0000ce90: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+0000cea0: 2e45 6e75 6d44 6573 6372 6970 746f 720a  .EnumDescriptor.
+0000ceb0: 2020 2020 2020 2020 4f4b 3a20 4765 7456          OK: GetV
+0000cec0: 6563 746f 7253 6574 7352 6573 706f 6e73  ectorSetsRespons
+0000ced0: 652e 5f53 7461 7475 732e 5661 6c75 6554  e._Status.ValueT
+0000cee0: 7970 6520 2023 2030 0a20 2020 2020 2020  ype  # 0.       
+0000cef0: 204e 4f54 464f 554e 443a 2047 6574 5665   NOTFOUND: GetVe
+0000cf00: 6374 6f72 5365 7473 5265 7370 6f6e 7365  ctorSetsResponse
+0000cf10: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
+0000cf20: 7065 2020 2320 310a 2020 2020 2020 2020  pe  # 1.        
+0000cf30: 4552 524f 523a 2047 6574 5665 6374 6f72  ERROR: GetVector
+0000cf40: 5365 7473 5265 7370 6f6e 7365 2e5f 5374  SetsResponse._St
+0000cf50: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+0000cf60: 2320 320a 0a20 2020 2063 6c61 7373 2053  # 2..    class S
+0000cf70: 7461 7475 7328 5f53 7461 7475 732c 206d  tatus(_Status, m
+0000cf80: 6574 6163 6c61 7373 3d5f 5374 6174 7573  etaclass=_Status
+0000cf90: 456e 756d 5479 7065 5772 6170 7065 7229  EnumTypeWrapper)
+0000cfa0: 3a20 2e2e 2e0a 2020 2020 4f4b 3a20 4765  : ....    OK: Ge
+0000cfb0: 7456 6563 746f 7253 6574 7352 6573 706f  tVectorSetsRespo
+0000cfc0: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+0000cfd0: 5479 7065 2020 2320 300a 2020 2020 4e4f  Type  # 0.    NO
+0000cfe0: 5446 4f55 4e44 3a20 4765 7456 6563 746f  TFOUND: GetVecto
+0000cff0: 7253 6574 7352 6573 706f 6e73 652e 5374  rSetsResponse.St
+0000d000: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+0000d010: 2320 310a 2020 2020 4552 524f 523a 2047  # 1.    ERROR: G
+0000d020: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
+0000d030: 6f6e 7365 2e53 7461 7475 732e 5661 6c75  onse.Status.Valu
+0000d040: 6554 7970 6520 2023 2032 0a0a 2020 2020  eType  # 2..    
+0000d050: 4b42 5f46 4945 4c44 5f4e 554d 4245 523a  KB_FIELD_NUMBER:
+0000d060: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000d070: 2020 5645 4354 4f52 5345 5453 5f46 4945    VECTORSETS_FIE
+0000d080: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+0000d090: 696e 732e 696e 740a 2020 2020 5354 4154  ins.int.    STAT
+0000d0a0: 5553 5f46 4945 4c44 5f4e 554d 4245 523a  US_FIELD_NUMBER:
+0000d0b0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000d0c0: 2020 7374 6174 7573 3a20 676c 6f62 616c    status: global
+0000d0d0: 5f5f 5f47 6574 5665 6374 6f72 5365 7473  ___GetVectorSets
+0000d0e0: 5265 7370 6f6e 7365 2e53 7461 7475 732e  Response.Status.
+0000d0f0: 5661 6c75 6554 7970 650a 2020 2020 4070  ValueType.    @p
+0000d100: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+0000d110: 6b62 2873 656c 6629 202d 3e20 6e75 636c  kb(self) -> nucl
+0000d120: 6961 6462 5f70 726f 746f 732e 6b6e 6f77  iadb_protos.know
+0000d130: 6c65 6467 6562 6f78 5f70 6232 2e4b 6e6f  ledgebox_pb2.Kno
+0000d140: 776c 6564 6765 426f 7849 443a 202e 2e2e  wledgeBoxID: ...
+0000d150: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0000d160: 2020 2064 6566 2076 6563 746f 7273 6574     def vectorset
+0000d170: 7328 7365 6c66 2920 2d3e 206e 7563 6c69  s(self) -> nucli
+0000d180: 6164 625f 7072 6f74 6f73 2e6b 6e6f 776c  adb_protos.knowl
+0000d190: 6564 6765 626f 785f 7062 322e 5665 6374  edgebox_pb2.Vect
+0000d1a0: 6f72 5365 7473 3a20 2e2e 2e0a 2020 2020  orSets: ....    
+0000d1b0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0000d1c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000d1d0: 2020 2020 2a2c 0a20 2020 2020 2020 206b      *,.        k
+0000d1e0: 623a 206e 7563 6c69 6164 625f 7072 6f74  b: nucliadb_prot
+0000d1f0: 6f73 2e6b 6e6f 776c 6564 6765 626f 785f  os.knowledgebox_
+0000d200: 7062 322e 4b6e 6f77 6c65 6467 6542 6f78  pb2.KnowledgeBox
+0000d210: 4944 207c 204e 6f6e 6520 3d20 2e2e 2e2c  ID | None = ...,
+0000d220: 0a20 2020 2020 2020 2076 6563 746f 7273  .        vectors
+0000d230: 6574 733a 206e 7563 6c69 6164 625f 7072  ets: nucliadb_pr
+0000d240: 6f74 6f73 2e6b 6e6f 776c 6564 6765 626f  otos.knowledgebo
+0000d250: 785f 7062 322e 5665 6374 6f72 5365 7473  x_pb2.VectorSets
+0000d260: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+0000d270: 2020 2020 2020 2073 7461 7475 733a 2067         status: g
+0000d280: 6c6f 6261 6c5f 5f5f 4765 7456 6563 746f  lobal___GetVecto
+0000d290: 7253 6574 7352 6573 706f 6e73 652e 5374  rSetsResponse.St
+0000d2a0: 6174 7573 2e56 616c 7565 5479 7065 203d  atus.ValueType =
+0000d2b0: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+0000d2c0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+0000d2d0: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
+0000d2e0: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+0000d2f0: 6e67 2e4c 6974 6572 616c 5b22 6b62 222c  ng.Literal["kb",
+0000d300: 2062 226b 6222 2c20 2276 6563 746f 7273   b"kb", "vectors
+0000d310: 6574 7322 2c20 6222 7665 6374 6f72 7365  ets", b"vectorse
+0000d320: 7473 225d 2920 2d3e 2062 7569 6c74 696e  ts"]) -> builtin
+0000d330: 732e 626f 6f6c 3a20 2e2e 2e0a 2020 2020  s.bool: ....    
+0000d340: 6465 6620 436c 6561 7246 6965 6c64 2873  def ClearField(s
+0000d350: 656c 662c 2066 6965 6c64 5f6e 616d 653a  elf, field_name:
+0000d360: 2074 7970 696e 672e 4c69 7465 7261 6c5b   typing.Literal[
+0000d370: 226b 6222 2c20 6222 6b62 222c 2022 7374  "kb", b"kb", "st
+0000d380: 6174 7573 222c 2062 2273 7461 7475 7322  atus", b"status"
+0000d390: 2c20 2276 6563 746f 7273 6574 7322 2c20  , "vectorsets", 
+0000d3a0: 6222 7665 6374 6f72 7365 7473 225d 2920  b"vectorsets"]) 
+0000d3b0: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 676c  -> None: .....gl
+0000d3c0: 6f62 616c 5f5f 5f47 6574 5665 6374 6f72  obal___GetVector
+0000d3d0: 5365 7473 5265 7370 6f6e 7365 203d 2047  SetsResponse = G
+0000d3e0: 6574 5665 6374 6f72 5365 7473 5265 7370  etVectorSetsResp
+0000d3f0: 6f6e 7365 0a0a 4074 7970 696e 672e 6669  onse..@typing.fi
+0000d400: 6e61 6c0a 636c 6173 7320 4f70 5374 6174  nal.class OpStat
+0000d410: 7573 5772 6974 6572 2867 6f6f 676c 652e  usWriter(google.
+0000d420: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
+0000d430: 2e4d 6573 7361 6765 293a 0a20 2020 2044  .Message):.    D
+0000d440: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+0000d450: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+0000d460: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
+0000d470: 0a0a 2020 2020 636c 6173 7320 5f53 7461  ..    class _Sta
+0000d480: 7475 733a 0a20 2020 2020 2020 2056 616c  tus:.        Val
+0000d490: 7565 5479 7065 203d 2074 7970 696e 672e  ueType = typing.
+0000d4a0: 4e65 7754 7970 6528 2256 616c 7565 5479  NewType("ValueTy
+0000d4b0: 7065 222c 2062 7569 6c74 696e 732e 696e  pe", builtins.in
+0000d4c0: 7429 0a20 2020 2020 2020 2056 3a20 7479  t).        V: ty
+0000d4d0: 7069 6e67 5f65 7874 656e 7369 6f6e 732e  ping_extensions.
+0000d4e0: 5479 7065 416c 6961 7320 3d20 5661 6c75  TypeAlias = Valu
+0000d4f0: 6554 7970 650a 0a20 2020 2063 6c61 7373  eType..    class
+0000d500: 205f 5374 6174 7573 456e 756d 5479 7065   _StatusEnumType
+0000d510: 5772 6170 7065 7228 676f 6f67 6c65 2e70  Wrapper(google.p
+0000d520: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
+0000d530: 2e65 6e75 6d5f 7479 7065 5f77 7261 7070  .enum_type_wrapp
+0000d540: 6572 2e5f 456e 756d 5479 7065 5772 6170  er._EnumTypeWrap
+0000d550: 7065 725b 4f70 5374 6174 7573 5772 6974  per[OpStatusWrit
+0000d560: 6572 2e5f 5374 6174 7573 2e56 616c 7565  er._Status.Value
+0000d570: 5479 7065 5d2c 2062 7569 6c74 696e 732e  Type], builtins.
+0000d580: 7479 7065 293a 0a20 2020 2020 2020 2044  type):.        D
+0000d590: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+0000d5a0: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+0000d5b0: 6970 746f 722e 456e 756d 4465 7363 7269  iptor.EnumDescri
+0000d5c0: 7074 6f72 0a20 2020 2020 2020 204f 4b3a  ptor.        OK:
+0000d5d0: 204f 7053 7461 7475 7357 7269 7465 722e   OpStatusWriter.
+0000d5e0: 5f53 7461 7475 732e 5661 6c75 6554 7970  _Status.ValueTyp
+0000d5f0: 6520 2023 2030 0a20 2020 2020 2020 2045  e  # 0.        E
+0000d600: 5252 4f52 3a20 4f70 5374 6174 7573 5772  RROR: OpStatusWr
+0000d610: 6974 6572 2e5f 5374 6174 7573 2e56 616c  iter._Status.Val
+0000d620: 7565 5479 7065 2020 2320 310a 2020 2020  ueType  # 1.    
+0000d630: 2020 2020 4e4f 5446 4f55 4e44 3a20 4f70      NOTFOUND: Op
+0000d640: 5374 6174 7573 5772 6974 6572 2e5f 5374  StatusWriter._St
+0000d650: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+0000d660: 2320 320a 0a20 2020 2063 6c61 7373 2053  # 2..    class S
+0000d670: 7461 7475 7328 5f53 7461 7475 732c 206d  tatus(_Status, m
+0000d680: 6574 6163 6c61 7373 3d5f 5374 6174 7573  etaclass=_Status
+0000d690: 456e 756d 5479 7065 5772 6170 7065 7229  EnumTypeWrapper)
+0000d6a0: 3a20 2e2e 2e0a 2020 2020 4f4b 3a20 4f70  : ....    OK: Op
+0000d6b0: 5374 6174 7573 5772 6974 6572 2e53 7461  StatusWriter.Sta
+0000d6c0: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
+0000d6d0: 2030 0a20 2020 2045 5252 4f52 3a20 4f70   0.    ERROR: Op
+0000d6e0: 5374 6174 7573 5772 6974 6572 2e53 7461  StatusWriter.Sta
+0000d6f0: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
+0000d700: 2031 0a20 2020 204e 4f54 464f 554e 443a   1.    NOTFOUND:
+0000d710: 204f 7053 7461 7475 7357 7269 7465 722e   OpStatusWriter.
+0000d720: 5374 6174 7573 2e56 616c 7565 5479 7065  Status.ValueType
+0000d730: 2020 2320 320a 0a20 2020 2053 5441 5455    # 2..    STATU
+0000d740: 535f 4649 454c 445f 4e55 4d42 4552 3a20  S_FIELD_NUMBER: 
+0000d750: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000d760: 2073 7461 7475 733a 2067 6c6f 6261 6c5f   status: global_
+0000d770: 5f5f 4f70 5374 6174 7573 5772 6974 6572  __OpStatusWriter
+0000d780: 2e53 7461 7475 732e 5661 6c75 6554 7970  .Status.ValueTyp
+0000d790: 650a 2020 2020 6465 6620 5f5f 696e 6974  e.    def __init
+0000d7a0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0000d7b0: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+0000d7c0: 2020 2020 2073 7461 7475 733a 2067 6c6f       status: glo
+0000d7d0: 6261 6c5f 5f5f 4f70 5374 6174 7573 5772  bal___OpStatusWr
+0000d7e0: 6974 6572 2e53 7461 7475 732e 5661 6c75  iter.Status.Valu
+0000d7f0: 6554 7970 6520 3d20 2e2e 2e2c 0a20 2020  eType = ...,.   
+0000d800: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+0000d810: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
+0000d820: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+0000d830: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+0000d840: 7261 6c5b 2273 7461 7475 7322 2c20 6222  ral["status", b"
+0000d850: 7374 6174 7573 225d 2920 2d3e 204e 6f6e  status"]) -> Non
+0000d860: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+0000d870: 5f4f 7053 7461 7475 7357 7269 7465 7220  _OpStatusWriter 
+0000d880: 3d20 4f70 5374 6174 7573 5772 6974 6572  = OpStatusWriter
+0000d890: 0a0a 4074 7970 696e 672e 6669 6e61 6c0a  ..@typing.final.
+0000d8a0: 636c 6173 7320 4e6f 7469 6669 6361 7469  class Notificati
+0000d8b0: 6f6e 2867 6f6f 676c 652e 7072 6f74 6f62  on(google.protob
+0000d8c0: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
+0000d8d0: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
+0000d8e0: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+0000d8f0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+0000d900: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+0000d910: 636c 6173 7320 5f41 6374 696f 6e3a 0a20  class _Action:. 
+0000d920: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
+0000d930: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
+0000d940: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
+0000d950: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
+0000d960: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
+0000d970: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
+0000d980: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
+0000d990: 0a20 2020 2063 6c61 7373 205f 4163 7469  .    class _Acti
+0000d9a0: 6f6e 456e 756d 5479 7065 5772 6170 7065  onEnumTypeWrappe
+0000d9b0: 7228 676f 6f67 6c65 2e70 726f 746f 6275  r(google.protobu
+0000d9c0: 662e 696e 7465 726e 616c 2e65 6e75 6d5f  f.internal.enum_
+0000d9d0: 7479 7065 5f77 7261 7070 6572 2e5f 456e  type_wrapper._En
+0000d9e0: 756d 5479 7065 5772 6170 7065 725b 4e6f  umTypeWrapper[No
+0000d9f0: 7469 6669 6361 7469 6f6e 2e5f 4163 7469  tification._Acti
+0000da00: 6f6e 2e56 616c 7565 5479 7065 5d2c 2062  on.ValueType], b
+0000da10: 7569 6c74 696e 732e 7479 7065 293a 0a20  uiltins.type):. 
+0000da20: 2020 2020 2020 2044 4553 4352 4950 544f         DESCRIPTO
+0000da30: 523a 2067 6f6f 676c 652e 7072 6f74 6f62  R: google.protob
+0000da40: 7566 2e64 6573 6372 6970 746f 722e 456e  uf.descriptor.En
+0000da50: 756d 4465 7363 7269 7074 6f72 0a20 2020  umDescriptor.   
+0000da60: 2020 2020 2043 4f4d 4d49 543a 204e 6f74       COMMIT: Not
+0000da70: 6966 6963 6174 696f 6e2e 5f41 6374 696f  ification._Actio
+0000da80: 6e2e 5661 6c75 6554 7970 6520 2023 2030  n.ValueType  # 0
+0000da90: 0a20 2020 2020 2020 2041 424f 5254 3a20  .        ABORT: 
+0000daa0: 4e6f 7469 6669 6361 7469 6f6e 2e5f 4163  Notification._Ac
+0000dab0: 7469 6f6e 2e56 616c 7565 5479 7065 2020  tion.ValueType  
+0000dac0: 2320 310a 2020 2020 2020 2020 494e 4445  # 1.        INDE
+0000dad0: 5845 443a 204e 6f74 6966 6963 6174 696f  XED: Notificatio
+0000dae0: 6e2e 5f41 6374 696f 6e2e 5661 6c75 6554  n._Action.ValueT
+0000daf0: 7970 6520 2023 2032 0a0a 2020 2020 636c  ype  # 2..    cl
+0000db00: 6173 7320 4163 7469 6f6e 285f 4163 7469  ass Action(_Acti
+0000db10: 6f6e 2c20 6d65 7461 636c 6173 733d 5f41  on, metaclass=_A
+0000db20: 6374 696f 6e45 6e75 6d54 7970 6557 7261  ctionEnumTypeWra
+0000db30: 7070 6572 293a 202e 2e2e 0a20 2020 2043  pper): ....    C
+0000db40: 4f4d 4d49 543a 204e 6f74 6966 6963 6174  OMMIT: Notificat
+0000db50: 696f 6e2e 4163 7469 6f6e 2e56 616c 7565  ion.Action.Value
+0000db60: 5479 7065 2020 2320 300a 2020 2020 4142  Type  # 0.    AB
+0000db70: 4f52 543a 204e 6f74 6966 6963 6174 696f  ORT: Notificatio
+0000db80: 6e2e 4163 7469 6f6e 2e56 616c 7565 5479  n.Action.ValueTy
+0000db90: 7065 2020 2320 310a 2020 2020 494e 4445  pe  # 1.    INDE
+0000dba0: 5845 443a 204e 6f74 6966 6963 6174 696f  XED: Notificatio
+0000dbb0: 6e2e 4163 7469 6f6e 2e56 616c 7565 5479  n.Action.ValueTy
+0000dbc0: 7065 2020 2320 320a 0a20 2020 2063 6c61  pe  # 2..    cla
+0000dbd0: 7373 205f 5772 6974 6554 7970 653a 0a20  ss _WriteType:. 
+0000dbe0: 2020 2020 2020 2056 616c 7565 5479 7065         ValueType
+0000dbf0: 203d 2074 7970 696e 672e 4e65 7754 7970   = typing.NewTyp
+0000dc00: 6528 2256 616c 7565 5479 7065 222c 2062  e("ValueType", b
+0000dc10: 7569 6c74 696e 732e 696e 7429 0a20 2020  uiltins.int).   
+0000dc20: 2020 2020 2056 3a20 7479 7069 6e67 5f65       V: typing_e
+0000dc30: 7874 656e 7369 6f6e 732e 5479 7065 416c  xtensions.TypeAl
+0000dc40: 6961 7320 3d20 5661 6c75 6554 7970 650a  ias = ValueType.
+0000dc50: 0a20 2020 2063 6c61 7373 205f 5772 6974  .    class _Writ
+0000dc60: 6554 7970 6545 6e75 6d54 7970 6557 7261  eTypeEnumTypeWra
+0000dc70: 7070 6572 2867 6f6f 676c 652e 7072 6f74  pper(google.prot
+0000dc80: 6f62 7566 2e69 6e74 6572 6e61 6c2e 656e  obuf.internal.en
+0000dc90: 756d 5f74 7970 655f 7772 6170 7065 722e  um_type_wrapper.
+0000dca0: 5f45 6e75 6d54 7970 6557 7261 7070 6572  _EnumTypeWrapper
+0000dcb0: 5b4e 6f74 6966 6963 6174 696f 6e2e 5f57  [Notification._W
+0000dcc0: 7269 7465 5479 7065 2e56 616c 7565 5479  riteType.ValueTy
+0000dcd0: 7065 5d2c 2062 7569 6c74 696e 732e 7479  pe], builtins.ty
+0000dce0: 7065 293a 0a20 2020 2020 2020 2044 4553  pe):.        DES
+0000dcf0: 4352 4950 544f 523a 2067 6f6f 676c 652e  CRIPTOR: google.
+0000dd00: 7072 6f74 6f62 7566 2e64 6573 6372 6970  protobuf.descrip
+0000dd10: 746f 722e 456e 756d 4465 7363 7269 7074  tor.EnumDescript
+0000dd20: 6f72 0a20 2020 2020 2020 2055 4e53 4554  or.        UNSET
+0000dd30: 3a20 4e6f 7469 6669 6361 7469 6f6e 2e5f  : Notification._
+0000dd40: 5772 6974 6554 7970 652e 5661 6c75 6554  WriteType.ValueT
+0000dd50: 7970 6520 2023 2030 0a20 2020 2020 2020  ype  # 0.       
+0000dd60: 2043 5245 4154 4544 3a20 4e6f 7469 6669   CREATED: Notifi
+0000dd70: 6361 7469 6f6e 2e5f 5772 6974 6554 7970  cation._WriteTyp
+0000dd80: 652e 5661 6c75 6554 7970 6520 2023 2031  e.ValueType  # 1
+0000dd90: 0a20 2020 2020 2020 204d 4f44 4946 4945  .        MODIFIE
+0000dda0: 443a 204e 6f74 6966 6963 6174 696f 6e2e  D: Notification.
+0000ddb0: 5f57 7269 7465 5479 7065 2e56 616c 7565  _WriteType.Value
+0000ddc0: 5479 7065 2020 2320 320a 2020 2020 2020  Type  # 2.      
+0000ddd0: 2020 4445 4c45 5445 443a 204e 6f74 6966    DELETED: Notif
+0000dde0: 6963 6174 696f 6e2e 5f57 7269 7465 5479  ication._WriteTy
+0000ddf0: 7065 2e56 616c 7565 5479 7065 2020 2320  pe.ValueType  # 
+0000de00: 330a 0a20 2020 2063 6c61 7373 2057 7269  3..    class Wri
+0000de10: 7465 5479 7065 285f 5772 6974 6554 7970  teType(_WriteTyp
+0000de20: 652c 206d 6574 6163 6c61 7373 3d5f 5772  e, metaclass=_Wr
+0000de30: 6974 6554 7970 6545 6e75 6d54 7970 6557  iteTypeEnumTypeW
+0000de40: 7261 7070 6572 293a 202e 2e2e 0a20 2020  rapper): ....   
+0000de50: 2055 4e53 4554 3a20 4e6f 7469 6669 6361   UNSET: Notifica
+0000de60: 7469 6f6e 2e57 7269 7465 5479 7065 2e56  tion.WriteType.V
+0000de70: 616c 7565 5479 7065 2020 2320 300a 2020  alueType  # 0.  
+0000de80: 2020 4352 4541 5445 443a 204e 6f74 6966    CREATED: Notif
+0000de90: 6963 6174 696f 6e2e 5772 6974 6554 7970  ication.WriteTyp
+0000dea0: 652e 5661 6c75 6554 7970 6520 2023 2031  e.ValueType  # 1
+0000deb0: 0a20 2020 204d 4f44 4946 4945 443a 204e  .    MODIFIED: N
+0000dec0: 6f74 6966 6963 6174 696f 6e2e 5772 6974  otification.Writ
+0000ded0: 6554 7970 652e 5661 6c75 6554 7970 6520  eType.ValueType 
+0000dee0: 2023 2032 0a20 2020 2044 454c 4554 4544   # 2.    DELETED
+0000def0: 3a20 4e6f 7469 6669 6361 7469 6f6e 2e57  : Notification.W
+0000df00: 7269 7465 5479 7065 2e56 616c 7565 5479  riteType.ValueTy
+0000df10: 7065 2020 2320 330a 0a20 2020 2050 4152  pe  # 3..    PAR
+0000df20: 5449 5449 4f4e 5f46 4945 4c44 5f4e 554d  TITION_FIELD_NUM
+0000df30: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+0000df40: 740a 2020 2020 4d55 4c54 495f 4649 454c  t.    MULTI_FIEL
+0000df50: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+0000df60: 6e73 2e69 6e74 0a20 2020 2055 5549 445f  ns.int.    UUID_
+0000df70: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+0000df80: 696c 7469 6e73 2e69 6e74 0a20 2020 204b  iltins.int.    K
+0000df90: 4249 445f 4649 454c 445f 4e55 4d42 4552  BID_FIELD_NUMBER
+0000dfa0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+0000dfb0: 2020 2053 4551 4944 5f46 4945 4c44 5f4e     SEQID_FIELD_N
+0000dfc0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+0000dfd0: 696e 740a 2020 2020 4143 5449 4f4e 5f46  int.    ACTION_F
+0000dfe0: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000dff0: 6c74 696e 732e 696e 740a 2020 2020 5752  ltins.int.    WR
+0000e000: 4954 455f 5459 5045 5f46 4945 4c44 5f4e  ITE_TYPE_FIELD_N
+0000e010: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+0000e020: 696e 740a 2020 2020 4d45 5353 4147 455f  int.    MESSAGE_
+0000e030: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+0000e040: 696c 7469 6e73 2e69 6e74 0a20 2020 2053  iltins.int.    S
+0000e050: 4f55 5243 455f 4649 454c 445f 4e55 4d42  OURCE_FIELD_NUMB
+0000e060: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000e070: 0a20 2020 2050 524f 4345 5353 494e 475f  .    PROCESSING_
+0000e080: 4552 524f 5253 5f46 4945 4c44 5f4e 554d  ERRORS_FIELD_NUM
+0000e090: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+0000e0a0: 740a 2020 2020 4d45 5353 4147 455f 4155  t.    MESSAGE_AU
+0000e0b0: 4449 545f 4649 454c 445f 4e55 4d42 4552  DIT_FIELD_NUMBER
+0000e0c0: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+0000e0d0: 2020 2070 6172 7469 7469 6f6e 3a20 6275     partition: bu
+0000e0e0: 696c 7469 6e73 2e69 6e74 0a20 2020 206d  iltins.int.    m
+0000e0f0: 756c 7469 3a20 6275 696c 7469 6e73 2e73  ulti: builtins.s
+0000e100: 7472 0a20 2020 2075 7569 643a 2062 7569  tr.    uuid: bui
+0000e110: 6c74 696e 732e 7374 720a 2020 2020 6b62  ltins.str.    kb
+0000e120: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
+0000e130: 0a20 2020 2073 6571 6964 3a20 6275 696c  .    seqid: buil
+0000e140: 7469 6e73 2e69 6e74 0a20 2020 2061 6374  tins.int.    act
+0000e150: 696f 6e3a 2067 6c6f 6261 6c5f 5f5f 4e6f  ion: global___No
+0000e160: 7469 6669 6361 7469 6f6e 2e41 6374 696f  tification.Actio
+0000e170: 6e2e 5661 6c75 6554 7970 650a 2020 2020  n.ValueType.    
+0000e180: 7772 6974 655f 7479 7065 3a20 676c 6f62  write_type: glob
+0000e190: 616c 5f5f 5f4e 6f74 6966 6963 6174 696f  al___Notificatio
+0000e1a0: 6e2e 5772 6974 6554 7970 652e 5661 6c75  n.WriteType.Valu
+0000e1b0: 6554 7970 650a 2020 2020 736f 7572 6365  eType.    source
+0000e1c0: 3a20 676c 6f62 616c 5f5f 5f4e 6f74 6966  : global___Notif
+0000e1d0: 6963 6174 696f 6e53 6f75 7263 652e 5661  icationSource.Va
+0000e1e0: 6c75 6554 7970 650a 2020 2020 7072 6f63  lueType.    proc
+0000e1f0: 6573 7369 6e67 5f65 7272 6f72 733a 2062  essing_errors: b
+0000e200: 7569 6c74 696e 732e 626f 6f6c 0a20 2020  uiltins.bool.   
+0000e210: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000e220: 6566 206d 6573 7361 6765 2873 656c 6629  ef message(self)
+0000e230: 202d 3e20 676c 6f62 616c 5f5f 5f42 726f   -> global___Bro
+0000e240: 6b65 724d 6573 7361 6765 3a20 2e2e 2e0a  kerMessage: ....
+0000e250: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000e260: 2020 6465 6620 6d65 7373 6167 655f 6175    def message_au
+0000e270: 6469 7428 7365 6c66 2920 2d3e 2067 6c6f  dit(self) -> glo
+0000e280: 6261 6c5f 5f5f 4175 6469 743a 202e 2e2e  bal___Audit: ...
+0000e290: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000e2a0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0000e2b0: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+0000e2c0: 2020 2020 7061 7274 6974 696f 6e3a 2062      partition: b
+0000e2d0: 7569 6c74 696e 732e 696e 7420 3d20 2e2e  uiltins.int = ..
+0000e2e0: 2e2c 0a20 2020 2020 2020 206d 756c 7469  .,.        multi
+0000e2f0: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+0000e300: 202e 2e2e 2c0a 2020 2020 2020 2020 7575   ...,.        uu
+0000e310: 6964 3a20 6275 696c 7469 6e73 2e73 7472  id: builtins.str
+0000e320: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+0000e330: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
+0000e340: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
+0000e350: 2020 7365 7169 643a 2062 7569 6c74 696e    seqid: builtin
+0000e360: 732e 696e 7420 3d20 2e2e 2e2c 0a20 2020  s.int = ...,.   
+0000e370: 2020 2020 2061 6374 696f 6e3a 2067 6c6f       action: glo
+0000e380: 6261 6c5f 5f5f 4e6f 7469 6669 6361 7469  bal___Notificati
+0000e390: 6f6e 2e41 6374 696f 6e2e 5661 6c75 6554  on.Action.ValueT
+0000e3a0: 7970 6520 3d20 2e2e 2e2c 0a20 2020 2020  ype = ...,.     
+0000e3b0: 2020 2077 7269 7465 5f74 7970 653a 2067     write_type: g
+0000e3c0: 6c6f 6261 6c5f 5f5f 4e6f 7469 6669 6361  lobal___Notifica
+0000e3d0: 7469 6f6e 2e57 7269 7465 5479 7065 2e56  tion.WriteType.V
+0000e3e0: 616c 7565 5479 7065 203d 202e 2e2e 2c0a  alueType = ...,.
+0000e3f0: 2020 2020 2020 2020 6d65 7373 6167 653a          message:
+0000e400: 2067 6c6f 6261 6c5f 5f5f 4272 6f6b 6572   global___Broker
+0000e410: 4d65 7373 6167 6520 7c20 4e6f 6e65 203d  Message | None =
+0000e420: 202e 2e2e 2c0a 2020 2020 2020 2020 736f   ...,.        so
+0000e430: 7572 6365 3a20 676c 6f62 616c 5f5f 5f4e  urce: global___N
+0000e440: 6f74 6966 6963 6174 696f 6e53 6f75 7263  otificationSourc
+0000e450: 652e 5661 6c75 6554 7970 6520 3d20 2e2e  e.ValueType = ..
+0000e460: 2e2c 0a20 2020 2020 2020 2070 726f 6365  .,.        proce
+0000e470: 7373 696e 675f 6572 726f 7273 3a20 6275  ssing_errors: bu
+0000e480: 696c 7469 6e73 2e62 6f6f 6c20 3d20 2e2e  iltins.bool = ..
+0000e490: 2e2c 0a20 2020 2020 2020 206d 6573 7361  .,.        messa
+0000e4a0: 6765 5f61 7564 6974 3a20 676c 6f62 616c  ge_audit: global
+0000e4b0: 5f5f 5f41 7564 6974 207c 204e 6f6e 6520  ___Audit | None 
+0000e4c0: 3d20 2e2e 2e2c 0a20 2020 2029 202d 3e20  = ...,.    ) -> 
+0000e4d0: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+0000e4e0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
+0000e4f0: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+0000e500: 696e 672e 4c69 7465 7261 6c5b 226d 6573  ing.Literal["mes
+0000e510: 7361 6765 222c 2062 226d 6573 7361 6765  sage", b"message
+0000e520: 222c 2022 6d65 7373 6167 655f 6175 6469  ", "message_audi
+0000e530: 7422 2c20 6222 6d65 7373 6167 655f 6175  t", b"message_au
+0000e540: 6469 7422 5d29 202d 3e20 6275 696c 7469  dit"]) -> builti
+0000e550: 6e73 2e62 6f6f 6c3a 202e 2e2e 0a20 2020  ns.bool: ....   
+0000e560: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
+0000e570: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+0000e580: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+0000e590: 5b22 6163 7469 6f6e 222c 2062 2261 6374  ["action", b"act
+0000e5a0: 696f 6e22 2c20 226b 6269 6422 2c20 6222  ion", "kbid", b"
+0000e5b0: 6b62 6964 222c 2022 6d65 7373 6167 6522  kbid", "message"
+0000e5c0: 2c20 6222 6d65 7373 6167 6522 2c20 226d  , b"message", "m
+0000e5d0: 6573 7361 6765 5f61 7564 6974 222c 2062  essage_audit", b
+0000e5e0: 226d 6573 7361 6765 5f61 7564 6974 222c  "message_audit",
+0000e5f0: 2022 6d75 6c74 6922 2c20 6222 6d75 6c74   "multi", b"mult
+0000e600: 6922 2c20 2270 6172 7469 7469 6f6e 222c  i", "partition",
+0000e610: 2062 2270 6172 7469 7469 6f6e 222c 2022   b"partition", "
+0000e620: 7072 6f63 6573 7369 6e67 5f65 7272 6f72  processing_error
+0000e630: 7322 2c20 6222 7072 6f63 6573 7369 6e67  s", b"processing
+0000e640: 5f65 7272 6f72 7322 2c20 2273 6571 6964  _errors", "seqid
+0000e650: 222c 2062 2273 6571 6964 222c 2022 736f  ", b"seqid", "so
+0000e660: 7572 6365 222c 2062 2273 6f75 7263 6522  urce", b"source"
+0000e670: 2c20 2275 7569 6422 2c20 6222 7575 6964  , "uuid", b"uuid
+0000e680: 222c 2022 7772 6974 655f 7479 7065 222c  ", "write_type",
+0000e690: 2062 2277 7269 7465 5f74 7970 6522 5d29   b"write_type"])
+0000e6a0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67   -> None: .....g
+0000e6b0: 6c6f 6261 6c5f 5f5f 4e6f 7469 6669 6361  lobal___Notifica
+0000e6c0: 7469 6f6e 203d 204e 6f74 6966 6963 6174  tion = Notificat
+0000e6d0: 696f 6e0a 0a40 7479 7069 6e67 2e66 696e  ion..@typing.fin
+0000e6e0: 616c 0a63 6c61 7373 204d 656d 6265 7228  al.class Member(
+0000e6f0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+0000e700: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+0000e710: 3a0a 2020 2020 2222 2254 6865 206d 656d  :.    """The mem
+0000e720: 6265 7220 696e 666f 726d 6174 696f 6e2e  ber information.
+0000e730: 2222 220a 0a20 2020 2044 4553 4352 4950  """..    DESCRIP
+0000e740: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+0000e750: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+0000e760: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+0000e770: 636c 6173 7320 5f54 7970 653a 0a20 2020  class _Type:.   
+0000e780: 2020 2020 2056 616c 7565 5479 7065 203d       ValueType =
+0000e790: 2074 7970 696e 672e 4e65 7754 7970 6528   typing.NewType(
+0000e7a0: 2256 616c 7565 5479 7065 222c 2062 7569  "ValueType", bui
+0000e7b0: 6c74 696e 732e 696e 7429 0a20 2020 2020  ltins.int).     
+0000e7c0: 2020 2056 3a20 7479 7069 6e67 5f65 7874     V: typing_ext
+0000e7d0: 656e 7369 6f6e 732e 5479 7065 416c 6961  ensions.TypeAlia
+0000e7e0: 7320 3d20 5661 6c75 6554 7970 650a 0a20  s = ValueType.. 
+0000e7f0: 2020 2063 6c61 7373 205f 5479 7065 456e     class _TypeEn
+0000e800: 756d 5479 7065 5772 6170 7065 7228 676f  umTypeWrapper(go
+0000e810: 6f67 6c65 2e70 726f 746f 6275 662e 696e  ogle.protobuf.in
+0000e820: 7465 726e 616c 2e65 6e75 6d5f 7479 7065  ternal.enum_type
+0000e830: 5f77 7261 7070 6572 2e5f 456e 756d 5479  _wrapper._EnumTy
+0000e840: 7065 5772 6170 7065 725b 4d65 6d62 6572  peWrapper[Member
+0000e850: 2e5f 5479 7065 2e56 616c 7565 5479 7065  ._Type.ValueType
+0000e860: 5d2c 2062 7569 6c74 696e 732e 7479 7065  ], builtins.type
+0000e870: 293a 0a20 2020 2020 2020 2044 4553 4352  ):.        DESCR
+0000e880: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+0000e890: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+0000e8a0: 722e 456e 756d 4465 7363 7269 7074 6f72  r.EnumDescriptor
+0000e8b0: 0a20 2020 2020 2020 2049 4f3a 204d 656d  .        IO: Mem
+0000e8c0: 6265 722e 5f54 7970 652e 5661 6c75 6554  ber._Type.ValueT
+0000e8d0: 7970 6520 2023 2030 0a20 2020 2020 2020  ype  # 0.       
+0000e8e0: 2053 4541 5243 483a 204d 656d 6265 722e   SEARCH: Member.
+0000e8f0: 5f54 7970 652e 5661 6c75 6554 7970 6520  _Type.ValueType 
+0000e900: 2023 2031 0a20 2020 2020 2020 2049 4e47   # 1.        ING
+0000e910: 4553 543a 204d 656d 6265 722e 5f54 7970  EST: Member._Typ
+0000e920: 652e 5661 6c75 6554 7970 6520 2023 2032  e.ValueType  # 2
+0000e930: 0a20 2020 2020 2020 2054 5241 494e 3a20  .        TRAIN: 
+0000e940: 4d65 6d62 6572 2e5f 5479 7065 2e56 616c  Member._Type.Val
+0000e950: 7565 5479 7065 2020 2320 330a 2020 2020  ueType  # 3.    
+0000e960: 2020 2020 554e 4b4e 4f57 4e3a 204d 656d      UNKNOWN: Mem
+0000e970: 6265 722e 5f54 7970 652e 5661 6c75 6554  ber._Type.ValueT
+0000e980: 7970 6520 2023 2034 0a0a 2020 2020 636c  ype  # 4..    cl
+0000e990: 6173 7320 5479 7065 285f 5479 7065 2c20  ass Type(_Type, 
+0000e9a0: 6d65 7461 636c 6173 733d 5f54 7970 6545  metaclass=_TypeE
+0000e9b0: 6e75 6d54 7970 6557 7261 7070 6572 293a  numTypeWrapper):
+0000e9c0: 202e 2e2e 0a20 2020 2049 4f3a 204d 656d   ....    IO: Mem
+0000e9d0: 6265 722e 5479 7065 2e56 616c 7565 5479  ber.Type.ValueTy
+0000e9e0: 7065 2020 2320 300a 2020 2020 5345 4152  pe  # 0.    SEAR
+0000e9f0: 4348 3a20 4d65 6d62 6572 2e54 7970 652e  CH: Member.Type.
+0000ea00: 5661 6c75 6554 7970 6520 2023 2031 0a20  ValueType  # 1. 
+0000ea10: 2020 2049 4e47 4553 543a 204d 656d 6265     INGEST: Membe
+0000ea20: 722e 5479 7065 2e56 616c 7565 5479 7065  r.Type.ValueType
+0000ea30: 2020 2320 320a 2020 2020 5452 4149 4e3a    # 2.    TRAIN:
+0000ea40: 204d 656d 6265 722e 5479 7065 2e56 616c   Member.Type.Val
+0000ea50: 7565 5479 7065 2020 2320 330a 2020 2020  ueType  # 3.    
+0000ea60: 554e 4b4e 4f57 4e3a 204d 656d 6265 722e  UNKNOWN: Member.
+0000ea70: 5479 7065 2e56 616c 7565 5479 7065 2020  Type.ValueType  
+0000ea80: 2320 340a 0a20 2020 2049 445f 4649 454c  # 4..    ID_FIEL
+0000ea90: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+0000eaa0: 6e73 2e69 6e74 0a20 2020 204c 4953 5445  ns.int.    LISTE
+0000eab0: 4e5f 4144 4452 4553 535f 4649 454c 445f  N_ADDRESS_FIELD_
+0000eac0: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000ead0: 2e69 6e74 0a20 2020 2049 535f 5345 4c46  .int.    IS_SELF
+0000eae0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+0000eaf0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+0000eb00: 5459 5045 5f46 4945 4c44 5f4e 554d 4245  TYPE_FIELD_NUMBE
+0000eb10: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+0000eb20: 2020 2020 4455 4d4d 595f 4649 454c 445f      DUMMY_FIELD_
+0000eb30: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000eb40: 2e69 6e74 0a20 2020 204c 4f41 445f 5343  .int.    LOAD_SC
+0000eb50: 4f52 455f 4649 454c 445f 4e55 4d42 4552  ORE_FIELD_NUMBER
+0000eb60: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+0000eb70: 2020 2053 4841 5244 5f43 4f55 4e54 5f46     SHARD_COUNT_F
+0000eb80: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000eb90: 6c74 696e 732e 696e 740a 2020 2020 5052  ltins.int.    PR
+0000eba0: 494d 4152 595f 4944 5f46 4945 4c44 5f4e  IMARY_ID_FIELD_N
+0000ebb0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+0000ebc0: 696e 740a 2020 2020 6964 3a20 6275 696c  int.    id: buil
+0000ebd0: 7469 6e73 2e73 7472 0a20 2020 2022 2222  tins.str.    """
+0000ebe0: 2f20 4d65 6d62 6572 2049 442e e380 8041  / Member ID....A
+0000ebf0: 2073 7472 696e 6720 6f66 2074 6865 2055   string of the U
+0000ec00: 5549 442e 2222 220a 2020 2020 6c69 7374  UID.""".    list
+0000ec10: 656e 5f61 6464 7265 7373 3a20 6275 696c  en_address: buil
+0000ec20: 7469 6e73 2e73 7472 0a20 2020 2022 2222  tins.str.    """
+0000ec30: 2f20 436c 7573 7465 7220 6c69 7374 656e  / Cluster listen
+0000ec40: 2061 6464 7265 7373 2e20 7374 7269 6e67   address. string
+0000ec50: 206f 6620 4950 2061 6e64 2070 6f72 7420   of IP and port 
+0000ec60: 6e75 6d62 6572 2e0a 2020 2020 2f20 452e  number..    / E.
+0000ec70: 672e 2031 3237 2e30 2e30 2e31 3a35 3030  g. 127.0.0.1:500
+0000ec80: 300a 2020 2020 2222 220a 2020 2020 6973  0.    """.    is
+0000ec90: 5f73 656c 663a 2062 7569 6c74 696e 732e  _self: builtins.
+0000eca0: 626f 6f6c 0a20 2020 2022 2222 2f20 4966  bool.    """/ If
+0000ecb0: 2074 7275 652c 2069 7420 6d65 616e 7320   true, it means 
+0000ecc0: 7365 6c66 2e22 2222 0a20 2020 2074 7970  self.""".    typ
+0000ecd0: 653a 2067 6c6f 6261 6c5f 5f5f 4d65 6d62  e: global___Memb
+0000ece0: 6572 2e54 7970 652e 5661 6c75 6554 7970  er.Type.ValueTyp
+0000ecf0: 650a 2020 2020 2222 222f 2049 6f2c 2049  e.    """/ Io, I
+0000ed00: 6e67 6573 742c 2053 6561 7263 682c 2054  ngest, Search, T
+0000ed10: 7261 696e 2e22 2222 0a20 2020 2064 756d  rain.""".    dum
+0000ed20: 6d79 3a20 6275 696c 7469 6e73 2e62 6f6f  my: builtins.boo
+0000ed30: 6c0a 2020 2020 2222 222f 2044 756d 6d79  l.    """/ Dummy
+0000ed40: 204d 656d 6265 7222 2222 0a20 2020 206c   Member""".    l
+0000ed50: 6f61 645f 7363 6f72 653a 2062 7569 6c74  oad_score: built
+0000ed60: 696e 732e 666c 6f61 740a 2020 2020 2222  ins.float.    ""
+0000ed70: 222f 2054 6865 206c 6f61 6420 7363 6f72  "/ The load scor
+0000ed80: 6520 6f66 2074 6865 206d 656d 6265 722e  e of the member.
+0000ed90: 2222 220a 2020 2020 7368 6172 645f 636f  """.    shard_co
+0000eda0: 756e 743a 2062 7569 6c74 696e 732e 696e  unt: builtins.in
+0000edb0: 740a 2020 2020 2222 222f 2054 6865 206e  t.    """/ The n
+0000edc0: 756d 6265 7220 6f66 2073 6861 7264 7320  umber of shards 
+0000edd0: 696e 2074 6865 206e 6f64 652e 2222 220a  in the node.""".
+0000ede0: 2020 2020 7072 696d 6172 795f 6964 3a20      primary_id: 
+0000edf0: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
+0000ee00: 2022 2222 2f20 5468 6520 6964 206f 6620   """/ The id of 
+0000ee10: 7468 6520 7072 696d 6172 7920 6e6f 6465  the primary node
+0000ee20: 2028 6966 2069 7420 6973 2061 2073 6563   (if it is a sec
+0000ee30: 6f6e 6461 7279 206e 6f64 6529 2e22 2222  ondary node)."""
+0000ee40: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000ee50: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0000ee60: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+0000ee70: 2020 2020 6964 3a20 6275 696c 7469 6e73      id: builtins
+0000ee80: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+0000ee90: 2020 2020 6c69 7374 656e 5f61 6464 7265      listen_addre
+0000eea0: 7373 3a20 6275 696c 7469 6e73 2e73 7472  ss: builtins.str
+0000eeb0: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+0000eec0: 6973 5f73 656c 663a 2062 7569 6c74 696e  is_self: builtin
+0000eed0: 732e 626f 6f6c 203d 202e 2e2e 2c0a 2020  s.bool = ...,.  
+0000eee0: 2020 2020 2020 7479 7065 3a20 676c 6f62        type: glob
+0000eef0: 616c 5f5f 5f4d 656d 6265 722e 5479 7065  al___Member.Type
+0000ef00: 2e56 616c 7565 5479 7065 203d 202e 2e2e  .ValueType = ...
+0000ef10: 2c0a 2020 2020 2020 2020 6475 6d6d 793a  ,.        dummy:
+0000ef20: 2062 7569 6c74 696e 732e 626f 6f6c 203d   builtins.bool =
+0000ef30: 202e 2e2e 2c0a 2020 2020 2020 2020 6c6f   ...,.        lo
+0000ef40: 6164 5f73 636f 7265 3a20 6275 696c 7469  ad_score: builti
+0000ef50: 6e73 2e66 6c6f 6174 203d 202e 2e2e 2c0a  ns.float = ...,.
+0000ef60: 2020 2020 2020 2020 7368 6172 645f 636f          shard_co
+0000ef70: 756e 743a 2062 7569 6c74 696e 732e 696e  unt: builtins.in
+0000ef80: 7420 3d20 2e2e 2e2c 0a20 2020 2020 2020  t = ...,.       
+0000ef90: 2070 7269 6d61 7279 5f69 643a 2062 7569   primary_id: bui
+0000efa0: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
+0000efb0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
+0000efc0: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+0000efd0: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+0000efe0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000eff0: 4c69 7465 7261 6c5b 2264 756d 6d79 222c  Literal["dummy",
+0000f000: 2062 2264 756d 6d79 222c 2022 6964 222c   b"dummy", "id",
+0000f010: 2062 2269 6422 2c20 2269 735f 7365 6c66   b"id", "is_self
+0000f020: 222c 2062 2269 735f 7365 6c66 222c 2022  ", b"is_self", "
+0000f030: 6c69 7374 656e 5f61 6464 7265 7373 222c  listen_address",
+0000f040: 2062 226c 6973 7465 6e5f 6164 6472 6573   b"listen_addres
+0000f050: 7322 2c20 226c 6f61 645f 7363 6f72 6522  s", "load_score"
+0000f060: 2c20 6222 6c6f 6164 5f73 636f 7265 222c  , b"load_score",
+0000f070: 2022 7072 696d 6172 795f 6964 222c 2062   "primary_id", b
+0000f080: 2270 7269 6d61 7279 5f69 6422 2c20 2273  "primary_id", "s
+0000f090: 6861 7264 5f63 6f75 6e74 222c 2062 2273  hard_count", b"s
+0000f0a0: 6861 7264 5f63 6f75 6e74 222c 2022 7479  hard_count", "ty
+0000f0b0: 7065 222c 2062 2274 7970 6522 5d29 202d  pe", b"type"]) -
+0000f0c0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+0000f0d0: 6261 6c5f 5f5f 4d65 6d62 6572 203d 204d  bal___Member = M
+0000f0e0: 656d 6265 720a 0a40 7479 7069 6e67 2e66  ember..@typing.f
+0000f0f0: 696e 616c 0a63 6c61 7373 204c 6973 744d  inal.class ListM
+0000f100: 656d 6265 7273 5265 7175 6573 7428 676f  embersRequest(go
+0000f110: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+0000f120: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+0000f130: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
+0000f140: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+0000f150: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
+0000f160: 6970 746f 720a 0a20 2020 2064 6566 205f  iptor..    def _
+0000f170: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000f180: 2073 656c 662c 0a20 2020 2029 202d 3e20   self,.    ) -> 
+0000f190: 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261  None: .....globa
+0000f1a0: 6c5f 5f5f 4c69 7374 4d65 6d62 6572 7352  l___ListMembersR
+0000f1b0: 6571 7565 7374 203d 204c 6973 744d 656d  equest = ListMem
+0000f1c0: 6265 7273 5265 7175 6573 740a 0a40 7479  bersRequest..@ty
+0000f1d0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+0000f1e0: 204c 6973 744d 656d 6265 7273 5265 7370   ListMembersResp
+0000f1f0: 6f6e 7365 2867 6f6f 676c 652e 7072 6f74  onse(google.prot
+0000f200: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+0000f210: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
+0000f220: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+0000f230: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+0000f240: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+0000f250: 2020 4d45 4d42 4552 535f 4649 454c 445f    MEMBERS_FIELD_
+0000f260: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000f270: 2e69 6e74 0a20 2020 2040 7072 6f70 6572  .int.    @proper
+0000f280: 7479 0a20 2020 2064 6566 206d 656d 6265  ty.    def membe
+0000f290: 7273 2873 656c 6629 202d 3e20 676f 6f67  rs(self) -> goog
+0000f2a0: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+0000f2b0: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+0000f2c0: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
+0000f2d0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
+0000f2e0: 676c 6f62 616c 5f5f 5f4d 656d 6265 725d  global___Member]
+0000f2f0: 3a20 2e2e 2e0a 2020 2020 6465 6620 5f5f  : ....    def __
+0000f300: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0000f310: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
+0000f320: 0a20 2020 2020 2020 206d 656d 6265 7273  .        members
+0000f330: 3a20 636f 6c6c 6563 7469 6f6e 732e 6162  : collections.ab
+0000f340: 632e 4974 6572 6162 6c65 5b67 6c6f 6261  c.Iterable[globa
+0000f350: 6c5f 5f5f 4d65 6d62 6572 5d20 7c20 4e6f  l___Member] | No
+0000f360: 6e65 203d 202e 2e2e 2c0a 2020 2020 2920  ne = ...,.    ) 
+0000f370: 2d3e 204e 6f6e 653a 202e 2e2e 0a20 2020  -> None: ....   
+0000f380: 2064 6566 2043 6c65 6172 4669 656c 6428   def ClearField(
+0000f390: 7365 6c66 2c20 6669 656c 645f 6e61 6d65  self, field_name
+0000f3a0: 3a20 7479 7069 6e67 2e4c 6974 6572 616c  : typing.Literal
+0000f3b0: 5b22 6d65 6d62 6572 7322 2c20 6222 6d65  ["members", b"me
+0000f3c0: 6d62 6572 7322 5d29 202d 3e20 4e6f 6e65  mbers"]) -> None
+0000f3d0: 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f  : .....global___
+0000f3e0: 4c69 7374 4d65 6d62 6572 7352 6573 706f  ListMembersRespo
+0000f3f0: 6e73 6520 3d20 4c69 7374 4d65 6d62 6572  nse = ListMember
+0000f400: 7352 6573 706f 6e73 650a 0a40 7479 7069  sResponse..@typi
+0000f410: 6e67 2e66 696e 616c 0a63 6c61 7373 2053  ng.final.class S
+0000f420: 6861 7264 5265 706c 6963 6128 676f 6f67  hardReplica(goog
+0000f430: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+0000f440: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+0000f450: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+0000f460: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+0000f470: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+0000f480: 746f 720a 0a20 2020 2053 4841 5244 5f46  tor..    SHARD_F
+0000f490: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+0000f4a0: 6c74 696e 732e 696e 740a 2020 2020 4e4f  ltins.int.    NO
+0000f4b0: 4445 5f46 4945 4c44 5f4e 554d 4245 523a  DE_FIELD_NUMBER:
+0000f4c0: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000f4d0: 2020 6e6f 6465 3a20 6275 696c 7469 6e73    node: builtins
+0000f4e0: 2e73 7472 0a20 2020 2040 7072 6f70 6572  .str.    @proper
+0000f4f0: 7479 0a20 2020 2064 6566 2073 6861 7264  ty.    def shard
+0000f500: 2873 656c 6629 202d 3e20 6e75 636c 6961  (self) -> nuclia
+0000f510: 6462 5f70 726f 746f 732e 6e6f 6465 7265  db_protos.nodere
+0000f520: 736f 7572 6365 735f 7062 322e 5368 6172  sources_pb2.Shar
+0000f530: 6443 7265 6174 6564 3a20 2e2e 2e0a 2020  dCreated: ....  
+0000f540: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0000f550: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000f560: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+0000f570: 2073 6861 7264 3a20 6e75 636c 6961 6462   shard: nucliadb
+0000f580: 5f70 726f 746f 732e 6e6f 6465 7265 736f  _protos.nodereso
+0000f590: 7572 6365 735f 7062 322e 5368 6172 6443  urces_pb2.ShardC
+0000f5a0: 7265 6174 6564 207c 204e 6f6e 6520 3d20  reated | None = 
+0000f5b0: 2e2e 2e2c 0a20 2020 2020 2020 206e 6f64  ...,.        nod
+0000f5c0: 653a 2062 7569 6c74 696e 732e 7374 7220  e: builtins.str 
+0000f5d0: 3d20 2e2e 2e2c 0a20 2020 2029 202d 3e20  = ...,.    ) -> 
+0000f5e0: 4e6f 6e65 3a20 2e2e 2e0a 2020 2020 6465  None: ....    de
+0000f5f0: 6620 4861 7346 6965 6c64 2873 656c 662c  f HasField(self,
+0000f600: 2066 6965 6c64 5f6e 616d 653a 2074 7970   field_name: typ
+0000f610: 696e 672e 4c69 7465 7261 6c5b 2273 6861  ing.Literal["sha
+0000f620: 7264 222c 2062 2273 6861 7264 225d 2920  rd", b"shard"]) 
+0000f630: 2d3e 2062 7569 6c74 696e 732e 626f 6f6c  -> builtins.bool
+0000f640: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+0000f650: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+0000f660: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+0000f670: 672e 4c69 7465 7261 6c5b 226e 6f64 6522  g.Literal["node"
+0000f680: 2c20 6222 6e6f 6465 222c 2022 7368 6172  , b"node", "shar
+0000f690: 6422 2c20 6222 7368 6172 6422 5d29 202d  d", b"shard"]) -
+0000f6a0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+0000f6b0: 6261 6c5f 5f5f 5368 6172 6452 6570 6c69  bal___ShardRepli
+0000f6c0: 6361 203d 2053 6861 7264 5265 706c 6963  ca = ShardReplic
+0000f6d0: 610a 0a40 7479 7069 6e67 2e66 696e 616c  a..@typing.final
+0000f6e0: 0a63 6c61 7373 2053 6861 7264 4f62 6a65  .class ShardObje
+0000f6f0: 6374 2867 6f6f 676c 652e 7072 6f74 6f62  ct(google.protob
+0000f700: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
+0000f710: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
+0000f720: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+0000f730: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+0000f740: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+0000f750: 5348 4152 445f 4649 454c 445f 4e55 4d42  SHARD_FIELD_NUMB
+0000f760: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000f770: 0a20 2020 2052 4550 4c49 4341 535f 4649  .    REPLICAS_FI
+0000f780: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+0000f790: 7469 6e73 2e69 6e74 0a20 2020 2054 494d  tins.int.    TIM
+0000f7a0: 4553 5441 4d50 5f46 4945 4c44 5f4e 554d  ESTAMP_FIELD_NUM
+0000f7b0: 4245 523a 2062 7569 6c74 696e 732e 696e  BER: builtins.in
+0000f7c0: 740a 2020 2020 5245 4144 5f4f 4e4c 595f  t.    READ_ONLY_
+0000f7d0: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+0000f7e0: 696c 7469 6e73 2e69 6e74 0a20 2020 2073  iltins.int.    s
+0000f7f0: 6861 7264 3a20 6275 696c 7469 6e73 2e73  hard: builtins.s
+0000f800: 7472 0a20 2020 2072 6561 645f 6f6e 6c79  tr.    read_only
+0000f810: 3a20 6275 696c 7469 6e73 2e62 6f6f 6c0a  : builtins.bool.
+0000f820: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000f830: 2020 6465 6620 7265 706c 6963 6173 2873    def replicas(s
+0000f840: 656c 6629 202d 3e20 676f 6f67 6c65 2e70  elf) -> google.p
+0000f850: 726f 746f 6275 662e 696e 7465 726e 616c  rotobuf.internal
+0000f860: 2e63 6f6e 7461 696e 6572 732e 5265 7065  .containers.Repe
+0000f870: 6174 6564 436f 6d70 6f73 6974 6546 6965  atedCompositeFie
+0000f880: 6c64 436f 6e74 6169 6e65 725b 676c 6f62  ldContainer[glob
+0000f890: 616c 5f5f 5f53 6861 7264 5265 706c 6963  al___ShardReplic
+0000f8a0: 615d 3a20 2e2e 2e0a 2020 2020 4070 726f  a]: ....    @pro
+0000f8b0: 7065 7274 790a 2020 2020 6465 6620 7469  perty.    def ti
+0000f8c0: 6d65 7374 616d 7028 7365 6c66 2920 2d3e  mestamp(self) ->
+0000f8d0: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+0000f8e0: 2e74 696d 6573 7461 6d70 5f70 6232 2e54  .timestamp_pb2.T
+0000f8f0: 696d 6573 7461 6d70 3a20 2e2e 2e0a 2020  imestamp: ....  
+0000f900: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0000f910: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000f920: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+0000f930: 2073 6861 7264 3a20 6275 696c 7469 6e73   shard: builtins
+0000f940: 2e73 7472 203d 202e 2e2e 2c0a 2020 2020  .str = ...,.    
+0000f950: 2020 2020 7265 706c 6963 6173 3a20 636f      replicas: co
+0000f960: 6c6c 6563 7469 6f6e 732e 6162 632e 4974  llections.abc.It
+0000f970: 6572 6162 6c65 5b67 6c6f 6261 6c5f 5f5f  erable[global___
+0000f980: 5368 6172 6452 6570 6c69 6361 5d20 7c20  ShardReplica] | 
+0000f990: 4e6f 6e65 203d 202e 2e2e 2c0a 2020 2020  None = ...,.    
+0000f9a0: 2020 2020 7469 6d65 7374 616d 703a 2067      timestamp: g
+0000f9b0: 6f6f 676c 652e 7072 6f74 6f62 7566 2e74  oogle.protobuf.t
+0000f9c0: 696d 6573 7461 6d70 5f70 6232 2e54 696d  imestamp_pb2.Tim
+0000f9d0: 6573 7461 6d70 207c 204e 6f6e 6520 3d20  estamp | None = 
+0000f9e0: 2e2e 2e2c 0a20 2020 2020 2020 2072 6561  ...,.        rea
+0000f9f0: 645f 6f6e 6c79 3a20 6275 696c 7469 6e73  d_only: builtins
+0000fa00: 2e62 6f6f 6c20 3d20 2e2e 2e2c 0a20 2020  .bool = ...,.   
+0000fa10: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+0000fa20: 2020 2020 6465 6620 4861 7346 6965 6c64      def HasField
+0000fa30: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+0000fa40: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+0000fa50: 6c5b 2274 696d 6573 7461 6d70 222c 2062  l["timestamp", b
+0000fa60: 2274 696d 6573 7461 6d70 225d 2920 2d3e  "timestamp"]) ->
+0000fa70: 2062 7569 6c74 696e 732e 626f 6f6c 3a20   builtins.bool: 
+0000fa80: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+0000fa90: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+0000faa0: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+0000fab0: 4c69 7465 7261 6c5b 2272 6561 645f 6f6e  Literal["read_on
+0000fac0: 6c79 222c 2062 2272 6561 645f 6f6e 6c79  ly", b"read_only
+0000fad0: 222c 2022 7265 706c 6963 6173 222c 2062  ", "replicas", b
+0000fae0: 2272 6570 6c69 6361 7322 2c20 2273 6861  "replicas", "sha
+0000faf0: 7264 222c 2062 2273 6861 7264 222c 2022  rd", b"shard", "
+0000fb00: 7469 6d65 7374 616d 7022 2c20 6222 7469  timestamp", b"ti
+0000fb10: 6d65 7374 616d 7022 5d29 202d 3e20 4e6f  mestamp"]) -> No
+0000fb20: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
+0000fb30: 5f5f 5368 6172 644f 626a 6563 7420 3d20  __ShardObject = 
+0000fb40: 5368 6172 644f 626a 6563 740a 0a40 7479  ShardObject..@ty
+0000fb50: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+0000fb60: 2053 6861 7264 7328 676f 6f67 6c65 2e70   Shards(google.p
+0000fb70: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+0000fb80: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+0000fb90: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+0000fba0: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+0000fbb0: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+0000fbc0: 0a20 2020 2040 7479 7069 6e67 2e66 696e  .    @typing.fin
+0000fbd0: 616c 0a20 2020 2063 6c61 7373 2045 7874  al.    class Ext
+0000fbe0: 7261 456e 7472 7928 676f 6f67 6c65 2e70  raEntry(google.p
+0000fbf0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+0000fc00: 4d65 7373 6167 6529 3a0a 2020 2020 2020  Message):.      
+0000fc10: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+0000fc20: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+0000fc30: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+0000fc40: 746f 720a 0a20 2020 2020 2020 204b 4559  tor..        KEY
+0000fc50: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+0000fc60: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+0000fc70: 2020 2020 5641 4c55 455f 4649 454c 445f      VALUE_FIELD_
+0000fc80: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+0000fc90: 2e69 6e74 0a20 2020 2020 2020 206b 6579  .int.        key
+0000fca0: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+0000fcb0: 2020 2020 2020 2076 616c 7565 3a20 6275         value: bu
+0000fcc0: 696c 7469 6e73 2e73 7472 0a20 2020 2020  iltins.str.     
+0000fcd0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000fce0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000fcf0: 662c 0a20 2020 2020 2020 2020 2020 202a  f,.            *
+0000fd00: 2c0a 2020 2020 2020 2020 2020 2020 6b65  ,.            ke
+0000fd10: 793a 2062 7569 6c74 696e 732e 7374 7220  y: builtins.str 
+0000fd20: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2020  = ...,.         
+0000fd30: 2020 2076 616c 7565 3a20 6275 696c 7469     value: builti
+0000fd40: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+0000fd50: 2020 2020 2020 2920 2d3e 204e 6f6e 653a        ) -> None:
+0000fd60: 202e 2e2e 0a20 2020 2020 2020 2064 6566   ....        def
+0000fd70: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+0000fd80: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+0000fd90: 7069 6e67 2e4c 6974 6572 616c 5b22 6b65  ping.Literal["ke
+0000fda0: 7922 2c20 6222 6b65 7922 2c20 2276 616c  y", b"key", "val
+0000fdb0: 7565 222c 2062 2276 616c 7565 225d 2920  ue", b"value"]) 
+0000fdc0: 2d3e 204e 6f6e 653a 202e 2e2e 0a0a 2020  -> None: .....  
+0000fdd0: 2020 5348 4152 4453 5f46 4945 4c44 5f4e    SHARDS_FIELD_N
+0000fde0: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+0000fdf0: 696e 740a 2020 2020 4b42 4944 5f46 4945  int.    KBID_FIE
+0000fe00: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+0000fe10: 696e 732e 696e 740a 2020 2020 4143 5455  ins.int.    ACTU
+0000fe20: 414c 5f46 4945 4c44 5f4e 554d 4245 523a  AL_FIELD_NUMBER:
+0000fe30: 2062 7569 6c74 696e 732e 696e 740a 2020   builtins.int.  
+0000fe40: 2020 5349 4d49 4c41 5249 5459 5f46 4945    SIMILARITY_FIE
+0000fe50: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+0000fe60: 696e 732e 696e 740a 2020 2020 4d4f 4445  ins.int.    MODE
+0000fe70: 4c5f 4649 454c 445f 4e55 4d42 4552 3a20  L_FIELD_NUMBER: 
+0000fe80: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+0000fe90: 2052 454c 4541 5345 5f43 4841 4e4e 454c   RELEASE_CHANNEL
+0000fea0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+0000feb0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+0000fec0: 4558 5452 415f 4649 454c 445f 4e55 4d42  EXTRA_FIELD_NUMB
+0000fed0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+0000fee0: 0a20 2020 206b 6269 643a 2062 7569 6c74  .    kbid: built
+0000fef0: 696e 732e 7374 720a 2020 2020 6163 7475  ins.str.    actu
+0000ff00: 616c 3a20 6275 696c 7469 6e73 2e69 6e74  al: builtins.int
+0000ff10: 0a20 2020 2022 2222 4445 5052 4543 4154  .    """DEPRECAT
+0000ff20: 4544 2061 204b 4220 6b6e 6f77 2063 616e  ED a KB know can
+0000ff30: 2068 6176 6520 6d75 6c74 6970 6c65 2061   have multiple a
+0000ff40: 6c69 7665 2073 6861 7264 7320 616e 6420  live shards and 
+0000ff50: 6973 2074 7261 636b 6564 2069 6e0a 2020  is tracked in.  
+0000ff60: 2020 6561 6368 2053 6861 7264 4f62 6a65    each ShardObje
+0000ff70: 6374 0a20 2020 2022 2222 0a20 2020 2073  ct.    """.    s
+0000ff80: 696d 696c 6172 6974 793a 206e 7563 6c69  imilarity: nucli
+0000ff90: 6164 625f 7072 6f74 6f73 2e75 7469 6c73  adb_protos.utils
+0000ffa0: 5f70 6232 2e56 6563 746f 7253 696d 696c  _pb2.VectorSimil
+0000ffb0: 6172 6974 792e 5661 6c75 6554 7970 650a  arity.ValueType.
+0000ffc0: 2020 2020 2222 2244 4550 5245 4341 5445      """DEPRECATE
+0000ffd0: 4420 696e 2066 6176 6f72 206f 6620 606d  D in favor of `m
+0000ffe0: 6f64 656c 6020 746f 2069 6e63 6c75 6465  odel` to include
+0000fff0: 206d 6f72 6520 6461 7461 2222 220a 2020   more data""".  
+00010000: 2020 7265 6c65 6173 655f 6368 616e 6e65    release_channe
+00010010: 6c3a 206e 7563 6c69 6164 625f 7072 6f74  l: nucliadb_prot
+00010020: 6f73 2e75 7469 6c73 5f70 6232 2e52 656c  os.utils_pb2.Rel
+00010030: 6561 7365 4368 616e 6e65 6c2e 5661 6c75  easeChannel.Valu
+00010040: 6554 7970 650a 2020 2020 4070 726f 7065  eType.    @prope
+00010050: 7274 790a 2020 2020 6465 6620 7368 6172  rty.    def shar
+00010060: 6473 2873 656c 6629 202d 3e20 676f 6f67  ds(self) -> goog
+00010070: 6c65 2e70 726f 746f 6275 662e 696e 7465  le.protobuf.inte
+00010080: 726e 616c 2e63 6f6e 7461 696e 6572 732e  rnal.containers.
+00010090: 5265 7065 6174 6564 436f 6d70 6f73 6974  RepeatedComposit
+000100a0: 6546 6965 6c64 436f 6e74 6169 6e65 725b  eFieldContainer[
+000100b0: 676c 6f62 616c 5f5f 5f53 6861 7264 4f62  global___ShardOb
+000100c0: 6a65 6374 5d3a 202e 2e2e 0a20 2020 2040  ject]: ....    @
+000100d0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000100e0: 206d 6f64 656c 2873 656c 6629 202d 3e20   model(self) -> 
+000100f0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00010100: 6b6e 6f77 6c65 6467 6562 6f78 5f70 6232  knowledgebox_pb2
+00010110: 2e53 656d 616e 7469 634d 6f64 656c 4d65  .SemanticModelMe
+00010120: 7461 6461 7461 3a20 2e2e 2e0a 2020 2020  tadata: ....    
+00010130: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00010140: 6620 6578 7472 6128 7365 6c66 2920 2d3e  f extra(self) ->
+00010150: 2067 6f6f 676c 652e 7072 6f74 6f62 7566   google.protobuf
+00010160: 2e69 6e74 6572 6e61 6c2e 636f 6e74 6169  .internal.contai
+00010170: 6e65 7273 2e53 6361 6c61 724d 6170 5b62  ners.ScalarMap[b
+00010180: 7569 6c74 696e 732e 7374 722c 2062 7569  uiltins.str, bui
+00010190: 6c74 696e 732e 7374 725d 3a20 2e2e 2e0a  ltins.str]: ....
+000101a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000101b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000101c0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+000101d0: 2020 2073 6861 7264 733a 2063 6f6c 6c65     shards: colle
+000101e0: 6374 696f 6e73 2e61 6263 2e49 7465 7261  ctions.abc.Itera
+000101f0: 626c 655b 676c 6f62 616c 5f5f 5f53 6861  ble[global___Sha
+00010200: 7264 4f62 6a65 6374 5d20 7c20 4e6f 6e65  rdObject] | None
+00010210: 203d 202e 2e2e 2c0a 2020 2020 2020 2020   = ...,.        
+00010220: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
+00010230: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
+00010240: 2020 6163 7475 616c 3a20 6275 696c 7469    actual: builti
+00010250: 6e73 2e69 6e74 203d 202e 2e2e 2c0a 2020  ns.int = ...,.  
+00010260: 2020 2020 2020 7369 6d69 6c61 7269 7479        similarity
+00010270: 3a20 6e75 636c 6961 6462 5f70 726f 746f  : nucliadb_proto
+00010280: 732e 7574 696c 735f 7062 322e 5665 6374  s.utils_pb2.Vect
+00010290: 6f72 5369 6d69 6c61 7269 7479 2e56 616c  orSimilarity.Val
+000102a0: 7565 5479 7065 203d 202e 2e2e 2c0a 2020  ueType = ...,.  
+000102b0: 2020 2020 2020 6d6f 6465 6c3a 206e 7563        model: nuc
+000102c0: 6c69 6164 625f 7072 6f74 6f73 2e6b 6e6f  liadb_protos.kno
+000102d0: 776c 6564 6765 626f 785f 7062 322e 5365  wledgebox_pb2.Se
+000102e0: 6d61 6e74 6963 4d6f 6465 6c4d 6574 6164  manticModelMetad
+000102f0: 6174 6120 7c20 4e6f 6e65 203d 202e 2e2e  ata | None = ...
+00010300: 2c0a 2020 2020 2020 2020 7265 6c65 6173  ,.        releas
+00010310: 655f 6368 616e 6e65 6c3a 206e 7563 6c69  e_channel: nucli
+00010320: 6164 625f 7072 6f74 6f73 2e75 7469 6c73  adb_protos.utils
+00010330: 5f70 6232 2e52 656c 6561 7365 4368 616e  _pb2.ReleaseChan
+00010340: 6e65 6c2e 5661 6c75 6554 7970 6520 3d20  nel.ValueType = 
+00010350: 2e2e 2e2c 0a20 2020 2020 2020 2065 7874  ...,.        ext
+00010360: 7261 3a20 636f 6c6c 6563 7469 6f6e 732e  ra: collections.
+00010370: 6162 632e 4d61 7070 696e 675b 6275 696c  abc.Mapping[buil
+00010380: 7469 6e73 2e73 7472 2c20 6275 696c 7469  tins.str, builti
+00010390: 6e73 2e73 7472 5d20 7c20 4e6f 6e65 203d  ns.str] | None =
+000103a0: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+000103b0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+000103c0: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
+000103d0: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+000103e0: 6e67 2e4c 6974 6572 616c 5b22 6d6f 6465  ng.Literal["mode
+000103f0: 6c22 2c20 6222 6d6f 6465 6c22 5d29 202d  l", b"model"]) -
+00010400: 3e20 6275 696c 7469 6e73 2e62 6f6f 6c3a  > builtins.bool:
+00010410: 202e 2e2e 0a20 2020 2064 6566 2043 6c65   ....    def Cle
+00010420: 6172 4669 656c 6428 7365 6c66 2c20 6669  arField(self, fi
+00010430: 656c 645f 6e61 6d65 3a20 7479 7069 6e67  eld_name: typing
+00010440: 2e4c 6974 6572 616c 5b22 6163 7475 616c  .Literal["actual
+00010450: 222c 2062 2261 6374 7561 6c22 2c20 2265  ", b"actual", "e
+00010460: 7874 7261 222c 2062 2265 7874 7261 222c  xtra", b"extra",
+00010470: 2022 6b62 6964 222c 2062 226b 6269 6422   "kbid", b"kbid"
+00010480: 2c20 226d 6f64 656c 222c 2062 226d 6f64  , "model", b"mod
+00010490: 656c 222c 2022 7265 6c65 6173 655f 6368  el", "release_ch
+000104a0: 616e 6e65 6c22 2c20 6222 7265 6c65 6173  annel", b"releas
+000104b0: 655f 6368 616e 6e65 6c22 2c20 2273 6861  e_channel", "sha
+000104c0: 7264 7322 2c20 6222 7368 6172 6473 222c  rds", b"shards",
+000104d0: 2022 7369 6d69 6c61 7269 7479 222c 2062   "similarity", b
+000104e0: 2273 696d 696c 6172 6974 7922 5d29 202d  "similarity"]) -
+000104f0: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+00010500: 6261 6c5f 5f5f 5368 6172 6473 203d 2053  bal___Shards = S
+00010510: 6861 7264 730a 0a40 7479 7069 6e67 2e66  hards..@typing.f
+00010520: 696e 616c 0a63 6c61 7373 2049 6e64 6578  inal.class Index
+00010530: 5265 736f 7572 6365 2867 6f6f 676c 652e  Resource(google.
+00010540: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
+00010550: 2e4d 6573 7361 6765 293a 0a20 2020 2044  .Message):.    D
+00010560: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+00010570: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+00010580: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
+00010590: 0a0a 2020 2020 4b42 4944 5f46 4945 4c44  ..    KBID_FIELD
+000105a0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+000105b0: 732e 696e 740a 2020 2020 5249 445f 4649  s.int.    RID_FI
+000105c0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+000105d0: 7469 6e73 2e69 6e74 0a20 2020 2052 4549  tins.int.    REI
+000105e0: 4e44 4558 5f56 4543 544f 5253 5f46 4945  NDEX_VECTORS_FIE
+000105f0: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00010600: 696e 732e 696e 740a 2020 2020 6b62 6964  ins.int.    kbid
+00010610: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+00010620: 2020 2072 6964 3a20 6275 696c 7469 6e73     rid: builtins
+00010630: 2e73 7472 0a20 2020 2072 6569 6e64 6578  .str.    reindex
+00010640: 5f76 6563 746f 7273 3a20 6275 696c 7469  _vectors: builti
+00010650: 6e73 2e62 6f6f 6c0a 2020 2020 6465 6620  ns.bool.    def 
+00010660: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00010670: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00010680: 2a2c 0a20 2020 2020 2020 206b 6269 643a  *,.        kbid:
+00010690: 2062 7569 6c74 696e 732e 7374 7220 3d20   builtins.str = 
+000106a0: 2e2e 2e2c 0a20 2020 2020 2020 2072 6964  ...,.        rid
+000106b0: 3a20 6275 696c 7469 6e73 2e73 7472 203d  : builtins.str =
+000106c0: 202e 2e2e 2c0a 2020 2020 2020 2020 7265   ...,.        re
+000106d0: 696e 6465 785f 7665 6374 6f72 733a 2062  index_vectors: b
+000106e0: 7569 6c74 696e 732e 626f 6f6c 203d 202e  uiltins.bool = .
+000106f0: 2e2e 2c0a 2020 2020 2920 2d3e 204e 6f6e  ..,.    ) -> Non
+00010700: 653a 202e 2e2e 0a20 2020 2064 6566 2043  e: ....    def C
+00010710: 6c65 6172 4669 656c 6428 7365 6c66 2c20  learField(self, 
+00010720: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+00010730: 6e67 2e4c 6974 6572 616c 5b22 6b62 6964  ng.Literal["kbid
+00010740: 222c 2062 226b 6269 6422 2c20 2272 6569  ", b"kbid", "rei
+00010750: 6e64 6578 5f76 6563 746f 7273 222c 2062  ndex_vectors", b
+00010760: 2272 6569 6e64 6578 5f76 6563 746f 7273  "reindex_vectors
+00010770: 222c 2022 7269 6422 2c20 6222 7269 6422  ", "rid", b"rid"
+00010780: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+00010790: 0a67 6c6f 6261 6c5f 5f5f 496e 6465 7852  .global___IndexR
+000107a0: 6573 6f75 7263 6520 3d20 496e 6465 7852  esource = IndexR
+000107b0: 6573 6f75 7263 650a 0a40 7479 7069 6e67  esource..@typing
+000107c0: 2e66 696e 616c 0a63 6c61 7373 2049 6e64  .final.class Ind
+000107d0: 6578 5374 6174 7573 2867 6f6f 676c 652e  exStatus(google.
+000107e0: 7072 6f74 6f62 7566 2e6d 6573 7361 6765  protobuf.message
+000107f0: 2e4d 6573 7361 6765 293a 0a20 2020 2044  .Message):.    D
+00010800: 4553 4352 4950 544f 523a 2067 6f6f 676c  ESCRIPTOR: googl
+00010810: 652e 7072 6f74 6f62 7566 2e64 6573 6372  e.protobuf.descr
+00010820: 6970 746f 722e 4465 7363 7269 7074 6f72  iptor.Descriptor
+00010830: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00010840: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00010850: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
+00010860: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f49   .....global___I
+00010870: 6e64 6578 5374 6174 7573 203d 2049 6e64  ndexStatus = Ind
+00010880: 6578 5374 6174 7573 0a0a 4074 7970 696e  exStatus..@typin
+00010890: 672e 6669 6e61 6c0a 636c 6173 7320 5365  g.final.class Se
+000108a0: 7456 6563 746f 7273 5265 7175 6573 7428  tVectorsRequest(
+000108b0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+000108c0: 6d65 7373 6167 652e 4d65 7373 6167 6529  message.Message)
+000108d0: 3a0a 2020 2020 4445 5343 5249 5054 4f52  :.    DESCRIPTOR
+000108e0: 3a20 676f 6f67 6c65 2e70 726f 746f 6275  : google.protobu
+000108f0: 662e 6465 7363 7269 7074 6f72 2e44 6573  f.descriptor.Des
+00010900: 6372 6970 746f 720a 0a20 2020 2056 4543  criptor..    VEC
+00010910: 544f 5253 5f46 4945 4c44 5f4e 554d 4245  TORS_FIELD_NUMBE
+00010920: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00010930: 2020 2020 4b42 4944 5f46 4945 4c44 5f4e      KBID_FIELD_N
+00010940: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00010950: 696e 740a 2020 2020 5249 445f 4649 454c  int.    RID_FIEL
+00010960: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00010970: 6e73 2e69 6e74 0a20 2020 2046 4945 4c44  ns.int.    FIELD
+00010980: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00010990: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+000109a0: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
+000109b0: 7472 0a20 2020 2072 6964 3a20 6275 696c  tr.    rid: buil
+000109c0: 7469 6e73 2e73 7472 0a20 2020 2040 7072  tins.str.    @pr
+000109d0: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
+000109e0: 6563 746f 7273 2873 656c 6629 202d 3e20  ectors(self) -> 
+000109f0: 6e75 636c 6961 6462 5f70 726f 746f 732e  nucliadb_protos.
+00010a00: 7574 696c 735f 7062 322e 5665 6374 6f72  utils_pb2.Vector
+00010a10: 4f62 6a65 6374 3a20 2e2e 2e0a 2020 2020  Object: ....    
+00010a20: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00010a30: 6620 6669 656c 6428 7365 6c66 2920 2d3e  f field(self) ->
+00010a40: 206e 7563 6c69 6164 625f 7072 6f74 6f73   nucliadb_protos
+00010a50: 2e72 6573 6f75 7263 6573 5f70 6232 2e46  .resources_pb2.F
+00010a60: 6965 6c64 4944 3a20 2e2e 2e0a 2020 2020  ieldID: ....    
+00010a70: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00010a80: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00010a90: 2020 2020 2a2c 0a20 2020 2020 2020 2076      *,.        v
+00010aa0: 6563 746f 7273 3a20 6e75 636c 6961 6462  ectors: nucliadb
+00010ab0: 5f70 726f 746f 732e 7574 696c 735f 7062  _protos.utils_pb
+00010ac0: 322e 5665 6374 6f72 4f62 6a65 6374 207c  2.VectorObject |
+00010ad0: 204e 6f6e 6520 3d20 2e2e 2e2c 0a20 2020   None = ...,.   
+00010ae0: 2020 2020 206b 6269 643a 2062 7569 6c74       kbid: built
+00010af0: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+00010b00: 2020 2020 2020 2072 6964 3a20 6275 696c         rid: buil
+00010b10: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
+00010b20: 2020 2020 2020 2020 6669 656c 643a 206e          field: n
+00010b30: 7563 6c69 6164 625f 7072 6f74 6f73 2e72  ucliadb_protos.r
+00010b40: 6573 6f75 7263 6573 5f70 6232 2e46 6965  esources_pb2.Fie
+00010b50: 6c64 4944 207c 204e 6f6e 6520 3d20 2e2e  ldID | None = ..
+00010b60: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+00010b70: 3a20 2e2e 2e0a 2020 2020 6465 6620 4861  : ....    def Ha
+00010b80: 7346 6965 6c64 2873 656c 662c 2066 6965  sField(self, fie
+00010b90: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00010ba0: 4c69 7465 7261 6c5b 2266 6965 6c64 222c  Literal["field",
+00010bb0: 2062 2266 6965 6c64 222c 2022 7665 6374   b"field", "vect
+00010bc0: 6f72 7322 2c20 6222 7665 6374 6f72 7322  ors", b"vectors"
+00010bd0: 5d29 202d 3e20 6275 696c 7469 6e73 2e62  ]) -> builtins.b
+00010be0: 6f6f 6c3a 202e 2e2e 0a20 2020 2064 6566  ool: ....    def
+00010bf0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+00010c00: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+00010c10: 7069 6e67 2e4c 6974 6572 616c 5b22 6669  ping.Literal["fi
+00010c20: 656c 6422 2c20 6222 6669 656c 6422 2c20  eld", b"field", 
+00010c30: 226b 6269 6422 2c20 6222 6b62 6964 222c  "kbid", b"kbid",
+00010c40: 2022 7269 6422 2c20 6222 7269 6422 2c20   "rid", b"rid", 
+00010c50: 2276 6563 746f 7273 222c 2062 2276 6563  "vectors", b"vec
+00010c60: 746f 7273 225d 2920 2d3e 204e 6f6e 653a  tors"]) -> None:
+00010c70: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f53   .....global___S
+00010c80: 6574 5665 6374 6f72 7352 6571 7565 7374  etVectorsRequest
+00010c90: 203d 2053 6574 5665 6374 6f72 7352 6571   = SetVectorsReq
+00010ca0: 7565 7374 0a0a 4074 7970 696e 672e 6669  uest..@typing.fi
+00010cb0: 6e61 6c0a 636c 6173 7320 5365 7456 6563  nal.class SetVec
+00010cc0: 746f 7273 5265 7370 6f6e 7365 2867 6f6f  torsResponse(goo
+00010cd0: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+00010ce0: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+00010cf0: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+00010d00: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00010d10: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+00010d20: 7074 6f72 0a0a 2020 2020 464f 554e 445f  ptor..    FOUND_
+00010d30: 4649 454c 445f 4e55 4d42 4552 3a20 6275  FIELD_NUMBER: bu
+00010d40: 696c 7469 6e73 2e69 6e74 0a20 2020 2066  iltins.int.    f
+00010d50: 6f75 6e64 3a20 6275 696c 7469 6e73 2e62  ound: builtins.b
+00010d60: 6f6f 6c0a 2020 2020 6465 6620 5f5f 696e  ool.    def __in
+00010d70: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00010d80: 6c66 2c0a 2020 2020 2020 2020 2a2c 0a20  lf,.        *,. 
+00010d90: 2020 2020 2020 2066 6f75 6e64 3a20 6275         found: bu
+00010da0: 696c 7469 6e73 2e62 6f6f 6c20 3d20 2e2e  iltins.bool = ..
+00010db0: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+00010dc0: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+00010dd0: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+00010de0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+00010df0: 672e 4c69 7465 7261 6c5b 2266 6f75 6e64  g.Literal["found
+00010e00: 222c 2062 2266 6f75 6e64 225d 2920 2d3e  ", b"found"]) ->
+00010e10: 204e 6f6e 653a 202e 2e2e 0a0a 676c 6f62   None: .....glob
+00010e20: 616c 5f5f 5f53 6574 5665 6374 6f72 7352  al___SetVectorsR
+00010e30: 6573 706f 6e73 6520 3d20 5365 7456 6563  esponse = SetVec
+00010e40: 746f 7273 5265 7370 6f6e 7365 0a0a 4074  torsResponse..@t
+00010e50: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
+00010e60: 7320 4669 6c65 5265 7175 6573 7428 676f  s FileRequest(go
+00010e70: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+00010e80: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+00010e90: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
+00010ea0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+00010eb0: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
+00010ec0: 6970 746f 720a 0a20 2020 2042 5543 4b45  iptor..    BUCKE
+00010ed0: 545f 4649 454c 445f 4e55 4d42 4552 3a20  T_FIELD_NUMBER: 
+00010ee0: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+00010ef0: 204b 4559 5f46 4945 4c44 5f4e 554d 4245   KEY_FIELD_NUMBE
+00010f00: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00010f10: 2020 2020 6275 636b 6574 3a20 6275 696c      bucket: buil
+00010f20: 7469 6e73 2e73 7472 0a20 2020 206b 6579  tins.str.    key
+00010f30: 3a20 6275 696c 7469 6e73 2e73 7472 0a20  : builtins.str. 
+00010f40: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00010f50: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00010f60: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00010f70: 2020 6275 636b 6574 3a20 6275 696c 7469    bucket: builti
+00010f80: 6e73 2e73 7472 203d 202e 2e2e 2c0a 2020  ns.str = ...,.  
+00010f90: 2020 2020 2020 6b65 793a 2062 7569 6c74        key: built
+00010fa0: 696e 732e 7374 7220 3d20 2e2e 2e2c 0a20  ins.str = ...,. 
+00010fb0: 2020 2029 202d 3e20 4e6f 6e65 3a20 2e2e     ) -> None: ..
+00010fc0: 2e0a 2020 2020 6465 6620 436c 6561 7246  ..    def ClearF
+00010fd0: 6965 6c64 2873 656c 662c 2066 6965 6c64  ield(self, field
+00010fe0: 5f6e 616d 653a 2074 7970 696e 672e 4c69  _name: typing.Li
+00010ff0: 7465 7261 6c5b 2262 7563 6b65 7422 2c20  teral["bucket", 
+00011000: 6222 6275 636b 6574 222c 2022 6b65 7922  b"bucket", "key"
+00011010: 2c20 6222 6b65 7922 5d29 202d 3e20 4e6f  , b"key"]) -> No
+00011020: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
+00011030: 5f5f 4669 6c65 5265 7175 6573 7420 3d20  __FileRequest = 
+00011040: 4669 6c65 5265 7175 6573 740a 0a40 7479  FileRequest..@ty
+00011050: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+00011060: 2042 696e 6172 7944 6174 6128 676f 6f67   BinaryData(goog
+00011070: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+00011080: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+00011090: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+000110a0: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+000110b0: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+000110c0: 746f 720a 0a20 2020 2044 4154 415f 4649  tor..    DATA_FI
+000110d0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+000110e0: 7469 6e73 2e69 6e74 0a20 2020 2064 6174  tins.int.    dat
+000110f0: 613a 2062 7569 6c74 696e 732e 6279 7465  a: builtins.byte
+00011100: 730a 2020 2020 6465 6620 5f5f 696e 6974  s.    def __init
+00011110: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00011120: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+00011130: 2020 2020 2064 6174 613a 2062 7569 6c74       data: built
+00011140: 696e 732e 6279 7465 7320 3d20 2e2e 2e2c  ins.bytes = ...,
+00011150: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
+00011160: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+00011170: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00011180: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00011190: 4c69 7465 7261 6c5b 2264 6174 6122 2c20  Literal["data", 
+000111a0: 6222 6461 7461 225d 2920 2d3e 204e 6f6e  b"data"]) -> Non
+000111b0: 653a 202e 2e2e 0a0a 676c 6f62 616c 5f5f  e: .....global__
+000111c0: 5f42 696e 6172 7944 6174 6120 3d20 4269  _BinaryData = Bi
+000111d0: 6e61 7279 4461 7461 0a0a 4074 7970 696e  naryData..@typin
+000111e0: 672e 6669 6e61 6c0a 636c 6173 7320 4269  g.final.class Bi
+000111f0: 6e61 7279 4d65 7461 6461 7461 2867 6f6f  naryMetadata(goo
+00011200: 676c 652e 7072 6f74 6f62 7566 2e6d 6573  gle.protobuf.mes
+00011210: 7361 6765 2e4d 6573 7361 6765 293a 0a20  sage.Message):. 
+00011220: 2020 2044 4553 4352 4950 544f 523a 2067     DESCRIPTOR: g
+00011230: 6f6f 676c 652e 7072 6f74 6f62 7566 2e64  oogle.protobuf.d
+00011240: 6573 6372 6970 746f 722e 4465 7363 7269  escriptor.Descri
+00011250: 7074 6f72 0a0a 2020 2020 4b42 4944 5f46  ptor..    KBID_F
+00011260: 4945 4c44 5f4e 554d 4245 523a 2062 7569  IELD_NUMBER: bui
+00011270: 6c74 696e 732e 696e 740a 2020 2020 4b45  ltins.int.    KE
+00011280: 595f 4649 454c 445f 4e55 4d42 4552 3a20  Y_FIELD_NUMBER: 
+00011290: 6275 696c 7469 6e73 2e69 6e74 0a20 2020  builtins.int.   
+000112a0: 2053 495a 455f 4649 454c 445f 4e55 4d42   SIZE_FIELD_NUMB
+000112b0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+000112c0: 0a20 2020 2046 494c 454e 414d 455f 4649  .    FILENAME_FI
+000112d0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+000112e0: 7469 6e73 2e69 6e74 0a20 2020 2043 4f4e  tins.int.    CON
+000112f0: 5445 4e54 5f54 5950 455f 4649 454c 445f  TENT_TYPE_FIELD_
+00011300: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00011310: 2e69 6e74 0a20 2020 206b 6269 643a 2062  .int.    kbid: b
+00011320: 7569 6c74 696e 732e 7374 720a 2020 2020  uiltins.str.    
+00011330: 6b65 793a 2062 7569 6c74 696e 732e 7374  key: builtins.st
+00011340: 720a 2020 2020 7369 7a65 3a20 6275 696c  r.    size: buil
+00011350: 7469 6e73 2e69 6e74 0a20 2020 2066 696c  tins.int.    fil
+00011360: 656e 616d 653a 2062 7569 6c74 696e 732e  ename: builtins.
+00011370: 7374 720a 2020 2020 636f 6e74 656e 745f  str.    content_
+00011380: 7479 7065 3a20 6275 696c 7469 6e73 2e73  type: builtins.s
+00011390: 7472 0a20 2020 2064 6566 205f 5f69 6e69  tr.    def __ini
+000113a0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000113b0: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
+000113c0: 2020 2020 2020 6b62 6964 3a20 6275 696c        kbid: buil
+000113d0: 7469 6e73 2e73 7472 203d 202e 2e2e 2c0a  tins.str = ...,.
+000113e0: 2020 2020 2020 2020 6b65 793a 2062 7569          key: bui
+000113f0: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
+00011400: 0a20 2020 2020 2020 2073 697a 653a 2062  .        size: b
+00011410: 7569 6c74 696e 732e 696e 7420 3d20 2e2e  uiltins.int = ..
+00011420: 2e2c 0a20 2020 2020 2020 2066 696c 656e  .,.        filen
+00011430: 616d 653a 2062 7569 6c74 696e 732e 7374  ame: builtins.st
+00011440: 7220 3d20 2e2e 2e2c 0a20 2020 2020 2020  r = ...,.       
+00011450: 2063 6f6e 7465 6e74 5f74 7970 653a 2062   content_type: b
+00011460: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+00011470: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+00011480: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+00011490: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+000114a0: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+000114b0: 672e 4c69 7465 7261 6c5b 2263 6f6e 7465  g.Literal["conte
+000114c0: 6e74 5f74 7970 6522 2c20 6222 636f 6e74  nt_type", b"cont
+000114d0: 656e 745f 7479 7065 222c 2022 6669 6c65  ent_type", "file
+000114e0: 6e61 6d65 222c 2062 2266 696c 656e 616d  name", b"filenam
+000114f0: 6522 2c20 226b 6269 6422 2c20 6222 6b62  e", "kbid", b"kb
+00011500: 6964 222c 2022 6b65 7922 2c20 6222 6b65  id", "key", b"ke
+00011510: 7922 2c20 2273 697a 6522 2c20 6222 7369  y", "size", b"si
+00011520: 7a65 225d 2920 2d3e 204e 6f6e 653a 202e  ze"]) -> None: .
+00011530: 2e2e 0a0a 676c 6f62 616c 5f5f 5f42 696e  ....global___Bin
+00011540: 6172 794d 6574 6164 6174 6120 3d20 4269  aryMetadata = Bi
+00011550: 6e61 7279 4d65 7461 6461 7461 0a0a 4074  naryMetadata..@t
+00011560: 7970 696e 672e 6669 6e61 6c0a 636c 6173  yping.final.clas
+00011570: 7320 5570 6c6f 6164 4269 6e61 7279 4461  s UploadBinaryDa
+00011580: 7461 2867 6f6f 676c 652e 7072 6f74 6f62  ta(google.protob
+00011590: 7566 2e6d 6573 7361 6765 2e4d 6573 7361  uf.message.Messa
+000115a0: 6765 293a 0a20 2020 2044 4553 4352 4950  ge):.    DESCRIP
+000115b0: 544f 523a 2067 6f6f 676c 652e 7072 6f74  TOR: google.prot
+000115c0: 6f62 7566 2e64 6573 6372 6970 746f 722e  obuf.descriptor.
+000115d0: 4465 7363 7269 7074 6f72 0a0a 2020 2020  Descriptor..    
+000115e0: 434f 554e 545f 4649 454c 445f 4e55 4d42  COUNT_FIELD_NUMB
+000115f0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00011600: 0a20 2020 204d 4554 4144 4154 415f 4649  .    METADATA_FI
+00011610: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00011620: 7469 6e73 2e69 6e74 0a20 2020 2050 4159  tins.int.    PAY
+00011630: 4c4f 4144 5f46 4945 4c44 5f4e 554d 4245  LOAD_FIELD_NUMBE
+00011640: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+00011650: 2020 2020 636f 756e 743a 2062 7569 6c74      count: built
+00011660: 696e 732e 696e 740a 2020 2020 7061 796c  ins.int.    payl
+00011670: 6f61 643a 2062 7569 6c74 696e 732e 6279  oad: builtins.by
+00011680: 7465 730a 2020 2020 4070 726f 7065 7274  tes.    @propert
+00011690: 790a 2020 2020 6465 6620 6d65 7461 6461  y.    def metada
+000116a0: 7461 2873 656c 6629 202d 3e20 676c 6f62  ta(self) -> glob
+000116b0: 616c 5f5f 5f42 696e 6172 794d 6574 6164  al___BinaryMetad
+000116c0: 6174 613a 202e 2e2e 0a20 2020 2064 6566  ata: ....    def
+000116d0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000116e0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000116f0: 202a 2c0a 2020 2020 2020 2020 636f 756e   *,.        coun
+00011700: 743a 2062 7569 6c74 696e 732e 696e 7420  t: builtins.int 
+00011710: 3d20 2e2e 2e2c 0a20 2020 2020 2020 206d  = ...,.        m
+00011720: 6574 6164 6174 613a 2067 6c6f 6261 6c5f  etadata: global_
+00011730: 5f5f 4269 6e61 7279 4d65 7461 6461 7461  __BinaryMetadata
+00011740: 207c 204e 6f6e 6520 3d20 2e2e 2e2c 0a20   | None = ...,. 
+00011750: 2020 2020 2020 2070 6179 6c6f 6164 3a20         payload: 
+00011760: 6275 696c 7469 6e73 2e62 7974 6573 203d  builtins.bytes =
+00011770: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+00011780: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+00011790: 2048 6173 4669 656c 6428 7365 6c66 2c20   HasField(self, 
+000117a0: 6669 656c 645f 6e61 6d65 3a20 7479 7069  field_name: typi
+000117b0: 6e67 2e4c 6974 6572 616c 5b22 6461 7461  ng.Literal["data
+000117c0: 222c 2062 2264 6174 6122 2c20 226d 6574  ", b"data", "met
+000117d0: 6164 6174 6122 2c20 6222 6d65 7461 6461  adata", b"metada
+000117e0: 7461 222c 2022 7061 796c 6f61 6422 2c20  ta", "payload", 
+000117f0: 6222 7061 796c 6f61 6422 5d29 202d 3e20  b"payload"]) -> 
+00011800: 6275 696c 7469 6e73 2e62 6f6f 6c3a 202e  builtins.bool: .
+00011810: 2e2e 0a20 2020 2064 6566 2043 6c65 6172  ...    def Clear
+00011820: 4669 656c 6428 7365 6c66 2c20 6669 656c  Field(self, fiel
+00011830: 645f 6e61 6d65 3a20 7479 7069 6e67 2e4c  d_name: typing.L
+00011840: 6974 6572 616c 5b22 636f 756e 7422 2c20  iteral["count", 
+00011850: 6222 636f 756e 7422 2c20 2264 6174 6122  b"count", "data"
+00011860: 2c20 6222 6461 7461 222c 2022 6d65 7461  , b"data", "meta
+00011870: 6461 7461 222c 2062 226d 6574 6164 6174  data", b"metadat
+00011880: 6122 2c20 2270 6179 6c6f 6164 222c 2062  a", "payload", b
+00011890: 2270 6179 6c6f 6164 225d 2920 2d3e 204e  "payload"]) -> N
+000118a0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+000118b0: 2057 6869 6368 4f6e 656f 6628 7365 6c66   WhichOneof(self
+000118c0: 2c20 6f6e 656f 665f 6772 6f75 703a 2074  , oneof_group: t
+000118d0: 7970 696e 672e 4c69 7465 7261 6c5b 2264  yping.Literal["d
+000118e0: 6174 6122 2c20 6222 6461 7461 225d 2920  ata", b"data"]) 
+000118f0: 2d3e 2074 7970 696e 672e 4c69 7465 7261  -> typing.Litera
+00011900: 6c5b 226d 6574 6164 6174 6122 2c20 2270  l["metadata", "p
+00011910: 6179 6c6f 6164 225d 207c 204e 6f6e 653a  ayload"] | None:
+00011920: 202e 2e2e 0a0a 676c 6f62 616c 5f5f 5f55   .....global___U
+00011930: 706c 6f61 6442 696e 6172 7944 6174 6120  ploadBinaryData 
+00011940: 3d20 5570 6c6f 6164 4269 6e61 7279 4461  = UploadBinaryDa
+00011950: 7461 0a0a 4074 7970 696e 672e 6669 6e61  ta..@typing.fina
+00011960: 6c0a 636c 6173 7320 4669 6c65 5570 6c6f  l.class FileUplo
+00011970: 6164 6564 2867 6f6f 676c 652e 7072 6f74  aded(google.prot
+00011980: 6f62 7566 2e6d 6573 7361 6765 2e4d 6573  obuf.message.Mes
+00011990: 7361 6765 293a 0a20 2020 2044 4553 4352  sage):.    DESCR
+000119a0: 4950 544f 523a 2067 6f6f 676c 652e 7072  IPTOR: google.pr
+000119b0: 6f74 6f62 7566 2e64 6573 6372 6970 746f  otobuf.descripto
+000119c0: 722e 4465 7363 7269 7074 6f72 0a0a 2020  r.Descriptor..  
+000119d0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000119e0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000119f0: 2020 2920 2d3e 204e 6f6e 653a 202e 2e2e    ) -> None: ...
+00011a00: 0a0a 676c 6f62 616c 5f5f 5f46 696c 6555  ..global___FileU
+00011a10: 706c 6f61 6465 6420 3d20 4669 6c65 5570  ploaded = FileUp
+00011a20: 6c6f 6164 6564 0a0a 4074 7970 696e 672e  loaded..@typing.
+00011a30: 6669 6e61 6c0a 636c 6173 7320 5379 6e6f  final.class Syno
+00011a40: 6e79 6d73 5265 7175 6573 7428 676f 6f67  nymsRequest(goog
+00011a50: 6c65 2e70 726f 746f 6275 662e 6d65 7373  le.protobuf.mess
+00011a60: 6167 652e 4d65 7373 6167 6529 3a0a 2020  age.Message):.  
+00011a70: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00011a80: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00011a90: 7363 7269 7074 6f72 2e44 6573 6372 6970  scriptor.Descrip
+00011aa0: 746f 720a 0a20 2020 204b 4249 445f 4649  tor..    KBID_FI
+00011ab0: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+00011ac0: 7469 6e73 2e69 6e74 0a20 2020 206b 6269  tins.int.    kbi
+00011ad0: 643a 2062 7569 6c74 696e 732e 7374 720a  d: builtins.str.
+00011ae0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00011af0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00011b00: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+00011b10: 2020 206b 6269 643a 2062 7569 6c74 696e     kbid: builtin
+00011b20: 732e 7374 7220 3d20 2e2e 2e2c 0a20 2020  s.str = ...,.   
+00011b30: 2029 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a   ) -> None: ....
+00011b40: 2020 2020 6465 6620 436c 6561 7246 6965      def ClearFie
+00011b50: 6c64 2873 656c 662c 2066 6965 6c64 5f6e  ld(self, field_n
+00011b60: 616d 653a 2074 7970 696e 672e 4c69 7465  ame: typing.Lite
+00011b70: 7261 6c5b 226b 6269 6422 2c20 6222 6b62  ral["kbid", b"kb
+00011b80: 6964 225d 2920 2d3e 204e 6f6e 653a 202e  id"]) -> None: .
+00011b90: 2e2e 0a0a 676c 6f62 616c 5f5f 5f53 796e  ....global___Syn
+00011ba0: 6f6e 796d 7352 6571 7565 7374 203d 2053  onymsRequest = S
+00011bb0: 796e 6f6e 796d 7352 6571 7565 7374 0a0a  ynonymsRequest..
+00011bc0: 4074 7970 696e 672e 6669 6e61 6c0a 636c  @typing.final.cl
+00011bd0: 6173 7320 4e65 7756 6563 746f 7253 6574  ass NewVectorSet
+00011be0: 5265 7175 6573 7428 676f 6f67 6c65 2e70  Request(google.p
+00011bf0: 726f 746f 6275 662e 6d65 7373 6167 652e  rotobuf.message.
+00011c00: 4d65 7373 6167 6529 3a0a 2020 2020 4445  Message):.    DE
+00011c10: 5343 5249 5054 4f52 3a20 676f 6f67 6c65  SCRIPTOR: google
+00011c20: 2e70 726f 746f 6275 662e 6465 7363 7269  .protobuf.descri
+00011c30: 7074 6f72 2e44 6573 6372 6970 746f 720a  ptor.Descriptor.
+00011c40: 0a20 2020 204b 4249 445f 4649 454c 445f  .    KBID_FIELD_
+00011c50: 4e55 4d42 4552 3a20 6275 696c 7469 6e73  NUMBER: builtins
+00011c60: 2e69 6e74 0a20 2020 2056 4543 544f 5253  .int.    VECTORS
+00011c70: 4554 5f49 445f 4649 454c 445f 4e55 4d42  ET_ID_FIELD_NUMB
+00011c80: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00011c90: 0a20 2020 2056 4543 544f 525f 5459 5045  .    VECTOR_TYPE
+00011ca0: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00011cb0: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+00011cc0: 5349 4d49 4c41 5249 5459 5f46 4945 4c44  SIMILARITY_FIELD
+00011cd0: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00011ce0: 732e 696e 740a 2020 2020 5645 4354 4f52  s.int.    VECTOR
+00011cf0: 5f44 494d 454e 5349 4f4e 5f46 4945 4c44  _DIMENSION_FIELD
+00011d00: 5f4e 554d 4245 523a 2062 7569 6c74 696e  _NUMBER: builtin
+00011d10: 732e 696e 740a 2020 2020 4e4f 524d 414c  s.int.    NORMAL
+00011d20: 495a 455f 5645 4354 4f52 535f 4649 454c  IZE_VECTORS_FIEL
+00011d30: 445f 4e55 4d42 4552 3a20 6275 696c 7469  D_NUMBER: builti
+00011d40: 6e73 2e69 6e74 0a20 2020 204d 4154 5259  ns.int.    MATRY
+00011d50: 4f53 484b 415f 4449 4d45 4e53 494f 4e53  OSHKA_DIMENSIONS
+00011d60: 5f46 4945 4c44 5f4e 554d 4245 523a 2062  _FIELD_NUMBER: b
+00011d70: 7569 6c74 696e 732e 696e 740a 2020 2020  uiltins.int.    
+00011d80: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
+00011d90: 7472 0a20 2020 2076 6563 746f 7273 6574  tr.    vectorset
+00011da0: 5f69 643a 2062 7569 6c74 696e 732e 7374  _id: builtins.st
+00011db0: 720a 2020 2020 7665 6374 6f72 5f74 7970  r.    vector_typ
+00011dc0: 653a 206e 7563 6c69 6164 625f 7072 6f74  e: nucliadb_prot
+00011dd0: 6f73 2e6e 6f64 6577 7269 7465 725f 7062  os.nodewriter_pb
+00011de0: 322e 5665 6374 6f72 5479 7065 2e56 616c  2.VectorType.Val
+00011df0: 7565 5479 7065 0a20 2020 2073 696d 696c  ueType.    simil
+00011e00: 6172 6974 793a 206e 7563 6c69 6164 625f  arity: nucliadb_
+00011e10: 7072 6f74 6f73 2e75 7469 6c73 5f70 6232  protos.utils_pb2
+00011e20: 2e56 6563 746f 7253 696d 696c 6172 6974  .VectorSimilarit
+00011e30: 792e 5661 6c75 6554 7970 650a 2020 2020  y.ValueType.    
+00011e40: 7665 6374 6f72 5f64 696d 656e 7369 6f6e  vector_dimension
+00011e50: 3a20 6275 696c 7469 6e73 2e69 6e74 0a20  : builtins.int. 
+00011e60: 2020 206e 6f72 6d61 6c69 7a65 5f76 6563     normalize_vec
+00011e70: 746f 7273 3a20 6275 696c 7469 6e73 2e62  tors: builtins.b
+00011e80: 6f6f 6c0a 2020 2020 4070 726f 7065 7274  ool.    @propert
+00011e90: 790a 2020 2020 6465 6620 6d61 7472 796f  y.    def matryo
+00011ea0: 7368 6b61 5f64 696d 656e 7369 6f6e 7328  shka_dimensions(
+00011eb0: 7365 6c66 2920 2d3e 2067 6f6f 676c 652e  self) -> google.
+00011ec0: 7072 6f74 6f62 7566 2e69 6e74 6572 6e61  protobuf.interna
+00011ed0: 6c2e 636f 6e74 6169 6e65 7273 2e52 6570  l.containers.Rep
+00011ee0: 6561 7465 6453 6361 6c61 7246 6965 6c64  eatedScalarField
+00011ef0: 436f 6e74 6169 6e65 725b 6275 696c 7469  Container[builti
+00011f00: 6e73 2e69 6e74 5d3a 202e 2e2e 0a20 2020  ns.int]: ....   
+00011f10: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00011f20: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00011f30: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00011f40: 6b62 6964 3a20 6275 696c 7469 6e73 2e73  kbid: builtins.s
+00011f50: 7472 203d 202e 2e2e 2c0a 2020 2020 2020  tr = ...,.      
+00011f60: 2020 7665 6374 6f72 7365 745f 6964 3a20    vectorset_id: 
+00011f70: 6275 696c 7469 6e73 2e73 7472 203d 202e  builtins.str = .
+00011f80: 2e2e 2c0a 2020 2020 2020 2020 7665 6374  ..,.        vect
+00011f90: 6f72 5f74 7970 653a 206e 7563 6c69 6164  or_type: nucliad
+00011fa0: 625f 7072 6f74 6f73 2e6e 6f64 6577 7269  b_protos.nodewri
+00011fb0: 7465 725f 7062 322e 5665 6374 6f72 5479  ter_pb2.VectorTy
+00011fc0: 7065 2e56 616c 7565 5479 7065 203d 202e  pe.ValueType = .
+00011fd0: 2e2e 2c0a 2020 2020 2020 2020 7369 6d69  ..,.        simi
+00011fe0: 6c61 7269 7479 3a20 6e75 636c 6961 6462  larity: nucliadb
+00011ff0: 5f70 726f 746f 732e 7574 696c 735f 7062  _protos.utils_pb
+00012000: 322e 5665 6374 6f72 5369 6d69 6c61 7269  2.VectorSimilari
+00012010: 7479 2e56 616c 7565 5479 7065 203d 202e  ty.ValueType = .
+00012020: 2e2e 2c0a 2020 2020 2020 2020 7665 6374  ..,.        vect
+00012030: 6f72 5f64 696d 656e 7369 6f6e 3a20 6275  or_dimension: bu
+00012040: 696c 7469 6e73 2e69 6e74 203d 202e 2e2e  iltins.int = ...
+00012050: 2c0a 2020 2020 2020 2020 6e6f 726d 616c  ,.        normal
+00012060: 697a 655f 7665 6374 6f72 733a 2062 7569  ize_vectors: bui
+00012070: 6c74 696e 732e 626f 6f6c 203d 202e 2e2e  ltins.bool = ...
+00012080: 2c0a 2020 2020 2020 2020 6d61 7472 796f  ,.        matryo
+00012090: 7368 6b61 5f64 696d 656e 7369 6f6e 733a  shka_dimensions:
+000120a0: 2063 6f6c 6c65 6374 696f 6e73 2e61 6263   collections.abc
+000120b0: 2e49 7465 7261 626c 655b 6275 696c 7469  .Iterable[builti
+000120c0: 6e73 2e69 6e74 5d20 7c20 4e6f 6e65 203d  ns.int] | None =
+000120d0: 202e 2e2e 2c0a 2020 2020 2920 2d3e 204e   ...,.    ) -> N
+000120e0: 6f6e 653a 202e 2e2e 0a20 2020 2064 6566  one: ....    def
+000120f0: 2043 6c65 6172 4669 656c 6428 7365 6c66   ClearField(self
+00012100: 2c20 6669 656c 645f 6e61 6d65 3a20 7479  , field_name: ty
+00012110: 7069 6e67 2e4c 6974 6572 616c 5b22 6b62  ping.Literal["kb
+00012120: 6964 222c 2062 226b 6269 6422 2c20 226d  id", b"kbid", "m
+00012130: 6174 7279 6f73 686b 615f 6469 6d65 6e73  atryoshka_dimens
+00012140: 696f 6e73 222c 2062 226d 6174 7279 6f73  ions", b"matryos
+00012150: 686b 615f 6469 6d65 6e73 696f 6e73 222c  hka_dimensions",
+00012160: 2022 6e6f 726d 616c 697a 655f 7665 6374   "normalize_vect
+00012170: 6f72 7322 2c20 6222 6e6f 726d 616c 697a  ors", b"normaliz
+00012180: 655f 7665 6374 6f72 7322 2c20 2273 696d  e_vectors", "sim
+00012190: 696c 6172 6974 7922 2c20 6222 7369 6d69  ilarity", b"simi
+000121a0: 6c61 7269 7479 222c 2022 7665 6374 6f72  larity", "vector
+000121b0: 5f64 696d 656e 7369 6f6e 222c 2062 2276  _dimension", b"v
+000121c0: 6563 746f 725f 6469 6d65 6e73 696f 6e22  ector_dimension"
+000121d0: 2c20 2276 6563 746f 725f 7479 7065 222c  , "vector_type",
+000121e0: 2062 2276 6563 746f 725f 7479 7065 222c   b"vector_type",
+000121f0: 2022 7665 6374 6f72 7365 745f 6964 222c   "vectorset_id",
+00012200: 2062 2276 6563 746f 7273 6574 5f69 6422   b"vectorset_id"
+00012210: 5d29 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a  ]) -> None: ....
+00012220: 0a67 6c6f 6261 6c5f 5f5f 4e65 7756 6563  .global___NewVec
+00012230: 746f 7253 6574 5265 7175 6573 7420 3d20  torSetRequest = 
+00012240: 4e65 7756 6563 746f 7253 6574 5265 7175  NewVectorSetRequ
+00012250: 6573 740a 0a40 7479 7069 6e67 2e66 696e  est..@typing.fin
+00012260: 616c 0a63 6c61 7373 204e 6577 5665 6374  al.class NewVect
+00012270: 6f72 5365 7452 6573 706f 6e73 6528 676f  orSetResponse(go
+00012280: 6f67 6c65 2e70 726f 746f 6275 662e 6d65  ogle.protobuf.me
+00012290: 7373 6167 652e 4d65 7373 6167 6529 3a0a  ssage.Message):.
+000122a0: 2020 2020 4445 5343 5249 5054 4f52 3a20      DESCRIPTOR: 
+000122b0: 676f 6f67 6c65 2e70 726f 746f 6275 662e  google.protobuf.
+000122c0: 6465 7363 7269 7074 6f72 2e44 6573 6372  descriptor.Descr
+000122d0: 6970 746f 720a 0a20 2020 2063 6c61 7373  iptor..    class
+000122e0: 205f 5374 6174 7573 3a0a 2020 2020 2020   _Status:.      
+000122f0: 2020 5661 6c75 6554 7970 6520 3d20 7479    ValueType = ty
+00012300: 7069 6e67 2e4e 6577 5479 7065 2822 5661  ping.NewType("Va
+00012310: 6c75 6554 7970 6522 2c20 6275 696c 7469  lueType", builti
+00012320: 6e73 2e69 6e74 290a 2020 2020 2020 2020  ns.int).        
+00012330: 563a 2074 7970 696e 675f 6578 7465 6e73  V: typing_extens
+00012340: 696f 6e73 2e54 7970 6541 6c69 6173 203d  ions.TypeAlias =
+00012350: 2056 616c 7565 5479 7065 0a0a 2020 2020   ValueType..    
+00012360: 636c 6173 7320 5f53 7461 7475 7345 6e75  class _StatusEnu
+00012370: 6d54 7970 6557 7261 7070 6572 2867 6f6f  mTypeWrapper(goo
+00012380: 676c 652e 7072 6f74 6f62 7566 2e69 6e74  gle.protobuf.int
+00012390: 6572 6e61 6c2e 656e 756d 5f74 7970 655f  ernal.enum_type_
+000123a0: 7772 6170 7065 722e 5f45 6e75 6d54 7970  wrapper._EnumTyp
+000123b0: 6557 7261 7070 6572 5b4e 6577 5665 6374  eWrapper[NewVect
+000123c0: 6f72 5365 7452 6573 706f 6e73 652e 5f53  orSetResponse._S
+000123d0: 7461 7475 732e 5661 6c75 6554 7970 655d  tatus.ValueType]
+000123e0: 2c20 6275 696c 7469 6e73 2e74 7970 6529  , builtins.type)
+000123f0: 3a0a 2020 2020 2020 2020 4445 5343 5249  :.        DESCRI
+00012400: 5054 4f52 3a20 676f 6f67 6c65 2e70 726f  PTOR: google.pro
+00012410: 746f 6275 662e 6465 7363 7269 7074 6f72  tobuf.descriptor
+00012420: 2e45 6e75 6d44 6573 6372 6970 746f 720a  .EnumDescriptor.
+00012430: 2020 2020 2020 2020 4f4b 3a20 4e65 7756          OK: NewV
+00012440: 6563 746f 7253 6574 5265 7370 6f6e 7365  ectorSetResponse
+00012450: 2e5f 5374 6174 7573 2e56 616c 7565 5479  ._Status.ValueTy
+00012460: 7065 2020 2320 300a 2020 2020 2020 2020  pe  # 0.        
+00012470: 4552 524f 523a 204e 6577 5665 6374 6f72  ERROR: NewVector
+00012480: 5365 7452 6573 706f 6e73 652e 5f53 7461  SetResponse._Sta
+00012490: 7475 732e 5661 6c75 6554 7970 6520 2023  tus.ValueType  #
+000124a0: 2031 0a20 2020 2020 2020 2022 2222 6765   1.        """ge
+000124b0: 6e65 7269 6320 6572 726f 7222 2222 0a0a  neric error"""..
+000124c0: 2020 2020 636c 6173 7320 5374 6174 7573      class Status
+000124d0: 285f 5374 6174 7573 2c20 6d65 7461 636c  (_Status, metacl
+000124e0: 6173 733d 5f53 7461 7475 7345 6e75 6d54  ass=_StatusEnumT
+000124f0: 7970 6557 7261 7070 6572 293a 202e 2e2e  ypeWrapper): ...
+00012500: 0a20 2020 204f 4b3a 204e 6577 5665 6374  .    OK: NewVect
+00012510: 6f72 5365 7452 6573 706f 6e73 652e 5374  orSetResponse.St
+00012520: 6174 7573 2e56 616c 7565 5479 7065 2020  atus.ValueType  
+00012530: 2320 300a 2020 2020 4552 524f 523a 204e  # 0.    ERROR: N
+00012540: 6577 5665 6374 6f72 5365 7452 6573 706f  ewVectorSetRespo
+00012550: 6e73 652e 5374 6174 7573 2e56 616c 7565  nse.Status.Value
+00012560: 5479 7065 2020 2320 310a 2020 2020 2222  Type  # 1.    ""
+00012570: 2267 656e 6572 6963 2065 7272 6f72 2222  "generic error""
+00012580: 220a 0a20 2020 2053 5441 5455 535f 4649  "..    STATUS_FI
+00012590: 454c 445f 4e55 4d42 4552 3a20 6275 696c  ELD_NUMBER: buil
+000125a0: 7469 6e73 2e69 6e74 0a20 2020 2044 4554  tins.int.    DET
+000125b0: 4149 4c53 5f46 4945 4c44 5f4e 554d 4245  AILS_FIELD_NUMBE
+000125c0: 523a 2062 7569 6c74 696e 732e 696e 740a  R: builtins.int.
+000125d0: 2020 2020 7374 6174 7573 3a20 676c 6f62      status: glob
+000125e0: 616c 5f5f 5f4e 6577 5665 6374 6f72 5365  al___NewVectorSe
+000125f0: 7452 6573 706f 6e73 652e 5374 6174 7573  tResponse.Status
+00012600: 2e56 616c 7565 5479 7065 0a20 2020 2064  .ValueType.    d
+00012610: 6574 6169 6c73 3a20 6275 696c 7469 6e73  etails: builtins
+00012620: 2e73 7472 0a20 2020 2064 6566 205f 5f69  .str.    def __i
+00012630: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00012640: 656c 662c 0a20 2020 2020 2020 202a 2c0a  elf,.        *,.
+00012650: 2020 2020 2020 2020 7374 6174 7573 3a20          status: 
+00012660: 676c 6f62 616c 5f5f 5f4e 6577 5665 6374  global___NewVect
+00012670: 6f72 5365 7452 6573 706f 6e73 652e 5374  orSetResponse.St
+00012680: 6174 7573 2e56 616c 7565 5479 7065 203d  atus.ValueType =
+00012690: 202e 2e2e 2c0a 2020 2020 2020 2020 6465   ...,.        de
+000126a0: 7461 696c 733a 2062 7569 6c74 696e 732e  tails: builtins.
+000126b0: 7374 7220 3d20 2e2e 2e2c 0a20 2020 2029  str = ...,.    )
+000126c0: 202d 3e20 4e6f 6e65 3a20 2e2e 2e0a 2020   -> None: ....  
+000126d0: 2020 6465 6620 436c 6561 7246 6965 6c64    def ClearField
+000126e0: 2873 656c 662c 2066 6965 6c64 5f6e 616d  (self, field_nam
+000126f0: 653a 2074 7970 696e 672e 4c69 7465 7261  e: typing.Litera
+00012700: 6c5b 2264 6574 6169 6c73 222c 2062 2264  l["details", b"d
+00012710: 6574 6169 6c73 222c 2022 7374 6174 7573  etails", "status
+00012720: 222c 2062 2273 7461 7475 7322 5d29 202d  ", b"status"]) -
+00012730: 3e20 4e6f 6e65 3a20 2e2e 2e0a 0a67 6c6f  > None: .....glo
+00012740: 6261 6c5f 5f5f 4e65 7756 6563 746f 7253  bal___NewVectorS
+00012750: 6574 5265 7370 6f6e 7365 203d 204e 6577  etResponse = New
+00012760: 5665 6374 6f72 5365 7452 6573 706f 6e73  VectorSetRespons
+00012770: 650a 0a40 7479 7069 6e67 2e66 696e 616c  e..@typing.final
+00012780: 0a63 6c61 7373 2044 656c 5665 6374 6f72  .class DelVector
+00012790: 5365 7452 6571 7565 7374 2867 6f6f 676c  SetRequest(googl
+000127a0: 652e 7072 6f74 6f62 7566 2e6d 6573 7361  e.protobuf.messa
+000127b0: 6765 2e4d 6573 7361 6765 293a 0a20 2020  ge.Message):.   
+000127c0: 2044 4553 4352 4950 544f 523a 2067 6f6f   DESCRIPTOR: goo
+000127d0: 676c 652e 7072 6f74 6f62 7566 2e64 6573  gle.protobuf.des
+000127e0: 6372 6970 746f 722e 4465 7363 7269 7074  criptor.Descript
+000127f0: 6f72 0a0a 2020 2020 4b42 4944 5f46 4945  or..    KBID_FIE
+00012800: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00012810: 696e 732e 696e 740a 2020 2020 5645 4354  ins.int.    VECT
+00012820: 4f52 5345 545f 4944 5f46 4945 4c44 5f4e  ORSET_ID_FIELD_N
+00012830: 554d 4245 523a 2062 7569 6c74 696e 732e  UMBER: builtins.
+00012840: 696e 740a 2020 2020 6b62 6964 3a20 6275  int.    kbid: bu
+00012850: 696c 7469 6e73 2e73 7472 0a20 2020 2076  iltins.str.    v
+00012860: 6563 746f 7273 6574 5f69 643a 2062 7569  ectorset_id: bui
+00012870: 6c74 696e 732e 7374 720a 2020 2020 6465  ltins.str.    de
+00012880: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00012890: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000128a0: 2020 2a2c 0a20 2020 2020 2020 206b 6269    *,.        kbi
+000128b0: 643a 2062 7569 6c74 696e 732e 7374 7220  d: builtins.str 
+000128c0: 3d20 2e2e 2e2c 0a20 2020 2020 2020 2076  = ...,.        v
+000128d0: 6563 746f 7273 6574 5f69 643a 2062 7569  ectorset_id: bui
+000128e0: 6c74 696e 732e 7374 7220 3d20 2e2e 2e2c  ltins.str = ...,
+000128f0: 0a20 2020 2029 202d 3e20 4e6f 6e65 3a20  .    ) -> None: 
+00012900: 2e2e 2e0a 2020 2020 6465 6620 436c 6561  ....    def Clea
+00012910: 7246 6965 6c64 2873 656c 662c 2066 6965  rField(self, fie
+00012920: 6c64 5f6e 616d 653a 2074 7970 696e 672e  ld_name: typing.
+00012930: 4c69 7465 7261 6c5b 226b 6269 6422 2c20  Literal["kbid", 
+00012940: 6222 6b62 6964 222c 2022 7665 6374 6f72  b"kbid", "vector
+00012950: 7365 745f 6964 222c 2062 2276 6563 746f  set_id", b"vecto
+00012960: 7273 6574 5f69 6422 5d29 202d 3e20 4e6f  rset_id"]) -> No
+00012970: 6e65 3a20 2e2e 2e0a 0a67 6c6f 6261 6c5f  ne: .....global_
+00012980: 5f5f 4465 6c56 6563 746f 7253 6574 5265  __DelVectorSetRe
+00012990: 7175 6573 7420 3d20 4465 6c56 6563 746f  quest = DelVecto
+000129a0: 7253 6574 5265 7175 6573 740a 0a40 7479  rSetRequest..@ty
+000129b0: 7069 6e67 2e66 696e 616c 0a63 6c61 7373  ping.final.class
+000129c0: 2044 656c 5665 6374 6f72 5365 7452 6573   DelVectorSetRes
+000129d0: 706f 6e73 6528 676f 6f67 6c65 2e70 726f  ponse(google.pro
+000129e0: 746f 6275 662e 6d65 7373 6167 652e 4d65  tobuf.message.Me
+000129f0: 7373 6167 6529 3a0a 2020 2020 4445 5343  ssage):.    DESC
+00012a00: 5249 5054 4f52 3a20 676f 6f67 6c65 2e70  RIPTOR: google.p
+00012a10: 726f 746f 6275 662e 6465 7363 7269 7074  rotobuf.descript
+00012a20: 6f72 2e44 6573 6372 6970 746f 720a 0a20  or.Descriptor.. 
+00012a30: 2020 2063 6c61 7373 205f 5374 6174 7573     class _Status
+00012a40: 3a0a 2020 2020 2020 2020 5661 6c75 6554  :.        ValueT
+00012a50: 7970 6520 3d20 7479 7069 6e67 2e4e 6577  ype = typing.New
+00012a60: 5479 7065 2822 5661 6c75 6554 7970 6522  Type("ValueType"
+00012a70: 2c20 6275 696c 7469 6e73 2e69 6e74 290a  , builtins.int).
+00012a80: 2020 2020 2020 2020 563a 2074 7970 696e          V: typin
+00012a90: 675f 6578 7465 6e73 696f 6e73 2e54 7970  g_extensions.Typ
+00012aa0: 6541 6c69 6173 203d 2056 616c 7565 5479  eAlias = ValueTy
+00012ab0: 7065 0a0a 2020 2020 636c 6173 7320 5f53  pe..    class _S
+00012ac0: 7461 7475 7345 6e75 6d54 7970 6557 7261  tatusEnumTypeWra
+00012ad0: 7070 6572 2867 6f6f 676c 652e 7072 6f74  pper(google.prot
+00012ae0: 6f62 7566 2e69 6e74 6572 6e61 6c2e 656e  obuf.internal.en
+00012af0: 756d 5f74 7970 655f 7772 6170 7065 722e  um_type_wrapper.
+00012b00: 5f45 6e75 6d54 7970 6557 7261 7070 6572  _EnumTypeWrapper
+00012b10: 5b44 656c 5665 6374 6f72 5365 7452 6573  [DelVectorSetRes
+00012b20: 706f 6e73 652e 5f53 7461 7475 732e 5661  ponse._Status.Va
+00012b30: 6c75 6554 7970 655d 2c20 6275 696c 7469  lueType], builti
+00012b40: 6e73 2e74 7970 6529 3a0a 2020 2020 2020  ns.type):.      
+00012b50: 2020 4445 5343 5249 5054 4f52 3a20 676f    DESCRIPTOR: go
+00012b60: 6f67 6c65 2e70 726f 746f 6275 662e 6465  ogle.protobuf.de
+00012b70: 7363 7269 7074 6f72 2e45 6e75 6d44 6573  scriptor.EnumDes
+00012b80: 6372 6970 746f 720a 2020 2020 2020 2020  criptor.        
+00012b90: 4f4b 3a20 4465 6c56 6563 746f 7253 6574  OK: DelVectorSet
+00012ba0: 5265 7370 6f6e 7365 2e5f 5374 6174 7573  Response._Status
+00012bb0: 2e56 616c 7565 5479 7065 2020 2320 300a  .ValueType  # 0.
+00012bc0: 2020 2020 2020 2020 4552 524f 523a 2044          ERROR: D
+00012bd0: 656c 5665 6374 6f72 5365 7452 6573 706f  elVectorSetRespo
+00012be0: 6e73 652e 5f53 7461 7475 732e 5661 6c75  nse._Status.Valu
+00012bf0: 6554 7970 6520 2023 2031 0a20 2020 2020  eType  # 1.     
+00012c00: 2020 2022 2222 6765 6e65 7269 6320 6572     """generic er
+00012c10: 726f 7222 2222 0a0a 2020 2020 636c 6173  ror"""..    clas
+00012c20: 7320 5374 6174 7573 285f 5374 6174 7573  s Status(_Status
+00012c30: 2c20 6d65 7461 636c 6173 733d 5f53 7461  , metaclass=_Sta
+00012c40: 7475 7345 6e75 6d54 7970 6557 7261 7070  tusEnumTypeWrapp
+00012c50: 6572 293a 202e 2e2e 0a20 2020 204f 4b3a  er): ....    OK:
+00012c60: 2044 656c 5665 6374 6f72 5365 7452 6573   DelVectorSetRes
+00012c70: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+00012c80: 7565 5479 7065 2020 2320 300a 2020 2020  ueType  # 0.    
+00012c90: 4552 524f 523a 2044 656c 5665 6374 6f72  ERROR: DelVector
+00012ca0: 5365 7452 6573 706f 6e73 652e 5374 6174  SetResponse.Stat
+00012cb0: 7573 2e56 616c 7565 5479 7065 2020 2320  us.ValueType  # 
+00012cc0: 310a 2020 2020 2222 2267 656e 6572 6963  1.    """generic
+00012cd0: 2065 7272 6f72 2222 220a 0a20 2020 2053   error"""..    S
+00012ce0: 5441 5455 535f 4649 454c 445f 4e55 4d42  TATUS_FIELD_NUMB
+00012cf0: 4552 3a20 6275 696c 7469 6e73 2e69 6e74  ER: builtins.int
+00012d00: 0a20 2020 2044 4554 4149 4c53 5f46 4945  .    DETAILS_FIE
+00012d10: 4c44 5f4e 554d 4245 523a 2062 7569 6c74  LD_NUMBER: built
+00012d20: 696e 732e 696e 740a 2020 2020 7374 6174  ins.int.    stat
+00012d30: 7573 3a20 676c 6f62 616c 5f5f 5f44 656c  us: global___Del
+00012d40: 5665 6374 6f72 5365 7452 6573 706f 6e73  VectorSetRespons
+00012d50: 652e 5374 6174 7573 2e56 616c 7565 5479  e.Status.ValueTy
+00012d60: 7065 0a20 2020 2064 6574 6169 6c73 3a20  pe.    details: 
+00012d70: 6275 696c 7469 6e73 2e73 7472 0a20 2020  builtins.str.   
+00012d80: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00012d90: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00012da0: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
+00012db0: 7374 6174 7573 3a20 676c 6f62 616c 5f5f  status: global__
+00012dc0: 5f44 656c 5665 6374 6f72 5365 7452 6573  _DelVectorSetRes
+00012dd0: 706f 6e73 652e 5374 6174 7573 2e56 616c  ponse.Status.Val
+00012de0: 7565 5479 7065 203d 202e 2e2e 2c0a 2020  ueType = ...,.  
+00012df0: 2020 2020 2020 6465 7461 696c 733a 2062        details: b
+00012e00: 7569 6c74 696e 732e 7374 7220 3d20 2e2e  uiltins.str = ..
+00012e10: 2e2c 0a20 2020 2029 202d 3e20 4e6f 6e65  .,.    ) -> None
+00012e20: 3a20 2e2e 2e0a 2020 2020 6465 6620 436c  : ....    def Cl
+00012e30: 6561 7246 6965 6c64 2873 656c 662c 2066  earField(self, f
+00012e40: 6965 6c64 5f6e 616d 653a 2074 7970 696e  ield_name: typin
+00012e50: 672e 4c69 7465 7261 6c5b 2264 6574 6169  g.Literal["detai
+00012e60: 6c73 222c 2062 2264 6574 6169 6c73 222c  ls", b"details",
+00012e70: 2022 7374 6174 7573 222c 2062 2273 7461   "status", b"sta
+00012e80: 7475 7322 5d29 202d 3e20 4e6f 6e65 3a20  tus"]) -> None: 
+00012e90: 2e2e 2e0a 0a67 6c6f 6261 6c5f 5f5f 4465  .....global___De
+00012ea0: 6c56 6563 746f 7253 6574 5265 7370 6f6e  lVectorSetRespon
+00012eb0: 7365 203d 2044 656c 5665 6374 6f72 5365  se = DelVectorSe
+00012ec0: 7452 6573 706f 6e73 650a                 tResponse.
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,34 +41,14 @@
                 response_deserializer=nucliadb__protos_dot_writer__pb2.SetVectorsResponse.FromString,
                 )
         self.ProcessMessage = channel.stream_unary(
                 '/fdbwriter.Writer/ProcessMessage',
                 request_serializer=nucliadb__protos_dot_writer__pb2.BrokerMessage.SerializeToString,
                 response_deserializer=nucliadb__protos_dot_writer__pb2.OpStatusWriter.FromString,
                 )
-        self.GetLabels = channel.unary_unary(
-                '/fdbwriter.Writer/GetLabels',
-                request_serializer=nucliadb__protos_dot_writer__pb2.GetLabelsRequest.SerializeToString,
-                response_deserializer=nucliadb__protos_dot_writer__pb2.GetLabelsResponse.FromString,
-                )
-        self.GetLabelSet = channel.unary_unary(
-                '/fdbwriter.Writer/GetLabelSet',
-                request_serializer=nucliadb__protos_dot_writer__pb2.GetLabelSetRequest.SerializeToString,
-                response_deserializer=nucliadb__protos_dot_writer__pb2.GetLabelSetResponse.FromString,
-                )
-        self.SetLabels = channel.unary_unary(
-                '/fdbwriter.Writer/SetLabels',
-                request_serializer=nucliadb__protos_dot_writer__pb2.SetLabelsRequest.SerializeToString,
-                response_deserializer=nucliadb__protos_dot_writer__pb2.OpStatusWriter.FromString,
-                )
-        self.DelLabels = channel.unary_unary(
-                '/fdbwriter.Writer/DelLabels',
-                request_serializer=nucliadb__protos_dot_writer__pb2.DelLabelsRequest.SerializeToString,
-                response_deserializer=nucliadb__protos_dot_writer__pb2.OpStatusWriter.FromString,
-                )
         self.NewEntitiesGroup = channel.unary_unary(
                 '/fdbwriter.Writer/NewEntitiesGroup',
                 request_serializer=nucliadb__protos_dot_writer__pb2.NewEntitiesGroupRequest.SerializeToString,
                 response_deserializer=nucliadb__protos_dot_writer__pb2.NewEntitiesGroupResponse.FromString,
                 )
         self.GetEntities = channel.unary_unary(
                 '/fdbwriter.Writer/GetEntities',
@@ -126,14 +106,24 @@
                 response_deserializer=nucliadb__protos_dot_writer__pb2.BinaryData.FromString,
                 )
         self.UploadFile = channel.stream_unary(
                 '/fdbwriter.Writer/UploadFile',
                 request_serializer=nucliadb__protos_dot_writer__pb2.UploadBinaryData.SerializeToString,
                 response_deserializer=nucliadb__protos_dot_writer__pb2.FileUploaded.FromString,
                 )
+        self.NewVectorSet = channel.unary_unary(
+                '/fdbwriter.Writer/NewVectorSet',
+                request_serializer=nucliadb__protos_dot_writer__pb2.NewVectorSetRequest.SerializeToString,
+                response_deserializer=nucliadb__protos_dot_writer__pb2.NewVectorSetResponse.FromString,
+                )
+        self.DelVectorSet = channel.unary_unary(
+                '/fdbwriter.Writer/DelVectorSet',
+                request_serializer=nucliadb__protos_dot_writer__pb2.DelVectorSetRequest.SerializeToString,
+                response_deserializer=nucliadb__protos_dot_writer__pb2.DelVectorSetResponse.FromString,
+                )
 
 
 class WriterServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def NewKnowledgeBox(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -167,39 +157,14 @@
 
     def ProcessMessage(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetLabels(self, request, context):
-        """Labels
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def GetLabelSet(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def SetLabels(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def DelLabels(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def NewEntitiesGroup(self, request, context):
         """Entities
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -271,14 +236,26 @@
 
     def UploadFile(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def NewVectorSet(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DelVectorSet(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_WriterServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'NewKnowledgeBox': grpc.unary_unary_rpc_method_handler(
                     servicer.NewKnowledgeBox,
                     request_deserializer=nucliadb__protos_dot_knowledgebox__pb2.KnowledgeBoxNew.FromString,
                     response_serializer=nucliadb__protos_dot_knowledgebox__pb2.NewKnowledgeBoxResponse.SerializeToString,
@@ -304,34 +281,14 @@
                     response_serializer=nucliadb__protos_dot_writer__pb2.SetVectorsResponse.SerializeToString,
             ),
             'ProcessMessage': grpc.stream_unary_rpc_method_handler(
                     servicer.ProcessMessage,
                     request_deserializer=nucliadb__protos_dot_writer__pb2.BrokerMessage.FromString,
                     response_serializer=nucliadb__protos_dot_writer__pb2.OpStatusWriter.SerializeToString,
             ),
-            'GetLabels': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetLabels,
-                    request_deserializer=nucliadb__protos_dot_writer__pb2.GetLabelsRequest.FromString,
-                    response_serializer=nucliadb__protos_dot_writer__pb2.GetLabelsResponse.SerializeToString,
-            ),
-            'GetLabelSet': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetLabelSet,
-                    request_deserializer=nucliadb__protos_dot_writer__pb2.GetLabelSetRequest.FromString,
-                    response_serializer=nucliadb__protos_dot_writer__pb2.GetLabelSetResponse.SerializeToString,
-            ),
-            'SetLabels': grpc.unary_unary_rpc_method_handler(
-                    servicer.SetLabels,
-                    request_deserializer=nucliadb__protos_dot_writer__pb2.SetLabelsRequest.FromString,
-                    response_serializer=nucliadb__protos_dot_writer__pb2.OpStatusWriter.SerializeToString,
-            ),
-            'DelLabels': grpc.unary_unary_rpc_method_handler(
-                    servicer.DelLabels,
-                    request_deserializer=nucliadb__protos_dot_writer__pb2.DelLabelsRequest.FromString,
-                    response_serializer=nucliadb__protos_dot_writer__pb2.OpStatusWriter.SerializeToString,
-            ),
             'NewEntitiesGroup': grpc.unary_unary_rpc_method_handler(
                     servicer.NewEntitiesGroup,
                     request_deserializer=nucliadb__protos_dot_writer__pb2.NewEntitiesGroupRequest.FromString,
                     response_serializer=nucliadb__protos_dot_writer__pb2.NewEntitiesGroupResponse.SerializeToString,
             ),
             'GetEntities': grpc.unary_unary_rpc_method_handler(
                     servicer.GetEntities,
@@ -389,14 +346,24 @@
                     response_serializer=nucliadb__protos_dot_writer__pb2.BinaryData.SerializeToString,
             ),
             'UploadFile': grpc.stream_unary_rpc_method_handler(
                     servicer.UploadFile,
                     request_deserializer=nucliadb__protos_dot_writer__pb2.UploadBinaryData.FromString,
                     response_serializer=nucliadb__protos_dot_writer__pb2.FileUploaded.SerializeToString,
             ),
+            'NewVectorSet': grpc.unary_unary_rpc_method_handler(
+                    servicer.NewVectorSet,
+                    request_deserializer=nucliadb__protos_dot_writer__pb2.NewVectorSetRequest.FromString,
+                    response_serializer=nucliadb__protos_dot_writer__pb2.NewVectorSetResponse.SerializeToString,
+            ),
+            'DelVectorSet': grpc.unary_unary_rpc_method_handler(
+                    servicer.DelVectorSet,
+                    request_deserializer=nucliadb__protos_dot_writer__pb2.DelVectorSetRequest.FromString,
+                    response_serializer=nucliadb__protos_dot_writer__pb2.DelVectorSetResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'fdbwriter.Writer', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -502,82 +469,14 @@
         return grpc.experimental.stream_unary(request_iterator, target, '/fdbwriter.Writer/ProcessMessage',
             nucliadb__protos_dot_writer__pb2.BrokerMessage.SerializeToString,
             nucliadb__protos_dot_writer__pb2.OpStatusWriter.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetLabels(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fdbwriter.Writer/GetLabels',
-            nucliadb__protos_dot_writer__pb2.GetLabelsRequest.SerializeToString,
-            nucliadb__protos_dot_writer__pb2.GetLabelsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetLabelSet(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fdbwriter.Writer/GetLabelSet',
-            nucliadb__protos_dot_writer__pb2.GetLabelSetRequest.SerializeToString,
-            nucliadb__protos_dot_writer__pb2.GetLabelSetResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def SetLabels(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fdbwriter.Writer/SetLabels',
-            nucliadb__protos_dot_writer__pb2.SetLabelsRequest.SerializeToString,
-            nucliadb__protos_dot_writer__pb2.OpStatusWriter.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def DelLabels(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fdbwriter.Writer/DelLabels',
-            nucliadb__protos_dot_writer__pb2.DelLabelsRequest.SerializeToString,
-            nucliadb__protos_dot_writer__pb2.OpStatusWriter.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def NewEntitiesGroup(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -789,7 +688,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.stream_unary(request_iterator, target, '/fdbwriter.Writer/UploadFile',
             nucliadb__protos_dot_writer__pb2.UploadBinaryData.SerializeToString,
             nucliadb__protos_dot_writer__pb2.FileUploaded.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def NewVectorSet(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/fdbwriter.Writer/NewVectorSet',
+            nucliadb__protos_dot_writer__pb2.NewVectorSetRequest.SerializeToString,
+            nucliadb__protos_dot_writer__pb2.NewVectorSetResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DelVectorSet(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/fdbwriter.Writer/DelVectorSet',
+            nucliadb__protos_dot_writer__pb2.DelVectorSetRequest.SerializeToString,
+            nucliadb__protos_dot_writer__pb2.DelVectorSetResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/nucliadb_protos/writer_pb2_grpc.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -190,35 +190,14 @@
     ]
 
     ProcessMessage: grpc.StreamUnaryMultiCallable[
         nucliadb_protos.writer_pb2.BrokerMessage,
         nucliadb_protos.writer_pb2.OpStatusWriter,
     ]
 
-    GetLabels: grpc.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.GetLabelsRequest,
-        nucliadb_protos.writer_pb2.GetLabelsResponse,
-    ]
-    """Labels"""
-
-    GetLabelSet: grpc.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.GetLabelSetRequest,
-        nucliadb_protos.writer_pb2.GetLabelSetResponse,
-    ]
-
-    SetLabels: grpc.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.SetLabelsRequest,
-        nucliadb_protos.writer_pb2.OpStatusWriter,
-    ]
-
-    DelLabels: grpc.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.DelLabelsRequest,
-        nucliadb_protos.writer_pb2.OpStatusWriter,
-    ]
-
     NewEntitiesGroup: grpc.UnaryUnaryMultiCallable[
         nucliadb_protos.writer_pb2.NewEntitiesGroupRequest,
         nucliadb_protos.writer_pb2.NewEntitiesGroupResponse,
     ]
     """Entities"""
 
     GetEntities: grpc.UnaryUnaryMultiCallable[
@@ -277,14 +256,24 @@
     ]
 
     UploadFile: grpc.StreamUnaryMultiCallable[
         nucliadb_protos.writer_pb2.UploadBinaryData,
         nucliadb_protos.writer_pb2.FileUploaded,
     ]
 
+    NewVectorSet: grpc.UnaryUnaryMultiCallable[
+        nucliadb_protos.writer_pb2.NewVectorSetRequest,
+        nucliadb_protos.writer_pb2.NewVectorSetResponse,
+    ]
+
+    DelVectorSet: grpc.UnaryUnaryMultiCallable[
+        nucliadb_protos.writer_pb2.DelVectorSetRequest,
+        nucliadb_protos.writer_pb2.DelVectorSetResponse,
+    ]
+
 class WriterAsyncStub:
     NewKnowledgeBox: grpc.aio.UnaryUnaryMultiCallable[
         nucliadb_protos.knowledgebox_pb2.KnowledgeBoxNew,
         nucliadb_protos.knowledgebox_pb2.NewKnowledgeBoxResponse,
     ]
 
     DeleteKnowledgeBox: grpc.aio.UnaryUnaryMultiCallable[
@@ -308,35 +297,14 @@
     ]
 
     ProcessMessage: grpc.aio.StreamUnaryMultiCallable[
         nucliadb_protos.writer_pb2.BrokerMessage,
         nucliadb_protos.writer_pb2.OpStatusWriter,
     ]
 
-    GetLabels: grpc.aio.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.GetLabelsRequest,
-        nucliadb_protos.writer_pb2.GetLabelsResponse,
-    ]
-    """Labels"""
-
-    GetLabelSet: grpc.aio.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.GetLabelSetRequest,
-        nucliadb_protos.writer_pb2.GetLabelSetResponse,
-    ]
-
-    SetLabels: grpc.aio.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.SetLabelsRequest,
-        nucliadb_protos.writer_pb2.OpStatusWriter,
-    ]
-
-    DelLabels: grpc.aio.UnaryUnaryMultiCallable[
-        nucliadb_protos.writer_pb2.DelLabelsRequest,
-        nucliadb_protos.writer_pb2.OpStatusWriter,
-    ]
-
     NewEntitiesGroup: grpc.aio.UnaryUnaryMultiCallable[
         nucliadb_protos.writer_pb2.NewEntitiesGroupRequest,
         nucliadb_protos.writer_pb2.NewEntitiesGroupResponse,
     ]
     """Entities"""
 
     GetEntities: grpc.aio.UnaryUnaryMultiCallable[
@@ -395,14 +363,24 @@
     ]
 
     UploadFile: grpc.aio.StreamUnaryMultiCallable[
         nucliadb_protos.writer_pb2.UploadBinaryData,
         nucliadb_protos.writer_pb2.FileUploaded,
     ]
 
+    NewVectorSet: grpc.aio.UnaryUnaryMultiCallable[
+        nucliadb_protos.writer_pb2.NewVectorSetRequest,
+        nucliadb_protos.writer_pb2.NewVectorSetResponse,
+    ]
+
+    DelVectorSet: grpc.aio.UnaryUnaryMultiCallable[
+        nucliadb_protos.writer_pb2.DelVectorSetRequest,
+        nucliadb_protos.writer_pb2.DelVectorSetResponse,
+    ]
+
 class WriterServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def NewKnowledgeBox(
         self,
         request: nucliadb_protos.knowledgebox_pb2.KnowledgeBoxNew,
         context: _ServicerContext,
     ) -> typing.Union[nucliadb_protos.knowledgebox_pb2.NewKnowledgeBoxResponse, collections.abc.Awaitable[nucliadb_protos.knowledgebox_pb2.NewKnowledgeBoxResponse]]: ...
@@ -439,43 +417,14 @@
     def ProcessMessage(
         self,
         request_iterator: _MaybeAsyncIterator[nucliadb_protos.writer_pb2.BrokerMessage],
         context: _ServicerContext,
     ) -> typing.Union[nucliadb_protos.writer_pb2.OpStatusWriter, collections.abc.Awaitable[nucliadb_protos.writer_pb2.OpStatusWriter]]: ...
 
     @abc.abstractmethod
-    def GetLabels(
-        self,
-        request: nucliadb_protos.writer_pb2.GetLabelsRequest,
-        context: _ServicerContext,
-    ) -> typing.Union[nucliadb_protos.writer_pb2.GetLabelsResponse, collections.abc.Awaitable[nucliadb_protos.writer_pb2.GetLabelsResponse]]:
-        """Labels"""
-
-    @abc.abstractmethod
-    def GetLabelSet(
-        self,
-        request: nucliadb_protos.writer_pb2.GetLabelSetRequest,
-        context: _ServicerContext,
-    ) -> typing.Union[nucliadb_protos.writer_pb2.GetLabelSetResponse, collections.abc.Awaitable[nucliadb_protos.writer_pb2.GetLabelSetResponse]]: ...
-
-    @abc.abstractmethod
-    def SetLabels(
-        self,
-        request: nucliadb_protos.writer_pb2.SetLabelsRequest,
-        context: _ServicerContext,
-    ) -> typing.Union[nucliadb_protos.writer_pb2.OpStatusWriter, collections.abc.Awaitable[nucliadb_protos.writer_pb2.OpStatusWriter]]: ...
-
-    @abc.abstractmethod
-    def DelLabels(
-        self,
-        request: nucliadb_protos.writer_pb2.DelLabelsRequest,
-        context: _ServicerContext,
-    ) -> typing.Union[nucliadb_protos.writer_pb2.OpStatusWriter, collections.abc.Awaitable[nucliadb_protos.writer_pb2.OpStatusWriter]]: ...
-
-    @abc.abstractmethod
     def NewEntitiesGroup(
         self,
         request: nucliadb_protos.writer_pb2.NewEntitiesGroupRequest,
         context: _ServicerContext,
     ) -> typing.Union[nucliadb_protos.writer_pb2.NewEntitiesGroupResponse, collections.abc.Awaitable[nucliadb_protos.writer_pb2.NewEntitiesGroupResponse]]:
         """Entities"""
 
@@ -559,8 +508,22 @@
     @abc.abstractmethod
     def UploadFile(
         self,
         request_iterator: _MaybeAsyncIterator[nucliadb_protos.writer_pb2.UploadBinaryData],
         context: _ServicerContext,
     ) -> typing.Union[nucliadb_protos.writer_pb2.FileUploaded, collections.abc.Awaitable[nucliadb_protos.writer_pb2.FileUploaded]]: ...
 
+    @abc.abstractmethod
+    def NewVectorSet(
+        self,
+        request: nucliadb_protos.writer_pb2.NewVectorSetRequest,
+        context: _ServicerContext,
+    ) -> typing.Union[nucliadb_protos.writer_pb2.NewVectorSetResponse, collections.abc.Awaitable[nucliadb_protos.writer_pb2.NewVectorSetResponse]]: ...
+
+    @abc.abstractmethod
+    def DelVectorSet(
+        self,
+        request: nucliadb_protos.writer_pb2.DelVectorSetRequest,
+        context: _ServicerContext,
+    ) -> typing.Union[nucliadb_protos.writer_pb2.DelVectorSetResponse, collections.abc.Awaitable[nucliadb_protos.writer_pb2.DelVectorSetResponse]]: ...
+
 def add_WriterServicer_to_server(servicer: WriterServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None: ...
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/python/setup.py` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/python/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/reader.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/reader.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/replication.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/replication.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/resources.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/resources.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/standalone.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/standalone.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/train.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/train.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/utils.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/utils.proto`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/nucliadb_protos/writer.proto` & `nucliadb_node_binding-4.0.3.post1388/nucliadb_protos/writer.proto`

 * *Files 3% similar despite different names*

```diff
@@ -143,39 +143,15 @@
     // map of last message processed
     map<string, int64> msgid = 2;
 }
 
 message WriterStatusRequest {
 }
 
-message SetLabelsRequest {
-    knowledgebox.KnowledgeBoxID kb = 1;
-    string id = 2;
-    knowledgebox.LabelSet labelset = 3;
-}
-
-message DelLabelsRequest {
-    knowledgebox.KnowledgeBoxID kb = 1;
-    string id = 2;
-}
-
-message GetLabelsResponse {
-    knowledgebox.KnowledgeBoxID kb = 1;
-    knowledgebox.Labels labels = 2;
-    enum Status {
-        OK = 0;
-        NOTFOUND = 1;
-    }
-    Status status = 3;
 
-}
-
-message GetLabelsRequest {
-    knowledgebox.KnowledgeBoxID kb = 1;
-}
 
 message NewEntitiesGroupRequest {
     knowledgebox.KnowledgeBoxID kb = 1;
     string group = 2;
     knowledgebox.EntitiesGroup entities = 3;
 }
 
@@ -265,29 +241,27 @@
         string entity = 2;
     }
     knowledgebox.KnowledgeBoxID kb = 1;
     EntityID from = 2;
     EntityID to = 3;
 }
 
-message GetLabelSetRequest {
-    knowledgebox.KnowledgeBoxID kb = 1;
-    string labelset = 2;
-}
-
-message GetLabelSetResponse {
+message GetLabelsResponse {
     knowledgebox.KnowledgeBoxID kb = 1;
-    knowledgebox.LabelSet labelset = 2;
+    knowledgebox.Labels labels = 2;
     enum Status {
         OK = 0;
         NOTFOUND = 1;
     }
     Status status = 3;
 }
 
+message GetLabelsRequest {
+    knowledgebox.KnowledgeBoxID kb = 1;
+}
 
 message GetEntitiesGroupRequest {
     knowledgebox.KnowledgeBoxID kb = 1;
     string group = 2;
 }
 
 message GetEntitiesGroupResponse {
@@ -313,25 +287,14 @@
         OK = 0;
         NOTFOUND = 1;
         ERROR = 2;
     }
     Status status = 3;
 }
 
-message DelVectorSetRequest {
-    knowledgebox.KnowledgeBoxID kb = 1;
-    string vectorset = 2;
-}
-
-message SetVectorSetRequest {
-    knowledgebox.KnowledgeBoxID kb = 1;
-    string id = 2;
-    knowledgebox.VectorSet vectorset = 3;
-}
-
 message OpStatusWriter {
     enum Status {
         OK = 0;
         ERROR = 1;
         NOTFOUND = 2;
     }
     Status status = 1;
@@ -490,30 +453,58 @@
 
 }
 
 message SynonymsRequest {
     string kbid = 1;
 }
 
+message NewVectorSetRequest {
+    string kbid = 1;
+    string vectorset_id = 2;
+    nodewriter.VectorType vector_type = 3;
+    utils.VectorSimilarity similarity = 4;
+    uint32 vector_dimension = 5;
+    bool normalize_vectors = 6;
+    repeated uint32 matryoshka_dimensions = 7;
+}
+
+message NewVectorSetResponse {
+    enum Status {
+        OK = 0;
+        ERROR = 1;              // generic error
+    }
+    Status status = 1;
+    string details = 2;
+}
+
+message DelVectorSetRequest {
+    string kbid = 1;
+    string vectorset_id = 2;
+}
+
+message DelVectorSetResponse {
+    enum Status {
+        OK = 0;
+        ERROR = 1;              // generic error
+    }
+    Status status = 1;
+    string details = 2;
+}
+
+
 
 service Writer {
     rpc NewKnowledgeBox(knowledgebox.KnowledgeBoxNew) returns (knowledgebox.NewKnowledgeBoxResponse) {}
     rpc DeleteKnowledgeBox(knowledgebox.KnowledgeBoxID) returns (knowledgebox.DeleteKnowledgeBoxResponse) {}
     rpc UpdateKnowledgeBox(knowledgebox.KnowledgeBoxUpdate) returns (knowledgebox.UpdateKnowledgeBoxResponse) {}
     rpc GCKnowledgeBox(knowledgebox.KnowledgeBoxID) returns (knowledgebox.GCKnowledgeBoxResponse) {}
     rpc SetVectors(SetVectorsRequest) returns (SetVectorsResponse) {}
 
     rpc ProcessMessage(stream BrokerMessage) returns (OpStatusWriter) {}
 
-    // Labels
-    rpc GetLabels(GetLabelsRequest) returns (GetLabelsResponse) {}
-    rpc GetLabelSet(GetLabelSetRequest) returns (GetLabelSetResponse) {}
-    rpc SetLabels(SetLabelsRequest) returns (OpStatusWriter) {}
-    rpc DelLabels(DelLabelsRequest) returns (OpStatusWriter) {}
-
     // Entities
     rpc NewEntitiesGroup(NewEntitiesGroupRequest) returns (NewEntitiesGroupResponse) {}
     rpc GetEntities(GetEntitiesRequest) returns (GetEntitiesResponse) {}
     rpc GetEntitiesGroup(GetEntitiesGroupRequest) returns (GetEntitiesGroupResponse) {}
     rpc ListEntitiesGroups(ListEntitiesGroupsRequest) returns (ListEntitiesGroupsResponse) {}
     rpc SetEntities(SetEntitiesRequest) returns (OpStatusWriter) {}
     rpc UpdateEntitiesGroup(UpdateEntitiesGroupRequest) returns (UpdateEntitiesGroupResponse) {}
@@ -524,8 +515,11 @@
     rpc ListMembers(ListMembersRequest) returns (ListMembersResponse);
 
     rpc Index(IndexResource) returns (IndexStatus) {}
     rpc ReIndex(IndexResource) returns (IndexStatus) {}
 
     rpc DownloadFile(FileRequest) returns (stream BinaryData) {}
     rpc UploadFile(stream UploadBinaryData) returns (FileUploaded) {}
+
+    rpc NewVectorSet(NewVectorSetRequest) returns (NewVectorSetResponse) {}
+    rpc DelVectorSet(DelVectorSetRequest) returns (DelVectorSetResponse) {}
 }
```

### Comparing `nucliadb_node_binding-4.0.1.post1382/pyproject.toml` & `nucliadb_node_binding-4.0.3.post1388/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/src/collect_garbage.rs` & `nucliadb_node_binding-4.0.3.post1388/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/src/errors.rs` & `nucliadb_node_binding-4.0.3.post1388/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/src/lib.rs` & `nucliadb_node_binding-4.0.3.post1388/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/src/reader.rs` & `nucliadb_node_binding-4.0.3.post1388/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/src/update.rs` & `nucliadb_node_binding-4.0.3.post1388/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/src/writer.rs` & `nucliadb_node_binding-4.0.3.post1388/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/tests/__init__.py` & `nucliadb_node_binding-4.0.3.post1388/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/tests/conftest.py` & `nucliadb_node_binding-4.0.3.post1388/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-4.0.1.post1382/tests/integration/test_indexing.py` & `nucliadb_node_binding-4.0.3.post1388/tests/integration/test_indexing.py`

 * *Files identical despite different names*

