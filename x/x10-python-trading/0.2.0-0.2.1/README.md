# Comparing `tmp/x10_python_trading-0.2.0.tar.gz` & `tmp/x10_python_trading-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x10_python_trading-0.2.0.tar", max compression
+gzip compressed data, was "x10_python_trading-0.2.1.tar", max compression
```

## Comparing `x10_python_trading-0.2.0.tar` & `x10_python_trading-0.2.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     7819 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/README.md
--rw-r--r--   0        0        0     1541 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/__init__.py
--rw-r--r--   0        0        0     3945 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/README.md
--rw-r--r--   0        0        0        0 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/__init__.py
--rw-r--r--   0        0        0     1840 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/fast_pedersen_hash.py
--rw-r--r--   0        0        0     3627 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/math_utils.py
--rw-r--r--   0        0        0     6074 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
--rw-r--r--   0        0        0   102708 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/pedersen_params.json
--rw-r--r--   0        0        0    11728 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/signature.py
--rw-r--r--   0        0        0     3759 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/src/config/assets_precomputed.json
--rw-r--r--   0        0        0    70705 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/src/config/constant_points.json
--rw-r--r--   0        0        0     3701 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/crypto/signature/src/config/keys_precomputed.json
--rw-r--r--   0        0        0     1955 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/BUILD
--rw-r--r--   0        0        0       31 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/CMakeLists.txt
--rw-r--r--   0        0        0     1254 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/CMakeLists_common.txt
--rw-r--r--   0        0        0        0 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/__init__.py
--rw-r--r--   0        0        0     1522 2024-05-17 15:29:00.974279 x10_python_trading-0.2.0/starkware/python/async_subprocess.py
--rw-r--r--   0        0        0     5946 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/expression_string.py
--rw-r--r--   0        0        0     1883 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/expression_string_test.py
--rw-r--r--   0        0        0     3938 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/fixed_point.py
--rw-r--r--   0        0        0      675 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/BUILD
--rw-r--r--   0        0        0      359 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/CMakeLists.txt
--rw-r--r--   0        0        0      812 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/client.py
--rw-r--r--   0        0        0      681 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/json_rpc/client_test.py
--rw-r--r--   0        0        0     8881 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/math_utils.py
--rw-r--r--   0        0        0     5102 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/math_utils_test.py
--rw-r--r--   0        0        0     1614 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/merkle_tree.py
--rw-r--r--   0        0        0     1796 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/object_utils.py
--rw-r--r--   0        0        0     1545 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/python_dependencies.py
--rw-r--r--   0        0        0     6247 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/random_test.py
--rw-r--r--   0        0        0     6247 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/random_test_utils.py
--rw-r--r--   0        0        0     3460 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/test_utils.py
--rw-r--r--   0        0        0     2783 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/test_utils_test.py
--rw-r--r--   0        0        0    19817 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils.py
--rw-r--r--   0        0        0      599 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils_stub_module.py
--rw-r--r--   0        0        0     1554 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils_stub_module.pyi
--rw-r--r--   0        0        0     7959 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/starkware/python/utils_test.py
--rw-r--r--   0        0        0        0 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/__init__.py
--rw-r--r--   0        0        0      429 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/config.py
--rw-r--r--   0        0        0       36 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/errors.py
--rw-r--r--   0        0        0        0 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/__init__.py
--rw-r--r--   0        0        0     1575 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/accounts.py
--rw-r--r--   0        0        0     1618 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/amounts.py
--rw-r--r--   0        0        0     1120 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/assets.py
--rw-r--r--   0        0        0      347 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/balances.py
--rw-r--r--   0        0        0      427 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/configuration.py
--rw-r--r--   0        0        0      327 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/fees.py
--rw-r--r--   0        0        0      459 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/funding_rates.py
--rw-r--r--   0        0        0     2744 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/markets.py
--rw-r--r--   0        0        0     4461 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/order_object.py
--rw-r--r--   0        0        0      739 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/orderbooks.py
--rw-r--r--   0        0        0     3058 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/orders.py
--rw-r--r--   0        0        0     1069 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/positions.py
--rw-r--r--   0        0        0     4227 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/simple_client/simple_trading_client.py
--rw-r--r--   0        0        0       99 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/stream_client/__init__.py
--rw-r--r--   0        0        0     2974 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/stream_client/perpetual_stream_connection.py
--rw-r--r--   0        0        0     2497 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/stream_client/stream_client.py
--rw-r--r--   0        0        0     1271 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trades.py
--rw-r--r--   0        0        0      102 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/__init__.py
--rw-r--r--   0        0        0     5214 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/account_module.py
--rw-r--r--   0        0        0      636 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/base_module.py
--rw-r--r--   0        0        0     1499 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/markets_information_module.py
--rw-r--r--   0        0        0     2353 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/order_management_module.py
--rw-r--r--   0        0        0     2953 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/perpetual/trading_client/trading_client.py
--rw-r--r--   0        0        0        0 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/__init__.py
--rw-r--r--   0        0        0      246 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/date.py
--rw-r--r--   0        0        0     5981 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/http.py
--rw-r--r--   0        0        0       79 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/log.py
--rw-r--r--   0        0        0     2336 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/model.py
--rw-r--r--   0        0        0    14980 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/starkex.py
--rw-r--r--   0        0        0      275 2024-05-17 15:29:00.978279 x10_python_trading-0.2.0/x10/utils/string.py
--rw-r--r--   0        0        0     8773 1970-01-01 00:00:00.000000 x10_python_trading-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7819 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/README.md
+-rw-r--r--   0        0        0     1541 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/__init__.py
+-rw-r--r--   0        0        0     3945 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/__init__.py
+-rw-r--r--   0        0        0     1840 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/fast_pedersen_hash.py
+-rw-r--r--   0        0        0     3627 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/math_utils.py
+-rw-r--r--   0        0        0     6074 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/nothing_up_my_sleeve_gen.py
+-rw-r--r--   0        0        0   102708 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/pedersen_params.json
+-rw-r--r--   0        0        0    11728 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/signature.py
+-rw-r--r--   0        0        0     3759 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/src/config/assets_precomputed.json
+-rw-r--r--   0        0        0    70705 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/src/config/constant_points.json
+-rw-r--r--   0        0        0     3701 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/crypto/signature/src/config/keys_precomputed.json
+-rw-r--r--   0        0        0     1955 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/python/BUILD
+-rw-r--r--   0        0        0       31 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/python/CMakeLists.txt
+-rw-r--r--   0        0        0     1254 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/python/CMakeLists_common.txt
+-rw-r--r--   0        0        0        0 2024-06-03 10:22:14.352589 x10_python_trading-0.2.1/starkware/python/__init__.py
+-rw-r--r--   0        0        0     1522 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/async_subprocess.py
+-rw-r--r--   0        0        0     5946 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/expression_string.py
+-rw-r--r--   0        0        0     1883 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/expression_string_test.py
+-rw-r--r--   0        0        0     3938 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/fixed_point.py
+-rw-r--r--   0        0        0      675 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/json_rpc/BUILD
+-rw-r--r--   0        0        0      359 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/json_rpc/CMakeLists.txt
+-rw-r--r--   0        0        0      812 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/json_rpc/client.py
+-rw-r--r--   0        0        0      681 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/json_rpc/client_test.py
+-rw-r--r--   0        0        0     8881 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/math_utils.py
+-rw-r--r--   0        0        0     5102 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/math_utils_test.py
+-rw-r--r--   0        0        0     1614 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/merkle_tree.py
+-rw-r--r--   0        0        0     1796 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/object_utils.py
+-rw-r--r--   0        0        0     1545 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/python_dependencies.py
+-rw-r--r--   0        0        0     6247 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/random_test.py
+-rw-r--r--   0        0        0     6247 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/random_test_utils.py
+-rw-r--r--   0        0        0     3460 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/test_utils.py
+-rw-r--r--   0        0        0     2783 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/test_utils_test.py
+-rw-r--r--   0        0        0    19817 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/utils.py
+-rw-r--r--   0        0        0      599 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/utils_stub_module.py
+-rw-r--r--   0        0        0     1554 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/utils_stub_module.pyi
+-rw-r--r--   0        0        0     7959 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/starkware/python/utils_test.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/__init__.py
+-rw-r--r--   0        0        0      429 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/config.py
+-rw-r--r--   0        0        0       36 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/errors.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/__init__.py
+-rw-r--r--   0        0        0     1575 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/accounts.py
+-rw-r--r--   0        0        0     1618 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/amounts.py
+-rw-r--r--   0        0        0     1120 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/assets.py
+-rw-r--r--   0        0        0      347 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/balances.py
+-rw-r--r--   0        0        0      427 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/configuration.py
+-rw-r--r--   0        0        0      327 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/fees.py
+-rw-r--r--   0        0        0      459 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/funding_rates.py
+-rw-r--r--   0        0        0     2744 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/markets.py
+-rw-r--r--   0        0        0     4461 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/order_object.py
+-rw-r--r--   0        0        0      739 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/orderbooks.py
+-rw-r--r--   0        0        0     3058 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/orders.py
+-rw-r--r--   0        0        0     1069 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/positions.py
+-rw-r--r--   0        0        0     4227 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/simple_client/simple_trading_client.py
+-rw-r--r--   0        0        0       99 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/stream_client/__init__.py
+-rw-r--r--   0        0        0     2974 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/stream_client/perpetual_stream_connection.py
+-rw-r--r--   0        0        0     2497 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/stream_client/stream_client.py
+-rw-r--r--   0        0        0     1271 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/trades.py
+-rw-r--r--   0        0        0      102 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/trading_client/__init__.py
+-rw-r--r--   0        0        0     5504 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/trading_client/account_module.py
+-rw-r--r--   0        0        0      964 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/trading_client/base_module.py
+-rw-r--r--   0        0        0     1660 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/trading_client/markets_information_module.py
+-rw-r--r--   0        0        0     2465 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/trading_client/order_management_module.py
+-rw-r--r--   0        0        0     3019 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/perpetual/trading_client/trading_client.py
+-rw-r--r--   0        0        0        0 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/utils/__init__.py
+-rw-r--r--   0        0        0      246 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/utils/date.py
+-rw-r--r--   0        0        0     5795 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/utils/http.py
+-rw-r--r--   0        0        0       79 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/utils/log.py
+-rw-r--r--   0        0        0     2336 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/utils/model.py
+-rw-r--r--   0        0        0    14980 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/utils/starkex.py
+-rw-r--r--   0        0        0      275 2024-06-03 10:22:14.356589 x10_python_trading-0.2.1/x10/utils/string.py
+-rw-r--r--   0        0        0     8773 1970-01-01 00:00:00.000000 x10_python_trading-0.2.1/PKG-INFO
```

### Comparing `x10_python_trading-0.2.0/README.md` & `x10_python_trading-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/pyproject.toml` & `x10_python_trading-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x10-python-trading"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python client for X10 API"
 authors = ["X10 <tech@ex10.org>"]
 packages = [
     { include = "starkware" },
     { include = "x10" },
 ]
 readme = "README.md"
```

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/README.md` & `x10_python_trading-0.2.1/starkware/crypto/signature/README.md`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/fast_pedersen_hash.py` & `x10_python_trading-0.2.1/starkware/crypto/signature/fast_pedersen_hash.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/math_utils.py` & `x10_python_trading-0.2.1/starkware/crypto/signature/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/nothing_up_my_sleeve_gen.py` & `x10_python_trading-0.2.1/starkware/crypto/signature/nothing_up_my_sleeve_gen.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/pedersen_params.json` & `x10_python_trading-0.2.1/starkware/crypto/signature/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/signature.py` & `x10_python_trading-0.2.1/starkware/crypto/signature/signature.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/src/config/assets_precomputed.json` & `x10_python_trading-0.2.1/starkware/crypto/signature/src/config/assets_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/src/config/constant_points.json` & `x10_python_trading-0.2.1/starkware/crypto/signature/src/config/constant_points.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/crypto/signature/src/config/keys_precomputed.json` & `x10_python_trading-0.2.1/starkware/crypto/signature/src/config/keys_precomputed.json`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/BUILD` & `x10_python_trading-0.2.1/starkware/python/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/CMakeLists_common.txt` & `x10_python_trading-0.2.1/starkware/python/CMakeLists_common.txt`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/async_subprocess.py` & `x10_python_trading-0.2.1/starkware/python/async_subprocess.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/expression_string.py` & `x10_python_trading-0.2.1/starkware/python/expression_string.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/expression_string_test.py` & `x10_python_trading-0.2.1/starkware/python/expression_string_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/fixed_point.py` & `x10_python_trading-0.2.1/starkware/python/fixed_point.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/json_rpc/BUILD` & `x10_python_trading-0.2.1/starkware/python/json_rpc/BUILD`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/json_rpc/client.py` & `x10_python_trading-0.2.1/starkware/python/json_rpc/client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/json_rpc/client_test.py` & `x10_python_trading-0.2.1/starkware/python/json_rpc/client_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/math_utils.py` & `x10_python_trading-0.2.1/starkware/python/math_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/math_utils_test.py` & `x10_python_trading-0.2.1/starkware/python/math_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/merkle_tree.py` & `x10_python_trading-0.2.1/starkware/python/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/object_utils.py` & `x10_python_trading-0.2.1/starkware/python/object_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/python_dependencies.py` & `x10_python_trading-0.2.1/starkware/python/python_dependencies.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/random_test.py` & `x10_python_trading-0.2.1/starkware/python/random_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/random_test_utils.py` & `x10_python_trading-0.2.1/starkware/python/random_test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/test_utils.py` & `x10_python_trading-0.2.1/starkware/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/test_utils_test.py` & `x10_python_trading-0.2.1/starkware/python/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/utils.py` & `x10_python_trading-0.2.1/starkware/python/utils.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/utils_stub_module.py` & `x10_python_trading-0.2.1/starkware/python/utils_stub_module.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/utils_stub_module.pyi` & `x10_python_trading-0.2.1/starkware/python/utils_stub_module.pyi`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/starkware/python/utils_test.py` & `x10_python_trading-0.2.1/starkware/python/utils_test.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/accounts.py` & `x10_python_trading-0.2.1/x10/perpetual/accounts.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/amounts.py` & `x10_python_trading-0.2.1/x10/perpetual/amounts.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/assets.py` & `x10_python_trading-0.2.1/x10/perpetual/assets.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/markets.py` & `x10_python_trading-0.2.1/x10/perpetual/markets.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/order_object.py` & `x10_python_trading-0.2.1/x10/perpetual/order_object.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/orderbooks.py` & `x10_python_trading-0.2.1/x10/perpetual/orderbooks.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/orders.py` & `x10_python_trading-0.2.1/x10/perpetual/orders.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/positions.py` & `x10_python_trading-0.2.1/x10/perpetual/positions.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/simple_client/simple_trading_client.py` & `x10_python_trading-0.2.1/x10/perpetual/simple_client/simple_trading_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/stream_client/perpetual_stream_connection.py` & `x10_python_trading-0.2.1/x10/perpetual/stream_client/perpetual_stream_connection.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/stream_client/stream_client.py` & `x10_python_trading-0.2.1/x10/perpetual/stream_client/stream_client.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/trades.py` & `x10_python_trading-0.2.1/x10/perpetual/trades.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/perpetual/trading_client/account_module.py` & `x10_python_trading-0.2.1/x10/perpetual/trading_client/account_module.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 class AccountModule(BaseModule):
     async def get_balance(self) -> WrappedApiResponse[BalanceModel]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-balance
         """
 
         url = self._get_url("/user/balance")
-        return await send_get_request(url, BalanceModel, api_key=self._get_api_key())
+        return await send_get_request(await self.get_session(), url, BalanceModel, api_key=self._get_api_key())
 
     async def get_positions(
         self, *, market_names: Optional[List[str]] = None, position_side: Optional[PositionSide] = None
     ) -> WrappedApiResponse[List[PositionModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-positions
         """
 
         url = self._get_url("/user/positions", query={"market": market_names, "side": position_side})
-        return await send_get_request(url, List[PositionModel], api_key=self._get_api_key())
+        return await send_get_request(await self.get_session(), url, List[PositionModel], api_key=self._get_api_key())
 
     async def get_positions_history(
         self,
         market_names: Optional[List[str]] = None,
         position_side: Optional[PositionSide] = None,
         cursor: Optional[int] = None,
         limit: Optional[int] = None,
@@ -42,15 +42,17 @@
         https://x101.docs.apiary.io/#reference/0/account/get-positions-history
         """
 
         url = self._get_url(
             "/user/positions/history",
             query={"market": market_names, "side": position_side, "cursor": cursor, "limit": limit},
         )
-        return await send_get_request(url, List[PositionHistoryModel], api_key=self._get_api_key())
+        return await send_get_request(
+            await self.get_session(), url, List[PositionHistoryModel], api_key=self._get_api_key()
+        )
 
     async def get_open_orders(
         self,
         market_names: Optional[List[str]] = None,
         order_type: Optional[OrderType] = None,
         order_side: Optional[OrderSide] = None,
     ) -> WrappedApiResponse[List[OpenOrderModel]]:
@@ -58,15 +60,15 @@
         https://x101.docs.apiary.io/#reference/0/account/get-open-orders
         """
 
         url = self._get_url(
             "/user/orders",
             query={"market": market_names, "type": order_type, "side": order_side},
         )
-        return await send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
+        return await send_get_request(await self.get_session(), url, List[OpenOrderModel], api_key=self._get_api_key())
 
     async def get_orders_history(
         self,
         market_names: Optional[List[str]] = None,
         order_type: Optional[OrderType] = None,
         order_side: Optional[OrderSide] = None,
         cursor: Optional[int] = None,
@@ -76,15 +78,15 @@
         https://x101.docs.apiary.io/#reference/0/account/get-orders-history
         """
 
         url = self._get_url(
             "/user/orders/history",
             query={"market": market_names, "type": order_type, "side": order_side, "cursor": cursor, "limit": limit},
         )
-        return await send_get_request(url, List[OpenOrderModel], api_key=self._get_api_key())
+        return await send_get_request(await self.get_session(), url, List[OpenOrderModel], api_key=self._get_api_key())
 
     async def get_trades(
         self,
         market_names: List[str],
         trade_side: Optional[OrderSide] = None,
         trade_type: Optional[TradeType] = None,
     ) -> WrappedApiResponse[List[AccountTradeModel]]:
@@ -93,38 +95,41 @@
         """
 
         url = self._get_url(
             "/user/trades",
             query={"market": market_names, "side": trade_side, "type": trade_type},
         )
 
-        return await send_get_request(url, List[AccountTradeModel], api_key=self._get_api_key())
+        return await send_get_request(
+            await self.get_session(), url, List[AccountTradeModel], api_key=self._get_api_key()
+        )
 
     async def get_fees(self, *, market_names: List[str]) -> WrappedApiResponse[List[TradingFeeModel]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-fees
         """
 
         url = self._get_url("/user/fees", query={"market": market_names})
-        return await send_get_request(url, List[TradingFeeModel], api_key=self._get_api_key())
+        return await send_get_request(await self.get_session(), url, List[TradingFeeModel], api_key=self._get_api_key())
 
     async def get_leverage(self, market_names: List[str]) -> WrappedApiResponse[List[AccountLeverage]]:
         """
         https://x101.docs.apiary.io/#reference/0/account/get-current-leverage
         """
 
         url = self._get_url("/user/leverage", query={"market": market_names})
-        return await send_get_request(url, List[AccountLeverage], api_key=self._get_api_key())
+        return await send_get_request(await self.get_session(), url, List[AccountLeverage], api_key=self._get_api_key())
 
     async def update_leverage(self, market_name: str, leverage: Decimal) -> WrappedApiResponse[EmptyModel]:
         """
         https://x101.docs.apiary.io/#reference/0/account/update-leverage
         """
 
         url = self._get_url("/user/leverage")
         request_model = AccountLeverage(market=market_name, leverage=leverage)
         return await send_patch_request(
+            await self.get_session(),
             url,
             EmptyModel,
             json=request_model.to_api_request_json(),
             api_key=self._get_api_key(),
         )
```

### Comparing `x10_python_trading-0.2.0/x10/perpetual/trading_client/base_module.py` & `x10_python_trading-0.2.1/x10/perpetual/trading_client/base_module.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Dict, Optional
 
+import aiohttp
+
 from x10.errors import X10Error
-from x10.utils.http import get_url
+from x10.utils.http import CLIENT_TIMEOUT, get_url
 
 
 class BaseModule:
     __api_url: str
     __api_key: Optional[str]
+    __session: aiohttp.ClientSession | None = None
 
     def __init__(self, api_url: str, api_key: Optional[str]):
         super().__init__()
 
         self.__api_url = api_url
         self.__api_key = api_key
 
@@ -18,7 +21,13 @@
         return get_url(f"{self.__api_url}{path}", query=query, **path_params)
 
     def _get_api_key(self):
         if not self.__api_key:
             raise X10Error("API key is not set")
 
         return self.__api_key
+
+    async def get_session(self) -> aiohttp.ClientSession:
+        if self.__session is None:
+            created_session = aiohttp.ClientSession(timeout=CLIENT_TIMEOUT)
+            self.__session = created_session
+        return self.__session
```

### Comparing `x10_python_trading-0.2.0/x10/perpetual/trading_client/markets_information_module.py` & `x10_python_trading-0.2.1/x10/perpetual/trading_client/markets_information_module.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,34 +5,37 @@
 from x10.perpetual.markets import MarketModel, MarketStatsModel
 from x10.perpetual.trading_client.base_module import BaseModule
 from x10.utils.date import to_epoch_millis
 from x10.utils.http import send_get_request
 
 
 class MarketsInformationModule(BaseModule):
-    def get_markets(self, *, market_names: Optional[List[str]] = None):
+    async def get_markets(self, *, market_names: Optional[List[str]] = None):
         """
         https://x101.docs.apiary.io/#reference/0/markets-information/get-markets
         """
 
         url = self._get_url("/info/markets", query={"market": market_names})
-        return send_get_request(url, List[MarketModel])
+        return await send_get_request(await self.get_session(), url, List[MarketModel])
 
-    def get_market_statistics(self, *, market_name: str):
+    async def get_market_statistics(self, *, market_name: str):
         """
         https://x101.docs.apiary.io/#reference/0/markets-information/get-market-statistics
         """
 
         url = self._get_url("/info/markets/<market>/stats", market=market_name)
-        return send_get_request(url, MarketStatsModel)
+        return await send_get_request(await self.get_session(), url, MarketStatsModel)
 
-    def get_funding_rates_history(self, *, market_name: str, start_time: datetime, end_time: datetime):
+    async def get_funding_rates_history(self, *, market_name: str, start_time: datetime, end_time: datetime):
         """
         https://x101.docs.apiary.io/#reference/0/markets-information/get-funding-rates-history
         """
 
         url = self._get_url(
             "/info/<market>/funding",
-            query={"startTime": to_epoch_millis(start_time), "endTime": to_epoch_millis(end_time)},
+            query={
+                "startTime": to_epoch_millis(start_time),
+                "endTime": to_epoch_millis(end_time),
+            },
             market=market_name,
         )
-        return send_get_request(url, List[FundingRateModel])
+        return await send_get_request(await self.get_session(), url, List[FundingRateModel])
```

### Comparing `x10_python_trading-0.2.0/x10/perpetual/trading_client/order_management_module.py` & `x10_python_trading-0.2.1/x10/perpetual/trading_client/order_management_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 LOGGER = get_logger(__name__)
 
 
 class _MassCancelRequestModel(X10BaseModel):
     order_ids: Optional[list[int]]
     external_order_ids: Optional[list[str]]
-    market_ids: Optional[list[int]]
+    markets: Optional[list[str]]
     cancel_all: Optional[bool]
 
 
 class OrderManagementModule(BaseModule):
     async def place_order(self, order: PerpetualOrderModel):
         """
         Placed new order on the exchange.
@@ -25,47 +25,51 @@
 
         https://x101.docs.apiary.io/#reference/0/order-managment/create-order
         """
         LOGGER.debug("Placing an order: id=%s", order.id)
 
         url = self._get_url("/user/order")
         response = await send_post_request(
+            await self.get_session(),
             url,
             PlacedOrderModel,
             json=order.to_api_request_json(),
             api_key=self._get_api_key(),
         )
         return response
 
     async def cancel_order(self, order_id: int):
         """
         https://x101.docs.apiary.io/#reference/0/order-managment/cancel-order
         """
 
         url = self._get_url("/user/order/<order_id>", order_id=order_id)
-        return await send_delete_request(url, EmptyModel, api_key=self._get_api_key(), idempotent=True, retry=True)
+        return await send_delete_request(
+            await self.get_session(), url, EmptyModel, api_key=self._get_api_key(), idempotent=True, retry=True
+        )
 
     async def mass_cancel(
         self,
         *,
         order_ids: Optional[list[int]] = None,
         external_order_ids: Optional[list[str]] = None,
-        market_ids: Optional[list[int]] = None,
+        markets: Optional[list[str]] = None,
         cancel_all: Optional[bool] = False,
     ):
         """
         https://x101.docs.apiary.io/#reference/0/order-managment/mass-cancel
         """
 
         url = self._get_url("/user/order/massCancel")
         request_model = _MassCancelRequestModel(
             order_ids=order_ids,
             external_order_ids=external_order_ids,
-            market_ids=market_ids,
+            markets=markets,
             cancel_all=cancel_all,
         )
         return await send_post_request(
+            await self.get_session(),
             url,
             EmptyModel,
             json=request_model.to_api_request_json(exclude_none=True),
             api_key=self._get_api_key(),
         )
```

### Comparing `x10_python_trading-0.2.0/x10/perpetual/trading_client/trading_client.py` & `x10_python_trading-0.2.1/x10/perpetual/trading_client/trading_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from x10.perpetual.orders import OrderSide, PlacedOrderModel
 from x10.perpetual.trading_client.account_module import AccountModule
 from x10.perpetual.trading_client.markets_information_module import (
     MarketsInformationModule,
 )
 from x10.perpetual.trading_client.order_management_module import OrderManagementModule
 from x10.utils.date import utc_now
+from x10.utils.http import WrappedApiResponse
 from x10.utils.log import get_logger
 
 LOGGER = get_logger(__name__)
 
 
 class PerpetualTradingClient:
     """
@@ -38,15 +39,15 @@
         market_name: str,
         amount_of_synthetic: Decimal,
         price: Decimal,
         side: OrderSide,
         post_only: bool = False,
         previous_order_id=None,
         expire_time=utc_now() + timedelta(hours=8),
-    ) -> PlacedOrderModel:
+    ) -> WrappedApiResponse[PlacedOrderModel]:
         if not self.__account:
             raise ValueError("Account not set")
 
         if not self.__markets:
             markets = await self.__markets_info_module.get_markets()
             self.__markets = {m.name: m for m in markets.data}
```

### Comparing `x10_python_trading-0.2.0/x10/utils/http.py` & `x10_python_trading-0.2.1/x10/utils/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,77 +96,79 @@
 
         template += "?" + "&".join(query_parts)
 
     return template
 
 
 async def send_get_request(
-    url: str, model_class: Type[ApiResponseType], *, api_key: Optional[str] = None
+    session: aiohttp.ClientSession,
+    url: str,
+    model_class: Type[ApiResponseType],
+    *,
+    api_key: Optional[str] = None,
 ) -> WrappedApiResponse[ApiResponseType]:
     LOGGER.debug("Sending GET %s", url)
-
     headers = __get_headers(api_key=api_key)
-
-    async with aiohttp.ClientSession(timeout=CLIENT_TIMEOUT) as session:
-        async with session.get(url, headers=headers) as response:
-            response_text = await response.text()
-            return parse_response_to_model(response_text, model_class)
+    async with session.get(url, headers=headers) as response:
+        response_text = await response.text()
+        return parse_response_to_model(response_text, model_class)
 
 
 async def send_post_request(
-    url: str, model_class: Type[ApiResponseType], *, json: Any = None, api_key: Optional[str] = None
+    session: aiohttp.ClientSession,
+    url: str,
+    model_class: Type[ApiResponseType],
+    *,
+    json: Any = None,
+    api_key: Optional[str] = None,
 ) -> WrappedApiResponse[ApiResponseType]:
     headers = __get_headers(api_key=api_key)
 
     LOGGER.debug("Sending POST %s, headers=%s, data=%s", url, headers, {})
-
-    async with aiohttp.ClientSession(timeout=CLIENT_TIMEOUT) as session:
-        async with session.post(url, json=json, headers=headers) as response:
-            response_text = await response.text()
-            response_model = parse_response_to_model(response_text, model_class)
-            if (response_model.status != ResponseStatus.OK.value) or (response_model.error is not None):
-                LOGGER.error("Error response from POST %s: %s", url, response_model.error)
-                raise ValueError(f"Error response from POST {url}: {response_model.error}")
-            return response_model
+    async with session.post(url, json=json, headers=headers) as response:
+        response_text = await response.text()
+        response_model = parse_response_to_model(response_text, model_class)
+        if (response_model.status != ResponseStatus.OK.value) or (response_model.error is not None):
+            LOGGER.error("Error response from POST %s: %s", url, response_model.error)
+            raise ValueError(f"Error response from POST {url}: {response_model.error}")
+        return response_model
 
 
 async def send_patch_request(
-    url: str, model_class: Type[ApiResponseType], *, json: Any = None, api_key: Optional[str] = None
+    session: aiohttp.ClientSession,
+    url: str,
+    model_class: Type[ApiResponseType],
+    *,
+    json: Any = None,
+    api_key: Optional[str] = None,
 ) -> WrappedApiResponse[ApiResponseType]:
     headers = __get_headers(api_key=api_key)
-
     LOGGER.debug("Sending PATCH %s, headers=%s, data=%s", url, headers, json)
-
-    async with aiohttp.ClientSession(timeout=CLIENT_TIMEOUT) as session:
-        async with session.patch(url, json=json, headers=headers) as response:
-            response_text = await response.text()
-
-            if response_text == "":
-                LOGGER.error("Empty HTTP %s response from PATCH %s", response.status, url)
-                response_text = '{"status": "OK"}'
-
-            return parse_response_to_model(response_text, model_class)
+    async with session.patch(url, json=json, headers=headers) as response:
+        response_text = await response.text()
+        if response_text == "":
+            LOGGER.error("Empty HTTP %s response from PATCH %s", response.status, url)
+            response_text = '{"status": "OK"}'
+        return parse_response_to_model(response_text, model_class)
 
 
 async def send_delete_request(
+    session: aiohttp.ClientSession,
     url: str,
     model_class: Type[ApiResponseType],
     *,
     api_key: Optional[str] = None,
     idempotent: bool = False,
     retry=False,
 ):
     headers = __get_headers(api_key=api_key)
-
     LOGGER.debug("Sending DELETE %s, headers=%s", url, headers)
-
-    async with aiohttp.ClientSession(timeout=CLIENT_TIMEOUT) as session:
-        async with session.delete(url, headers=headers) as response:
-            response_text = await response.text()
-            return parse_response_to_model(response_text, model_class)
+    async with session.delete(url, headers=headers) as response:
+        response_text = await response.text()
+        return parse_response_to_model(response_text, model_class)
 
 
 def __get_headers(*, api_key: Optional[str] = None):
     headers = {
         RequestHeader.ACCEPT.value: "application/json",
         RequestHeader.CONTENT_TYPE.value: "application/json",
         RequestHeader.USER_AGENT.value: USER_AGENT,
```

### Comparing `x10_python_trading-0.2.0/x10/utils/model.py` & `x10_python_trading-0.2.1/x10/utils/model.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/x10/utils/starkex.py` & `x10_python_trading-0.2.1/x10/utils/starkex.py`

 * *Files identical despite different names*

### Comparing `x10_python_trading-0.2.0/PKG-INFO` & `x10_python_trading-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x10-python-trading
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for X10 API
 Author: X10
 Author-email: tech@ex10.org
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

