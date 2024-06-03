# Comparing `tmp/boulder_opal-1.4.0.tar.gz` & `tmp/boulder_opal-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boulder_opal-1.4.0.tar", max compression
+gzip compressed data, was "boulder_opal-2.0.0.tar", max compression
```

## Comparing `boulder_opal-1.4.0.tar` & `boulder_opal-2.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    36587 2024-03-26 02:19:13.250002 boulder_opal-1.4.0/LICENSE
--rw-r--r--   0        0        0      400 2024-03-26 02:19:13.250002 boulder_opal-1.4.0/README.md
--rw-r--r--   0        0        0     1804 2024-03-26 02:19:36.450317 boulder_opal-1.4.0/boulderopal/__init__.py
--rw-r--r--   0        0        0      550 2024-03-26 02:19:36.474317 boulder_opal-1.4.0/boulderopal/_configuration/__init__.py
--rw-r--r--   0        0        0     3503 2024-03-26 02:19:13.250002 boulder_opal-1.4.0/boulderopal/_configuration/activity_monitor.py
--rw-r--r--   0        0        0     2569 2024-03-26 02:19:13.250002 boulder_opal-1.4.0/boulderopal/_configuration/authenticate.py
--rw-r--r--   0        0        0     5983 2024-03-26 02:19:13.250002 boulder_opal-1.4.0/boulderopal/_configuration/cloud.py
--rw-r--r--   0        0        0     5197 2024-03-26 02:19:13.250002 boulder_opal-1.4.0/boulderopal/_configuration/configuration.py
--rw-r--r--   0        0        0     1283 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_configuration/constants.py
--rw-r--r--   0        0        0     2497 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_configuration/verbosity.py
--rw-r--r--   0        0        0     1109 2024-03-26 02:19:36.458317 boulder_opal-1.4.0/boulderopal/_core/__init__.py
--rw-r--r--   0        0        0     1649 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_core/base.py
--rw-r--r--   0        0        0     1957 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_core/formatter.py
--rw-r--r--   0        0        0     4605 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_core/workflows.py
--rw-r--r--   0        0        0      550 2024-03-26 02:19:36.462317 boulder_opal-1.4.0/boulderopal/_nodes/__init__.py
--rw-r--r--   0        0        0    25199 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/arithmetic_binary.py
--rw-r--r--   0        0        0    38826 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/arithmetic_unary.py
--rw-r--r--   0        0        0     2511 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/base.py
--rw-r--r--   0        0        0     3757 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/differentiation.py
--rw-r--r--   0        0        0     9366 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/filter_function.py
--rw-r--r--   0        0        0    38736 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/fock_space.py
--rw-r--r--   0        0        0    16706 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/infidelity.py
--rw-r--r--   0        0        0    34875 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/ions.py
--rw-r--r--   0        0        0    18695 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/node_data.py
--rw-r--r--   0        0        0    26195 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/optimization.py
--rw-r--r--   0        0        0    24466 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/oqs.py
--rw-r--r--   0        0        0    38261 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/pwc.py
--rw-r--r--   0        0        0    16819 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/random.py
--rw-r--r--   0        0        0      872 2024-03-26 02:19:36.466317 boulder_opal-1.4.0/boulderopal/_nodes/signals/__init__.py
--rw-r--r--   0        0        0    65670 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/signals/signals_pwc.py
--rw-r--r--   0        0        0    23430 2024-03-26 02:19:13.254002 boulder_opal-1.4.0/boulderopal/_nodes/signals/signals_stf.py
--rw-r--r--   0        0        0    23999 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_nodes/sparse.py
--rw-r--r--   0        0        0    26904 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_nodes/stf.py
--rw-r--r--   0        0        0    74003 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_nodes/tensor.py
--rw-r--r--   0        0        0     7264 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_nodes/utils.py
--rw-r--r--   0        0        0     8931 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_nodes/validation.py
--rw-r--r--   0        0        0     1188 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_typing.py
--rw-r--r--   0        0        0     4023 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_utils.py
--rw-r--r--   0        0        0     1023 2024-03-26 02:19:36.458317 boulder_opal-1.4.0/boulderopal/_validation/__init__.py
--rw-r--r--   0        0        0    14209 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_validation/basic.py
--rw-r--r--   0        0        0     1391 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_validation/exceptions.py
--rw-r--r--   0        0        0     7980 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_validation/graph.py
--rw-r--r--   0        0        0    11899 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/_validation/pydantic.py
--rw-r--r--   0        0        0      973 2024-03-26 02:19:36.462317 boulder_opal-1.4.0/boulderopal/closed_loop/__init__.py
--rw-r--r--   0        0        0    19820 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/closed_loop/_optimization.py
--rw-r--r--   0        0        0    16240 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/closed_loop/_optimizers.py
--rw-r--r--   0        0        0     1111 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/cloud.py
--rw-r--r--   0        0        0      680 2024-03-26 02:19:36.466317 boulder_opal-1.4.0/boulderopal/gradient_free/__init__.py
--rw-r--r--   0        0        0     9577 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/gradient_free/_optimization.py
--rw-r--r--   0        0        0     1668 2024-03-26 02:19:36.470317 boulder_opal-1.4.0/boulderopal/graph/__init__.py
--rw-r--r--   0        0        0     5124 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/graph/_execute_graph.py
--rw-r--r--   0        0        0     9846 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/graph/_graph.py
--rw-r--r--   0        0        0     1027 2024-03-26 02:19:36.462317 boulder_opal-1.4.0/boulderopal/ions/__init__.py
--rw-r--r--   0        0        0     9611 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/ions/_drives.py
--rw-r--r--   0        0        0     4577 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/ions/_ion_chain_properties.py
--rw-r--r--   0        0        0    20375 2024-03-26 02:19:13.258002 boulder_opal-1.4.0/boulderopal/ions/_molmer_sorensen.py
--rw-r--r--   0        0        0      985 2024-03-26 02:19:36.454317 boulder_opal-1.4.0/boulderopal/noise_reconstruction/__init__.py
--rw-r--r--   0        0        0     9645 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/noise_reconstruction/_classes.py
--rw-r--r--   0        0        0    12185 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/noise_reconstruction/_reconstruct.py
--rw-r--r--   0        0        0      694 2024-03-26 02:19:36.474317 boulder_opal-1.4.0/boulderopal/optimization/__init__.py
--rw-r--r--   0        0        0    12635 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/optimization/_optimization.py
--rw-r--r--   0        0        0        0 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/py.typed
--rw-r--r--   0        0        0      925 2024-03-26 02:19:36.454317 boulder_opal-1.4.0/boulderopal/signals/__init__.py
--rw-r--r--   0        0        0    35040 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/signals/_functions.py
--rw-r--r--   0        0        0      729 2024-03-26 02:19:36.474317 boulder_opal-1.4.0/boulderopal/stochastic/__init__.py
--rw-r--r--   0        0        0    12469 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/stochastic/_optimization.py
--rw-r--r--   0        0        0     1396 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/stochastic/_optimizer.py
--rw-r--r--   0        0        0     1339 2024-03-26 02:19:36.470317 boulder_opal-1.4.0/boulderopal/superconducting/__init__.py
--rw-r--r--   0        0        0    13205 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/superconducting/_components.py
--rw-r--r--   0        0        0     6627 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/superconducting/_drives.py
--rw-r--r--   0        0        0    32366 2024-03-26 02:19:13.262002 boulder_opal-1.4.0/boulderopal/superconducting/_functions.py
--rw-r--r--   0        0        0     3360 2024-03-26 02:19:36.438317 boulder_opal-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 boulder_opal-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/LICENSE
+-rw-r--r--   0        0        0      400 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/README.md
+-rw-r--r--   0        0        0     1804 2024-06-03 06:33:22.259518 boulder_opal-2.0.0/boulderopal/__init__.py
+-rw-r--r--   0        0        0      550 2024-06-03 06:33:22.271519 boulder_opal-2.0.0/boulderopal/_configuration/__init__.py
+-rw-r--r--   0        0        0     3503 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_configuration/activity_monitor.py
+-rw-r--r--   0        0        0     2569 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_configuration/authenticate.py
+-rw-r--r--   0        0        0     5932 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_configuration/cloud.py
+-rw-r--r--   0        0        0     5197 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_configuration/configuration.py
+-rw-r--r--   0        0        0     1283 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_configuration/constants.py
+-rw-r--r--   0        0        0     2497 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_configuration/verbosity.py
+-rw-r--r--   0        0        0     1109 2024-06-03 06:33:22.263518 boulder_opal-2.0.0/boulderopal/_core/__init__.py
+-rw-r--r--   0        0        0     1649 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_core/base.py
+-rw-r--r--   0        0        0     1957 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_core/formatter.py
+-rw-r--r--   0        0        0     4605 2024-06-03 06:32:58.087052 boulder_opal-2.0.0/boulderopal/_core/workflows.py
+-rw-r--r--   0        0        0      550 2024-06-03 06:33:22.279519 boulder_opal-2.0.0/boulderopal/_nodes/__init__.py
+-rw-r--r--   0        0        0    25199 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/arithmetic_binary.py
+-rw-r--r--   0        0        0    38826 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/arithmetic_unary.py
+-rw-r--r--   0        0        0     2511 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/base.py
+-rw-r--r--   0        0        0     3757 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/differentiation.py
+-rw-r--r--   0        0        0     9366 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/filter_function.py
+-rw-r--r--   0        0        0    38736 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/fock_space.py
+-rw-r--r--   0        0        0    16706 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/infidelity.py
+-rw-r--r--   0        0        0    34875 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/ions.py
+-rw-r--r--   0        0        0    18695 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/node_data.py
+-rw-r--r--   0        0        0    26171 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/optimization.py
+-rw-r--r--   0        0        0    24466 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/oqs.py
+-rw-r--r--   0        0        0    38248 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/pwc.py
+-rw-r--r--   0        0        0    16819 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/random.py
+-rw-r--r--   0        0        0      872 2024-06-03 06:33:22.279519 boulder_opal-2.0.0/boulderopal/_nodes/signals/__init__.py
+-rw-r--r--   0        0        0    65358 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/signals/signals_pwc.py
+-rw-r--r--   0        0        0    23120 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/signals/signals_stf.py
+-rw-r--r--   0        0        0    24018 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/sparse.py
+-rw-r--r--   0        0        0    26921 2024-06-03 06:32:58.091052 boulder_opal-2.0.0/boulderopal/_nodes/stf.py
+-rwxr-xr-x   0        0        0    74798 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_nodes/tensor.py
+-rw-r--r--   0        0        0     7264 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_nodes/utils.py
+-rw-r--r--   0        0        0     9317 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_nodes/validation.py
+-rw-r--r--   0        0        0     1015 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_typing.py
+-rw-r--r--   0        0        0     4023 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_utils.py
+-rw-r--r--   0        0        0      981 2024-06-03 06:33:22.267519 boulder_opal-2.0.0/boulderopal/_validation/__init__.py
+-rw-r--r--   0        0        0    14209 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_validation/basic.py
+-rw-r--r--   0        0        0     1391 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_validation/exceptions.py
+-rw-r--r--   0        0        0     7980 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_validation/graph.py
+-rw-r--r--   0        0        0     5636 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/_validation/pydantic.py
+-rw-r--r--   0        0        0      973 2024-06-03 06:33:22.267519 boulder_opal-2.0.0/boulderopal/closed_loop/__init__.py
+-rw-r--r--   0        0        0    19820 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/closed_loop/_optimization.py
+-rw-r--r--   0        0        0    16240 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/closed_loop/_optimizers.py
+-rw-r--r--   0        0        0     1111 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/cloud.py
+-rw-r--r--   0        0        0      680 2024-06-03 06:33:22.271519 boulder_opal-2.0.0/boulderopal/gradient_free/__init__.py
+-rw-r--r--   0        0        0     9577 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/gradient_free/_optimization.py
+-rw-r--r--   0        0        0     1668 2024-06-03 06:33:22.267519 boulder_opal-2.0.0/boulderopal/graph/__init__.py
+-rw-r--r--   0        0        0     5124 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/graph/_execute_graph.py
+-rw-r--r--   0        0        0     9846 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/graph/_graph.py
+-rw-r--r--   0        0        0     1027 2024-06-03 06:33:22.279519 boulder_opal-2.0.0/boulderopal/ions/__init__.py
+-rw-r--r--   0        0        0     9611 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/ions/_drives.py
+-rw-r--r--   0        0        0     4577 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/ions/_ion_chain_properties.py
+-rw-r--r--   0        0        0    20375 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/ions/_molmer_sorensen.py
+-rw-r--r--   0        0        0      985 2024-06-03 06:33:22.263518 boulder_opal-2.0.0/boulderopal/noise_reconstruction/__init__.py
+-rw-r--r--   0        0        0     9645 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/noise_reconstruction/_classes.py
+-rw-r--r--   0        0        0    12185 2024-06-03 06:32:58.095052 boulder_opal-2.0.0/boulderopal/noise_reconstruction/_reconstruct.py
+-rw-r--r--   0        0        0      694 2024-06-03 06:33:22.283519 boulder_opal-2.0.0/boulderopal/optimization/__init__.py
+-rw-r--r--   0        0        0    12635 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/optimization/_optimization.py
+-rw-r--r--   0        0        0        0 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/py.typed
+-rw-r--r--   0        0        0      925 2024-06-03 06:33:22.283519 boulder_opal-2.0.0/boulderopal/signals/__init__.py
+-rw-r--r--   0        0        0    35040 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/signals/_functions.py
+-rw-r--r--   0        0        0      729 2024-06-03 06:33:22.275519 boulder_opal-2.0.0/boulderopal/stochastic/__init__.py
+-rw-r--r--   0        0        0    12469 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/stochastic/_optimization.py
+-rw-r--r--   0        0        0     1396 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/stochastic/_optimizer.py
+-rw-r--r--   0        0        0     1339 2024-06-03 06:33:22.275519 boulder_opal-2.0.0/boulderopal/superconducting/__init__.py
+-rw-r--r--   0        0        0    13205 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/superconducting/_components.py
+-rw-r--r--   0        0        0     6627 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/superconducting/_drives.py
+-rw-r--r--   0        0        0    32366 2024-06-03 06:32:58.099052 boulder_opal-2.0.0/boulderopal/superconducting/_functions.py
+-rw-r--r--   0        0        0     3314 2024-06-03 06:33:22.247518 boulder_opal-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2551 1970-01-01 00:00:00.000000 boulder_opal-2.0.0/PKG-INFO
```

### Comparing `boulder_opal-1.4.0/LICENSE` & `boulder_opal-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/__init__.py` & `boulder_opal-2.0.0/boulderopal/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-__version__ = "1.4.0"
+__version__ = "2.0.0"
 
 from qctrlworkflowclient.utils import check_package_version as _check_package_version
 
 from boulderopal import (
     closed_loop,
     cloud,
     gradient_free,
```

### Comparing `boulder_opal-1.4.0/boulderopal/_configuration/__init__.py` & `boulder_opal-2.0.0/boulderopal/_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_configuration/activity_monitor.py` & `boulder_opal-2.0.0/boulderopal/_configuration/activity_monitor.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_configuration/authenticate.py` & `boulder_opal-2.0.0/boulderopal/_configuration/authenticate.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_configuration/cloud.py` & `boulder_opal-2.0.0/boulderopal/_configuration/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     Returns
     -------
     ContextManager
         A context manager to collect and run computation requests.
 
     Notes
     -----
-    You can to group up to five requests together.
     All grouped calculations must be independent from each other.
 
     Within the context manager, the object returned from each request is a placeholder.
     When exiting, the context manager waits until all calculations have finished,
     hence this command blocks execution.
     When all results are received, the placeholders are replaced with them.
```

### Comparing `boulder_opal-1.4.0/boulderopal/_configuration/configuration.py` & `boulder_opal-2.0.0/boulderopal/_configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_configuration/constants.py` & `boulder_opal-2.0.0/boulderopal/_configuration/constants.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_configuration/verbosity.py` & `boulder_opal-2.0.0/boulderopal/_configuration/verbosity.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_core/__init__.py` & `boulder_opal-2.0.0/boulderopal/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_core/base.py` & `boulder_opal-2.0.0/boulderopal/_core/base.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_core/formatter.py` & `boulder_opal-2.0.0/boulderopal/_core/formatter.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_core/workflows.py` & `boulder_opal-2.0.0/boulderopal/_core/workflows.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/__init__.py` & `boulder_opal-2.0.0/boulderopal/_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/arithmetic_binary.py` & `boulder_opal-2.0.0/boulderopal/_nodes/arithmetic_binary.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/arithmetic_unary.py` & `boulder_opal-2.0.0/boulderopal/_nodes/arithmetic_unary.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/base.py` & `boulder_opal-2.0.0/boulderopal/_nodes/base.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/differentiation.py` & `boulder_opal-2.0.0/boulderopal/_nodes/differentiation.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/filter_function.py` & `boulder_opal-2.0.0/boulderopal/_nodes/filter_function.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/fock_space.py` & `boulder_opal-2.0.0/boulderopal/_nodes/fock_space.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/infidelity.py` & `boulder_opal-2.0.0/boulderopal/_nodes/infidelity.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/ions.py` & `boulder_opal-2.0.0/boulderopal/_nodes/ions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/node_data.py` & `boulder_opal-2.0.0/boulderopal/_nodes/node_data.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/optimization.py` & `boulder_opal-2.0.0/boulderopal/_nodes/optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     Callable,
     List,
     Optional,
     Union,
 )
 
 import numpy as np
+from pydantic import SkipValidation
 
 from boulderopal._nodes.base import create_operation
 from boulderopal._nodes.node_data import (
     Pwc,
     Stf,
     Tensor,
 )
@@ -34,15 +35,14 @@
     ArrayT,
     Checker,
     ScalarT,
     pipe,
     sequence_like,
     validated,
 )
-from boulderopal._validation.pydantic import SkipValidation
 
 
 def _validate_initial_values(
     values: Any, count: int, lower: float, upper: float
 ) -> Optional[np.ndarray | list[np.ndarray]]:
     Checker.VALUE(
         upper > lower,
```

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/oqs.py` & `boulder_opal-2.0.0/boulderopal/_nodes/oqs.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/pwc.py` & `boulder_opal-2.0.0/boulderopal/_nodes/pwc.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import (
     List,
     Optional,
     Union,
 )
 
 import numpy as np
+from pydantic import Field
 
 from boulderopal._nodes.base import create_operation
 from boulderopal._nodes.node_data import (
     Pwc,
     Tensor,
 )
 from boulderopal._nodes.utils import (
@@ -37,15 +38,14 @@
     strict_real_array,
 )
 from boulderopal._typing import Annotated
 from boulderopal._validation import (
     ArrayT,
     Checker,
     ScalarT,
-    minimum_length,
     pipe,
     validated,
 )
 
 
 class PwcGraph:  # pylint: disable=unused-argument
     """
@@ -591,15 +591,15 @@
             durations=np.array([duration]),
             batch_shape=shape[:batch_dimension_count],
         )
 
     @validated
     def pwc_sum(
         self,
-        terms: Annotated[List[Pwc], pipe(after=minimum_length(1))],
+        terms: Annotated[List[Pwc], Field(min_length=1)],
         *,
         name: Optional[str] = None,
     ) -> Pwc:
         r"""
         Create the sum of multiple piecewise-constant terms.
 
         Parameters
@@ -780,15 +780,15 @@
             durations=symmetrized_durations,
             batch_shape=pwc.batch_shape,
         )
 
     @validated
     def time_concatenate_pwc(
         self,
-        pwc_list: Annotated[List[Pwc], pipe(after=minimum_length(1))],
+        pwc_list: Annotated[List[Pwc], Field(min_length=1)],
         *,
         name: Optional[str] = None,
     ) -> Pwc:
         r"""
         Concatenate multiple piecewise-constant functions in the time dimension.
 
         Parameters
```

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/random.py` & `boulder_opal-2.0.0/boulderopal/_nodes/random.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/signals/__init__.py` & `boulder_opal-2.0.0/boulderopal/_nodes/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/signals/signals_pwc.py` & `boulder_opal-2.0.0/boulderopal/_nodes/signals/signals_pwc.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,43 +25,32 @@
 
 from boulderopal._nodes.node_data import (
     Pwc,
     Tensor,
 )
 from boulderopal._nodes.validation import (
     ShapeT,
-    _to_scalar_tensor,
+    positive_scalar,
+    scalar,
     shapeable,
 )
 from boulderopal._typing import Annotated
 from boulderopal._validation import (
     Checker,
     ScalarT,
     pipe,
-    type_pipe,
     validate_enum,
     validated,
 )
 
 if TYPE_CHECKING:
     from boulderopal._nodes.node_data import Stf
     from boulderopal.graph._graph import Graph
 
 
-def _scalar_messenger(name: str) -> str:
-    return f"The {name} must be a scalar or a scalar-like Tensor."
-
-
-_scalar = type_pipe([ScalarT.NUMERIC(), _to_scalar_tensor], _scalar_messenger)
-
-_positive_scalar = type_pipe(
-    [ScalarT.REAL().gt(0), _to_scalar_tensor], _scalar_messenger
-)
-
-
 class SegmentationType(str, Enum):
     """
     An enumeration of segmentation types for piecewise-constant signals.
 
     You can use this Enum to specify the segmentation type for graph nodes that
     define a PWC signal containing a constant part.
 
@@ -109,15 +98,15 @@
         self._graph = graph
 
     @validated
     def square_pulse_pwc(
         self,
         duration: Annotated[float, pipe(ScalarT.REAL().gt(0))],
         segment_count: Annotated[int, pipe(ScalarT.INT().ge(1))],
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
         start_time: float = 0,
         end_time: Optional[Annotated[float, pipe(ScalarT.REAL())]] = None,
         segmentation: SegmentationType = SegmentationType.UNIFORM,
         *,
         name: Optional[str] = None,
     ) -> Pwc:
         r"""
@@ -273,17 +262,17 @@
         return self._graph.time_concatenate_pwc(pwcs, name=name)
 
     @validated
     def sech_pulse_pwc(
         self,
         duration: Annotated[float, pipe(ScalarT.REAL().gt(0))],
         segment_count: Annotated[int, pipe(ScalarT.INT().ge(1))],
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        width: Optional[Annotated[Union[float, Tensor], pipe(_positive_scalar)]] = None,
-        center_time: Optional[Annotated[Union[float, Tensor], pipe(_scalar)]] = None,
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        width: Optional[Annotated[Union[float, Tensor], pipe(positive_scalar)]] = None,
+        center_time: Optional[Annotated[Union[float, Tensor], pipe(scalar)]] = None,
         *,
         name: Optional[str] = None,
     ) -> Pwc:
         r"""
         Create a `Pwc` representing a hyperbolic secant pulse.
 
         Parameters
@@ -402,17 +391,17 @@
         return self._graph.discretize_stf(stf, duration, segment_count, name=name)  # type: ignore
 
     @validated
     def linear_ramp_pwc(
         self,
         duration: Annotated[float, pipe(ScalarT.REAL().gt(0))],
         segment_count: Annotated[int, pipe(ScalarT.INT().ge(1))],
-        end_value: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
+        end_value: Annotated[Union[float, complex, Tensor], pipe(scalar)],
         start_value: Optional[
-            Annotated[Union[float, complex, Tensor], pipe(_scalar)]
+            Annotated[Union[float, complex, Tensor], pipe(scalar)]
         ] = None,
         start_time: float = 0,
         end_time: Optional[float] = None,
         segmentation: SegmentationType = SegmentationType.UNIFORM,
         *,
         name: Optional[str] = None,
     ) -> Pwc:
@@ -604,22 +593,22 @@
         return self._graph.time_concatenate_pwc(pwcs, name=name)
 
     @validated
     def tanh_ramp_pwc(
         self,
         duration: Annotated[float, pipe(ScalarT.REAL().gt(0))],
         segment_count: Annotated[int, pipe(ScalarT.INT().ge(1))],
-        end_value: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
+        end_value: Annotated[Union[float, complex, Tensor], pipe(scalar)],
         start_value: Optional[
-            Annotated[Union[float, complex, Tensor], pipe(_scalar)]
+            Annotated[Union[float, complex, Tensor], pipe(scalar)]
         ] = None,
         ramp_duration: Optional[
-            Annotated[Union[float, Tensor], pipe(_positive_scalar)]
+            Annotated[Union[float, Tensor], pipe(positive_scalar)]
         ] = None,
-        center_time: Optional[Annotated[Union[float, Tensor], pipe(_scalar)]] = None,
+        center_time: Optional[Annotated[Union[float, Tensor], pipe(scalar)]] = None,
         *,
         name: Optional[str] = None,
     ) -> Pwc:
         r"""
         Create a `Pwc` representing a hyperbolic tangent ramp.
 
         Parameters
@@ -770,18 +759,18 @@
         return self._graph.discretize_stf(stf, duration, segment_count, name=name)  # type: ignore
 
     @validated
     def gaussian_pulse_pwc(
         self,
         duration: Annotated[float, pipe(ScalarT.REAL().gt(0))],
         segment_count: Annotated[int, pipe(ScalarT.INT().ge(4))],
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        width: Optional[Annotated[Union[float, Tensor], pipe(_positive_scalar)]] = None,
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        width: Optional[Annotated[Union[float, Tensor], pipe(positive_scalar)]] = None,
         center_time: Optional[float] = None,
-        drag: Optional[Annotated[Union[float, Tensor], pipe(_scalar)]] = None,
+        drag: Optional[Annotated[Union[float, Tensor], pipe(scalar)]] = None,
         flat_duration: Optional[Annotated[float, pipe(ScalarT.REAL().gt(0))]] = None,
         segmentation: SegmentationType = SegmentationType.UNIFORM,
         *,
         name: Optional[str] = None,
     ) -> Pwc:
         r"""
         Create a `Pwc` representing a Gaussian pulse.
@@ -1039,16 +1028,16 @@
         return self._graph.time_concatenate_pwc(pwcs, name=name)
 
     @validated
     def cosine_pulse_pwc(
         self,
         duration: Annotated[float, pipe(ScalarT.REAL().gt(0))],
         segment_count: Annotated[int, pipe(ScalarT.INT().gt(0))],
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        drag: Optional[Annotated[Union[float, Tensor], pipe(_scalar)]] = None,
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        drag: Optional[Annotated[Union[float, Tensor], pipe(scalar)]] = None,
         start_time: float = 0.0,
         end_time: Optional[float] = None,
         flat_duration: Optional[Annotated[float, pipe(ScalarT.REAL().gt(0))]] = None,
         segmentation: SegmentationType = SegmentationType.UNIFORM,
         *,
         name: Optional[str] = None,
     ) -> Pwc:
@@ -1387,17 +1376,17 @@
         return self._graph.time_concatenate_pwc(pwcs, name=name)
 
     @validated
     def sinusoid_pwc(
         self,
         duration: Annotated[float, pipe(ScalarT.REAL().gt(0))],
         segment_count: Annotated[int, pipe(ScalarT.INT().gt(0))],
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        angular_frequency: Annotated[Union[float, Tensor], pipe(_scalar)],
-        phase: Annotated[Union[float, Tensor], pipe(_scalar)] = 0.0,
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        angular_frequency: Annotated[Union[float, Tensor], pipe(scalar)],
+        phase: Annotated[Union[float, Tensor], pipe(scalar)] = 0.0,
         *,
         name: Optional[str] = None,
     ) -> Pwc:
         r"""
         Create a `Pwc` representing a sinusoidal oscillation.
 
         Parameters
```

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/signals/signals_stf.py` & `boulder_opal-2.0.0/boulderopal/_nodes/signals/signals_stf.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,55 +26,44 @@
 
 from boulderopal._nodes.node_data import (
     Stf,
     Tensor,
 )
 from boulderopal._nodes.validation import (
     ShapeT,
-    _to_scalar_tensor,
+    positive_scalar,
+    scalar,
     shapeable,
 )
 from boulderopal._typing import Annotated
 from boulderopal._validation import (
     Checker,
     ScalarT,
     pipe,
-    type_pipe,
     validated,
 )
 
 if TYPE_CHECKING:
     from boulderopal.graph._graph import Graph
 
 
-def _scalar_messenger(name: str) -> str:
-    return f"The {name} must be a scalar or a scalar-like Tensor."
-
-
-_scalar = type_pipe([ScalarT.NUMERIC(), _to_scalar_tensor], _scalar_messenger)
-
-_positive_scalar = type_pipe(
-    [ScalarT.REAL().gt(0), _to_scalar_tensor], _scalar_messenger
-)
-
-
 class StfSignals:
     """
     Base class implementing Stf signal graph methods.
     """
 
     def __init__(self, graph: "Graph") -> None:
         self._graph = graph
 
     @validated
     def sech_pulse_stf(
         self,
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        width: Annotated[Union[float, Tensor], pipe(_positive_scalar)],
-        center_time: Annotated[Union[float, Tensor], pipe(_scalar)],
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        width: Annotated[Union[float, Tensor], pipe(positive_scalar)],
+        center_time: Annotated[Union[float, Tensor], pipe(scalar)],
     ) -> Stf:
         r"""
         Create an `Stf` representing a hyperbolic secant pulse.
 
         Parameters
         ----------
         amplitude : float or complex or Tensor
@@ -145,18 +134,18 @@
         return amplitude / self._graph.cosh(  # type:ignore
             (self._graph.identity_stf() - center_time) / width
         )
 
     @validated
     def gaussian_pulse_stf(
         self,
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        width: Annotated[Union[float, Tensor], pipe(_positive_scalar)],
-        center_time: Annotated[Union[float, Tensor], pipe(_scalar)],
-        drag: Optional[Annotated[Union[float, Tensor], pipe(_scalar)]] = None,
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        width: Annotated[Union[float, Tensor], pipe(positive_scalar)],
+        center_time: Annotated[Union[float, Tensor], pipe(scalar)],
+        drag: Optional[Annotated[Union[float, Tensor], pipe(scalar)]] = None,
     ) -> Stf:
         r"""
         Create an `Stf` representing a Gaussian pulse.
 
         Parameters
         ----------
         amplitude : float or complex or Tensor
@@ -256,17 +245,17 @@
         return amplitude * self._graph.exp(  # type: ignore
             -((self._graph.identity_stf() - center_time) ** 2) / (2 * width**2)
         )
 
     @validated
     def sinusoid_stf(
         self,
-        amplitude: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        angular_frequency: Annotated[Union[float, Tensor], pipe(_positive_scalar)],
-        phase: Annotated[Union[float, Tensor], pipe(_scalar)] = 0.0,
+        amplitude: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        angular_frequency: Annotated[Union[float, Tensor], pipe(positive_scalar)],
+        phase: Annotated[Union[float, Tensor], pipe(scalar)] = 0.0,
     ) -> Stf:
         r"""
         Create an `Stf` representing a sinusoidal oscillation.
 
         Parameters
         ----------
         amplitude : float or complex or Tensor
@@ -436,16 +425,16 @@
             for idx in range(coefficients.shape[0])
         ]
         return self._graph.stf_sum(stfs)
 
     @validated
     def linear_ramp_stf(
         self,
-        slope: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
-        shift: Annotated[Union[float, complex, Tensor], pipe(_scalar)] = 0.0,
+        slope: Annotated[Union[float, complex, Tensor], pipe(scalar)],
+        shift: Annotated[Union[float, complex, Tensor], pipe(scalar)] = 0.0,
     ) -> Stf:
         r"""
         Create an `Stf` representing a linear ramp.
 
         Parameters
         ----------
         slope : float or complex or Tensor
@@ -502,19 +491,19 @@
         <Stf: operation_name="add", value_shape=(), batch_shape=()>
         """
         return slope * self._graph.identity_stf() + shift
 
     @validated
     def tanh_ramp_stf(
         self,
-        center_time: Annotated[Union[float, Tensor], pipe(_scalar)],
-        ramp_duration: Annotated[Union[float, Tensor], pipe(_positive_scalar)],
-        end_value: Annotated[Union[float, complex, Tensor], pipe(_scalar)],
+        center_time: Annotated[Union[float, Tensor], pipe(scalar)],
+        ramp_duration: Annotated[Union[float, Tensor], pipe(positive_scalar)],
+        end_value: Annotated[Union[float, complex, Tensor], pipe(scalar)],
         start_value: Optional[
-            Annotated[Union[float, complex, Tensor], pipe(_scalar)]
+            Annotated[Union[float, complex, Tensor], pipe(scalar)]
         ] = None,
     ) -> Stf:
         r"""
         Create an `Stf` representing a hyperbolic tangent ramp.
 
         Parameters
         ----------
```

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/sparse.py` & `boulder_opal-2.0.0/boulderopal/_nodes/sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import (
     List,
     Optional,
     Union,
 )
 
 import numpy as np
+from pydantic import Field
 from scipy.sparse import (
     issparse,
     spmatrix,
 )
 
 from boulderopal._nodes.base import create_operation
 from boulderopal._nodes.validation import (
@@ -32,15 +33,14 @@
     bounded_by,
     shapeable,
 )
 from boulderopal._typing import Annotated
 from boulderopal._validation import (
     Checker,
     ScalarT,
-    minimum_length,
     pipe,
     type_pipe,
     validated,
 )
 
 from .node_data import (
     Pwc,
@@ -58,27 +58,27 @@
     return f"The {name} must be a positive float or a scalar Tensor."
 
 
 _scalar_int = type_pipe([ScalarT.INT().gt(0), _to_scalar_tensor], _int_messenger)
 _scalar_float = type_pipe([ScalarT.REAL().gt(0), _to_scalar_tensor], _float_messenger)
 
 
-def _validate_terms(terms: list[SparsePwc], *, name: str) -> list[SparsePwc]:
+def _validate_terms(value: list[SparsePwc], *, name: str) -> list[SparsePwc]:
     """
     Validate a list of SparsePwc terms.
     """
-    shape_0 = terms[0].value_shape
-    for i, term in enumerate(terms):
+    shape_0 = value[0].value_shape
+    for i, term in enumerate(value):
         shape = term.value_shape
         Checker.VALUE(
             shape == shape_0,
             f"All the elements in {name} must have the same shape.",
             {"terms[0].value_shape": shape_0, f"terms[{i}].value_shape": shape},
         )
-    return terms
+    return value
 
 
 class SparseGraph:  # pylint: disable=unused-argument
     """
     Base class implementing sparse graph methods.
     """
 
@@ -194,15 +194,16 @@
         self,
         terms: Annotated[
             List[
                 Annotated[
                     SparsePwc, pipe(shapeable, after=ShapeT.OPERATOR().no_batch())
                 ]
             ],
-            pipe(after=[minimum_length(1), _validate_terms]),
+            Field(min_length=1),
+            pipe(after=_validate_terms),
         ],
     ) -> SparsePwc:
         r"""
         Create the sum of multiple sparse-matrix-valued piecewise-constant functions.
 
         Parameters
         ----------
```

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/stf.py` & `boulder_opal-2.0.0/boulderopal/_nodes/stf.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,34 +14,36 @@
 from typing import (
     List,
     Optional,
     Union,
 )
 
 import numpy as np
+from pydantic import Field
 
 from boulderopal._nodes.base import create_operation
 from boulderopal._nodes.node_data import (
     ConvolutionKernel,
     Pwc,
     Stf,
     Tensor,
 )
 from boulderopal._nodes.validation import (
     ArrayT,
     ShapeT,
+    non_negative_scalar,
+    positive_scalar,
     scalar_or_shapeable,
     shapeable,
     starts_with_zero,
 )
 from boulderopal._typing import Annotated
 from boulderopal._validation import (
     Checker,
     ScalarT,
-    minimum_length,
     pipe,
     validated,
 )
 
 
 class StfGraph:  # pylint: disable=unused-argument
     """
@@ -184,17 +186,15 @@
         return Stf(
             operation=create_operation(self.constant_stf, locals()),
             value_shape=shape[batch_dimension_count:],
             batch_shape=shape[:batch_dimension_count],
         )
 
     @validated
-    def stf_sum(
-        self, terms: Annotated[List[Stf], pipe(after=minimum_length(1))]
-    ) -> Stf:
+    def stf_sum(self, terms: Annotated[List[Stf], Field(min_length=1)]) -> Stf:
         r"""
         Create the sum of multiple sampleable functions.
 
         Parameters
         ----------
         terms : list[Stf]
             The individual sampleable function :math:`\{v_j(t)\}` to sum.
@@ -472,15 +472,15 @@
         """
         operation = create_operation(self.convolve_pwc, locals())
         return Stf(operation, value_shape=pwc.value_shape, batch_shape=pwc.batch_shape)
 
     @validated
     def sinc_convolution_kernel(
         self,
-        cutoff_frequency: Union[Annotated[float, pipe(ScalarT.REAL().gt(0))], Tensor],
+        cutoff_frequency: Annotated[Union[float, Tensor], pipe(positive_scalar)],
     ) -> ConvolutionKernel:
         r"""
         Create a convolution kernel representing the sinc function.
 
         Use this kernel to eliminate angular frequencies above a certain cutoff.
 
         Parameters
@@ -530,24 +530,23 @@
         >>> filtered_signal
         <Stf: operation_name="convolve_pwc", value_shape=(), batch_shape=()>
 
         Refer to the `How to create leakage-robust single-qubit gates
         <https://docs.q-ctrl.com/boulder-opal/user-guides/how-to-create-leakage-robust-single-qubit-gates>`_
         user guide to find the example in context.
         """
-
         return ConvolutionKernel(
             create_operation(self.sinc_convolution_kernel, locals())
         )
 
     @validated
     def gaussian_convolution_kernel(
         self,
-        std: Union[Annotated[float, pipe(ScalarT.REAL().gt(0))], Tensor],
-        offset: Union[Annotated[float, pipe(ScalarT.REAL().ge(0))], Tensor] = 0,
+        std: Annotated[Union[float, Tensor], pipe(positive_scalar)],
+        offset: Annotated[Union[float, Tensor], pipe(non_negative_scalar)] = 0,
     ) -> ConvolutionKernel:
         r"""
         Create a convolution kernel representing a normalized Gaussian.
 
         Use this kernel to allow angular frequencies in the range roughly determined by
         its width, and progressively suppress components outside that range.
```

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/tensor.py` & `boulder_opal-2.0.0/boulderopal/_nodes/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     Literal,
     Optional,
     Tuple,
     Union,
 )
 
 import numpy as np
+from pydantic import Field
 
 from boulderopal._typing import Annotated
 from boulderopal._validation import (
     Checker,
     ScalarT,
-    minimum_length,
     pipe,
     sequence_like,
     type_pipe,
     validated,
 )
 
 from .base import create_operation
@@ -110,15 +110,15 @@
     @validated
     def concatenate(
         self,
         tensors: Annotated[
             List[
                 Annotated[Union[np.ndarray, Tensor], pipe(shapeable, after=no_scalar)]
             ],
-            pipe(after=minimum_length(2)),
+            Field(min_length=2),
         ],
         axis: Annotated[int, pipe(ScalarT.INT())],
         *,
         name: Optional[str] = None,
     ) -> Tensor:
         """
         Concatenate a list of tensors along a specified dimension.
@@ -627,15 +627,15 @@
         labels: Annotated[
             List[
                 Tuple[
                     Literal["I", "X", "Y", "Z", "M", "P"],
                     Annotated[int, pipe(ScalarT.INT().ge(0))],
                 ]
             ],
-            pipe(after=minimum_length(1)),
+            Field(min_length=1),
         ],
         subsystem_count: Annotated[int, pipe(ScalarT.INT().gt(0))],
         *,
         name: Optional[str] = None,
     ) -> Tensor:
         r"""
         Place Pauli matrices into their two-dimensional subsystems of a system and
@@ -1233,21 +1233,19 @@
     @validated
     def partial_trace(
         self,
         density_matrix: Annotated[
             Union[np.ndarray, Tensor], pipe(shapeable, after=ShapeT.OPERATOR())
         ],
         subsystem_dimensions: Annotated[
-            List[Annotated[int, pipe(ScalarT.INT().gt(0))]],
-            pipe(after=minimum_length(1)),
+            List[Annotated[int, pipe(ScalarT.INT().gt(0))]], Field(min_length=1)
         ],
         traced_subsystems: Union[
             Annotated[
-                List[Annotated[int, pipe(ScalarT.INT().ge(0))]],
-                pipe(after=minimum_length(1)),
+                List[Annotated[int, pipe(ScalarT.INT().ge(0))]], Field(min_length=1)
             ],
             Annotated[int, pipe(ScalarT.INT().ge(0))],
         ],
         *,
         name: Optional[str] = None,
     ) -> Tensor:
         r"""
@@ -1350,21 +1348,38 @@
 
         Parameters
         ----------
         tensor : np.ndarray or Tensor
             The tensor you want to reshape.
         shape : tuple[int, ...]
             The new shape of the tensor.
+            One and only one of the dimensions can be set to -1.
+            In that case, the method will automatically calculate that dimension's size by
+            keeping the total size constant.
         name : str or None, optional
             The name of the node.
 
         Returns
         -------
         Tensor
             The reshaped tensor.
+
+        Examples
+        --------
+        >>> graph.reshape(tensor=np.ones((4, 4)), shape=(2, 8), name='reshape')
+        <Tensor: name="reshape", operation_name="reshape", shape=(2, 8)>
+
+        >>> graph.reshape(tensor=np.ones((4, 4)), shape=(2, -1), name='reshape_1')
+        <Tensor: name="reshape_1", operation_name="reshape", shape=(2, 8)>
+
+        >>> graph.reshape(tensor=np.ones((4, 4)), shape=(2, -1, 2), name='reshape_2')
+        <Tensor: name="reshape_2", operation_name="reshape", shape=(2, 4, 2)>
+
+        >>> graph.reshape(tensor=np.ones((2, 2)), shape=(-1,), name='reshape_3')
+        <Tensor: name="reshape_3", operation_name="reshape", shape=(4,)>
         """
         tensor_element_count = np.prod(tensor.shape)
         shape_element_count = np.prod(shape)
 
         missing_dimensions = np.nonzero(np.asarray(shape) == -1)[0]
         if len(missing_dimensions) > 0:
             Checker.VALUE(
@@ -1767,15 +1782,15 @@
         self,
         operators: Annotated[
             List[
                 Annotated[
                     Union[np.ndarray, Tensor], pipe(shapeable, after=ShapeT.MATRIX())
                 ]
             ],
-            pipe(after=minimum_length(1)),
+            Field(min_length=1),
         ],
         *,
         name: Optional[str] = None,
     ) -> Tensor:
         r"""
         Calculate the Kronecker product between a list of operators.
```

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/utils.py` & `boulder_opal-2.0.0/boulderopal/_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_nodes/validation.py` & `boulder_opal-2.0.0/boulderopal/_nodes/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -279,7 +279,20 @@
         f"The variable {name} must be "
         "a real number, a real NumPy array, a Pwc, an Stf, or a real Tensor."
     )
 
 
 real_shapeable = type_pipe([_qutip_obj, ScalarT.REAL(), shapeable], _real_messenger)
 real_array = type_pipe([strict_real_array], messenger=_real_messenger)
+
+
+def _scalar_messenger(name: str) -> str:
+    return f"The {name} must be a scalar or a scalar-like Tensor."
+
+
+scalar = type_pipe([ScalarT.NUMERIC(), _to_scalar_tensor], _scalar_messenger)
+positive_scalar = type_pipe(
+    [ScalarT.REAL().gt(0), _to_scalar_tensor], _scalar_messenger
+)
+non_negative_scalar = type_pipe(
+    [ScalarT.REAL().ge(0), _to_scalar_tensor], _scalar_messenger
+)
```

### Comparing `boulder_opal-1.4.0/boulderopal/_typing.py` & `boulder_opal-2.0.0/boulderopal/_typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,19 @@
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
 import sys
-
-if sys.version_info.minor != 8:
-    from typing import (
-        Annotated,
-        get_args,
-        get_origin,
-    )
-else:
-    from typing_extensions import (  # type:ignore
-        Annotated,
-        get_args,
-        get_origin,
-    )
+from typing import (
+    Annotated,
+    get_args,
+    get_origin,
+)
 
 if sys.version_info >= (3, 10):
     from typing import (
         Concatenate,
         ParamSpec,
     )
 else:
```

### Comparing `boulder_opal-1.4.0/boulderopal/_utils.py` & `boulder_opal-2.0.0/boulderopal/_utils.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_validation/__init__.py` & `boulder_opal-2.0.0/boulderopal/_validation/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,26 +15,24 @@
     ArrayT,
     ScalarT,
     nullable,
     validate_enum,
 )
 from boulderopal._validation.exceptions import Checker
 from boulderopal._validation.pydantic import (
-    minimum_length,
     pipe,
     sequence_like,
     type_pipe,
     validated,
 )
 
 __all__ = [
     "ArrayT",
     "Checker",
     "ScalarT",
-    "minimum_length",
     "nullable",
     "pipe",
     "sequence_like",
     "type_pipe",
     "validated",
     "validate_enum",
 ]
```

### Comparing `boulder_opal-1.4.0/boulderopal/_validation/basic.py` & `boulder_opal-2.0.0/boulderopal/_validation/basic.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_validation/exceptions.py` & `boulder_opal-2.0.0/boulderopal/_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/_validation/graph.py` & `boulder_opal-2.0.0/boulderopal/_validation/graph.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/closed_loop/__init__.py` & `boulder_opal-2.0.0/boulderopal/closed_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/closed_loop/_optimization.py` & `boulder_opal-2.0.0/boulderopal/closed_loop/_optimization.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/closed_loop/_optimizers.py` & `boulder_opal-2.0.0/boulderopal/closed_loop/_optimizers.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/cloud.py` & `boulder_opal-2.0.0/boulderopal/cloud.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/gradient_free/__init__.py` & `boulder_opal-2.0.0/boulderopal/gradient_free/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/gradient_free/_optimization.py` & `boulder_opal-2.0.0/boulderopal/gradient_free/_optimization.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/graph/__init__.py` & `boulder_opal-2.0.0/boulderopal/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/graph/_execute_graph.py` & `boulder_opal-2.0.0/boulderopal/graph/_execute_graph.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/graph/_graph.py` & `boulder_opal-2.0.0/boulderopal/graph/_graph.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/ions/__init__.py` & `boulder_opal-2.0.0/boulderopal/ions/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/ions/_drives.py` & `boulder_opal-2.0.0/boulderopal/ions/_drives.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/ions/_ion_chain_properties.py` & `boulder_opal-2.0.0/boulderopal/ions/_ion_chain_properties.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/ions/_molmer_sorensen.py` & `boulder_opal-2.0.0/boulderopal/ions/_molmer_sorensen.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/noise_reconstruction/__init__.py` & `boulder_opal-2.0.0/boulderopal/noise_reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/noise_reconstruction/_classes.py` & `boulder_opal-2.0.0/boulderopal/noise_reconstruction/_classes.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/noise_reconstruction/_reconstruct.py` & `boulder_opal-2.0.0/boulderopal/noise_reconstruction/_reconstruct.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/optimization/__init__.py` & `boulder_opal-2.0.0/boulderopal/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/optimization/_optimization.py` & `boulder_opal-2.0.0/boulderopal/optimization/_optimization.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/signals/__init__.py` & `boulder_opal-2.0.0/boulderopal/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/signals/_functions.py` & `boulder_opal-2.0.0/boulderopal/signals/_functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/stochastic/__init__.py` & `boulder_opal-2.0.0/boulderopal/stochastic/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/stochastic/_optimization.py` & `boulder_opal-2.0.0/boulderopal/stochastic/_optimization.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/stochastic/_optimizer.py` & `boulder_opal-2.0.0/boulderopal/stochastic/_optimizer.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/superconducting/__init__.py` & `boulder_opal-2.0.0/boulderopal/superconducting/__init__.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/superconducting/_components.py` & `boulder_opal-2.0.0/boulderopal/superconducting/_components.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/superconducting/_drives.py` & `boulder_opal-2.0.0/boulderopal/superconducting/_drives.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/boulderopal/superconducting/_functions.py` & `boulder_opal-2.0.0/boulderopal/superconducting/_functions.py`

 * *Files identical despite different names*

### Comparing `boulder_opal-1.4.0/pyproject.toml` & `boulder_opal-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boulder-opal"
-version = "1.4.0"
+version = "2.0.0"
 description = "Boulder Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com/boulder-opal"
@@ -41,15 +41,14 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Software Development :: Embedded Systems",
@@ -73,21 +72,21 @@
 
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 priority = "primary"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.12"
+python = ">=3.9, <3.12"
 numpy = "^1.23.5"
-pydantic = ">=1.10.13, <3.0"
+pydantic = "^2.6.4"
 rich = "^13.6.0"
 typing-extensions = "^4.8.0"
-qctrl-commons = "^22.0.0"
-qctrl-workflow-client = { version = "~3.0.0", source = "PyPI" }
+qctrl-commons = { version = "^23.0.0", source = "PyPI" }
+qctrl-workflow-client = { version = "~4.0.0", source = "PyPI" }
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 isort = "^5.12.0"
 lemminflect = "^0.2.3"
 mypy = "^1.6.1"
 numpydoc = "^1.5.0"
@@ -96,18 +95,18 @@
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.11.1"
 pytest-xdist = "^3.3.1"
 sphinx = "5.3.0"
 tomli = "^2.0.1"
 types-requests= "^2.31.0"
-boulder-opal-core = {version = "50.0.2", python = ">=3.9"}
-qctrl-core-workflow-manager = "^3.0.0"
-qctrl-sphinx-theme = "^2.1.3"
-qctrl-client = "^9.1.0"
+boulder-opal-core = "^50.0.4"
+qctrl-core-workflow-manager = "^4.0.0"
+qctrl-client = "^10.0.0"
+sphinx-markdown-builder = "^0.6.6"
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = "2"
 
 [tool.mypy]
 files = ["boulderopal/**/*.py", "tests/**/*.py"]
```

### Comparing `boulder_opal-1.4.0/PKG-INFO` & `boulder_opal-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: boulder-opal
-Version: 1.4.0
+Version: 2.0.0
 Summary: Boulder Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pydantic (>=1.10.13,<3.0)
-Requires-Dist: qctrl-commons (>=22.0.0,<23.0.0)
-Requires-Dist: qctrl-workflow-client (>=3.0.0,<3.1.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: qctrl-commons (>=23.0.0,<24.0.0)
+Requires-Dist: qctrl-workflow-client (>=4.0.0,<4.1.0)
 Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
```

