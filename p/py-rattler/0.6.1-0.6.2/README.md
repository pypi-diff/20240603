# Comparing `tmp/py_rattler-0.6.1.tar.gz` & `tmp/py_rattler-0.6.2.tar.gz`

## Comparing `py_rattler-0.6.1.tar` & `py_rattler-0.6.2.tar`

### file list

```diff
@@ -1,493 +1,494 @@
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/Cargo.toml
--rw-r--r--   0     1001      127     4319 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/CHANGELOG.md
--rw-r--r--   0     1001      127     2053 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/fs.rs
--rw-r--r--   0     1001      127     2392 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/lib.rs
--rw-r--r--   0     1001      127     3671 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/read.rs
--rw-r--r--   0     1001      127       98 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/reqwest/mod.rs
--rw-r--r--   0     1001      127     6148 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs
--rw-r--r--   0     1001      127     4387 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/seek.rs
--rw-r--r--   0     1001      127     1732 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs
--rw-r--r--   0     1001      127     3101 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/fs.rs
--rw-r--r--   0     1001      127      113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/mod.rs
--rw-r--r--   0     1001      127    14225 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/write.rs
--rw-r--r--   0     1001      127     9266 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/extract.rs
--rw-r--r--   0     1001      127     7864 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/write.rs
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/Cargo.toml
--rw-r--r--   0     1001      127     3970 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/CHANGELOG.md
--rw-r--r--   0     1001      127     8878 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/builder.rs
--rw-r--r--   0     1001      127      871 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/channel.rs
--rw-r--r--   0     1001      127     5792 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/conda.rs
--rw-r--r--   0     1001      127     2006 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/file_format_version.rs
--rw-r--r--   0     1001      127     4879 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/hash.rs
--rw-r--r--   0     1001      127    24726 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/lib.rs
--rw-r--r--   0     1001      127     6083 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/deserialize.rs
--rw-r--r--   0     1001      127     2613 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/mod.rs
--rw-r--r--   0     1001      127     9114 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/serialize.rs
--rw-r--r--   0     1001      127     8677 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/v3.rs
--rw-r--r--   0     1001      127     5293 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi.rs
--rw-r--r--   0     1001      127     1480 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi_indexes.rs
--rw-r--r--   0     1001      127    15803 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap
--rw-r--r--   0     1001      127    22538 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap
--rw-r--r--   0     1001      127   487177 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap
--rw-r--r--   0     1001      127    40002 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap
--rw-r--r--   0     1001      127    52187 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap
--rw-r--r--   0     1001      127  1811359 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap
--rw-r--r--   0     1001      127   487177 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap
--rw-r--r--   0     1001      127    19608 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap
--rw-r--r--   0     1001      127    40002 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap
--rw-r--r--   0     1001      127    52187 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap
--rw-r--r--   0     1001      127  1811359 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap
--rw-r--r--   0     1001      127    10278 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap
--rw-r--r--   0     1001      127   242145 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap
--rw-r--r--   0     1001      127     6457 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/url_or_path.rs
--rw-r--r--   0     1001      127       22 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/mod.rs
--rw-r--r--   0     1001      127     1693 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs
--rw-r--r--   0     1001      127      372 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/mod.rs
--rw-r--r--   0     1001      127     2012 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/ordered.rs
--rw-r--r--   0     1001      127     1609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs
--rw-r--r--   0     1001      127     7980 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs
--rw-r--r--   0     1001      127     1441 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs
--rw-r--r--   0     1001      127     1407 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/Cargo.toml
--rw-r--r--   0     1001      127     4535 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/CHANGELOG.md
--rw-r--r--   0     1001      127     2806 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs
--rw-r--r--   0     1001      127     7713 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs
--rw-r--r--   0     1001      127      956 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap
--rw-r--r--   0     1001      127      465 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_one.snap
--rw-r--r--   0     1001      127      604 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap
--rw-r--r--   0     1001      127    38981 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs
--rw-r--r--   0     1001      127    52612 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs
--rw-r--r--   0     1001      127     3926 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs
--rw-r--r--   0     1001      127     3219 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs
--rw-r--r--   0     1001      127     1738 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs
--rw-r--r--   0     1001      127     2627 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs
--rw-r--r--   0     1001      127     2335 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs
--rw-r--r--   0     1001      127    18116 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs
--rw-r--r--   0     1001      127     8435 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs
--rw-r--r--   0     1001      127     2409 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs
--rw-r--r--   0     1001      127     2377 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs
--rw-r--r--   0     1001      127    13060 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs
--rw-r--r--   0     1001      127     8026 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs
--rw-r--r--   0     1001      127     5798 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs
--rw-r--r--   0     1001      127     6178 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs
--rw-r--r--   0     1001      127     2151 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/lib.rs
--rw-r--r--   0     1001      127     3977 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/reporter.rs
--rw-r--r--   0     1001      127    22540 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs
--rw-r--r--   0     1001      127     2167 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/body.rs
--rw-r--r--   0     1001      127     2718 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs
--rw-r--r--   0     1001      127    13393 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs
--rw-r--r--   0     1001      127     1715 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs
--rw-r--r--   0     1001      127     2609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/Cargo.toml
--rw-r--r--   0     1001      127      987 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/CHANGELOG.md
--rw-r--r--   0     1001      127     2664 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/src/lib.rs
--rw-r--r--   0     1001      127      113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/01-sorted-enum.rs
--rw-r--r--   0     1001      127      155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/02-sorted-struct.rs
--rw-r--r--   0     1001      127      113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/03-out-of-order-enum.rs
--rw-r--r--   0     1001      127      127 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/03-out-of-order-enum.stderr
--rw-r--r--   0     1001      127      155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/04-out-of-order-struct.rs
--rw-r--r--   0     1001      127      137 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/04-out-of-order-struct.stderr
--rw-r--r--   0     1001      127      251 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_macros/tests/tests.rs
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/Cargo.toml
--rw-r--r--   0     1001      127     1233 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/CHANGELOG.md
--rw-r--r--   0     1001      127     7607 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/src/lib.rs
--rw-r--r--   0     1001      127     4014 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/src/serde.rs
--rw-r--r--   0     1001      127     2155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_digest/src/tokio.rs
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/Cargo.toml
--rw-r--r--   0     1001      127     3627 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/CHANGELOG.md
--rw-r--r--   0     1001      127    14736 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_middleware.rs
--rw-r--r--   0     1001      127     1266 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs
--rw-r--r--   0     1001      127     6690 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs
--rw-r--r--   0     1001      127     2852 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs
--rw-r--r--   0     1001      127      103 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/mod.rs
--rw-r--r--   0     1001      127     5769 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs
--rw-r--r--   0     1001      127      270 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/snapshots/rattler_networking__authentication_storage__backends__file__tests__file_storage.snap
--rw-r--r--   0     1001      127      727 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/mod.rs
--rw-r--r--   0     1001      127     6830 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/storage.rs
--rw-r--r--   0     1001      127     2287 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/gcs_middleware.rs
--rw-r--r--   0     1001      127      726 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/lib.rs
--rw-r--r--   0     1001      127    10298 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/mirror_middleware.rs
--rw-r--r--   0     1001      127    10902 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/oci_middleware.rs
--rw-r--r--   0     1001      127     3489 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/redaction.rs
--rw-r--r--   0     1001      127      920 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_networking/src/retry_policies.rs
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/file_url/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/file_url/.gitignore
--rw-r--r--   0     1001      127      486 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/file_url/CHANGELOG.md
--rw-r--r--   0     1001      127     7791 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/file_url/src/lib.rs
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_index/Cargo.toml
--rw-r--r--   0     1001      127     3536 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_index/CHANGELOG.md
--rw-r--r--   0     1001      127     6989 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_index/src/lib.rs
--rw-r--r--   0     1001      127     2162 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_index/tests/test_index.rs
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/Cargo.toml
--rw-r--r--   0     1001      127     1011 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/CHANGELOG.md
--rw-r--r--   0     1001      127     1394 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/build.rs
--rw-r--r--   0     1001      127    77341 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/src/lib.rs
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/Cargo.toml
--rw-r--r--   0     1001      127     5252 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/CHANGELOG.md
--rw-r--r--   0     1001      127     1016 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/benches/parse.rs
--rw-r--r--   0     1001      127     3220 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/mod.rs
--rw-r--r--   0     1001      127     6519 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/parse.rs
--rw-r--r--   0     1001      127    23177 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel/mod.rs
--rw-r--r--   0     1001      127     4187 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel_data.rs
--rw-r--r--   0     1001      127    11580 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs
--rw-r--r--   0     1001      127      770 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs
--rw-r--r--   0     1001      127     2299 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/lib.rs
--rw-r--r--   0     1001      127     6012 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs
--rw-r--r--   0     1001      127    20372 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/mod.rs
--rw-r--r--   0     1001      127    28472 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/parse.rs
--rw-r--r--   0     1001      127      506 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__parse__tests__parsed matchspecs.snap
--rw-r--r--   0     1001      127      537 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap
--rw-r--r--   0     1001      127     5728 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/no_arch_type.rs
--rw-r--r--   0     1001      127     3206 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/about.rs
--rw-r--r--   0     1001      127     4183 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs
--rw-r--r--   0     1001      127     1400 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_type.rs
--rw-r--r--   0     1001      127     3244 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/entry_point.rs
--rw-r--r--   0     1001      127     1348 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/files.rs
--rw-r--r--   0     1001      127     6460 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/has_prefix.rs
--rw-r--r--   0     1001      127     3942 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/index.rs
--rw-r--r--   0     1001      127     1977 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/link.rs
--rw-r--r--   0     1001      127     3607 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/mod.rs
--rw-r--r--   0     1001      127     1510 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_link.rs
--rw-r--r--   0     1001      127     1495 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_softlink.rs
--rw-r--r--   0     1001      127      507 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/package_metadata.rs
--rw-r--r--   0     1001      127    12387 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/paths.rs
--rw-r--r--   0     1001      127     2780 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/run_exports.rs
--rw-r--r--   0     1001      127      754 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap
--rw-r--r--   0     1001      127     2515 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap
--rw-r--r--   0     1001      127      134 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__entry_point__test__entry_point.snap
--rw-r--r--   0     1001      127      329 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json.snap
--rw-r--r--   0     1001      127      309 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json_with_symlinks.snap
--rw-r--r--   0     1001      127      349 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__jupyterlab-link.json.snap
--rw-r--r--   0     1001      127      137 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__setuptools-link.json.snap
--rw-r--r--   0     1001      127      138 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__tzdata-link.json.snap
--rw-r--r--   0     1001      127     1171 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap
--rw-r--r--   0     1001      127      776 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap
--rw-r--r--   0     1001      127      601 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap
--rw-r--r--   0     1001      127     6782 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap
--rw-r--r--   0     1001      127      185 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__run_exports__test__reconstruct_run_exports_json_with_symlinks.snap
--rw-r--r--   0     1001      127     5305 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package_name.rs
--rw-r--r--   0     1001      127      233 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/parse_mode.rs
--rw-r--r--   0     1001      127    15923 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/platform.rs
--rw-r--r--   0     1001      127    12758 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/prefix_record.rs
--rw-r--r--   0     1001      127    20250 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/mod.rs
--rw-r--r--   0     1001      127    11158 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/patches.rs
--rw-r--r--   0     1001      127     1554 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs
--rw-r--r--   0     1001      127      181 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__null_values.snap
--rw-r--r--   0     1001      127     2154 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap
--rw-r--r--   0     1001      127     2091 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap
--rw-r--r--   0     1001      127      843 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap
--rw-r--r--   0     1001      127     1595 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap
--rw-r--r--   0     1001      127      873 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap
--rw-r--r--   0     1001      127     4832 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap
--rw-r--r--   0     1001      127      232 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize.snap
--rw-r--r--   0     1001      127     6461 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap
--rw-r--r--   0     1001      127     5154 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap
--rw-r--r--   0     1001      127    77589 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs
--rw-r--r--   0     1001      127     1063 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data_record.rs
--rw-r--r--   0     1001      127      455 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/run_export.rs
--rw-r--r--   0     1001      127    53039 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap
--rw-r--r--   0     1001      127      353 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__vs2015_runtime_win-64.txt.snap
--rw-r--r--   0     1001      127      974 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap
--rw-r--r--   0     1001      127     2269 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap
--rw-r--r--   0     1001      127    12047 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap
--rw-r--r--   0     1001      127   269415 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     4590 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap
--rw-r--r--   0     1001      127    12519 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127   345345 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap
--rw-r--r--   0     1001      127    23076 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     1054 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap
--rw-r--r--   0     1001      127    12151 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     7102 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap
--rw-r--r--   0     1001      127       22 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/utils/mod.rs
--rw-r--r--   0     1001      127     6107 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/utils/serde.rs
--rw-r--r--   0     1001      127     8204 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/bump.rs
--rw-r--r--   0     1001      127     3760 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/flags.rs
--rw-r--r--   0     1001      127    46846 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/mod.rs
--rw-r--r--   0     1001      127    18817 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/parse.rs
--rw-r--r--   0     1001      127     6410 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/segment.rs
--rw-r--r--   0     1001      127     2495 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap
--rw-r--r--   0     1001      127     4817 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/with_source.rs
--rw-r--r--   0     1001      127    10262 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs
--rw-r--r--   0     1001      127    19332 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/mod.rs
--rw-r--r--   0     1001      127    18092 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/parse.rs
--rw-r--r--   0     1001      127    15169 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/Cargo.toml
--rw-r--r--   0     1001      127     3218 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/CHANGELOG.md
--rw-r--r--   0     1001      127    27911 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/activation.rs
--rw-r--r--   0     1001      127      196 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/lib.rs
--rw-r--r--   0     1001      127     2232 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/run/mod.rs
--rw-r--r--   0     1001      127    28467 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/mod.rs
--rw-r--r--   0     1001      127      123 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__bash.snap
--rw-r--r--   0     1001      127      128 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__fish.snap
--rw-r--r--   0     1001      127      104 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_bash.snap
--rw-r--r--   0     1001      127      122 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_xsh.snap
--rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_bash.snap
--rw-r--r--   0     1001      127      185 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_cmd.snap
--rw-r--r--   0     1001      127      190 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_fish.snap
--rw-r--r--   0     1001      127      192 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_powershell.snap
--rw-r--r--   0     1001      127      239 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_xonsh.snap
--rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_zsh.snap
--rw-r--r--   0     1001      127      171 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__after_activation.snap
--rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_append.snap
--rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_prepend.snap
--rw-r--r--   0     1001      127      229 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_replace.snap
--rw-r--r--   0     1001      127      202 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_append.snap
--rw-r--r--   0     1001      127      202 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_prepend.snap
--rw-r--r--   0     1001      127      195 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_replace.snap
--rw-r--r--   0     1001      127      311 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_append.snap
--rw-r--r--   0     1001      127      311 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_prepend.snap
--rw-r--r--   0     1001      127      301 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_replace.snap
--rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/.gitignore
--rw-r--r--   0     1001      127     5659 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/CHANGELOG.md
--rw-r--r--   0     1001      127    74752 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/resources/launcher64.exe
--rw-r--r--   0     1001      127    99068 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/resources/versions.txt
--rw-r--r--   0     1001      127     4794 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/cli/auth.rs
--rw-r--r--   0     1001      127      122 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/cli/mod.rs
--rw-r--r--   0     1001      127     1358 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/apple_codesign.rs
--rw-r--r--   0     1001      127    35510 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/clobber_registry.rs
--rw-r--r--   0     1001      127     9786 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/driver.rs
--rw-r--r--   0     1001      127     8511 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/entry_point.rs
--rw-r--r--   0     1001      127     1666 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/error.rs
--rw-r--r--   0     1001      127    27383 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/indicatif.rs
--rw-r--r--   0     1001      127    20030 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/mod.rs
--rw-r--r--   0     1001      127     4261 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/reporter.rs
--rw-r--r--   0     1001      127    33225 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/link.rs
--rw-r--r--   0     1001      127     9691 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/link_script.rs
--rw-r--r--   0     1001      127    33679 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/mod.rs
--rw-r--r--   0     1001      127     3839 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/python.rs
--rw-r--r--   0     1001      127      609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap
--rw-r--r--   0     1001      127      190 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-3.snap
--rw-r--r--   0     1001      127      727 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap
--rw-r--r--   0     1001      127      142 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-5.snap
--rw-r--r--   0     1001      127      609 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap
--rw-r--r--   0     1001      127      727 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap
--rw-r--r--   0     1001      127      142 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber.snap
--rw-r--r--   0     1001      127      297 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__entry_point_script.snap
--rw-r--r--   0     1001      127      271 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__windows.snap
--rw-r--r--   0     1001      127      155 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__link__test__replace_long_prefix_in_text_file.snap
--rw-r--r--   0     1001      127     3732 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap
--rw-r--r--   0     1001      127     4688 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/test_utils.rs
--rw-r--r--   0     1001      127     8426 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/transaction.rs
--rw-r--r--   0     1001      127     9414 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/install/unlink.rs
--rw-r--r--   0     1001      127     2983 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/lib.rs
--rw-r--r--   0     1001      127    22292 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/package_cache.rs
--rw-r--r--   0     1001      127    24363 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/range.rs
--rw-r--r--   0     1001      127    13775 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler/src/validation.rs
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/Cargo.toml
--rw-r--r--   0     1001      127     4417 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/CHANGELOG.md
--rw-r--r--   0     1001      127     2914 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/benches/bench.rs
--rw-r--r--   0     1001      127     8738 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/lib.rs
--rw-r--r--   0     1001      127    13226 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/input.rs
--rw-r--r--   0     1001      127     1173 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs
--rw-r--r--   0     1001      127     9630 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/mod.rs
--rw-r--r--   0     1001      127     2444 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/output.rs
--rw-r--r--   0     1001      127      561 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs
--rw-r--r--   0     1001      127      864 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs
--rw-r--r--   0     1001      127     1047 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs
--rw-r--r--   0     1001      127    11669 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs
--rw-r--r--   0     1001      127     2720 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs
--rw-r--r--   0     1001      127     6299 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs
--rw-r--r--   0     1001      127     3402 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs
--rw-r--r--   0     1001      127     1262 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs
--rw-r--r--   0     1001      127     3451 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs
--rw-r--r--   0     1001      127     4718 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs
--rw-r--r--   0     1001      127     5589 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs
--rw-r--r--   0     1001      127     2468 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs
--rw-r--r--   0     1001      127     7734 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/conda_util.rs
--rw-r--r--   0     1001      127    24305 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/mod.rs
--rw-r--r--   0     1001      127    34012 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/backends.rs
--rw-r--r--   0     1001      127      165 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_dummy_repo_install_non_existent.snap
--rw-r--r--   0     1001      127      738 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap
--rw-r--r--   0     1001      127     1105 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap
--rw-r--r--   0     1001      127     3069 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap
--rw-r--r--   0     1001      127     2590 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap
--rw-r--r--   0     1001      127     3631 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap
--rw-r--r--   0     1001      127      216 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_with_error.snap
--rw-r--r--   0     1001      127      411 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_xtensor_xsimd.snap
--rw-r--r--   0     1001      127      369 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__exclude_newer_error.snap
--rw-r--r--   0     1001      127      172 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_dummy_repo_install_non_existent.snap
--rw-r--r--   0     1001      127      412 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_locked.snap
--rw-r--r--   0     1001      127      736 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap
--rw-r--r--   0     1001      127     1103 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap
--rw-r--r--   0     1001      127     3067 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap
--rw-r--r--   0     1001      127     2588 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap
--rw-r--r--   0     1001      127     3629 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap
--rw-r--r--   0     1001      127      588 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap
--rw-r--r--   0     1001      127      400 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_xtensor_xsimd.snap
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/Cargo.toml
--rw-r--r--   0     1001      127      237 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/src/lib.rs
--rw-r--r--   0     1001      127      692 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/src/tokio.rs
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/Cargo.toml
--rw-r--r--   0     1001      127     3446 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/CHANGELOG.md
--rw-r--r--   0     1001      127    11042 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/cuda.rs
--rw-r--r--   0     1001      127    12929 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/lib.rs
--rw-r--r--   0     1001      127     3047 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/libc.rs
--rw-r--r--   0     1001      127     3969 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/linux.rs
--rw-r--r--   0     1001      127     2381 2024-05-28 14:47:59.000000 py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/osx.rs
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 py_rattler-0.6.1/Cargo.toml
--rw-r--r--   0     1001      127      743 2024-05-28 14:47:59.000000 py_rattler-0.6.1/.gitignore
--rw-r--r--   0     1001      127     1502 2024-05-28 14:47:59.000000 py_rattler-0.6.1/LICENSE
--rw-r--r--   0     1001      127     6880 2024-05-28 14:47:59.000000 py_rattler-0.6.1/README.md
--rw-r--r--   0     1001      127       71 2024-05-28 14:47:59.000000 py_rattler-0.6.1/build.rs
--rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/about_json.md
--rw-r--r--   0     1001      127       45 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activate.md
--rw-r--r--   0     1001      127       58 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activation_error.md
--rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activation_result.md
--rw-r--r--   0     1001      127       67 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/activation_variables.md
--rw-r--r--   0     1001      127       34 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/arch.md
--rw-r--r--   0     1001      127       62 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/authenticated_client.md
--rw-r--r--   0     1001      127       54 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/cache_dir_error.md
--rw-r--r--   0     1001      127       39 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/channel.md
--rw-r--r--   0     1001      127       52 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/channel_config.md
--rw-r--r--   0     1001      127       79 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/detect_virtual_package_error.md
--rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/environment.md
--rw-r--r--   0     1001      127       76 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/environment_creation_error.md
--rw-r--r--   0     1001      127       58 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/fetch_repo_data.md
--rw-r--r--   0     1001      127       65 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/fetch_repo_data_error.md
--rw-r--r--   0     1001      127       51 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/file_mode.md
--rw-r--r--   0     1001      127       41 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/gateway.md
--rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/generic_virtual_package.md
--rw-r--r--   0     1001      127     5592 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/index.md
--rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/index_json.md
--rw-r--r--   0     1001      127       41 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/installer.md
--rw-r--r--   0     1001      127       67 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_channel_error.md
--rw-r--r--   0     1001      127       71 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_match_spec_error.md
--rw-r--r--   0     1001      127       75 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_package_name_error.md
--rw-r--r--   0     1001      127       59 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_url_error.md
--rw-r--r--   0     1001      127       67 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/invalid_version_error.md
--rw-r--r--   0     1001      127       43 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/io_error.md
--rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/link_error.md
--rw-r--r--   0     1001      127       38 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/lock_file.md
--rw-r--r--   0     1001      127       48 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/locked_package.md
--rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/match_spec.md
--rw-r--r--   0     1001      127       64 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/nameless_match_spec.md
--rw-r--r--   0     1001      127       48 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/package_hashes.md
--rw-r--r--   0     1001      127       48 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/package_name.md
--rw-r--r--   0     1001      127       54 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/package_record.md
--rw-r--r--   0     1001      127       57 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/parse_arch_error.md
--rw-r--r--   0     1001      127       65 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/parse_platform_error.md
--rw-r--r--   0     1001      127       62 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/patch_instructions.md
--rw-r--r--   0     1001      127       77 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/path_modification_behavior.md
--rw-r--r--   0     1001      127       52 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/path_type.md
--rw-r--r--   0     1001      127       56 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/paths_entry.md
--rw-r--r--   0     1001      127       55 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/paths_json.md
--rw-r--r--   0     1001      127       42 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/platform.md
--rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/prefix_paths.md
--rw-r--r--   0     1001      127       69 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/prefix_placeholder.md
--rw-r--r--   0     1001      127       49 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/prefix_record.md
--rw-r--r--   0     1001      127       52 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/pypi_package_data.md
--rw-r--r--   0     1001      127       74 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/pypi_package_environment_data.md
--rw-r--r--   0     1001      127       44 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/repo_data.md
--rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/repo_data_record.md
--rw-r--r--   0     1001      127       56 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/run_exports_json.md
--rw-r--r--   0     1001      127       39 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/shell.md
--rw-r--r--   0     1001      127       35 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/solver.md
--rw-r--r--   0     1001      127       51 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/solver_error.md
--rw-r--r--   0     1001      127       47 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/sparse_repo_data.md
--rw-r--r--   0     1001      127     2082 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/transaction_error.md
--rw-r--r--   0     1001      127       39 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/version.md
--rw-r--r--   0     1001      127       53 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/version_with_source.md
--rw-r--r--   0     1001      127       62 2024-05-28 14:47:59.000000 py_rattler-0.6.1/docs/virtual_package.md
--rw-r--r--   0     1001      127     5280 2024-05-28 14:47:59.000000 py_rattler-0.6.1/mkdocs.yml
--rw-r--r--   0     1001      127   210327 2024-05-28 14:47:59.000000 py_rattler-0.6.1/pixi.lock
--rw-r--r--   0     1001      127     1898 2024-05-28 14:47:59.000000 py_rattler-0.6.1/pixi.toml
--rw-r--r--   0     1001      127     1863 2024-05-28 14:47:59.000000 py_rattler-0.6.1/pyproject.toml
--rw-r--r--   0     1001      127     2070 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/__init__.py
--rw-r--r--   0     1001      127      221 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/__init__.py
--rw-r--r--   0     1001      127     2295 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/channel.py
--rw-r--r--   0     1001      127     1532 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/channel_config.py
--rw-r--r--   0     1001      127      474 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/channel/channel_priority.py
--rw-r--r--   0     1001      127     3842 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/exceptions.py
--rw-r--r--   0     1001      127       59 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/index/__init__.py
--rw-r--r--   0     1001      127     1133 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/index/index.py
--rw-r--r--   0     1001      127       69 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/install/__init__.py
--rw-r--r--   0     1001      127     3407 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/install/installer.py
--rw-r--r--   0     1001      127      471 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/__init__.py
--rw-r--r--   0     1001      127     1277 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/channel.py
--rw-r--r--   0     1001      127     7624 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/environment.py
--rw-r--r--   0     1001      127      805 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/hash.py
--rw-r--r--   0     1001      127     3264 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/lock_file.py
--rw-r--r--   0     1001      127     5336 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/package.py
--rw-r--r--   0     1001      127     6544 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/lock/pypi.py
--rw-r--r--   0     1001      127      167 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/match_spec/__init__.py
--rw-r--r--   0     1001      127     7953 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/match_spec/match_spec.py
--rw-r--r--   0     1001      127     4293 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/match_spec/nameless_match_spec.py
--rw-r--r--   0     1001      127      189 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/networking/__init__.py
--rw-r--r--   0     1001      127      915 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/networking/authenticated_client.py
--rw-r--r--   0     1001      127     1393 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/networking/fetch_repo_data.py
--rw-r--r--   0     1001      127      518 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/__init__.py
--rw-r--r--   0     1001      127     7060 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/about_json.py
--rw-r--r--   0     1001      127     9422 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/index_json.py
--rw-r--r--   0     1001      127     3672 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/no_arch_type.py
--rw-r--r--   0     1001      127     4111 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/package_name.py
--rw-r--r--   0     1001      127    15226 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/paths_json.py
--rw-r--r--   0     1001      127     6238 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/package/run_exports_json.py
--rw-r--r--   0     1001      127      154 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/platform/__init__.py
--rw-r--r--   0     1001      127     1145 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/platform/arch.py
--rw-r--r--   0     1001      127     3993 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/platform/platform.py
--rw-r--r--   0     1001      127      221 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/prefix/__init__.py
--rw-r--r--   0     1001      127     8542 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/prefix/prefix_paths.py
--rw-r--r--   0     1001      127     4514 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/prefix/prefix_record.py
--rw-r--r--   0     1001      127        0 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/py.typed
--rw-r--r--   0     1001      127      495 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/__init__.py
--rw-r--r--   0     1001      127     8268 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/gateway.py
--rw-r--r--   0     1001      127    13342 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/package_record.py
--rw-r--r--   0     1001      127      694 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/patch_instructions.py
--rw-r--r--   0     1001      127     2660 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/record.py
--rw-r--r--   0     1001      127     2264 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/repo_data.py
--rw-r--r--   0     1001      127     6245 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/repo_data/sparse.py
--rw-r--r--   0     1001      127      179 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/shell/__init__.py
--rw-r--r--   0     1001      127     4442 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/shell/shell.py
--rw-r--r--   0     1001      127       61 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/solver/__init__.py
--rw-r--r--   0     1001      127     5197 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/solver/solver.py
--rw-r--r--   0     1001      127      526 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/utils/rattler_version.py
--rw-r--r--   0     1001      127      146 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/version/__init__.py
--rw-r--r--   0     1001      127    14868 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/version/version.py
--rw-r--r--   0     1001      127     2539 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/version/with_source.py
--rw-r--r--   0     1001      127      188 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/virtual_package/__init__.py
--rw-r--r--   0     1001      127     4411 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/virtual_package/generic.py
--rw-r--r--   0     1001      127     1509 2024-05-28 14:47:59.000000 py_rattler-0.6.1/rattler/virtual_package/virtual_package.py
--rw-r--r--   0     1001      127     4356 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/about_json.rs
--rw-r--r--   0     1001      127     2929 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/channel/mod.rs
--rw-r--r--   0     1001      127     8225 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/error.rs
--rw-r--r--   0     1001      127     1743 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/generic_virtual_package.rs
--rw-r--r--   0     1001      127      593 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/index.rs
--rw-r--r--   0     1001      127     5113 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/index_json.rs
--rw-r--r--   0     1001      127     2334 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/installer.rs
--rw-r--r--   0     1001      127     6766 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/lib.rs
--rw-r--r--   0     1001      127    15021 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/lock/mod.rs
--rw-r--r--   0     1001      127     3683 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/match_spec.rs
--rw-r--r--   0     1001      127      147 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/meta.rs
--rw-r--r--   0     1001      127     3550 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/nameless_match_spec.rs
--rw-r--r--   0     1001      127     1017 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/networking/authenticated_client.rs
--rw-r--r--   0     1001      127      804 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/networking/cached_repo_data.rs
--rw-r--r--   0     1001      127     3328 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/networking/mod.rs
--rw-r--r--   0     1001      127     1619 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/no_arch_type.rs
--rw-r--r--   0     1001      127     2124 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/package_name.rs
--rw-r--r--   0     1001      127     9546 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/paths_json.rs
--rw-r--r--   0     1001      127     2521 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/platform.rs
--rw-r--r--   0     1001      127     5691 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/prefix_paths.rs
--rw-r--r--   0     1001      127    13360 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/record.rs
--rw-r--r--   0     1001      127     4735 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/gateway.rs
--rw-r--r--   0     1001      127     1672 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/mod.rs
--rw-r--r--   0     1001      127      189 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/patch_instructions.rs
--rw-r--r--   0     1001      127     2096 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/repo_data/sparse.rs
--rw-r--r--   0     1001      127     4469 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/run_exports_json.rs
--rw-r--r--   0     1001      127     3878 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/shell.rs
--rw-r--r--   0     1001      127     3842 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/solver.rs
--rw-r--r--   0     1001      127      814 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/version/component.rs
--rw-r--r--   0     1001      127     5899 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/version/mod.rs
--rw-r--r--   0     1001      127     1190 2024-05-28 14:47:59.000000 py_rattler-0.6.1/src/virtual_package.rs
--rw-r--r--   0     1001      127        0 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/__init__.py
--rw-r--r--   0     1001      127      696 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/conftest.py
--rw-r--r--   0     1001      127        0 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/__init__.py
--rw-r--r--   0     1001      127     2129 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_fetch_repo_data.py
--rw-r--r--   0     1001      127     2159 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_index.py
--rw-r--r--   0     1001      127      730 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_install.py
--rw-r--r--   0     1001      127     1732 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_prefix_record.py
--rw-r--r--   0     1001      127     3531 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_solver.py
--rw-r--r--   0     1001      127      892 2024-05-28 14:47:59.000000 py_rattler-0.6.1/tests/unit/test_version.py
--rw-r--r--   0     1001      127   109244 2024-05-28 14:47:59.000000 py_rattler-0.6.1/Cargo.lock
--rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 py_rattler-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/Cargo.toml
+-rw-r--r--   0     1001      127     4159 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/CHANGELOG.md
+-rw-r--r--   0     1001      127     8878 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/builder.rs
+-rw-r--r--   0     1001      127      871 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/channel.rs
+-rw-r--r--   0     1001      127     5792 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/conda.rs
+-rw-r--r--   0     1001      127     2006 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/file_format_version.rs
+-rw-r--r--   0     1001      127     4879 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/hash.rs
+-rw-r--r--   0     1001      127    24726 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/lib.rs
+-rw-r--r--   0     1001      127     6083 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/deserialize.rs
+-rw-r--r--   0     1001      127     2613 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/mod.rs
+-rw-r--r--   0     1001      127     9114 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/serialize.rs
+-rw-r--r--   0     1001      127     8677 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/v3.rs
+-rw-r--r--   0     1001      127     5293 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/pypi.rs
+-rw-r--r--   0     1001      127     1480 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/pypi_indexes.rs
+-rw-r--r--   0     1001      127    15803 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap
+-rw-r--r--   0     1001      127    22538 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap
+-rw-r--r--   0     1001      127   487177 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap
+-rw-r--r--   0     1001      127    40002 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap
+-rw-r--r--   0     1001      127    52187 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap
+-rw-r--r--   0     1001      127  1811359 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap
+-rw-r--r--   0     1001      127   487177 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap
+-rw-r--r--   0     1001      127    19608 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap
+-rw-r--r--   0     1001      127    40002 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap
+-rw-r--r--   0     1001      127    52187 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap
+-rw-r--r--   0     1001      127  1811359 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap
+-rw-r--r--   0     1001      127    10278 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap
+-rw-r--r--   0     1001      127   242145 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap
+-rw-r--r--   0     1001      127     6457 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/url_or_path.rs
+-rw-r--r--   0     1001      127       22 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1693 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs
+-rw-r--r--   0     1001      127      372 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/mod.rs
+-rw-r--r--   0     1001      127     2012 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/ordered.rs
+-rw-r--r--   0     1001      127     1609 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs
+-rw-r--r--   0     1001      127     7980 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs
+-rw-r--r--   0     1001      127     1441 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs
+-rw-r--r--   0     1001      127     1407 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/Cargo.toml
+-rw-r--r--   0     1001      127     5510 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/CHANGELOG.md
+-rw-r--r--   0     1001      127     1016 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/benches/parse.rs
+-rw-r--r--   0     1001      127     3220 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/build_spec/mod.rs
+-rw-r--r--   0     1001      127     6519 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/build_spec/parse.rs
+-rw-r--r--   0     1001      127    23177 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/channel/mod.rs
+-rw-r--r--   0     1001      127     4187 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/channel_data.rs
+-rw-r--r--   0     1001      127    11580 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs
+-rw-r--r--   0     1001      127      770 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs
+-rw-r--r--   0     1001      127     2299 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/lib.rs
+-rw-r--r--   0     1001      127     6012 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs
+-rw-r--r--   0     1001      127    20372 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/mod.rs
+-rw-r--r--   0     1001      127    28472 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/parse.rs
+-rw-r--r--   0     1001      127      506 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__parse__tests__parsed matchspecs.snap
+-rw-r--r--   0     1001      127      537 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap
+-rw-r--r--   0     1001      127     5728 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/no_arch_type.rs
+-rw-r--r--   0     1001      127     3206 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/about.rs
+-rw-r--r--   0     1001      127     4183 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs
+-rw-r--r--   0     1001      127     1400 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/archive_type.rs
+-rw-r--r--   0     1001      127     3244 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/entry_point.rs
+-rw-r--r--   0     1001      127     1348 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/files.rs
+-rw-r--r--   0     1001      127     6460 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/has_prefix.rs
+-rw-r--r--   0     1001      127     3942 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/index.rs
+-rw-r--r--   0     1001      127     1977 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/link.rs
+-rw-r--r--   0     1001      127     3607 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/mod.rs
+-rw-r--r--   0     1001      127     1510 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/no_link.rs
+-rw-r--r--   0     1001      127     1495 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/no_softlink.rs
+-rw-r--r--   0     1001      127      507 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/package_metadata.rs
+-rw-r--r--   0     1001      127    12387 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/paths.rs
+-rw-r--r--   0     1001      127     2780 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/run_exports.rs
+-rw-r--r--   0     1001      127      754 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap
+-rw-r--r--   0     1001      127     2515 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap
+-rw-r--r--   0     1001      127      134 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__entry_point__test__entry_point.snap
+-rw-r--r--   0     1001      127      329 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json.snap
+-rw-r--r--   0     1001      127      309 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json_with_symlinks.snap
+-rw-r--r--   0     1001      127      349 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__jupyterlab-link.json.snap
+-rw-r--r--   0     1001      127      137 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__setuptools-link.json.snap
+-rw-r--r--   0     1001      127      138 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__tzdata-link.json.snap
+-rw-r--r--   0     1001      127     1171 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap
+-rw-r--r--   0     1001      127      776 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap
+-rw-r--r--   0     1001      127      601 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap
+-rw-r--r--   0     1001      127     6782 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap
+-rw-r--r--   0     1001      127      185 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__run_exports__test__reconstruct_run_exports_json_with_symlinks.snap
+-rw-r--r--   0     1001      127     5305 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package_name.rs
+-rw-r--r--   0     1001      127      233 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/parse_mode.rs
+-rw-r--r--   0     1001      127    15923 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/platform.rs
+-rw-r--r--   0     1001      127    12758 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/prefix_record.rs
+-rw-r--r--   0     1001      127    20250 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/mod.rs
+-rw-r--r--   0     1001      127    11158 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/patches.rs
+-rw-r--r--   0     1001      127     1554 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs
+-rw-r--r--   0     1001      127      181 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__null_values.snap
+-rw-r--r--   0     1001      127     2154 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap
+-rw-r--r--   0     1001      127     2091 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap
+-rw-r--r--   0     1001      127      843 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap
+-rw-r--r--   0     1001      127     1595 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap
+-rw-r--r--   0     1001      127      873 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap
+-rw-r--r--   0     1001      127     4832 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap
+-rw-r--r--   0     1001      127      232 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize.snap
+-rw-r--r--   0     1001      127     6461 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap
+-rw-r--r--   0     1001      127     5154 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap
+-rw-r--r--   0     1001      127    77589 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs
+-rw-r--r--   0     1001      127     1063 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data_record.rs
+-rw-r--r--   0     1001      127      455 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/run_export.rs
+-rw-r--r--   0     1001      127    53039 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap
+-rw-r--r--   0     1001      127      353 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__vs2015_runtime_win-64.txt.snap
+-rw-r--r--   0     1001      127      974 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap
+-rw-r--r--   0     1001      127     2269 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap
+-rw-r--r--   0     1001      127    12047 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap
+-rw-r--r--   0     1001      127   269415 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     4590 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap
+-rw-r--r--   0     1001      127    12519 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127   345345 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap
+-rw-r--r--   0     1001      127    23076 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     1054 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap
+-rw-r--r--   0     1001      127    12151 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     7102 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap
+-rw-r--r--   0     1001      127       22 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/utils/mod.rs
+-rw-r--r--   0     1001      127     6107 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/utils/serde.rs
+-rw-r--r--   0     1001      127    11988 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/bump.rs
+-rw-r--r--   0     1001      127     3760 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/flags.rs
+-rw-r--r--   0     1001      127    46846 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/mod.rs
+-rw-r--r--   0     1001      127    18817 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/parse.rs
+-rw-r--r--   0     1001      127     6410 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/segment.rs
+-rw-r--r--   0     1001      127     2495 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap
+-rw-r--r--   0     1001      127     4817 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/with_source.rs
+-rw-r--r--   0     1001      127    10262 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs
+-rw-r--r--   0     1001      127    19332 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/mod.rs
+-rw-r--r--   0     1001      127    18092 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/parse.rs
+-rw-r--r--   0     1001      127    15169 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_digest/Cargo.toml
+-rw-r--r--   0     1001      127     1233 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_digest/CHANGELOG.md
+-rw-r--r--   0     1001      127     7607 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_digest/src/lib.rs
+-rw-r--r--   0     1001      127     4014 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_digest/src/serde.rs
+-rw-r--r--   0     1001      127     2155 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_digest/src/tokio.rs
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/Cargo.toml
+-rw-r--r--   0     1001      127     3627 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/CHANGELOG.md
+-rw-r--r--   0     1001      127    14736 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_middleware.rs
+-rw-r--r--   0     1001      127     1266 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs
+-rw-r--r--   0     1001      127     6690 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs
+-rw-r--r--   0     1001      127     2852 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs
+-rw-r--r--   0     1001      127      103 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/mod.rs
+-rw-r--r--   0     1001      127     5769 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs
+-rw-r--r--   0     1001      127      270 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/snapshots/rattler_networking__authentication_storage__backends__file__tests__file_storage.snap
+-rw-r--r--   0     1001      127      727 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/mod.rs
+-rw-r--r--   0     1001      127     6830 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/storage.rs
+-rw-r--r--   0     1001      127     2287 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/gcs_middleware.rs
+-rw-r--r--   0     1001      127      726 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/lib.rs
+-rw-r--r--   0     1001      127    10298 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/mirror_middleware.rs
+-rw-r--r--   0     1001      127    10902 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/oci_middleware.rs
+-rw-r--r--   0     1001      127     3489 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/redaction.rs
+-rw-r--r--   0     1001      127      920 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_networking/src/retry_policies.rs
+-rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/.gitignore
+-rw-r--r--   0     1001      127     5863 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/CHANGELOG.md
+-rw-r--r--   0     1001      127    74752 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/resources/launcher64.exe
+-rw-r--r--   0     1001      127    99068 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/resources/versions.txt
+-rw-r--r--   0     1001      127     4794 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/cli/auth.rs
+-rw-r--r--   0     1001      127      122 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/cli/mod.rs
+-rw-r--r--   0     1001      127     1358 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/apple_codesign.rs
+-rw-r--r--   0     1001      127    35510 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/clobber_registry.rs
+-rw-r--r--   0     1001      127     9786 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/driver.rs
+-rw-r--r--   0     1001      127     8511 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/entry_point.rs
+-rw-r--r--   0     1001      127     1666 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/error.rs
+-rw-r--r--   0     1001      127    27383 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/indicatif.rs
+-rw-r--r--   0     1001      127    20030 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/mod.rs
+-rw-r--r--   0     1001      127     4261 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/reporter.rs
+-rw-r--r--   0     1001      127    33225 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/link.rs
+-rw-r--r--   0     1001      127     9691 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/link_script.rs
+-rw-r--r--   0     1001      127    33679 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/mod.rs
+-rw-r--r--   0     1001      127     3839 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/python.rs
+-rw-r--r--   0     1001      127      609 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap
+-rw-r--r--   0     1001      127      190 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-3.snap
+-rw-r--r--   0     1001      127      727 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap
+-rw-r--r--   0     1001      127      142 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-5.snap
+-rw-r--r--   0     1001      127      609 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap
+-rw-r--r--   0     1001      127      727 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap
+-rw-r--r--   0     1001      127      142 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber.snap
+-rw-r--r--   0     1001      127      297 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__entry_point_script.snap
+-rw-r--r--   0     1001      127      271 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__windows.snap
+-rw-r--r--   0     1001      127      155 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__link__test__replace_long_prefix_in_text_file.snap
+-rw-r--r--   0     1001      127     3732 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap
+-rw-r--r--   0     1001      127     4688 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/test_utils.rs
+-rw-r--r--   0     1001      127     8426 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/transaction.rs
+-rw-r--r--   0     1001      127     9414 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/install/unlink.rs
+-rw-r--r--   0     1001      127     2983 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/lib.rs
+-rw-r--r--   0     1001      127    22292 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/package_cache.rs
+-rw-r--r--   0     1001      127    24363 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/range.rs
+-rw-r--r--   0     1001      127    13775 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler/src/validation.rs
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_index/Cargo.toml
+-rw-r--r--   0     1001      127     3755 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_index/CHANGELOG.md
+-rw-r--r--   0     1001      127     6989 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_index/src/lib.rs
+-rw-r--r--   0     1001      127     2162 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_index/tests/test_index.rs
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/simple_spawn_blocking/Cargo.toml
+-rw-r--r--   0     1001      127      237 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/simple_spawn_blocking/src/lib.rs
+-rw-r--r--   0     1001      127      692 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/simple_spawn_blocking/src/tokio.rs
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/Cargo.toml
+-rw-r--r--   0     1001      127     1011 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/CHANGELOG.md
+-rw-r--r--   0     1001      127     1394 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/build.rs
+-rw-r--r--   0     1001      127    77341 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/src/lib.rs
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/Cargo.toml
+-rw-r--r--   0     1001      127     4767 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/CHANGELOG.md
+-rw-r--r--   0     1001      127     2806 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs
+-rw-r--r--   0     1001      127     7713 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs
+-rw-r--r--   0     1001      127      956 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap
+-rw-r--r--   0     1001      127      465 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_one.snap
+-rw-r--r--   0     1001      127      604 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap
+-rw-r--r--   0     1001      127    38981 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs
+-rw-r--r--   0     1001      127    52612 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs
+-rw-r--r--   0     1001      127     3926 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs
+-rw-r--r--   0     1001      127     3219 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs
+-rw-r--r--   0     1001      127     1738 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs
+-rw-r--r--   0     1001      127     2627 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs
+-rw-r--r--   0     1001      127     2335 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs
+-rw-r--r--   0     1001      127    18116 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs
+-rw-r--r--   0     1001      127     8435 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs
+-rw-r--r--   0     1001      127     2409 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs
+-rw-r--r--   0     1001      127     2377 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs
+-rw-r--r--   0     1001      127    13060 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs
+-rw-r--r--   0     1001      127     8026 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs
+-rw-r--r--   0     1001      127     5798 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs
+-rw-r--r--   0     1001      127     6178 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs
+-rw-r--r--   0     1001      127     2151 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/lib.rs
+-rw-r--r--   0     1001      127     3977 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/reporter.rs
+-rw-r--r--   0     1001      127    22540 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs
+-rw-r--r--   0     1001      127     2167 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/body.rs
+-rw-r--r--   0     1001      127     2718 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs
+-rw-r--r--   0     1001      127    13393 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs
+-rw-r--r--   0     1001      127     1715 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs
+-rw-r--r--   0     1001      127     2609 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/Cargo.toml
+-rw-r--r--   0     1001      127     4849 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/CHANGELOG.md
+-rw-r--r--   0     1001      127     2914 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/benches/bench.rs
+-rw-r--r--   0     1001      127     9021 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/lib.rs
+-rw-r--r--   0     1001      127    13226 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/input.rs
+-rw-r--r--   0     1001      127     1173 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs
+-rw-r--r--   0     1001      127     9767 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/mod.rs
+-rw-r--r--   0     1001      127     2444 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/output.rs
+-rw-r--r--   0     1001      127      561 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs
+-rw-r--r--   0     1001      127      864 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs
+-rw-r--r--   0     1001      127     1047 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs
+-rw-r--r--   0     1001      127    11669 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs
+-rw-r--r--   0     1001      127     2720 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs
+-rw-r--r--   0     1001      127     6299 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs
+-rw-r--r--   0     1001      127     3402 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs
+-rw-r--r--   0     1001      127     1262 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs
+-rw-r--r--   0     1001      127     3451 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs
+-rw-r--r--   0     1001      127     4718 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs
+-rw-r--r--   0     1001      127     5589 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs
+-rw-r--r--   0     1001      127     2468 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs
+-rw-r--r--   0     1001      127     7734 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/resolvo/conda_util.rs
+-rw-r--r--   0     1001      127    24769 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/src/resolvo/mod.rs
+-rw-r--r--   0     1001      127    35241 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/backends.rs
+-rw-r--r--   0     1001      127      165 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_dummy_repo_install_non_existent.snap
+-rw-r--r--   0     1001      127      738 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap
+-rw-r--r--   0     1001      127     1105 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap
+-rw-r--r--   0     1001      127     3069 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap
+-rw-r--r--   0     1001      127     2590 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap
+-rw-r--r--   0     1001      127     3631 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap
+-rw-r--r--   0     1001      127      216 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_with_error.snap
+-rw-r--r--   0     1001      127      411 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_xtensor_xsimd.snap
+-rw-r--r--   0     1001      127      369 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__exclude_newer_error.snap
+-rw-r--r--   0     1001      127      172 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_dummy_repo_install_non_existent.snap
+-rw-r--r--   0     1001      127      412 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_locked.snap
+-rw-r--r--   0     1001      127      736 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap
+-rw-r--r--   0     1001      127     1103 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap
+-rw-r--r--   0     1001      127     3067 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap
+-rw-r--r--   0     1001      127     2588 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap
+-rw-r--r--   0     1001      127     3629 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap
+-rw-r--r--   0     1001      127      588 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap
+-rw-r--r--   0     1001      127      400 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_xtensor_xsimd.snap
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/Cargo.toml
+-rw-r--r--   0     1001      127     3660 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/CHANGELOG.md
+-rw-r--r--   0     1001      127    11042 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/cuda.rs
+-rw-r--r--   0     1001      127    12929 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/lib.rs
+-rw-r--r--   0     1001      127     3047 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/libc.rs
+-rw-r--r--   0     1001      127     3969 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/linux.rs
+-rw-r--r--   0     1001      127     2381 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/osx.rs
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/Cargo.toml
+-rw-r--r--   0     1001      127     3407 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/CHANGELOG.md
+-rw-r--r--   0     1001      127    27911 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/activation.rs
+-rw-r--r--   0     1001      127      196 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/lib.rs
+-rw-r--r--   0     1001      127     2232 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/run/mod.rs
+-rw-r--r--   0     1001      127    28467 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/shell/mod.rs
+-rw-r--r--   0     1001      127      123 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__bash.snap
+-rw-r--r--   0     1001      127      128 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__fish.snap
+-rw-r--r--   0     1001      127      104 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_bash.snap
+-rw-r--r--   0     1001      127      122 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_xsh.snap
+-rw-r--r--   0     1001      127      237 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_bash.snap
+-rw-r--r--   0     1001      127      185 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_cmd.snap
+-rw-r--r--   0     1001      127      190 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_fish.snap
+-rw-r--r--   0     1001      127      192 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_powershell.snap
+-rw-r--r--   0     1001      127      239 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_xonsh.snap
+-rw-r--r--   0     1001      127      237 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_zsh.snap
+-rw-r--r--   0     1001      127      171 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__after_activation.snap
+-rw-r--r--   0     1001      127      237 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_append.snap
+-rw-r--r--   0     1001      127      237 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_prepend.snap
+-rw-r--r--   0     1001      127      229 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_replace.snap
+-rw-r--r--   0     1001      127      202 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_append.snap
+-rw-r--r--   0     1001      127      202 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_prepend.snap
+-rw-r--r--   0     1001      127      195 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_replace.snap
+-rw-r--r--   0     1001      127      311 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_append.snap
+-rw-r--r--   0     1001      127      311 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_prepend.snap
+-rw-r--r--   0     1001      127      301 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_replace.snap
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/file_url/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/file_url/.gitignore
+-rw-r--r--   0     1001      127      486 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/file_url/CHANGELOG.md
+-rw-r--r--   0     1001      127     7791 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/file_url/src/lib.rs
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/Cargo.toml
+-rw-r--r--   0     1001      127      987 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/CHANGELOG.md
+-rw-r--r--   0     1001      127     2664 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/src/lib.rs
+-rw-r--r--   0     1001      127      113 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/tests/01-sorted-enum.rs
+-rw-r--r--   0     1001      127      155 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/tests/02-sorted-struct.rs
+-rw-r--r--   0     1001      127      113 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/tests/03-out-of-order-enum.rs
+-rw-r--r--   0     1001      127      127 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/tests/03-out-of-order-enum.stderr
+-rw-r--r--   0     1001      127      155 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/tests/04-out-of-order-struct.rs
+-rw-r--r--   0     1001      127      137 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/tests/04-out-of-order-struct.stderr
+-rw-r--r--   0     1001      127      251 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_macros/tests/tests.rs
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/Cargo.toml
+-rw-r--r--   0     1001      127     4572 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/CHANGELOG.md
+-rw-r--r--   0     1001      127     2053 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/fs.rs
+-rw-r--r--   0     1001      127     2392 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/lib.rs
+-rw-r--r--   0     1001      127     3671 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/read.rs
+-rw-r--r--   0     1001      127       98 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/reqwest/mod.rs
+-rw-r--r--   0     1001      127     6136 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs
+-rw-r--r--   0     1001      127     4387 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/seek.rs
+-rw-r--r--   0     1001      127     1732 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs
+-rw-r--r--   0     1001      127     3101 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/tokio/fs.rs
+-rw-r--r--   0     1001      127      113 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/tokio/mod.rs
+-rw-r--r--   0     1001      127    14225 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/write.rs
+-rw-r--r--   0     1001      127     9266 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/tests/extract.rs
+-rw-r--r--   0     1001      127     7864 2024-06-03 09:38:42.000000 py_rattler-0.6.2/local_dependencies/rattler_package_streaming/tests/write.rs
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 py_rattler-0.6.2/Cargo.toml
+-rw-r--r--   0     1001      127      743 2024-06-03 09:38:42.000000 py_rattler-0.6.2/.gitignore
+-rw-r--r--   0     1001      127     1502 2024-06-03 09:38:42.000000 py_rattler-0.6.2/LICENSE
+-rw-r--r--   0     1001      127     6880 2024-06-03 09:38:42.000000 py_rattler-0.6.2/README.md
+-rw-r--r--   0     1001      127       71 2024-06-03 09:38:42.000000 py_rattler-0.6.2/build.rs
+-rw-r--r--   0     1001      127       44 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/about_json.md
+-rw-r--r--   0     1001      127       45 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/activate.md
+-rw-r--r--   0     1001      127       58 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/activation_error.md
+-rw-r--r--   0     1001      127       61 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/activation_result.md
+-rw-r--r--   0     1001      127       67 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/activation_variables.md
+-rw-r--r--   0     1001      127       34 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/arch.md
+-rw-r--r--   0     1001      127       62 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/authenticated_client.md
+-rw-r--r--   0     1001      127       54 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/cache_dir_error.md
+-rw-r--r--   0     1001      127       39 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/channel.md
+-rw-r--r--   0     1001      127       52 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/channel_config.md
+-rw-r--r--   0     1001      127       79 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/detect_virtual_package_error.md
+-rw-r--r--   0     1001      127       44 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/environment.md
+-rw-r--r--   0     1001      127       76 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/environment_creation_error.md
+-rw-r--r--   0     1001      127       58 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/fetch_repo_data.md
+-rw-r--r--   0     1001      127       65 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/fetch_repo_data_error.md
+-rw-r--r--   0     1001      127       51 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/file_mode.md
+-rw-r--r--   0     1001      127       41 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/gateway.md
+-rw-r--r--   0     1001      127       61 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/generic_virtual_package.md
+-rw-r--r--   0     1001      127     3826 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/index.md
+-rw-r--r--   0     1001      127       44 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/index_json.md
+-rw-r--r--   0     1001      127       41 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/installer.md
+-rw-r--r--   0     1001      127       67 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/invalid_channel_error.md
+-rw-r--r--   0     1001      127       71 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/invalid_match_spec_error.md
+-rw-r--r--   0     1001      127       75 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/invalid_package_name_error.md
+-rw-r--r--   0     1001      127       59 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/invalid_url_error.md
+-rw-r--r--   0     1001      127       67 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/invalid_version_error.md
+-rw-r--r--   0     1001      127       43 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/io_error.md
+-rw-r--r--   0     1001      127       47 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/link_error.md
+-rw-r--r--   0     1001      127       38 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/lock_file.md
+-rw-r--r--   0     1001      127       48 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/locked_package.md
+-rw-r--r--   0     1001      127       47 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/match_spec.md
+-rw-r--r--   0     1001      127       64 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/nameless_match_spec.md
+-rw-r--r--   0     1001      127       48 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/package_hashes.md
+-rw-r--r--   0     1001      127       48 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/package_name.md
+-rw-r--r--   0     1001      127       54 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/package_record.md
+-rw-r--r--   0     1001      127       57 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/parse_arch_error.md
+-rw-r--r--   0     1001      127       65 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/parse_platform_error.md
+-rw-r--r--   0     1001      127       62 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/patch_instructions.md
+-rw-r--r--   0     1001      127       77 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/path_modification_behavior.md
+-rw-r--r--   0     1001      127       52 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/path_type.md
+-rw-r--r--   0     1001      127       56 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/paths_entry.md
+-rw-r--r--   0     1001      127       55 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/paths_json.md
+-rw-r--r--   0     1001      127       42 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/platform.md
+-rw-r--r--   0     1001      127       47 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/prefix_paths.md
+-rw-r--r--   0     1001      127       69 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/prefix_placeholder.md
+-rw-r--r--   0     1001      127       49 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/prefix_record.md
+-rw-r--r--   0     1001      127       52 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/pypi_package_data.md
+-rw-r--r--   0     1001      127       74 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/pypi_package_environment_data.md
+-rw-r--r--   0     1001      127       44 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/repo_data.md
+-rw-r--r--   0     1001      127       47 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/repo_data_record.md
+-rw-r--r--   0     1001      127       56 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/run_exports_json.md
+-rw-r--r--   0     1001      127       39 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/shell.md
+-rw-r--r--   0     1001      127       35 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/solver.md
+-rw-r--r--   0     1001      127       51 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/solver_error.md
+-rw-r--r--   0     1001      127       47 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/sparse_repo_data.md
+-rw-r--r--   0     1001      127     2082 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127       61 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/transaction_error.md
+-rw-r--r--   0     1001      127       39 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/version.md
+-rw-r--r--   0     1001      127       53 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/version_with_source.md
+-rw-r--r--   0     1001      127       62 2024-06-03 09:38:42.000000 py_rattler-0.6.2/docs/virtual_package.md
+-rw-r--r--   0     1001      127     1030 2024-06-03 09:38:42.000000 py_rattler-0.6.2/examples/solve_and_install.py
+-rw-r--r--   0     1001      127     5304 2024-06-03 09:38:42.000000 py_rattler-0.6.2/mkdocs.yml
+-rw-r--r--   0     1001      127   233003 2024-06-03 09:38:42.000000 py_rattler-0.6.2/pixi.lock
+-rw-r--r--   0     1001      127     1971 2024-06-03 09:38:42.000000 py_rattler-0.6.2/pixi.toml
+-rw-r--r--   0     1001      127     1875 2024-06-03 09:38:42.000000 py_rattler-0.6.2/pyproject.toml
+-rw-r--r--   0     1001      127     2070 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/__init__.py
+-rw-r--r--   0     1001      127      221 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/channel/__init__.py
+-rw-r--r--   0     1001      127     2295 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/channel/channel.py
+-rw-r--r--   0     1001      127     1532 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/channel/channel_config.py
+-rw-r--r--   0     1001      127      474 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/channel/channel_priority.py
+-rw-r--r--   0     1001      127     3842 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/exceptions.py
+-rw-r--r--   0     1001      127       59 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/index/__init__.py
+-rw-r--r--   0     1001      127     1133 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/index/index.py
+-rw-r--r--   0     1001      127       69 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/install/__init__.py
+-rw-r--r--   0     1001      127     3418 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/install/installer.py
+-rw-r--r--   0     1001      127      471 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/lock/__init__.py
+-rw-r--r--   0     1001      127     1277 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/lock/channel.py
+-rw-r--r--   0     1001      127     7624 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/lock/environment.py
+-rw-r--r--   0     1001      127      805 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/lock/hash.py
+-rw-r--r--   0     1001      127     3238 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/lock/lock_file.py
+-rw-r--r--   0     1001      127     5336 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/lock/package.py
+-rw-r--r--   0     1001      127     6544 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/lock/pypi.py
+-rw-r--r--   0     1001      127      167 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/match_spec/__init__.py
+-rw-r--r--   0     1001      127     7953 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/match_spec/match_spec.py
+-rw-r--r--   0     1001      127     4293 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/match_spec/nameless_match_spec.py
+-rw-r--r--   0     1001      127      189 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/networking/__init__.py
+-rw-r--r--   0     1001      127      915 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/networking/authenticated_client.py
+-rw-r--r--   0     1001      127     1393 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/networking/fetch_repo_data.py
+-rw-r--r--   0     1001      127      518 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/package/__init__.py
+-rw-r--r--   0     1001      127     7060 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/package/about_json.py
+-rw-r--r--   0     1001      127     9589 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/package/index_json.py
+-rw-r--r--   0     1001      127     3672 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/package/no_arch_type.py
+-rw-r--r--   0     1001      127     4111 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/package/package_name.py
+-rw-r--r--   0     1001      127    15226 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/package/paths_json.py
+-rw-r--r--   0     1001      127     6238 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/package/run_exports_json.py
+-rw-r--r--   0     1001      127      154 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/platform/__init__.py
+-rw-r--r--   0     1001      127     1145 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/platform/arch.py
+-rw-r--r--   0     1001      127     3993 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/platform/platform.py
+-rw-r--r--   0     1001      127      221 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/prefix/__init__.py
+-rw-r--r--   0     1001      127     8542 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/prefix/prefix_paths.py
+-rw-r--r--   0     1001      127     4514 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/prefix/prefix_record.py
+-rw-r--r--   0     1001      127        0 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/py.typed
+-rw-r--r--   0     1001      127      495 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/repo_data/__init__.py
+-rw-r--r--   0     1001      127     8268 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/repo_data/gateway.py
+-rw-r--r--   0     1001      127    14914 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/repo_data/package_record.py
+-rw-r--r--   0     1001      127      694 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/repo_data/patch_instructions.py
+-rw-r--r--   0     1001      127     2660 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/repo_data/record.py
+-rw-r--r--   0     1001      127     2264 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/repo_data/repo_data.py
+-rw-r--r--   0     1001      127     6245 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/repo_data/sparse.py
+-rw-r--r--   0     1001      127      179 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/shell/__init__.py
+-rw-r--r--   0     1001      127     4442 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/shell/shell.py
+-rw-r--r--   0     1001      127       61 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/solver/__init__.py
+-rw-r--r--   0     1001      127     6008 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/solver/solver.py
+-rw-r--r--   0     1001      127      526 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/utils/rattler_version.py
+-rw-r--r--   0     1001      127      146 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/version/__init__.py
+-rw-r--r--   0     1001      127    15973 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/version/version.py
+-rw-r--r--   0     1001      127     2539 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/version/with_source.py
+-rw-r--r--   0     1001      127      188 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/virtual_package/__init__.py
+-rw-r--r--   0     1001      127     4411 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/virtual_package/generic.py
+-rw-r--r--   0     1001      127     1509 2024-06-03 09:38:42.000000 py_rattler-0.6.2/rattler/virtual_package/virtual_package.py
+-rw-r--r--   0     1001      127     4356 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/about_json.rs
+-rw-r--r--   0     1001      127     2929 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/channel/mod.rs
+-rw-r--r--   0     1001      127     8225 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/error.rs
+-rw-r--r--   0     1001      127     1743 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/generic_virtual_package.rs
+-rw-r--r--   0     1001      127      593 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/index.rs
+-rw-r--r--   0     1001      127     5120 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/index_json.rs
+-rw-r--r--   0     1001      127     2334 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/installer.rs
+-rw-r--r--   0     1001      127     6766 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/lib.rs
+-rw-r--r--   0     1001      127    15021 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/lock/mod.rs
+-rw-r--r--   0     1001      127     3683 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/match_spec.rs
+-rw-r--r--   0     1001      127      147 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/meta.rs
+-rw-r--r--   0     1001      127     3550 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/nameless_match_spec.rs
+-rw-r--r--   0     1001      127     1017 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/networking/authenticated_client.rs
+-rw-r--r--   0     1001      127      804 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/networking/cached_repo_data.rs
+-rw-r--r--   0     1001      127     3328 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/networking/mod.rs
+-rw-r--r--   0     1001      127     1619 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/no_arch_type.rs
+-rw-r--r--   0     1001      127     2124 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/package_name.rs
+-rw-r--r--   0     1001      127     9546 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/paths_json.rs
+-rw-r--r--   0     1001      127     2521 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/platform.rs
+-rw-r--r--   0     1001      127     5691 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/prefix_paths.rs
+-rw-r--r--   0     1001      127    13367 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/record.rs
+-rw-r--r--   0     1001      127     4735 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/repo_data/gateway.rs
+-rw-r--r--   0     1001      127     1672 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/repo_data/mod.rs
+-rw-r--r--   0     1001      127      189 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/repo_data/patch_instructions.rs
+-rw-r--r--   0     1001      127     2096 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/repo_data/sparse.rs
+-rw-r--r--   0     1001      127     4469 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/run_exports_json.rs
+-rw-r--r--   0     1001      127     3878 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/shell.rs
+-rw-r--r--   0     1001      127     3957 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/solver.rs
+-rw-r--r--   0     1001      127      814 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/version/component.rs
+-rw-r--r--   0     1001      127     6340 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/version/mod.rs
+-rw-r--r--   0     1001      127     1190 2024-06-03 09:38:42.000000 py_rattler-0.6.2/src/virtual_package.rs
+-rw-r--r--   0     1001      127        0 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/__init__.py
+-rw-r--r--   0     1001      127      696 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/unit/__init__.py
+-rw-r--r--   0     1001      127     2129 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/unit/test_fetch_repo_data.py
+-rw-r--r--   0     1001      127     2159 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/unit/test_index.py
+-rw-r--r--   0     1001      127      730 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/unit/test_install.py
+-rw-r--r--   0     1001      127     1732 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/unit/test_prefix_record.py
+-rw-r--r--   0     1001      127     4031 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/unit/test_solver.py
+-rw-r--r--   0     1001      127      892 2024-06-03 09:38:42.000000 py_rattler-0.6.2/tests/unit/test_version.py
+-rw-r--r--   0     1001      127   110026 2024-06-03 09:38:54.000000 py_rattler-0.6.2/Cargo.lock
+-rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 py_rattler-0.6.2/PKG-INFO
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_package_streaming"
-version = "0.21.1"
+version = "0.21.2"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Extract and stream of Conda package archives"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.1", default-features = false }
 rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
 rattler_networking = { path= "../rattler_networking", version = "0.20.8", default-features = false }
 bzip2 = "0.4.4"
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.21.2](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.21.1...rattler_package_streaming-v0.21.2) - 2024-06-03
+
+### Fixed
+- call on_download_start also for file URLs ([#708](https://github.com/mamba-org/rattler/pull/708))
+
 ## [0.21.1](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.21.0...rattler_package_streaming-v0.21.1) - 2024-05-28
 
 ### Other
 - updated the following local packages: rattler_conda_types
 
 ## [0.21.0](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.10...rattler_package_streaming-v0.21.0) - 2024-05-27
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/fs.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/fs.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/read.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/read.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 async fn get_reader(
     url: Url,
     client: reqwest_middleware::ClientWithMiddleware,
     expected_sha256: Option<Sha256Hash>,
     reporter: Option<Arc<dyn DownloadReporter>>,
 ) -> Result<impl tokio::io::AsyncRead, ExtractError> {
+    if let Some(reporter) = &reporter {
+        reporter.on_download_start();
+    }
+
     if url.scheme() == "file" {
         let file =
             tokio::fs::File::open(url.to_file_path().expect("Could not convert to file path"))
                 .await
                 .map_err(ExtractError::IoError)?;
 
         Ok(Either::Left(BufReader::new(file)))
@@ -37,18 +41,14 @@
         let mut request = client.get(url.clone());
 
         if let Some(sha256) = expected_sha256 {
             // This is used by the OCI registry middleware to verify the sha256 of the response
             request = request.header("X-Expected-Sha256", format!("{sha256:x}"));
         }
 
-        if let Some(reporter) = &reporter {
-            reporter.on_download_start();
-        }
-
         let response = request
             .send()
             .await
             .and_then(error_for_status)
             .map_err(ExtractError::ReqwestError)?;
 
         let total_bytes = response.content_length();
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/seek.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/seek.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/tokio/fs.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/tokio/fs.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/src/write.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/src/write.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/extract.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/tests/extract.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_package_streaming/tests/write.rs` & `py_rattler-0.6.2/local_dependencies/rattler_package_streaming/tests/write.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_lock/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_lock"
-version = "0.22.9"
+version = "0.22.10"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Rust data types for conda lock"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.0", default-features = false }
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.1", default-features = false }
 rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false }
 file_url = { path = "../file_url", version = "0.1.1" }
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_lock/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.22.10](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.9...rattler_lock-v0.22.10) - 2024-06-03
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.22.9](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.8...rattler_lock-v0.22.9) - 2024-05-28
 
 ### Added
 - add run exports to package data ([#671](https://github.com/mamba-org/rattler/pull/671))
 
 ### Other
 - bump ([#683](https://github.com/mamba-org/rattler/pull/683))
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/builder.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/builder.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/channel.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/channel.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/conda.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/conda.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/file_format_version.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/file_format_version.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/hash.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/hash.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/deserialize.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/deserialize.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/serialize.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/serialize.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/parse/v3.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/parse/v3.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/pypi.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/pypi_indexes.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/pypi_indexes.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/url_or_path.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/url_or_path.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/ordered.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/ordered.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs` & `py_rattler-0.6.2/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "rattler_repodata_gateway"
-version = "0.20.3"
+version = "0.20.4"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "A crate to interact with Conda repodata"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
 file_url = { path = "../file_url", version = "0.1.1" }
-rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.0", default-features = false, optional = true }
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.1", default-features = false, optional = true }
 rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false, features = ["tokio", "serde"] }
 rattler_networking = { path = "../rattler_networking", version = "0.20.8", default-features = false }
 simple_spawn_blocking = { path = "../simple_spawn_blocking", version = "1.0", features = ["tokio"] }
 anyhow = "1.0.82"
 async-compression = { version = "0.4.8", features = [
     "gzip",
     "tokio",
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.20.4](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.20.3...rattler_repodata_gateway-v0.20.4) - 2024-06-03
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_conda_types
+
 ## [0.20.3](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.20.2...rattler_repodata_gateway-v0.20.3) - 2024-05-28
 
 ### Other
 - updated the following local packages: rattler_conda_types, rattler_conda_types
 
 ## [0.20.2](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.20.1...rattler_repodata_gateway-v0.20.2) - 2024-05-27
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/reporter.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/body.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/body.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs` & `py_rattler-0.6.2/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_macros/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_macros/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_macros/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_macros/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_digest/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_digest/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_digest/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_digest/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_digest/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_digest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_digest/src/serde.rs` & `py_rattler-0.6.2/local_dependencies/rattler_digest/src/serde.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_digest/src/tokio.rs` & `py_rattler-0.6.2/local_dependencies/rattler_digest/src/tokio.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_networking/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_networking/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_middleware.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/authentication_storage/storage.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/authentication_storage/storage.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/gcs_middleware.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/gcs_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/mirror_middleware.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/mirror_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/oci_middleware.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/oci_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/redaction.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/redaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_networking/src/retry_policies.rs` & `py_rattler-0.6.2/local_dependencies/rattler_networking/src/retry_policies.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/file_url/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/file_url/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_index/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_index/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "rattler_index"
-version = "0.19.14"
+version = "0.19.15"
 edition= "2021"
 authors = []
 description = "A crate that indexes directories containing conda packages to create local conda channels"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.1", default-features = false }
 rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
-rattler_package_streaming = { path= "../rattler_package_streaming", version = "0.21.1", default-features = false }
+rattler_package_streaming = { path= "../rattler_package_streaming", version = "0.21.2", default-features = false }
 fs-err = "2.11.0"
 serde_json = { version = "1.0.116" }
 tracing = "0.1.40"
 walkdir = "2.5.0"
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_index/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_index/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.19.15](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.14...rattler_index-v0.19.15) - 2024-06-03
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_package_streaming
+
 ## [0.19.14](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.13...rattler_index-v0.19.14) - 2024-05-28
 
 ### Added
 - add run exports to package data ([#671](https://github.com/mamba-org/rattler/pull/671))
 
 ## [0.19.13](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.12...rattler_index-v0.19.13) - 2024-05-27
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_index/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_index/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_index/tests/test_index.rs` & `py_rattler-0.6.2/local_dependencies/rattler_index/tests/test_index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/build.rs` & `py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/build.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_libsolv_c/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_libsolv_c/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rattler_conda_types"
-version = "0.25.0"
+version = "0.25.1"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Rust data types for common types used within the Conda ecosystem"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.25.1](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.25.0...rattler_conda_types-v0.25.1) - 2024-06-03
+
+### Added
+- add a `with_alpha` function that adds `0a0` to the version ([#696](https://github.com/mamba-org/rattler/pull/696))
+
 ## [0.25.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.24.0...rattler_conda_types-v0.25.0) - 2024-05-28
 
 ### Added
 - when bumping, extend versions with `0` to match the bump request ([#695](https://github.com/mamba-org/rattler/pull/695))
 - extend tests and handle characters better when bumping versions ([#694](https://github.com/mamba-org/rattler/pull/694))
 - add a function to extend version with `0s` ([#689](https://github.com/mamba-org/rattler/pull/689))
 - add run exports to package data ([#671](https://github.com/mamba-org/rattler/pull/671))
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/benches/parse.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/benches/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/build_spec/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/build_spec/parse.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/build_spec/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/channel/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/channel_data.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/channel_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/parse.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/no_arch_type.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/no_arch_type.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/about.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/about.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/archive_type.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/archive_type.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/entry_point.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/entry_point.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/files.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/files.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/has_prefix.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/has_prefix.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/index.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/link.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_link.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/no_link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/no_softlink.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/no_softlink.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/paths.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/paths.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/run_exports.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/run_exports.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/package_name.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/platform.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/platform.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/prefix_record.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/prefix_record.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/patches.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/patches.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/repo_data_record.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/repo_data_record.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/utils/serde.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/utils/serde.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/bump.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/bump.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use std::borrow::Cow;
+
 use thiserror::Error;
 
 use crate::{Component, Version};
 
 use super::{segment::Segment, ComponentVec, SegmentVec};
 
 /// `VersionBumpType` is used to specify the type of bump to perform on a version.
@@ -31,14 +33,75 @@
 
     /// Could not extend the version
     #[error("could not extend the version: {0}")]
     VersionExtendError(#[from] crate::VersionExtendError),
 }
 
 impl Version {
+    /// Add alpha specifier to the end of the version when the last element does not contain an `iden` component.
+    ///
+    /// For example, `1.0.0` will become `1.0.0.0a0`.
+    /// If the last version element contains a character, it's not modified (e.g. `1.0.0a` will remain `1.0.0a`).
+    pub fn with_alpha(&self) -> Cow<'_, Self> {
+        let last_segment = self.segments().last().expect("at least one segment");
+        // check if there is an iden component in the last segment
+        let has_iden = last_segment.components().any(|c| c.as_iden().is_some());
+        if has_iden {
+            return Cow::Borrowed(self);
+        }
+        let local_segment_index = self.local_segment_index().unwrap_or(self.segments.len());
+        let mut segments = self.segments[0..local_segment_index].to_vec();
+        let components_offset = segments.iter().map(|s| s.len() as usize).sum::<usize>()
+            + usize::from(self.has_epoch());
+
+        segments.push(Segment::new(3).unwrap().with_separator(Some('.')).unwrap());
+        segments.extend(self.segments[local_segment_index..].iter());
+
+        let mut components = self.components.clone();
+        components.insert(components_offset, Component::Numeral(0));
+        components.insert(components_offset + 1, Component::Iden("a".into()));
+        components.insert(components_offset + 2, Component::Numeral(0));
+
+        let flags = if let Some(local_segment_index) = self.local_segment_index() {
+            self.flags
+                .with_local_segment_index((local_segment_index + 1) as u8)
+                .unwrap()
+        } else {
+            self.flags
+        };
+
+        Cow::Owned(Version {
+            components,
+            segments: segments.into(),
+            flags,
+        })
+    }
+
+    /// Remove the local segment from the version if it exists.
+    /// Returns a new version without the local segment.
+    ///
+    /// For example, `1.0.0+3.4` will become `1.0.0`.
+    pub fn remove_local(&self) -> Cow<'_, Self> {
+        if let Some(local_segment_index) = self.local_segment_index() {
+            let segments = self.segments[0..local_segment_index].to_vec();
+            let components_offset = segments.iter().map(|s| s.len() as usize).sum::<usize>()
+                + usize::from(self.has_epoch());
+            let mut components = self.components.clone();
+            components.drain(components_offset..);
+
+            Cow::Owned(Version {
+                components,
+                segments: segments.into(),
+                flags: self.flags.with_local_segment_index(0).unwrap(),
+            })
+        } else {
+            return Cow::Borrowed(self);
+        }
+    }
+
     /// Returns a new version after bumping it according to the specified bump type.
     /// Note: if a version ends with a character, the next bigger version will use `a` as the character.
     /// For example: `1.1l` -> `1.2a`, but also `1.1.0alpha` -> `1.1.1a`.
     pub fn bump(&self, bump_type: VersionBumpType) -> Result<Self, VersionBumpError> {
         // Sanity check whether the version has enough segments for this bump type.
         let segment_count = self.segment_count();
         let segment_to_bump = match bump_type {
@@ -232,8 +295,43 @@
             Version::from_str(input)
                 .unwrap()
                 .bump(VersionBumpType::Segment(idx))
                 .unwrap(),
             Version::from_str(expected).unwrap()
         );
     }
+
+    #[rstest]
+    #[case(0, "1.1.9", "2.1.9.0a0")]
+    #[case(2, "1.0.0", "1.0.1.0a0")]
+    #[case(2, "1.0.0a", "1.0.1a")]
+    #[case(2, "1.0.0f", "1.0.1a")]
+    #[case(2, "5!1.0.0", "5!1.0.1.0a0")]
+    #[case(2, "5!1.0.0+3.4", "5!1.0.1.0a0+3.4")]
+    fn with_alpha(#[case] idx: i32, #[case] input: &str, #[case] expected: &str) {
+        assert_eq!(
+            Version::from_str(input)
+                .unwrap()
+                .bump(VersionBumpType::Segment(idx))
+                .unwrap()
+                .with_alpha()
+                .into_owned(),
+            Version::from_str(expected).unwrap()
+        );
+    }
+
+    #[rstest]
+    #[case("1.1.9", "1.1.9")]
+    #[case("1.0.0+3", "1.0.0")]
+    #[case("1.0.0+3.4", "1.0.0")]
+    #[case("1.0.0+3.4alpha.2.4", "1.0.0")]
+    #[case("5!1.0.0+3.4alpha.2.4", "5!1.0.0")]
+    fn remove_local(#[case] input: &str, #[case] expected: &str) {
+        assert_eq!(
+            Version::from_str(input)
+                .unwrap()
+                .remove_local()
+                .into_owned(),
+            Version::from_str(expected).unwrap()
+        );
+    }
 }
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/flags.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/flags.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/parse.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/segment.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/segment.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version/with_source.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version/with_source.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/parse.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs` & `py_rattler-0.6.2/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_shell/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_shell/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_shell"
-version = "0.20.6"
+version = "0.20.7"
 edition= "2021"
 authors = ["Wolf Vollprecht <w.vollprecht@gmail.com>"]
 description = "A crate to help with activation and deactivation of a conda environment"
 categories = ["conda", "mamba", "package_management", "virtual_environment"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.1", default-features = false }
 enum_dispatch = "0.3.13"
 indexmap = "2.2.6"
 itertools = "0.12.1"
 serde_json = { version = "1.0.116" , features = ["preserve_order"] }
 shlex = "1.3.0"
 sysinfo = { version = "0.30.10", optional = true }
 tempfile = "3.10.1"
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_shell/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_shell/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.20.7](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.6...rattler_shell-v0.20.7) - 2024-06-03
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.20.6](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.5...rattler_shell-v0.20.6) - 2024-05-28
 
 ### Other
 - updated the following local packages: rattler_conda_types
 
 ## [0.20.5](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.4...rattler_shell-v0.20.5) - 2024-05-27
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_shell/src/activation.rs` & `py_rattler-0.6.2/local_dependencies/rattler_shell/src/activation.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_shell/src/run/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_shell/src/run/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_shell/src/shell/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_shell/src/shell/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rattler"
-version = "0.26.1"
+version = "0.26.2"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Rust library to install conda environments"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
@@ -15,19 +15,19 @@
 default = ['native-tls']
 native-tls = ['reqwest/native-tls', 'rattler_package_streaming/native-tls']
 rustls-tls = ['reqwest/rustls-tls', 'rattler_package_streaming/rustls-tls']
 cli-tools = ['dep:clap']
 indicatif = ['dep:indicatif', 'dep:console']
 
 [dependencies]
-rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.0", default-features = false }
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.25.1", default-features = false }
 rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false }
 rattler_networking = { path = "../rattler_networking", version = "0.20.8", default-features = false }
-rattler_shell = { path = "../rattler_shell", version = "0.20.6", default-features = false }
-rattler_package_streaming = { path = "../rattler_package_streaming", version = "0.21.1", default-features = false, features = ["reqwest"] }
+rattler_shell = { path = "../rattler_shell", version = "0.20.7", default-features = false }
+rattler_package_streaming = { path = "../rattler_package_streaming", version = "0.21.2", default-features = false, features = ["reqwest"] }
 simple_spawn_blocking = { path = "../simple_spawn_blocking", version = "1.0", default-features = false, features = ["tokio"] }
 anyhow = "1.0.82"
 bytes = "1.6.0"
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.26.2](https://github.com/mamba-org/rattler/compare/rattler-v0.26.1...rattler-v0.26.2) - 2024-06-03
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_package_streaming
+
 ## [0.26.1](https://github.com/mamba-org/rattler/compare/rattler-v0.26.0...rattler-v0.26.1) - 2024-05-28
 
 ### Other
 - updated the following local packages: rattler_conda_types
 
 ## [0.26.0](https://github.com/mamba-org/rattler/compare/rattler-v0.25.0...rattler-v0.26.0) - 2024-05-27
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/resources/launcher64.exe` & `py_rattler-0.6.2/local_dependencies/rattler/resources/launcher64.exe`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/resources/versions.txt` & `py_rattler-0.6.2/local_dependencies/rattler/resources/versions.txt`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/cli/auth.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/cli/auth.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/apple_codesign.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/apple_codesign.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/clobber_registry.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/clobber_registry.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/driver.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/driver.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/entry_point.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/entry_point.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/error.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/error.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/indicatif.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/indicatif.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/installer/reporter.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/installer/reporter.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/link.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/link_script.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/link_script.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/python.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/python.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/test_utils.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/test_utils.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/transaction.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/transaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/install/unlink.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/install/unlink.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/package_cache.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/package_cache.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/range.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/range.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler/src/validation.rs` & `py_rattler-0.6.2/local_dependencies/rattler/src/validation.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_solve/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [package]
 name = "rattler_solve"
-version = "0.23.1"
+version = "0.24.0"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "A crate to solve conda environments"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.1", default-features = false }
 rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
 rattler_libsolv_c = { path= "../rattler_libsolv_c", version = "0.19.3", default-features = false, optional = true }
 libc = { version = "0.2" , optional = true }
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
 thiserror = "1.0"
 tracing = "0.1.40"
 itertools = "0.12.1"
 url = { version = "2.5.0" }
 tempfile = "3.10.1"
-resolvo = { version = "0.4.1" , optional = true }
+resolvo = { version = "0.5.0" , optional = true }
 futures = { version = "0.3.30", optional = true }
 serde = { version = "1.0.198" , optional = true }
 
 [features]
 default = ["resolvo"]
 libsolv_c = ["rattler_libsolv_c", "libc"]
 resolvo = ["dep:resolvo", "dep:futures"]
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_solve/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.24.0](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.23.2...rattler_solve-v0.24.0) - 2024-06-03
+
+### Added
+- add constraints to solve ([#713](https://github.com/mamba-org/rattler/pull/713))
+
+## [0.23.2](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.23.1...rattler_solve-v0.23.2) - 2024-05-28
+
+### Fixed
+- ChannelPriority implements Debug ([#701](https://github.com/mamba-org/rattler/pull/701))
+
 ## [0.23.1](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.23.0...rattler_solve-v0.23.1) - 2024-05-28
 
 ### Added
 - add run exports to package data ([#671](https://github.com/mamba-org/rattler/pull/671))
 
 ### Other
 - enable serialization of enums ([#698](https://github.com/mamba-org/rattler/pull/698))
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/benches/bench.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 write!(f, "encountered duplicate records for {filename}")
             }
         }
     }
 }
 
 /// Represents the channel priority option to use during solves.
-#[derive(Clone, Copy, PartialEq, Eq, Default)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, Default)]
 #[cfg_attr(feature = "serde", derive(serde::Serialize, serde::Deserialize))]
 #[cfg_attr(feature = "serde", serde(rename_all = "kebab-case"))]
 pub enum ChannelPriority {
     /// The channel that the package is first found in will be used as the only
     /// channel for that package.
     #[default]
     Strict,
@@ -127,14 +127,19 @@
 
     /// Virtual packages considered active
     pub virtual_packages: Vec<GenericVirtualPackage>,
 
     /// The specs we want to solve
     pub specs: Vec<MatchSpec>,
 
+    /// Additional constraints that should be satisfied by the solver.
+    /// Packages included in the `constraints` are not necessarily
+    /// installed, but they must be satisfied by the solution.
+    pub constraints: Vec<MatchSpec>,
+
     /// The timeout after which the solver should stop
     pub timeout: Option<std::time::Duration>,
 
     /// The channel priority to solve with, either [`ChannelPriority::Strict`]
     /// or [`ChannelPriority::Disabled`]
     pub channel_priority: ChannelPriority,
 
@@ -152,14 +157,15 @@
     fn from_iter<T: IntoIterator<Item = I>>(iter: T) -> Self {
         Self {
             available_packages: iter.into_iter().map(|iter| RepoDataIter(iter)).collect(),
             locked_packages: Vec::new(),
             pinned_packages: Vec::new(),
             virtual_packages: Vec::new(),
             specs: Vec::new(),
+            constraints: Vec::new(),
             timeout: None,
             channel_priority: ChannelPriority::default(),
             exclude_newer: None,
             strategy: SolveStrategy::default(),
         }
     }
 }
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/input.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/input.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,19 @@
 
         // Specify the matchspec requests
         for spec in task.specs {
             let id = pool.intern_matchspec(&spec);
             goal.install(id, false);
         }
 
+        for spec in task.constraints {
+            let id = pool.intern_matchspec(&spec);
+            goal.install(id, true);
+        }
+
         // Construct a solver and solve the problems in the queue
         let mut solver = pool.create_solver();
         solver.set_flag(SolverFlag::allow_uninstall(), true);
         solver.set_flag(SolverFlag::allow_downgrade(), true);
         solver.set_flag(
             SolverFlag::strict_channel_priority(),
             task.channel_priority == ChannelPriority::Strict,
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/output.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/output.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/conda_util.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/resolvo/conda_util.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/src/resolvo/mod.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/src/resolvo/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -564,30 +564,41 @@
                 let (name, spec) = spec.clone().into_nameless();
                 let name = name.expect("cannot use matchspec without a name");
                 let name_id = provider.pool.intern_package_name(name.as_normalized());
                 provider.pool.intern_version_set(name_id, spec.into())
             })
             .collect();
 
+        let root_constraints = task
+            .constraints
+            .iter()
+            .map(|spec| {
+                let (name, spec) = spec.clone().into_nameless();
+                let name = name.expect("cannot use matchspec without a name");
+                let name_id = provider.pool.intern_package_name(name.as_normalized());
+                provider.pool.intern_version_set(name_id, spec.into())
+            })
+            .collect();
+
         // Construct a solver and solve the problems in the queue
         let mut solver = LibSolvRsSolver::new(provider);
-        let solvables = solver
-            .solve(root_requirements)
-            .map_err(|unsolvable_or_cancelled| {
+        let solvables = solver.solve(root_requirements, root_constraints).map_err(
+            |unsolvable_or_cancelled| {
                 match unsolvable_or_cancelled {
                     UnsolvableOrCancelled::Unsolvable(problem) => {
                         SolveError::Unsolvable(vec![problem
                             .display_user_friendly(&solver, pool, &CondaSolvableDisplay)
                             .to_string()])
                     }
                     // We are not doing this as of yet
                     // put a generic message in here for now
                     UnsolvableOrCancelled::Cancelled(_) => SolveError::Cancelled,
                 }
-            })?;
+            },
+        )?;
 
         // Get the resulting packages from the solver.
         let required_records = solvables
             .into_iter()
             .filter_map(|id| match *solver.pool.resolve_solvable(id).inner() {
                 SolverPackageRecord::Record(rec) => Some(rec.clone()),
                 SolverPackageRecord::VirtualPackage(_) => None,
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/backends.rs` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/backends.rs`

 * *Files 11% similar despite different names*

```diff
@@ -536,14 +536,35 @@
 
             let result = <$T>::default().solve(task);
             match result {
                Err(rattler_solve::SolveError::DuplicateRecords(_)) => {},
                 _ => panic!("expected a DuplicateRecord error"),
             }
         }
+
+        #[test]
+        fn test_constraints() {
+            // There following package is provided as .tar.bz and as .conda in repodata.json
+            let mut operations = solve::<$T>(
+                dummy_channel_json_path(),
+                SimpleSolveTask {
+                    specs: &["foobar"],
+                    constraints: vec!["bors <=1", "nonexisting"],
+                    ..SimpleSolveTask::default()
+                },
+            )
+            .unwrap();
+
+            // Sort operations by file name to make the test deterministic
+            operations.sort_by(|a, b| a.file_name.cmp(&b.file_name));
+
+            assert_eq!(operations.len(), 2);
+            assert_eq!(operations[0].file_name, "bors-1.0-bla_1.tar.bz2");
+            assert_eq!(operations[1].file_name, "foobar-2.1-bla_1.tar.bz2");
+        }
     };
 }
 
 #[cfg(feature = "libsolv_c")]
 mod libsolv_c {
     #![allow(unused_imports)] // For some reason windows thinks this is an unused import.
 
@@ -588,14 +609,15 @@
 
         let pkgs = rattler_solve::libsolv_c::Solver
             .solve(SolverTask {
                 locked_packages: Vec::new(),
                 virtual_packages: Vec::new(),
                 available_packages: [libsolv_repodata],
                 specs,
+                constraints: Vec::new(),
                 pinned_packages: Vec::new(),
                 timeout: None,
                 channel_priority: ChannelPriority::default(),
                 exclude_newer: None,
                 strategy: SolveStrategy::default(),
             })
             .unwrap();
@@ -764,14 +786,15 @@
         );
     }
 }
 
 #[derive(Default)]
 struct SimpleSolveTask<'a> {
     specs: &'a [&'a str],
+    constraints: Vec<&'a str>,
     installed_packages: Vec<RepoDataRecord>,
     pinned_packages: Vec<RepoDataRecord>,
     virtual_packages: Vec<GenericVirtualPackage>,
     exclude_newer: Option<DateTime<Utc>>,
     strategy: SolveStrategy,
 }
 
@@ -783,18 +806,25 @@
 
     let specs: Vec<_> = task
         .specs
         .iter()
         .map(|m| MatchSpec::from_str(m, ParseStrictness::Lenient).unwrap())
         .collect();
 
+    let constraints = task
+        .constraints
+        .into_iter()
+        .map(|m| MatchSpec::from_str(m, ParseStrictness::Lenient).unwrap())
+        .collect();
+
     let task = SolverTask {
         locked_packages: task.installed_packages,
         virtual_packages: task.virtual_packages,
         specs,
+        constraints,
         pinned_packages: task.pinned_packages,
         exclude_newer: task.exclude_newer,
         strategy: task.strategy,
         ..SolverTask::from_iter([&repo_data])
     };
 
     let pkgs = T::default().solve(task)?;
@@ -938,108 +968,97 @@
 fn compare_solve_xtensor_xsimd() {
     compare_solve(CompareTask {
         specs: vec!["xtensor", "xsimd"],
         ..CompareTask::default()
     });
 }
 
-fn solve_to_get_channel_of_spec(
+fn solve_to_get_channel_of_spec<T: SolverImpl + Default>(
     spec_str: &str,
     expected_channel: &str,
     repo_data: Vec<&SparseRepoData>,
     channel_priority: ChannelPriority,
-    use_resolvo: bool,
 ) {
     let spec = MatchSpec::from_str(spec_str, ParseStrictness::Lenient).unwrap();
     let specs = vec![spec.clone()];
     let names = specs.iter().filter_map(|s| s.name.as_ref().cloned());
 
     let available_packages =
         SparseRepoData::load_records_recursive(repo_data, names, None).unwrap();
 
     let task = SolverTask {
         specs: specs.clone(),
         channel_priority,
         ..SolverTask::from_iter(&available_packages)
     };
 
-    let result = if use_resolvo {
-        rattler_solve::resolvo::Solver.solve(task).unwrap()
-    } else {
-        rattler_solve::libsolv_c::Solver.solve(task).unwrap()
-    };
+    let result = T::default().solve(task).unwrap();
 
     let record = result.iter().find(|record| {
         record.package_record.name.as_normalized() == spec.name.as_ref().unwrap().as_normalized()
     });
     assert_eq!(record.unwrap().channel, expected_channel.to_string());
 }
 
 #[test]
 fn channel_specific_requirement() {
     let repodata = vec![
         read_conda_forge_sparse_repo_data(),
         read_pytorch_sparse_repo_data(),
     ];
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "conda-forge::pytorch-cpu",
         "https://conda.anaconda.org/conda-forge/",
         repodata.clone(),
         ChannelPriority::Strict,
-        true,
     );
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "conda-forge::pytorch-cpu",
         "https://conda.anaconda.org/conda-forge/",
         repodata.clone(),
         ChannelPriority::Disabled,
-        true,
     );
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "pytorch::pytorch-cpu",
         "https://conda.anaconda.org/pytorch/",
         repodata.clone(),
         ChannelPriority::Strict,
-        true,
     );
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "pytorch::pytorch-cpu",
         "https://conda.anaconda.org/pytorch/",
         repodata,
         ChannelPriority::Disabled,
-        true,
     );
 }
 
 #[test]
 fn channel_priority_strict() {
     // Solve with conda-forge as the first channel
     let repodata = vec![
         read_conda_forge_sparse_repo_data(),
         read_pytorch_sparse_repo_data(),
     ];
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "pytorch-cpu",
         "https://conda.anaconda.org/conda-forge/",
         repodata,
         ChannelPriority::Strict,
-        true,
     );
 
     // Solve with pytorch as the first channel
     let repodata = vec![
         read_pytorch_sparse_repo_data(),
         read_conda_forge_sparse_repo_data(),
     ];
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "pytorch-cpu",
         "https://conda.anaconda.org/pytorch/",
         repodata,
         ChannelPriority::Strict,
-        true,
     );
 }
 
 #[test]
 #[should_panic(
     expected = "called `Result::unwrap()` on an `Err` value: Unsolvable([\"The following packages \
     are incompatible\\n└─ pytorch-cpu ==0.4.1 py36_cpu_1 cannot be installed because there are no \
@@ -1047,66 +1066,64 @@
     not using this option from: 'https://conda.anaconda.org/pytorch/'\\n\"])"
 )]
 fn channel_priority_strict_panic() {
     let repodata = vec![
         read_conda_forge_sparse_repo_data(),
         read_pytorch_sparse_repo_data(),
     ];
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "pytorch-cpu=0.4.1=py36_cpu_1",
         "https://conda.anaconda.org/pytorch/",
         repodata,
         ChannelPriority::Strict,
-        true,
     );
 }
 
 #[test]
 fn channel_priority_disabled() {
     let repodata = vec![
         read_conda_forge_sparse_repo_data(),
         read_pytorch_sparse_repo_data(),
     ];
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::resolvo::Solver>(
         "pytorch-cpu=0.4.1=py36_cpu_1",
         "https://conda.anaconda.org/pytorch/",
         repodata,
         ChannelPriority::Disabled,
-        true,
     );
 }
 
+#[cfg(feature = "libsolv_c")]
 #[test]
 #[should_panic(
     expected = "called `Result::unwrap()` on an `Err` value: Unsolvable([\"package \
     pytorch-cpu-0.4.1-py36_cpu_1 is excluded by strict repo priority\"])"
 )]
 fn channel_priority_strict_libsolv_c() {
     let repodata = vec![
         read_conda_forge_sparse_repo_data(),
         read_pytorch_sparse_repo_data(),
     ];
 
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::libsolv_c::Solver>(
         "pytorch-cpu=0.4.1=py36_cpu_1",
         "https://conda.anaconda.org/pytorch/",
         repodata,
         ChannelPriority::Strict,
-        false,
     );
 }
 
+#[cfg(feature = "libsolv_c")]
 #[test]
 fn channel_priority_disabled_libsolv_c() {
     let repodata = vec![
         read_conda_forge_sparse_repo_data(),
         read_pytorch_sparse_repo_data(),
     ];
 
-    solve_to_get_channel_of_spec(
+    solve_to_get_channel_of_spec::<rattler_solve::libsolv_c::Solver>(
         "pytorch-cpu=0.4.1=py36_cpu_1",
         "https://conda.anaconda.org/pytorch/",
         repodata,
         ChannelPriority::Disabled,
-        false,
     );
 }
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap` & `py_rattler-0.6.2/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/simple_spawn_blocking/src/tokio.rs` & `py_rattler-0.6.2/local_dependencies/simple_spawn_blocking/src/tokio.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/Cargo.toml` & `py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_virtual_packages"
-version = "0.19.13"
+version = "0.19.14"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Library to work with and detect Conda virtual packages"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.25.1", default-features = false }
 libloading = "0.8.3"
 nom = "7.1.3"
 once_cell = "1.19.0"
 regex = "1.10.4"
 serde = { version = "1.0.198" , features = ["derive"] }
 thiserror = "1.0"
 tracing = "0.1.40"
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/CHANGELOG.md` & `py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.19.14](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.13...rattler_virtual_packages-v0.19.14) - 2024-06-03
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.19.13](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.12...rattler_virtual_packages-v0.19.13) - 2024-05-28
 
 ### Other
 - updated the following local packages: rattler_conda_types
 
 ## [0.19.12](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.11...rattler_virtual_packages-v0.19.12) - 2024-05-27
```

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/cuda.rs` & `py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/cuda.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/lib.rs` & `py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/libc.rs` & `py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/libc.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/linux.rs` & `py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/linux.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/local_dependencies/rattler_virtual_packages/src/osx.rs` & `py_rattler-0.6.2/local_dependencies/rattler_virtual_packages/src/osx.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/Cargo.toml` & `py_rattler-0.6.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-rattler"
-version = "0.6.1"
+version = "0.6.2"
 edition = "2021"
 license = "BSD-3-Clause"
 publish = false
 
 [lib]
 name = "rattler"
 crate-type = ["cdylib"]
```

### Comparing `py_rattler-0.6.1/.gitignore` & `py_rattler-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/LICENSE` & `py_rattler-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/README.md` & `py_rattler-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/docs/index.md` & `py_rattler-0.6.2/docs/index.md`

 * *Files 25% similar despite different names*

```diff
@@ -66,285 +66,175 @@
 00000410: 7420 6c61 6e67 7561 6765 7320 746f 206d  t languages to m
 00000420: 616b 6520 6974 2065 6173 7920 746f 2069  ake it easy to i
 00000430: 6e74 6567 7261 7465 2052 6174 746c 6572  ntegrate Rattler
 00000440: 2069 6e20 6e6f 6e2d 7275 7374 2070 726f   in non-rust pro
 00000450: 6a65 6374 732e 0a50 792d 7261 7474 6c65  jects..Py-rattle
 00000460: 7220 6973 2074 6865 2070 7974 686f 6e20  r is the python 
 00000470: 6269 6e64 696e 6773 2066 6f72 2072 6174  bindings for rat
-00000480: 746c 6572 2e0a 0a23 2320 5768 6174 2069  tler...## What i
-00000490: 7320 636f 6e64 6120 2620 636f 6e64 612d  s conda & conda-
-000004a0: 666f 7267 653f 0a0a 5468 6520 636f 6e64  forge?..The cond
-000004b0: 6120 6563 6f73 7973 7465 6d20 7072 6f76  a ecosystem prov
-000004c0: 6964 6573 202a 2a63 726f 7373 2d70 6c61  ides **cross-pla
-000004d0: 7466 6f72 6d2a 2a2c 202a 2a62 696e 6172  tform**, **binar
-000004e0: 792a 2a20 7061 636b 6167 6573 2074 6861  y** packages tha
-000004f0: 7420 796f 7520 6361 6e20 7573 6520 7769  t you can use wi
-00000500: 7468 202a 2a61 6e79 2070 726f 6772 616d  th **any program
-00000510: 6d69 6e67 206c 616e 6775 6167 652a 2a2e  ming language**.
-00000520: 0a60 636f 6e64 6160 2069 7320 616e 206f  .`conda` is an o
-00000530: 7065 6e2d 736f 7572 6365 2070 6163 6b61  pen-source packa
-00000540: 6765 206d 616e 6167 656d 656e 7420 7379  ge management sy
-00000550: 7374 656d 2061 6e64 2065 6e76 6972 6f6e  stem and environ
-00000560: 6d65 6e74 206d 616e 6167 656d 656e 7420  ment management 
-00000570: 7379 7374 656d 2074 6861 7420 6361 6e20  system that can 
-00000580: 696e 7374 616c 6c20 616e 6420 6d61 6e61  install and mana
-00000590: 6765 206d 756c 7469 706c 6520 7665 7273  ge multiple vers
-000005a0: 696f 6e73 206f 6620 736f 6674 7761 7265  ions of software
-000005b0: 2070 6163 6b61 6765 7320 616e 6420 7468   packages and th
-000005c0: 6569 7220 6465 7065 6e64 656e 6369 6573  eir dependencies
-000005d0: 2e0a 6063 6f6e 6461 6020 6973 2077 7269  ..`conda` is wri
-000005e0: 7474 656e 2069 6e20 5079 7468 6f6e 2e0a  tten in Python..
-000005f0: 5468 6520 6169 6d20 6f66 2052 6174 746c  The aim of Rattl
-00000600: 6572 2069 7320 746f 2070 726f 7669 6465  er is to provide
-00000610: 2061 6c6c 2066 756e 6374 696f 6e61 6c69   all functionali
-00000620: 7479 2072 6571 7569 7265 6420 746f 2077  ty required to w
-00000630: 6f72 6b20 7769 7468 2074 6865 2063 6f6e  ork with the con
-00000640: 6461 2065 636f 7379 7374 656d 2066 726f  da ecosystem fro
-00000650: 6d20 5275 7374 2e0a 5261 7474 6c65 7220  m Rust..Rattler 
-00000660: 6973 206e 6f74 2061 2072 6569 6d70 6c65  is not a reimple
-00000670: 6d65 6e74 6174 696f 6e20 6f66 2060 636f  mentation of `co
-00000680: 6e64 6160 2e0a 6063 6f6e 6461 6020 6973  nda`..`conda` is
-00000690: 2061 2070 6163 6b61 6765 206d 616e 6167   a package manag
-000006a0: 656d 656e 7420 746f 6f6c 2e0a 5261 7474  ement tool..Ratt
-000006b0: 6c65 7220 6973 2061 205f 6c69 6272 6172  ler is a _librar
-000006c0: 795f 2074 6f20 776f 726b 2077 6974 6820  y_ to work with 
-000006d0: 7468 6520 636f 6e64 6120 6563 6f73 7973  the conda ecosys
-000006e0: 7465 6d20 6672 6f6d 2064 6966 6665 7265  tem from differe
-000006f0: 6e74 206c 616e 6775 6167 6573 2061 6e64  nt languages and
-00000700: 2061 7070 6c69 6361 7469 6f6e 732e 0a46   applications..F
-00000710: 6f72 2065 7861 6d70 6c65 2c20 6974 2070  or example, it p
-00000720: 6f77 6572 7320 7468 6520 6261 636b 656e  owers the backen
-00000730: 6420 6f66 2068 7474 7073 3a2f 2f70 7265  d of https://pre
-00000740: 6669 782e 6465 762e 0a0a 6063 6f6e 6461  fix.dev...`conda
-00000750: 2d66 6f72 6765 6020 6973 2061 2063 6f6d  -forge` is a com
-00000760: 6d75 6e69 7479 2d64 7269 7665 6e20 6566  munity-driven ef
-00000770: 666f 7274 2074 6f20 6272 696e 6720 6e65  fort to bring ne
-00000780: 7720 616e 6420 6578 6973 7469 6e67 2073  w and existing s
-00000790: 6f66 7477 6172 6520 696e 746f 2074 6865  oftware into the
-000007a0: 2063 6f6e 6461 2065 636f 7379 7374 656d   conda ecosystem
-000007b0: 2e0a 4974 2070 726f 7669 6465 7320 5f74  ..It provides _t
-000007c0: 656e 732d 6f66 2d74 686f 7573 616e 6473  ens-of-thousands
-000007d0: 206f 6620 7570 2d74 6f2d 6461 7465 5f20   of up-to-date_ 
-000007e0: 7061 636b 6167 6573 2074 6861 7420 6172  packages that ar
-000007f0: 6520 6d61 696e 7461 696e 6564 2062 7920  e maintained by 
-00000800: 6120 636f 6d6d 756e 6974 7920 6f66 2063  a community of c
-00000810: 6f6e 7472 6962 7574 6f72 732e 0a46 6f72  ontributors..For
-00000820: 2061 6e20 6f76 6572 7669 6577 206f 6620   an overview of 
-00000830: 6176 6169 6c61 626c 6520 7061 636b 6167  available packag
-00000840: 6573 2073 6565 2068 7474 7073 3a2f 2f70  es see https://p
-00000850: 7265 6669 782e 6465 762e 0a0a 2323 2048  refix.dev...## H
-00000860: 6f77 2073 686f 756c 6420 4920 7573 6520  ow should I use 
-00000870: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-00000880: 6e3f 0a0a 4966 2079 6f75 2061 7265 2067  n?..If you are g
-00000890: 6574 7469 6e67 2073 7461 7274 6564 2077  etting started w
-000008a0: 6974 6820 7468 6520 6c69 6272 6172 792c  ith the library,
-000008b0: 2079 6f75 2073 686f 756c 6420 666f 6c6c   you should foll
-000008c0: 6f77 2074 6865 2027 4669 7273 7420 5374  ow the 'First St
-000008d0: 6570 7327 2073 6563 7469 6f6e 2069 6e20  eps' section in 
-000008e0: 6f72 6465 722e 0a59 6f75 2063 616e 2061  order..You can a
-000008f0: 6c73 6f20 7573 6520 7468 6520 6d65 6e75  lso use the menu
-00000900: 206f 6e20 7468 6520 6c65 6674 2074 6f20   on the left to 
-00000910: 7175 6963 6b6c 7920 736b 6970 206f 7665  quickly skip ove
-00000920: 7220 7365 6374 696f 6e73 2061 6e64 2073  r sections and s
-00000930: 6561 7263 6820 666f 7220 7370 6563 6966  earch for specif
-00000940: 6963 2074 6869 6e67 732e 0a0a 2323 2049  ic things...## I
-00000950: 6e73 7461 6c6c 6174 696f 6e0a 0a50 792d  nstallation..Py-
-00000960: 5261 7474 6c65 7220 6973 2061 2070 7974  Rattler is a pyt
-00000970: 686f 6e20 6c69 6272 6172 792c 2077 6869  hon library, whi
-00000980: 6368 206d 6561 6e73 2079 6f75 206e 6565  ch means you nee
-00000990: 6420 746f 2064 6f77 6e6c 6f61 6420 616e  d to download an
-000009a0: 6420 696e 7374 616c 6c20 5079 7468 6f6e  d install Python
-000009b0: 2066 726f 6d20 6874 7470 733a 2f2f 7777   from https://ww
-000009c0: 772e 7079 7468 6f6e 2e6f 7267 2f64 6f77  w.python.org/dow
-000009d0: 6e6c 6f61 6473 0a69 6620 796f 7520 6861  nloads.if you ha
-000009e0: 7665 6e27 7420 616c 7265 6164 792e 2041  ven't already. A
-000009f0: 6c74 6572 6e61 7469 7665 6c79 2c20 796f  lternatively, yo
-00000a00: 7520 6361 6e20 7573 6520 6361 6e20 6765  u can use can ge
-00000a10: 7420 7669 6120 636f 6e64 612e 0a0a 2323  t via conda...##
-00000a20: 2320 5079 7069 0a0a 6060 6073 6865 6c6c  # Pypi..```shell
-00000a30: 0a24 2070 7974 686f 6e33 202d 6d20 7069  .$ python3 -m pi
-00000a40: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
-00000a50: 6164 6520 7079 2d72 6174 746c 6572 0a60  ade py-rattler.`
-00000a60: 6060 0a0a 2323 2320 5069 7869 0a0a 6060  ``..### Pixi..``
-00000a70: 6073 6865 6c6c 0a24 2070 6978 6920 6164  `shell.$ pixi ad
-00000a80: 6420 7079 2d72 6174 746c 6572 0a60 6060  d py-rattler.```
-00000a90: 0a0a 2323 2320 436f 6e64 610a 0a60 6060  ..### Conda..```
-00000aa0: 7368 656c 6c0a 2420 636f 6e64 6120 696e  shell.$ conda in
-00000ab0: 7374 616c 6c20 7079 2d72 6174 746c 6572  stall py-rattler
-00000ac0: 0a60 6060 0a0a 2323 2320 4d61 6d62 610a  .```..### Mamba.
-00000ad0: 0a60 6060 7368 656c 6c0a 2420 6d61 6d62  .```shell.$ mamb
-00000ae0: 6120 696e 7374 616c 6c20 7079 2d72 6174  a install py-rat
-00000af0: 746c 6572 202d 6320 636f 6e64 612d 666f  tler -c conda-fo
-00000b00: 7267 650a 6060 600a 0a23 2320 5175 6963  rge.```..## Quic
-00000b10: 6b2d 5374 6172 740a 0a4c 6574 2773 2073  k-Start..Let's s
-00000b20: 6565 2061 6e20 6578 616d 706c 6520 746f  ee an example to
-00000b30: 206c 6561 726e 2073 6f6d 6520 6f66 2074   learn some of t
-00000b40: 6865 2066 756e 6374 696f 6e61 6c69 7479  he functionality
-00000b50: 2074 6865 206c 6962 7261 7279 2068 6173   the library has
-00000b60: 2074 6f20 6f66 6665 722e 0a0a 6060 6070   to offer...```p
-00000b70: 7974 686f 6e0a 0a69 6d70 6f72 7420 6173  ython..import as
-00000b80: 796e 6369 6f0a 0a66 726f 6d20 7261 7474  yncio..from ratt
-00000b90: 6c65 7220 696d 706f 7274 2066 6574 6368  ler import fetch
-00000ba0: 5f72 6570 6f5f 6461 7461 2c20 736f 6c76  _repo_data, solv
-00000bb0: 652c 206c 696e 6b2c 2043 6861 6e6e 656c  e, link, Channel
-00000bc0: 2c20 506c 6174 666f 726d 2c20 4d61 7463  , Platform, Matc
-00000bd0: 6853 7065 632c 2056 6972 7475 616c 5061  hSpec, VirtualPa
-00000be0: 636b 6167 650a 0a64 6566 2064 6f77 6e6c  ckage..def downl
-00000bf0: 6f61 645f 6361 6c6c 6261 636b 2864 6f6e  oad_callback(don
-00000c00: 652c 2074 6f74 616c 293a 0a20 2020 2070  e, total):.    p
-00000c10: 7269 6e74 2822 222c 2065 6e64 203d 2022  rint("", end = "
-00000c20: 5c72 2229 0a20 2020 2070 7269 6e74 2866  \r").    print(f
-00000c30: 277b 646f 6e65 2f31 3032 342f 3130 3234  '{done/1024/1024
-00000c40: 3a2e 3266 7d4d 6942 2f7b 746f 7461 6c2f  :.2f}MiB/{total/
-00000c50: 3130 3234 2f31 3032 343a 2e32 667d 4d69  1024/1024:.2f}Mi
-00000c60: 4227 2c20 656e 6420 3d20 225c 7222 290a  B', end = "\r").
-00000c70: 2020 2020 6966 2064 6f6e 6520 3d3d 2074      if done == t
-00000c80: 6f74 616c 3a0a 2020 2020 2020 2020 7072  otal:.        pr
-00000c90: 696e 7428 290a 0a61 7379 6e63 2064 6566  int()..async def
-00000ca0: 206d 6169 6e28 293a 0a20 2020 2023 2063   main():.    # c
-00000cb0: 6861 6e6e 656c 2074 6f20 7573 6520 746f  hannel to use to
-00000cc0: 2067 6574 2074 6865 2064 6570 656e 6465   get the depende
-00000cd0: 6e63 6965 730a 2020 2020 6368 616e 6e65  ncies.    channe
-00000ce0: 6c20 3d20 4368 616e 6e65 6c28 2263 6f6e  l = Channel("con
-00000cf0: 6461 2d66 6f72 6765 2229 0a0a 2020 2020  da-forge")..    
-00000d00: 2320 6c69 7374 206f 6620 6465 7065 6e64  # list of depend
-00000d10: 656e 6369 6573 2074 6f20 696e 7374 616c  encies to instal
-00000d20: 6c20 696e 2074 6865 2065 6e76 0a20 2020  l in the env.   
-00000d30: 206d 6174 6368 5f73 7065 6373 203d 205b   match_specs = [
-00000d40: 0a20 2020 2020 2020 204d 6174 6368 5370  .        MatchSp
-00000d50: 6563 2822 7079 7468 6f6e 207e 3d33 2e31  ec("python ~=3.1
-00000d60: 322e 2a22 292c 0a20 2020 2020 2020 204d  2.*"),.        M
-00000d70: 6174 6368 5370 6563 2822 7069 7022 292c  atchSpec("pip"),
-00000d80: 0a20 2020 2020 2020 204d 6174 6368 5370  .        MatchSp
-00000d90: 6563 2822 7265 7175 6573 7473 2032 2e33  ec("requests 2.3
-00000da0: 312e 3022 290a 2020 2020 5d0a 0a20 2020  1.0").    ]..   
-00000db0: 2023 206c 6973 7420 6f66 2070 6c61 7466   # list of platf
-00000dc0: 6f72 6d73 2074 6f20 6765 7420 7468 6520  orms to get the 
-00000dd0: 7265 706f 2064 6174 610a 2020 2020 706c  repo data.    pl
-00000de0: 6174 666f 726d 7320 3d20 5b50 6c61 7466  atforms = [Platf
-00000df0: 6f72 6d2e 6375 7272 656e 7428 292c 2050  orm.current(), P
-00000e00: 6c61 7466 6f72 6d28 226e 6f61 7263 6822  latform("noarch"
-00000e10: 295d 0a0a 2020 2020 7669 7274 7561 6c5f  )]..    virtual_
-00000e20: 7061 636b 6167 6573 203d 205b 702e 696e  packages = [p.in
-00000e30: 746f 5f67 656e 6572 6963 2829 2066 6f72  to_generic() for
-00000e40: 2070 2069 6e20 5669 7274 7561 6c50 6163   p in VirtualPac
-00000e50: 6b61 6765 2e63 7572 7265 6e74 2829 5d0a  kage.current()].
-00000e60: 0a20 2020 2063 6163 6865 5f70 6174 6820  .    cache_path 
-00000e70: 3d20 222f 746d 702f 7079 2d72 6174 746c  = "/tmp/py-rattl
-00000e80: 6572 2d63 6163 6865 2f22 0a20 2020 2065  er-cache/".    e
-00000e90: 6e76 5f70 6174 6820 3d20 222f 746d 702f  nv_path = "/tmp/
-00000ea0: 656e 762d 7061 7468 2f65 6e76 220a 0a20  env-path/env".. 
-00000eb0: 2020 2070 7269 6e74 2822 7374 6172 7465     print("starte
-00000ec0: 6420 6665 7463 6869 6e67 2072 6570 6f5f  d fetching repo_
-00000ed0: 6461 7461 2229 0a20 2020 2072 6570 6f5f  data").    repo_
-00000ee0: 6461 7461 203d 2061 7761 6974 2066 6574  data = await fet
-00000ef0: 6368 5f72 6570 6f5f 6461 7461 280a 2020  ch_repo_data(.  
-00000f00: 2020 2020 2020 6368 616e 6e65 6c73 203d        channels =
-00000f10: 205b 6368 616e 6e65 6c5d 2c0a 2020 2020   [channel],.    
-00000f20: 2020 2020 706c 6174 666f 726d 7320 3d20      platforms = 
-00000f30: 706c 6174 666f 726d 732c 0a20 2020 2020  platforms,.     
-00000f40: 2020 2063 6163 6865 5f70 6174 6820 3d20     cache_path = 
-00000f50: 6622 7b63 6163 6865 5f70 6174 687d 2f72  f"{cache_path}/r
-00000f60: 6570 6f64 6174 6122 2c0a 2020 2020 2020  epodata",.      
-00000f70: 2020 6361 6c6c 6261 636b 203d 2064 6f77    callback = dow
-00000f80: 6e6c 6f61 645f 6361 6c6c 6261 636b 2c0a  nload_callback,.
-00000f90: 2020 2020 290a 2020 2020 7072 696e 7428      ).    print(
-00000fa0: 2266 696e 6973 6865 6420 6665 7463 6869  "finished fetchi
-00000fb0: 6e67 2072 6570 6f5f 6461 7461 2229 0a0a  ng repo_data")..
-00000fc0: 2020 2020 736f 6c76 6564 5f64 6570 656e      solved_depen
-00000fd0: 6465 6e63 6965 7320 3d20 736f 6c76 6528  dencies = solve(
-00000fe0: 0a20 2020 2020 2020 2073 7065 6373 203d  .        specs =
-00000ff0: 206d 6174 6368 5f73 7065 6373 2c0a 2020   match_specs,.  
-00001000: 2020 2020 2020 6176 6169 6c61 626c 655f        available_
-00001010: 7061 636b 6167 6573 203d 2072 6570 6f5f  packages = repo_
-00001020: 6461 7461 2c0a 2020 2020 2020 2020 7669  data,.        vi
-00001030: 7274 7561 6c5f 7061 636b 6167 6573 203d  rtual_packages =
-00001040: 2076 6972 7475 616c 5f70 6163 6b61 6765   virtual_package
-00001050: 732c 0a20 2020 2029 0a20 2020 2070 7269  s,.    ).    pri
-00001060: 6e74 2822 736f 6c76 6564 2072 6571 7569  nt("solved requi
-00001070: 7265 6420 6465 7065 6e64 656e 6369 6573  red dependencies
-00001080: 2229 0a0a 2020 2020 6177 6169 7420 6c69  ")..    await li
-00001090: 6e6b 280a 2020 2020 2020 2020 6465 7065  nk(.        depe
-000010a0: 6e64 656e 6369 6573 203d 2073 6f6c 7665  ndencies = solve
-000010b0: 645f 6465 7065 6e64 656e 6369 6573 2c0a  d_dependencies,.
-000010c0: 2020 2020 2020 2020 7461 7267 6574 5f70          target_p
-000010d0: 7265 6669 7820 3d20 656e 765f 7061 7468  refix = env_path
-000010e0: 2c0a 2020 2020 2020 2020 6361 6368 655f  ,.        cache_
-000010f0: 6469 7220 3d20 6622 7b63 6163 6865 5f70  dir = f"{cache_p
-00001100: 6174 687d 2f70 6b67 7322 2c0a 2020 2020  ath}/pkgs",.    
-00001110: 290a 2020 2020 7072 696e 7428 6622 6372  ).    print(f"cr
-00001120: 6561 7465 6420 656e 7669 726f 6e6d 656e  eated environmen
-00001130: 743a 207b 656e 765f 7061 7468 7d22 290a  t: {env_path}").
-00001140: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00001150: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00001160: 6173 796e 6369 6f2e 7275 6e28 6d61 696e  asyncio.run(main
-00001170: 2829 290a 0a60 6060 0a0a 5079 2d72 6174  ())..```..Py-rat
-00001180: 746c 6572 2070 726f 7669 6465 7320 6672  tler provides fr
-00001190: 6965 6e64 6c79 2068 6967 6820 6c65 7665  iendly high leve
-000011a0: 6c20 6675 6e63 7469 6f6e 7320 746f 2064  l functions to d
-000011b0: 6f77 6e6c 6f61 640a 6465 7065 6e64 656e  ownload.dependen
-000011c0: 6369 6573 2061 6e64 2063 7265 6174 6520  cies and create 
-000011d0: 656e 7669 726f 6e6d 656e 7473 2e20 5468  environments. Th
-000011e0: 6973 2069 7320 646f 6e65 2074 6872 6f75  is is done throu
-000011f0: 6768 2074 6865 0a60 6665 7463 685f 7265  gh the.`fetch_re
-00001200: 706f 5f64 6174 6160 2c20 6073 6f6c 7665  po_data`, `solve
-00001210: 6020 616e 6420 606c 696e 6b60 2066 756e  ` and `link` fun
-00001220: 6374 696f 6e73 2e0a 0a2d 2060 6665 7463  ctions...- `fetc
-00001230: 685f 7265 706f 5f64 6174 6160 2061 7320  h_repo_data` as 
-00001240: 7468 6520 6e61 6d65 2069 6d70 6c69 6573  the name implies
-00001250: 2c20 6665 7463 6865 7320 7265 706f 2064  , fetches repo d
-00001260: 6174 6120 6672 6f6d 2063 6f6e 6461 2072  ata from conda r
-00001270: 6567 6973 7472 6965 732e 0a2d 2060 736f  egistries..- `so
-00001280: 6c76 6560 2066 756e 6374 696f 6e20 736f  lve` function so
-00001290: 6c76 6573 2074 6865 2072 6571 7569 7265  lves the require
-000012a0: 6d65 6e74 7320 746f 2067 6574 2061 6c6c  ments to get all
-000012b0: 2074 6865 2070 6163 6b61 6765 730a 2020   the packages.  
-000012c0: 7768 6963 6820 776f 756c 6420 6265 2072  which would be r
-000012d0: 6571 7569 7265 6420 746f 2063 7265 6174  equired to creat
-000012e0: 6520 7468 6520 656e 7669 726f 6e6d 656e  e the environmen
-000012f0: 742e 0a2d 2060 6c69 6e6b 6020 6675 6e63  t..- `link` func
-00001300: 7469 6f6e 2074 616b 6573 2061 206c 6973  tion takes a lis
-00001310: 7420 6f66 2073 6f6c 7665 6420 6465 7065  t of solved depe
-00001320: 6e64 656e 6369 6573 2074 6f20 6372 6561  ndencies to crea
-00001330: 7465 2061 6e0a 2020 656e 7669 726f 6e6d  te an.  environm
-00001340: 656e 742e 0a0a 2323 204e 6578 7420 5374  ent...## Next St
-00001350: 6570 730a 0a54 6865 7365 2062 6173 6963  eps..These basic
-00001360: 2066 6972 7374 2073 7465 7073 2073 686f   first steps sho
-00001370: 756c 6420 6861 7665 2067 6f74 7465 6e20  uld have gotten 
-00001380: 796f 7520 7374 6172 7465 6420 7769 7468  you started with
-00001390: 2074 6865 206c 6962 7261 7279 2e0a 0a42   the library...B
-000013a0: 7920 6e6f 772c 2079 6f75 2073 686f 756c  y now, you shoul
-000013b0: 6420 6b6e 6f77 2068 6f77 2074 6f20 646f  d know how to do
-000013c0: 776e 6c6f 6164 2072 6570 6f20 6461 7461  wnload repo data
-000013d0: 2c20 736f 6c76 6520 6465 7065 6e64 656e  , solve dependen
-000013e0: 6369 6573 2061 6e64 2063 7265 6174 6520  cies and create 
-000013f0: 616e 0a65 6e76 6972 6f6e 6d65 6e74 2e0a  an.environment..
-00001400: 0a4e 6578 742c 2077 6520 7769 6c6c 2073  .Next, we will s
-00001410: 6565 2061 2071 7569 636b 2072 6566 6572  ee a quick refer
-00001420: 656e 6365 2073 756d 6d61 7279 206f 6620  ence summary of 
-00001430: 616c 6c20 7468 6520 6d65 7468 6f64 7320  all the methods 
-00001440: 616e 6420 7072 6f70 6572 7469 6573 2074  and properties t
-00001450: 6861 7420 796f 7520 7769 6c6c 206e 6565  hat you will nee
-00001460: 6420 7768 656e 2075 7369 6e67 2074 6865  d when using the
-00001470: 206c 6962 7261 7279 2e20 4966 2079 6f75   library. If you
-00001480: 2066 6f6c 6c6f 7720 7468 6520 6c69 6e6b   follow the link
-00001490: 7320 7468 6572 652c 2079 6f75 2077 696c  s there, you wil
-000014a0: 6c20 6578 7061 6e64 2074 6865 2064 6f63  l expand the doc
-000014b0: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
-000014c0: 6865 206d 6574 686f 6420 616e 6420 7072  he method and pr
-000014d0: 6f70 6572 7479 2c20 7769 7468 206d 6f72  operty, with mor
-000014e0: 6520 6578 616d 706c 6573 206f 6e20 686f  e examples on ho
-000014f0: 7720 746f 2075 7365 2074 6865 6d2e 0a0a  w to use them...
-00001500: 2323 2043 6f6e 7472 6962 7574 696e 6720  ## Contributing 
-00001510: f09f 988d 0a0a 5765 2077 6f75 6c64 206c  ......We would l
-00001520: 6f76 6520 746f 2068 6176 6520 796f 7520  ove to have you 
-00001530: 636f 6e74 7269 6275 7465 210a 5365 6520  contribute!.See 
-00001540: 7468 6520 434f 4e54 5249 4255 5449 4f4e  the CONTRIBUTION
-00001550: 2e6d 6420 666f 7220 6d6f 7265 2069 6e66  .md for more inf
-00001560: 6f2e 2046 6f72 2071 7565 7374 696f 6e73  o. For questions
-00001570: 2c20 7265 7175 6573 7473 206f 7220 6120  , requests or a 
-00001580: 6361 7375 616c 2063 6861 742c 2077 6520  casual chat, we 
-00001590: 6172 6520 7665 7279 2061 6374 6976 6520  are very active 
-000015a0: 6f6e 206f 7572 205b 6469 7363 6f72 6420  on our [discord 
-000015b0: 7365 7276 6572 5d28 6874 7470 733a 2f2f  server](https://
-000015c0: 6469 7363 6f72 642e 6767 2f6b 4b56 385a  discord.gg/kKV8Z
-000015d0: 7879 7a59 3429 2e0a                      xyzY4)..
+00000480: 746c 6572 2e0a 0a23 2320 5175 6963 6b2d  tler...## Quick-
+00000490: 5374 6172 740a 0a4c 6574 2773 2073 6565  Start..Let's see
+000004a0: 2061 6e20 6578 616d 706c 6520 746f 206c   an example to l
+000004b0: 6561 726e 2073 6f6d 6520 6f66 2074 6865  earn some of the
+000004c0: 2066 756e 6374 696f 6e61 6c69 7479 2074   functionality t
+000004d0: 6865 206c 6962 7261 7279 2068 6173 2074  he library has t
+000004e0: 6f20 6f66 6665 722e 0a0a 6060 6070 7974  o offer...```pyt
+000004f0: 686f 6e0a 2d2d 383c 2d2d 2022 6578 616d  hon.--8<-- "exam
+00000500: 706c 6573 5c73 6f6c 7665 5f61 6e64 5f69  ples\solve_and_i
+00000510: 6e73 7461 6c6c 2e70 7922 0a60 6060 0a0a  nstall.py".```..
+00000520: 5079 2d72 6174 746c 6572 2070 726f 7669  Py-rattler provi
+00000530: 6465 7320 6672 6965 6e64 6c79 2068 6967  des friendly hig
+00000540: 6820 6c65 7665 6c20 6675 6e63 7469 6f6e  h level function
+00000550: 7320 746f 2064 6f77 6e6c 6f61 6420 6465  s to download de
+00000560: 7065 6e64 656e 6369 6573 2061 6e64 2063  pendencies and c
+00000570: 7265 6174 6520 656e 7669 726f 6e6d 656e  reate environmen
+00000580: 7473 2e0a 5468 6520 6073 6f6c 7665 6020  ts..The `solve` 
+00000590: 616e 6420 6069 6e73 7461 6c6c 6020 6675  and `install` fu
+000005a0: 6e63 7469 6f6e 7320 6172 6520 6578 6365  nctions are exce
+000005b0: 6c6c 656e 7420 6578 616d 706c 6573 206f  llent examples o
+000005c0: 6620 7375 6368 2068 6967 682d 6c65 7665  f such high-leve
+000005d0: 6c20 6675 6e63 7469 6f6e 732e 0a0a 2323  l functions...##
+000005e0: 2057 6861 7420 6973 2063 6f6e 6461 2026   What is conda &
+000005f0: 2063 6f6e 6461 2d66 6f72 6765 3f0a 0a54   conda-forge?..T
+00000600: 6865 2063 6f6e 6461 2065 636f 7379 7374  he conda ecosyst
+00000610: 656d 2070 726f 7669 6465 7320 2a2a 6372  em provides **cr
+00000620: 6f73 732d 706c 6174 666f 726d 2a2a 2c20  oss-platform**, 
+00000630: 2a2a 6269 6e61 7279 2a2a 2070 6163 6b61  **binary** packa
+00000640: 6765 7320 7468 6174 2079 6f75 2063 616e  ges that you can
+00000650: 2075 7365 2077 6974 6820 2a2a 616e 7920   use with **any 
+00000660: 7072 6f67 7261 6d6d 696e 6720 6c61 6e67  programming lang
+00000670: 7561 6765 2a2a 2e0a 6063 6f6e 6461 6020  uage**..`conda` 
+00000680: 6973 2061 6e20 6f70 656e 2d73 6f75 7263  is an open-sourc
+00000690: 6520 7061 636b 6167 6520 6d61 6e61 6765  e package manage
+000006a0: 6d65 6e74 2073 7973 7465 6d20 616e 6420  ment system and 
+000006b0: 656e 7669 726f 6e6d 656e 7420 6d61 6e61  environment mana
+000006c0: 6765 6d65 6e74 2073 7973 7465 6d20 7468  gement system th
+000006d0: 6174 2063 616e 2069 6e73 7461 6c6c 2061  at can install a
+000006e0: 6e64 206d 616e 6167 6520 6d75 6c74 6970  nd manage multip
+000006f0: 6c65 2076 6572 7369 6f6e 7320 6f66 2073  le versions of s
+00000700: 6f66 7477 6172 6520 7061 636b 6167 6573  oftware packages
+00000710: 2061 6e64 2074 6865 6972 2064 6570 656e   and their depen
+00000720: 6465 6e63 6965 732e 0a60 636f 6e64 6160  dencies..`conda`
+00000730: 2069 7320 7772 6974 7465 6e20 696e 2050   is written in P
+00000740: 7974 686f 6e2e 0a54 6865 2061 696d 206f  ython..The aim o
+00000750: 6620 5261 7474 6c65 7220 6973 2074 6f20  f Rattler is to 
+00000760: 7072 6f76 6964 6520 616c 6c20 6675 6e63  provide all func
+00000770: 7469 6f6e 616c 6974 7920 7265 7175 6972  tionality requir
+00000780: 6564 2074 6f20 776f 726b 2077 6974 6820  ed to work with 
+00000790: 7468 6520 636f 6e64 6120 6563 6f73 7973  the conda ecosys
+000007a0: 7465 6d20 6672 6f6d 2052 7573 742e 0a52  tem from Rust..R
+000007b0: 6174 746c 6572 2069 7320 6e6f 7420 6120  attler is not a 
+000007c0: 7265 696d 706c 656d 656e 7461 7469 6f6e  reimplementation
+000007d0: 206f 6620 6063 6f6e 6461 602e 0a60 636f   of `conda`..`co
+000007e0: 6e64 6160 2069 7320 6120 7061 636b 6167  nda` is a packag
+000007f0: 6520 6d61 6e61 6765 6d65 6e74 2074 6f6f  e management too
+00000800: 6c2e 0a52 6174 746c 6572 2069 7320 6120  l..Rattler is a 
+00000810: 5f6c 6962 7261 7279 5f20 746f 2077 6f72  _library_ to wor
+00000820: 6b20 7769 7468 2074 6865 2063 6f6e 6461  k with the conda
+00000830: 2065 636f 7379 7374 656d 2066 726f 6d20   ecosystem from 
+00000840: 6469 6666 6572 656e 7420 6c61 6e67 7561  different langua
+00000850: 6765 7320 616e 6420 6170 706c 6963 6174  ges and applicat
+00000860: 696f 6e73 2e0a 466f 7220 6578 616d 706c  ions..For exampl
+00000870: 652c 2069 7420 706f 7765 7273 2074 6865  e, it powers the
+00000880: 2062 6163 6b65 6e64 206f 6620 6874 7470   backend of http
+00000890: 733a 2f2f 7072 6566 6978 2e64 6576 2e0a  s://prefix.dev..
+000008a0: 0a60 636f 6e64 612d 666f 7267 6560 2069  .`conda-forge` i
+000008b0: 7320 6120 636f 6d6d 756e 6974 792d 6472  s a community-dr
+000008c0: 6976 656e 2065 6666 6f72 7420 746f 2062  iven effort to b
+000008d0: 7269 6e67 206e 6577 2061 6e64 2065 7869  ring new and exi
+000008e0: 7374 696e 6720 736f 6674 7761 7265 2069  sting software i
+000008f0: 6e74 6f20 7468 6520 636f 6e64 6120 6563  nto the conda ec
+00000900: 6f73 7973 7465 6d2e 0a49 7420 7072 6f76  osystem..It prov
+00000910: 6964 6573 205f 7465 6e73 2d6f 662d 7468  ides _tens-of-th
+00000920: 6f75 7361 6e64 7320 6f66 2075 702d 746f  ousands of up-to
+00000930: 2d64 6174 655f 2070 6163 6b61 6765 7320  -date_ packages 
+00000940: 7468 6174 2061 7265 206d 6169 6e74 6169  that are maintai
+00000950: 6e65 6420 6279 2061 2063 6f6d 6d75 6e69  ned by a communi
+00000960: 7479 206f 6620 636f 6e74 7269 6275 746f  ty of contributo
+00000970: 7273 2e0a 466f 7220 616e 206f 7665 7276  rs..For an overv
+00000980: 6965 7720 6f66 2061 7661 696c 6162 6c65  iew of available
+00000990: 2070 6163 6b61 6765 7320 7365 6520 6874   packages see ht
+000009a0: 7470 733a 2f2f 7072 6566 6978 2e64 6576  tps://prefix.dev
+000009b0: 2e0a 0a23 2320 486f 7720 7368 6f75 6c64  ...## How should
+000009c0: 2049 2075 7365 2074 6865 2064 6f63 756d   I use the docum
+000009d0: 656e 7461 7469 6f6e 3f0a 0a49 6620 796f  entation?..If yo
+000009e0: 7520 6172 6520 6765 7474 696e 6720 7374  u are getting st
+000009f0: 6172 7465 6420 7769 7468 2074 6865 206c  arted with the l
+00000a00: 6962 7261 7279 2c20 796f 7520 7368 6f75  ibrary, you shou
+00000a10: 6c64 2066 6f6c 6c6f 7720 7468 6520 2746  ld follow the 'F
+00000a20: 6972 7374 2053 7465 7073 2720 7365 6374  irst Steps' sect
+00000a30: 696f 6e20 696e 206f 7264 6572 2e0a 596f  ion in order..Yo
+00000a40: 7520 6361 6e20 616c 736f 2075 7365 2074  u can also use t
+00000a50: 6865 206d 656e 7520 6f6e 2074 6865 206c  he menu on the l
+00000a60: 6566 7420 746f 2071 7569 636b 6c79 2073  eft to quickly s
+00000a70: 6b69 7020 6f76 6572 2073 6563 7469 6f6e  kip over section
+00000a80: 7320 616e 6420 7365 6172 6368 2066 6f72  s and search for
+00000a90: 2073 7065 6369 6669 6320 7468 696e 6773   specific things
+00000aa0: 2e0a 0a23 2320 496e 7374 616c 6c61 7469  ...## Installati
+00000ab0: 6f6e 0a0a 5079 2d52 6174 746c 6572 2069  on..Py-Rattler i
+00000ac0: 7320 6120 7079 7468 6f6e 206c 6962 7261  s a python libra
+00000ad0: 7279 2c20 7768 6963 6820 6d65 616e 7320  ry, which means 
+00000ae0: 796f 7520 6e65 6564 2074 6f20 646f 776e  you need to down
+00000af0: 6c6f 6164 2061 6e64 2069 6e73 7461 6c6c  load and install
+00000b00: 2050 7974 686f 6e20 6672 6f6d 2068 7474   Python from htt
+00000b10: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+00000b20: 6f72 672f 646f 776e 6c6f 6164 730a 6966  org/downloads.if
+00000b30: 2079 6f75 2068 6176 656e 2774 2061 6c72   you haven't alr
+00000b40: 6561 6479 2e20 416c 7465 726e 6174 6976  eady. Alternativ
+00000b50: 656c 792c 2079 6f75 2063 616e 2075 7365  ely, you can use
+00000b60: 2063 616e 2067 6574 2076 6961 2063 6f6e   can get via con
+00000b70: 6461 2e0a 0a23 2323 2050 7970 690a 0a60  da...### Pypi..`
+00000b80: 6060 7368 656c 6c0a 2420 7079 7468 6f6e  ``shell.$ python
+00000b90: 3320 2d6d 2070 6970 2069 6e73 7461 6c6c  3 -m pip install
+00000ba0: 202d 2d75 7067 7261 6465 2070 792d 7261   --upgrade py-ra
+00000bb0: 7474 6c65 720a 6060 600a 0a23 2323 2050  ttler.```..### P
+00000bc0: 6978 690a 0a60 6060 7368 656c 6c0a 2420  ixi..```shell.$ 
+00000bd0: 7069 7869 2061 6464 2070 792d 7261 7474  pixi add py-ratt
+00000be0: 6c65 720a 6060 600a 0a23 2323 2043 6f6e  ler.```..### Con
+00000bf0: 6461 0a0a 6060 6073 6865 6c6c 0a24 2063  da..```shell.$ c
+00000c00: 6f6e 6461 2069 6e73 7461 6c6c 2070 792d  onda install py-
+00000c10: 7261 7474 6c65 720a 6060 600a 0a23 2323  rattler.```..###
+00000c20: 204d 616d 6261 0a0a 6060 6073 6865 6c6c   Mamba..```shell
+00000c30: 0a24 206d 616d 6261 2069 6e73 7461 6c6c  .$ mamba install
+00000c40: 2070 792d 7261 7474 6c65 7220 2d63 2063   py-rattler -c c
+00000c50: 6f6e 6461 2d66 6f72 6765 0a60 6060 0a0a  onda-forge.```..
+00000c60: 2323 204e 6578 7420 5374 6570 730a 0a54  ## Next Steps..T
+00000c70: 6865 7365 2062 6173 6963 2066 6972 7374  hese basic first
+00000c80: 2073 7465 7073 2073 686f 756c 6420 6861   steps should ha
+00000c90: 7665 2067 6f74 7465 6e20 796f 7520 7374  ve gotten you st
+00000ca0: 6172 7465 6420 7769 7468 2074 6865 206c  arted with the l
+00000cb0: 6962 7261 7279 2e0a 0a42 7920 6e6f 772c  ibrary...By now,
+00000cc0: 2079 6f75 2073 686f 756c 6420 6b6e 6f77   you should know
+00000cd0: 2068 6f77 2074 6f20 646f 776e 6c6f 6164   how to download
+00000ce0: 2072 6570 6f20 6461 7461 2c20 736f 6c76   repo data, solv
+00000cf0: 6520 6465 7065 6e64 656e 6369 6573 2061  e dependencies a
+00000d00: 6e64 2063 7265 6174 6520 616e 0a65 6e76  nd create an.env
+00000d10: 6972 6f6e 6d65 6e74 2e0a 0a4e 6578 742c  ironment...Next,
+00000d20: 2077 6520 7769 6c6c 2073 6565 2061 2071   we will see a q
+00000d30: 7569 636b 2072 6566 6572 656e 6365 2073  uick reference s
+00000d40: 756d 6d61 7279 206f 6620 616c 6c20 7468  ummary of all th
+00000d50: 6520 6d65 7468 6f64 7320 616e 6420 7072  e methods and pr
+00000d60: 6f70 6572 7469 6573 2074 6861 7420 796f  operties that yo
+00000d70: 7520 7769 6c6c 206e 6565 6420 7768 656e  u will need when
+00000d80: 2075 7369 6e67 2074 6865 206c 6962 7261   using the libra
+00000d90: 7279 2e20 4966 2079 6f75 2066 6f6c 6c6f  ry. If you follo
+00000da0: 7720 7468 6520 6c69 6e6b 7320 7468 6572  w the links ther
+00000db0: 652c 2079 6f75 2077 696c 6c20 6578 7061  e, you will expa
+00000dc0: 6e64 2074 6865 2064 6f63 756d 656e 7461  nd the documenta
+00000dd0: 7469 6f6e 2066 6f72 2074 6865 206d 6574  tion for the met
+00000de0: 686f 6420 616e 6420 7072 6f70 6572 7479  hod and property
+00000df0: 2c20 7769 7468 206d 6f72 6520 6578 616d  , with more exam
+00000e00: 706c 6573 206f 6e20 686f 7720 746f 2075  ples on how to u
+00000e10: 7365 2074 6865 6d2e 0a0a 2323 2043 6f6e  se them...## Con
+00000e20: 7472 6962 7574 696e 6720 f09f 988d 0a0a  tributing ......
+00000e30: 5765 2077 6f75 6c64 206c 6f76 6520 746f  We would love to
+00000e40: 2068 6176 6520 796f 7520 636f 6e74 7269   have you contri
+00000e50: 6275 7465 210a 5365 6520 7468 6520 434f  bute!.See the CO
+00000e60: 4e54 5249 4255 5449 4f4e 2e6d 6420 666f  NTRIBUTION.md fo
+00000e70: 7220 6d6f 7265 2069 6e66 6f2e 2046 6f72  r more info. For
+00000e80: 2071 7565 7374 696f 6e73 2c20 7265 7175   questions, requ
+00000e90: 6573 7473 206f 7220 6120 6361 7375 616c  ests or a casual
+00000ea0: 2063 6861 742c 2077 6520 6172 6520 7665   chat, we are ve
+00000eb0: 7279 2061 6374 6976 6520 6f6e 206f 7572  ry active on our
+00000ec0: 205b 6469 7363 6f72 6420 7365 7276 6572   [discord server
+00000ed0: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
+00000ee0: 642e 6767 2f6b 4b56 385a 7879 7a59 3429  d.gg/kKV8ZxyzY4)
+00000ef0: 2e0a                                     ..
```

### Comparing `py_rattler-0.6.1/docs/stylesheets/extra.css` & `py_rattler-0.6.2/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/mkdocs.yml` & `py_rattler-0.6.2/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -80,22 +80,23 @@
           class: mermaid
   - pymdownx.tabbed:
       alternate_style: true
   - toc:
       toc_depth: 3
       permalink: "#"
   - mdx_truly_sane_lists
+  - pymdownx.snippets
 
 nav:
   - First Steps: index.md
   - References:
       - core:
           - fetch: fetch_repo_data.md
           - solve: solver.md
-          - install: install.md
+          - install: installer.md
       - channel:
           - ChannelConfig: channel_config.md
           - Channel: channel.md
       - lock:
           - LockFile: lock_file.md
           - Environment: environment.md
           - LockedPackage: locked_package.md
```

### Comparing `py_rattler-0.6.1/pixi.lock` & `py_rattler-0.6.2/pixi.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,117 +1,9 @@
-version: 4
+version: 5
 environments:
-  build:
-    channels:
-    - url: https://conda.anaconda.org/conda-forge/
-    packages:
-      linux-64:
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/binutils_impl_linux-64-2.40-ha885e6a_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/gcc_impl_linux-64-13.2.0-h9eb54c0_6.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/kernel-headers_linux-64-2.6.32-he073ed8_17.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/libgcc-devel_linux-64-13.2.0-hceb6213_106.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsanitizer-13.2.0-h6ddb7a1_6.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/maturin-1.2.3-py38hcdda232_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/patchelf-0.17.2-h58526e2_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.8.19-hd12c33a_0_cpython.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-4_cp38.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/rust-1.77.2-h70c747d_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-unknown-linux-gnu-1.77.2-h2c6d0dc_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/sysroot_linux-64-2.12-he073ed8_17.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
-      osx-64:
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/maturin-1.2.3-py38h196e9ca_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.8.19-h5ba8234_0_cpython.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-4_cp38.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/rust-1.77.2-h7e1429e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-apple-darwin-1.77.2-h38e4360_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
-      osx-arm64:
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/maturin-1.2.3-py38h92a0862_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.8.19-h2469fbe_0_cpython.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.8-4_cp38.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/rust-1.77.2-h4ff7c5d_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-aarch64-apple-darwin-1.77.2-hf6ec828_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
-      win-64:
-      - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-core-5.3.0-7.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/maturin-1.2.3-py38hf90c7e5_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.8.19-h4de0772_0_cpython.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-4_cp38.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/rust-1.77.2-hf8d6059_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-pc-windows-msvc-1.77.2-h17fc481_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
   default:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
     packages: {}
   docs:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
@@ -531,14 +423,16 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
   test:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
+    indexes:
+    - https://pypi.org/simple
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/binutils_impl_linux-64-2.40-ha885e6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
@@ -581,14 +475,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sysroot_linux-64-2.12-he073ed8_17.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/98/5d/5738903efe0ecb73e51eb44feafba32bdba2081263d40c5043568ff60faf/numpy-1.24.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/98/ab/3c2794cf8ce4daa7f451008e5b8a9880a7ff8357ddb383e9de4f35034842/types_networkx-3.2.1.20240531-py3-none-any.whl
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
@@ -615,14 +511,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-apple-darwin-1.77.2-h38e4360_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/11/10/943cfb579f1a02909ff96464c69893b1d25be3731b5d3652c2e0cf1281ea/numpy-1.24.4-cp38-cp38-macosx_10_9_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/98/ab/3c2794cf8ce4daa7f451008e5b8a9880a7ff8357ddb383e9de4f35034842/types_networkx-3.2.1.20240531-py3-none-any.whl
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
@@ -649,14 +547,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-aarch64-apple-darwin-1.77.2-hf6ec828_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/a7/ae/f53b7b265fdc701e663fbb322a8e9d4b14d9cb7b2385f45ddfabfc4327e4/numpy-1.24.4-cp38-cp38-macosx_11_0_arm64.whl
+      - pypi: https://files.pythonhosted.org/packages/98/ab/3c2794cf8ce4daa7f451008e5b8a9880a7ff8357ddb383e9de4f35034842/types_networkx-3.2.1.20240531-py3-none-any.whl
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
@@ -690,27 +590,60 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/69/65/0d47953afa0ad569d12de5f65d964321c208492064c38fe3b0b9744f8d44/numpy-1.24.4-cp38-cp38-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/98/ab/3c2794cf8ce4daa7f451008e5b8a9880a7ff8357ddb383e9de4f35034842/types_networkx-3.2.1.20240531-py3-none-any.whl
 packages:
 - kind: conda
   name: _libgcc_mutex
   version: '0.1'
   build: conda_forge
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
   sha256: fe51de6107f9edc7aa4f786a70f4a883943bc9d39b3bb7307c04c41410990726
   md5: d7c89558ba9fa0495403155b64376d81
   license: None
+  purls: []
   size: 2562
   timestamp: 1578324546067
 - kind: conda
+  name: _libgcc_mutex
+  version: '0.1'
+  build: conda_forge
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
+  sha256: fe51de6107f9edc7aa4f786a70f4a883943bc9d39b3bb7307c04c41410990726
+  md5: d7c89558ba9fa0495403155b64376d81
+  license: None
+  size: 2562
+  timestamp: 1578324546067
+- kind: conda
+  name: _openmp_mutex
+  version: '4.5'
+  build: 2_gnu
+  build_number: 16
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+  sha256: fbe2c5e56a653bebb982eda4876a9178aedfc2b545f25d0ce9c4c0b508253d22
+  md5: 73aaf86a425cc6e73fcf236a5a46396d
+  depends:
+  - _libgcc_mutex 0.1 conda_forge
+  - libgomp >=7.5.0
+  constrains:
+  - openmp_impl 9999
+  license: BSD-3-Clause
+  license_family: BSD
+  purls: []
+  size: 23621
+  timestamp: 1650670423406
+- kind: conda
   name: _openmp_mutex
   version: '4.5'
   build: 2_gnu
   build_number: 16
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
   sha256: fbe2c5e56a653bebb982eda4876a9178aedfc2b545f25d0ce9c4c0b508253d22
@@ -765,14 +698,15 @@
   sha256: 180b268f207d1481beb9de5c173751d14c429a7226fa9a85941e4a54cf6be1b4
   md5: 800a4c872b5bc06fa83888d112fe6c4f
   depends:
   - ld_impl_linux-64 2.40 h55db66e_0
   - sysroot_linux-64
   license: GPL-3.0-only
   license_family: GPL
+  purls: []
   size: 5797310
   timestamp: 1713651250214
 - kind: conda
   name: brotli-python
   version: 1.1.0
   build: py312h30efb56_1
   build_number: 1
@@ -858,27 +792,55 @@
   build_number: 5
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
   sha256: 61fb2b488928a54d9472113e1280b468a309561caa54f33825a3593da390b242
   md5: 6097a6ca9ada32699b5fc4312dd6ef18
   license: bzip2-1.0.6
   license_family: BSD
+  purls: []
+  size: 127885
+  timestamp: 1699280178474
+- kind: conda
+  name: bzip2
+  version: 1.0.8
+  build: h10d778d_5
+  build_number: 5
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
+  sha256: 61fb2b488928a54d9472113e1280b468a309561caa54f33825a3593da390b242
+  md5: 6097a6ca9ada32699b5fc4312dd6ef18
+  license: bzip2-1.0.6
+  license_family: BSD
   size: 127885
   timestamp: 1699280178474
 - kind: conda
   name: bzip2
   version: 1.0.8
   build: h93a5062_5
   build_number: 5
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
   sha256: bfa84296a638bea78a8bb29abc493ee95f2a0218775642474a840411b950fe5f
   md5: 1bbc659ca658bfd49a481b5ef7a0f40f
   license: bzip2-1.0.6
   license_family: BSD
+  purls: []
+  size: 122325
+  timestamp: 1699280294368
+- kind: conda
+  name: bzip2
+  version: 1.0.8
+  build: h93a5062_5
+  build_number: 5
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
+  sha256: bfa84296a638bea78a8bb29abc493ee95f2a0218775642474a840411b950fe5f
+  md5: 1bbc659ca658bfd49a481b5ef7a0f40f
+  license: bzip2-1.0.6
+  license_family: BSD
   size: 122325
   timestamp: 1699280294368
 - kind: conda
   name: bzip2
   version: 1.0.8
   build: hcfcfb64_5
   build_number: 5
@@ -888,14 +850,32 @@
   md5: 26eb8ca6ea332b675e11704cce84a3be
   depends:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: bzip2-1.0.6
   license_family: BSD
+  purls: []
+  size: 124580
+  timestamp: 1699280668742
+- kind: conda
+  name: bzip2
+  version: 1.0.8
+  build: hcfcfb64_5
+  build_number: 5
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
+  sha256: ae5f47a5c86fd6db822931255dcf017eb12f60c77f07dc782ccb477f7808aab2
+  md5: 26eb8ca6ea332b675e11704cce84a3be
+  depends:
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: bzip2-1.0.6
+  license_family: BSD
   size: 124580
   timestamp: 1699280668742
 - kind: conda
   name: bzip2
   version: 1.0.8
   build: hd590300_5
   build_number: 5
@@ -903,17 +883,45 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
   sha256: 242c0c324507ee172c0e0dd2045814e746bb303d1eb78870d182ceb0abc726a8
   md5: 69b8b6202a07720f448be700e300ccf4
   depends:
   - libgcc-ng >=12
   license: bzip2-1.0.6
   license_family: BSD
+  purls: []
   size: 254228
   timestamp: 1699279927352
 - kind: conda
+  name: bzip2
+  version: 1.0.8
+  build: hd590300_5
+  build_number: 5
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
+  sha256: 242c0c324507ee172c0e0dd2045814e746bb303d1eb78870d182ceb0abc726a8
+  md5: 69b8b6202a07720f448be700e300ccf4
+  depends:
+  - libgcc-ng >=12
+  license: bzip2-1.0.6
+  license_family: BSD
+  size: 254228
+  timestamp: 1699279927352
+- kind: conda
+  name: ca-certificates
+  version: 2024.2.2
+  build: h56e8100_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
+  sha256: 4d587088ecccd393fec3420b64f1af4ee1a0e6897a45cfd5ef38055322cea5d0
+  md5: 63da060240ab8087b60d1357051ea7d6
+  license: ISC
+  purls: []
+  size: 155886
+  timestamp: 1706843918052
+- kind: conda
   name: ca-certificates
   version: 2024.2.2
   build: h56e8100_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
   sha256: 4d587088ecccd393fec3420b64f1af4ee1a0e6897a45cfd5ef38055322cea5d0
   md5: 63da060240ab8087b60d1357051ea7d6
@@ -925,30 +933,66 @@
   version: 2024.2.2
   build: h8857fd0_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
   sha256: 54a794aedbb4796afeabdf54287b06b1d27f7b13b3814520925f4c2c80f58ca9
   md5: f2eacee8c33c43692f1ccfd33d0f50b1
   license: ISC
+  purls: []
+  size: 155665
+  timestamp: 1706843838227
+- kind: conda
+  name: ca-certificates
+  version: 2024.2.2
+  build: h8857fd0_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
+  sha256: 54a794aedbb4796afeabdf54287b06b1d27f7b13b3814520925f4c2c80f58ca9
+  md5: f2eacee8c33c43692f1ccfd33d0f50b1
+  license: ISC
   size: 155665
   timestamp: 1706843838227
 - kind: conda
   name: ca-certificates
   version: 2024.2.2
   build: hbcca054_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
   sha256: 91d81bfecdbb142c15066df70cc952590ae8991670198f92c66b62019b251aeb
   md5: 2f4327a1cbe7f022401b236e915a5fef
   license: ISC
+  purls: []
   size: 155432
   timestamp: 1706843687645
 - kind: conda
   name: ca-certificates
   version: 2024.2.2
+  build: hbcca054_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
+  sha256: 91d81bfecdbb142c15066df70cc952590ae8991670198f92c66b62019b251aeb
+  md5: 2f4327a1cbe7f022401b236e915a5fef
+  license: ISC
+  size: 155432
+  timestamp: 1706843687645
+- kind: conda
+  name: ca-certificates
+  version: 2024.2.2
+  build: hf0a4a13_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
+  sha256: 49bc3439816ac72d0c0e0f144b8cc870fdcc4adec2e861407ec818d8116b2204
+  md5: fb416a1795f18dcc5a038bc2dc54edf9
+  license: ISC
+  purls: []
+  size: 155725
+  timestamp: 1706844034242
+- kind: conda
+  name: ca-certificates
+  version: 2024.2.2
   build: hf0a4a13_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
   sha256: 49bc3439816ac72d0c0e0f144b8cc870fdcc4adec2e861407ec818d8116b2204
   md5: fb416a1795f18dcc5a038bc2dc54edf9
   license: ISC
   size: 155725
@@ -1232,14 +1276,31 @@
   url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
   sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
   md5: 3faab06a954c2a04039983f2c4a50d99
   depends:
   - python >=3.7
   license: BSD-3-Clause
   license_family: BSD
+  purls:
+  - pkg:pypi/colorama?source=conda-forge-mapping
+  size: 25170
+  timestamp: 1666700778190
+- kind: conda
+  name: colorama
+  version: 0.4.6
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+  sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
+  md5: 3faab06a954c2a04039983f2c4a50d99
+  depends:
+  - python >=3.7
+  license: BSD-3-Clause
+  license_family: BSD
   size: 25170
   timestamp: 1666700778190
 - kind: conda
   name: cssselect2
   version: 0.2.1
   build: pyh9f0ad1d_1
   build_number: 1
@@ -1279,14 +1340,16 @@
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
   sha256: a6ae416383bda0e3ed14eaa187c653e22bec94ff2aa3b56970cdf0032761e80d
   md5: 8d652ea2ee8eaee02ed8dc820bc794aa
   depends:
   - python >=3.7
   license: MIT and PSF-2.0
+  purls:
+  - pkg:pypi/exceptiongroup?source=conda-forge-mapping
   size: 20551
   timestamp: 1704921321122
 - kind: conda
   name: expat
   version: 2.6.2
   build: h59595ed_0
   subdir: linux-64
@@ -1577,14 +1640,15 @@
   - libgcc-ng >=13.2.0
   - libgomp >=13.2.0
   - libsanitizer 13.2.0 h6ddb7a1_6
   - libstdcxx-ng >=13.2.0
   - sysroot_linux-64
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
+  purls: []
   size: 53360656
   timestamp: 1714581875812
 - kind: conda
   name: ghp-import
   version: 2.1.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -1710,14 +1774,16 @@
   url: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
   sha256: 38740c939b668b36a50ef455b077e8015b8c9cf89860d421b3fff86048f49666
   md5: f800d2da156d08e289b14e87e43c1ae5
   depends:
   - python >=3.7
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/iniconfig?source=conda-forge-mapping
   size: 11101
   timestamp: 1673103208955
 - kind: conda
   name: jinja2
   version: 3.1.3
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -1742,14 +1808,15 @@
   url: https://conda.anaconda.org/conda-forge/noarch/kernel-headers_linux-64-2.6.32-he073ed8_17.conda
   sha256: fb39d64b48f3d9d1acc3df208911a41f25b6a00bd54935d5973b4739a9edd5b6
   md5: d731b543793afc0433c4fd593e693fce
   constrains:
   - sysroot_linux-64 ==2.12
   license: LGPL-2.0-or-later AND LGPL-2.0-or-later WITH exceptions AND GPL-2.0-or-later AND MPL-2.0
   license_family: GPL
+  purls: []
   size: 710627
   timestamp: 1708000830116
 - kind: conda
   name: lcms2
   version: '2.16'
   build: h67d730c_0
   subdir: win-64
@@ -1820,14 +1887,29 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
   sha256: ef969eee228cfb71e55146eaecc6af065f468cb0bc0a5239bc053b39db0b5f09
   md5: 10569984e7db886e4f1abc2b47ad79a1
   constrains:
   - binutils_impl_linux-64 2.40
   license: GPL-3.0-only
   license_family: GPL
+  purls: []
+  size: 713322
+  timestamp: 1713651222435
+- kind: conda
+  name: ld_impl_linux-64
+  version: '2.40'
+  build: h55db66e_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
+  sha256: ef969eee228cfb71e55146eaecc6af065f468cb0bc0a5239bc053b39db0b5f09
+  md5: 10569984e7db886e4f1abc2b47ad79a1
+  constrains:
+  - binutils_impl_linux-64 2.40
+  license: GPL-3.0-only
+  license_family: GPL
   size: 713322
   timestamp: 1713651222435
 - kind: conda
   name: lerc
   version: 4.0.0
   build: h27087fc_0
   subdir: linux-64
@@ -1890,26 +1972,52 @@
   build: h4653b0c_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
   sha256: 11d3fb51c14832d9e4f6d84080a375dec21ea8a3a381a1910e67ff9cedc20355
   md5: 9d7d724faf0413bf1dbc5a85935700c8
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
+  purls: []
+  size: 1160232
+  timestamp: 1686896993785
+- kind: conda
+  name: libcxx
+  version: 16.0.6
+  build: h4653b0c_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
+  sha256: 11d3fb51c14832d9e4f6d84080a375dec21ea8a3a381a1910e67ff9cedc20355
+  md5: 9d7d724faf0413bf1dbc5a85935700c8
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
   size: 1160232
   timestamp: 1686896993785
 - kind: conda
   name: libcxx
   version: 16.0.6
   build: hd57cbcb_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
   sha256: 9063271847cf05f3a6cc6cae3e7f0ced032ab5f3a3c9d3f943f876f39c5c2549
   md5: 7d6972792161077908b62971802f289a
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
+  purls: []
+  size: 1142172
+  timestamp: 1686896907750
+- kind: conda
+  name: libcxx
+  version: 16.0.6
+  build: hd57cbcb_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
+  sha256: 9063271847cf05f3a6cc6cae3e7f0ced032ab5f3a3c9d3f943f876f39c5c2549
+  md5: 7d6972792161077908b62971802f289a
+  license: Apache-2.0 WITH LLVM-exception
+  license_family: Apache
   size: 1142172
   timestamp: 1686896907750
 - kind: conda
   name: libdeflate
   version: '1.20'
   build: h49d49c5_0
   subdir: osx-64
@@ -2027,27 +2135,55 @@
   build_number: 5
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
   sha256: 7a2d27a936ceee6942ea4d397f9c7d136f12549d86f7617e8b6bad51e01a941f
   md5: ccb34fb14960ad8b125962d3d79b31a9
   license: MIT
   license_family: MIT
+  purls: []
+  size: 51348
+  timestamp: 1636488394370
+- kind: conda
+  name: libffi
+  version: 3.4.2
+  build: h0d85af4_5
+  build_number: 5
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
+  sha256: 7a2d27a936ceee6942ea4d397f9c7d136f12549d86f7617e8b6bad51e01a941f
+  md5: ccb34fb14960ad8b125962d3d79b31a9
+  license: MIT
+  license_family: MIT
   size: 51348
   timestamp: 1636488394370
 - kind: conda
   name: libffi
   version: 3.4.2
   build: h3422bc3_5
   build_number: 5
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
   sha256: 41b3d13efb775e340e4dba549ab5c029611ea6918703096b2eaa9c015c0750ca
   md5: 086914b672be056eb70fd4285b6783b6
   license: MIT
   license_family: MIT
+  purls: []
+  size: 39020
+  timestamp: 1636488587153
+- kind: conda
+  name: libffi
+  version: 3.4.2
+  build: h3422bc3_5
+  build_number: 5
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
+  sha256: 41b3d13efb775e340e4dba549ab5c029611ea6918703096b2eaa9c015c0750ca
+  md5: 086914b672be056eb70fd4285b6783b6
+  license: MIT
+  license_family: MIT
   size: 39020
   timestamp: 1636488587153
 - kind: conda
   name: libffi
   version: 3.4.2
   build: h7f98852_5
   build_number: 5
@@ -2055,19 +2191,52 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
   sha256: ab6e9856c21709b7b517e940ae7028ae0737546122f83c2aa5d692860c3b149e
   md5: d645c6d2ac96843a2bfaccd2d62b3ac3
   depends:
   - libgcc-ng >=9.4.0
   license: MIT
   license_family: MIT
+  purls: []
   size: 58292
   timestamp: 1636488182923
 - kind: conda
   name: libffi
   version: 3.4.2
+  build: h7f98852_5
+  build_number: 5
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+  sha256: ab6e9856c21709b7b517e940ae7028ae0737546122f83c2aa5d692860c3b149e
+  md5: d645c6d2ac96843a2bfaccd2d62b3ac3
+  depends:
+  - libgcc-ng >=9.4.0
+  license: MIT
+  license_family: MIT
+  size: 58292
+  timestamp: 1636488182923
+- kind: conda
+  name: libffi
+  version: 3.4.2
+  build: h8ffe710_5
+  build_number: 5
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
+  sha256: 1951ab740f80660e9bc07d2ed3aefb874d78c107264fd810f24a1a6211d4b1a5
+  md5: 2c96d1b6915b408893f9472569dee135
+  depends:
+  - vc >=14.1,<15.0a0
+  - vs2015_runtime >=14.16.27012
+  license: MIT
+  license_family: MIT
+  purls: []
+  size: 42063
+  timestamp: 1636489106777
+- kind: conda
+  name: libffi
+  version: 3.4.2
   build: h8ffe710_5
   build_number: 5
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
   sha256: 1951ab740f80660e9bc07d2ed3aefb874d78c107264fd810f24a1a6211d4b1a5
   md5: 2c96d1b6915b408893f9472569dee135
   depends:
@@ -2085,14 +2254,15 @@
   subdir: noarch
   noarch: generic
   url: https://conda.anaconda.org/conda-forge/noarch/libgcc-devel_linux-64-13.2.0-hceb6213_106.conda
   sha256: f5af7a346ba0a2c322028a7fa8ba99f5094911439d5aab2c6bc42a4e9022bc68
   md5: b85d6b583f498b4ddc9150aefb492f7f
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
+  purls: []
   size: 2575829
   timestamp: 1714581666472
 - kind: conda
   name: libgcc-ng
   version: 13.2.0
   build: hc881cc4_6
   build_number: 6
@@ -2103,14 +2273,33 @@
   depends:
   - _libgcc_mutex 0.1 conda_forge
   - _openmp_mutex >=4.5
   constrains:
   - libgomp 13.2.0 hc881cc4_6
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
+  purls: []
+  size: 777315
+  timestamp: 1713755001744
+- kind: conda
+  name: libgcc-ng
+  version: 13.2.0
+  build: hc881cc4_6
+  build_number: 6
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda
+  sha256: 836a0057525f1414de43642d357d0ab21ac7f85e24800b010dbc17d132e6efec
+  md5: df88796bd09a0d2ed292e59101478ad8
+  depends:
+  - _libgcc_mutex 0.1 conda_forge
+  - _openmp_mutex >=4.5
+  constrains:
+  - libgomp 13.2.0 hc881cc4_6
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
   size: 777315
   timestamp: 1713755001744
 - kind: conda
   name: libglib
   version: 2.80.0
   build: h39d0aa6_6
   build_number: 6
@@ -2201,14 +2390,30 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda
   sha256: e722b19b23b31a14b1592d5eceabb38dc52452ff5e4d346e330526971c22e52a
   md5: aae89d3736661c36a5591788aebd0817
   depends:
   - _libgcc_mutex 0.1 conda_forge
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
+  purls: []
+  size: 422363
+  timestamp: 1713754915251
+- kind: conda
+  name: libgomp
+  version: 13.2.0
+  build: hc881cc4_6
+  build_number: 6
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda
+  sha256: e722b19b23b31a14b1592d5eceabb38dc52452ff5e4d346e330526971c22e52a
+  md5: aae89d3736661c36a5591788aebd0817
+  depends:
+  - _libgcc_mutex 0.1 conda_forge
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
   size: 422363
   timestamp: 1713754915251
 - kind: conda
   name: libiconv
   version: '1.17'
   build: h0d3ecfb_2
   build_number: 2
@@ -2373,14 +2578,29 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
   sha256: 26d77a3bb4dceeedc2a41bd688564fe71bf2d149fdcf117049970bc02ff1add6
   md5: 30fd6e37fe21f86f4bd26d6ee73eeec7
   depends:
   - libgcc-ng >=12
   license: LGPL-2.1-only
   license_family: GPL
+  purls: []
+  size: 33408
+  timestamp: 1697359010159
+- kind: conda
+  name: libnsl
+  version: 2.0.1
+  build: hd590300_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
+  sha256: 26d77a3bb4dceeedc2a41bd688564fe71bf2d149fdcf117049970bc02ff1add6
+  md5: 30fd6e37fe21f86f4bd26d6ee73eeec7
+  depends:
+  - libgcc-ng >=12
+  license: LGPL-2.1-only
+  license_family: GPL
   size: 33408
   timestamp: 1697359010159
 - kind: conda
   name: libpng
   version: 1.6.43
   build: h091b4b1_0
   subdir: osx-arm64
@@ -2444,59 +2664,119 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libsanitizer-13.2.0-h6ddb7a1_6.conda
   sha256: 06f3695963ee86badbfe006f13fa9fe600539acb77f19c5c972d498a14e9b53d
   md5: 95b48df99634d9e706a0bf7e30ae91c8
   depends:
   - libgcc-ng >=13.2.0
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
+  purls: []
   size: 4188343
   timestamp: 1714581787957
 - kind: conda
   name: libsqlite
   version: 3.45.3
   build: h091b4b1_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
   sha256: 4337f466eb55bbdc74e168b52ec8c38f598e3664244ec7a2536009036e2066cc
   md5: c8c1186c7f3351f6ffddb97b1f54fc58
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: Unlicense
+  purls: []
+  size: 824794
+  timestamp: 1713367748819
+- kind: conda
+  name: libsqlite
+  version: 3.45.3
+  build: h091b4b1_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
+  sha256: 4337f466eb55bbdc74e168b52ec8c38f598e3664244ec7a2536009036e2066cc
+  md5: c8c1186c7f3351f6ffddb97b1f54fc58
+  depends:
+  - libzlib >=1.2.13,<1.3.0a0
+  license: Unlicense
   size: 824794
   timestamp: 1713367748819
 - kind: conda
   name: libsqlite
   version: 3.45.3
   build: h2797004_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
   sha256: e2273d6860eadcf714a759ffb6dc24a69cfd01f2a0ea9d6c20f86049b9334e0c
   md5: b3316cbe90249da4f8e84cd66e1cc55b
   depends:
   - libgcc-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   license: Unlicense
+  purls: []
+  size: 859858
+  timestamp: 1713367435849
+- kind: conda
+  name: libsqlite
+  version: 3.45.3
+  build: h2797004_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
+  sha256: e2273d6860eadcf714a759ffb6dc24a69cfd01f2a0ea9d6c20f86049b9334e0c
+  md5: b3316cbe90249da4f8e84cd66e1cc55b
+  depends:
+  - libgcc-ng >=12
+  - libzlib >=1.2.13,<1.3.0a0
+  license: Unlicense
   size: 859858
   timestamp: 1713367435849
 - kind: conda
   name: libsqlite
   version: 3.45.3
   build: h92b6c6a_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
   sha256: 4d44b68fb29dcbc2216a8cae0b274b02ef9b4ae05d1d0f785362ed30b91c9b52
   md5: 68e462226209f35182ef66eda0f794ff
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: Unlicense
+  purls: []
   size: 902546
   timestamp: 1713367776445
 - kind: conda
   name: libsqlite
   version: 3.45.3
+  build: h92b6c6a_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
+  sha256: 4d44b68fb29dcbc2216a8cae0b274b02ef9b4ae05d1d0f785362ed30b91c9b52
+  md5: 68e462226209f35182ef66eda0f794ff
+  depends:
+  - libzlib >=1.2.13,<1.3.0a0
+  license: Unlicense
+  size: 902546
+  timestamp: 1713367776445
+- kind: conda
+  name: libsqlite
+  version: 3.45.3
+  build: hcfcfb64_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
+  sha256: 06ec75faa51d7ec6d5db98889e869b579a9df19d7d3d9baff8359627da4a3b7e
+  md5: 73f5dc8e2d55d9a1e14b11f49c3b4a28
+  depends:
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: Unlicense
+  purls: []
+  size: 870518
+  timestamp: 1713367888406
+- kind: conda
+  name: libsqlite
+  version: 3.45.3
   build: hcfcfb64_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
   sha256: 06ec75faa51d7ec6d5db98889e869b579a9df19d7d3d9baff8359627da4a3b7e
   md5: 73f5dc8e2d55d9a1e14b11f49c3b4a28
   depends:
   - ucrt >=10.0.20348.0
@@ -2512,14 +2792,28 @@
   build_number: 6
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda
   sha256: 2616dbf9d28431eea20b6e307145c6a92ea0328a047c725ff34b0316de2617da
   md5: 3cfab3e709f77e9f1b3d380eb622494a
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
+  purls: []
+  size: 3842900
+  timestamp: 1713755068572
+- kind: conda
+  name: libstdcxx-ng
+  version: 13.2.0
+  build: h95c4c6d_6
+  build_number: 6
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda
+  sha256: 2616dbf9d28431eea20b6e307145c6a92ea0328a047c725ff34b0316de2617da
+  md5: 3cfab3e709f77e9f1b3d380eb622494a
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
   size: 3842900
   timestamp: 1713755068572
 - kind: conda
   name: libtiff
   version: 4.6.0
   build: h07db509_3
   build_number: 3
@@ -2612,14 +2906,29 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
   sha256: 787eb542f055a2b3de553614b25f09eefb0a0931b0c87dbcce6efdfd92f04f18
   md5: 40b61aab5c7ba9ff276c41cfffe6b80b
   depends:
   - libgcc-ng >=12
   license: BSD-3-Clause
   license_family: BSD
+  purls: []
+  size: 33601
+  timestamp: 1680112270483
+- kind: conda
+  name: libuuid
+  version: 2.38.1
+  build: h0b41bf4_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
+  sha256: 787eb542f055a2b3de553614b25f09eefb0a0931b0c87dbcce6efdfd92f04f18
+  md5: 40b61aab5c7ba9ff276c41cfffe6b80b
+  depends:
+  - libgcc-ng >=12
+  license: BSD-3-Clause
+  license_family: BSD
   size: 33601
   timestamp: 1680112270483
 - kind: conda
   name: libwebp-base
   version: 1.4.0
   build: h10d778d_0
   subdir: osx-64
@@ -2755,14 +3064,29 @@
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
   sha256: 6ae68e0b86423ef188196fff6207ed0c8195dd84273cb5623b85aa08033a410c
   md5: 5aa797f8787fe7a17d1b0821485b5adc
   depends:
   - libgcc-ng >=12
   license: LGPL-2.1-or-later
+  purls: []
+  size: 100393
+  timestamp: 1702724383534
+- kind: conda
+  name: libxcrypt
+  version: 4.4.36
+  build: hd590300_1
+  build_number: 1
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
+  sha256: 6ae68e0b86423ef188196fff6207ed0c8195dd84273cb5623b85aa08033a410c
+  md5: 5aa797f8787fe7a17d1b0821485b5adc
+  depends:
+  - libgcc-ng >=12
+  license: LGPL-2.1-or-later
   size: 100393
   timestamp: 1702724383534
 - kind: conda
   name: libzlib
   version: 1.2.13
   build: h53f4e23_5
   build_number: 5
@@ -2770,19 +3094,51 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
   sha256: ab1c8aefa2d54322a63aaeeefe9cf877411851738616c4068e0dccc66b9c758a
   md5: 1a47f5236db2e06a320ffa0392f81bd8
   constrains:
   - zlib 1.2.13 *_5
   license: Zlib
   license_family: Other
+  purls: []
   size: 48102
   timestamp: 1686575426584
 - kind: conda
   name: libzlib
   version: 1.2.13
+  build: h53f4e23_5
+  build_number: 5
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+  sha256: ab1c8aefa2d54322a63aaeeefe9cf877411851738616c4068e0dccc66b9c758a
+  md5: 1a47f5236db2e06a320ffa0392f81bd8
+  constrains:
+  - zlib 1.2.13 *_5
+  license: Zlib
+  license_family: Other
+  size: 48102
+  timestamp: 1686575426584
+- kind: conda
+  name: libzlib
+  version: 1.2.13
+  build: h8a1eda9_5
+  build_number: 5
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
+  sha256: fc58ad7f47ffea10df1f2165369978fba0a1cc32594aad778f5eec725f334867
+  md5: 4a3ad23f6e16f99c04e166767193d700
+  constrains:
+  - zlib 1.2.13 *_5
+  license: Zlib
+  license_family: Other
+  purls: []
+  size: 59404
+  timestamp: 1686575566695
+- kind: conda
+  name: libzlib
+  version: 1.2.13
   build: h8a1eda9_5
   build_number: 5
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
   sha256: fc58ad7f47ffea10df1f2165369978fba0a1cc32594aad778f5eec725f334867
   md5: 4a3ad23f6e16f99c04e166767193d700
   constrains:
@@ -2804,14 +3160,34 @@
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   constrains:
   - zlib 1.2.13 *_5
   license: Zlib
   license_family: Other
+  purls: []
+  size: 55800
+  timestamp: 1686575452215
+- kind: conda
+  name: libzlib
+  version: 1.2.13
+  build: hcfcfb64_5
+  build_number: 5
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
+  sha256: c161822ee8130b71e08b6d282b9919c1de2c5274b29921a867bca0f7d30cad26
+  md5: 5fdb9c6a113b6b6cb5e517fd972d5f41
+  depends:
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  constrains:
+  - zlib 1.2.13 *_5
+  license: Zlib
+  license_family: Other
   size: 55800
   timestamp: 1686575452215
 - kind: conda
   name: libzlib
   version: 1.2.13
   build: hd590300_5
   build_number: 5
@@ -2821,14 +3197,32 @@
   md5: f36c115f1ee199da648e0597ec2047ad
   depends:
   - libgcc-ng >=12
   constrains:
   - zlib 1.2.13 *_5
   license: Zlib
   license_family: Other
+  purls: []
+  size: 61588
+  timestamp: 1686575217516
+- kind: conda
+  name: libzlib
+  version: 1.2.13
+  build: hd590300_5
+  build_number: 5
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
+  sha256: 370c7c5893b737596fd6ca0d9190c9715d89d888b8c88537ae1ef168c25e82e4
+  md5: f36c115f1ee199da648e0597ec2047ad
+  depends:
+  - libgcc-ng >=12
+  constrains:
+  - zlib 1.2.13 *_5
+  license: Zlib
+  license_family: Other
   size: 61588
   timestamp: 1686575217516
 - kind: conda
   name: m2w64-gcc-libgfortran
   version: 5.3.0
   build: '6'
   build_number: 6
@@ -2836,17 +3230,52 @@
   url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2
   sha256: 9de95a7996d5366ae0808eef2acbc63f9b11b874aa42375f55379e6715845dc6
   md5: 066552ac6b907ec6d72c0ddab29050dc
   depends:
   - m2w64-gcc-libs-core
   - msys2-conda-epoch ==20160418
   license: GPL, LGPL, FDL, custom
+  purls: []
   size: 350687
   timestamp: 1608163451316
 - kind: conda
+  name: m2w64-gcc-libgfortran
+  version: 5.3.0
+  build: '6'
+  build_number: 6
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2
+  sha256: 9de95a7996d5366ae0808eef2acbc63f9b11b874aa42375f55379e6715845dc6
+  md5: 066552ac6b907ec6d72c0ddab29050dc
+  depends:
+  - m2w64-gcc-libs-core
+  - msys2-conda-epoch ==20160418
+  license: GPL, LGPL, FDL, custom
+  size: 350687
+  timestamp: 1608163451316
+- kind: conda
+  name: m2w64-gcc-libs
+  version: 5.3.0
+  build: '7'
+  build_number: 7
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2
+  sha256: 3bd1ab02b7c89a5b153a17be03b36d833f1517ff2a6a77ead7c4a808b88196aa
+  md5: fe759119b8b3bfa720b8762c6fdc35de
+  depends:
+  - m2w64-gcc-libgfortran
+  - m2w64-gcc-libs-core
+  - m2w64-gmp
+  - m2w64-libwinpthread-git
+  - msys2-conda-epoch ==20160418
+  license: GPL3+, partial:GCCRLE, partial:LGPL2+
+  purls: []
+  size: 532390
+  timestamp: 1608163512830
+- kind: conda
   name: m2w64-gcc-libs
   version: 5.3.0
   build: '7'
   build_number: 7
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2
   sha256: 3bd1ab02b7c89a5b153a17be03b36d833f1517ff2a6a77ead7c4a808b88196aa
@@ -2870,31 +3299,78 @@
   sha256: 58afdfe859ed2e9a9b1cc06bc408720cb2c3a6a132e59d4805b090d7574f4ee0
   md5: 4289d80fb4d272f1f3b56cfe87ac90bd
   depends:
   - m2w64-gmp
   - m2w64-libwinpthread-git
   - msys2-conda-epoch ==20160418
   license: GPL3+, partial:GCCRLE, partial:LGPL2+
+  purls: []
+  size: 219240
+  timestamp: 1608163481341
+- kind: conda
+  name: m2w64-gcc-libs-core
+  version: 5.3.0
+  build: '7'
+  build_number: 7
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-core-5.3.0-7.tar.bz2
+  sha256: 58afdfe859ed2e9a9b1cc06bc408720cb2c3a6a132e59d4805b090d7574f4ee0
+  md5: 4289d80fb4d272f1f3b56cfe87ac90bd
+  depends:
+  - m2w64-gmp
+  - m2w64-libwinpthread-git
+  - msys2-conda-epoch ==20160418
+  license: GPL3+, partial:GCCRLE, partial:LGPL2+
   size: 219240
   timestamp: 1608163481341
 - kind: conda
   name: m2w64-gmp
   version: 6.1.0
   build: '2'
   build_number: 2
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2
   sha256: 7e3cd95f554660de45f8323fca359e904e8d203efaf07a4d311e46d611481ed1
   md5: 53a1c73e1e3d185516d7e3af177596d9
   depends:
   - msys2-conda-epoch ==20160418
   license: LGPL3
+  purls: []
   size: 743501
   timestamp: 1608163782057
 - kind: conda
+  name: m2w64-gmp
+  version: 6.1.0
+  build: '2'
+  build_number: 2
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2
+  sha256: 7e3cd95f554660de45f8323fca359e904e8d203efaf07a4d311e46d611481ed1
+  md5: 53a1c73e1e3d185516d7e3af177596d9
+  depends:
+  - msys2-conda-epoch ==20160418
+  license: LGPL3
+  size: 743501
+  timestamp: 1608163782057
+- kind: conda
+  name: m2w64-libwinpthread-git
+  version: 5.0.0.4634.697f757
+  build: '2'
+  build_number: 2
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2
+  sha256: f63a09b2cae7defae0480f1740015d6235f1861afa6fe2e2d3e10bd0d1314ee0
+  md5: 774130a326dee16f1ceb05cc687ee4f0
+  depends:
+  - msys2-conda-epoch ==20160418
+  license: MIT, BSD
+  purls: []
+  size: 31928
+  timestamp: 1608166099896
+- kind: conda
   name: m2w64-libwinpthread-git
   version: 5.0.0.4634.697f757
   build: '2'
   build_number: 2
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2
   sha256: f63a09b2cae7defae0480f1740015d6235f1861afa6fe2e2d3e10bd0d1314ee0
@@ -3005,14 +3481,16 @@
   depends:
   - openssl >=3.1.3,<4.0a0
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/maturin?source=conda-forge-mapping
   size: 4954588
   timestamp: 1695301365076
 - kind: conda
   name: maturin
   version: 1.2.3
   build: py38h92a0862_1
   build_number: 1
@@ -3024,14 +3502,16 @@
   - openssl >=3.1.3,<4.0a0
   - python >=3.8,<3.9.0a0
   - python >=3.8,<3.9.0a0 *_cpython
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/maturin?source=conda-forge-mapping
   size: 4911655
   timestamp: 1695301265510
 - kind: conda
   name: maturin
   version: 1.2.3
   build: py38hcdda232_1
   build_number: 1
@@ -3043,14 +3523,16 @@
   - libgcc-ng >=12
   - openssl >=3.1.3,<4.0a0
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/maturin?source=conda-forge-mapping
   size: 6347816
   timestamp: 1695300476324
 - kind: conda
   name: maturin
   version: 1.2.3
   build: py38hf90c7e5_1
   build_number: 1
@@ -3062,14 +3544,16 @@
   - m2w64-gcc-libs
   - m2w64-gcc-libs-core
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/maturin?source=conda-forge-mapping
   size: 4675089
   timestamp: 1695301899264
 - kind: conda
   name: mdx_truly_sane_lists
   version: '1.3'
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -3239,14 +3723,26 @@
   version: '20160418'
   build: '1'
   build_number: 1
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2
   sha256: 99358d58d778abee4dca82ad29fb58058571f19b0f86138363c260049d4ac7f1
   md5: b0309b72560df66f71a9d5e34a5efdfa
+  purls: []
+  size: 3227
+  timestamp: 1608166968312
+- kind: conda
+  name: msys2-conda-epoch
+  version: '20160418'
+  build: '1'
+  build_number: 1
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2
+  sha256: 99358d58d778abee4dca82ad29fb58058571f19b0f86138363c260049d4ac7f1
+  md5: b0309b72560df66f71a9d5e34a5efdfa
   size: 3227
   timestamp: 1608166968312
 - kind: conda
   name: mypy
   version: 1.5.1
   build: py38h01eb140_1
   build_number: 1
@@ -3260,14 +3756,16 @@
   - psutil >=4.0
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   - typing_extensions >=4.1.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/mypy?source=conda-forge-mapping
   size: 16146866
   timestamp: 1695442675379
 - kind: conda
   name: mypy
   version: 1.5.1
   build: py38h91455d4_1
   build_number: 1
@@ -3283,14 +3781,16 @@
   - tomli >=1.1.0
   - typing_extensions >=4.1.0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/mypy?source=conda-forge-mapping
   size: 8981331
   timestamp: 1695442268532
 - kind: conda
   name: mypy
   version: 1.5.1
   build: py38hb192615_1
   build_number: 1
@@ -3304,14 +3804,16 @@
   - python >=3.8,<3.9.0a0
   - python >=3.8,<3.9.0a0 *_cpython
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   - typing_extensions >=4.1.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/mypy?source=conda-forge-mapping
   size: 8908642
   timestamp: 1695442718816
 - kind: conda
   name: mypy
   version: 1.5.1
   build: py38hcafd530_1
   build_number: 1
@@ -3324,14 +3826,16 @@
   - psutil >=4.0
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   - typing_extensions >=4.1.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/mypy?source=conda-forge-mapping
   size: 11027655
   timestamp: 1695442955398
 - kind: conda
   name: mypy_extensions
   version: 1.0.0
   build: pyha770c72_0
   subdir: noarch
@@ -3339,51 +3843,115 @@
   url: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
   sha256: f240217476e148e825420c6bc3a0c0efb08c0718b7042fae960400c02af858a3
   md5: 4eccaeba205f0aed9ac3a9ea58568ca3
   depends:
   - python >=3.5
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/mypy-extensions?source=conda-forge-mapping
   size: 10492
   timestamp: 1675543414256
 - kind: conda
   name: ncurses
   version: 6.4.20240210
   build: h078ce10_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
   sha256: 06f0905791575e2cd3aa961493c56e490b3d82ad9eb49f1c332bd338b0216911
   md5: 616ae8691e6608527d0071e6766dcb81
   license: X11 AND BSD-3-Clause
+  purls: []
+  size: 820249
+  timestamp: 1710866874348
+- kind: conda
+  name: ncurses
+  version: 6.4.20240210
+  build: h078ce10_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
+  sha256: 06f0905791575e2cd3aa961493c56e490b3d82ad9eb49f1c332bd338b0216911
+  md5: 616ae8691e6608527d0071e6766dcb81
+  license: X11 AND BSD-3-Clause
   size: 820249
   timestamp: 1710866874348
 - kind: conda
   name: ncurses
   version: 6.4.20240210
   build: h59595ed_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
   sha256: aa0f005b6727aac6507317ed490f0904430584fa8ca722657e7f0fb94741de81
   md5: 97da8860a0da5413c7c98a3b3838a645
   depends:
   - libgcc-ng >=12
   license: X11 AND BSD-3-Clause
+  purls: []
+  size: 895669
+  timestamp: 1710866638986
+- kind: conda
+  name: ncurses
+  version: 6.4.20240210
+  build: h59595ed_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
+  sha256: aa0f005b6727aac6507317ed490f0904430584fa8ca722657e7f0fb94741de81
+  md5: 97da8860a0da5413c7c98a3b3838a645
+  depends:
+  - libgcc-ng >=12
+  license: X11 AND BSD-3-Clause
   size: 895669
   timestamp: 1710866638986
 - kind: conda
   name: ncurses
   version: 6.4.20240210
   build: h73e2aa4_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
   sha256: 50b72acf08acbc4e5332807653e2ca6b26d4326e8af16fad1fd3f2ce9ea55503
   md5: 50f28c512e9ad78589e3eab34833f762
   license: X11 AND BSD-3-Clause
+  purls: []
+  size: 823010
+  timestamp: 1710866856626
+- kind: conda
+  name: ncurses
+  version: 6.4.20240210
+  build: h73e2aa4_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
+  sha256: 50b72acf08acbc4e5332807653e2ca6b26d4326e8af16fad1fd3f2ce9ea55503
+  md5: 50f28c512e9ad78589e3eab34833f762
+  license: X11 AND BSD-3-Clause
   size: 823010
   timestamp: 1710866856626
+- kind: pypi
+  name: numpy
+  version: 1.24.4
+  url: https://files.pythonhosted.org/packages/98/5d/5738903efe0ecb73e51eb44feafba32bdba2081263d40c5043568ff60faf/numpy-1.24.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: dd80e219fd4c71fc3699fc1dadac5dcf4fd882bfc6f7ec53d30fa197b8ee22dc
+  requires_python: '>=3.8'
+- kind: pypi
+  name: numpy
+  version: 1.24.4
+  url: https://files.pythonhosted.org/packages/a7/ae/f53b7b265fdc701e663fbb322a8e9d4b14d9cb7b2385f45ddfabfc4327e4/numpy-1.24.4-cp38-cp38-macosx_11_0_arm64.whl
+  sha256: 04640dab83f7c6c85abf9cd729c5b65f1ebd0ccf9de90b270cd61935eef0197f
+  requires_python: '>=3.8'
+- kind: pypi
+  name: numpy
+  version: 1.24.4
+  url: https://files.pythonhosted.org/packages/11/10/943cfb579f1a02909ff96464c69893b1d25be3731b5d3652c2e0cf1281ea/numpy-1.24.4-cp38-cp38-macosx_10_9_x86_64.whl
+  sha256: 1452241c290f3e2a312c137a9999cdbf63f78864d63c79039bda65ee86943f61
+  requires_python: '>=3.8'
+- kind: pypi
+  name: numpy
+  version: 1.24.4
+  url: https://files.pythonhosted.org/packages/69/65/0d47953afa0ad569d12de5f65d964321c208492064c38fe3b0b9744f8d44/numpy-1.24.4-cp38-cp38-win_amd64.whl
+  sha256: 692f2e0f55794943c5bfff12b3f56f99af76f902fc47487bdfe97856de51a706
+  requires_python: '>=3.8'
 - kind: conda
   name: openjpeg
   version: 2.5.2
   build: h3d672ee_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda
   sha256: dda71cbe094234ab208f3552dec1f4ca6f2e614175d010808d6cb66ecf0bc753
@@ -3462,14 +4030,32 @@
   md5: eb580fb888d93d5d550c557323ac5cee
   depends:
   - ca-certificates
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
+  purls: []
+  size: 2855250
+  timestamp: 1710793435903
+- kind: conda
+  name: openssl
+  version: 3.2.1
+  build: h0d3ecfb_1
+  build_number: 1
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
+  sha256: 519dc941d7ab0ebf31a2878d85c2f444450e7c5f6f41c4d07252c6bb3417b78b
+  md5: eb580fb888d93d5d550c557323ac5cee
+  depends:
+  - ca-certificates
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
   size: 2855250
   timestamp: 1710793435903
 - kind: conda
   name: openssl
   version: 3.2.1
   build: hcfcfb64_1
   build_number: 1
@@ -3482,14 +4068,35 @@
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
+  purls: []
+  size: 8230112
+  timestamp: 1710796158475
+- kind: conda
+  name: openssl
+  version: 3.2.1
+  build: hcfcfb64_1
+  build_number: 1
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
+  sha256: 61ce4e11c3c26ed4e4d9b7e7e2483121a1741ad0f9c8db0a91a28b6e05182ce6
+  md5: 958e0418e93e50c575bff70fbcaa12d8
+  depends:
+  - ca-certificates
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
   size: 8230112
   timestamp: 1710796158475
 - kind: conda
   name: openssl
   version: 3.2.1
   build: hd590300_1
   build_number: 1
@@ -3500,14 +4107,33 @@
   depends:
   - ca-certificates
   - libgcc-ng >=12
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
+  purls: []
+  size: 2865379
+  timestamp: 1710793235846
+- kind: conda
+  name: openssl
+  version: 3.2.1
+  build: hd590300_1
+  build_number: 1
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
+  sha256: 2c689444ed19a603be457284cf2115ee728a3fafb7527326e96054dee7cdc1a7
+  md5: 9d731343cff6ee2e5a25c4a091bf8e2a
+  depends:
+  - ca-certificates
+  - libgcc-ng >=12
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
   size: 2865379
   timestamp: 1710793235846
 - kind: conda
   name: openssl
   version: 3.2.1
   build: hd75f5a5_1
   build_number: 1
@@ -3517,14 +4143,32 @@
   md5: 570a6f04802df580be529f3a72d2bbf7
   depends:
   - ca-certificates
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
+  purls: []
+  size: 2506344
+  timestamp: 1710793930515
+- kind: conda
+  name: openssl
+  version: 3.2.1
+  build: hd75f5a5_1
+  build_number: 1
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
+  sha256: 7ae0ac6a1673584a8a380c2ff3d46eca48ed53bc7174c0d4eaa0dd2f247a0984
+  md5: 570a6f04802df580be529f3a72d2bbf7
+  depends:
+  - ca-certificates
+  constrains:
+  - pyopenssl >=22.1
+  license: Apache-2.0
+  license_family: Apache
   size: 2506344
   timestamp: 1710793930515
 - kind: conda
   name: packaging
   version: '24.0'
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -3532,14 +4176,31 @@
   url: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
   sha256: a390182d74c31dfd713c16db888c92c277feeb6d1fe96ff9d9c105f9564be48a
   md5: 248f521b64ce055e7feae3105e7abeb8
   depends:
   - python >=3.8
   license: Apache-2.0
   license_family: APACHE
+  purls:
+  - pkg:pypi/packaging?source=conda-forge-mapping
+  size: 49832
+  timestamp: 1710076089469
+- kind: conda
+  name: packaging
+  version: '24.0'
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+  sha256: a390182d74c31dfd713c16db888c92c277feeb6d1fe96ff9d9c105f9564be48a
+  md5: 248f521b64ce055e7feae3105e7abeb8
+  depends:
+  - python >=3.8
+  license: Apache-2.0
+  license_family: APACHE
   size: 49832
   timestamp: 1710076089469
 - kind: conda
   name: paginate
   version: 0.5.6
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -3562,14 +4223,15 @@
   sha256: eb355ac225be2f698e19dba4dcab7cb0748225677a9799e9cc8e4cadc3cb738f
   md5: ba76a6a448819560b5f8b08a9c74f415
   depends:
   - libgcc-ng >=7.5.0
   - libstdcxx-ng >=7.5.0
   license: GPL-3.0-or-later
   license_family: GPL
+  purls: []
   size: 94048
   timestamp: 1673473024463
 - kind: conda
   name: pathspec
   version: 0.12.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -3755,14 +4417,16 @@
   md5: e2783aa3f9235225eec92f9081c5b801
   depends:
   - python >=3.7
   - setuptools
   - wheel
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/pip?source=conda-forge-mapping
   size: 1386212
   timestamp: 1690024763393
 - kind: conda
   name: pixman
   version: 0.43.2
   build: h59595ed_0
   subdir: linux-64
@@ -3844,14 +4508,16 @@
   url: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
   sha256: 33eaa3359948a260ebccf9cdc2fd862cea5a6029783289e13602d8e634cd9a26
   md5: d3483c8fc2dc2cc3f5cf43e26d60cabf
   depends:
   - python >=3.8
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/pluggy?source=conda-forge-mapping
   size: 23815
   timestamp: 1713667175451
 - kind: conda
   name: psutil
   version: 5.9.8
   build: py38h01eb140_0
   subdir: linux-64
@@ -3860,14 +4526,16 @@
   md5: 571da172be3f0f94f49c069e5b775f05
   depends:
   - libgcc-ng >=12
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   license: BSD-3-Clause
   license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
   size: 362990
   timestamp: 1705722552521
 - kind: conda
   name: psutil
   version: 5.9.8
   build: py38h336bac9_0
   subdir: osx-arm64
@@ -3876,14 +4544,16 @@
   md5: 40175a55b8436b2bd216e94bfa168fdd
   depends:
   - python >=3.8,<3.9.0a0
   - python >=3.8,<3.9.0a0 *_cpython
   - python_abi 3.8.* *_cp38
   license: BSD-3-Clause
   license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
   size: 371521
   timestamp: 1705722783018
 - kind: conda
   name: psutil
   version: 5.9.8
   build: py38h91455d4_0
   subdir: win-64
@@ -3894,14 +4564,16 @@
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: BSD-3-Clause
   license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
   size: 380039
   timestamp: 1705723097147
 - kind: conda
   name: psutil
   version: 5.9.8
   build: py38hae2e43d_0
   subdir: osx-64
@@ -3909,14 +4581,16 @@
   sha256: d946b6d24f33047f50ade6187fd84bde4c989b235c941225d02e62fb279c86ba
   md5: 472f759cff3581370fac5d574c559d0a
   depends:
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   license: BSD-3-Clause
   license_family: BSD
+  purls:
+  - pkg:pypi/psutil?source=conda-forge-mapping
   size: 368246
   timestamp: 1705722700095
 - kind: conda
   name: pthread-stubs
   version: '0.4'
   build: h27ca646_1001
   build_number: 1001
@@ -4070,14 +4744,16 @@
   - pluggy >=0.12,<2.0
   - python >=3.7
   - tomli >=1.0.0
   constrains:
   - pytest-faulthandler >=2
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/pytest?source=conda-forge-mapping
   size: 244564
   timestamp: 1704035308916
 - kind: conda
   name: pytest-asyncio
   version: 0.21.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -4087,14 +4763,16 @@
   md5: c8fd31da9b1059c4440f31f6ab4d620c
   depends:
   - pytest >=7.0.0,<8.0.0a0
   - python >=3.7
   - typing_extensions >=3.7.2
   license: Apache-2.0
   license_family: APACHE
+  purls:
+  - pkg:pypi/pytest-asyncio?source=conda-forge-mapping
   size: 26068
   timestamp: 1689174411610
 - kind: conda
   name: pytest-xprocess
   version: 0.23.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -4104,14 +4782,16 @@
   md5: c9178b28f47fd191ac0a668b84e8fa18
   depends:
   - psutil
   - pytest >=2.8
   - python >=3.8
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/pytest-xprocess?source=conda-forge-mapping
   size: 19270
   timestamp: 1695495262467
 - kind: conda
   name: python
   version: 3.8.19
   build: h2469fbe_0_cpython
   subdir: osx-arm64
@@ -4127,14 +4807,15 @@
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.8.* *_cp38
   license: Python-2.0
+  purls: []
   size: 11719163
   timestamp: 1710939584543
 - kind: conda
   name: python
   version: 3.8.19
   build: h4de0772_0_cpython
   subdir: win-64
@@ -4150,14 +4831,15 @@
   - tk >=8.6.13,<8.7.0a0
   - vc >=14.1,<15
   - vc14_runtime >=14.16.27033
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.8.* *_cp38
   license: Python-2.0
+  purls: []
   size: 16090293
   timestamp: 1710939361361
 - kind: conda
   name: python
   version: 3.8.19
   build: h5ba8234_0_cpython
   subdir: osx-64
@@ -4173,14 +4855,15 @@
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.8.* *_cp38
   license: Python-2.0
+  purls: []
   size: 12325720
   timestamp: 1710939847267
 - kind: conda
   name: python
   version: 3.8.19
   build: hd12c33a_0_cpython
   subdir: linux-64
@@ -4201,14 +4884,15 @@
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.8.* *_cp38
   license: Python-2.0
+  purls: []
   size: 22357104
   timestamp: 1710939954552
 - kind: conda
   name: python
   version: 3.12.3
   build: h1411813_0_cpython
   subdir: osx-64
@@ -4340,14 +5024,15 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-4_cp38.conda
   sha256: 54276b9259f5c72d160c75c45c50c4e03695da56e6646518801f567fc5979030
   md5: ea6b353536f42246cd130c7fef1285cf
   constrains:
   - python 3.8.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
+  purls: []
   size: 6371
   timestamp: 1695147367061
 - kind: conda
   name: python_abi
   version: '3.8'
   build: 4_cp38
   build_number: 4
@@ -4355,14 +5040,15 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-4_cp38.conda
   sha256: 0dab6ce7b8e48f2308aa9c37e8feceaa7c84ee335745c1803686fbbb59a19926
   md5: 74bec187a12aed00501eaafd35e694bf
   constrains:
   - python 3.8.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
+  purls: []
   size: 6479
   timestamp: 1695147767216
 - kind: conda
   name: python_abi
   version: '3.8'
   build: 4_cp38
   build_number: 4
@@ -4370,14 +5056,15 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.8-4_cp38.conda
   sha256: 81a67cd91e7f07af481bae8cdea913bccab9a1b6155b2c81d21fbf31efe846a0
   md5: 69175aa707e394d51c35dda08bb339d9
   constrains:
   - python 3.8.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
+  purls: []
   size: 6461
   timestamp: 1695147757654
 - kind: conda
   name: python_abi
   version: '3.8'
   build: 4_cp38
   build_number: 4
@@ -4385,14 +5072,15 @@
   url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-4_cp38.conda
   sha256: fa131149ca3b73aac06f839ee9525581517f50829eaa93fc0e8787b4797e4df0
   md5: b1059de1664cef9a785dda079a50f1ed
   constrains:
   - python 3.8.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
+  purls: []
   size: 6751
   timestamp: 1695147671006
 - kind: conda
   name: python_abi
   version: '3.12'
   build: 4_cp312
   build_number: 4
@@ -4565,14 +5253,31 @@
   sha256: 5435cf39d039387fbdc977b0a762357ea909a7694d9528ab40f005e9208744d7
   md5: 47d31b792659ce70f470b5c82fdfb7a4
   depends:
   - libgcc-ng >=12
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
+  purls: []
+  size: 281456
+  timestamp: 1679532220005
+- kind: conda
+  name: readline
+  version: '8.2'
+  build: h8228510_1
+  build_number: 1
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
+  sha256: 5435cf39d039387fbdc977b0a762357ea909a7694d9528ab40f005e9208744d7
+  md5: 47d31b792659ce70f470b5c82fdfb7a4
+  depends:
+  - libgcc-ng >=12
+  - ncurses >=6.3,<7.0a0
+  license: GPL-3.0-only
+  license_family: GPL
   size: 281456
   timestamp: 1679532220005
 - kind: conda
   name: readline
   version: '8.2'
   build: h92ec313_1
   build_number: 1
@@ -4580,14 +5285,30 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
   sha256: a1dfa679ac3f6007362386576a704ad2d0d7a02e98f5d0b115f207a2da63e884
   md5: 8cbb776a2f641b943d413b3e19df71f4
   depends:
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
+  purls: []
+  size: 250351
+  timestamp: 1679532511311
+- kind: conda
+  name: readline
+  version: '8.2'
+  build: h92ec313_1
+  build_number: 1
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
+  sha256: a1dfa679ac3f6007362386576a704ad2d0d7a02e98f5d0b115f207a2da63e884
+  md5: 8cbb776a2f641b943d413b3e19df71f4
+  depends:
+  - ncurses >=6.3,<7.0a0
+  license: GPL-3.0-only
+  license_family: GPL
   size: 250351
   timestamp: 1679532511311
 - kind: conda
   name: readline
   version: '8.2'
   build: h9e318b2_1
   build_number: 1
@@ -4595,14 +5316,30 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
   sha256: 41e7d30a097d9b060037f0c6a2b1d4c4ae7e942c06c943d23f9d481548478568
   md5: f17f77f2acf4d344734bda76829ce14e
   depends:
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
+  purls: []
+  size: 255870
+  timestamp: 1679532707590
+- kind: conda
+  name: readline
+  version: '8.2'
+  build: h9e318b2_1
+  build_number: 1
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
+  sha256: 41e7d30a097d9b060037f0c6a2b1d4c4ae7e942c06c943d23f9d481548478568
+  md5: f17f77f2acf4d344734bda76829ce14e
+  depends:
+  - ncurses >=6.3,<7.0a0
+  license: GPL-3.0-only
+  license_family: GPL
   size: 255870
   timestamp: 1679532707590
 - kind: conda
   name: regex
   version: 2024.4.28
   build: py312h4389bb4_0
   subdir: win-64
@@ -4700,14 +5437,16 @@
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/ruff?source=conda-forge-mapping
   size: 6422629
   timestamp: 1712962234140
 - kind: conda
   name: ruff
   version: 0.3.7
   build: py38h1916ca8_0
   subdir: osx-64
@@ -4718,14 +5457,16 @@
   - libcxx >=16
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   constrains:
   - __osx >=10.12
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/ruff?source=conda-forge-mapping
   size: 6191203
   timestamp: 1712963583220
 - kind: conda
   name: ruff
   version: 0.3.7
   build: py38h5477e86_0
   subdir: osx-arm64
@@ -4737,14 +5478,16 @@
   - python >=3.8,<3.9.0a0
   - python >=3.8,<3.9.0a0 *_cpython
   - python_abi 3.8.* *_cp38
   constrains:
   - __osx >=11.0
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/ruff?source=conda-forge-mapping
   size: 5874349
   timestamp: 1712963888097
 - kind: conda
   name: ruff
   version: 0.3.7
   build: py38h5e48be7_0
   subdir: win-64
@@ -4755,28 +5498,31 @@
   - python >=3.8,<3.9.0a0
   - python_abi 3.8.* *_cp38
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/ruff?source=conda-forge-mapping
   size: 6343187
   timestamp: 1712963346969
 - kind: conda
   name: rust
   version: 1.77.2
   build: h4ff7c5d_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/rust-1.77.2-h4ff7c5d_0.conda
   sha256: 048ffabbbbd1b5109d59ec15610cf0e489c39b4f6f380953816bcb26dad8da17
   md5: 4083c1a9d7f5c9591273f578530d6388
   depends:
   - rust-std-aarch64-apple-darwin 1.77.2 hf6ec828_0
   license: MIT
   license_family: MIT
+  purls: []
   size: 145759919
   timestamp: 1712743398771
 - kind: conda
   name: rust
   version: 1.77.2
   build: h70c747d_0
   subdir: linux-64
@@ -4786,42 +5532,45 @@
   depends:
   - gcc_impl_linux-64
   - libgcc-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   - rust-std-x86_64-unknown-linux-gnu 1.77.2 h2c6d0dc_0
   license: MIT
   license_family: MIT
+  purls: []
   size: 186765686
   timestamp: 1712741423714
 - kind: conda
   name: rust
   version: 1.77.2
   build: h7e1429e_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/rust-1.77.2-h7e1429e_0.conda
   sha256: d12cde3691eb50148b49460ac2bff0c0716204099a38d36132762ffb0c6c79fd
   md5: 13c8a97dd157999cdd23adaac7919047
   depends:
   - rust-std-x86_64-apple-darwin 1.77.2 h38e4360_0
   license: MIT
   license_family: MIT
+  purls: []
   size: 192493395
   timestamp: 1712743664947
 - kind: conda
   name: rust
   version: 1.77.2
   build: hf8d6059_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/rust-1.77.2-hf8d6059_0.conda
   sha256: 978228c14a3d2af2d9d52230443f232d7a22cbbe98d359a306b1a761773d4589
   md5: ba05fee8761e5bd25ae642a4b77d2ed7
   depends:
   - rust-std-x86_64-pc-windows-msvc 1.77.2 h17fc481_0
   license: MIT
   license_family: MIT
+  purls: []
   size: 187565499
   timestamp: 1712743189902
 - kind: conda
   name: rust-std-aarch64-apple-darwin
   version: 1.77.2
   build: hf6ec828_0
   subdir: noarch
@@ -4831,14 +5580,15 @@
   md5: 729f181cdeb249ff2da37f434b548633
   depends:
   - __unix
   constrains:
   - rust >=1.77.2,<1.77.3.0a0
   license: MIT
   license_family: MIT
+  purls: []
   size: 30933811
   timestamp: 1712740743456
 - kind: conda
   name: rust-std-x86_64-apple-darwin
   version: 1.77.2
   build: h38e4360_0
   subdir: noarch
@@ -4848,14 +5598,15 @@
   md5: 67db6d59468a8145fb076d75d156b69c
   depends:
   - __unix
   constrains:
   - rust >=1.77.2,<1.77.3.0a0
   license: MIT
   license_family: MIT
+  purls: []
   size: 31857486
   timestamp: 1712740749097
 - kind: conda
   name: rust-std-x86_64-pc-windows-msvc
   version: 1.77.2
   build: h17fc481_0
   subdir: noarch
@@ -4865,14 +5616,15 @@
   md5: 2149767f1c882154246a9a569991e3c3
   depends:
   - __win
   constrains:
   - rust >=1.77.2,<1.77.3.0a0
   license: MIT
   license_family: MIT
+  purls: []
   size: 25276039
   timestamp: 1712742986757
 - kind: conda
   name: rust-std-x86_64-unknown-linux-gnu
   version: 1.77.2
   build: h2c6d0dc_0
   subdir: noarch
@@ -4882,14 +5634,15 @@
   md5: db8b81b3806faafe2f6f7bd431f72e37
   depends:
   - __unix
   constrains:
   - rust >=1.77.2,<1.77.3.0a0
   license: MIT
   license_family: MIT
+  purls: []
   size: 33827015
   timestamp: 1712741238767
 - kind: conda
   name: setuptools
   version: 69.5.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -4897,14 +5650,31 @@
   url: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
   sha256: 72d143408507043628b32bed089730b6d5f5445eccc44b59911ec9f262e365e7
   md5: 7462280d81f639363e6e63c81276bd9e
   depends:
   - python >=3.8
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/setuptools?source=conda-forge-mapping
+  size: 501790
+  timestamp: 1713094963112
+- kind: conda
+  name: setuptools
+  version: 69.5.1
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+  sha256: 72d143408507043628b32bed089730b6d5f5445eccc44b59911ec9f262e365e7
+  md5: 7462280d81f639363e6e63c81276bd9e
+  depends:
+  - python >=3.8
+  license: MIT
+  license_family: MIT
   size: 501790
   timestamp: 1713094963112
 - kind: conda
   name: six
   version: 1.16.0
   build: pyh6c4a22f_0
   subdir: noarch
@@ -4928,14 +5698,15 @@
   url: https://conda.anaconda.org/conda-forge/noarch/sysroot_linux-64-2.12-he073ed8_17.conda
   sha256: b4e4d685e41cb36cfb16f0cb15d2c61f8f94f56fab38987a44eff95d8a673fb5
   md5: 595db67e32b276298ff3d94d07d47fbf
   depends:
   - kernel-headers_linux-64 2.6.32 he073ed8_17
   license: LGPL-2.0-or-later AND LGPL-2.0-or-later WITH exceptions AND GPL-2.0-or-later AND MPL-2.0
   license_family: GPL
+  purls: []
   size: 15127123
   timestamp: 1708000843849
 - kind: conda
   name: tinycss2
   version: 1.3.0
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -4959,14 +5730,30 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
   sha256: 30412b2e9de4ff82d8c2a7e5d06a15f4f4fef1809a72138b6ccb53a33b26faf5
   md5: bf830ba5afc507c6232d4ef0fb1a882d
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: TCL
   license_family: BSD
+  purls: []
+  size: 3270220
+  timestamp: 1699202389792
+- kind: conda
+  name: tk
+  version: 8.6.13
+  build: h1abcd95_1
+  build_number: 1
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
+  sha256: 30412b2e9de4ff82d8c2a7e5d06a15f4f4fef1809a72138b6ccb53a33b26faf5
+  md5: bf830ba5afc507c6232d4ef0fb1a882d
+  depends:
+  - libzlib >=1.2.13,<1.3.0a0
+  license: TCL
+  license_family: BSD
   size: 3270220
   timestamp: 1699202389792
 - kind: conda
   name: tk
   version: 8.6.13
   build: h5083fa2_1
   build_number: 1
@@ -4974,14 +5761,30 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
   sha256: 72457ad031b4c048e5891f3f6cb27a53cb479db68a52d965f796910e71a403a8
   md5: b50a57ba89c32b62428b71a875291c9b
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: TCL
   license_family: BSD
+  purls: []
+  size: 3145523
+  timestamp: 1699202432999
+- kind: conda
+  name: tk
+  version: 8.6.13
+  build: h5083fa2_1
+  build_number: 1
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
+  sha256: 72457ad031b4c048e5891f3f6cb27a53cb479db68a52d965f796910e71a403a8
+  md5: b50a57ba89c32b62428b71a875291c9b
+  depends:
+  - libzlib >=1.2.13,<1.3.0a0
+  license: TCL
+  license_family: BSD
   size: 3145523
   timestamp: 1699202432999
 - kind: conda
   name: tk
   version: 8.6.13
   build: h5226925_1
   build_number: 1
@@ -4991,14 +5794,32 @@
   md5: fc048363eb8f03cd1737600a5d08aafe
   depends:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: TCL
   license_family: BSD
+  purls: []
+  size: 3503410
+  timestamp: 1699202577803
+- kind: conda
+  name: tk
+  version: 8.6.13
+  build: h5226925_1
+  build_number: 1
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
+  sha256: 2c4e914f521ccb2718946645108c9bd3fc3216ba69aea20c2c3cedbd8db32bb1
+  md5: fc048363eb8f03cd1737600a5d08aafe
+  depends:
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: TCL
+  license_family: BSD
   size: 3503410
   timestamp: 1699202577803
 - kind: conda
   name: tk
   version: 8.6.13
   build: noxft_h4845f30_101
   build_number: 101
@@ -5007,14 +5828,31 @@
   sha256: e0569c9caa68bf476bead1bed3d79650bb080b532c64a4af7d8ca286c08dea4e
   md5: d453b98d9c83e71da0741bb0ff4d76bc
   depends:
   - libgcc-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   license: TCL
   license_family: BSD
+  purls: []
+  size: 3318875
+  timestamp: 1699202167581
+- kind: conda
+  name: tk
+  version: 8.6.13
+  build: noxft_h4845f30_101
+  build_number: 101
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
+  sha256: e0569c9caa68bf476bead1bed3d79650bb080b532c64a4af7d8ca286c08dea4e
+  md5: d453b98d9c83e71da0741bb0ff4d76bc
+  depends:
+  - libgcc-ng >=12
+  - libzlib >=1.2.13,<1.3.0a0
+  license: TCL
+  license_family: BSD
   size: 3318875
   timestamp: 1699202167581
 - kind: conda
   name: tomli
   version: 2.0.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -5022,16 +5860,26 @@
   url: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
   sha256: 4cd48aba7cd026d17e86886af48d0d2ebc67ed36f87f6534f4b67138f5a5a58f
   md5: 5844808ffab9ebdb694585b50ba02a96
   depends:
   - python >=3.7
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/tomli?source=conda-forge-mapping
   size: 15940
   timestamp: 1644342331069
+- kind: pypi
+  name: types-networkx
+  version: 3.2.1.20240531
+  url: https://files.pythonhosted.org/packages/98/ab/3c2794cf8ce4daa7f451008e5b8a9880a7ff8357ddb383e9de4f35034842/types_networkx-3.2.1.20240531-py3-none-any.whl
+  sha256: de335c599ed79d065ac0937c667c61c26a45f8f6d7b9f628b4420df5c2ca2fa5
+  requires_dist:
+  - numpy
+  requires_python: '>=3.8'
 - kind: conda
   name: typing-extensions
   version: 4.11.0
   build: hd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
@@ -5052,14 +5900,31 @@
   url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
   sha256: a7e8714d14f854058e971a6ed44f18cc37cc685f98ddefb2e6b7899a0cc4d1a2
   md5: 6ef2fc37559256cf682d8b3375e89b80
   depends:
   - python >=3.8
   license: PSF-2.0
   license_family: PSF
+  purls:
+  - pkg:pypi/typing-extensions?source=conda-forge-mapping
+  size: 37583
+  timestamp: 1712330089194
+- kind: conda
+  name: typing_extensions
+  version: 4.11.0
+  build: pyha770c72_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+  sha256: a7e8714d14f854058e971a6ed44f18cc37cc685f98ddefb2e6b7899a0cc4d1a2
+  md5: 6ef2fc37559256cf682d8b3375e89b80
+  depends:
+  - python >=3.8
+  license: PSF-2.0
+  license_family: PSF
   size: 37583
   timestamp: 1712330089194
 - kind: conda
   name: tzdata
   version: 2024a
   build: h0c530f3_0
   subdir: noarch
@@ -5078,14 +5943,29 @@
   url: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
   sha256: f29cdaf8712008f6b419b8b1a403923b00ab2504bfe0fb2ba8eb60e72d4f14c6
   md5: 72608f6cd3e5898229c3ea16deb1ac43
   constrains:
   - vs2015_runtime >=14.29.30037
   license: LicenseRef-Proprietary
   license_family: PROPRIETARY
+  purls: []
+  size: 1283972
+  timestamp: 1666630199266
+- kind: conda
+  name: ucrt
+  version: 10.0.22621.0
+  build: h57928b3_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
+  sha256: f29cdaf8712008f6b419b8b1a403923b00ab2504bfe0fb2ba8eb60e72d4f14c6
+  md5: 72608f6cd3e5898229c3ea16deb1ac43
+  constrains:
+  - vs2015_runtime >=14.29.30037
+  license: LicenseRef-Proprietary
+  license_family: PROPRIETARY
   size: 1283972
   timestamp: 1666630199266
 - kind: conda
   name: urllib3
   version: 2.2.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -5112,17 +5992,53 @@
   md5: 20e1e652a4c740fa719002a8449994a2
   depends:
   - vc14_runtime >=14.38.33130
   track_features:
   - vc14
   license: BSD-3-Clause
   license_family: BSD
+  purls: []
   size: 16977
   timestamp: 1702511255313
 - kind: conda
+  name: vc
+  version: '14.3'
+  build: hcf57466_18
+  build_number: 18
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
+  sha256: 447a8d8292a7b2107dcc18afb67f046824711a652725fc0f522c368e7a7b8318
+  md5: 20e1e652a4c740fa719002a8449994a2
+  depends:
+  - vc14_runtime >=14.38.33130
+  track_features:
+  - vc14
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 16977
+  timestamp: 1702511255313
+- kind: conda
+  name: vc14_runtime
+  version: 14.38.33130
+  build: h82b7239_18
+  build_number: 18
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
+  sha256: bf94c9af4b2e9cba88207001197e695934eadc96a5c5e4cd7597e950aae3d8ff
+  md5: 8be79fdd2725ddf7bbf8a27a4c1f79ba
+  depends:
+  - ucrt >=10.0.20348.0
+  constrains:
+  - vs2015_runtime 14.38.33130.* *_18
+  license: LicenseRef-ProprietaryMicrosoft
+  license_family: Proprietary
+  purls: []
+  size: 749868
+  timestamp: 1702511239004
+- kind: conda
   name: vc14_runtime
   version: 14.38.33130
   build: h82b7239_18
   build_number: 18
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
   sha256: bf94c9af4b2e9cba88207001197e695934eadc96a5c5e4cd7597e950aae3d8ff
@@ -5144,14 +6060,30 @@
   url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
   sha256: a2fec221f361d6263c117f4ea6d772b21c90a2f8edc6f3eb0eadec6bfe8843db
   md5: 10d42885e3ed84e575b454db30f1aa93
   depends:
   - vc14_runtime >=14.38.33130
   license: BSD-3-Clause
   license_family: BSD
+  purls: []
+  size: 16988
+  timestamp: 1702511261442
+- kind: conda
+  name: vs2015_runtime
+  version: 14.38.33130
+  build: hcb4865c_18
+  build_number: 18
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
+  sha256: a2fec221f361d6263c117f4ea6d772b21c90a2f8edc6f3eb0eadec6bfe8843db
+  md5: 10d42885e3ed84e575b454db30f1aa93
+  depends:
+  - vc14_runtime >=14.38.33130
+  license: BSD-3-Clause
+  license_family: BSD
   size: 16988
   timestamp: 1702511261442
 - kind: conda
   name: watchdog
   version: 4.0.0
   build: py312h2e8e312_0
   subdir: win-64
@@ -5241,14 +6173,16 @@
   url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
   sha256: cb318f066afd6fd64619f14c030569faf3f53e6f50abf743b4c865e7d95b96bc
   md5: 0b5293a157c2b5cd513dd1b03d8d3aae
   depends:
   - python >=3.8
   license: MIT
   license_family: MIT
+  purls:
+  - pkg:pypi/wheel?source=conda-forge-mapping
   size: 57963
   timestamp: 1711546009410
 - kind: conda
   name: win_inet_pton
   version: 1.1.0
   build: pyhd8ed1ab_6
   build_number: 6
@@ -5516,41 +6450,94 @@
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
   sha256: 03a6d28ded42af8a347345f82f3eebdd6807a08526d47899a42d62d319609162
   md5: 2161070d867d1b1204ea749c8eec4ef0
   depends:
   - libgcc-ng >=12
   license: LGPL-2.1 and GPL-2.0
+  purls: []
+  size: 418368
+  timestamp: 1660346797927
+- kind: conda
+  name: xz
+  version: 5.2.6
+  build: h166bdaf_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+  sha256: 03a6d28ded42af8a347345f82f3eebdd6807a08526d47899a42d62d319609162
+  md5: 2161070d867d1b1204ea749c8eec4ef0
+  depends:
+  - libgcc-ng >=12
+  license: LGPL-2.1 and GPL-2.0
   size: 418368
   timestamp: 1660346797927
 - kind: conda
   name: xz
   version: 5.2.6
   build: h57fd34a_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
   sha256: 59d78af0c3e071021cfe82dc40134c19dab8cdf804324b62940f5c8cd71803ec
   md5: 39c6b54e94014701dd157f4f576ed211
   license: LGPL-2.1 and GPL-2.0
+  purls: []
+  size: 235693
+  timestamp: 1660346961024
+- kind: conda
+  name: xz
+  version: 5.2.6
+  build: h57fd34a_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+  sha256: 59d78af0c3e071021cfe82dc40134c19dab8cdf804324b62940f5c8cd71803ec
+  md5: 39c6b54e94014701dd157f4f576ed211
+  license: LGPL-2.1 and GPL-2.0
   size: 235693
   timestamp: 1660346961024
 - kind: conda
   name: xz
   version: 5.2.6
   build: h775f41a_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
   sha256: eb09823f34cc2dd663c0ec4ab13f246f45dcd52e5b8c47b9864361de5204a1c8
   md5: a72f9d4ea13d55d745ff1ed594747f10
   license: LGPL-2.1 and GPL-2.0
+  purls: []
   size: 238119
   timestamp: 1660346964847
 - kind: conda
   name: xz
   version: 5.2.6
+  build: h775f41a_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+  sha256: eb09823f34cc2dd663c0ec4ab13f246f45dcd52e5b8c47b9864361de5204a1c8
+  md5: a72f9d4ea13d55d745ff1ed594747f10
+  license: LGPL-2.1 and GPL-2.0
+  size: 238119
+  timestamp: 1660346964847
+- kind: conda
+  name: xz
+  version: 5.2.6
+  build: h8d14728_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+  sha256: 54d9778f75a02723784dc63aff4126ff6e6749ba21d11a6d03c1f4775f269fe0
+  md5: 515d77642eaa3639413c6b1bc3f94219
+  depends:
+  - vc >=14.1,<15
+  - vs2015_runtime >=14.16.27033
+  license: LGPL-2.1 and GPL-2.0
+  purls: []
+  size: 217804
+  timestamp: 1660346976440
+- kind: conda
+  name: xz
+  version: 5.2.6
   build: h8d14728_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
   sha256: 54d9778f75a02723784dc63aff4126ff6e6749ba21d11a6d03c1f4775f269fe0
   md5: 515d77642eaa3639413c6b1bc3f94219
   depends:
   - vc >=14.1,<15
```

### Comparing `py_rattler-0.6.1/pixi.toml` & `py_rattler-0.6.2/pixi.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,27 +32,30 @@
 ruff = ">=0.3.3,<0.4"
 mypy = "~=1.5.1"
 
 pytest = "~=7.4.0"
 pytest-asyncio = "0.21.1.*"
 pytest-xprocess = ">=0.23.0,<0.24"
 
+[feature.test.pypi-dependencies]
+types-networkx = "*"
+
 [feature.test.tasks]
 test = { cmd = "pytest --doctest-modules", depends_on = ["build"] }
-fmt-python = "ruff format rattler"
+fmt-python = "ruff format rattler examples"
 fmt-rust = "cargo fmt --all"
 lint-python = "ruff check ."
 lint-rust = "cargo clippy --all"
 fmt = { depends_on = ["fmt-python", "fmt-rust"] }
 lint = { depends_on = ["type-check", "lint-python", "lint-rust"] }
 type-check = { cmd = "mypy", depends_on = ["build"] }
 
 # checks for the CI
 fmt-rust-check = "cargo fmt --all --check"
-fmt-python-check = "ruff format rattler --diff"
+fmt-python-check = "ruff format rattler examples --diff"
 fmt-check = { depends_on = ["fmt-python-check", "fmt-rust-check"] }
 
 [feature.docs.dependencies]
 mkdocs = "1.5.3.*"
 mkdocstrings-python = ">=1.9.0,<1.10"
 mkdocstrings = ">=0.24.1,<0.25"
 mkdocs-material = ">=9.5.20"
```

### Comparing `py_rattler-0.6.1/pyproject.toml` & `py_rattler-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 [tool.ruff]
 line-length = 120
 target-version = "py38"
 
 [tool.mypy]
 python_version = "3.8"
-files = ["rattler", "tests"]
+files = ["rattler", "tests", "examples"]
 strict = true
 enable_error_code = ["redundant-expr", "truthy-bool", "ignore-without-code"]
 disable_error_code = ["empty-body"]
 
 [[tool.mypy.overrides]]
 module = ["rattler.rattler"]
 ignore_missing_imports = true
```

### Comparing `py_rattler-0.6.1/rattler/__init__.py` & `py_rattler-0.6.2/rattler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/channel/channel.py` & `py_rattler-0.6.2/rattler/channel/channel.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/channel/channel_config.py` & `py_rattler-0.6.2/rattler/channel/channel_config.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/exceptions.py` & `py_rattler-0.6.2/rattler/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/index/index.py` & `py_rattler-0.6.2/rattler/index/index.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/install/installer.py` & `py_rattler-0.6.2/rattler/install/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from rattler.repo_data.record import RepoDataRecord
 
 from rattler.rattler import py_install
 
 
 async def install(
     records: List[RepoDataRecord],
-    target_prefix: os.PathLike[str],
+    target_prefix: str | os.PathLike[str],
     cache_dir: Optional[os.PathLike[str]] = None,
     installed_packages: Optional[List[PrefixRecord]] = None,
     platform: Optional[Platform] = None,
     execute_link_scripts: bool = False,
     show_progress: bool = True,
     client: Optional[AuthenticatedClient] = None,
 ) -> None:
@@ -69,15 +69,15 @@
         show_progress: If set to `True` a progress bar will be shown on the CLI.
         client: An authenticated client to use for downloading packages. If not specified a default
                 client will be used.
     """
 
     await py_install(
         records=records,
-        target_prefix=target_prefix,
+        target_prefix=str(target_prefix),
         cache_dir=cache_dir,
         installed_packages=installed_packages,
         platform=platform._inner if platform is not None else None,
         client=client._client if client is not None else None,
         execute_link_scripts=execute_link_scripts,
         show_progress=show_progress,
     )
```

### Comparing `py_rattler-0.6.1/rattler/lock/channel.py` & `py_rattler-0.6.2/rattler/lock/channel.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/lock/environment.py` & `py_rattler-0.6.2/rattler/lock/environment.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/lock/hash.py` & `py_rattler-0.6.2/rattler/lock/hash.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/lock/lock_file.py` & `py_rattler-0.6.2/rattler/lock/lock_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         Returns an iterator over all environments defined in the lock-file.
 
         Examples
         --------
         ```python
         >>> lock_file = LockFile.from_path("./pixi.lock")
         >>> lock_file.environments()
-        [('default', Environment()), ('docs', Environment()), ('build', Environment()), ('test', Environment())]
+        [('default', Environment()), ('docs', Environment()), ('test', Environment())]
         >>>
         ```
         """
         return [(name, Environment._from_py_environment(e)) for (name, e) in self._lock_file.environments()]
 
     def environment(self, name: str) -> Optional[Environment]:
         """
```

### Comparing `py_rattler-0.6.1/rattler/lock/package.py` & `py_rattler-0.6.2/rattler/lock/package.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/lock/pypi.py` & `py_rattler-0.6.2/rattler/lock/pypi.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/match_spec/match_spec.py` & `py_rattler-0.6.2/rattler/match_spec/match_spec.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/match_spec/nameless_match_spec.py` & `py_rattler-0.6.2/rattler/match_spec/nameless_match_spec.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/networking/authenticated_client.py` & `py_rattler-0.6.2/rattler/networking/authenticated_client.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/networking/fetch_repo_data.py` & `py_rattler-0.6.2/rattler/networking/fetch_repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/package/__init__.py` & `py_rattler-0.6.2/rattler/package/__init__.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/package/about_json.py` & `py_rattler-0.6.2/rattler/package/about_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/package/index_json.py` & `py_rattler-0.6.2/rattler/package/index_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import os
+import datetime
 from pathlib import Path
 from typing import List, Optional
 
 from rattler.package.package_name import PackageName
 from rattler.rattler import PyIndexJson
 
 
@@ -281,31 +282,31 @@
         """
         if subdir := self._inner.subdir:
             return subdir
 
         return None
 
     @property
-    def timestamp(self) -> Optional[int]:
+    def timestamp(self) -> Optional[datetime.datetime]:
         """
         The timestamp when this package was created
 
         Examples
         --------
         ```python
         >>> idx_json = IndexJson.from_package_archive(
         ...     "../test-data/with-symlinks/python-3.10.6-h2c4edbf_0_cpython.tar.bz2"
         ... )
         >>> idx_json.timestamp
-        1661200742
+        datetime.datetime(2022, 8, 22, 20, 39, 2, 467000, tzinfo=datetime.timezone.utc)
         >>>
         ```
         """
         if timestamp := self._inner.timestamp:
-            return timestamp
+            return datetime.datetime.fromtimestamp(timestamp / 1000.0, tz=datetime.timezone.utc)
 
         return None
 
     @property
     def track_features(self) -> List[str]:
         """
         Track features are nowadays only used to downweight packages (ie. give them less priority). To
```

### Comparing `py_rattler-0.6.1/rattler/package/no_arch_type.py` & `py_rattler-0.6.2/rattler/package/no_arch_type.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/package/package_name.py` & `py_rattler-0.6.2/rattler/package/package_name.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/package/paths_json.py` & `py_rattler-0.6.2/rattler/package/paths_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/package/run_exports_json.py` & `py_rattler-0.6.2/rattler/package/run_exports_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/platform/arch.py` & `py_rattler-0.6.2/rattler/platform/arch.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/platform/platform.py` & `py_rattler-0.6.2/rattler/platform/platform.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/prefix/prefix_paths.py` & `py_rattler-0.6.2/rattler/prefix/prefix_paths.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/prefix/prefix_record.py` & `py_rattler-0.6.2/rattler/prefix/prefix_record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/repo_data/gateway.py` & `py_rattler-0.6.2/rattler/repo_data/gateway.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/repo_data/package_record.py` & `py_rattler-0.6.2/rattler/repo_data/package_record.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from __future__ import annotations
 import os
-from typing import List, Optional
+from typing import List, Optional, TYPE_CHECKING
+import datetime
 
 from rattler import VersionWithSource
 from rattler.match_spec.match_spec import MatchSpec
 from rattler.package.no_arch_type import NoArchType
 from rattler.package.package_name import PackageName
 from rattler.rattler import PyRecord
 
+if TYPE_CHECKING:
+    import networkx as nx
+else:
+    try:
+        import networkx as nx
+    except ImportError:
+        nx = None
+
 
 class PackageRecord:
     """
     A single record in the Conda repodata. A single
     record refers to a single binary distribution
     of a package on a Conda channel.
     """
@@ -71,14 +80,49 @@
         >>> sorted[0].name
         PackageName("vc")
         >>>
         ```
         """
         return [PackageRecord._from_py_record(p) for p in PyRecord.sort_topologically(records)]
 
+    @staticmethod
+    def to_graph(records: List[PackageRecord]) -> nx.DiGraph:  # type: ignore[type-arg]
+        """
+        Converts a list of PackageRecords to a DAG (`networkx.DiGraph`).
+        The nodes in the graph are the PackageRecords and the edges are the dependencies.
+
+        Examples
+        --------
+        ```python
+        import rattler
+        import asyncio
+        import networkx as nx
+        from matplotlib import pyplot as plt
+
+        records = asyncio.run(rattler.solve(['main'], ['python'], platforms=['osx-arm64', 'noarch']))
+        graph = rattler.PackageRecord.to_graph(records)
+
+        nx.draw(graph, with_labels=True, font_weight='bold')
+        plt.show()
+        ```
+        """
+        if nx is None:
+            raise ImportError("networkx is not installed")
+
+        names_to_records = {record.name: record for record in records}
+
+        graph = nx.DiGraph()  # type: ignore[var-annotated]
+        for record in records:
+            graph.add_node(record)
+            for dep in record.depends:
+                name = dep.split(" ")[0]
+                graph.add_edge(record, names_to_records[PackageName(name)])
+
+        return graph
+
     @classmethod
     def _from_py_record(cls, py_record: PyRecord) -> PackageRecord:
         """
         Construct Rattler PackageRecord from FFI PyRecord object.
         """
 
         # quick sanity check
@@ -388,30 +432,33 @@
         'win-64'
         >>>
         ```
         """
         return self._record.subdir
 
     @property
-    def timestamp(self) -> Optional[int]:
+    def timestamp(self) -> Optional[datetime.datetime]:
         """
         The date this entry was created.
 
         Examples
         --------
         ```python
         >>> from rattler import PrefixRecord
         >>> record = PrefixRecord.from_path(
         ...     "../test-data/conda-meta/libsqlite-3.40.0-hcfcfb64_0.json"
         ... )
         >>> record.timestamp
-        1668697639
+        datetime.datetime(2022, 11, 17, 15, 7, 19, 781000, tzinfo=datetime.timezone.utc)
         >>>
         ```
         """
+        if self._record.timestamp:
+            return datetime.datetime.fromtimestamp(self._record.timestamp / 1000.0, tz=datetime.timezone.utc)
+
         return self._record.timestamp
 
     @property
     def track_features(self) -> List[str]:
         """
         Track features are nowadays only used to downweight
         packages (ie. give them less priority).
```

### Comparing `py_rattler-0.6.1/rattler/repo_data/patch_instructions.py` & `py_rattler-0.6.2/rattler/repo_data/patch_instructions.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/repo_data/record.py` & `py_rattler-0.6.2/rattler/repo_data/record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/repo_data/repo_data.py` & `py_rattler-0.6.2/rattler/repo_data/repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/repo_data/sparse.py` & `py_rattler-0.6.2/rattler/repo_data/sparse.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/shell/shell.py` & `py_rattler-0.6.2/rattler/shell/shell.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/utils/rattler_version.py` & `py_rattler-0.6.2/rattler/utils/rattler_version.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/version/version.py` & `py_rattler-0.6.2/rattler/version/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,53 @@
         >>> Version("1.5").bump_segment(5)
         Version("1.5.0.0.0.1")
         >>>
         ```
         """
         return Version._from_py_version(self._version.bump_segment(index))
 
+    def with_alpha(self) -> Version:
+        """
+        Returns a new version where the last segment of this version has
+        been bumped with an alpha character. If the last segment contains a
+        character, nothing is added.
+
+        Examples
+        --------
+        ```python
+        >>> v = Version('1.0')
+        >>> v.with_alpha()
+        Version("1.0.0a0")
+        >>> v = Version('1.0.f')
+        >>> v.with_alpha()
+        Version("1.0.f")
+        >>>
+        ```
+        """
+        return Version._from_py_version(self._version.with_alpha())
+
+    def remove_local(self) -> Version:
+        """
+        Returns a new version where the local segment of the version has been removed.
+        Leaves the version unchanged if it does not have a local segment.
+
+        Examples
+        --------
+        ```python
+        >>> v = Version('1.0+3.4')
+        >>> v.remove_local()
+        Version("1.0")
+        >>> v = Version('1.0')
+        >>> v.remove_local()
+        Version("1.0")
+        >>>
+        ```
+        """
+        return Version._from_py_version(self._version.remove_local())
+
     def extend_to_length(self, length: int) -> Version:
         """
         Returns a new version that is extended with `0s` to the specified length.
 
         Examples
         --------
         ```python
```

### Comparing `py_rattler-0.6.1/rattler/version/with_source.py` & `py_rattler-0.6.2/rattler/version/with_source.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/virtual_package/generic.py` & `py_rattler-0.6.2/rattler/virtual_package/generic.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/rattler/virtual_package/virtual_package.py` & `py_rattler-0.6.2/rattler/virtual_package/virtual_package.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/about_json.rs` & `py_rattler-0.6.2/src/about_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/channel/mod.rs` & `py_rattler-0.6.2/src/channel/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/error.rs` & `py_rattler-0.6.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/generic_virtual_package.rs` & `py_rattler-0.6.2/src/generic_virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/index.rs` & `py_rattler-0.6.2/src/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/index_json.rs` & `py_rattler-0.6.2/src/index_json.rs`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     pub fn subdir(&self) -> Option<String> {
         self.inner.subdir.clone()
     }
 
     /// The timestamp when this package was created
     #[getter]
     pub fn timestamp(&self) -> Option<i64> {
-        self.inner.timestamp.map(|time| time.timestamp())
+        self.inner.timestamp.map(|time| time.timestamp_millis())
     }
 
     /// Track features are nowadays only used to downweight packages (ie. give them less priority). To
     /// that effect, the number of track features is counted (number of commas) and the package is downweighted
     /// by the number of track_features.
     #[getter]
     pub fn track_features(&self) -> Vec<String> {
```

### Comparing `py_rattler-0.6.1/src/installer.rs` & `py_rattler-0.6.2/src/installer.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/lib.rs` & `py_rattler-0.6.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/lock/mod.rs` & `py_rattler-0.6.2/src/lock/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/match_spec.rs` & `py_rattler-0.6.2/src/match_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/nameless_match_spec.rs` & `py_rattler-0.6.2/src/nameless_match_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/networking/authenticated_client.rs` & `py_rattler-0.6.2/src/networking/authenticated_client.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/networking/cached_repo_data.rs` & `py_rattler-0.6.2/src/networking/cached_repo_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/networking/mod.rs` & `py_rattler-0.6.2/src/networking/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/no_arch_type.rs` & `py_rattler-0.6.2/src/no_arch_type.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/package_name.rs` & `py_rattler-0.6.2/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/paths_json.rs` & `py_rattler-0.6.2/src/paths_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/platform.rs` & `py_rattler-0.6.2/src/platform.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/prefix_paths.rs` & `py_rattler-0.6.2/src/prefix_paths.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/record.rs` & `py_rattler-0.6.2/src/record.rs`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     }
 
     /// The date this entry was created.
     #[getter]
     pub fn timestamp(&self) -> Option<i64> {
         self.as_package_record()
             .timestamp
-            .map(|time| time.timestamp())
+            .map(|time| time.timestamp_millis())
     }
 
     /// Track features are nowadays only used to downweight packages
     /// (ie. give them less priority). To that effect, the number of track
     /// features is counted (number of commas) and the package is downweighted
     /// by the number of track_features.
     #[getter]
```

### Comparing `py_rattler-0.6.1/src/repo_data/gateway.rs` & `py_rattler-0.6.2/src/repo_data/gateway.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/repo_data/mod.rs` & `py_rattler-0.6.2/src/repo_data/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/repo_data/sparse.rs` & `py_rattler-0.6.2/src/repo_data/sparse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/run_exports_json.rs` & `py_rattler-0.6.2/src/run_exports_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/shell.rs` & `py_rattler-0.6.2/src/shell.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/solver.rs` & `py_rattler-0.6.2/src/solver.rs`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 #[allow(clippy::too_many_arguments)]
 #[pyfunction]
 pub fn py_solve(
     py: Python<'_>,
     channels: Vec<PyChannel>,
     platforms: Vec<PyPlatform>,
     specs: Vec<PyMatchSpec>,
+    constraints: Vec<PyMatchSpec>,
     gateway: PyGateway,
     locked_packages: Vec<PyRecord>,
     pinned_packages: Vec<PyRecord>,
     virtual_packages: Vec<PyGenericVirtualPackage>,
     channel_priority: PyChannelPriority,
     timeout: Option<u64>,
     exclude_newer_timestamp_ms: Option<i64>,
@@ -73,14 +74,15 @@
                     .collect::<PyResult<Vec<_>>>()?,
                 pinned_packages: pinned_packages
                     .into_iter()
                     .map(TryInto::try_into)
                     .collect::<PyResult<Vec<_>>>()?,
                 virtual_packages: virtual_packages.into_iter().map(Into::into).collect(),
                 specs: specs.into_iter().map(Into::into).collect(),
+                constraints: constraints.into_iter().map(Into::into).collect(),
                 timeout: timeout.map(std::time::Duration::from_micros),
                 channel_priority: channel_priority.into(),
                 exclude_newer,
                 strategy: strategy.map_or_else(Default::default, |v| v.0),
             };
 
             Ok::<_, PyErr>(
```

### Comparing `py_rattler-0.6.1/src/version/component.rs` & `py_rattler-0.6.2/src/version/component.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/src/version/mod.rs` & `py_rattler-0.6.2/src/version/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,28 @@
         Ok(self
             .inner
             .bump(VersionBumpType::Segment(index))
             .map(Into::into)
             .map_err(PyRattlerError::from)?)
     }
 
+    /// Returns a new version where the last segment is an "alpha" segment (ie. `.0a0`)
+    pub fn with_alpha(&self) -> Self {
+        Self {
+            inner: self.inner.with_alpha().into_owned(),
+        }
+    }
+
+    /// Returns a new version where the local segment is removed (e.g. `1.0+local` -> `1.0`)
+    pub fn remove_local(&self) -> Self {
+        Self {
+            inner: self.inner.remove_local().into_owned(),
+        }
+    }
+
     /// Compute the hash of the version.
     fn __hash__(&self) -> u64 {
         let mut hasher = DefaultHasher::new();
         self.inner.hash(&mut hasher);
         hasher.finish()
     }
```

### Comparing `py_rattler-0.6.1/src/virtual_package.rs` & `py_rattler-0.6.2/src/virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/tests/conftest.py` & `py_rattler-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/tests/unit/test_fetch_repo_data.py` & `py_rattler-0.6.2/tests/unit/test_fetch_repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/tests/unit/test_index.py` & `py_rattler-0.6.2/tests/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/tests/unit/test_install.py` & `py_rattler-0.6.2/tests/unit/test_install.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/tests/unit/test_prefix_record.py` & `py_rattler-0.6.2/tests/unit/test_prefix_record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/tests/unit/test_solver.py` & `py_rattler-0.6.2/tests/unit/test_solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,7 +118,23 @@
     assert isinstance(solved_data[0], RepoDataRecord)
     assert (
             list(filter(lambda r: r.file_name.startswith("pytorch-cpu-0.4.1-py36_cpu_1"),
                         solved_data))[0].channel
             == pytorch_channel.base_url
     )
     assert len(solved_data) == 32
+
+@pytest.mark.asyncio
+async def test_solve_constraints(gateway: Gateway, dummy_channel: Channel) -> None:
+    solved_data = await solve(
+        [dummy_channel],
+        ["foobar"],
+        constraints=["bors <=1", "nonexisting"],
+        platforms=["linux-64"],
+        gateway=gateway,
+    )
+
+    assert isinstance(solved_data, list)
+    assert len(solved_data) == 2
+
+    assert solved_data[0].file_name == "foobar-2.1-bla_1.tar.bz2"
+    assert solved_data[1].file_name == "bors-1.0-bla_1.tar.bz2"
```

### Comparing `py_rattler-0.6.1/tests/unit/test_version.py` & `py_rattler-0.6.2/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.6.1/Cargo.lock` & `py_rattler-0.6.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,27 @@
  "cfg-if",
  "cipher",
  "cpufeatures",
  "opaque-debug",
 ]
 
 [[package]]
+name = "ahash"
+version = "0.8.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
+dependencies = [
+ "cfg-if",
+ "getrandom",
+ "once_cell",
+ "version_check",
+ "zerocopy",
+]
+
+[[package]]
 name = "aho-corasick"
 version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
@@ -2345,15 +2358,15 @@
  "smartstring",
  "thiserror",
  "unicase",
 ]
 
 [[package]]
 name = "py-rattler"
-version = "0.6.1"
+version = "0.6.2"
 dependencies = [
  "anyhow",
  "chrono",
  "futures",
  "openssl",
  "pep508_rs",
  "pyo3",
@@ -2517,15 +2530,15 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rattler"
-version = "0.26.1"
+version = "0.26.2"
 dependencies = [
  "anyhow",
  "bytes",
  "chrono",
  "console",
  "digest",
  "dirs",
@@ -2558,15 +2571,15 @@
  "tracing",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "rattler_conda_types"
-version = "0.25.0"
+version = "0.25.1"
 dependencies = [
  "chrono",
  "file_url",
  "fxhash",
  "glob",
  "hex",
  "itertools 0.12.1",
@@ -2601,28 +2614,28 @@
  "serde_with",
  "sha2",
  "tokio",
 ]
 
 [[package]]
 name = "rattler_index"
-version = "0.19.14"
+version = "0.19.15"
 dependencies = [
  "fs-err",
  "rattler_conda_types",
  "rattler_digest",
  "rattler_package_streaming",
  "serde_json",
  "tracing",
  "walkdir",
 ]
 
 [[package]]
 name = "rattler_lock"
-version = "0.22.9"
+version = "0.22.10"
 dependencies = [
  "chrono",
  "file_url",
  "fxhash",
  "indexmap 2.2.6",
  "itertools 0.12.1",
  "pep440_rs",
@@ -2674,15 +2687,15 @@
  "thiserror",
  "tracing",
  "url",
 ]
 
 [[package]]
 name = "rattler_package_streaming"
-version = "0.21.1"
+version = "0.21.2"
 dependencies = [
  "bzip2",
  "chrono",
  "futures-util",
  "num_cpus",
  "rattler_conda_types",
  "rattler_digest",
@@ -2698,15 +2711,15 @@
  "url",
  "zip",
  "zstd",
 ]
 
 [[package]]
 name = "rattler_repodata_gateway"
-version = "0.20.3"
+version = "0.20.4"
 dependencies = [
  "anyhow",
  "async-compression",
  "async-trait",
  "blake2",
  "bytes",
  "cache_control",
@@ -2748,30 +2761,30 @@
  "url",
  "windows-sys 0.52.0",
  "zstd",
 ]
 
 [[package]]
 name = "rattler_shell"
-version = "0.20.6"
+version = "0.20.7"
 dependencies = [
  "enum_dispatch",
  "indexmap 2.2.6",
  "itertools 0.12.1",
  "rattler_conda_types",
  "serde_json",
  "shlex",
  "tempfile",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "rattler_solve"
-version = "0.23.1"
+version = "0.24.0"
 dependencies = [
  "chrono",
  "futures",
  "itertools 0.12.1",
  "rattler_conda_types",
  "rattler_digest",
  "resolvo",
@@ -2779,15 +2792,15 @@
  "thiserror",
  "tracing",
  "url",
 ]
 
 [[package]]
 name = "rattler_virtual_packages"
-version = "0.19.13"
+version = "0.19.14"
 dependencies = [
  "archspec",
  "libloading",
  "nom",
  "once_cell",
  "plist",
  "rattler_conda_types",
@@ -2971,18 +2984,19 @@
  "serde",
  "thiserror",
  "tower-service",
 ]
 
 [[package]]
 name = "resolvo"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d299d168910c5d71f3c0f5441abe38ca4a6ae21f70fae909bfc6bead28f6620f"
+checksum = "e7b73dc355efbb88c372550b92bf17d36bf555ecf319a4783a5b8b7c34488bc5"
 dependencies = [
+ "ahash",
  "bitvec",
  "elsa",
  "event-listener 5.3.0",
  "futures",
  "itertools 0.13.0",
  "petgraph",
  "tracing",
@@ -4444,14 +4458,34 @@
 dependencies = [
  "serde",
  "static_assertions",
  "zvariant",
 ]
 
 [[package]]
+name = "zerocopy"
+version = "0.7.34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
+dependencies = [
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.7.34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.66",
+]
+
+[[package]]
 name = "zeroize"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ced3678a2879b30306d323f4542626697a464a97c0a07c9aebf7ebca65cd4dde"
 
 [[package]]
 name = "zip"
```

### Comparing `py_rattler-0.6.1/PKG-INFO` & `py_rattler-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-rattler
-Version: 0.6.1
+Version: 0.6.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-rattler Version: 0.6.1 Classifier: Development
+Metadata-Version: 2.1 Name: py-rattler Version: 0.6.2 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed License-File: LICENSE Summary: A blazing fast
 library to work with the conda ecosystem Author-email: Bas Zalmstra
 gmail.com>, Tarun Pratap Singh
```

