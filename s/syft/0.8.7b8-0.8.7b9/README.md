# Comparing `tmp/syft-0.8.7b8.tar.gz` & `tmp/syft-0.8.7b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.7b8.tar", last modified: Sun May 26 12:36:35 2024, max compression
+gzip compressed data, was "syft-0.8.7b9.tar", last modified: Tue May 28 06:40:27 2024, max compression
```

## Comparing `syft-0.8.7b8.tar` & `syft-0.8.7b9.tar`

### file list

```diff
@@ -1,335 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.151306 syft-0.8.7b8/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-26 12:33:03.000000 syft-0.8.7b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-26 12:33:03.000000 syft-0.8.7b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-26 12:36:35.151306 syft-0.8.7b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-05-26 12:34:23.000000 syft-0.8.7b8/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    16925 2024-05-26 12:33:03.000000 syft-0.8.7b8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-26 12:33:03.000000 syft-0.8.7b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-26 12:36:35.151306 syft-0.8.7b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-26 12:33:03.000000 syft-0.8.7b8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.087306 syft-0.8.7b8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-26 12:33:57.000000 syft-0.8.7b8/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-26 12:33:57.000000 syft-0.8.7b8/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.087306 syft-0.8.7b8/src/syft/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/itables.css
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)    41577 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/css/tabulator_pysyft.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/img/
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/jinja/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/jinja/table.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.095306 syft-0.8.7b8/src/syft/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/js/table.js
--rw-r--r--   0 runner    (1001) docker     (127)   437328 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/js/tabulator.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.099306 syft-0.8.7b8/src/syft/assets/svg/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/copy.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/folder.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/request.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/search.svg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/assets/svg/table.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.099306 syft-0.8.7b8/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.103306 syft-0.8.7b8/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47324 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37620 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/sync_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.103306 syft-0.8.7b8/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    65150 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/node/worker_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/orchestra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.107306 syft-0.8.7b8/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/protocol/releases/0.8.6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.111306 syft-0.8.7b8/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/third_party.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/serde/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.111306 syft-0.8.7b8/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    74426 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/api/
--rw-r--r--   0 runner    (1001) docker     (127)    24157 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/api/api_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/api/api_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/attestation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/attestation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/attestation/attestation_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/attestation/attestation_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.115306 syft-0.8.7b8/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    57343 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    26547 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27907 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.119306 syft-0.8.7b8/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/html_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    31391 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/association_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/network/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.123306 syft-0.8.7b8/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28215 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.127306 syft-0.8.7b8/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50857 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58990 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/resolve_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.131306 syft-0.8.7b8/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21714 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/user/user_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.135306 syft-0.8.7b8/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    21379 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.139306 syft-0.8.7b8/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.139306 syft-0.8.7b8/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    26625 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    36893 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.143306 syft-0.8.7b8/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/cache_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    30658 2024-05-26 12:35:37.000000 syft-0.8.7b8/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.143306 syft-0.8.7b8/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.147306 syft-0.8.7b8/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.147306 syft-0.8.7b8/src/syft/util/notebook_ui/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/table_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/components/tabulator_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/notebook_ui/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-26 12:33:03.000000 syft-0.8.7b8/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:36:35.147306 syft-0.8.7b8/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:33:58.000000 syft-0.8.7b8/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 12:36:35.000000 syft-0.8.7b8/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.364268 syft-0.8.7b9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-05-28 06:37:12.000000 syft-0.8.7b9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 06:37:12.000000 syft-0.8.7b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-05-28 06:40:27.360267 syft-0.8.7b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18142 2024-05-28 06:38:26.000000 syft-0.8.7b9/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16925 2024-05-28 06:37:11.000000 syft-0.8.7b9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 06:37:12.000000 syft-0.8.7b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-28 06:40:27.364268 syft-0.8.7b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 06:37:12.000000 syft-0.8.7b9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.296268 syft-0.8.7b9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.304268 syft-0.8.7b9/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 06:38:01.000000 syft-0.8.7b9/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-28 06:38:01.000000 syft-0.8.7b9/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.296268 syft-0.8.7b9/src/syft/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.304268 syft-0.8.7b9/src/syft/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/css/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/css/itables.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    46125 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/css/tabulator_pysyft.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.304268 syft-0.8.7b9/src/syft/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.304268 syft-0.8.7b9/src/syft/assets/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/jinja/table.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.304268 syft-0.8.7b9/src/syft/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/js/table.js
+-rw-r--r--   0 runner    (1001) docker     (127)   437328 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/js/tabulator.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.308267 syft-0.8.7b9/src/syft/assets/svg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/request.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/search.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/assets/svg/table.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.308267 syft-0.8.7b9/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.312268 syft-0.8.7b9/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47324 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37620 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/sync_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.312268 syft-0.8.7b9/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.312268 syft-0.8.7b9/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.316268 syft-0.8.7b9/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65150 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/node/worker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/orchestra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.316268 syft-0.8.7b9/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    24797 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.316268 syft-0.8.7b9/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/protocol/releases/0.8.6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.320268 syft-0.8.7b9/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/serde/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.320268 syft-0.8.7b9/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.324267 syft-0.8.7b9/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74426 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39167 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.324267 syft-0.8.7b9/src/syft/service/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    24157 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/api/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/api/api_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.324267 syft-0.8.7b9/src/syft/service/attestation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/attestation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/attestation/attestation_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/attestation/attestation_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.324267 syft-0.8.7b9/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.328267 syft-0.8.7b9/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57343 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26547 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.328267 syft-0.8.7b9/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.328267 syft-0.8.7b9/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.328267 syft-0.8.7b9/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28097 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.328267 syft-0.8.7b9/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.328267 syft-0.8.7b9/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/job/html_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31391 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.328267 syft-0.8.7b9/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.332268 syft-0.8.7b9/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.332268 syft-0.8.7b9/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/network/association_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/network/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/network/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.332268 syft-0.8.7b9/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.332268 syft-0.8.7b9/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.332268 syft-0.8.7b9/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.336268 syft-0.8.7b9/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.336268 syft-0.8.7b9/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28215 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.336268 syft-0.8.7b9/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.336268 syft-0.8.7b9/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.336268 syft-0.8.7b9/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51946 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16942 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.340268 syft-0.8.7b9/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.340268 syft-0.8.7b9/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26830 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/sync/resolve_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.340268 syft-0.8.7b9/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21714 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/user/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.344267 syft-0.8.7b9/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25813 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.344267 syft-0.8.7b9/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.348268 syft-0.8.7b9/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26625 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36893 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.348268 syft-0.8.7b9/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30658 2024-05-28 06:39:29.000000 syft-0.8.7b9/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.352268 syft-0.8.7b9/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.352268 syft-0.8.7b9/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.356268 syft-0.8.7b9/src/syft/util/notebook_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/components/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/components/table_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/components/tabulator_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/notebook_ui/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-28 06:37:12.000000 syft-0.8.7b9/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:40:27.356268 syft-0.8.7b9/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-05-28 06:40:27.000000 syft-0.8.7b9/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-05-28 06:40:27.000000 syft-0.8.7b9/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:40:27.000000 syft-0.8.7b9/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 06:40:27.000000 syft-0.8.7b9/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:38:02.000000 syft-0.8.7b9/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 06:40:27.000000 syft-0.8.7b9/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 06:40:27.000000 syft-0.8.7b9/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.7b8/LICENSE` & `syft-0.8.7b9/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/PKG-INFO` & `syft-0.8.7b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b8
+Version: 0.8.7b9
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -15,15 +15,14 @@
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: bcrypt==4.1.2
 Requires-Dist: boto3==1.34.56
 Requires-Dist: forbiddenfruit==0.1.4
 Requires-Dist: loguru==0.7.2
-Requires-Dist: networkx==3.2.1
 Requires-Dist: packaging>=23.0
 Requires-Dist: pyarrow==15.0.0
 Requires-Dist: pycapnp==2.0.0b2
 Requires-Dist: pydantic[email]==2.6.0
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pymongo==4.6.2
 Requires-Dist: pynacl==1.5.0
```

### Comparing `syft-0.8.7b8/PYPI.md` & `syft-0.8.7b9/PYPI.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/README.md` & `syft-0.8.7b9/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/setup.cfg` & `syft-0.8.7b9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.7-beta.8"
+version = attr: "0.8.7-beta.9"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -24,15 +24,14 @@
 	=src
 syft = 
 	setuptools
 	bcrypt==4.1.2
 	boto3==1.34.56
 	forbiddenfruit==0.1.4
 	loguru==0.7.2
-	networkx==3.2.1
 	packaging>=23.0
 	pyarrow==15.0.0
 	pycapnp==2.0.0b2
 	pydantic[email]==2.6.0
 	pydantic-settings==2.2.1
 	pymongo==4.6.2
 	pynacl==1.5.0
```

### Comparing `syft-0.8.7b8/src/syft/VERSION` & `syft-0.8.7b9/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.7-beta.8"
+__version__ = "0.8.7-beta.9"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.7b8/src/syft/__init__.py` & `syft-0.8.7b9/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.7-beta.8"
+__version__ = "0.8.7-beta.9"
 
 # stdlib
 from collections.abc import Callable
 import pathlib
 from pathlib import Path
 import sys
 from types import MethodType
@@ -21,14 +21,15 @@
 from .client.registry import EnclaveRegistry  # noqa: F401
 from .client.registry import NetworkRegistry  # noqa: F401
 from .client.search import Search  # noqa: F401
 from .client.search import SearchResults  # noqa: F401
 from .client.user_settings import UserSettings  # noqa: F401
 from .client.user_settings import settings  # noqa: F401
 from .custom_worker.config import DockerWorkerConfig  # noqa: F401
+from .custom_worker.config import PrebuiltWorkerConfig  # noqa: F401
 from .node.credentials import SyftSigningKey  # noqa: F401
 from .node.domain import Domain  # noqa: F401
 from .node.enclave import Enclave  # noqa: F401
 from .node.gateway import Gateway  # noqa: F401
 from .node.server import serve_node  # noqa: F401
 from .node.server import serve_node as bind_worker  # noqa: F401
 from .node.worker import Worker  # noqa: F401
```

### Comparing `syft-0.8.7b8/src/syft/abstract_node.py` & `syft-0.8.7b9/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/css/fonts.css` & `syft-0.8.7b9/src/syft/assets/css/fonts.css`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/css/style.css` & `syft-0.8.7b9/src/syft/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/img/logo.png` & `syft-0.8.7b9/src/syft/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/img/small-grid-symbol-logo.png` & `syft-0.8.7b9/src/syft/assets/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/jinja/table.jinja2` & `syft-0.8.7b9/src/syft/assets/jinja/table.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -34,18 +34,21 @@
   </div>
 </div>
 <div id="table-{{ uid }}"></div>
 
 <script type="application/javascript">
   {{ js | safe }}
 
-  buildTable(
+  table_{{ uid }} = buildTable(
     {{ columns | safe }},
     {{ row_header | safe }},
     {{ data | safe }},
-    "{{ uid }}"
+    "{{ uid }}",
+    pagination={{ pagination }},
+    maxHeight={{ max_height }},
+    headerSort={{ header_sort }},
   )
 </script>
 
 <style>
   {{ css | safe }}
 </style>
```

### Comparing `syft-0.8.7b8/src/syft/assets/js/tabulator.min.js` & `syft-0.8.7b9/src/syft/assets/js/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/arrow.svg` & `syft-0.8.7b9/src/syft/assets/svg/arrow.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/clipboard.svg` & `syft-0.8.7b9/src/syft/assets/svg/clipboard.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/copy.svg` & `syft-0.8.7b9/src/syft/assets/svg/copy.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/folder.svg` & `syft-0.8.7b9/src/syft/assets/svg/folder.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/info.svg` & `syft-0.8.7b9/src/syft/assets/svg/info.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/request.svg` & `syft-0.8.7b9/src/syft/assets/svg/request.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/search.svg` & `syft-0.8.7b9/src/syft/assets/svg/search.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/assets/svg/table.svg` & `syft-0.8.7b9/src/syft/assets/svg/table.svg`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/api.py` & `syft-0.8.7b9/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/client.py` & `syft-0.8.7b9/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/connection.py` & `syft-0.8.7b9/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/domain_client.py` & `syft-0.8.7b9/src/syft/client/domain_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/enclave_client.py` & `syft-0.8.7b9/src/syft/client/enclave_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/gateway_client.py` & `syft-0.8.7b9/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/registry.py` & `syft-0.8.7b9/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/search.py` & `syft-0.8.7b9/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/sync_decision.py` & `syft-0.8.7b9/src/syft/client/sync_decision.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/client/syncing.py` & `syft-0.8.7b9/src/syft/client/syncing.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ..abstract_node import NodeSideType
 from ..node.credentials import SyftVerifyKey
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.sync.diff_state import NodeDiff
 from ..service.sync.diff_state import ObjectDiffBatch
 from ..service.sync.diff_state import SyncInstruction
+from ..service.sync.resolve_widget import PaginatedResolveWidget
 from ..service.sync.resolve_widget import ResolveWidget
 from ..service.sync.sync_state import SyncState
 from ..types.uid import UID
 from ..util.decorators import deprecated
 from .client import SyftClient
 from .sync_decision import SyncDecision
 from .sync_decision import SyncDirection
@@ -67,36 +68,26 @@
         include_ignored=include_ignored,
         include_same=include_same,
         filter_by_email=filter_by_email,
         filter_by_type=filter_by_type,
     )
 
 
-def get_user_input_for_resolve() -> SyncDecision:
-    options = [x.value for x in SyncDecision]
-    options_str = ", ".join(options[:-1]) + f" or {options[-1]}"
-    print(f"How do you want to sync these objects? choose between {options_str}")
-
-    while True:
-        decision = input()
-        decision = decision.lower()
-
-        try:
-            return SyncDecision(decision)
-        except ValueError:
-            print(f"Please choose between {options_str}")
-
-
-def resolve(obj_diff_batch: ObjectDiffBatch) -> ResolveWidget:
-    widget = ResolveWidget(obj_diff_batch)
-    return widget
+def resolve(obj: ObjectDiffBatch | NodeDiff) -> ResolveWidget | PaginatedResolveWidget:
+    if not isinstance(obj, ObjectDiffBatch | NodeDiff):
+        raise ValueError(
+            f"Invalid type: could not resolve object with type {type(obj).__qualname__}"
+        )
+    return obj.resolve()
 
 
 @deprecated(reason="resolve_single has been renamed to resolve", return_syfterror=True)
-def resolve_single(obj_diff_batch: ObjectDiffBatch) -> ResolveWidget:
+def resolve_single(
+    obj_diff_batch: ObjectDiffBatch,
+) -> ResolveWidget | PaginatedResolveWidget:
     return resolve(obj_diff_batch)
 
 
 def handle_sync_batch(
     obj_diff_batch: ObjectDiffBatch,
     share_private_data: dict[UID, bool],
     mockify: dict[UID, bool],
```

### Comparing `syft-0.8.7b8/src/syft/client/user_settings.py` & `syft-0.8.7b9/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/custom_worker/builder.py` & `syft-0.8.7b9/src/syft/custom_worker/builder.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/custom_worker/builder_docker.py` & `syft-0.8.7b9/src/syft/custom_worker/builder_docker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.7b9/src/syft/custom_worker/builder_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/custom_worker/builder_types.py` & `syft-0.8.7b9/src/syft/custom_worker/builder_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/custom_worker/config.py` & `syft-0.8.7b9/src/syft/custom_worker/config.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/custom_worker/k8s.py` & `syft-0.8.7b9/src/syft/custom_worker/k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.7b9/src/syft/custom_worker/runner_k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # relative
 from .k8s import KUBERNETES_NAMESPACE
 from .k8s import KubeUtils
 from .k8s import PodStatus
 from .k8s import get_kr8s_client
 
 JSONPATH_AVAILABLE_REPLICAS = "{.status.availableReplicas}"
-CREATE_POOL_TIMEOUT_SEC = 60
+CREATE_POOL_TIMEOUT_SEC = 180
 SCALE_POOL_TIMEOUT_SEC = 60
 
 
 class KubernetesRunner:
     def __init__(self) -> None:
         self.client = get_kr8s_client()
 
@@ -56,16 +56,14 @@
             )
 
             # wait for replicas to be available and ready
             deployment.wait(
                 f"jsonpath='{JSONPATH_AVAILABLE_REPLICAS}'={replicas}",
                 timeout=CREATE_POOL_TIMEOUT_SEC,
             )
-        except Exception:
-            raise
         finally:
             if pull_secret:
                 pull_secret.delete(propagation_policy="Foreground")
 
         # return
         return deployment
```

### Comparing `syft-0.8.7b8/src/syft/custom_worker/utils.py` & `syft-0.8.7b9/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/exceptions/exception.py` & `syft-0.8.7b9/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/node/credentials.py` & `syft-0.8.7b9/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/node/node.py` & `syft-0.8.7b9/src/syft/node/node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/node/routes.py` & `syft-0.8.7b9/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/node/run.py` & `syft-0.8.7b9/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/node/server.py` & `syft-0.8.7b9/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/node/worker_settings.py` & `syft-0.8.7b9/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/orchestra.py` & `syft-0.8.7b9/src/syft/orchestra.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/protocol/data_protocol.py` & `syft-0.8.7b9/src/syft/protocol/data_protocol.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/protocol/protocol_version.json` & `syft-0.8.7b9/src/syft/protocol/protocol_version.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978260869565216%*

 * *Differences: {"'dev'": "{'object_versions': {'CreateCustomImageChange': OrderedDict([('3', "*

 * *          "OrderedDict([('version', 3), ('hash', "*

 * *          "'e5f099940a7623f145f51f3e15b97a910a1d7fda1f67739420fed3035d1f2995'), ('action', "*

 * *          "'add')]))])}}"}*

```diff
@@ -30,14 +30,21 @@
             "BlobRetrievalByURL": {
                 "5": {
                     "action": "add",
                     "hash": "4934bf72bb10ac0a670c87ab735175088274e090819436563543473e64cf15e3",
                     "version": 5
                 }
             },
+            "CreateCustomImageChange": {
+                "3": {
+                    "action": "add",
+                    "hash": "e5f099940a7623f145f51f3e15b97a910a1d7fda1f67739420fed3035d1f2995",
+                    "version": 3
+                }
+            },
             "CreateTwinAPIEndpoint": {
                 "1": {
                     "action": "add",
                     "hash": "55e0a7b0ac428a6abb771ffcb925ee79cdd752a4b83058aa4b71fbef2a9fee63",
                     "version": 1
                 }
             },
```

### Comparing `syft-0.8.7b8/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.7b9/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.7b9/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.7b9/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/protocol/releases/0.8.6.json` & `syft-0.8.7b9/src/syft/protocol/releases/0.8.6.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/array.py` & `syft-0.8.7b9/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/arrow.py` & `syft-0.8.7b9/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/deserialize.py` & `syft-0.8.7b9/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/lib_permissions.py` & `syft-0.8.7b9/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/lib_service_registry.py` & `syft-0.8.7b9/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/mock.py` & `syft-0.8.7b9/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/recursive.py` & `syft-0.8.7b9/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/recursive_primitives.py` & `syft-0.8.7b9/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/serializable.py` & `syft-0.8.7b9/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/serialize.py` & `syft-0.8.7b9/src/syft/serde/serialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/signature.py` & `syft-0.8.7b9/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/serde/third_party.py` & `syft-0.8.7b9/src/syft/serde/third_party.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from importlib.util import find_spec
 from io import BytesIO
 
 # third party
 from dateutil import parser
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
-import networkx as nx
-from networkx import DiGraph
 import numpy as np
 from pandas import DataFrame
 from pandas import Series
 from pandas._libs.tslibs.timestamps import Timestamp
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pydantic
@@ -225,32 +223,14 @@
     deserialize=lambda x: pydantic.EmailStr(x.decode()),
 )
 
 
 # how else do you import a relative file to execute it?
 NOTHING = None
 
-
-# TODO: debug serializing after updating a node
-def serialize_networkx_graph(graph: DiGraph) -> bytes:
-    graph_dict: dict = nx.node_link_data(graph)
-    return serialize(graph_dict, to_bytes=True)
-
-
-def deserialize_networkx_graph(buf: bytes) -> DiGraph:
-    graph_dict: dict = deserialize(buf, from_bytes=True)
-    return nx.node_link_graph(graph_dict)
-
-
-recursive_serde_register(
-    DiGraph,
-    serialize=serialize_networkx_graph,
-    deserialize=deserialize_networkx_graph,
-)
-
 try:
     # Just register these serializers if the google.cloud.bigquery & db_dtypes module are available
     # third party
     from google.cloud.bigquery.job.query import QueryJob
     from google.cloud.bigquery.table import RowIterator
 
     # Checking db_dtypes availability this way to avoid unused ruff issues, but this package is used internally
```

### Comparing `syft-0.8.7b8/src/syft/service/action/action_data_empty.py` & `syft-0.8.7b9/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/action_endpoint.py` & `syft-0.8.7b9/src/syft/service/action/action_endpoint.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/action_object.py` & `syft-0.8.7b9/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/action_permissions.py` & `syft-0.8.7b9/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/action_service.py` & `syft-0.8.7b9/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/action_store.py` & `syft-0.8.7b9/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/action_types.py` & `syft-0.8.7b9/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/numpy.py` & `syft-0.8.7b9/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/pandas.py` & `syft-0.8.7b9/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/plan.py` & `syft-0.8.7b9/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/action/verification.py` & `syft-0.8.7b9/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/api/api.py` & `syft-0.8.7b9/src/syft/service/api/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/api/api_service.py` & `syft-0.8.7b9/src/syft/service/api/api_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/api/api_stash.py` & `syft-0.8.7b9/src/syft/service/api/api_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/attestation/attestation_service.py` & `syft-0.8.7b9/src/syft/service/attestation/attestation_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.7b9/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/blob_storage/service.py` & `syft-0.8.7b9/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/blob_storage/stash.py` & `syft-0.8.7b9/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code/code_parse.py` & `syft-0.8.7b9/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code/status_service.py` & `syft-0.8.7b9/src/syft/service/code/status_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code/user_code.py` & `syft-0.8.7b9/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code/user_code_parse.py` & `syft-0.8.7b9/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code/user_code_service.py` & `syft-0.8.7b9/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code/user_code_stash.py` & `syft-0.8.7b9/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code/utils.py` & `syft-0.8.7b9/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code_history/code_history.py` & `syft-0.8.7b9/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code_history/code_history_service.py` & `syft-0.8.7b9/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.7b9/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/context.py` & `syft-0.8.7b9/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/data_subject/data_subject.py` & `syft-0.8.7b9/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.7b9/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.7b9/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.7b9/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/dataset/dataset.py` & `syft-0.8.7b9/src/syft/service/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from ...util.notebook_ui.styles import ITABLES_CSS
 from ..data_subject.data_subject import DataSubject
 from ..data_subject.data_subject import DataSubjectCreate
 from ..data_subject.data_subject_service import DataSubjectService
 from ..response import SyftError
 from ..response import SyftException
 from ..response import SyftSuccess
+from ..response import SyftWarning
 
 NamePartitionKey = PartitionKey(key="name", type_=str)
 
 
 @serializable()
 class Contributor(SyftObject):
     __canonical_name__ = "Contributor"
@@ -279,14 +280,18 @@
         )
         if api is None or api.services is None:
             return None
         res = api.services.action.get(self.action_id)
         if self.has_permission(res):
             return res.syft_action_data
         else:
+            warning = SyftWarning(
+                message="You do not have permission to access private data."
+            )
+            display(warning)
             return None
 
 
 def _is_action_data_empty(obj: Any) -> bool:
     # just a wrapper of action_object.is_action_data_empty
     # to work around circular import error
```

### Comparing `syft-0.8.7b8/src/syft/service/dataset/dataset_service.py` & `syft-0.8.7b9/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.7b9/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/enclave/enclave_service.py` & `syft-0.8.7b9/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/job/html_template.py` & `syft-0.8.7b9/src/syft/service/job/html_template.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/job/job_service.py` & `syft-0.8.7b9/src/syft/service/job/job_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/job/job_stash.py` & `syft-0.8.7b9/src/syft/service/job/job_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/log/log.py` & `syft-0.8.7b9/src/syft/service/log/log.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/log/log_service.py` & `syft-0.8.7b9/src/syft/service/log/log_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/log/log_stash.py` & `syft-0.8.7b9/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/metadata/metadata_service.py` & `syft-0.8.7b9/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/metadata/migrations.py` & `syft-0.8.7b9/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/metadata/node_metadata.py` & `syft-0.8.7b9/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/network/association_request.py` & `syft-0.8.7b9/src/syft/service/network/association_request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/network/network_service.py` & `syft-0.8.7b9/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/network/node_peer.py` & `syft-0.8.7b9/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/network/routes.py` & `syft-0.8.7b9/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/network/utils.py` & `syft-0.8.7b9/src/syft/service/network/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notification/email_templates.py` & `syft-0.8.7b9/src/syft/service/notification/email_templates.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notification/notification_service.py` & `syft-0.8.7b9/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notification/notification_stash.py` & `syft-0.8.7b9/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notification/notifications.py` & `syft-0.8.7b9/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notifier/notifier.py` & `syft-0.8.7b9/src/syft/service/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notifier/notifier_service.py` & `syft-0.8.7b9/src/syft/service/notifier/notifier_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.7b9/src/syft/service/notifier/notifier_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/notifier/smtp_client.py` & `syft-0.8.7b9/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.7b9/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.7b9/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/output/output_service.py` & `syft-0.8.7b9/src/syft/service/output/output_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/policy/policy.py` & `syft-0.8.7b9/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/policy/policy_service.py` & `syft-0.8.7b9/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.7b9/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/project/project.py` & `syft-0.8.7b9/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/project/project_service.py` & `syft-0.8.7b9/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/project/project_stash.py` & `syft-0.8.7b9/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/queue/base_queue.py` & `syft-0.8.7b9/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/queue/queue.py` & `syft-0.8.7b9/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/queue/queue_service.py` & `syft-0.8.7b9/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/queue/queue_stash.py` & `syft-0.8.7b9/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/queue/zmq_queue.py` & `syft-0.8.7b9/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/request/request.py` & `syft-0.8.7b9/src/syft/service/request/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from collections.abc import Callable
 from enum import Enum
 import hashlib
 import inspect
 from typing import Any
 
 # third party
+from pydantic import model_validator
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
 from ...abstract_node import NodeSideType
 from ...client.api import APIRegistry
 from ...client.client import SyftClient
+from ...custom_worker.config import DockerWorkerConfig
 from ...custom_worker.config import WorkerConfig
 from ...custom_worker.k8s import IN_KUBERNETES
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
@@ -183,77 +185,106 @@
 
     def __repr_syft_nested__(self) -> str:
         return f"Apply <b>{self.apply_permission_type}</b> to \
 <i>{self.linked_obj.object_type.__canonical_name__}:{self.linked_obj.object_uid.short()}</i>."
 
 
 @serializable()
-class CreateCustomImageChange(Change):
+class CreateCustomImageChangeV2(Change):
     __canonical_name__ = "CreateCustomImageChange"
     __version__ = SYFT_OBJECT_VERSION_2
 
     config: WorkerConfig
     tag: str
     registry_uid: UID | None = None
     pull_image: bool = True
 
     __repr_attrs__ = ["config", "tag"]
 
+
+@serializable()
+class CreateCustomImageChange(Change):
+    __canonical_name__ = "CreateCustomImageChange"
+    __version__ = SYFT_OBJECT_VERSION_3
+
+    config: WorkerConfig
+    tag: str | None = None
+    registry_uid: UID | None = None
+    pull_image: bool = True
+
+    __repr_attrs__ = ["config", "tag"]
+
+    @model_validator(mode="after")
+    def _tag_required_for_dockerworkerconfig(self) -> Self:
+        if isinstance(self.config, DockerWorkerConfig) and self.tag is None:
+            raise ValueError("`tag` is required for `DockerWorkerConfig`.")
+        return self
+
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
             worker_image_service = context.node.get_service("SyftWorkerImageService")
 
             service_context = context.to_service_ctx()
-            result = worker_image_service.submit_dockerfile(
-                service_context, docker_config=self.config
+            result = worker_image_service.submit(
+                service_context, worker_config=self.config
             )
 
             if isinstance(result, SyftError):
                 return Err(result)
 
-            result = worker_image_service.stash.get_by_docker_config(
+            result = worker_image_service.stash.get_by_worker_config(
                 service_context.credentials, config=self.config
             )
 
             if result.is_err():
                 return Err(SyftError(message=f"{result.err()}"))
 
-            worker_image = result.ok()
+            if (worker_image := result.ok()) is None:
+                return Err(SyftError(message="The worker image does not exist."))
 
-            build_result = worker_image_service.build(
-                service_context,
-                image_uid=worker_image.id,
-                tag=self.tag,
-                registry_uid=self.registry_uid,
-                pull=self.pull_image,
-            )
+            build_success_message = "Image was pre-built."
+
+            if not worker_image.is_prebuilt:
+                build_result = worker_image_service.build(
+                    service_context,
+                    image_uid=worker_image.id,
+                    tag=self.tag,
+                    registry_uid=self.registry_uid,
+                    pull=self.pull_image,
+                )
+
+                if isinstance(build_result, SyftError):
+                    return Err(build_result)
 
-            if isinstance(build_result, SyftError):
-                return Err(build_result)
+                build_success_message = build_result.message
+
+            build_success = SyftSuccess(
+                message=f"Build result: {build_success_message}"
+            )
 
-            if IN_KUBERNETES:
+            if IN_KUBERNETES and not worker_image.is_prebuilt:
                 push_result = worker_image_service.push(
                     service_context,
                     image=worker_image.id,
                     username=context.extra_kwargs.get("reg_username", None),
                     password=context.extra_kwargs.get("reg_password", None),
                 )
 
                 if isinstance(push_result, SyftError):
                     return Err(push_result)
 
                 return Ok(
                     SyftSuccess(
-                        message=f"Build Result: {build_result.message} \n Push Result: {push_result.message}"
+                        message=f"{build_success}\nPush result: {push_result.message}"
                     )
                 )
 
-            return Ok(build_result)
+            return Ok(build_success)
 
         except Exception as e:
             return Err(SyftError(message=f"Failed to create/build image: {e}"))
 
     def apply(self, context: ChangeContext) -> Result[SyftSuccess, SyftError]:
         return self._run(context=context, apply=True)
 
@@ -287,15 +318,15 @@
         # SyftError or SyftSuccess
         if apply:
             # get the worker pool service and try to launch a pool
             worker_pool_service = context.node.get_service("SyftWorkerPoolService")
             service_context: AuthedServiceContext = context.to_service_ctx()
 
             if self.config is not None:
-                result = worker_pool_service.image_stash.get_by_docker_config(
+                result = worker_pool_service.image_stash.get_by_worker_config(
                     service_context.credentials, self.config
                 )
                 if result.is_err():
                     return Err(SyftError(message=f"{result.err()}"))
                 worker_image = result.ok()
                 self.image_uid = worker_image.id
```

### Comparing `syft-0.8.7b8/src/syft/service/request/request_service.py` & `syft-0.8.7b9/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/request/request_stash.py` & `syft-0.8.7b9/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/response.py` & `syft-0.8.7b9/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/service.py` & `syft-0.8.7b9/src/syft/service/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,18 @@
             final_kwargs[param_key] = kwargs[param_key]
         elif param_key in autosplat_objs:
             final_kwargs[param_key] = autosplat_objs[param_key]
         elif not isinstance(param.default, type(Parameter.empty)):
             final_kwargs[param_key] = param.default
         else:
             raise Exception(f"Missing {param_key} not in kwargs.")
+
+    if "context":
+        final_kwargs["context"] = kwargs["context"]
+
     return (args, final_kwargs)
 
 
 def expand_signature(signature: Signature, autosplat: list[str]) -> Signature:
     new_mapping = {}
     for k, v in signature.parameters.items():
         if k in autosplat:
```

### Comparing `syft-0.8.7b8/src/syft/service/settings/settings.py` & `syft-0.8.7b9/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/settings/settings_service.py` & `syft-0.8.7b9/src/syft/service/settings/settings_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,18 +57,44 @@
         """Set a new the Node Settings"""
         result = self.stash.set(context.credentials, settings)
         if result.is_ok():
             return result
         else:
             return SyftError(message=result.err())
 
-    @service_method(path="settings.update", name="update")
+    @service_method(path="settings.update", name="update", autosplat=["settings"])
     def update(
         self, context: AuthedServiceContext, settings: NodeSettingsUpdate
     ) -> Result[SyftSuccess, SyftError]:
+        """
+        Update the Node Settings using the provided values.
+
+        Args:
+            name: Optional[str]
+                Node name
+            organization: Optional[str]
+                Organization name
+            description: Optional[str]
+                Node description
+            on_board: Optional[bool]
+                Show onboarding panel when a user logs in for the first time
+            signup_enabled: Optional[bool]
+                Enable/Disable registration
+            admin_email: Optional[str]
+                Administrator email
+            association_request_auto_approval: Optional[bool]
+
+        Returns:
+            Result[SyftSuccess, SyftError]: A result indicating the success or failure of the update operation.
+
+        Example:
+        >>> node_client.update(name='foo', organization='bar', description='baz', signup_enabled=True)
+        SyftSuccess: Settings updated successfully.
+        """
+
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             current_settings = result.ok()
             if len(current_settings) > 0:
                 new_settings = current_settings[0].model_copy(
                     update=settings.to_dict(exclude_empty=True)
                 )
@@ -135,15 +161,15 @@
         flags.CAN_REGISTER = enable
 
         method = context.node.get_service_method(SettingsService.update)
         settings = NodeSettingsUpdate(signup_enabled=enable)
 
         result = method(context=context, settings=settings)
 
-        if result.is_err():
+        if isinstance(result, SyftError):
             return SyftError(message=f"Failed to update settings: {result.err()}")
 
         message = "enabled" if enable else "disabled"
         return SyftSuccess(message=f"Registration feature successfully {message}")
 
     @service_method(
         path="settings.allow_association_request_auto_approval",
```

### Comparing `syft-0.8.7b8/src/syft/service/settings/settings_stash.py` & `syft-0.8.7b9/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/sync/diff_state.py` & `syft-0.8.7b9/src/syft/service/sync/diff_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import enum
 import html
 import operator
 import textwrap
 from typing import Any
 from typing import ClassVar
 from typing import Literal
+from typing import TYPE_CHECKING
 
 # third party
 from loguru import logger
 import pandas as pd
 from pydantic import model_validator
 from rich import box
 from rich.console import Console
@@ -34,14 +35,15 @@
 from ...types.syft_object import SyftObject
 from ...types.syft_object import short_uid
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
+from ...util.notebook_ui.components.sync import Label
 from ...util.notebook_ui.components.sync import SyncTableObject
 from ...util.notebook_ui.icons import Icon
 from ...util.notebook_ui.styles import FONT_CSS
 from ...util.notebook_ui.styles import ITABLES_CSS
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
@@ -55,14 +57,19 @@
 from ..output.output_service import ExecutionOutput
 from ..request.request import Request
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..user.user import UserView
 from .sync_state import SyncState
 
+if TYPE_CHECKING:
+    # relative
+    from .resolve_widget import PaginatedResolveWidget
+    from .resolve_widget import ResolveWidget
+
 sketchy_tab = "‎ " * 4
 
 
 class AttrDiff(SyftObject):
     # version
     __canonical_name__ = "AttrDiff"
     __version__ = SYFT_OBJECT_VERSION_2
@@ -550,14 +557,20 @@
     hierarchy_levels: list[int]
     dependencies: dict[UID, list[UID]] = {}
     dependents: dict[UID, list[UID]] = {}
     decision: SyncDecision | None = None
     root_diff: ObjectDiff
     sync_direction: SyncDirection | None
 
+    def resolve(self) -> "ResolveWidget":
+        # relative
+        from .resolve_widget import ResolveWidget
+
+        return ResolveWidget(self)
+
     def walk_graph(
         self,
         deps: dict[UID, list[UID]],
         include_roots: bool = False,
         include_batch_root: bool = True,
     ) -> list[ObjectDiff]:
         root_id = self.root_diff.object_id
@@ -700,14 +713,29 @@
     def root_id(self) -> UID:
         return self.root_diff.object_id
 
     @property
     def root_type(self) -> type:
         return self.root_diff.obj_type
 
+    def decision_badge(self) -> str:
+        if self.decision is None:
+            return ""
+        if self.decision == SyncDecision.IGNORE:
+            decision_str = "IGNORED"
+            badge_color = "label-red"
+        if self.decision == SyncDecision.SKIP:
+            decision_str = "SKIPPED"
+            badge_color = "label-gray"
+        else:
+            decision_str = "SYNCED"
+            badge_color = "label-green"
+
+        return Label(value=decision_str, label_class=badge_color).to_html()
+
     @property
     def is_ignored(self) -> bool:
         return self.decision == SyncDecision.IGNORE
 
     @property
     def is_skipped(self) -> bool:
         return self.decision == SyncDecision.SKIP
@@ -842,17 +870,18 @@
 
         if self.root_diff.high_obj is None:
             high_html = no_obj_html
         else:
             high_html = SyncTableObject(object=self.root_diff.high_obj).to_html()
 
         return {
-            "Merge status": self.status_badge(),
+            "Diff status": self.status_badge(),
             "Public Sync State": low_html,
             "Private sync state": high_html,
+            "Decision": self.decision_badge(),
         }
 
     @property
     def visual_hierarchy(self) -> tuple[type, dict]:
         # Returns
         root_obj = (
             self.root.low_obj if self.root.low_obj is not None else self.root.high_obj
@@ -1114,14 +1143,20 @@
     low_state: SyncState
     high_state: SyncState
     direction: SyncDirection | None
     filters: list[NodeDiffFilter] = []
 
     include_ignored: bool = False
 
+    def resolve(self) -> "PaginatedResolveWidget":
+        # relative
+        from .resolve_widget import PaginatedResolveWidget
+
+        return PaginatedResolveWidget(batches=self.batches)
+
     def __getitem__(self, idx: Any) -> ObjectDiffBatch:
         return self.batches[idx]
 
     @property
     def ignored_batches(self) -> list[ObjectDiffBatch]:
         return [
             batch for batch in self.all_batches if batch.decision == SyncDecision.IGNORE
```

### Comparing `syft-0.8.7b8/src/syft/service/sync/resolve_widget.py` & `syft-0.8.7b9/src/syft/service/sync/resolve_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # stdlib
+from collections.abc import Callable
 from enum import Enum
 from enum import auto
+from functools import partial
 import html
+import secrets
 from typing import Any
 from uuid import uuid4
 
 # third party
+from IPython import display
 import ipywidgets as widgets
 from ipywidgets import Button
 from ipywidgets import Checkbox
 from ipywidgets import HBox
 from ipywidgets import HTML
 from ipywidgets import Layout
 from ipywidgets import VBox
@@ -18,14 +22,17 @@
 from ...client.sync_decision import SyncDirection
 from ...types.uid import UID
 from ...util.notebook_ui.components.sync import Alert
 from ...util.notebook_ui.components.sync import CopyIDButton
 from ...util.notebook_ui.components.sync import MainDescription
 from ...util.notebook_ui.components.sync import SyncWidgetHeader
 from ...util.notebook_ui.components.sync import TypeLabel
+from ...util.notebook_ui.components.tabulator_template import build_tabulator_table
+from ...util.notebook_ui.components.tabulator_template import highlight_single_row
+from ...util.notebook_ui.components.tabulator_template import update_table_cell
 from ...util.notebook_ui.styles import CSS_CODE
 from ..action.action_object import ActionObject
 from ..api.api import TwinAPIEndpoint
 from ..log.log import SyftLog
 from ..response import SyftError
 from ..response import SyftSuccess
 from .diff_state import ObjectDiff
@@ -402,19 +409,22 @@
         self.sync = change["new"]
 
     def _on_share_private_data_change(self, change: Any) -> None:
         self.share_private_data = change["new"]
 
 
 class ResolveWidget:
-    def __init__(self, obj_diff_batch: ObjectDiffBatch):
+    def __init__(
+        self, obj_diff_batch: ObjectDiffBatch, on_sync_callback: Callable | None = None
+    ):
         self.obj_diff_batch: ObjectDiffBatch = obj_diff_batch
         self.id2widget: dict[
             UID, CollapsableObjectDiffWidget | MainObjectDiffWidget
         ] = {}
+        self.on_sync_callback = on_sync_callback
         self.main_widget = self.build()
         self.result_widget = VBox()  # Placeholder for SyftSuccess / SyftError
         self.widget = VBox(
             [self.build_css_widget(), self.main_widget, self.result_widget]
         )
         self.is_synced = False
         self.hide_result_widget()
@@ -459,14 +469,16 @@
         res = handle_sync_batch(
             obj_diff_batch=self.obj_diff_batch,
             share_private_data=self.get_share_private_data_state(),
             mockify=self.get_mockify_state(),
         )
 
         self.set_widget_result_state(res)
+        if self.on_sync_callback:
+            self.on_sync_callback()
         return res
 
     @property
     def batch_diff_widgets(self) -> list[CollapsableObjectDiffWidget]:
         dependents = self.obj_diff_batch.get_dependents(
             include_roots=False, include_batch_root=False
         )
@@ -586,7 +598,195 @@
             value='<div style="text-align: center; margin: 3px 0; border: 1px dashed #B4B0BF;"></div>',
             layout=Layout(width="100%"),
         )
 
     def build_header(self) -> HTML:
         header_html = SyncWidgetHeader(diff_batch=self.obj_diff_batch).to_html()
         return HTML(value=header_html)
+
+
+class PaginationControl:
+    def __init__(self, data: list, callback: Callable[[int], None]):
+        self.data = data
+        self.callback = callback
+        self.current_index = 0
+        self.index_label = widgets.Label(value=f"Index: {self.current_index}")
+
+        self.first_button = widgets.Button(description="First")
+        self.previous_button = widgets.Button(description="Previous")
+        self.next_button = widgets.Button(description="Next")
+        self.last_button = widgets.Button(description="Last")
+
+        self.first_button.on_click(self.go_to_first)
+        self.previous_button.on_click(self.go_to_previous)
+        self.next_button.on_click(self.go_to_next)
+        self.last_button.on_click(self.go_to_last)
+        self.output = widgets.Output()
+
+        self.buttons = widgets.HBox(
+            [
+                self.first_button,
+                self.previous_button,
+                self.next_button,
+                self.last_button,
+            ]
+        )
+        self.update_buttons()
+        self.update_index_callback()
+
+    def update_index_label(self) -> None:
+        self.index_label.value = f"Current: {self.current_index}"
+
+    def update_buttons(self) -> None:
+        self.first_button.disabled = self.current_index == 0
+        self.previous_button.disabled = self.current_index == 0
+        self.next_button.disabled = self.current_index == len(self.data) - 1
+        self.last_button.disabled = self.current_index == len(self.data) - 1
+
+    def go_to_first(self, b: Button | None) -> None:
+        self.current_index = 0
+        self.update_index_callback()
+
+    def go_to_previous(self, b: Button | None) -> None:
+        if self.current_index > 0:
+            self.current_index -= 1
+        self.update_index_callback()
+
+    def go_to_next(self, b: Button | None) -> None:
+        if self.current_index < len(self.data) - 1:
+            self.current_index += 1
+        self.update_index_callback()
+
+    def go_to_last(self, b: Button | None) -> None:
+        self.current_index = len(self.data) - 1
+        self.update_index_callback()
+
+    def update_index_callback(self) -> None:
+        self.update_index_label()
+        self.update_buttons()
+
+        # NOTE self.output is required to display IPython.display.HTML
+        # IPython.display.HTML is used to execute JS code
+        with self.output:
+            self.callback(self.current_index)
+
+    def build(self) -> widgets.VBox:
+        return widgets.VBox(
+            [widgets.HBox([self.buttons, self.index_label]), self.output]
+        )
+
+
+class PaginatedWidget:
+    def __init__(
+        self, children: list, on_paginate_callback: Callable[[int], None] | None = None
+    ):
+        # on_paginate_callback is an optional secondary callback,
+        # called after updating the page index and displaying the new widget
+        self.children = children
+        self.on_paginate_callback = on_paginate_callback
+        self.current_index = 0
+        self.container = widgets.VBox()
+
+        self.pagination_control = PaginationControl(children, self.on_paginate)
+
+        # Initial display
+        self.on_paginate(self.pagination_control.current_index)
+
+    def __getitem__(self, index: int) -> widgets.Widget:
+        return self.children[index]
+
+    def on_paginate(self, index: int) -> None:
+        self.container.children = [self.children[index]]
+        if self.on_paginate_callback:
+            self.on_paginate_callback(index)
+
+    def spacer(self, height: int) -> widgets.HTML:
+        return widgets.HTML(f"<div style='height: {height}px'></div>")
+
+    def build(self) -> widgets.VBox:
+        return widgets.VBox(
+            [self.pagination_control.build(), self.spacer(8), self.container]
+        )
+
+
+class PaginatedResolveWidget:
+    """
+    PaginatedResolveWidget is a widget that displays
+    a ResolveWidget for each ObjectDiffBatch,
+    paginated by a PaginationControl widget.
+    """
+
+    def __init__(self, batches: list[ObjectDiffBatch]):
+        self.batches = batches
+        self.resolve_widgets: list[ResolveWidget] = [
+            ResolveWidget(
+                batch,
+                on_sync_callback=partial(self.on_click_sync, i),
+            )
+            for i, batch in enumerate(self.batches)
+        ]
+
+        self.table_uid = secrets.token_hex(4)
+
+        # Disable the table pagination to avoid the double pagination buttons
+        self.batch_table = build_tabulator_table(
+            obj=batches,
+            uid=self.table_uid,
+            max_height=500,
+            pagination=False,
+            header_sort=False,
+        )
+
+        self.paginated_widget = PaginatedWidget(
+            children=[widget.widget for widget in self.resolve_widgets],
+            on_paginate_callback=self.on_paginate,
+        )
+
+        self.table_output = widgets.Output()
+        with self.table_output:
+            display.display(display.HTML(self.batch_table))
+            highlight_single_row(
+                self.table_uid, self.paginated_widget.current_index, jump_to_row=True
+            )
+
+        self.widget = self.build()
+
+    def on_click_sync(self, index: int) -> None:
+        self.update_table_sync_decision(index)
+        if self.batches[index].decision is not None:
+            self.paginated_widget.pagination_control.go_to_next(None)
+
+    def update_table_sync_decision(self, index: int) -> None:
+        new_decision = self.batches[index].decision_badge()
+        with self.table_output:
+            update_table_cell(
+                uid=self.table_uid,
+                index=index,
+                field="Decision",
+                value=new_decision,
+            )
+
+    def __getitem__(self, index: int) -> ResolveWidget:
+        return self.resolve_widgets[index]
+
+    def on_paginate(self, index: int) -> None:
+        return highlight_single_row(self.table_uid, index, jump_to_row=True)
+
+    def build(self) -> widgets.VBox:
+        return widgets.VBox([self.table_output, self.paginated_widget.build()])
+
+    def click_sync(self, index: int) -> SyftSuccess | SyftError:
+        return self.resolve_widgets[index].click_sync()
+
+    def click_share_all_private_data(self, index: int) -> None:
+        self.resolve_widgets[index].click_share_all_private_data()
+
+    def _share_all(self) -> None:
+        for widget in self.resolve_widgets:
+            widget.click_share_all_private_data()
+
+    def _sync_all(self) -> None:
+        for widget in self.resolve_widgets:
+            widget.click_sync()
+
+    def _repr_mimebundle_(self, **kwargs: dict) -> dict[str, str] | None:
+        return self.widget._repr_mimebundle_(**kwargs)
```

### Comparing `syft-0.8.7b8/src/syft/service/sync/sync_service.py` & `syft-0.8.7b9/src/syft/service/sync/sync_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/sync/sync_stash.py` & `syft-0.8.7b9/src/syft/service/sync/sync_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/sync/sync_state.py` & `syft-0.8.7b9/src/syft/service/sync/sync_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/user/user.py` & `syft-0.8.7b9/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/user/user_roles.py` & `syft-0.8.7b9/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/user/user_service.py` & `syft-0.8.7b9/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/user/user_stash.py` & `syft-0.8.7b9/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/warnings.py` & `syft-0.8.7b9/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/image_identifier.py` & `syft-0.8.7b9/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/image_registry.py` & `syft-0.8.7b9/src/syft/service/worker/image_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/image_registry_service.py` & `syft-0.8.7b9/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.7b9/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/utils.py` & `syft-0.8.7b9/src/syft/service/worker/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,14 @@
     debug: bool,
     reg_username: str | None = None,
     reg_password: str | None = None,
     reg_url: str | None = None,
     **kwargs: Any,
 ) -> list[Pod] | SyftError:
     pool = None
-    error = False
 
     try:
         print(
             "Creating new pool "
             f"name={pool_name} "
             f"tag={tag} "
             f"replicas={replicas}"
@@ -362,19 +361,22 @@
             env_vars=env_vars,
             mount_secrets=mount_secrets,
             reg_username=reg_username,
             reg_password=reg_password,
             reg_url=reg_url,
         )
     except Exception as e:
-        error = True
-        return SyftError(message=f"Failed to start workers {e}")
-    finally:
-        if error and pool:
+        if pool:
             pool.delete()
+        # stdlib
+        import traceback
+
+        return SyftError(
+            message=f"Failed to start workers {e} {e.__class__} {e.args} {traceback.format_exc()}."
+        )
 
     return runner.get_pool_pods(pool_name=pool_name)
 
 
 def scale_kubernetes_pool(
     runner: KubernetesRunner,
     pool_name: str,
@@ -560,15 +562,15 @@
     # create SyftWorkerImage from a pre-built image
     _new_image = SyftWorkerImage(
         config=worker_config,
         created_by=credentials,
         image_identifier=SyftWorkerImageIdentifier.from_str(tag),
     )
 
-    result = image_stash.get_by_docker_config(
+    result = image_stash.get_by_worker_config(
         credentials=credentials,
         config=worker_config,
     )
 
     if result.ok() is None:
         result = image_stash.set(credentials, _new_image)
         if result.is_err():
```

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker.py` & `syft-0.8.7b9/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_image.py` & `syft-0.8.7b9/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_image_service.py` & `syft-0.8.7b9/src/syft/service/worker/worker_image_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import contextlib
 
 # third party
 import docker
 import pydantic
 
 # relative
-from ...custom_worker.config import DockerWorkerConfig
+from ...custom_worker.config import PrebuiltWorkerConfig
+from ...custom_worker.config import WorkerConfig
 from ...custom_worker.k8s import IN_KUBERNETES
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...types.datetime import DateTime
 from ...types.dicttuple import DictTuple
 from ...types.uid import UID
 from ..context import AuthedServiceContext
@@ -35,24 +36,35 @@
     stash: SyftWorkerImageStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
         self.stash = SyftWorkerImageStash(store=store)
 
     @service_method(
-        path="worker_image.submit_dockerfile",
-        name="submit_dockerfile",
+        path="worker_image.submit",
+        name="submit",
         roles=DATA_OWNER_ROLE_LEVEL,
     )
-    def submit_dockerfile(
-        self, context: AuthedServiceContext, docker_config: DockerWorkerConfig
+    def submit(
+        self, context: AuthedServiceContext, worker_config: WorkerConfig
     ) -> SyftSuccess | SyftError:
+        image_identifier: SyftWorkerImageIdentifier | None = None
+        if isinstance(worker_config, PrebuiltWorkerConfig):
+            try:
+                image_identifier = SyftWorkerImageIdentifier.from_str(worker_config.tag)
+            except Exception:
+                return SyftError(
+                    f"Invalid Docker image name: {worker_config.tag}.\n"
+                    + "Please specify the image name in this format <registry>/<repo>:<tag>."
+                )
+
         worker_image = SyftWorkerImage(
-            config=docker_config,
+            config=worker_config,
             created_by=context.credentials,
+            image_identifier=image_identifier,
         )
         res = self.stash.set(context.credentials, worker_image)
 
         if res.is_err():
             return SyftError(message=res.err())
 
         return SyftSuccess(
@@ -274,18 +286,18 @@
 
     @service_method(
         path="worker_image.get_by_config",
         name="get_by_config",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def get_by_config(
-        self, context: AuthedServiceContext, docker_config: DockerWorkerConfig
+        self, context: AuthedServiceContext, worker_config: WorkerConfig
     ) -> SyftWorkerImage | SyftError:
-        res = self.stash.get_by_docker_config(
-            credentials=context.credentials, config=docker_config
+        res = self.stash.get_by_worker_config(
+            credentials=context.credentials, config=worker_config
         )
         if res.is_err():
             return SyftError(
-                message=f"Failed to get image with docker config {docker_config}. Error: {res.err()}"
+                message=f"Failed to get image with docker config {worker_config}. Error: {res.err()}"
             )
         image: SyftWorkerImage = res.ok()
         return image
```

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.7b9/src/syft/service/worker/worker_image_stash.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,26 @@
 
         # By default syft images have all read permission
         add_permissions.append(
             ActionObjectPermission(uid=obj.id, permission=ActionPermission.ALL_READ)
         )
 
         if isinstance(obj.config, DockerWorkerConfig):
-            result = self.get_by_docker_config(
+            result = self.get_by_worker_config(
                 credentials=credentials, config=obj.config
             )
             if result.is_ok() and result.ok() is not None:
                 return Err(f"Image already exists for: {obj.config}")
 
         return super().set(
             credentials,
             obj,
             add_permissions=add_permissions,
             add_storage_permission=add_storage_permission,
             ignore_duplicates=ignore_duplicates,
         )
 
-    def get_by_docker_config(
-        self, credentials: SyftVerifyKey, config: DockerWorkerConfig
+    def get_by_worker_config(
+        self, credentials: SyftVerifyKey, config: WorkerConfig
     ) -> Result[SyftWorkerImage | None, str]:
         qks = QueryKeys(qks=[WorkerConfigPK.with_obj(config)])
         return self.query_one(credentials=credentials, qks=qks)
```

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_pool.py` & `syft-0.8.7b9/src/syft/service/worker/worker_pool.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.7b9/src/syft/service/worker/worker_pool_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from typing import Any
 
 # third party
 import pydantic
 from result import OkErr
 
 # relative
-from ...custom_worker.config import CustomWorkerConfig
+from ...custom_worker.config import DockerWorkerConfig
+from ...custom_worker.config import PrebuiltWorkerConfig
 from ...custom_worker.config import WorkerConfig
 from ...custom_worker.k8s import IN_KUBERNETES
 from ...custom_worker.runner_k8s import KubernetesRunner
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.dicttuple import DictTuple
@@ -228,60 +229,70 @@
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def create_image_and_pool_request(
         self,
         context: AuthedServiceContext,
         pool_name: str,
         num_workers: int,
-        tag: str,
         config: WorkerConfig,
+        tag: str | None = None,
         registry_uid: UID | None = None,
         reason: str | None = "",
         pull_image: bool = True,
     ) -> SyftError | SyftSuccess:
         """
         Create a request to launch the worker pool based on a built image.
 
         Args:
             context (AuthedServiceContext): The authenticated service context.
             pool_name (str): The name of the worker pool.
             num_workers (int): The number of workers in the pool.
             config: (WorkerConfig): Config of the image to be built.
-            tag (str): human-readable manifest identifier that is typically a specific version or variant of an image
-            reason (Optional[str], optional): The reason for creating the worker image and pool. Defaults to "".
+            tag (str | None, optional):
+                a human-readable manifest identifier that is typically a specific version or variant of an image,
+                only needed for `DockerWorkerConfig` to tag the image after it is built.
+            reason (str | None, optional): The reason for creating the worker image and pool. Defaults to "".
         """
 
-        if isinstance(config, CustomWorkerConfig):
-            return SyftError(message="We only support DockerWorkerConfig.")
+        if not isinstance(config, DockerWorkerConfig | PrebuiltWorkerConfig):
+            return SyftError(
+                message="We only support either `DockerWorkerConfig` or `PrebuiltWorkerConfig`."
+            )
 
-        if IN_KUBERNETES and registry_uid is None:
-            return SyftError(message="Registry UID is required in Kubernetes mode.")
+        if isinstance(config, DockerWorkerConfig):
+            if tag is None:
+                return SyftError(message="`tag` is required for `DockerWorkerConfig`.")
+
+            # Validate image tag
+            try:
+                SyftWorkerImageIdentifier.from_str(tag=tag)
+            except pydantic.ValidationError as e:
+                return SyftError(message=f"Invalid `tag`: {e}.")
+
+            if IN_KUBERNETES and registry_uid is None:
+                return SyftError(
+                    message="`registry_uid` is required in Kubernetes mode for `DockerWorkerConfig`."
+                )
 
         # Check if an image already exists for given docker config
-        search_result = self.image_stash.get_by_docker_config(
+        search_result = self.image_stash.get_by_worker_config(
             credentials=context.credentials, config=config
         )
 
         if search_result.is_err():
             return SyftError(message=str(search_result.err()))
 
         worker_image: SyftWorkerImage | None = search_result.ok()
 
         if worker_image is not None:
             return SyftError(
                 message="Image already exists for given config. \
                     Please use `worker_pool.create_pool_request` to request pool creation."
             )
 
-        # Validate Image Tag
-        try:
-            SyftWorkerImageIdentifier.from_str(tag=tag)
-        except pydantic.ValidationError as e:
-            return SyftError(message=f"Failed to create tag: {e}")
-
         # create a list of Change objects and submit a
         # request for these changes for approval
         changes: list[Change] = []
 
         # Add create custom image change
         # If this change is approved, then build an image using the config
         create_custom_image_change = CreateCustomImageChange(
```

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.7b9/src/syft/service/worker/worker_pool_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_service.py` & `syft-0.8.7b9/src/syft/service/worker/worker_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/service/worker/worker_stash.py` & `syft-0.8.7b9/src/syft/service/worker/worker_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/blob_storage/__init__.py` & `syft-0.8.7b9/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.7b9/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.7b9/src/syft/store/blob_storage/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/dict_document_store.py` & `syft-0.8.7b9/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/document_store.py` & `syft-0.8.7b9/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/kv_document_store.py` & `syft-0.8.7b9/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/linked_obj.py` & `syft-0.8.7b9/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/locks.py` & `syft-0.8.7b9/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/mongo_client.py` & `syft-0.8.7b9/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/mongo_codecs.py` & `syft-0.8.7b9/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/mongo_document_store.py` & `syft-0.8.7b9/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/store/sqlite_document_store.py` & `syft-0.8.7b9/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/blob_storage.py` & `syft-0.8.7b9/src/syft/types/blob_storage.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/datetime.py` & `syft-0.8.7b9/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/dicttuple.py` & `syft-0.8.7b9/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/grid_url.py` & `syft-0.8.7b9/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/identity.py` & `syft-0.8.7b9/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/syft_metaclass.py` & `syft-0.8.7b9/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/syft_migration.py` & `syft-0.8.7b9/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/syft_object.py` & `syft-0.8.7b9/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/syncable_object.py` & `syft-0.8.7b9/src/syft/types/syncable_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/transforms.py` & `syft-0.8.7b9/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/twin_object.py` & `syft-0.8.7b9/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/types/uid.py` & `syft-0.8.7b9/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/_std_stream_capture.py` & `syft-0.8.7b9/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/assets.py` & `syft-0.8.7b9/src/syft/util/assets.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/autoreload.py` & `syft-0.8.7b9/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/decorators.py` & `syft-0.8.7b9/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/experimental_flags.py` & `syft-0.8.7b9/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/filterwarnings.py` & `syft-0.8.7b9/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/logger.py` & `syft-0.8.7b9/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/markdown.py` & `syft-0.8.7b9/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/notebook_ui/components/base.py` & `syft-0.8.7b9/src/syft/util/notebook_ui/components/base.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/notebook_ui/components/sync.py` & `syft-0.8.7b9/src/syft/util/notebook_ui/components/sync.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/notebook_ui/components/table_template.py` & `syft-0.8.7b9/src/syft/util/notebook_ui/components/table_template.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/notebook_ui/icons.py` & `syft-0.8.7b9/src/syft/util/notebook_ui/icons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/notebook_ui/styles.py` & `syft-0.8.7b9/src/syft/util/notebook_ui/styles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/schema.py` & `syft-0.8.7b9/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/table.py` & `syft-0.8.7b9/src/syft/util/table.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/telemetry.py` & `syft-0.8.7b9/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/trace_decorator.py` & `syft-0.8.7b9/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/util.py` & `syft-0.8.7b9/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft/util/version_compare.py` & `syft-0.8.7b9/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b8/src/syft.egg-info/PKG-INFO` & `syft-0.8.7b9/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b8
+Version: 0.8.7b9
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -15,15 +15,14 @@
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: bcrypt==4.1.2
 Requires-Dist: boto3==1.34.56
 Requires-Dist: forbiddenfruit==0.1.4
 Requires-Dist: loguru==0.7.2
-Requires-Dist: networkx==3.2.1
 Requires-Dist: packaging>=23.0
 Requires-Dist: pyarrow==15.0.0
 Requires-Dist: pycapnp==2.0.0b2
 Requires-Dist: pydantic[email]==2.6.0
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pymongo==4.6.2
 Requires-Dist: pynacl==1.5.0
```

### Comparing `syft-0.8.7b8/src/syft.egg-info/SOURCES.txt` & `syft-0.8.7b9/src/syft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,14 @@
 src/syft/service/context.py
 src/syft/service/response.py
 src/syft/service/service.py
 src/syft/service/warnings.py
 src/syft/service/action/__init__.py
 src/syft/service/action/action_data_empty.py
 src/syft/service/action/action_endpoint.py
-src/syft/service/action/action_graph.py
-src/syft/service/action/action_graph_service.py
 src/syft/service/action/action_object.py
 src/syft/service/action/action_permissions.py
 src/syft/service/action/action_service.py
 src/syft/service/action/action_store.py
 src/syft/service/action/action_types.py
 src/syft/service/action/numpy.py
 src/syft/service/action/pandas.py
```

### Comparing `syft-0.8.7b8/src/syft.egg-info/requires.txt` & `syft-0.8.7b9/src/syft.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 setuptools
 bcrypt==4.1.2
 boto3==1.34.56
 forbiddenfruit==0.1.4
 loguru==0.7.2
-networkx==3.2.1
 packaging>=23.0
 pyarrow==15.0.0
 pycapnp==2.0.0b2
 pydantic[email]==2.6.0
 pydantic-settings==2.2.1
 pymongo==4.6.2
 pynacl==1.5.0
```

