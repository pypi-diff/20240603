# Comparing `tmp/pymimir-0.9.12.tar.gz` & `tmp/pymimir-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymimir-0.9.12.tar", last modified: Mon Jun  3 13:24:03 2024, max compression
+gzip compressed data, was "pymimir-0.9.9.tar", last modified: Sat Jun  1 20:19:46 2024, max compression
```

## Comparing `pymimir-0.9.12.tar` & `pymimir-0.9.9.tar`

### file list

```diff
@@ -1,326 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-06-03 13:23:49.000000 pymimir-0.9.12/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-06-03 13:23:49.000000 pymimir-0.9.12/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 13:23:49.000000 pymimir-0.9.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-06-03 13:23:49.000000 pymimir-0.9.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 13:24:03.669065 pymimir-0.9.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-06-03 13:23:49.000000 pymimir-0.9.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.633065 pymimir-0.9.12/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-03 13:23:49.000000 pymimir-0.9.12/cmake/configure_boost.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-03 13:23:49.000000 pymimir-0.9.12/cmake/configure_ccache.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 13:23:49.000000 pymimir-0.9.12/cmake/configure_loki.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.633065 pymimir-0.9.12/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-06-03 13:23:49.000000 pymimir-0.9.12/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/dependencies/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-06-03 13:23:49.000000 pymimir-0.9.12/dependencies/benchmark/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/dependencies/boost/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-03 13:23:49.000000 pymimir-0.9.12/dependencies/boost/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/dependencies/flatmemory/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-06-03 13:23:49.000000 pymimir-0.9.12/dependencies/flatmemory/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/dependencies/googletest/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-03 13:23:49.000000 pymimir-0.9.12/dependencies/googletest/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/dependencies/loki/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-03 13:23:49.000000 pymimir-0.9.12/dependencies/loki/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-06-03 13:23:49.000000 pymimir-0.9.12/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/exe/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-03 13:23:49.000000 pymimir-0.9.12/exe/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-06-03 13:23:49.000000 pymimir-0.9.12/exe/planner.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.625064 pymimir-0.9.12/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/include/mimir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/include/mimir/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/algorithms/kpkc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/algorithms/memory_pool.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/algorithms/murmurhash3.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/include/mimir/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/common/collections.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/common/concepts.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/common/itertools.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/common/printers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/common/random.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/common/timers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.637065 pymimir-0.9.12/include/mimir/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/datasets/state_space.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.641065 pymimir-0.9.12/include/mimir/formalism/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/action.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/atom.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/axiom.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/domain.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/effects.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34086 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/factories.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/formalism.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/function.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/function_expressions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/function_skeleton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/ground_atom.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/ground_function.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/ground_function_expressions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/ground_literal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/grounding_table.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/literal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/metric.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/numeric_fluent.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/object.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/parser.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/pddl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/predicate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/predicate_category.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/problem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/requirements.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/term.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.645064 pymimir-0.9.12/include/mimir/formalism/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)    31332 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/transformers/base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    39537 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/transformers/base_cached_recurse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/transformers/copy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/transformers/delete_relax.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/transformers/encode_parameter_index_in_variables.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/transformers/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/transformers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.645064 pymimir-0.9.12/include/mimir/formalism/translators/
--rw-r--r--   0 runner    (1001) docker     (127)    33324 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/base_cached_recurse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28787 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/base_recurse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/move_existential_quantifiers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/remove_types.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/remove_universal_quantifiers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/rename_quantified_variables.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/simplify_goal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/split_disjunctive_conditions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/to_disjunctive_normal_form.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/to_effect_normal_form.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/to_mimir_structures.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/to_negation_normal_form.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/translators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/formalism/variable.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/mimir.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.649065 pymimir-0.9.12/include/mimir/search/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.649065 pymimir-0.9.12/include/mimir/search/actions/
--rw-r--r--   0 runner    (1001) docker     (127)    19435 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/actions/dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/actions/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/actions/tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/actions.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.649065 pymimir-0.9.12/include/mimir/search/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/astar.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/brfs.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.649065 pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/default.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/statistics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/event_handlers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/algorithms.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.649065 pymimir-0.9.12/include/mimir/search/applicable_action_generators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.649065 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/default.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/statistics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/match_tree.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/assignment_set.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/consistency_graph.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/default.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/statistics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/grounding_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators/tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/applicable_action_generators.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/axiom_evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axiom_evaluators/axiom_stratification.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axiom_evaluators/dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axiom_evaluators/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axiom_evaluators/tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axiom_evaluators.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/axioms/
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axioms/dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axioms/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axioms/tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/axioms.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/builder.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.629064 pymimir-0.9.12/include/mimir/search/condition_grounders/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/condition_grounders/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/condition_grounders/event_handlers/default.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/condition_grounders/event_handlers/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/condition_grounders.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/flat_types.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/heuristics/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/heuristics/blind.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/heuristics/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/heuristics/tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/heuristics.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.653065 pymimir-0.9.12/include/mimir/search/openlists/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/openlists/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/openlists/priority_queue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/openlists/tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/openlists.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/plan.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/include/mimir/search/planners/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/planners/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/planners/single.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/planners.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/include/mimir/search/search_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/search_nodes/cost.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/search_nodes.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/include/mimir/search/states/
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/states/dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/states/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/states/tags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/states.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/include/mimir/search/successor_state_generators/
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/successor_state_generators/dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/successor_state_generators/interface.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/successor_state_generators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/translations.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/view.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-06-03 13:23:49.000000 pymimir-0.9.12/include/mimir/search/view_const.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-06-03 13:23:49.000000 pymimir-0.9.12/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.629064 pymimir-0.9.12/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/python/src/pymimir/
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/src/pymimir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40986 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/src/pymimir/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/src/pymimir/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/python/src/pymimir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 13:24:03.000000 pymimir-0.9.12/python/src/pymimir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-06-03 13:24:03.000000 pymimir-0.9.12/python/src/pymimir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:24:03.000000 pymimir-0.9.12/python/src/pymimir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:24:03.000000 pymimir-0.9.12/python/src/pymimir.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 13:24:03.000000 pymimir-0.9.12/python/src/pymimir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 13:24:03.000000 pymimir-0.9.12/python/src/pymimir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/python/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/tests/datasets/test_state_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/python/tests/formalism/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/tests/formalism/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/python/tests/search/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 13:23:49.000000 pymimir-0.9.12/python/tests/search/test_brfs.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:24:03.669065 pymimir-0.9.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-06-03 13:23:49.000000 pymimir-0.9.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/common/kpkc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/common/murmurhash3.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.657065 pymimir-0.9.12/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/datasets/state_space.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.661064 pymimir-0.9.12/src/formalism/
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/action.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/axiom.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/domain.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/effects.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/function.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/function_expressions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/function_skeleton.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/ground_function.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/ground_function_expressions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/metric.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/numeric_fluent.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/object.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/problem.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/requirements.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/term.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.661064 pymimir-0.9.12/src/formalism/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/transformers/delete_relax.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/transformers/encode_parameter_index_in_variables.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/formalism/translators/
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/move_existential_quantifiers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15263 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/remove_types.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/remove_universal_quantifiers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11304 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/rename_quantified_variables.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/simplify_goal.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/split_disjunctive_conditions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/to_disjunctive_normal_form.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/to_effect_normal_form.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    45110 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/to_mimir_structures.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/to_negation_normal_form.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/translators/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/formalism/variable.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/actions/dense.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.629064 pymimir-0.9.12/src/search/algorithms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/algorithms/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/algorithms/event_handlers/debug.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/algorithms/event_handlers/default.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/applicable_action_generators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.629064 pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded/event_handlers/debug.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded/event_handlers/default.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/consistency_graph.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/event_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/event_handlers/debug.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/event_handlers/default.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/axiom_evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/axiom_evaluators/axiom_stratification.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/axiom_evaluators/dense.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/axioms/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/axioms/dense.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/plan.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/src/search/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-06-03 13:23:49.000000 pymimir-0.9.12/src/search/states/dense.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/integration/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/integration/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/integration/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/integration/dependencies/boost/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/integration/dependencies/boost/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/integration/dependencies/flatmemory/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/integration/dependencies/flatmemory/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/integration/dependencies/loki/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/integration/dependencies/loki/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/integration/dependencies/mimir/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/integration/dependencies/mimir/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/integration/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.665065 pymimir-0.9.12/tests/unit/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/algorithms/memory_pool.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/datasets/state_space.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.633065 pymimir-0.9.12/tests/unit/formalism/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/formalism/translators/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/formalism/translators/remove_types.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/formalism/translators/remove_universal_quantifiers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/formalism/translators/to_disjunctive_normal_form.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/formalism/translators/to_negation_normal_form.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.633065 pymimir-0.9.12/tests/unit/search/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/actions/default.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/algorithms/astar.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    59294 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/algorithms/brfs.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/applicable_action_generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/applicable_action_generators/dense-grounded.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/applicable_action_generators/dense-lifted.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/heuristics/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/heuristics/blind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/openlists/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/openlists/priority_queue.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/planners/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/planners/single.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/search_nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/search_nodes/cost.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.633065 pymimir-0.9.12/tests/unit/search/states/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/states/bitset/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/states/bitset/bitset.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:24:03.669065 pymimir-0.9.12/tests/unit/search/successor_state_generators/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-06-03 13:23:49.000000 pymimir-0.9.12/tests/unit/search/successor_state_generators/dense.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/
+-rw-r--r--   0 simon     (1000) simon     (1000)     5508 2024-05-30 11:46:06.000000 pymimir-0.9.9/CMakeLists.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)     2020 2024-04-26 11:36:50.000000 pymimir-0.9.9/Config.cmake.in
+-rw-r--r--   0 simon     (1000) simon     (1000)    35149 2023-06-05 19:38:20.000000 pymimir-0.9.9/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)      609 2024-03-16 22:47:48.000000 pymimir-0.9.9/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1000)      328 2024-06-01 20:19:46.984371 pymimir-0.9.9/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     3818 2024-05-30 15:04:35.000000 pymimir-0.9.9/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/cmake/
+-rw-r--r--   0 simon     (1000) simon     (1000)      100 2024-01-23 12:01:44.000000 pymimir-0.9.9/cmake/configure_boost.cmake
+-rw-r--r--   0 simon     (1000) simon     (1000)      544 2024-02-22 10:03:11.000000 pymimir-0.9.9/cmake/configure_ccache.cmake
+-rw-r--r--   0 simon     (1000) simon     (1000)       66 2024-02-22 10:03:11.000000 pymimir-0.9.9/cmake/configure_loki.cmake
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/dependencies/
+-rw-r--r--   0 simon     (1000) simon     (1000)      831 2024-05-17 09:24:16.000000 pymimir-0.9.9/dependencies/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/dependencies/benchmark/
+-rw-r--r--   0 simon     (1000) simon     (1000)      583 2024-02-22 10:03:11.000000 pymimir-0.9.9/dependencies/benchmark/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/dependencies/boost/
+-rw-r--r--   0 simon     (1000) simon     (1000)      632 2024-05-23 10:50:53.000000 pymimir-0.9.9/dependencies/boost/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/dependencies/flatmemory/
+-rw-r--r--   0 simon     (1000) simon     (1000)      620 2024-05-17 09:24:16.000000 pymimir-0.9.9/dependencies/flatmemory/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/dependencies/googletest/
+-rw-r--r--   0 simon     (1000) simon     (1000)      525 2024-02-22 10:03:11.000000 pymimir-0.9.9/dependencies/googletest/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/dependencies/loki/
+-rw-r--r--   0 simon     (1000) simon     (1000)      651 2024-05-29 21:32:38.000000 pymimir-0.9.9/dependencies/loki/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/dependencies/pybind11/
+-rw-r--r--   0 simon     (1000) simon     (1000)      515 2024-02-22 10:03:11.000000 pymimir-0.9.9/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/exe/
+-rw-r--r--   0 simon     (1000) simon     (1000)      136 2024-03-16 22:47:48.000000 pymimir-0.9.9/exe/CMakeLists.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)     2975 2024-05-26 18:00:33.000000 pymimir-0.9.9/exe/planner.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.954371 pymimir-0.9.9/include/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/include/mimir/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/include/mimir/algorithms/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1226 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/algorithms/kpkc.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2449 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/algorithms/memory_pool.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1117 2023-11-17 13:04:00.000000 pymimir-0.9.9/include/mimir/algorithms/murmurhash3.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/include/mimir/common/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2073 2024-05-23 10:11:36.000000 pymimir-0.9.9/include/mimir/common/collections.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      907 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/common/concepts.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3856 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/common/itertools.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2007 2024-05-23 20:59:04.000000 pymimir-0.9.9/include/mimir/common/printers.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1167 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/common/random.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1411 2024-05-30 09:58:54.000000 pymimir-0.9.9/include/mimir/common/timers.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/include/mimir/datasets/
+-rw-r--r--   0 simon     (1000) simon     (1000)     4886 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/datasets/state_space.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/formalism/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3690 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/action.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3310 2024-05-29 09:54:55.000000 pymimir-0.9.9/include/mimir/formalism/atom.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2477 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/axiom.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3128 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/domain.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     5095 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/effects.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    34188 2024-05-30 09:58:54.000000 pymimir-0.9.9/include/mimir/formalism/factories.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1114 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/formalism.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1960 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/function.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     8430 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/function_expressions.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2020 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/function_skeleton.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3966 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/ground_atom.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1985 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/ground_function.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     7765 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/ground_function_expressions.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3384 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/ground_literal.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      801 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/grounding_table.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3220 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/literal.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2110 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/metric.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1968 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/numeric_fluent.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1931 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/object.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1769 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/parser.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1715 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/pddl.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3961 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/predicate.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2214 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/predicate_category.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     4458 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/problem.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1882 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/requirements.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2822 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/term.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/formalism/transformers/
+-rw-r--r--   0 simon     (1000) simon     (1000)    31332 2024-05-29 09:54:55.000000 pymimir-0.9.9/include/mimir/formalism/transformers/base.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    39537 2024-05-29 09:54:55.000000 pymimir-0.9.9/include/mimir/formalism/transformers/base_cached_recurse.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1448 2024-05-17 09:24:16.000000 pymimir-0.9.9/include/mimir/formalism/transformers/copy.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3574 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/transformers/delete_relax.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2339 2024-05-29 21:32:38.000000 pymimir-0.9.9/include/mimir/formalism/transformers/encode_parameter_index_in_variables.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     9882 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/transformers/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      916 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/transformers.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/formalism/translators/
+-rw-r--r--   0 simon     (1000) simon     (1000)    33324 2024-05-29 09:54:55.000000 pymimir-0.9.9/include/mimir/formalism/translators/base_cached_recurse.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    28787 2024-05-29 09:54:55.000000 pymimir-0.9.9/include/mimir/formalism/translators/base_recurse.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    10493 2024-04-26 11:36:50.000000 pymimir-0.9.9/include/mimir/formalism/translators/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2519 2024-05-17 09:24:16.000000 pymimir-0.9.9/include/mimir/formalism/translators/move_existential_quantifiers.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2263 2024-05-29 09:54:55.000000 pymimir-0.9.9/include/mimir/formalism/translators/remove_types.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3622 2024-05-27 12:54:59.000000 pymimir-0.9.9/include/mimir/formalism/translators/remove_universal_quantifiers.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     4977 2024-05-27 12:54:59.000000 pymimir-0.9.9/include/mimir/formalism/translators/rename_quantified_variables.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1846 2024-05-27 12:54:59.000000 pymimir-0.9.9/include/mimir/formalism/translators/simplify_goal.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2221 2024-04-26 11:36:50.000000 pymimir-0.9.9/include/mimir/formalism/translators/split_disjunctive_conditions.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2671 2024-04-26 11:36:50.000000 pymimir-0.9.9/include/mimir/formalism/translators/to_disjunctive_normal_form.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3076 2024-04-26 11:36:50.000000 pymimir-0.9.9/include/mimir/formalism/translators/to_effect_normal_form.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     9510 2024-05-29 09:54:55.000000 pymimir-0.9.9/include/mimir/formalism/translators/to_mimir_structures.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3903 2024-04-26 11:36:50.000000 pymimir-0.9.9/include/mimir/formalism/translators/to_negation_normal_form.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2795 2024-05-27 12:54:59.000000 pymimir-0.9.9/include/mimir/formalism/translators/utils.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1472 2024-04-26 11:36:50.000000 pymimir-0.9.9/include/mimir/formalism/translators.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2178 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/formalism/variable.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/isomorphism/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1084 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/isomorphism/exact.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1007 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/isomorphism/wl.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2101 2024-05-23 10:11:36.000000 pymimir-0.9.9/include/mimir/mimir.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/actions/
+-rw-r--r--   0 simon     (1000) simon     (1000)    19243 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/actions/dense.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2247 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/actions/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1385 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/actions/tags.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1159 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/actions.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/algorithms/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2715 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/algorithms/astar.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     7707 2024-05-29 21:32:38.000000 pymimir-0.9.9/include/mimir/search/algorithms/brfs.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1830 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/debug.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1840 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/default.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     4469 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     4040 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/statistics.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      993 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/algorithms/event_handlers.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1173 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/algorithms/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1016 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/algorithms.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/applicable_action_generators/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2132 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/debug.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2142 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/default.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     5243 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3426 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/statistics.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1125 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    13332 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/match_tree.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2932 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/
+-rw-r--r--   0 simon     (1000) simon     (1000)    13371 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/assignment_set.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     5344 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/consistency_graph.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2286 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/debug.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2296 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/default.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     5345 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     6064 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/statistics.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1117 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     4428 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2074 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/grounding_utils.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3732 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1776 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators/tags.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1250 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/applicable_action_generators.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/axiom_evaluators/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1987 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/axiom_evaluators/axiom_stratification.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     4479 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/axiom_evaluators/dense.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2239 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/axiom_evaluators/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1430 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/axiom_evaluators/tags.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1083 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/axiom_evaluators.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/axioms/
+-rw-r--r--   0 simon     (1000) simon     (1000)     7417 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/axioms/dense.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2118 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/axioms/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1377 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/axioms/tags.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1148 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/axioms.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1499 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/builder.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/include/mimir/search/condition_grounders/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/condition_grounders/event_handlers/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1307 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/condition_grounders/event_handlers/default.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1178 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/condition_grounders/event_handlers/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    11732 2024-05-30 15:03:52.000000 pymimir-0.9.9/include/mimir/search/condition_grounders.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1776 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/flat_types.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/heuristics/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1473 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/heuristics/blind.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1813 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/heuristics/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1955 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/heuristics/tags.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1132 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/heuristics.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/openlists/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1697 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/openlists/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1946 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/openlists/priority_queue.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1727 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/openlists/tags.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      924 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/openlists.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1478 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/plan.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/planners/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1158 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/planners/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1526 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/planners/single.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      912 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/planners.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/search_nodes/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3221 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/search_nodes/cost.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      891 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/search_nodes.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/states/
+-rw-r--r--   0 simon     (1000) simon     (1000)     7504 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/states/dense.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2376 2024-05-26 18:00:33.000000 pymimir-0.9.9/include/mimir/search/states/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1836 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/states/tags.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1143 2024-05-23 10:11:36.000000 pymimir-0.9.9/include/mimir/search/states.hpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/include/mimir/search/successor_state_generators/
+-rw-r--r--   0 simon     (1000) simon     (1000)     6758 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/successor_state_generators/dense.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2785 2024-06-01 20:13:09.000000 pymimir-0.9.9/include/mimir/search/successor_state_generators/interface.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1133 2024-05-22 20:30:59.000000 pymimir-0.9.9/include/mimir/search/successor_state_generators.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1503 2024-05-29 21:32:38.000000 pymimir-0.9.9/include/mimir/search/translations.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1430 2024-05-30 09:58:54.000000 pymimir-0.9.9/include/mimir/search/view.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1467 2024-05-30 09:58:54.000000 pymimir-0.9.9/include/mimir/search/view_const.hpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      544 2024-05-19 19:34:48.000000 pymimir-0.9.9/pyproject.toml
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/python/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/python/src/
+-rw-r--r--   0 simon     (1000) simon     (1000)      489 2024-05-19 19:34:48.000000 pymimir-0.9.9/python/src/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/python/src/pymimir/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1873 2024-05-30 15:03:52.000000 pymimir-0.9.9/python/src/pymimir/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)    36490 2024-05-30 15:03:52.000000 pymimir-0.9.9/python/src/pymimir/bindings.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)      491 2024-05-19 19:34:48.000000 pymimir-0.9.9/python/src/pymimir/main.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/python/src/pymimir.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)      328 2024-06-01 20:19:46.000000 pymimir-0.9.9/python/src/pymimir.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)    10770 2024-06-01 20:19:46.000000 pymimir-0.9.9/python/src/pymimir.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-06-01 20:19:46.000000 pymimir-0.9.9/python/src/pymimir.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-06-01 20:19:46.000000 pymimir-0.9.9/python/src/pymimir.egg-info/not-zip-safe
+-rw-r--r--   0 simon     (1000) simon     (1000)       27 2024-06-01 20:19:46.000000 pymimir-0.9.9/python/src/pymimir.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       17 2024-06-01 20:19:46.000000 pymimir-0.9.9/python/src/pymimir.egg-info/top_level.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/python/tests/
+-rw-r--r--   0 simon     (1000) simon     (1000)        0 2024-03-16 22:47:48.000000 pymimir-0.9.9/python/tests/__init__.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/python/tests/datasets/
+-rw-r--r--   0 simon     (1000) simon     (1000)      645 2024-05-30 15:03:52.000000 pymimir-0.9.9/python/tests/datasets/test_state_space.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/python/tests/formalism/
+-rw-r--r--   0 simon     (1000) simon     (1000)      494 2024-05-19 19:34:48.000000 pymimir-0.9.9/python/tests/formalism/test_parser.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/python/tests/search/
+-rw-r--r--   0 simon     (1000) simon     (1000)      694 2024-05-19 21:51:00.000000 pymimir-0.9.9/python/tests/search/test_brfs.py
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-06-01 20:19:46.984371 pymimir-0.9.9/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)     4183 2024-06-01 20:13:09.000000 pymimir-0.9.9/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/src/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1662 2024-05-30 11:46:10.000000 pymimir-0.9.9/src/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/src/common/
+-rw-r--r--   0 simon     (1000) simon     (1000)     5999 2024-03-14 13:40:22.000000 pymimir-0.9.9/src/common/kpkc.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     9319 2024-03-14 13:40:22.000000 pymimir-0.9.9/src/common/murmurhash3.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/src/datasets/
+-rw-r--r--   0 simon     (1000) simon     (1000)    10215 2024-05-30 15:03:52.000000 pymimir-0.9.9/src/datasets/state_space.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/src/formalism/
+-rw-r--r--   0 simon     (1000) simon     (1000)     7641 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/action.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3851 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/axiom.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     7165 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/domain.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     8038 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/effects.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2130 2024-05-22 20:30:59.000000 pymimir-0.9.9/src/formalism/function.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     6986 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/function_expressions.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1861 2024-05-22 20:30:59.000000 pymimir-0.9.9/src/formalism/function_skeleton.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2175 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/ground_function.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     7357 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/ground_function_expressions.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2119 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/metric.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1712 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/numeric_fluent.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1341 2024-05-22 20:30:59.000000 pymimir-0.9.9/src/formalism/object.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3387 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/parser.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    10958 2024-05-29 21:32:38.000000 pymimir-0.9.9/src/formalism/problem.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1825 2024-05-22 20:30:59.000000 pymimir-0.9.9/src/formalism/requirements.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2141 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/formalism/term.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.974371 pymimir-0.9.9/src/formalism/transformers/
+-rw-r--r--   0 simon     (1000) simon     (1000)    11659 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/transformers/delete_relax.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     7433 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/transformers/encode_parameter_index_in_variables.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/formalism/translators/
+-rw-r--r--   0 simon     (1000) simon     (1000)     4912 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/translators/move_existential_quantifiers.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    15263 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/translators/remove_types.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    11883 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/translators/remove_universal_quantifiers.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    11304 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/translators/rename_quantified_variables.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     5664 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/translators/simplify_goal.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     6432 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/translators/split_disjunctive_conditions.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     5566 2024-04-26 11:36:50.000000 pymimir-0.9.9/src/formalism/translators/to_disjunctive_normal_form.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     7264 2024-04-26 11:36:50.000000 pymimir-0.9.9/src/formalism/translators/to_effect_normal_form.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    45110 2024-05-29 09:54:55.000000 pymimir-0.9.9/src/formalism/translators/to_mimir_structures.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     6007 2024-04-26 11:36:50.000000 pymimir-0.9.9/src/formalism/translators/to_negation_normal_form.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     6869 2024-05-27 12:54:59.000000 pymimir-0.9.9/src/formalism/translators/utils.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1587 2024-05-27 12:54:59.000000 pymimir-0.9.9/src/formalism/variable.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/actions/
+-rw-r--r--   0 simon     (1000) simon     (1000)     8976 2024-06-01 20:13:09.000000 pymimir-0.9.9/src/search/actions/dense.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/src/search/algorithms/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/algorithms/event_handlers/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3120 2024-05-30 09:58:54.000000 pymimir-0.9.9/src/search/algorithms/event_handlers/debug.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2585 2024-05-30 09:58:54.000000 pymimir-0.9.9/src/search/algorithms/event_handlers/default.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/applicable_action_generators/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded/event_handlers/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3065 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded/event_handlers/debug.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     3081 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded/event_handlers/default.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    12251 2024-06-01 20:13:09.000000 pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/
+-rw-r--r--   0 simon     (1000) simon     (1000)     5709 2024-05-29 21:32:38.000000 pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/consistency_graph.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/event_handlers/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2310 2024-05-30 15:03:52.000000 pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/event_handlers/debug.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     2336 2024-05-30 15:03:52.000000 pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/event_handlers/default.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    21804 2024-06-01 20:13:09.000000 pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/axiom_evaluators/
+-rw-r--r--   0 simon     (1000) simon     (1000)     7799 2024-05-26 18:00:33.000000 pymimir-0.9.9/src/search/axiom_evaluators/axiom_stratification.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    12328 2024-06-01 20:13:09.000000 pymimir-0.9.9/src/search/axiom_evaluators/dense.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/axioms/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2374 2024-06-01 20:13:09.000000 pymimir-0.9.9/src/search/axioms/dense.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1328 2024-05-22 20:30:59.000000 pymimir-0.9.9/src/search/plan.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/src/search/states/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1797 2024-05-29 21:32:38.000000 pymimir-0.9.9/src/search/states/dense.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/
+-rw-r--r--   0 simon     (1000) simon     (1000)       22 2024-02-22 10:03:11.000000 pymimir-0.9.9/tests/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/integration/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1009 2024-05-19 19:34:48.000000 pymimir-0.9.9/tests/integration/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/integration/dependencies/
+-rw-r--r--   0 simon     (1000) simon     (1000)      166 2024-02-22 10:03:11.000000 pymimir-0.9.9/tests/integration/dependencies/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/integration/dependencies/boost/
+-rw-r--r--   0 simon     (1000) simon     (1000)      613 2024-02-22 10:03:11.000000 pymimir-0.9.9/tests/integration/dependencies/boost/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/integration/dependencies/flatmemory/
+-rw-r--r--   0 simon     (1000) simon     (1000)      517 2024-02-22 10:03:11.000000 pymimir-0.9.9/tests/integration/dependencies/flatmemory/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/integration/dependencies/loki/
+-rw-r--r--   0 simon     (1000) simon     (1000)      584 2024-02-22 10:03:11.000000 pymimir-0.9.9/tests/integration/dependencies/loki/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/integration/dependencies/mimir/
+-rw-r--r--   0 simon     (1000) simon     (1000)      615 2024-04-26 11:36:50.000000 pymimir-0.9.9/tests/integration/dependencies/mimir/CMakeLists.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)     3127 2024-05-26 18:00:33.000000 pymimir-0.9.9/tests/integration/main.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1403 2024-05-30 15:03:52.000000 pymimir-0.9.9/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/algorithms/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1000 2024-03-14 13:40:22.000000 pymimir-0.9.9/tests/unit/algorithms/memory_pool.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/datasets/
+-rw-r--r--   0 simon     (1000) simon     (1000)      684 2024-05-30 15:03:52.000000 pymimir-0.9.9/tests/unit/datasets/state_space.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/tests/unit/formalism/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/formalism/translators/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1393 2024-04-26 11:36:50.000000 pymimir-0.9.9/tests/unit/formalism/translators/remove_types.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1713 2024-05-17 09:24:16.000000 pymimir-0.9.9/tests/unit/formalism/translators/remove_universal_quantifiers.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1280 2024-05-29 21:32:38.000000 pymimir-0.9.9/tests/unit/formalism/translators/to_disjunctive_normal_form.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1179 2024-04-26 11:36:50.000000 pymimir-0.9.9/tests/unit/formalism/translators/to_negation_normal_form.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/tests/unit/search/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/actions/
+-rw-r--r--   0 simon     (1000) simon     (1000)      138 2024-04-26 11:36:50.000000 pymimir-0.9.9/tests/unit/search/actions/default.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/algorithms/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2306 2024-05-26 18:00:33.000000 pymimir-0.9.9/tests/unit/search/algorithms/astar.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)    59294 2024-06-01 20:13:09.000000 pymimir-0.9.9/tests/unit/search/algorithms/brfs.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/applicable_action_generators/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1901 2024-05-29 21:32:38.000000 pymimir-0.9.9/tests/unit/search/applicable_action_generators/dense-grounded.cpp
+-rw-r--r--   0 simon     (1000) simon     (1000)     1699 2024-05-30 15:03:52.000000 pymimir-0.9.9/tests/unit/search/applicable_action_generators/dense-lifted.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/heuristics/
+-rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-03-15 08:43:48.000000 pymimir-0.9.9/tests/unit/search/heuristics/blind.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/openlists/
+-rw-r--r--   0 simon     (1000) simon     (1000)      406 2024-03-14 13:40:22.000000 pymimir-0.9.9/tests/unit/search/openlists/priority_queue.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/planners/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1005 2024-05-19 19:34:48.000000 pymimir-0.9.9/tests/unit/search/planners/single.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/search_nodes/
+-rw-r--r--   0 simon     (1000) simon     (1000)     2841 2024-05-17 09:24:16.000000 pymimir-0.9.9/tests/unit/search/search_nodes/cost.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.964371 pymimir-0.9.9/tests/unit/search/states/
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/states/bitset/
+-rw-r--r--   0 simon     (1000) simon     (1000)      888 2024-05-26 18:00:33.000000 pymimir-0.9.9/tests/unit/search/states/bitset/bitset.cpp
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-06-01 20:19:46.984371 pymimir-0.9.9/tests/unit/search/successor_state_generators/
+-rw-r--r--   0 simon     (1000) simon     (1000)      712 2024-06-01 20:13:09.000000 pymimir-0.9.9/tests/unit/search/successor_state_generators/dense.cpp
```

### Comparing `pymimir-0.9.12/CMakeLists.txt` & `pymimir-0.9.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/Config.cmake.in` & `pymimir-0.9.9/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/LICENSE` & `pymimir-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/MANIFEST.in` & `pymimir-0.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/README.md` & `pymimir-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Mimir: Planner library
 
 Mimir is a C++20 planning library with Python bindings for grounded and lifted planning. We created Mimir to be 1) efficient, 2) easy to integrate, use, and extend. Mimir implements standard search algorithms such as breadth-first search and AStar search.
 
-## 1. Supported PDDL Requirements
+## Supported PDDL Requirements
 
 Mimir supports the following PDDL requirements in the grounded and lifting setting.
 
 - [x] :strips
 - [x] :typing
 - [x] :negative-preconditions
 - [x] :disjunctive-preconditions
@@ -15,83 +15,74 @@
 - [x] :universal-preconditions
 - [x] :quantified-preconditions
 - [x] :conditional-effects
 - [x] :adl
 - [x] :derived-predicates
 - [x] :action-costs
 
-## 2. Getting Started (Python)
+## Example C++ API
 
-### 2.1. Example Python API
+```cpp
+const auto parser = PDDLParser("domain.pddl", "problem.pddl")
+const auto aag = std::make_shared<LiftedAAG>(parser.get_problem(), parser.get_factories())
+const auto brfs = BrFsAlgorithm(aag)
+const auto [status, plan] = brfs.find_solution()
+```
+
+## Example Python API
 
 ```python
 parser = PDDLParser("domain.pddl", "problem.pddl")
 aag = LiftedAAG(parser.get_problem(), parser.get_factories())
 brfs = BrFsAlgorithm(aag)
 status, plan = brfs.find_solution()
 ```
 
-### 2.2. Installing the Python Bindings Pymimir
-
-Mimir is available on pypi.
-
-```console
-pip install pymimir
-```
-
-## 3. Getting Started (C++)
-
-### 3.1. Example C++ API
-
-```cpp
-const auto parser = PDDLParser("domain.pddl", "problem.pddl")
-const auto aag = std::make_shared<LiftedAAG>(parser.get_problem(), parser.get_factories())
-const auto brfs = BrFsAlgorithm(aag)
-const auto [status, plan] = brfs.find_solution()
-```
+## Getting Started
 
-### 3.2. Installing the Dependencies
+### Installing the Dependencies
 
 Mimir depends on the following set of libraries:
 
 - [Loki](https://github.com/drexlerd/Loki) for parsing PDDL files,
 - [Boost](boost.org) header-only libraries (Fusion, Spirit x3, Container),
 - [flatmemory](https://github.com/drexlerd/flatmemory) for flattening memory layouts of complex composite types,
+- [nauty and Traces](https://pallini.di.uniroma1.it/) for isomorphism testing,
 - [GoogleBenchmark](https://github.com/google/benchmark) for automated performance benchmarking, and
 - [GoogleTest](https://github.com/google/googletest) for unit testing.
 
 Run the following sequence of commands to commands to download, configure, build, and install all dependencies:
 
 ```console
 # Configure dependencies
 cmake -S dependencies -B dependencies/build -DCMAKE_INSTALL_PREFIX=dependencies/installs
 # Build and install dependencies
 cmake --build dependencies/build -j16
 ```
 
-### 3.3. Building Mimir
+### Building Mimir
 
 Run the following sequence of commands to configure, build, and install Mimir:
 
 ```console
 # Configure with installation prefixes of all dependencies
 cmake -S . -B build -DCMAKE_PREFIX_PATH=${PWD}/dependencies/installs
 # Build
 cmake --build build -j16
 # Install (optional)
 cmake --install build --prefix=<path/to/installation-directory>
 ```
 
-### 3.4. Creating your own Planner based on Mimir
+### Creating your own Planner based on Mimir
 
 We provide a CMake Superbuild project [here](https://github.com/simon-stahlberg/mimir/tree/dynamic/tests/integration) that downloads, builds, and installs Mimir and all its dependencies. We recommend using it as a dependency project for your project, similar to how we handle Mimir's dependencies.
 
-## 4.For Developers
+## For Developers
 
-### 4.1. IDE Support
+### IDE Support
 
 We developed Mimir in Visual Studio Code. We recommend installing the `C/C++` and `CMake Tools` extensions by Microsoft. To get maximum IDE support, you should set the following `Cmake: Configure Args` in the `CMake Tools` extension settings under `Workspace`:
 
 - `-DCMAKE_PREFIX_PATH=${workspaceFolder}/dependencies/installs`
 
 After running `CMake: Configure` in Visual Studio Code (ctrl + shift + p), you should see all include paths being correctly resolved.
 
@@ -99,14 +90,14 @@
 
 ```json
 {
     "cmake.configureArgs": [ "-DCMAKE_PREFIX_PATH=${workspaceFolder}/dependencies/installs" ]
 }
 ```
 
-### 4.2. Argument passing
+### Argument passing
 
 - Use prefix `ref_` for initialized output parameters and `out_` for non-initialized output parameters. Try to keep the number of output parameters as small as possible. Never use stack-allocated types as output parameters.
 
-### 4.3. Concepts
+### Concepts
 
-- Use prefixes `Is` or `Has` to obtain more meaningful names. Every template parameter must be constrained using a suitable concept.
+- Use prefixes `Is` or `Has` to obtain more meaningful names.
```

### Comparing `pymimir-0.9.12/cmake/configure_ccache.cmake` & `pymimir-0.9.9/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/dependencies/CMakeLists.txt` & `pymimir-0.9.9/dependencies/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/dependencies/benchmark/CMakeLists.txt` & `pymimir-0.9.9/dependencies/benchmark/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/dependencies/boost/CMakeLists.txt` & `pymimir-0.9.9/dependencies/boost/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/dependencies/flatmemory/CMakeLists.txt` & `pymimir-0.9.9/dependencies/flatmemory/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/dependencies/googletest/CMakeLists.txt` & `pymimir-0.9.9/dependencies/googletest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/dependencies/loki/CMakeLists.txt` & `pymimir-0.9.9/dependencies/loki/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/dependencies/pybind11/CMakeLists.txt` & `pymimir-0.9.9/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/exe/planner.cpp` & `pymimir-0.9.9/exe/planner.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -43,26 +43,22 @@
     std::cout << "Domain:" << std::endl;
     std::cout << *parser.get_domain() << std::endl;
 
     std::cout << std::endl;
     std::cout << "Problem:" << std::endl;
     std::cout << *parser.get_problem() << std::endl;
 
-    auto applicable_action_generator =
-        (grounded) ? std::shared_ptr<IDynamicAAG> { std::make_shared<GroundedDenseAAG>(parser.get_problem(),
-                                                                                       parser.get_factories(),
-                                                                                       std::make_shared<DebugGroundedAAGEventHandler>(false)) } :
-                     std::shared_ptr<IDynamicAAG> {
-                         std::make_shared<LiftedDenseAAG>(parser.get_problem(), parser.get_factories(), std::make_shared<DebugLiftedAAGEventHandler>(false))
-                     };
+    auto applicable_action_generator = (grounded) ?
+                                           std::shared_ptr<IDynamicAAG> { std::make_shared<GroundedDenseAAG>(parser.get_problem(), parser.get_factories()) } :
+                                           std::shared_ptr<IDynamicAAG> { std::make_shared<LiftedDenseAAG>(parser.get_problem(), parser.get_factories()) };
 
     auto successor_state_generator = std::shared_ptr<IDynamicSSG> { std::make_shared<DenseSSG>(applicable_action_generator) };
 
-    auto event_handler = (debug) ? std::shared_ptr<IAlgorithmEventHandler> { std::make_shared<DebugAlgorithmEventHandler>(false) } :
-                                   std::shared_ptr<IAlgorithmEventHandler> { std::make_shared<DefaultAlgorithmEventHandler>(false) };
+    auto event_handler = (debug) ? std::shared_ptr<IAlgorithmEventHandler> { std::make_shared<DebugAlgorithmEventHandler>() } :
+                                   std::shared_ptr<IAlgorithmEventHandler> { std::make_shared<DefaultAlgorithmEventHandler>() };
 
     auto lifted_brfs = std::make_shared<BrFsAlgorithm>(applicable_action_generator, successor_state_generator, event_handler);
 
     auto planner = std::make_shared<SinglePlanner>(std::move(lifted_brfs));
 
     auto [stats, plan] = planner->find_solution();
```

### Comparing `pymimir-0.9.12/include/mimir/algorithms/kpkc.hpp` & `pymimir-0.9.9/include/mimir/algorithms/kpkc.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/algorithms/memory_pool.hpp` & `pymimir-0.9.9/include/mimir/algorithms/memory_pool.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/algorithms/murmurhash3.hpp` & `pymimir-0.9.9/include/mimir/algorithms/murmurhash3.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/common/collections.hpp` & `pymimir-0.9.9/include/mimir/common/collections.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/common/concepts.hpp` & `pymimir-0.9.9/include/mimir/common/concepts.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/common/itertools.hpp` & `pymimir-0.9.9/include/mimir/common/itertools.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/common/printers.hpp` & `pymimir-0.9.9/include/mimir/common/printers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/common/random.hpp` & `pymimir-0.9.9/include/mimir/common/random.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/common/timers.hpp` & `pymimir-0.9.9/include/mimir/common/timers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/datasets/state_space.hpp` & `pymimir-0.9.9/include/mimir/datasets/state_space.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 
 #include "mimir/search/actions.hpp"
 #include "mimir/search/algorithms/brfs.hpp"
 #include "mimir/search/applicable_action_generators.hpp"
 #include "mimir/search/states.hpp"
 #include "mimir/search/successor_state_generators.hpp"
 
-#include <cstddef>
 #include <loki/loki.hpp>
-#include <unordered_map>
-#include <vector>
 
 namespace mimir
 {
 
 class Transition
 {
 private:
@@ -67,17 +64,14 @@
     std::vector<Transitions> m_backward_transitions;
 
     std::vector<int> m_goal_distances;
 
     StateSet m_goal_states;
     StateSet m_deadend_states;
 
-    StateMap<size_t> m_state_indices;
-    std::unordered_map<int, StateList> m_states_by_goal_distance;
-
     /// @brief Constructs a state state from data.
     /// The create function calls this constructor and ensures that
     /// the state space is in a legal state allowing other parts of
     /// the code base to operate on the invariants in the implementation.
     StateSpaceImpl(PDDLParser parser,
                    std::shared_ptr<GroundedAAG> aag,
                    std::shared_ptr<SuccessorStateGenerator> ssg,
@@ -120,33 +114,25 @@
 
     const std::vector<Transitions>& get_forward_transitions() const;
 
     const std::vector<Transitions>& get_backward_transitions() const;
 
     const std::vector<int>& get_goal_distances() const;
 
-    int get_goal_distance(const State& state) const;
-
-    int get_max_goal_distance() const;
-
     const StateSet& get_goal_states() const;
 
     const StateSet& get_deadend_states() const;
 
     size_t get_num_states() const;
 
     size_t get_num_transitions() const;
 
     size_t get_num_goal_states() const;
 
     size_t get_num_deadend_states() const;
-
-    bool is_deadend_state(const State& state) const;
-
-    State sample_state_with_goal_distance(int goal_distance) const;
 };
 
 using StateSpace = std::shared_ptr<StateSpaceImpl>;
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/formalism/action.hpp` & `pymimir-0.9.9/include/mimir/formalism/action.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/atom.hpp` & `pymimir-0.9.9/include/mimir/formalism/atom.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/axiom.hpp` & `pymimir-0.9.9/include/mimir/formalism/axiom.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/domain.hpp` & `pymimir-0.9.9/include/mimir/formalism/domain.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/effects.hpp` & `pymimir-0.9.9/include/mimir/formalism/effects.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/factories.hpp` & `pymimir-0.9.9/include/mimir/formalism/factories.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -572,27 +572,29 @@
         }
         else
         {
             static_assert(dependent_false<P>::value, "Missing implementation for PredicateCategory.");
         }
     }
 
-    template<PredicateCategory P, std::ranges::forward_range Iterable>
-    void get_ground_atoms_from_ids(const Iterable& atom_ids, GroundAtomList<P>& out_ground_atoms) const
+    template<PredicateCategory P, flatmemory::IsBitset Bitset>
+        requires flatmemory::HasCompatibleTagType<Bitset, P>
+    void get_ground_atoms_from_ids(const Bitset& atom_ids, GroundAtomList<P>& out_ground_atoms) const
     {
         out_ground_atoms.clear();
 
         for (const auto& atom_id : atom_ids)
         {
             out_ground_atoms.push_back(get_ground_atom<P>(atom_id));
         }
     }
 
-    template<PredicateCategory P, std::ranges::forward_range Iterable>
-    GroundAtomList<P> get_ground_atoms_from_ids(const Iterable& atom_ids) const
+    template<PredicateCategory P, flatmemory::IsBitset Bitset>
+        requires flatmemory::HasCompatibleTagType<Bitset, P>
+    GroundAtomList<P> get_ground_atoms_from_ids(const Bitset& atom_ids) const
     {
         auto result = GroundAtomList<P> {};
         get_ground_atoms_from_ids(atom_ids, result);
         return result;
     }
 
     // Object
```

### Comparing `pymimir-0.9.12/include/mimir/formalism/formalism.hpp` & `pymimir-0.9.9/include/mimir/formalism/formalism.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/function.hpp` & `pymimir-0.9.9/include/mimir/formalism/function.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/function_expressions.hpp` & `pymimir-0.9.9/include/mimir/formalism/function_expressions.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/function_skeleton.hpp` & `pymimir-0.9.9/include/mimir/formalism/function_skeleton.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/ground_atom.hpp` & `pymimir-0.9.9/include/mimir/formalism/ground_atom.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/ground_function.hpp` & `pymimir-0.9.9/include/mimir/formalism/ground_function.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/ground_function_expressions.hpp` & `pymimir-0.9.9/include/mimir/formalism/ground_function_expressions.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/ground_literal.hpp` & `pymimir-0.9.9/include/mimir/formalism/ground_literal.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/grounding_table.hpp` & `pymimir-0.9.9/include/mimir/formalism/grounding_table.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/literal.hpp` & `pymimir-0.9.9/include/mimir/formalism/literal.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/metric.hpp` & `pymimir-0.9.9/include/mimir/formalism/metric.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/numeric_fluent.hpp` & `pymimir-0.9.9/include/mimir/formalism/numeric_fluent.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/object.hpp` & `pymimir-0.9.9/include/mimir/formalism/object.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/parser.hpp` & `pymimir-0.9.9/include/mimir/formalism/parser.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/pddl.hpp` & `pymimir-0.9.9/include/mimir/formalism/pddl.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/predicate.hpp` & `pymimir-0.9.9/include/mimir/formalism/predicate.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/predicate_category.hpp` & `pymimir-0.9.9/include/mimir/formalism/predicate_category.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/problem.hpp` & `pymimir-0.9.9/include/mimir/formalism/problem.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/requirements.hpp` & `pymimir-0.9.9/include/mimir/formalism/requirements.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/term.hpp` & `pymimir-0.9.9/include/mimir/formalism/term.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/transformers/base.hpp` & `pymimir-0.9.9/include/mimir/formalism/transformers/base.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/transformers/base_cached_recurse.hpp` & `pymimir-0.9.9/include/mimir/formalism/transformers/base_cached_recurse.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/transformers/copy.hpp` & `pymimir-0.9.9/include/mimir/formalism/transformers/copy.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/transformers/delete_relax.hpp` & `pymimir-0.9.9/include/mimir/formalism/transformers/delete_relax.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/transformers/encode_parameter_index_in_variables.hpp` & `pymimir-0.9.9/include/mimir/formalism/transformers/encode_parameter_index_in_variables.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/transformers/interface.hpp` & `pymimir-0.9.9/include/mimir/formalism/transformers/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/transformers.hpp` & `pymimir-0.9.9/include/mimir/formalism/transformers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/base_cached_recurse.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/base_cached_recurse.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/base_recurse.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/base_recurse.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/interface.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/move_existential_quantifiers.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/move_existential_quantifiers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/remove_types.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/remove_types.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/remove_universal_quantifiers.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/remove_universal_quantifiers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/rename_quantified_variables.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/rename_quantified_variables.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/simplify_goal.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/simplify_goal.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/split_disjunctive_conditions.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/split_disjunctive_conditions.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/to_disjunctive_normal_form.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/to_disjunctive_normal_form.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/to_effect_normal_form.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/to_effect_normal_form.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/to_mimir_structures.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/to_mimir_structures.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/to_negation_normal_form.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/to_negation_normal_form.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators/utils.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators/utils.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/translators.hpp` & `pymimir-0.9.9/include/mimir/formalism/translators.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/formalism/variable.hpp` & `pymimir-0.9.9/include/mimir/formalism/variable.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/mimir.hpp` & `pymimir-0.9.9/include/mimir/mimir.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/actions/dense.hpp` & `pymimir-0.9.9/include/mimir/search/actions/dense.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -221,31 +221,25 @@
         else
         {
             static_assert(dependent_false<P>::value, "Missing implementation for PredicateCategory.");
         }
     }
 
     template<PredicateCategory P>
-    [[nodiscard]] bool is_applicable(const Problem problem, const DenseState state) const
+    [[nodiscard]] bool is_applicable(const DenseState state) const
     {
-        const auto state_atoms = state.get_atoms<P>(problem);
+        const auto state_atoms = state.get_atoms<P>();
 
         return state_atoms.is_superseteq(get_positive_precondition<P>())  //
                && state_atoms.are_disjoint(get_negative_precondition<P>());
     }
 
-    [[nodiscard]] bool is_applicable(const Problem problem, const DenseState state) const
+    [[nodiscard]] bool is_applicable(const DenseState state) const
     {
-        return is_applicable<Fluent>(problem, state) && is_applicable<Static>(problem, state) && is_applicable<Derived>(problem, state);
-    }
-
-    template<flatmemory::IsBitset Bitset>
-    [[nodiscard]] bool is_statically_applicable(const Bitset static_positive_atoms) const
-    {
-        return is_applicable<Static>(static_positive_atoms);
+        return is_applicable<Fluent>(state) && is_applicable<Static>(state) && is_applicable<Derived>(state);
     }
 
     template<PredicateCategory P, flatmemory::IsBitset Bitset>
         requires flatmemory::HasCompatibleTagType<Bitset, P>
     [[nodiscard]] bool is_applicable(const Bitset& atoms) const
     {
         return atoms.is_superseteq(get_positive_precondition<P>())  //
@@ -253,14 +247,20 @@
     }
 
     template<flatmemory::IsBitset Bitset1, flatmemory::IsBitset Bitset2, flatmemory::IsBitset Bitset3>
     [[nodiscard]] bool is_applicable(const Bitset1 fluent_state_atoms, const Bitset2 derived_state_atoms, const Bitset3 static_positive_bitset) const
     {
         return is_applicable<Fluent>(fluent_state_atoms) && is_applicable<Static>(static_positive_bitset) && is_applicable<Derived>(derived_state_atoms);
     }
+
+    template<flatmemory::IsBitset Bitset>
+    [[nodiscard]] bool is_statically_applicable(const Bitset static_positive_atoms) const
+    {
+        return is_applicable<Static>(static_positive_atoms);
+    }
 };
 
 class DenseStripsActionEffectBuilderProxy
 {
 private:
     FlatDenseStripsActionEffectBuilder& m_builder;
 
@@ -392,25 +392,25 @@
         }
     }
 
     /* Simple effects */
     [[nodiscard]] const FlatSimpleEffect& get_simple_effect() const { return m_view.get<6>(); }
 
     template<PredicateCategory P>
-    [[nodiscard]] bool is_applicable(const Problem problem, const DenseState state) const
+    [[nodiscard]] bool is_applicable(const DenseState state) const
     {
-        const auto state_atoms = state.get_atoms<P>(problem);
+        const auto state_atoms = state.get_atoms<P>();
 
         return state_atoms.is_superseteq(get_positive_precondition<P>())  //
                && state_atoms.are_disjoint(get_negative_precondition<P>());
     }
 
-    [[nodiscard]] bool is_applicable(const Problem problem, const DenseState state) const
+    [[nodiscard]] bool is_applicable(const DenseState state) const
     {
-        return is_applicable<Fluent>(problem, state) && is_applicable<Static>(problem, state) && is_applicable<Derived>(problem, state);
+        return is_applicable<Fluent>(state) && is_applicable<Static>(state) && is_applicable<Derived>(state);
     }
 };
 
 template<>
 class Builder<ActionDispatcher<DenseStateTag>> :
     public IBuilder<Builder<ActionDispatcher<DenseStateTag>>>,
     public IActionBuilder<Builder<ActionDispatcher<DenseStateTag>>>
@@ -485,17 +485,17 @@
 
     /* STRIPS part */
     [[nodiscard]] FlatDenseStripsActionPrecondition get_strips_precondition() const { return m_view.get<4>(); }
     [[nodiscard]] FlatDenseStripsActionEffect get_strips_effect() const { return m_view.get<5>(); }
     /* Conditional effects */
     [[nodiscard]] FlatDenseConditionalEffects get_conditional_effects() const { return m_view.get<6>(); }
 
-    [[nodiscard]] bool is_applicable(const Problem problem, DenseState state) const
+    [[nodiscard]] bool is_applicable(DenseState state) const
     {  //
-        return DenseStripsActionPrecondition(get_strips_precondition()).is_applicable(problem, state);
+        return DenseStripsActionPrecondition(get_strips_precondition()).is_applicable(state);
     }
 
     template<flatmemory::IsBitset Bitset>
     [[nodiscard]] bool is_statically_applicable(const Bitset static_positive_bitset) const
     {  //
         return DenseStripsActionPrecondition(get_strips_precondition()).is_statically_applicable(static_positive_bitset);
     }
```

### Comparing `pymimir-0.9.12/include/mimir/search/actions/interface.hpp` & `pymimir-0.9.9/include/mimir/search/actions/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/actions/tags.hpp` & `pymimir-0.9.9/include/mimir/search/actions/tags.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/actions.hpp` & `pymimir-0.9.9/include/mimir/search/actions.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/astar.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/astar.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/brfs.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/brfs.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -102,32 +102,30 @@
         m_search_nodes(flat::CostSearchNodeVector(create_default_search_node_builder())),
         m_event_handler(std::move(event_handler))
     {
     }
 
     SearchStatus find_solution(GroundActionList& out_plan) override
     {
-        const auto problem = m_successor_generator->get_problem();
-        const auto& pddl_factories = m_successor_generator->get_pddl_factories();
-        m_event_handler->on_start_search(problem, this->m_initial_state, pddl_factories);
+        m_event_handler->on_start_search(this->m_initial_state, m_successor_generator->get_pddl_factories());
 
         auto initial_search_node = CostSearchNode(this->m_search_nodes[this->m_initial_state.get_id()]);
         initial_search_node.get_g_value() = 0;
         initial_search_node.get_status() = SearchNodeStatus::OPEN;
 
-        const auto& static_goal_ground_literals = problem->get_static_goal_condition();
-        if (!m_initial_state.literals_hold(problem, static_goal_ground_literals))
+        const auto& static_goal_ground_literals = m_successor_generator->get_problem()->get_static_goal_condition();
+        if (!m_initial_state.literals_hold(static_goal_ground_literals))
         {
             m_event_handler->on_unsolvable();
 
             return SearchStatus::UNSOLVABLE;
         }
 
-        const auto& fluent_goal_ground_literals = problem->get_fluent_goal_condition();
-        const auto& derived_goal_ground_literals = problem->get_derived_goal_condition();
+        const auto& fluent_goal_ground_literals = m_successor_generator->get_problem()->get_fluent_goal_condition();
+        const auto& derived_goal_ground_literals = m_successor_generator->get_problem()->get_derived_goal_condition();
 
         auto applicable_actions = GroundActionList {};
 
         m_queue.emplace_back(m_initial_state);
 
         auto g_value = uint64_t { 0 };
 
@@ -142,15 +140,15 @@
             if (static_cast<uint64_t>(search_node.get_g_value()) > g_value)
             {
                 g_value = search_node.get_g_value();
                 m_successor_generator->on_finish_f_layer();
                 m_event_handler->on_finish_f_layer();
             }
 
-            if (state.literals_hold(problem, fluent_goal_ground_literals) && state.literals_hold(problem, derived_goal_ground_literals))
+            if (state.literals_hold(fluent_goal_ground_literals) && state.literals_hold(derived_goal_ground_literals))
             {
                 set_plan(ConstCostSearchNode(this->m_search_nodes[state.get_id()]), out_plan);
 
                 m_event_handler->on_end_search();
                 m_successor_generator->on_end_search();
                 m_event_handler->on_solved(out_plan);
 
@@ -158,24 +156,24 @@
             }
 
             if (g_value == 1)
             {
                 // return SearchStatus::FAILED;
             }
 
-            m_event_handler->on_expand_state(problem, state, pddl_factories);
+            m_event_handler->on_expand_state(state, m_successor_generator->get_pddl_factories());
 
             this->m_successor_generator->generate_applicable_actions(state, applicable_actions);
 
             for (const auto& action : applicable_actions)
             {
                 const auto state_count = m_state_repository->get_state_count();
                 const auto& successor_state = this->m_state_repository->get_or_create_successor_state(state, action);
 
-                m_event_handler->on_generate_state(problem, action, successor_state, pddl_factories);
+                m_event_handler->on_generate_state(action, successor_state, m_successor_generator->get_pddl_factories());
 
                 if (state_count != m_state_repository->get_state_count())
                 {
                     auto successor_search_node = CostSearchNode(this->m_search_nodes[successor_state.get_id()]);
                     successor_search_node.get_status() = SearchNodeStatus::OPEN;
                     successor_search_node.get_g_value() = search_node.get_g_value() + 1;
                     successor_search_node.get_parent_state_id() = state.get_id();
```

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/debug.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/debug.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -30,30 +30,27 @@
  */
 class DebugAlgorithmEventHandler : public AlgorithmEventHandlerBase<DebugAlgorithmEventHandler>
 {
 private:
     /* Implement AlgorithmEventHandlerBase interface */
     friend class AlgorithmEventHandlerBase<DebugAlgorithmEventHandler>;
 
-    void on_generate_state_impl(const Problem problem, GroundAction action, const State successor_state, const PDDLFactories& pddl_factories) const;
+    void on_generate_state_impl(GroundAction action, State successor_state, const PDDLFactories& pddl_factories) const;
 
     void on_finish_f_layer_impl(uint64_t f_value, uint64_t num_expanded_states, uint64_t num_generated_states) const;
 
-    void on_expand_state_impl(const Problem problem, const State state, const PDDLFactories& pddl_factories) const;
+    void on_expand_state_impl(State state, const PDDLFactories& pddl_factories) const;
 
-    void on_start_search_impl(const Problem problem, const State initial_state, const PDDLFactories& pddl_factories) const;
+    void on_start_search_impl(State initial_state, const PDDLFactories& pddl_factories) const;
 
     void on_end_search_impl() const;
 
     void on_solved_impl(const GroundActionList& ground_action_plan) const;
 
     void on_unsolvable_impl() const;
 
     void on_exhausted_impl() const;
-
-public:
-    explicit DebugAlgorithmEventHandler(bool quiet = true) : AlgorithmEventHandlerBase<DebugAlgorithmEventHandler>(quiet) {}
 };
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/default.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/default.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -30,30 +30,27 @@
  */
 class DefaultAlgorithmEventHandler : public AlgorithmEventHandlerBase<DefaultAlgorithmEventHandler>
 {
 private:
     /* Implement AlgorithmEventHandlerBase interface */
     friend class AlgorithmEventHandlerBase<DefaultAlgorithmEventHandler>;
 
-    void on_generate_state_impl(const Problem problem, const GroundAction action, const State successor_state, const PDDLFactories& pddl_factories) const;
+    void on_generate_state_impl(GroundAction action, State successor_state, const PDDLFactories& pddl_factories) const;
 
     void on_finish_f_layer_impl(uint64_t f_value, uint64_t num_expanded_states, uint64_t num_generated_states) const;
 
-    void on_expand_state_impl(const Problem problem, const State state, const PDDLFactories& pddl_factories) const;
+    void on_expand_state_impl(State state, const PDDLFactories& pddl_factories) const;
 
-    void on_start_search_impl(const Problem problem, const State initial_state, const PDDLFactories& pddl_factories) const;
+    void on_start_search_impl(State initial_state, const PDDLFactories& pddl_factories) const;
 
     void on_end_search_impl() const;
 
     void on_solved_impl(const GroundActionList& ground_action_plan) const;
 
     void on_unsolvable_impl() const;
 
     void on_exhausted_impl() const;
-
-public:
-    explicit DefaultAlgorithmEventHandler(bool quiet = true) : AlgorithmEventHandlerBase<DefaultAlgorithmEventHandler>(quiet) {}
 };
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/interface.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/interface.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -34,24 +34,24 @@
  */
 class IAlgorithmEventHandler
 {
 public:
     virtual ~IAlgorithmEventHandler() = default;
 
     /// @brief React on generating a successor_state by applying an action.
-    virtual void on_generate_state(const Problem problem, const GroundAction action, const State successor_state, const PDDLFactories& pddl_factories) = 0;
+    virtual void on_generate_state(GroundAction action, State successor_state, const PDDLFactories& pddl_factories) = 0;
 
     /// @brief React on finishing expanding a f-layer.
     virtual void on_finish_f_layer() = 0;
 
     /// @brief React on expanding a state.
-    virtual void on_expand_state(const Problem problem, const State state, const PDDLFactories& pddl_factories) = 0;
+    virtual void on_expand_state(State state, const PDDLFactories& pddl_factories) = 0;
 
     /// @brief React on starting a search.
-    virtual void on_start_search(const Problem problem, const State initial_state, const PDDLFactories& pddl_factories) = 0;
+    virtual void on_start_search(State initial_state, const PDDLFactories& pddl_factories) = 0;
 
     /// @brief React on ending a search.
     virtual void on_end_search() = 0;
 
     /// @brief React on solving a search.
     virtual void on_solved(const GroundActionList& ground_action_plan) = 0;
 
@@ -70,103 +70,67 @@
  * Collect statistics and call implementation of derived class.
  */
 template<typename Derived>
 class AlgorithmEventHandlerBase : public IAlgorithmEventHandler
 {
 protected:
     AlgorithmStatistics m_statistics;
-    bool m_quiet;
 
 private:
     AlgorithmEventHandlerBase() = default;
     friend Derived;
 
     /// @brief Helper to cast to Derived.
     constexpr const auto& self() const { return static_cast<const Derived&>(*this); }
     constexpr auto& self() { return static_cast<Derived&>(*this); }
 
 public:
-    explicit AlgorithmEventHandlerBase(bool quiet = true) : m_statistics(), m_quiet(quiet) {}
-
-    void on_generate_state(const Problem problem, const GroundAction action, const State successor_state, const PDDLFactories& pddl_factories) override
+    void on_generate_state(GroundAction action, State successor_state, const PDDLFactories& pddl_factories) override
     {
         m_statistics.increment_num_generated();
 
-        if (!m_quiet)
-        {
-            self().on_generate_state_impl(problem, action, successor_state, pddl_factories);
-        }
+        self().on_generate_state_impl(action, successor_state, pddl_factories);
     }
 
     void on_finish_f_layer() override
     {
         m_statistics.on_finish_f_layer();
 
-        if (!m_quiet)
-        {
-            assert(!m_statistics.get_num_expanded_until_f_value().empty());
-            self().on_finish_f_layer_impl(m_statistics.get_num_expanded_until_f_value().size() - 1,
-                                          m_statistics.get_num_expanded_until_f_value().back(),
-                                          m_statistics.get_num_generated_until_f_value().back());
-        }
+        assert(!m_statistics.get_num_expanded_until_f_value().empty());
+        self().on_finish_f_layer_impl(m_statistics.get_num_expanded_until_f_value().size() - 1,
+                                      m_statistics.get_num_expanded_until_f_value().back(),
+                                      m_statistics.get_num_generated_until_f_value().back());
     }
 
-    void on_expand_state(const Problem problem, const State state, const PDDLFactories& pddl_factories) override
+    void on_expand_state(State state, const PDDLFactories& pddl_factories) override
     {
         m_statistics.increment_num_expanded();
 
-        if (!m_quiet)
-        {
-            self().on_expand_state_impl(problem, state, pddl_factories);
-        }
+        self().on_expand_state_impl(state, pddl_factories);
     }
 
-    void on_start_search(const Problem problem, const State initial_state, const PDDLFactories& pddl_factories) override
+    void on_start_search(State initial_state, const PDDLFactories& pddl_factories) override
     {
         m_statistics.set_search_start_time_point(std::chrono::high_resolution_clock::now());
 
-        if (!m_quiet)
-        {
-            self().on_start_search_impl(problem, initial_state, pddl_factories);
-        }
+        self().on_start_search_impl(initial_state, pddl_factories);
     }
 
     void on_end_search() override
     {
         m_statistics.set_search_end_time_point(std::chrono::high_resolution_clock::now());
 
-        if (!m_quiet)
-        {
-            self().on_end_search_impl();
-        }
+        self().on_end_search_impl();
     }
 
-    void on_solved(const GroundActionList& ground_action_plan) override
-    {
-        if (!m_quiet)
-        {
-            self().on_solved_impl(ground_action_plan);
-        }
-    }
+    void on_solved(const GroundActionList& ground_action_plan) override { self().on_solved_impl(ground_action_plan); }
 
-    void on_unsolvable() override
-    {
-        if (!m_quiet)
-        {
-            self().on_unsolvable_impl();
-        }
-    }
+    void on_unsolvable() override { self().on_unsolvable_impl(); }
 
-    void on_exhausted() override
-    {
-        if (!m_quiet)
-        {
-            self().on_exhausted_impl();
-        }
-    }
+    void on_exhausted() override { self().on_exhausted_impl(); }
 
     /// @brief Get the statistics.
     const AlgorithmStatistics& get_statistics() const override { return m_statistics; }
 };
 
 }
```

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/event_handlers/statistics.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/event_handlers/statistics.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/event_handlers.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/event_handlers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms/interface.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/algorithms.hpp` & `pymimir-0.9.9/include/mimir/search/algorithms.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/debug.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/debug.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,12 @@
     void on_finish_grounding_unrelaxed_axioms_impl(const GroundAxiomList& unrelaxed_axioms);
 
     void on_finish_build_axiom_match_tree_impl(const MatchTree<GroundAxiom>& axiom_match_tree);
 
     void on_finish_f_layer_impl() const;
 
     void on_end_search_impl() const;
-
-public:
-    explicit DebugGroundedAAGEventHandler(bool quiet = true) : GroundedAAGEventHandlerBase<DebugGroundedAAGEventHandler>(quiet) {}
 };
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/default.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/default.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,12 @@
     void on_finish_grounding_unrelaxed_axioms_impl(const GroundAxiomList& unrelaxed_axioms);
 
     void on_finish_build_axiom_match_tree_impl(const MatchTree<GroundAxiom>& axiom_match_tree);
 
     void on_finish_f_layer_impl() const;
 
     void on_end_search_impl() const;
-
-public:
-    explicit DefaultGroundedAAGEventHandler(bool quiet = true) : GroundedAAGEventHandlerBase<DefaultGroundedAAGEventHandler>(quiet) {}
 };
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/interface.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/interface.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -65,97 +65,73 @@
  * Collect statistics and call implementation of derived class.
  */
 template<typename Derived_>
 class GroundedAAGEventHandlerBase : public IGroundedAAGEventHandler
 {
 protected:
     GroundedAAGStatistics m_statistics;
-    bool m_quiet;
 
 private:
     GroundedAAGEventHandlerBase() = default;
     friend Derived_;
 
     /// @brief Helper to cast to Derived.
     constexpr const auto& self() const { return static_cast<const Derived_&>(*this); }
     constexpr auto& self() { return static_cast<Derived_&>(*this); }
 
 public:
-    explicit GroundedAAGEventHandlerBase(bool quiet = true) : m_statistics(), m_quiet(quiet) {}
-
     void on_finish_delete_free_exploration(const GroundAtomList<Fluent>& reached_fluent_atoms,
                                            const GroundAtomList<Derived>& reached_derived_atoms,
                                            const GroundActionList& instantiated_actions,
                                            const GroundAxiomList& instantiated_axioms) override
     {  //
         m_statistics.set_num_delete_free_reachable_fluent_ground_atoms(reached_fluent_atoms.size());
         m_statistics.set_num_delete_free_reachable_derived_ground_atoms(reached_derived_atoms.size());
         m_statistics.set_num_delete_free_actions(instantiated_actions.size());
         m_statistics.set_num_delete_free_axioms(instantiated_axioms.size());
 
-        if (!m_quiet)
-        {
-            self().on_finish_delete_free_exploration_impl(reached_fluent_atoms, reached_derived_atoms, instantiated_actions, instantiated_axioms);
-        }
+        self().on_finish_delete_free_exploration_impl(reached_fluent_atoms, reached_derived_atoms, instantiated_actions, instantiated_axioms);
     }
 
     void on_finish_grounding_unrelaxed_actions(const GroundActionList& unrelaxed_actions) override
     {  //
         m_statistics.set_num_ground_actions(unrelaxed_actions.size());
 
-        if (!m_quiet)
-        {
-            self().on_finish_grounding_unrelaxed_actions_impl(unrelaxed_actions);
-        }
+        self().on_finish_grounding_unrelaxed_actions_impl(unrelaxed_actions);
     }
 
     void on_finish_build_action_match_tree(const MatchTree<GroundAction>& action_match_tree) override
     {  //
         m_statistics.set_num_nodes_in_action_match_tree(action_match_tree.get_num_nodes());
 
-        if (!m_quiet)
-        {
-            self().on_finish_build_action_match_tree_impl(action_match_tree);
-        }
+        self().on_finish_build_action_match_tree_impl(action_match_tree);
     }
 
     void on_finish_grounding_unrelaxed_axioms(const GroundAxiomList& unrelaxed_axioms) override
     {  //
         m_statistics.set_num_ground_axioms(unrelaxed_axioms.size());
 
-        if (!m_quiet)
-        {
-            self().on_finish_grounding_unrelaxed_axioms_impl(unrelaxed_axioms);
-        }
+        self().on_finish_grounding_unrelaxed_axioms_impl(unrelaxed_axioms);
     }
 
     void on_finish_build_axiom_match_tree(const MatchTree<GroundAxiom>& axiom_match_tree) override
     {  //
         m_statistics.set_num_nodes_in_axiom_match_tree(axiom_match_tree.get_num_nodes());
 
-        if (!m_quiet)
-        {
-            self().on_finish_build_axiom_match_tree_impl(axiom_match_tree);
-        }
+        self().on_finish_build_axiom_match_tree_impl(axiom_match_tree);
     }
 
     void on_finish_f_layer() override
     {  //
-        if (!m_quiet)
-        {
-            self().on_finish_f_layer_impl();
-        }
+        self().on_finish_f_layer_impl();
     }
 
     void on_end_search() override
     {  //
-        if (!m_quiet)
-        {
-            self().on_end_search_impl();
-        }
+        self().on_end_search_impl();
     }
 
     const GroundedAAGStatistics& get_statistics() const override { return m_statistics; }
 };
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/statistics.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers/statistics.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/event_handlers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded/match_tree.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded/match_tree.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_grounded.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_grounded.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/assignment_set.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/assignment_set.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/consistency_graph.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/consistency_graph.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/debug.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/default.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,27 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program. If not, see <https://www.gnu.org/licenses/>.
  */
 
-#ifndef MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEBUG_HPP_
-#define MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEBUG_HPP_
+#ifndef MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEFAULT_HPP_
+#define MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEFAULT_HPP_
 
 #include "mimir/search/applicable_action_generators/dense_lifted/event_handlers/interface.hpp"
 
 namespace mimir
 {
 
-class DebugLiftedAAGEventHandler : public LiftedAAGEventHandlerBase<DebugLiftedAAGEventHandler>
+class DefaultLiftedAAGEventHandler : public LiftedAAGEventHandlerBase<DefaultLiftedAAGEventHandler>
 {
 private:
     /* Implement LiftedAAGEventHandlerBase interface */
-    friend class LiftedAAGEventHandlerBase<DebugLiftedAAGEventHandler>;
+    friend class LiftedAAGEventHandlerBase<DefaultLiftedAAGEventHandler>;
 
     void on_start_generating_applicable_actions_impl() const;
 
     void on_ground_action_impl(const Action action, const ObjectList& binding) const;
 
     void on_ground_action_cache_hit_impl(const Action action, const ObjectList& binding) const;
 
@@ -48,15 +48,12 @@
     void on_ground_axiom_cache_miss_impl(const Axiom axiom, const ObjectList& binding) const;
 
     void on_end_generating_applicable_axioms_impl(const GroundAxiomList& ground_axioms, const PDDLFactories& pddl_factories) const;
 
     void on_finish_f_layer_impl() const;
 
     void on_end_search_impl() const;
-
-public:
-    explicit DebugLiftedAAGEventHandler(bool quiet = true) : LiftedAAGEventHandlerBase<DebugLiftedAAGEventHandler>(quiet) {}
 };
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/default.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/debug.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -11,27 +11,27 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program. If not, see <https://www.gnu.org/licenses/>.
  */
 
-#ifndef MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEFAULT_HPP_
-#define MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEFAULT_HPP_
+#ifndef MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEBUG_HPP_
+#define MIMIR_SEARCH_APPLICABLE_ACTION_GENERATORS_DENSE_LIFTED_EVENT_HANDLERS_DEBUG_HPP_
 
 #include "mimir/search/applicable_action_generators/dense_lifted/event_handlers/interface.hpp"
 
 namespace mimir
 {
 
-class DefaultLiftedAAGEventHandler : public LiftedAAGEventHandlerBase<DefaultLiftedAAGEventHandler>
+class DebugLiftedAAGEventHandler : public LiftedAAGEventHandlerBase<DebugLiftedAAGEventHandler>
 {
 private:
     /* Implement LiftedAAGEventHandlerBase interface */
-    friend class LiftedAAGEventHandlerBase<DefaultLiftedAAGEventHandler>;
+    friend class LiftedAAGEventHandlerBase<DebugLiftedAAGEventHandler>;
 
     void on_start_generating_applicable_actions_impl() const;
 
     void on_ground_action_impl(const Action action, const ObjectList& binding) const;
 
     void on_ground_action_cache_hit_impl(const Action action, const ObjectList& binding) const;
 
@@ -48,15 +48,12 @@
     void on_ground_axiom_cache_miss_impl(const Axiom axiom, const ObjectList& binding) const;
 
     void on_end_generating_applicable_axioms_impl(const GroundAxiomList& ground_axioms, const PDDLFactories& pddl_factories) const;
 
     void on_finish_f_layer_impl() const;
 
     void on_end_search_impl() const;
-
-public:
-    explicit DefaultLiftedAAGEventHandler(bool quiet = true) : LiftedAAGEventHandlerBase<DefaultLiftedAAGEventHandler>(quiet) {}
 };
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/interface.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/interface.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -71,131 +71,92 @@
  * Collect statistics and call implementation of derived class.
  */
 template<typename Derived>
 class LiftedAAGEventHandlerBase : public ILiftedAAGEventHandler
 {
 protected:
     LiftedAAGStatistics m_statistics;
-    bool m_quiet;
 
 private:
     LiftedAAGEventHandlerBase() = default;
     friend Derived;
 
     /// @brief Helper to cast to Derived.
     constexpr const auto& self() const { return static_cast<const Derived&>(*this); }
     constexpr auto& self() { return static_cast<Derived&>(*this); }
 
 public:
-    explicit LiftedAAGEventHandlerBase(bool quiet = true) : m_statistics(), m_quiet(quiet) {}
-
     void on_start_generating_applicable_actions() override
-    {
-        if (!m_quiet)
-        {
-            self().on_start_generating_applicable_actions_impl();
-        }
+    {  //
+        self().on_start_generating_applicable_actions_impl();
     }
 
     void on_ground_action(const Action action, const ObjectList& binding) override
-    {
-        if (!m_quiet)
-        {
-            self().on_ground_action_impl(action, binding);
-        }
+    {  //
+        self().on_ground_action_impl(action, binding);
     }
 
     void on_ground_action_cache_hit(const Action action, const ObjectList& binding) override
-    {
+    {  //
         m_statistics.increment_num_ground_action_cache_hits();
 
-        if (!m_quiet)
-        {
-            self().on_ground_action_cache_hit_impl(action, binding);
-        }
+        self().on_ground_action_cache_hit_impl(action, binding);
     }
 
     void on_ground_action_cache_miss(const Action action, const ObjectList& binding) override
-    {
+    {  //
         m_statistics.increment_num_ground_action_cache_misses();
 
-        if (!m_quiet)
-        {
-            self().on_ground_action_cache_miss_impl(action, binding);
-        }
+        self().on_ground_action_cache_miss_impl(action, binding);
     }
 
     void on_end_generating_applicable_actions(const GroundActionList& ground_actions, const PDDLFactories& pddl_factories) override
-    {
-        if (!m_quiet)
-        {
-            self().on_end_generating_applicable_actions_impl(ground_actions, pddl_factories);
-        }
+    {  //
+        self().on_end_generating_applicable_actions_impl(ground_actions, pddl_factories);
     }
 
     void on_start_generating_applicable_axioms() override
-    {
-        if (!m_quiet)
-        {
-            self().on_start_generating_applicable_axioms_impl();
-        }
+    {  //
+        self().on_start_generating_applicable_axioms_impl();
     }
 
     void on_ground_axiom(const Axiom axiom, const ObjectList& binding) override
-    {
-        if (!m_quiet)
-        {
-            self().on_ground_axiom_impl(axiom, binding);
-        }
+    {  //
+        self().on_ground_axiom_impl(axiom, binding);
     }
 
     void on_ground_axiom_cache_hit(const Axiom axiom, const ObjectList& binding) override
-    {
+    {  //
         m_statistics.increment_num_ground_axiom_cache_hits();
 
-        if (!m_quiet)
-        {
-            self().on_ground_axiom_cache_hit_impl(axiom, binding);
-        }
+        self().on_ground_axiom_cache_hit_impl(axiom, binding);
     }
 
     void on_ground_axiom_cache_miss(const Axiom axiom, const ObjectList& binding) override
-    {
+    {  //
         m_statistics.increment_num_ground_axiom_cache_misses();
 
-        if (!m_quiet)
-        {
-            self().on_ground_axiom_cache_miss_impl(axiom, binding);
-        }
+        self().on_ground_axiom_cache_miss_impl(axiom, binding);
     }
 
     void on_end_generating_applicable_axioms(const GroundAxiomList& ground_axioms, const PDDLFactories& pddl_factories) override
-    {
-        if (!m_quiet)
-        {
-            self().on_end_generating_applicable_axioms_impl(ground_axioms, pddl_factories);
-        }
+    {  //
+        self().on_end_generating_applicable_axioms_impl(ground_axioms, pddl_factories);
     }
 
     void on_finish_f_layer() override
-    {
+    {  //
         m_statistics.on_finish_f_layer();
 
-        if (!m_quiet)
-        {
-            self().on_finish_f_layer_impl();
-        }
+        self().on_finish_f_layer_impl();
     }
 
     void on_end_search() override
-    {
-        if (!m_quiet)
-        {
-            self().on_end_search_impl();
-        }
+    {  //
+        self().on_end_search_impl();
     }
 
     const LiftedAAGStatistics& get_statistics() const override { return m_statistics; }
 };
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/statistics.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers/statistics.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted/event_handlers.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/dense_lifted.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/dense_lifted.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/grounding_utils.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/grounding_utils.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/interface.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators/tags.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators/tags.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/applicable_action_generators.hpp` & `pymimir-0.9.9/include/mimir/search/applicable_action_generators.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axiom_evaluators/axiom_stratification.hpp` & `pymimir-0.9.9/include/mimir/search/axiom_evaluators/axiom_stratification.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axiom_evaluators/dense.hpp` & `pymimir-0.9.9/include/mimir/search/axiom_evaluators/dense.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -38,35 +38,37 @@
 
 namespace mimir
 {
 
 class PartiallyExtendedState
 {
 private:
+    const Problem& m_problem;
     const FlatBitsetBuilder<Fluent>& m_fluent_state_atoms;
     FlatBitsetBuilder<Derived>& m_ref_derived_state_atoms;
 
 public:
-    PartiallyExtendedState(const FlatBitsetBuilder<Fluent>& fluent_state_atoms, FlatBitsetBuilder<Derived>& ref_derived_state_atoms) :
+    PartiallyExtendedState(const Problem& problem, const FlatBitsetBuilder<Fluent>& fluent_state_atoms, FlatBitsetBuilder<Derived>& ref_derived_state_atoms) :
+        m_problem(problem),
         m_fluent_state_atoms(fluent_state_atoms),
         m_ref_derived_state_atoms(ref_derived_state_atoms)
     {
     }
 
-    bool literal_holds(const Problem problem, GroundLiteral<Static> static_literal) const
+    bool literal_holds(GroundLiteral<Static> static_literal) const
     {
-        return problem->get_static_initial_positive_atoms_bitset().get(static_literal->get_atom()->get_identifier()) != static_literal->is_negated();
+        return m_problem->get_static_initial_positive_atoms_bitset().get(static_literal->get_atom()->get_identifier()) != static_literal->is_negated();
     }
 
-    bool literal_holds(const Problem, GroundLiteral<Fluent> fluent_literal) const
+    bool literal_holds(GroundLiteral<Fluent> fluent_literal) const
     {
         return m_fluent_state_atoms.get(fluent_literal->get_atom()->get_identifier()) != fluent_literal->is_negated();
     }
 
-    bool literal_holds(const Problem, GroundLiteral<Derived> derived_literal) const
+    bool literal_holds(GroundLiteral<Derived> derived_literal) const
     {
         return m_ref_derived_state_atoms.get(derived_literal->get_atom()->get_identifier()) != derived_literal->is_negated();
     }
 };
 
 /**
  * Fully specialized implementation class.
```

### Comparing `pymimir-0.9.12/include/mimir/search/axiom_evaluators/interface.hpp` & `pymimir-0.9.9/include/mimir/search/axiom_evaluators/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axiom_evaluators/tags.hpp` & `pymimir-0.9.9/include/mimir/search/axiom_evaluators/tags.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axiom_evaluators.hpp` & `pymimir-0.9.9/include/mimir/search/axiom_evaluators.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axioms/dense.hpp` & `pymimir-0.9.9/include/mimir/search/axioms/dense.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axioms/interface.hpp` & `pymimir-0.9.9/include/mimir/search/axioms/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axioms/tags.hpp` & `pymimir-0.9.9/include/mimir/search/axioms/tags.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/axioms.hpp` & `pymimir-0.9.9/include/mimir/search/axioms.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/builder.hpp` & `pymimir-0.9.9/include/mimir/search/builder.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/condition_grounders/event_handlers/default.hpp` & `pymimir-0.9.9/include/mimir/search/condition_grounders/event_handlers/default.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/condition_grounders/event_handlers/interface.hpp` & `pymimir-0.9.9/include/mimir/search/condition_grounders/event_handlers/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/condition_grounders.hpp` & `pymimir-0.9.9/include/mimir/search/condition_grounders.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -35,29 +35,23 @@
 #include <stdexcept>
 #include <utility>
 
 namespace mimir
 {
 
 template<typename S>
-concept HasLiteralHolds =
-    requires(S state, Problem problem, GroundLiteral<Static> static_literal, GroundLiteral<Fluent> fluent_literal, GroundLiteral<Derived> derived_literal) {
-        {
-            state.literal_holds(problem, static_literal)
-        } -> std::convertible_to<bool>;
-        {
-            state.literal_holds(problem, fluent_literal)
-        } -> std::convertible_to<bool>;
-        {
-            state.literal_holds(problem, derived_literal)
-        } -> std::convertible_to<bool>;
-    };
+concept HasLiteralHolds = requires(S state, GroundLiteral<Static> static_literal, GroundLiteral<Fluent> fluent_literal, GroundLiteral<Derived> derived_literal)
+{
+    { state.literal_holds(static_literal) } -> std::convertible_to<bool>;
+    { state.literal_holds(fluent_literal) } -> std::convertible_to<bool>;
+    { state.literal_holds(derived_literal) } -> std::convertible_to<bool>;
+};
 
 template<typename State>
-    requires HasLiteralHolds<State>
+requires HasLiteralHolds<State>
 class ConditionGrounder
 {
 private:
     Problem m_problem;
     VariableList m_variables;
     LiteralList<Static> m_static_conditions;
     LiteralList<Fluent> m_fluent_conditions;
@@ -65,66 +59,66 @@
     AssignmentSet<Static> m_static_assignment_set;
     PDDLFactories& m_ref_pddl_factories;
     std::shared_ptr<IConditionGrounderEventHandler> m_event_handler;
 
     consistency_graph::StaticConsistencyGraph m_static_consistency_graph;
 
     template<PredicateCategory P>
-    bool is_valid_binding(const Problem problem, const LiteralList<P>& literals, const State state, const ObjectList& binding)
+    bool is_valid_binding(const LiteralList<P>& literals, const State state, const ObjectList& binding)
     {
         for (const auto& literal : literals)
         {
             auto ground_literal = m_ref_pddl_factories.ground_literal(literal, binding);
 
-            if (!state.literal_holds(problem, ground_literal))
+            if (!state.literal_holds(ground_literal))
             {
                 return false;
             }
         }
 
         return true;
     }
 
-    bool is_valid_binding(const Problem problem, const State state, const ObjectList& binding)
+    bool is_valid_binding(const State state, const ObjectList& binding)
     {
-        return is_valid_binding(problem, m_static_conditions, state, binding)       // We need to test all
-               && is_valid_binding(problem, m_fluent_conditions, state, binding)    // types of conditions
-               && is_valid_binding(problem, m_derived_conditions, state, binding);  // due to over-approx.
+        return is_valid_binding(m_static_conditions, state, binding)       // We need to test all
+               && is_valid_binding(m_fluent_conditions, state, binding)    // types of conditions
+               && is_valid_binding(m_derived_conditions, state, binding);  // due to over-approx.
     }
 
     template<PredicateCategory P>
-    bool nullary_literals_hold(const LiteralList<P>& literals, const Problem problem, const State state, PDDLFactories& pddl_factories)
+    bool nullary_literals_hold(const LiteralList<P>& literals, const State state, PDDLFactories& pddl_factories)
     {
         for (const auto& literal : literals)
         {
             if (literal->get_atom()->get_predicate()->get_arity() == 0)
             {
-                if (!state.literal_holds(problem, pddl_factories.ground_literal(literal, {})))
+                if (!state.literal_holds(pddl_factories.ground_literal(literal, {})))
                 {
                     return false;
                 }
             }
         }
 
         return true;
     }
 
     /// @brief Returns true if all nullary literals in the precondition hold, false otherwise.
-    bool nullary_conditions_hold(const Problem problem, const State state)
+    bool nullary_conditions_hold(const State state)
     {
-        return (nullary_literals_hold(m_fluent_conditions, problem, state, m_ref_pddl_factories))
-               && (nullary_literals_hold(m_derived_conditions, problem, state, m_ref_pddl_factories));
+        return (nullary_literals_hold(m_fluent_conditions, state, m_ref_pddl_factories))
+               && (nullary_literals_hold(m_derived_conditions, state, m_ref_pddl_factories));
     }
 
     void nullary_case(const State state, std::vector<ObjectList>& ref_bindings)
     {
         // There are no parameters, meaning that the preconditions are already fully ground. Simply check if the single ground action is applicable.
         auto binding = ObjectList {};
 
-        if (is_valid_binding(m_problem, state, binding))
+        if (is_valid_binding(state, binding))
         {
             ref_bindings.emplace_back(std::move(binding));
         }
         else
         {
             m_event_handler->on_invalid_binding(binding, m_ref_pddl_factories);
         }
@@ -138,15 +132,15 @@
         for (const auto& vertex : m_static_consistency_graph.get_vertices())
         {
             if (fluent_assignment_sets.literal_all_consistent(m_fluent_conditions, vertex)
                 && derived_assignment_sets.literal_all_consistent(m_derived_conditions, vertex))
             {
                 auto binding = ObjectList { m_ref_pddl_factories.get_object(vertex.get_object_index()) };
 
-                if (is_valid_binding(m_problem, state, binding))
+                if (is_valid_binding(state, binding))
                 {
                     ref_bindings.emplace_back(std::move(binding));
                 }
                 else
                 {
                     m_event_handler->on_invalid_binding(binding, m_ref_pddl_factories);
                 }
@@ -200,15 +194,15 @@
             {
                 const auto& vertex = vertices[clique[index]];
                 const auto param_index = vertex.get_param_index();
                 const auto object_id = vertex.get_object_index();
                 binding[param_index] = m_ref_pddl_factories.get_object(object_id);
             }
 
-            if (is_valid_binding(m_problem, state, binding))
+            if (is_valid_binding(state, binding))
             {
                 ref_bindings.emplace_back(std::move(binding));
             }
             else
             {
                 m_event_handler->on_invalid_binding(binding, m_ref_pddl_factories);
             }
@@ -274,15 +268,15 @@
     void compute_bindings(const State state,
                           const AssignmentSet<Fluent>& fluent_assignment_set,
                           const AssignmentSet<Derived>& derived_assignment_set,
                           std::vector<ObjectList>& out_bindings)
     {
         out_bindings.clear();
 
-        if (nullary_conditions_hold(m_problem, state))
+        if (nullary_conditions_hold(state))
         {
             if (m_variables.size() == 0)
             {
                 nullary_case(state, out_bindings);
             }
             else if (m_variables.size() == 1)
             {
```

### Comparing `pymimir-0.9.12/include/mimir/search/flat_types.hpp` & `pymimir-0.9.9/include/mimir/search/flat_types.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/heuristics/blind.hpp` & `pymimir-0.9.9/include/mimir/search/heuristics/blind.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/heuristics/interface.hpp` & `pymimir-0.9.9/include/mimir/search/heuristics/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/heuristics/tags.hpp` & `pymimir-0.9.9/include/mimir/search/heuristics/tags.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/heuristics.hpp` & `pymimir-0.9.9/include/mimir/search/heuristics.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/openlists/interface.hpp` & `pymimir-0.9.9/include/mimir/search/openlists/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/openlists/priority_queue.hpp` & `pymimir-0.9.9/include/mimir/search/openlists/priority_queue.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/openlists/tags.hpp` & `pymimir-0.9.9/include/mimir/search/openlists/tags.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/openlists.hpp` & `pymimir-0.9.9/include/mimir/search/openlists.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/plan.hpp` & `pymimir-0.9.9/include/mimir/search/plan.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/planners/interface.hpp` & `pymimir-0.9.9/include/mimir/search/planners/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/planners/single.hpp` & `pymimir-0.9.9/include/mimir/search/planners/single.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/planners.hpp` & `pymimir-0.9.9/include/mimir/search/planners.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/search_nodes/cost.hpp` & `pymimir-0.9.9/include/mimir/search/search_nodes/cost.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/search_nodes.hpp` & `pymimir-0.9.9/include/mimir/search/search_nodes.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/states/dense.hpp` & `pymimir-0.9.9/include/mimir/search/states/dense.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -23,43 +23,45 @@
 #include "mimir/formalism/formalism.hpp"
 #include "mimir/search/flat_types.hpp"
 #include "mimir/search/states/interface.hpp"
 
 #include <flatmemory/flatmemory.hpp>
 #include <ostream>
 #include <tuple>
-#include <unordered_map>
 
 namespace mimir
 {
 /**
  * Flatmemory types
  */
-using FlatDenseStateLayout = flatmemory::Tuple<uint32_t, FlatBitsetLayout<Fluent>, FlatBitsetLayout<Derived>>;
+using FlatDenseStateLayout = flatmemory::Tuple<uint32_t, FlatBitsetLayout<Fluent>, FlatBitsetLayout<Derived>, Problem>;
 using FlatDenseStateBuilder = flatmemory::Builder<FlatDenseStateLayout>;
 using FlatDenseState = flatmemory::ConstView<FlatDenseStateLayout>;
 
 // Only hash/compare the non-extended portion of a state, and the problem.
 // The extended portion is computed automatically, when calling ssg.create_state(...)
 struct FlatDenseStateHash
 {
     size_t operator()(const FlatDenseState& view) const
     {
         const auto fluent_atoms = view.get<1>();
-        return loki::hash_combine(fluent_atoms.hash());
+        const auto problem = view.get<3>();
+        return loki::hash_combine(fluent_atoms.hash(), problem);
     }
 };
 
 struct FlatDenseStateEqual
 {
     bool operator()(const FlatDenseState& view_left, const FlatDenseState& view_right) const
     {
         const auto fluent_atoms_left = view_left.get<1>();
         const auto fluent_atoms_right = view_right.get<1>();
-        return (fluent_atoms_left == fluent_atoms_right);
+        const auto problem_left = view_left.get<3>();
+        const auto problem_right = view_right.get<3>();
+        return (fluent_atoms_left == fluent_atoms_right) && (problem_left == problem_right);
     }
 };
 
 using FlatDenseStateSet = flatmemory::UnorderedSet<FlatDenseStateLayout, FlatDenseStateHash, FlatDenseStateEqual>;
 using FlatDenseStateVector = flatmemory::FixedSizedTypeVector<FlatDenseStateLayout>;
 
 /**
@@ -89,29 +91,31 @@
 
 public:
     template<PredicateCategory P>
     [[nodiscard]] FlatBitsetBuilder<P>& get_atoms()
     {
         if constexpr (std::is_same_v<P, Static>)
         {
-            static_assert(dependent_false<P>::value, "Static ground atoms must be accessed from the corresponding problem.");
+            static_assert(dependent_false<P>::value, "Modifying static grounded atoms is not allowed.");
         }
         else if constexpr (std::is_same_v<P, Fluent>)
         {
             return m_builder.get<1>();
         }
         else if constexpr (std::is_same_v<P, Derived>)
         {
             return m_builder.get<2>();
         }
         else
         {
             static_assert(dependent_false<P>::value, "Missing implementation for PredicateCategory.");
         }
     }
+
+    [[nodiscard]] Problem& get_problem() { return m_builder.get<3>(); }
 };
 
 /**
  * Implementation class
  *
  * Reads the memory layout generated by the lifted state builder.
  */
@@ -140,96 +144,90 @@
     [[nodiscard]] size_t hash_impl() const { return loki::hash_combine(m_view.buffer()); }
 
     /* Implement IStateView interface */
     friend class IStateView<ConstView<StateDispatcher<DenseStateTag>>>;
 
     [[nodiscard]] uint32_t get_id_impl() const { return m_view.get<0>(); }
 
-    [[nodiscard]] auto begin_fluent_ground_atoms_impl() const { return m_view.get<1>().begin(); }
-    [[nodiscard]] auto end_fluent_ground_atoms_impl() const { return m_view.get<1>().end(); }
-    [[nodiscard]] auto begin_derived_ground_atoms_impl() const { return m_view.get<2>().begin(); }
-    [[nodiscard]] auto end_derived_ground_atoms_impl() const { return m_view.get<2>().end(); }
-
-    /**
-     * Fluent and Derived
-     */
-    template<PredicateCategory P>
-    [[nodiscard]] bool contains(const Problem problem, const GroundAtom<P>& ground_atom) const
-    {
-        return get_atoms<P>(problem).get(ground_atom->get_identifier());
-    }
-
-    template<PredicateCategory P>
-    [[nodiscard]] bool literal_holds_impl(const Problem problem, const GroundLiteral<P>& literal) const
-    {
-        return literal->is_negated() != contains(problem, literal->get_atom());
-    }
-
-    template<PredicateCategory P>
-    [[nodiscard]] bool literals_hold_impl(const Problem problem, const GroundLiteralList<P>& literals) const
-    {
-        for (const auto& literal : literals)
-        {
-            if (!literal_holds_impl(problem, literal))
-            {
-                return false;
-            }
-        }
-
-        return true;
-    }
+    [[nodiscard]] auto begin_impl() const { return get_atoms<Fluent>().begin(); }
+    [[nodiscard]] auto end_impl() const { return get_atoms<Fluent>().end(); }
 
 public:
     explicit ConstView(FlatDenseState view) : m_view(view) {}
 
     template<PredicateCategory P>
-    [[nodiscard]] FlatBitset<P> get_atoms(const Problem problem) const
+    [[nodiscard]] FlatBitset<P> get_atoms() const
     {
         if constexpr (std::is_same_v<P, Static>)
         {
-            return problem->get_static_initial_positive_atoms_bitset();
+            return get_problem()->get_static_initial_positive_atoms_bitset();
         }
         else if constexpr (std::is_same_v<P, Fluent>)
         {
             return m_view.get<1>();
         }
         else if constexpr (std::is_same_v<P, Derived>)
         {
             return m_view.get<2>();
         }
         else
         {
             static_assert(dependent_false<P>::value, "Missing implementation for PredicateCategory.");
         }
     }
+
+    [[nodiscard]] Problem get_problem() const { return m_view.get<3>(); }
+
+    template<PredicateCategory P>
+    bool contains(const GroundAtom<P>& ground_atom) const
+    {
+        return get_atoms<P>().get(ground_atom->get_identifier());
+    }
+
+    template<PredicateCategory P>
+    bool literal_holds(const GroundLiteral<P>& literal) const
+    {
+        return literal->is_negated() != contains(literal->get_atom());
+    }
+
+    template<PredicateCategory P>
+    bool literals_hold(const GroundLiteralList<P>& literals) const
+    {
+        for (const auto& literal : literals)
+        {
+            if (!literal_holds(literal))
+            {
+                return false;
+            }
+        }
+
+        return true;
+    }
 };
 
 /**
  * Mimir types
  */
 
 // TODO: differentiate registered and unregistered state can help us remove some duplicate code.
 // We could use unregistered states internally to represent some unfinished state.
 
 using DenseStateBuilder = Builder<StateDispatcher<DenseStateTag>>;
 using DenseState = ConstView<StateDispatcher<DenseStateTag>>;
 using DenseStateList = std::vector<DenseState>;
 
-
 struct DenseStateHash
 {
     size_t operator()(const DenseState& view) const { return view.hash(); }
 };
 
-template<typename T>
-using DenseStateMap = std::unordered_map<DenseState, T, DenseStateHash>;
 using DenseStateSet = std::unordered_set<DenseState, DenseStateHash>;
 
 /**
  * Pretty printing
  */
 
-extern std::ostream& operator<<(std::ostream& os, const std::tuple<const Problem, const DenseState, const PDDLFactories&>& data);
+extern std::ostream& operator<<(std::ostream& os, const std::tuple<DenseState, const PDDLFactories&>& data);
 
 }
 
 #endif
```

### Comparing `pymimir-0.9.12/include/mimir/search/states/interface.hpp` & `pymimir-0.9.9/include/mimir/search/states/interface.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -64,34 +64,16 @@
 
     [[nodiscard]] uint32_t get_id() const { return self().get_id_impl(); }
 
     /**
      * Iterators
      */
 
-    [[nodiscard]] auto begin_fluent_ground_atoms() const { return self().begin_fluent_ground_atoms_impl(); }
-    [[nodiscard]] auto end_fluent_ground_atoms() const { return self().end_fluent_ground_atoms_impl(); }
-    [[nodiscard]] auto begin_derived_ground_atoms() const { return self().begin_derived_ground_atoms_impl(); }
-    [[nodiscard]] auto end_derived_ground_atoms() const { return self().end_derived_ground_atoms_impl(); }
-
-    /**
-     * Extended
-     */
-
-    template<PredicateCategory P>
-    [[nodiscard]] bool literal_holds(const Problem problem, const GroundLiteral<P>& literal) const
-    {
-        return self().literal_holds_impl(problem, literal);
-    }
-
-    template<PredicateCategory P>
-    [[nodiscard]] bool literals_hold(const Problem problem, const GroundLiteralList<P>& literals) const
-    {
-        return self().literals_hold_impl(problem, literals);
-    }
+    [[nodiscard]] auto begin() const { return self().begin_impl(); }
+    [[nodiscard]] auto end() const { return self().end_impl(); }
 };
 
 /**
  * General implementation class.
  *
  * Specialize the wrapped tag to provide your own implementation of a state representation.
  */
```

### Comparing `pymimir-0.9.12/include/mimir/search/states/tags.hpp` & `pymimir-0.9.9/include/mimir/search/states/tags.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/states.hpp` & `pymimir-0.9.9/include/mimir/search/states.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 
 #if defined(STATE_REPR_DENSE)
 
 #include "mimir/search/states/dense.hpp"
 
 namespace mimir
 {
-template<typename T>
-using StateMap = DenseStateMap<T>;
 using StateBuilder = DenseStateBuilder;
 using State = DenseState;
 using StateList = DenseStateList;
 using StateSet = DenseStateSet;
 }
 
 #else
```

### Comparing `pymimir-0.9.12/include/mimir/search/successor_state_generators/dense.hpp` & `pymimir-0.9.9/include/mimir/search/successor_state_generators/dense.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -68,119 +68,129 @@
     {
         /* Fetch member references for non extended construction. */
 
         auto& flatmemory_builder = m_state_builder.get_flatmemory_builder();
         auto& state_id = m_state_builder.get_id();
         auto& fluent_state_atoms = m_state_builder.get_atoms<Fluent>();
         fluent_state_atoms.unset_all();
+        auto& problem = m_state_builder.get_problem();
 
         /* 1. Set state id */
 
         int next_state_id = m_states.size();
         state_id = next_state_id;
 
-        /* 2. Construct non-extended state */
+        /* 2. Set problem */
+
+        problem = m_aag->get_problem();
+
+        /* 3. Construct non-extended state */
 
         for (const auto& atom : atoms)
         {
             fluent_state_atoms.set(atom->get_identifier());
         }
 
-        /* 3. Retrieve cached extended state */
+        /* 4. Retrieve cached extended state */
 
         // Test whether there exists an extended state for the given non extended state
         flatmemory_builder.finish();
         auto iter = m_states.find(FlatDenseState(flatmemory_builder.buffer().data()));
         if (iter != m_states.end())
         {
             return DenseState(*iter);
         }
 
         /* Fetch member references for extended construction. */
 
         auto& derived_state_atoms = m_state_builder.get_atoms<Derived>();
         derived_state_atoms.unset_all();
 
-        /* 4. Construct extended state by evaluating Axioms */
+        /* 5. Construct extended state by evaluating Axioms */
 
         m_aag->generate_and_apply_axioms(fluent_state_atoms, derived_state_atoms);
 
-        /* 5. Cache extended state */
+        /* 6. Cache extended state */
 
         flatmemory_builder.finish();
         auto [iter2, inserted] = m_states.insert(flatmemory_builder);
 
-        /* 6. Return newly generated extended state */
+        /* 7. Return newly generated extended state */
 
         return DenseState(*iter2);
     }
 
     [[nodiscard]] DenseState get_or_create_successor_state_impl(const DenseState state, const DenseGroundAction action)
     {
         /* Fetch member references for non extended construction. */
 
         auto& flatmemory_builder = m_state_builder.get_flatmemory_builder();
         auto& state_id = m_state_builder.get_id();
         auto& fluent_state_atoms = m_state_builder.get_atoms<Fluent>();
         fluent_state_atoms.unset_all();
+        auto& problem = m_state_builder.get_problem();
 
         // 1. Initialize non-extended state
-        fluent_state_atoms = state.get_atoms<Fluent>(m_aag->get_problem());
+        fluent_state_atoms = state.get_atoms<Fluent>();
 
         /* 2. Set state id */
 
         int next_state_id = m_states.size();
         state_id = next_state_id;
 
-        /* 3. Construct non-extended state */
+        /* 3. Set problem */
+
+        problem = m_aag->get_problem();
+
+        /* 4. Construct non-extended state */
 
         /* STRIPS effects*/
         auto strips_part_proxy = DenseStripsActionEffect(action.get_strips_effect());
         fluent_state_atoms -= strips_part_proxy.get_negative_effects();
         fluent_state_atoms |= strips_part_proxy.get_positive_effects();
         /* Conditional effects */
         for (const auto flat_conditional_effect : action.get_conditional_effects())
         {
             auto cond_effect_proxy = DenseConditionalEffect(flat_conditional_effect);
 
-            if (cond_effect_proxy.is_applicable(m_aag->get_problem(), state))
+            if (cond_effect_proxy.is_applicable(state))
             {
                 const auto& simple_effect = cond_effect_proxy.get_simple_effect();
 
                 if (simple_effect.is_negated)
                 {
                     fluent_state_atoms.unset(simple_effect.atom_id);
                 }
                 else
                 {
                     fluent_state_atoms.set(simple_effect.atom_id);
                 }
             }
         }
 
-        /* 4. Retrieve cached extended state */
+        /* 5. Retrieve cached extended state */
 
         // Test whether there exists an extended state for the given non extended state
         flatmemory_builder.finish();
         auto iter = m_states.find(FlatDenseState(flatmemory_builder.buffer().data()));
         if (iter != m_states.end())
         {
             return DenseState(*iter);
         }
 
         /* Fetch member references for extended construction. */
 
         auto& derived_state_atoms = m_state_builder.get_atoms<Derived>();
         derived_state_atoms.unset_all();
 
-        /* 5. Construct extended state by evaluating Axioms */
+        /* 6. Construct extended state by evaluating Axioms */
 
         m_aag->generate_and_apply_axioms(fluent_state_atoms, derived_state_atoms);
 
-        /* 6. Cache extended state */
+        /* 7. Cache extended state */
 
         flatmemory_builder.finish();
         auto [iter2, inserted] = m_states.insert(flatmemory_builder);
 
         /* 7. Return newly generated extended state */
 
         return DenseState(*iter2);
```

### Comparing `pymimir-0.9.12/include/mimir/search/successor_state_generators/interface.hpp` & `pymimir-0.9.9/include/mimir/search/successor_state_generators/interface.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/successor_state_generators.hpp` & `pymimir-0.9.9/include/mimir/search/successor_state_generators.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/translations.hpp` & `pymimir-0.9.9/include/mimir/search/translations.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/view.hpp` & `pymimir-0.9.9/include/mimir/search/view.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/include/mimir/search/view_const.hpp` & `pymimir-0.9.9/include/mimir/search/view_const.hpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/pyproject.toml` & `pymimir-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/python/src/pymimir/__init__.py` & `pymimir-0.9.9/python/src/pymimir/__init__.py`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/python/src/pymimir/bindings.cpp` & `pymimir-0.9.9/python/src/pymimir/bindings.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#include "mimir/datasets/state_space.hpp"
-#include <pybind11/detail/common.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>  // Necessary for automatic conversion of e.g. std::vectors
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
 #include "mimir/mimir.hpp"
@@ -183,36 +181,27 @@
         .def("get_name", &PredicateImpl<Derived>::get_name, py::return_value_policy::reference)
         .def("get_parameters", &PredicateImpl<Derived>::get_parameters, py::return_value_policy::reference);
 
     py::class_<AtomImpl<Static>>(m, "StaticAtom")  //
         .def("__str__", py::overload_cast<>(&loki::Base<AtomImpl<Static>>::str, py::const_))
         .def("get_identifier", &AtomImpl<Static>::get_identifier)
         .def("get_predicate", &AtomImpl<Static>::get_predicate, py::return_value_policy::reference)
-        .def(
-            "get_terms",
-            [](const AtomImpl<Static>& atom) { return to_term_variant_list(atom.get_terms()); },
-            py::return_value_policy::reference);
+        .def("get_terms", [](const AtomImpl<Static>& atom) { return to_term_variant_list(atom.get_terms()); });
 
     py::class_<AtomImpl<Fluent>>(m, "FluentAtom")  //
         .def("__str__", py::overload_cast<>(&loki::Base<AtomImpl<Fluent>>::str, py::const_))
         .def("get_identifier", &AtomImpl<Fluent>::get_identifier)
         .def("get_predicate", &AtomImpl<Fluent>::get_predicate, py::return_value_policy::reference)
-        .def(
-            "get_terms",
-            [](const AtomImpl<Fluent>& atom) { return to_term_variant_list(atom.get_terms()); },
-            py::return_value_policy::reference);
+        .def("get_terms", [](const AtomImpl<Fluent>& atom) { return to_term_variant_list(atom.get_terms()); });
 
     py::class_<AtomImpl<Derived>>(m, "DerivedAtom")  //
         .def("__str__", py::overload_cast<>(&loki::Base<AtomImpl<Derived>>::str, py::const_))
         .def("get_identifier", &AtomImpl<Derived>::get_identifier)
         .def("get_predicate", &AtomImpl<Derived>::get_predicate, py::return_value_policy::reference)
-        .def(
-            "get_terms",
-            [](const AtomImpl<Derived>& atom) { return to_term_variant_list(atom.get_terms()); },
-            py::return_value_policy::reference);
+        .def("get_terms", [](const AtomImpl<Derived>& atom) { return to_term_variant_list(atom.get_terms()); });
 
     py::class_<FunctionSkeletonImpl>(m, "FunctionSkeleton")  //
         .def("__str__", py::overload_cast<>(&loki::Base<FunctionSkeletonImpl>::str, py::const_))
         .def("get_identifier", &FunctionSkeletonImpl::get_identifier)
         .def("get_name", &FunctionSkeletonImpl::get_name, py::return_value_policy::reference)
         .def("get_parameters", &FunctionSkeletonImpl::get_parameters, py::return_value_policy::reference);
 
@@ -301,18 +290,15 @@
         .def("get_identifier", &EffectConditionalImpl::get_identifier)
         .def("get_static_conditions", &EffectConditionalImpl::get_static_conditions, py::return_value_policy::reference)
         .def("get_fluent_conditions", &EffectConditionalImpl::get_fluent_conditions, py::return_value_policy::reference)
         .def("get_derived_conditions", &EffectConditionalImpl::get_derived_conditions, py::return_value_policy::reference)
         .def("get_effect", &EffectConditionalImpl::get_effect, py::return_value_policy::reference);
 
     py::class_<FunctionExpressionVariant>(m, "FunctionExpression")  //
-        .def(
-            "get",
-            [](const FunctionExpressionVariant& arg) -> py::object { return std::visit(CastVisitor(), *arg.function_expression); },
-            py::return_value_policy::reference);
+        .def("get", [](const FunctionExpressionVariant& arg) -> py::object { return std::visit(CastVisitor(), *arg.function_expression); });
     ;
 
     py::class_<EffectUniversalImpl>(m, "UniversalEffect")  //
         .def("__str__", py::overload_cast<>(&loki::Base<EffectUniversalImpl>::str, py::const_))
         .def("get_identifier", &EffectUniversalImpl::get_identifier)
         .def("get_parameters", &EffectUniversalImpl::get_parameters, py::return_value_policy::reference)
         .def("get_static_conditions", &EffectUniversalImpl::get_static_conditions, py::return_value_policy::reference)
@@ -325,98 +311,81 @@
         .def("get_identifier", &FunctionExpressionNumberImpl::get_identifier)
         .def("get_number", &FunctionExpressionNumberImpl::get_number);
 
     py::class_<FunctionExpressionBinaryOperatorImpl>(m, "FunctionExpressionBinaryOperator")  //
         .def("__str__", py::overload_cast<>(&loki::Base<FunctionExpressionBinaryOperatorImpl>::str, py::const_))
         .def("get_identifier", &FunctionExpressionBinaryOperatorImpl::get_identifier)
         .def("get_binary_operator", &FunctionExpressionBinaryOperatorImpl::get_binary_operator)
-        .def(
-            "get_left_function_expression",
-            [](const FunctionExpressionBinaryOperatorImpl& function_expression)
-            { return FunctionExpressionVariant(function_expression.get_left_function_expression()); },
-            py::return_value_policy::reference)
-        .def(
-            "get_right_function_expression",
-            [](const FunctionExpressionBinaryOperatorImpl& function_expression)
-            { return FunctionExpressionVariant(function_expression.get_right_function_expression()); },
-            py::return_value_policy::reference);
+        .def("get_left_function_expression",
+             [](const FunctionExpressionBinaryOperatorImpl& function_expression)
+             { return FunctionExpressionVariant(function_expression.get_left_function_expression()); })
+        .def("get_right_function_expression",
+             [](const FunctionExpressionBinaryOperatorImpl& function_expression)
+             { return FunctionExpressionVariant(function_expression.get_right_function_expression()); });
 
     py::class_<FunctionExpressionMultiOperatorImpl>(m, "FunctionExpressionMultiOperator")  //
         .def("__str__", py::overload_cast<>(&loki::Base<FunctionExpressionMultiOperatorImpl>::str, py::const_))
         .def("get_identifier", &FunctionExpressionMultiOperatorImpl::get_identifier)
         .def("get_multi_operator", &FunctionExpressionMultiOperatorImpl::get_multi_operator)
-        .def(
-            "get_function_expressions",
-            [](const FunctionExpressionMultiOperatorImpl& function_expression)
-            { return to_function_expression_variant_list(function_expression.get_function_expressions()); },
-            py::return_value_policy::reference);
+        .def("get_function_expressions",
+             [](const FunctionExpressionMultiOperatorImpl& function_expression)
+             { return to_function_expression_variant_list(function_expression.get_function_expressions()); });
 
     py::class_<FunctionExpressionMinusImpl>(m, "FunctionExpressionMinus")  //
         .def("__str__", py::overload_cast<>(&loki::Base<FunctionExpressionMinusImpl>::str, py::const_))
         .def("get_identifier", &FunctionExpressionMinusImpl::get_identifier)
         .def("get_function_expression",
              [](const FunctionExpressionMinusImpl& function_expression) { return FunctionExpressionVariant(function_expression.get_function_expression()); });
     ;
 
     py::class_<FunctionExpressionFunctionImpl>(m, "FunctionExpressionFunction")  //
         .def("__str__", py::overload_cast<>(&loki::Base<FunctionExpressionFunctionImpl>::str, py::const_))
         .def("get_identifier", &FunctionExpressionFunctionImpl::get_identifier)
-        .def("get_function", &FunctionExpressionFunctionImpl::get_function, py::return_value_policy::reference);
+        .def("get_function", &FunctionExpressionFunctionImpl::get_function);
 
     py::class_<GroundFunctionExpressionVariant>(m, "GroundFunctionExpression")  //
-        .def(
-            "get",
-            [](const GroundFunctionExpressionVariant& arg) -> py::object { return std::visit(CastVisitor(), *arg.function_expression); },
-            py::return_value_policy::reference);
+        .def("get", [](const GroundFunctionExpressionVariant& arg) -> py::object { return std::visit(CastVisitor(), *arg.function_expression); });
     ;
 
     py::class_<GroundFunctionExpressionNumberImpl>(m, "GroundFunctionExpressionNumber")  //
         .def("__str__", py::overload_cast<>(&loki::Base<GroundFunctionExpressionNumberImpl>::str, py::const_))
         .def("get_identifier", &GroundFunctionExpressionNumberImpl::get_identifier)
         .def("get_number", &GroundFunctionExpressionNumberImpl::get_number);
 
     py::class_<GroundFunctionExpressionBinaryOperatorImpl>(m, "GroundFunctionExpressionBinaryOperator")  //
         .def("__str__", py::overload_cast<>(&loki::Base<GroundFunctionExpressionBinaryOperatorImpl>::str, py::const_))
         .def("get_identifier", &GroundFunctionExpressionBinaryOperatorImpl::get_identifier)
         .def("get_binary_operator", &GroundFunctionExpressionBinaryOperatorImpl::get_binary_operator)
-        .def(
-            "get_left_function_expression",
-            [](const GroundFunctionExpressionBinaryOperatorImpl& function_expression)
-            { return GroundFunctionExpressionVariant(function_expression.get_left_function_expression()); },
-            py::return_value_policy::reference)
-        .def(
-            "get_right_function_expression",
-            [](const GroundFunctionExpressionBinaryOperatorImpl& function_expression)
-            { return GroundFunctionExpressionVariant(function_expression.get_right_function_expression()); },
-            py::return_value_policy::reference);
+        .def("get_left_function_expression",
+             [](const GroundFunctionExpressionBinaryOperatorImpl& function_expression)
+             { return GroundFunctionExpressionVariant(function_expression.get_left_function_expression()); })
+        .def("get_right_function_expression",
+             [](const GroundFunctionExpressionBinaryOperatorImpl& function_expression)
+             { return GroundFunctionExpressionVariant(function_expression.get_right_function_expression()); });
 
     py::class_<GroundFunctionExpressionMultiOperatorImpl>(m, "GroundFunctionExpressionMultiOperator")  //
         .def("__str__", py::overload_cast<>(&loki::Base<GroundFunctionExpressionMultiOperatorImpl>::str, py::const_))
         .def("get_identifier", &GroundFunctionExpressionMultiOperatorImpl::get_identifier)
         .def("get_multi_operator", &GroundFunctionExpressionMultiOperatorImpl::get_multi_operator)
-        .def(
-            "get_function_expressions",
-            [](const GroundFunctionExpressionMultiOperatorImpl& function_expression)
-            { return to_ground_function_expression_variant_list(function_expression.get_function_expressions()); },
-            py::return_value_policy::reference);
+        .def("get_function_expressions",
+             [](const GroundFunctionExpressionMultiOperatorImpl& function_expression)
+             { return to_ground_function_expression_variant_list(function_expression.get_function_expressions()); });
 
     py::class_<GroundFunctionExpressionMinusImpl>(m, "GroundFunctionExpressionMinus")  //
         .def("__str__", py::overload_cast<>(&loki::Base<GroundFunctionExpressionMinusImpl>::str, py::const_))
         .def("get_identifier", &GroundFunctionExpressionMinusImpl::get_identifier)
-        .def(
-            "get_function_expression",
-            [](const GroundFunctionExpressionMinusImpl& function_expression)
-            { return GroundFunctionExpressionVariant(function_expression.get_function_expression()); },
-            py::return_value_policy::reference);
+        .def("get_function_expression",
+             [](const GroundFunctionExpressionMinusImpl& function_expression)
+             { return GroundFunctionExpressionVariant(function_expression.get_function_expression()); });
     ;
 
     py::class_<GroundFunctionExpressionFunctionImpl>(m, "GroundFunctionExpressionFunction")  //
         .def("__str__", py::overload_cast<>(&loki::Base<GroundFunctionExpressionFunctionImpl>::str, py::const_))
         .def("get_identifier", &GroundFunctionExpressionFunctionImpl::get_identifier)
-        .def("get_function", &GroundFunctionExpressionFunctionImpl::get_function, py::return_value_policy::reference);
+        .def("get_function", &GroundFunctionExpressionFunctionImpl::get_function);
 
     py::class_<OptimizationMetricImpl>(m, "OptimizationMetric")  //
         .def("__str__", py::overload_cast<>(&loki::Base<OptimizationMetricImpl>::str, py::const_))
         .def("get_identifier", &OptimizationMetricImpl::get_identifier)
         .def("get_function_expression", [](const OptimizationMetricImpl& metric) { return GroundFunctionExpressionVariant(metric.get_function_expression()); })
         .def("get_optimization_metric", &OptimizationMetricImpl::get_optimization_metric, py::return_value_policy::reference);
 
@@ -464,31 +433,15 @@
         .def("get_fluent_initial_literals", &ProblemImpl::get_fluent_initial_literals, py::return_value_policy::reference)
         .def("get_numeric_fluents", &ProblemImpl::get_numeric_fluents, py::return_value_policy::reference)
         .def("get_optimization_metric", &ProblemImpl::get_optimization_metric, py::return_value_policy::reference)
         .def("get_static_goal_condition", &ProblemImpl::get_static_goal_condition, py::return_value_policy::reference)
         .def("get_fluent_goal_condition", &ProblemImpl::get_fluent_goal_condition, py::return_value_policy::reference)
         .def("get_derived_goal_condition", &ProblemImpl::get_derived_goal_condition, py::return_value_policy::reference);
 
-    py::class_<PDDLFactories>(m, "PDDLFactories")  //
-        .def("get_static_ground_atom", &PDDLFactories::get_ground_atom<Static>, py::return_value_policy::reference)
-        .def("get_fluent_ground_atom", &PDDLFactories::get_ground_atom<Fluent>, py::return_value_policy::reference)
-        .def("get_derived_ground_atom", &PDDLFactories::get_ground_atom<Derived>, py::return_value_policy::reference)
-        .def("get_static_ground_atoms_from_ids",
-             py::overload_cast<const std::vector<size_t>&>(&PDDLFactories::get_ground_atoms_from_ids<Static, std::vector<size_t>>, py::const_),
-             py::return_value_policy::reference)
-        .def("get_fluent_ground_atoms_from_ids",
-             py::overload_cast<const std::vector<size_t>&>(&PDDLFactories::get_ground_atoms_from_ids<Fluent, std::vector<size_t>>, py::const_),
-             py::return_value_policy::reference)
-        .def("get_derived_ground_atoms_from_ids",
-             py::overload_cast<const std::vector<size_t>&>(&PDDLFactories::get_ground_atoms_from_ids<Derived, std::vector<size_t>>, py::const_),
-             py::return_value_policy::reference)
-        .def("get_object", &PDDLFactories::get_object, py::return_value_policy::reference)
-        .def("get_objects_from_ids",
-             py::overload_cast<const std::vector<size_t>&>(&PDDLFactories::get_objects_from_ids<std::vector<size_t>>, py::const_),
-             py::return_value_policy::reference);
+    py::class_<PDDLFactories>(m, "PDDLFactories");
 
     py::class_<PDDLParser>(m, "PDDLParser")  //
         .def(py::init<std::string, std::string>())
         .def("get_domain", &PDDLParser::get_domain, py::return_value_policy::reference)
         .def("get_problem", &PDDLParser::get_problem, py::return_value_policy::reference)
         .def("get_factories", &PDDLParser::get_factories, py::return_value_policy::reference);
 
@@ -512,73 +465,45 @@
         .value("SOLVED", SearchStatus::SOLVED)
         .export_values();
 
     /* State */
     py::class_<State>(m, "State")  //
         .def("__hash__", &State::hash)
         .def("__eq__", &State::operator==)
-        .def("get_static_atoms",
-             [](const State& self, const Problem& problem)
-             {
-                 auto atoms = self.get_atoms<Static>(problem);
-                 return std::vector<size_t>(atoms.begin(), atoms.end());
-             })
-        .def("get_fluent_atoms",
-             [](const State& self, const Problem& problem)
-             {
-                 auto atoms = self.get_atoms<Fluent>(problem);
-                 return std::vector<size_t>(atoms.begin(), atoms.end());
-             })
-        .def("get_derived_atoms",
-             [](const State& self, const Problem& problem)
-             {
-                 auto atoms = self.get_atoms<Derived>(problem);
-                 return std::vector<size_t>(atoms.begin(), atoms.end());
-             })
-        .def("literal_holds", py::overload_cast<const Problem, const GroundLiteral<Static>&>(&State::literal_holds<Static>, py::const_))
-        .def("literal_holds", py::overload_cast<const Problem, const GroundLiteral<Fluent>&>(&State::literal_holds<Fluent>, py::const_))
-        .def("literal_holds", py::overload_cast<const Problem, const GroundLiteral<Derived>&>(&State::literal_holds<Derived>, py::const_))
-        .def("literals_hold", py::overload_cast<const Problem, const GroundLiteralList<Static>&>(&State::literals_hold<Static>, py::const_))
-        .def("literals_hold", py::overload_cast<const Problem, const GroundLiteralList<Fluent>&>(&State::literals_hold<Fluent>, py::const_))
-        .def("literals_hold", py::overload_cast<const Problem, const GroundLiteralList<Derived>&>(&State::literals_hold<Derived>, py::const_))
+        .def(
+            "__iter__",
+            [](State& state) { return py::make_iterator(state.begin(), state.end()); },
+            py::keep_alive<0, 1>())
         .def("to_string",
-             [](const State& self, const Problem& problem, const PDDLFactories& pddl_factories)
+             [](State self, PDDLFactories& pddl_factories)
              {
                  std::stringstream ss;
-                 ss << std::make_tuple(problem, self, std::cref(pddl_factories));
+                 ss << std::make_tuple(self, std::cref(pddl_factories));
                  return ss.str();
              })
         .def("get_id", &State::get_id);
 
     /* Action */
     py::class_<GroundAction>(m, "GroundAction")  //
         .def("__hash__", &GroundAction::hash)
         .def("__eq__", &GroundAction::operator==)
         .def("to_string",
-             [](const GroundAction& self, PDDLFactories& pddl_factories)
+             [](GroundAction self, PDDLFactories& pddl_factories)
              {
                  std::stringstream ss;
                  ss << std::make_tuple(self, std::cref(pddl_factories));
                  return ss.str();
              })
         .def("get_id", &GroundAction::get_id);
 
     /* AAGs */
 
     py::class_<IDynamicAAG, std::shared_ptr<IDynamicAAG>>(m, "IAAG")  //
-        .def(
-            "compute_applicable_actions",
-            [](IDynamicAAG& self, const State& state)
-            {
-                auto applicable_actions = GroundActionList {};
-                self.generate_applicable_actions(state, applicable_actions);
-                return applicable_actions;
-            },
-            py::return_value_policy::reference)
-        .def("get_action", &IDynamicAAG::get_action, py::return_value_policy::reference)
+        .def("generate_applicable_actions", &IDynamicAAG::generate_applicable_actions)
+        .def("get_action", &IDynamicAAG::get_action)
         .def("get_problem", &IDynamicAAG::get_problem, py::return_value_policy::reference)
         .def("get_pddl_factories", py::overload_cast<>(&IDynamicAAG::get_pddl_factories), py::return_value_policy::reference);
 
     // Lifted
     py::class_<ILiftedAAGEventHandler, std::shared_ptr<ILiftedAAGEventHandler>>(m, "ILiftedAAGEventHandler");  //
     py::class_<DefaultLiftedAAGEventHandler, ILiftedAAGEventHandler, std::shared_ptr<DefaultLiftedAAGEventHandler>>(m,
                                                                                                                     "DefaultLiftedAAGEventHandler")  //
@@ -668,13 +593,9 @@
         .def("get_problem", &StateSpaceImpl::get_problem, py::return_value_policy::reference)
         .def("get_goal_distances", &StateSpaceImpl::get_goal_distances, py::return_value_policy::reference)
         .def("get_goal_states", &StateSpaceImpl::get_goal_states, py::return_value_policy::reference)
         .def("get_deadend_states", &StateSpaceImpl::get_deadend_states, py::return_value_policy::reference)
         .def("get_num_states", &StateSpaceImpl::get_num_states)
         .def("get_num_transitions", &StateSpaceImpl::get_num_transitions)
         .def("get_num_goal_states", &StateSpaceImpl::get_num_goal_states)
-        .def("get_num_deadend_states", &StateSpaceImpl::get_num_deadend_states)
-        .def("get_goal_distance", &StateSpaceImpl::get_goal_distance)
-        .def("get_max_goal_distance", &StateSpaceImpl::get_max_goal_distance)
-        .def("is_deadend_state", &StateSpaceImpl::is_deadend_state)
-        .def("sample_state_with_goal_distance", &StateSpaceImpl::sample_state_with_goal_distance, py::return_value_policy::reference);
-}
+        .def("get_num_deadend_states", &StateSpaceImpl::get_num_deadend_states);
+}
```

### Comparing `pymimir-0.9.12/python/src/pymimir.egg-info/SOURCES.txt` & `pymimir-0.9.9/python/src/pymimir.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 include/mimir/formalism/translators/simplify_goal.hpp
 include/mimir/formalism/translators/split_disjunctive_conditions.hpp
 include/mimir/formalism/translators/to_disjunctive_normal_form.hpp
 include/mimir/formalism/translators/to_effect_normal_form.hpp
 include/mimir/formalism/translators/to_mimir_structures.hpp
 include/mimir/formalism/translators/to_negation_normal_form.hpp
 include/mimir/formalism/translators/utils.hpp
+include/mimir/isomorphism/exact.hpp
+include/mimir/isomorphism/wl.hpp
 include/mimir/search/actions.hpp
 include/mimir/search/algorithms.hpp
 include/mimir/search/applicable_action_generators.hpp
 include/mimir/search/axiom_evaluators.hpp
 include/mimir/search/axioms.hpp
 include/mimir/search/builder.hpp
 include/mimir/search/condition_grounders.hpp
```

### Comparing `pymimir-0.9.12/python/tests/datasets/test_state_space.py` & `pymimir-0.9.9/python/tests/datasets/test_state_space.py`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/python/tests/search/test_brfs.py` & `pymimir-0.9.9/python/tests/search/test_brfs.py`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/setup.py` & `pymimir-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.9.12"
+__version__ = "0.9.9"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pymimir-0.9.12/src/CMakeLists.txt` & `pymimir-0.9.9/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/common/kpkc.cpp` & `pymimir-0.9.9/src/common/kpkc.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/common/murmurhash3.cpp` & `pymimir-0.9.9/src/common/murmurhash3.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/datasets/state_space.cpp` & `pymimir-0.9.9/src/datasets/state_space.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,14 @@
  * along with this program. If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include "mimir/datasets/state_space.hpp"
 
 #include "mimir/common/timers.hpp"
 
-#include <algorithm>
-#include <cstdlib>
 #include <deque>
 
 namespace mimir
 {
 
 static std::vector<int>
 compute_shortest_distances_from_states_impl(const size_t num_total_states, const StateList& states, const std::vector<Transitions>& transitions)
@@ -94,41 +92,29 @@
     m_states(std::move(states)),
     m_initial_state(std::move(initial_state)),
     m_num_transitions(num_transitions),
     m_forward_transitions(std::move(forward_transitions)),
     m_backward_transitions(std::move(backward_transitions)),
     m_goal_distances(std::move(goal_distances)),
     m_goal_states(std::move(goal_states)),
-    m_deadend_states(std::move(deadend_states)),
-    m_state_indices(),
-    m_states_by_goal_distance()
+    m_deadend_states(std::move(deadend_states))
 {
-    for (size_t index = 0; index < m_states.size(); ++index)
-    {
-        auto state = m_states.at(index);
-        m_state_indices.emplace(state, index);
-
-        auto distance = m_goal_distances.at(index);
-        auto& states_with_distance = m_states_by_goal_distance[distance];
-        states_with_distance.emplace_back(state);
-    }
 }
 
 std::shared_ptr<StateSpaceImpl>
 StateSpaceImpl::create(const fs::path& domain_file_path, const fs::path& problem_file_path, const size_t max_num_states, const size_t timeout_ms)
 {
     auto stop_watch = StopWatch(timeout_ms);
 
     auto pddl_parser = PDDLParser(domain_file_path, problem_file_path);
-    const auto problem = pddl_parser.get_problem();
-    auto aag = std::make_shared<GroundedAAG>(problem, pddl_parser.get_factories());
+    auto aag = std::make_shared<GroundedAAG>(pddl_parser.get_problem(), pddl_parser.get_factories());
     auto ssg = std::make_shared<SuccessorStateGenerator>(aag);
 
     auto initial_state = ssg->get_or_create_initial_state();
-    if (!initial_state.literals_hold(problem, problem->get_static_initial_literals()))
+    if (!initial_state.literals_hold(aag->get_problem()->get_static_initial_literals()))
     {
         // Unsolvable
         return nullptr;
     }
 
     auto lifo_queue = std::deque<State>();
     lifo_queue.push_back(initial_state);
@@ -143,15 +129,15 @@
     stop_watch.start();
     while (!lifo_queue.empty() && !stop_watch.has_finished())
     {
         const auto state = lifo_queue.back();
 
         lifo_queue.pop_back();
 
-        if (state.literals_hold(problem, problem->get_fluent_goal_condition()) && state.literals_hold(problem, problem->get_derived_goal_condition()))
+        if (state.literals_hold(aag->get_problem()->get_fluent_goal_condition()) && state.literals_hold(aag->get_problem()->get_derived_goal_condition()))
         {
             goal_states.insert(state);
         }
 
         aag->generate_applicable_actions(state, applicable_actions);
 
         for (const auto& action : applicable_actions)
@@ -263,33 +249,19 @@
 
 const std::vector<Transitions>& StateSpaceImpl::get_forward_transitions() const { return m_forward_transitions; }
 
 const std::vector<Transitions>& StateSpaceImpl::get_backward_transitions() const { return m_backward_transitions; }
 
 const std::vector<int>& StateSpaceImpl::get_goal_distances() const { return m_goal_distances; }
 
-int StateSpaceImpl::get_goal_distance(const State& state) const { return m_goal_distances.at(m_state_indices.at(state)); }
-
-int StateSpaceImpl::get_max_goal_distance() const { return *std::max_element(m_goal_distances.begin(), m_goal_distances.end()); }
-
 const StateSet& StateSpaceImpl::get_goal_states() const { return m_goal_states; }
 
 const StateSet& StateSpaceImpl::get_deadend_states() const { return m_deadend_states; }
 
 size_t StateSpaceImpl::get_num_states() const { return m_states.size(); }
 
 size_t StateSpaceImpl::get_num_transitions() const { return m_num_transitions; }
 
 size_t StateSpaceImpl::get_num_goal_states() const { return m_goal_states.size(); }
 
 size_t StateSpaceImpl::get_num_deadend_states() const { return m_deadend_states.size(); }
-
-bool StateSpaceImpl::is_deadend_state(const State& state) const { return m_goal_distances.at(m_state_indices.at(state)) < 0; }
-
-State StateSpaceImpl::sample_state_with_goal_distance(int goal_distance) const
-{
-    const auto& states = m_states_by_goal_distance.at(goal_distance);
-    const auto index = std::rand() % static_cast<int>(states.size());
-    return states[index];
-}
-
-}
+}
```

### Comparing `pymimir-0.9.12/src/formalism/action.cpp` & `pymimir-0.9.9/src/formalism/action.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/axiom.cpp` & `pymimir-0.9.9/src/formalism/axiom.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/domain.cpp` & `pymimir-0.9.9/src/formalism/domain.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/effects.cpp` & `pymimir-0.9.9/src/formalism/effects.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/function.cpp` & `pymimir-0.9.9/src/formalism/function.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/function_expressions.cpp` & `pymimir-0.9.9/src/formalism/function_expressions.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/function_skeleton.cpp` & `pymimir-0.9.9/src/formalism/function_skeleton.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/ground_function.cpp` & `pymimir-0.9.9/src/formalism/ground_function.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/ground_function_expressions.cpp` & `pymimir-0.9.9/src/formalism/ground_function_expressions.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/metric.cpp` & `pymimir-0.9.9/src/formalism/metric.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/numeric_fluent.cpp` & `pymimir-0.9.9/src/formalism/numeric_fluent.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/object.cpp` & `pymimir-0.9.9/src/formalism/object.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/parser.cpp` & `pymimir-0.9.9/src/formalism/parser.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/problem.cpp` & `pymimir-0.9.9/src/formalism/problem.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/requirements.cpp` & `pymimir-0.9.9/src/formalism/requirements.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/term.cpp` & `pymimir-0.9.9/src/formalism/term.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/transformers/delete_relax.cpp` & `pymimir-0.9.9/src/formalism/transformers/delete_relax.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/transformers/encode_parameter_index_in_variables.cpp` & `pymimir-0.9.9/src/formalism/transformers/encode_parameter_index_in_variables.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/move_existential_quantifiers.cpp` & `pymimir-0.9.9/src/formalism/translators/move_existential_quantifiers.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/remove_types.cpp` & `pymimir-0.9.9/src/formalism/translators/remove_types.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/remove_universal_quantifiers.cpp` & `pymimir-0.9.9/src/formalism/translators/remove_universal_quantifiers.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/rename_quantified_variables.cpp` & `pymimir-0.9.9/src/formalism/translators/rename_quantified_variables.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/simplify_goal.cpp` & `pymimir-0.9.9/src/formalism/translators/simplify_goal.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/split_disjunctive_conditions.cpp` & `pymimir-0.9.9/src/formalism/translators/split_disjunctive_conditions.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/to_disjunctive_normal_form.cpp` & `pymimir-0.9.9/src/formalism/translators/to_disjunctive_normal_form.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/to_effect_normal_form.cpp` & `pymimir-0.9.9/src/formalism/translators/to_effect_normal_form.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/to_mimir_structures.cpp` & `pymimir-0.9.9/src/formalism/translators/to_mimir_structures.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/to_negation_normal_form.cpp` & `pymimir-0.9.9/src/formalism/translators/to_negation_normal_form.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/translators/utils.cpp` & `pymimir-0.9.9/src/formalism/translators/utils.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/formalism/variable.cpp` & `pymimir-0.9.9/src/formalism/variable.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/actions/dense.cpp` & `pymimir-0.9.9/src/search/actions/dense.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/algorithms/event_handlers/debug.cpp` & `pymimir-0.9.9/src/search/algorithms/event_handlers/debug.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -18,41 +18,38 @@
 #include "mimir/search/algorithms/event_handlers/debug.hpp"
 
 #include "mimir/common/printers.hpp"
 #include "mimir/search/plan.hpp"
 
 namespace mimir
 {
-void DebugAlgorithmEventHandler::on_generate_state_impl(const Problem problem,
-                                                        const GroundAction action,
-                                                        const State successor_state,
-                                                        const PDDLFactories& pddl_factories) const
+void DebugAlgorithmEventHandler::on_generate_state_impl(GroundAction action, State successor_state, const PDDLFactories& pddl_factories) const
 {
     std::cout << "[Algorithm] Action: " << std::make_tuple(action, std::cref(pddl_factories)) << "\n"
-              << "[Algorithm] Successor: " << std::make_tuple(problem, successor_state, std::cref(pddl_factories)) << "\n"
+              << "[Algorithm] Successor: " << std::make_tuple(successor_state, std::cref(pddl_factories)) << "\n"
               << std::endl;
 }
 
 void DebugAlgorithmEventHandler::on_finish_f_layer_impl(uint64_t f_value, uint64_t num_expanded_states, uint64_t num_generated_states) const
 {
     std::cout << "[Algorithm] Finished state expansion until f-layer " << f_value << " with num expanded states " << num_expanded_states
               << " and num generated states " << num_generated_states << std::endl;
 }
 
-void DebugAlgorithmEventHandler::on_expand_state_impl(const Problem problem, const State state, const PDDLFactories& pddl_factories) const
+void DebugAlgorithmEventHandler::on_expand_state_impl(State state, const PDDLFactories& pddl_factories) const
 {
     std::cout << "[Algorithm] ----------------------------------------\n"
-              << "[Algorithm] State: " << std::make_tuple(problem, state, std::cref(pddl_factories)) << std::endl
+              << "[Algorithm] State: " << std::make_tuple(state, std::cref(pddl_factories)) << std::endl
               << std::endl;
 }
 
-void DebugAlgorithmEventHandler::on_start_search_impl(const Problem problem, const State initial_state, const PDDLFactories& pddl_factories) const
+void DebugAlgorithmEventHandler::on_start_search_impl(State initial_state, const PDDLFactories& pddl_factories) const
 {
     std::cout << "[Algorithm] Search started.\n"
-              << "[Algorithm] Initial: " << std::make_tuple(problem, initial_state, std::cref(pddl_factories)) << std::endl;
+              << "[Algorithm] Initial: " << std::make_tuple(initial_state, std::cref(pddl_factories)) << std::endl;
 }
 
 void DebugAlgorithmEventHandler::on_end_search_impl() const { std::cout << "[Algorithm] Search ended.\n" << m_statistics << std::endl; }
 
 void DebugAlgorithmEventHandler::on_solved_impl(const GroundActionList& ground_action_plan) const
 {
     auto plan = to_plan(ground_action_plan);
```

### Comparing `pymimir-0.9.12/src/search/algorithms/event_handlers/default.cpp` & `pymimir-0.9.9/src/search/algorithms/event_handlers/default.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,25 @@
 #include "mimir/search/algorithms/event_handlers/default.hpp"
 
 #include "mimir/common/printers.hpp"
 #include "mimir/search/plan.hpp"
 
 namespace mimir
 {
-void DefaultAlgorithmEventHandler::on_generate_state_impl(const Problem problem,
-                                                          const GroundAction action,
-                                                          const State successor_state,
-                                                          const PDDLFactories& pddl_factories) const
-{
-}
+void DefaultAlgorithmEventHandler::on_generate_state_impl(GroundAction action, State successor_state, const PDDLFactories& pddl_factories) const {}
 
 void DefaultAlgorithmEventHandler::on_finish_f_layer_impl(uint64_t f_value, uint64_t num_expanded_states, uint64_t num_generated_states) const
 {
     std::cout << "[Algorithm] Finished state expansion until f-layer " << f_value << " with num expanded states " << num_expanded_states
               << " and num generated states " << num_generated_states << std::endl;
 }
 
-void DefaultAlgorithmEventHandler::on_expand_state_impl(const Problem problem, const State state, const PDDLFactories& pddl_factories) const {}
+void DefaultAlgorithmEventHandler::on_expand_state_impl(State state, const PDDLFactories& pddl_factories) const {}
 
-void DefaultAlgorithmEventHandler::on_start_search_impl(const Problem problem, const State initial_state, const PDDLFactories& pddl_factories) const
+void DefaultAlgorithmEventHandler::on_start_search_impl(State initial_state, const PDDLFactories& pddl_factories) const
 {  //
     std::cout << "[Algorithm] Search started." << std::endl;
 }
 
 void DefaultAlgorithmEventHandler::on_end_search_impl() const { std::cout << "[Algorithm] Search ended.\n" << m_statistics << std::endl; }
 
 void DefaultAlgorithmEventHandler::on_solved_impl(const GroundActionList& ground_action_plan) const
```

### Comparing `pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded/event_handlers/debug.cpp` & `pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded/event_handlers/debug.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded/event_handlers/default.cpp` & `pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded/event_handlers/default.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/applicable_action_generators/dense_grounded.cpp` & `pymimir-0.9.9/src/search/applicable_action_generators/dense_grounded.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,17 @@
     const auto delete_free_problem = delete_relax_transformer.run(*m_problem);
     auto delete_free_lifted_aag = std::make_shared<LiftedDenseAAG>(delete_free_problem, m_pddl_factories);
     auto delete_free_ssg = DenseSSG(delete_free_lifted_aag);
 
     auto state_builder = StateBuilder();
     auto& fluent_state_atoms = state_builder.get_atoms<Fluent>();
     auto& derived_state_atoms = state_builder.get_atoms<Derived>();
-    fluent_state_atoms = delete_free_ssg.get_or_create_initial_state().get_atoms<Fluent>(m_problem);
+    auto& state_problem = state_builder.get_problem();
+    fluent_state_atoms = delete_free_ssg.get_or_create_initial_state().get_atoms<Fluent>();
+    state_problem = delete_free_problem;
 
     // Keep track of changes
     bool reached_delete_free_explore_fixpoint = true;
 
     auto actions = DenseGroundActionList {};
     do
     {
@@ -114,15 +116,15 @@
 
         // Create and all applicable actions and apply them
         // Attention: we cannot just apply newly generated actions because conditional effects might trigger later.
         delete_free_lifted_aag->generate_applicable_actions(state, actions);
         for (const auto& action : actions)
         {
             const auto succ_state = delete_free_ssg.get_or_create_successor_state(state, action);
-            for (const auto atom_id : succ_state.get_atoms<Fluent>(m_problem))
+            for (const auto atom_id : succ_state.get_atoms<Fluent>())
             {
                 fluent_state_atoms.set(atom_id);
             }
         }
 
         // Create and all applicable axioms and apply them
         delete_free_lifted_aag->generate_and_apply_axioms(fluent_state_atoms, derived_state_atoms);
@@ -191,15 +193,15 @@
     m_event_handler->on_finish_build_axiom_match_tree(m_axiom_match_tree);
 }
 
 void AAG<GroundedAAGDispatcher<DenseStateTag>>::generate_applicable_actions_impl(DenseState state, DenseGroundActionList& out_applicable_actions)
 {
     out_applicable_actions.clear();
 
-    m_action_match_tree.get_applicable_elements(state.get_atoms<Fluent>(m_problem), state.get_atoms<Derived>(m_problem), out_applicable_actions);
+    m_action_match_tree.get_applicable_elements(state.get_atoms<Fluent>(), state.get_atoms<Derived>(), out_applicable_actions);
 }
 
 void AAG<GroundedAAGDispatcher<DenseStateTag>>::generate_and_apply_axioms_impl(const FlatBitsetBuilder<Fluent>& fluent_state_atoms,
                                                                                FlatBitsetBuilder<Derived>& ref_derived_state_atoms)
 {
     for (const auto& lifted_partition : m_lifted_aag.get_axiom_partitioning())
     {
```

### Comparing `pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/consistency_graph.cpp` & `pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/consistency_graph.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/event_handlers/debug.cpp` & `pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/event_handlers/debug.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted/event_handlers/default.cpp` & `pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted/event_handlers/default.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/applicable_action_generators/dense_lifted.cpp` & `pymimir-0.9.9/src/search/applicable_action_generators/dense_lifted.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -322,19 +322,19 @@
     out_applicable_actions.clear();
 
     m_event_handler->on_start_generating_applicable_actions();
 
     // Create the assignment sets that are shared by all action schemas.
 
     auto& fluent_predicates = m_problem->get_domain()->get_fluent_predicates();
-    auto fluent_atoms = m_ref_pddl_factories.get_ground_atoms_from_ids<Fluent>(state.get_atoms<Fluent>(m_problem));
+    auto fluent_atoms = m_ref_pddl_factories.get_ground_atoms_from_ids<Fluent>(state.get_atoms<Fluent>());
     auto fluent_assignment_set = AssignmentSet<Fluent>(m_problem, fluent_predicates, fluent_atoms);
 
     auto& derived_predicates = m_problem->get_problem_and_domain_derived_predicates();
-    auto derived_atoms = m_ref_pddl_factories.get_ground_atoms_from_ids<Derived>(state.get_atoms<Derived>(m_problem));
+    auto derived_atoms = m_ref_pddl_factories.get_ground_atoms_from_ids<Derived>(state.get_atoms<Derived>());
     auto derived_assignment_set = AssignmentSet<Derived>(m_problem, derived_predicates, derived_atoms);
 
     // Get all applicable ground actions.
     // This is done by getting bindings in the given state using the precondition.
     // These bindings are then used to ground the actual action schemas.
 
     std::vector<ObjectList> bindings;
```

### Comparing `pymimir-0.9.12/src/search/axiom_evaluators/axiom_stratification.cpp` & `pymimir-0.9.9/src/search/axiom_evaluators/axiom_stratification.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/axiom_evaluators/dense.cpp` & `pymimir-0.9.9/src/search/axiom_evaluators/dense.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             reached_partition_fixed_point = true;
 
             /* Compute applicable axioms */
 
             applicable_axioms.clear();
             for (const auto& axiom : relevant_axioms)
             {
-                auto partially_extended_state = PartiallyExtendedState(fluent_state_atoms, ref_derived_state_atoms);
+                auto partially_extended_state = PartiallyExtendedState(m_problem, fluent_state_atoms, ref_derived_state_atoms);
                 auto& condition_grounder = m_condition_grounders.at(axiom);
                 condition_grounder.compute_bindings(partially_extended_state, fluent_assignment_set, derived_assignment_set, bindings);
 
                 for (auto& binding : bindings)
                 {
                     applicable_axioms.emplace_back(ground_axiom(axiom, std::move(binding)));
                 }
```

### Comparing `pymimir-0.9.12/src/search/axioms/dense.cpp` & `pymimir-0.9.9/src/search/axioms/dense.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/plan.cpp` & `pymimir-0.9.9/src/search/plan.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/src/search/states/dense.cpp` & `pymimir-0.9.9/src/search/states/dense.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 #include <flatmemory/flatmemory.hpp>
 #include <ostream>
 #include <tuple>
 
 namespace mimir
 {
 
-std::ostream& operator<<(std::ostream& os, const std::tuple<const Problem, const DenseState, const PDDLFactories&>& data)
+std::ostream& operator<<(std::ostream& os, const std::tuple<DenseState, const PDDLFactories&>& data)
 {
-    const auto [problem, state, pddl_factories] = data;
+    const auto [state, pddl_factories] = data;
 
     auto out_fluent_ground_atoms = GroundAtomList<Fluent> {};
-    auto out_static_ground_atoms = GroundAtomList<Static> {};
     auto out_derived_ground_atoms = GroundAtomList<Derived> {};
+    auto out_static_ground_atoms = GroundAtomList<Static> {};
 
-    pddl_factories.get_ground_atoms_from_ids(state.get_atoms<Fluent>(problem), out_fluent_ground_atoms);
-    pddl_factories.get_ground_atoms_from_ids(state.get_atoms<Static>(problem), out_static_ground_atoms);
-    pddl_factories.get_ground_atoms_from_ids(state.get_atoms<Derived>(problem), out_derived_ground_atoms);
+    pddl_factories.get_ground_atoms_from_ids(state.get_atoms<Fluent>(), out_fluent_ground_atoms);
+    pddl_factories.get_ground_atoms_from_ids(state.get_atoms<Derived>(), out_derived_ground_atoms);
+    pddl_factories.get_ground_atoms_from_ids(state.get_atoms<Static>(), out_static_ground_atoms);
 
     os << "State("
        << "state id=" << state.get_id() << ", "
        << "fluent atoms=" << out_fluent_ground_atoms << ", "
-       << "static atoms=" << out_static_ground_atoms << ", "
-       << "derived atoms=" << out_derived_ground_atoms << ")";
+       << "derived atoms=" << out_derived_ground_atoms << ", "
+       << "static atoms=" << out_static_ground_atoms << ")";
 
     return os;
 }
 
 }
```

### Comparing `pymimir-0.9.12/tests/integration/CMakeLists.txt` & `pymimir-0.9.9/tests/integration/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/integration/dependencies/boost/CMakeLists.txt` & `pymimir-0.9.9/tests/integration/dependencies/boost/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/integration/dependencies/flatmemory/CMakeLists.txt` & `pymimir-0.9.9/tests/integration/dependencies/flatmemory/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/integration/dependencies/loki/CMakeLists.txt` & `pymimir-0.9.9/tests/integration/dependencies/loki/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/integration/dependencies/mimir/CMakeLists.txt` & `pymimir-0.9.9/tests/integration/dependencies/mimir/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/integration/main.cpp` & `pymimir-0.9.9/tests/integration/main.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/CMakeLists.txt` & `pymimir-0.9.9/tests/unit/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/algorithms/memory_pool.cpp` & `pymimir-0.9.9/tests/unit/algorithms/memory_pool.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/datasets/state_space.cpp` & `pymimir-0.9.9/tests/unit/datasets/state_space.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/formalism/translators/remove_types.cpp` & `pymimir-0.9.9/tests/unit/formalism/translators/remove_types.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/formalism/translators/remove_universal_quantifiers.cpp` & `pymimir-0.9.9/tests/unit/formalism/translators/remove_universal_quantifiers.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/formalism/translators/to_disjunctive_normal_form.cpp` & `pymimir-0.9.9/tests/unit/formalism/translators/to_disjunctive_normal_form.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/formalism/translators/to_negation_normal_form.cpp` & `pymimir-0.9.9/tests/unit/formalism/translators/to_negation_normal_form.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/algorithms/astar.cpp` & `pymimir-0.9.9/tests/unit/search/algorithms/astar.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/algorithms/brfs.cpp` & `pymimir-0.9.9/tests/unit/search/algorithms/brfs.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/applicable_action_generators/dense-grounded.cpp` & `pymimir-0.9.9/tests/unit/search/applicable_action_generators/dense-grounded.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/applicable_action_generators/dense-lifted.cpp` & `pymimir-0.9.9/tests/unit/search/applicable_action_generators/dense-lifted.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/planners/single.cpp` & `pymimir-0.9.9/tests/unit/search/planners/single.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/search_nodes/cost.cpp` & `pymimir-0.9.9/tests/unit/search/search_nodes/cost.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/states/bitset/bitset.cpp` & `pymimir-0.9.9/tests/unit/search/states/bitset/bitset.cpp`

 * *Files identical despite different names*

### Comparing `pymimir-0.9.12/tests/unit/search/successor_state_generators/dense.cpp` & `pymimir-0.9.9/tests/unit/search/successor_state_generators/dense.cpp`

 * *Files identical despite different names*

