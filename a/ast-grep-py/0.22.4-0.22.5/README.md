# Comparing `tmp/ast_grep_py-0.22.4.tar.gz` & `tmp/ast_grep_py-0.22.5.tar.gz`

## Comparing `ast_grep_py-0.22.4.tar` & `ast_grep_py-0.22.5.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0     1001      127      692 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/Cargo.toml
--rw-r--r--   0     1001      127     2331 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/language.rs
--rw-r--r--   0     1001      127     3904 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/lib.rs
--rw-r--r--   0     1001      127    15102 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/match_tree.rs
--rw-r--r--   0     1001      127     3610 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/matcher/kind.rs
--rw-r--r--   0     1001      127     3689 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/matcher/node_match.rs
--rw-r--r--   0     1001      127    15793 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/matcher/pattern.rs
--rw-r--r--   0     1001      127      982 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/matcher/text.rs
--rw-r--r--   0     1001      127     5317 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/matcher.rs
--rw-r--r--   0     1001      127    10527 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/meta_var.rs
--rw-r--r--   0     1001      127    18135 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/node.rs
--rw-r--r--   0     1001      127    15251 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/ops.rs
--rw-r--r--   0     1001      127     4789 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/pinned.rs
--rw-r--r--   0     1001      127    10854 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/replacer/indent.rs
--rw-r--r--   0     1001      127     6157 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/replacer/structural.rs
--rw-r--r--   0     1001      127    10186 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/replacer/template.rs
--rw-r--r--   0     1001      127     2855 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/replacer.rs
--rw-r--r--   0     1001      127     8489 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/source.rs
--rw-r--r--   0     1001      127    16602 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/core/src/traversal.rs
--rw-r--r--   0     1001      127     2472 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/Cargo.toml
--rw-r--r--   0     1001      127     1047 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/bash.rs
--rw-r--r--   0     1001      127     1023 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/cpp.rs
--rw-r--r--   0     1001      127      860 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/csharp.rs
--rw-r--r--   0     1001      127      815 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/css.rs
--rw-r--r--   0     1001      127     2412 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/elixir.rs
--rw-r--r--   0     1001      127     1192 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/go.rs
--rw-r--r--   0     1001      127     1450 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/haskell.rs
--rw-r--r--   0     1001      127     1142 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/html.rs
--rw-r--r--   0     1001      127     1013 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/json.rs
--rw-r--r--   0     1001      127     1216 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/kotlin.rs
--rw-r--r--   0     1001      127    13779 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/lib.rs
--rw-r--r--   0     1001      127      924 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/lua.rs
--rw-r--r--   0     1001      127     3523 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/parsers.rs
--rw-r--r--   0     1001      127      372 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/php.rs
--rw-r--r--   0     1001      127     2494 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/python.rs
--rw-r--r--   0     1001      127      846 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/ruby.rs
--rw-r--r--   0     1001      127     2147 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/rust.rs
--rw-r--r--   0     1001      127     1646 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/scala.rs
--rw-r--r--   0     1001      127     1362 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/language/src/swift.rs
--rw-r--r--   0     1001      127      682 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/Cargo.toml
--rw-r--r--   0     1001      127     8951 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/check_var.rs
--rw-r--r--   0     1001      127     7022 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/combined.rs
--rw-r--r--   0     1001      127     8734 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/fixer.rs
--rw-r--r--   0     1001      127     5244 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/lib.rs
--rw-r--r--   0     1001      127     3677 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/maybe.rs
--rw-r--r--   0     1001      127     8987 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule/deserialize_env.rs
--rw-r--r--   0     1001      127    18489 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule/mod.rs
--rw-r--r--   0     1001      127     8432 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule/referent_rule.rs
--rw-r--r--   0     1001      127    19521 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule/relational_rule.rs
--rw-r--r--   0     1001      127     5481 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule/stop_by.rs
--rw-r--r--   0     1001      127     6342 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule_collection.rs
--rw-r--r--   0     1001      127    17934 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule_config.rs
--rw-r--r--   0     1001      127    13828 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/rule_core.rs
--rw-r--r--   0     1001      127     3341 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/transform/mod.rs
--rw-r--r--   0     1001      127    11131 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/transform/rewrite.rs
--rw-r--r--   0     1001      127     7418 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/transform/string_case.rs
--rw-r--r--   0     1001      127    11870 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/config/src/transform/transformation.rs
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.22.4/crates/pyo3/Cargo.toml
--rw-r--r--   0     1001      127     1459 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/README.md
--rw-r--r--   0     1001      127     1356 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     2131 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1090 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/src/lib.rs
--rw-r--r--   0     1001      127     8897 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/src/py_node.rs
--rw-r--r--   0     1001      127     2358 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/src/range.rs
--rw-r--r--   0     1001      127      864 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/tests/test_fix.py
--rw-r--r--   0     1001      127     1213 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/tests/test_range.py
--rw-r--r--   0     1001      127     3641 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/tests/test_rule.py
--rw-r--r--   0     1001      127     3463 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/tests/test_simple.py
--rw-r--r--   0     1001      127     3221 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/tests/test_traversal.py
--rw-r--r--   0     1001      127     1214 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/crates/pyo3/tests/test_wrong_usage.py
--rw-r--r--   0     1001      127    61831 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/Cargo.lock
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 ast_grep_py-0.22.4/Cargo.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.22.4/pyproject.toml
--rw-r--r--   0     1001      127     1356 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     2131 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127     1459 2024-05-27 04:53:27.000000 ast_grep_py-0.22.4/README.md
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.22.4/PKG-INFO
+-rw-r--r--   0     1001      127     2472 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/Cargo.toml
+-rw-r--r--   0     1001      127     1047 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/bash.rs
+-rw-r--r--   0     1001      127     1023 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/cpp.rs
+-rw-r--r--   0     1001      127      860 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/csharp.rs
+-rw-r--r--   0     1001      127      815 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/css.rs
+-rw-r--r--   0     1001      127     2412 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/elixir.rs
+-rw-r--r--   0     1001      127     1192 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/go.rs
+-rw-r--r--   0     1001      127     1450 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/haskell.rs
+-rw-r--r--   0     1001      127     1142 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/html.rs
+-rw-r--r--   0     1001      127     1013 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/json.rs
+-rw-r--r--   0     1001      127     1216 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/kotlin.rs
+-rw-r--r--   0     1001      127    13779 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/lib.rs
+-rw-r--r--   0     1001      127      924 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/lua.rs
+-rw-r--r--   0     1001      127     3523 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/parsers.rs
+-rw-r--r--   0     1001      127      372 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/php.rs
+-rw-r--r--   0     1001      127     2494 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/python.rs
+-rw-r--r--   0     1001      127      846 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/ruby.rs
+-rw-r--r--   0     1001      127     2147 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/rust.rs
+-rw-r--r--   0     1001      127     1646 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/scala.rs
+-rw-r--r--   0     1001      127     1362 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/language/src/swift.rs
+-rw-r--r--   0     1001      127      682 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/Cargo.toml
+-rw-r--r--   0     1001      127     8951 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/check_var.rs
+-rw-r--r--   0     1001      127     7022 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/combined.rs
+-rw-r--r--   0     1001      127     8734 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/fixer.rs
+-rw-r--r--   0     1001      127     5244 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/lib.rs
+-rw-r--r--   0     1001      127     3677 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/maybe.rs
+-rw-r--r--   0     1001      127     8987 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule/deserialize_env.rs
+-rw-r--r--   0     1001      127    18489 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule/mod.rs
+-rw-r--r--   0     1001      127     8432 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule/referent_rule.rs
+-rw-r--r--   0     1001      127    19521 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule/relational_rule.rs
+-rw-r--r--   0     1001      127     5481 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule/stop_by.rs
+-rw-r--r--   0     1001      127     6342 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule_collection.rs
+-rw-r--r--   0     1001      127    17934 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule_config.rs
+-rw-r--r--   0     1001      127    13828 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/rule_core.rs
+-rw-r--r--   0     1001      127     3341 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/transform/mod.rs
+-rw-r--r--   0     1001      127    11131 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/transform/rewrite.rs
+-rw-r--r--   0     1001      127     7418 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/transform/string_case.rs
+-rw-r--r--   0     1001      127    11870 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/config/src/transform/transformation.rs
+-rw-r--r--   0     1001      127      692 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/Cargo.toml
+-rw-r--r--   0     1001      127     2331 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/language.rs
+-rw-r--r--   0     1001      127     3904 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/lib.rs
+-rw-r--r--   0     1001      127    15102 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/match_tree.rs
+-rw-r--r--   0     1001      127     3610 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/matcher/kind.rs
+-rw-r--r--   0     1001      127     3689 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      127    15793 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      127      982 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/matcher/text.rs
+-rw-r--r--   0     1001      127     5317 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/matcher.rs
+-rw-r--r--   0     1001      127    10527 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/meta_var.rs
+-rw-r--r--   0     1001      127    18135 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/node.rs
+-rw-r--r--   0     1001      127    15251 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/ops.rs
+-rw-r--r--   0     1001      127     4789 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/pinned.rs
+-rw-r--r--   0     1001      127    10854 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/replacer/indent.rs
+-rw-r--r--   0     1001      127     6157 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/replacer/structural.rs
+-rw-r--r--   0     1001      127    10186 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/replacer/template.rs
+-rw-r--r--   0     1001      127     2855 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/replacer.rs
+-rw-r--r--   0     1001      127     8489 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/source.rs
+-rw-r--r--   0     1001      127    16602 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/core/src/traversal.rs
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.22.5/crates/pyo3/Cargo.toml
+-rw-r--r--   0     1001      127     1459 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/README.md
+-rw-r--r--   0     1001      127     1356 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     2131 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1254 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     9747 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/src/py_node.rs
+-rw-r--r--   0     1001      127     2488 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/src/range.rs
+-rw-r--r--   0     1001      127     1617 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/src/unicode_position.rs
+-rw-r--r--   0     1001      127     1274 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/tests/test_fix.py
+-rw-r--r--   0     1001      127     1142 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/tests/test_range.py
+-rw-r--r--   0     1001      127     3641 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/tests/test_rule.py
+-rw-r--r--   0     1001      127     3463 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/tests/test_simple.py
+-rw-r--r--   0     1001      127     3221 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/tests/test_traversal.py
+-rw-r--r--   0     1001      127     1214 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/crates/pyo3/tests/test_wrong_usage.py
+-rw-r--r--   0     1001      127    61853 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/Cargo.lock
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 ast_grep_py-0.22.5/Cargo.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.22.5/pyproject.toml
+-rw-r--r--   0     1001      127     1356 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127        0 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     2131 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127     1459 2024-06-02 22:06:30.000000 ast_grep_py-0.22.5/README.md
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.22.5/PKG-INFO
```

### Comparing `ast_grep_py-0.22.4/crates/core/Cargo.toml` & `ast_grep_py-0.22.5/crates/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/language.rs` & `ast_grep_py-0.22.5/crates/core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/lib.rs` & `ast_grep_py-0.22.5/crates/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/match_tree.rs` & `ast_grep_py-0.22.5/crates/core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/matcher/kind.rs` & `ast_grep_py-0.22.5/crates/core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/matcher/node_match.rs` & `ast_grep_py-0.22.5/crates/core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/matcher/pattern.rs` & `ast_grep_py-0.22.5/crates/core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/matcher/text.rs` & `ast_grep_py-0.22.5/crates/core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/matcher.rs` & `ast_grep_py-0.22.5/crates/core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/meta_var.rs` & `ast_grep_py-0.22.5/crates/core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/node.rs` & `ast_grep_py-0.22.5/crates/core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/ops.rs` & `ast_grep_py-0.22.5/crates/core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/pinned.rs` & `ast_grep_py-0.22.5/crates/core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/replacer/indent.rs` & `ast_grep_py-0.22.5/crates/core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/replacer/structural.rs` & `ast_grep_py-0.22.5/crates/core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/replacer/template.rs` & `ast_grep_py-0.22.5/crates/core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/replacer.rs` & `ast_grep_py-0.22.5/crates/core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/source.rs` & `ast_grep_py-0.22.5/crates/core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/core/src/traversal.rs` & `ast_grep_py-0.22.5/crates/core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/Cargo.toml` & `ast_grep_py-0.22.5/crates/language/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/bash.rs` & `ast_grep_py-0.22.5/crates/language/src/bash.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/cpp.rs` & `ast_grep_py-0.22.5/crates/language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/csharp.rs` & `ast_grep_py-0.22.5/crates/language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/css.rs` & `ast_grep_py-0.22.5/crates/language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/elixir.rs` & `ast_grep_py-0.22.5/crates/language/src/elixir.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/go.rs` & `ast_grep_py-0.22.5/crates/language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/haskell.rs` & `ast_grep_py-0.22.5/crates/language/src/haskell.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/html.rs` & `ast_grep_py-0.22.5/crates/language/src/html.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/json.rs` & `ast_grep_py-0.22.5/crates/language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/kotlin.rs` & `ast_grep_py-0.22.5/crates/language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/lib.rs` & `ast_grep_py-0.22.5/crates/language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/lua.rs` & `ast_grep_py-0.22.5/crates/language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/parsers.rs` & `ast_grep_py-0.22.5/crates/language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/python.rs` & `ast_grep_py-0.22.5/crates/language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/ruby.rs` & `ast_grep_py-0.22.5/crates/language/src/ruby.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/rust.rs` & `ast_grep_py-0.22.5/crates/language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/scala.rs` & `ast_grep_py-0.22.5/crates/language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/language/src/swift.rs` & `ast_grep_py-0.22.5/crates/language/src/swift.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/Cargo.toml` & `ast_grep_py-0.22.5/crates/config/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/check_var.rs` & `ast_grep_py-0.22.5/crates/config/src/check_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/combined.rs` & `ast_grep_py-0.22.5/crates/config/src/combined.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/fixer.rs` & `ast_grep_py-0.22.5/crates/config/src/fixer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/lib.rs` & `ast_grep_py-0.22.5/crates/config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/maybe.rs` & `ast_grep_py-0.22.5/crates/config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule/deserialize_env.rs` & `ast_grep_py-0.22.5/crates/config/src/rule/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule/mod.rs` & `ast_grep_py-0.22.5/crates/config/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule/referent_rule.rs` & `ast_grep_py-0.22.5/crates/config/src/rule/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule/relational_rule.rs` & `ast_grep_py-0.22.5/crates/config/src/rule/relational_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule/stop_by.rs` & `ast_grep_py-0.22.5/crates/config/src/rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule_collection.rs` & `ast_grep_py-0.22.5/crates/config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule_config.rs` & `ast_grep_py-0.22.5/crates/config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/rule_core.rs` & `ast_grep_py-0.22.5/crates/config/src/rule_core.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/transform/mod.rs` & `ast_grep_py-0.22.5/crates/config/src/transform/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/transform/rewrite.rs` & `ast_grep_py-0.22.5/crates/config/src/transform/rewrite.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/transform/string_case.rs` & `ast_grep_py-0.22.5/crates/config/src/transform/string_case.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/config/src/transform/transformation.rs` & `ast_grep_py-0.22.5/crates/config/src/transform/transformation.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/Cargo.toml` & `ast_grep_py-0.22.5/crates/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/README.md` & `ast_grep_py-0.22.5/crates/pyo3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/ast_grep_py/__init__.py` & `ast_grep_py-0.22.5/crates/pyo3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.5/crates/pyo3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/src/py_node.rs` & `ast_grep_py-0.22.5/crates/pyo3/src/py_node.rs`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 // because it is refcnt and concurrency safe
 unsafe impl Send for SgNode {}
 
 #[pymethods]
 impl SgNode {
   /*----------  Node Inspection ----------*/
   fn range(&self) -> Range {
-    Range::from(&self.inner)
+    Python::with_gil(|py| {
+      let root = self.root.bind(py);
+      let root = root.borrow();
+      Range::from(&self.inner, &root.position)
+    })
   }
 
   fn is_leaf(&self) -> bool {
     self.inner.is_leaf()
   }
 
   fn is_named(&self) -> bool {
@@ -235,28 +239,49 @@
       })
       .collect()
   }
 
   /*---------- Edit  ----------*/
   fn replace(&self, text: &str) -> Edit {
     let byte_range = self.inner.range();
-    Edit {
-      position: byte_range.start,
-      deleted_length: byte_range.len(),
-      inserted_text: text.to_string(),
-    }
+    Python::with_gil(|py| {
+      let root = self.root.bind(py);
+      let root = root.borrow();
+      let position = root.position.byte_to_char(byte_range.start);
+      let end = root.position.byte_to_char(byte_range.end);
+      Edit {
+        position,
+        deleted_length: end - position,
+        inserted_text: text.to_string(),
+      }
+    })
   }
 
   fn commit_edits(&self, mut edits: Vec<Edit>) -> String {
     edits.sort_by_key(|edit| edit.position);
     let mut new_content = String::new();
     let old_content = self.text();
+    let converted: Vec<_> = Python::with_gil(move |py| {
+      let root = self.root.bind(py);
+      let root = root.borrow();
+      let conv = &root.position;
+      edits
+        .into_iter()
+        .map(|mut e| {
+          let char_offset = e.position + e.deleted_length;
+          let byte_offset = conv.char_to_byte(char_offset);
+          e.position = conv.char_to_byte(e.position);
+          e.deleted_length = byte_offset - e.position;
+          e
+        })
+        .collect()
+    });
     let offset = self.inner.range().start;
     let mut start = 0;
-    for diff in edits {
+    for diff in converted {
       let pos = diff.position - offset;
       // skip overlapping edits
       if start > pos {
         continue;
       }
       new_content.push_str(&old_content[start..pos]);
       new_content.push_str(&diff.inserted_text);
@@ -345,14 +370,14 @@
   let matcher = config.get_matcher(env).context("cannot get matcher")?;
   Ok(matcher)
 }
 
 #[pyclass(frozen, get_all)]
 #[derive(Clone, PartialEq, Eq, Hash)]
 pub struct Edit {
-  /// The position of the edit
+  /// The char position of the edit
   pub position: usize,
-  /// The length of the text to be deleted
+  /// The char length of the text to be deleted
   pub deleted_length: usize,
   /// The text to be inserted
   pub inserted_text: String,
 }
```

### Comparing `ast_grep_py-0.22.4/crates/pyo3/src/range.rs` & `ast_grep_py-0.22.5/crates/pyo3/src/range.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+use crate::unicode_position::UnicodePosition;
 use ast_grep_core::{Doc, Node};
 use pyo3::prelude::*;
 use std::collections::hash_map::DefaultHasher;
 use std::fmt::{self, Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 
 #[pyclass(frozen, get_all)]
 #[derive(Clone, PartialEq, Eq, Hash)]
 pub struct Pos {
   /// line number starting from 0
   line: usize,
   /// column number starting from 0
   column: usize,
-  // TODO: this should be char offset
-  /// byte offset of the position
+  /// char offset of the position
   index: usize,
 }
 
 impl Display for Pos {
   fn fmt(&self, f: &mut Formatter<'_>) -> Result<(), fmt::Error> {
     write!(f, "({},{})", self.line, self.column)
   }
@@ -94,17 +94,19 @@
   }
   fn __str__(&self) -> String {
     self.to_string()
   }
 }
 
 impl Range {
-  pub fn from<D: Doc>(node: &Node<D>) -> Self {
+  pub fn from<D: Doc>(node: &Node<D>, positioner: &UnicodePosition) -> Self {
     let byte_range = node.range();
     let start_pos = node.start_pos();
     let end_pos = node.end_pos();
+    let start = positioner.byte_to_char(byte_range.start);
+    let end = positioner.byte_to_char(byte_range.end);
     Range {
-      start: to_pos(start_pos, byte_range.start),
-      end: to_pos(end_pos, byte_range.end),
+      start: to_pos(start_pos, start),
+      end: to_pos(end_pos, end),
     }
   }
 }
```

### Comparing `ast_grep_py-0.22.4/crates/pyo3/tests/test_range.py` & `ast_grep_py-0.22.5/crates/pyo3/tests/test_range.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,9 +42,8 @@
 
 def test_unicode():
     source = "ハロ = console.log(世界)".strip()
     sg = SgRoot(source, "javascript")
     root = sg.root()
     node = root.find(pattern="console.log($A)")
     assert node is not None
-    # it should be unicode char offset, but currently it's byte offset
-    assert node.range().start.index == 9
+    assert node.range().start.index == 5
```

### Comparing `ast_grep_py-0.22.4/crates/pyo3/tests/test_rule.py` & `ast_grep_py-0.22.5/crates/pyo3/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/tests/test_simple.py` & `ast_grep_py-0.22.5/crates/pyo3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/tests/test_traversal.py` & `ast_grep_py-0.22.5/crates/pyo3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/crates/pyo3/tests/test_wrong_usage.py` & `ast_grep_py-0.22.5/crates/pyo3/tests/test_wrong_usage.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/Cargo.lock` & `ast_grep_py-0.22.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -140,15 +140,15 @@
  "similar",
  "tempfile",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "schemars",
@@ -156,38 +156,38 @@
  "serde_yaml",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "serde",
  "tree-sitter-bash",
  "tree-sitter-c",
  "tree-sitter-c-sharp",
@@ -210,47 +210,48 @@
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "dashmap",
  "serde",
  "serde_json",
  "tokio",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
+ "ast-grep-language",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
  "serde_json",
  "tree-sitter-css",
  "tree-sitter-facade-sg",
  "tree-sitter-html",
  "tree-sitter-javascript-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-py"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "anyhow",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "pyo3",
  "pythonize",
@@ -308,15 +309,15 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "benches"
-version = "0.22.4"
+version = "0.22.5"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -1721,17 +1722,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.37.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
+checksum = "ba4f4a02a7a80d6f274636f0aa95c7e383b912d41fe721a31f29e29698585a4a"
 dependencies = [
  "backtrace",
  "bytes",
  "num_cpus",
  "pin-project-lite",
 ]
 
@@ -1874,17 +1875,17 @@
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-c"
-version = "0.21.3"
+version = "0.21.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e942d789b24dda298d41c95db353841159232feb80a52103c717e7c062bb9f3"
+checksum = "f956d5351d62652864a4ff3ae861747e7a1940dc96c9998ae400ac0d3ce30427"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-c-sharp"
```

### Comparing `ast_grep_py-0.22.4/Cargo.toml` & `ast_grep_py-0.22.5/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 default-members = ["crates/*"]
 resolver = "2"
 
 [profile.release]
 lto = true
 
 [workspace.package]
-version = "0.22.4"
+version = "0.22.5"
 authors = ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition = "2021"
 license = "MIT"
 documentation = "https://ast-grep.github.io/guide/introduction.html"
 homepage = "https://ast-grep.github.io/"
 repository = "https://github.com/ast-grep/ast-grep"
 rust-version = "1.67"
 readme = "README.md"
 
 [workspace.dependencies]
-ast-grep-core = { path = "crates/core", version = "0.22.4" }
-ast-grep-config = { path = "crates/config", version = "0.22.4" }
-ast-grep-dynamic = { path = "crates/dynamic", version = "0.22.4" }
-ast-grep-language = { path = "crates/language", version = "0.22.4" }
-ast-grep-lsp = { path = "crates/lsp", version = "0.22.4" }
+ast-grep-core = { path = "crates/core", version = "0.22.5" }
+ast-grep-config = { path = "crates/config", version = "0.22.5" }
+ast-grep-dynamic = { path = "crates/dynamic", version = "0.22.5" }
+ast-grep-language = { path = "crates/language", version = "0.22.5" }
+ast-grep-lsp = { path = "crates/lsp", version = "0.22.5" }
 
 bit-set = { version = "0.5.3" }
 ignore = { version = "0.4.22" }
 regex = { version = "1.10.4" }
 serde = { version = "1.0.200", features = ["derive"] }
 tree-sitter = { version = "0.21.4", package = "tree-sitter-facade-sg" }
 thiserror = "1.0.59"
```

### Comparing `ast_grep_py-0.22.4/pyproject.toml` & `ast_grep_py-0.22.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-py"
 requires-python = ">=3.8"
-version = "0.22.4"
+version = "0.22.5"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_py-0.22.4/ast_grep_py/__init__.py` & `ast_grep_py-0.22.5/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.22.5/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/README.md` & `ast_grep_py-0.22.5/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.22.4/PKG-INFO` & `ast_grep_py-0.22.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ast-grep-py
-Version: 0.22.4
+Version: 0.22.5
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

