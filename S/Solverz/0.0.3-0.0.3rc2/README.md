# Comparing `tmp/solverz-0.0.3.tar.gz` & `tmp/solverz-0.0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solverz-0.0.3.tar", last modified: Mon Jun  3 13:51:39 2024, max compression
+gzip compressed data, was "solverz-0.0.3rc2.tar", last modified: Mon Jun  3 13:39:07 2024, max compression
```

## Comparing `solverz-0.0.3.tar` & `solverz-0.0.3rc2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.846237 solverz-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 13:51:29.000000 solverz-0.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.822237 solverz-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.826237 solverz-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-03 13:51:29.000000 solverz-0.0.3/.github/workflows/cookbook-practice.yml
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-06-03 13:51:29.000000 solverz-0.0.3/.github/workflows/debug github action.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-03 13:51:29.000000 solverz-0.0.3/.github/workflows/doc-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-06-03 13:51:29.000000 solverz-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-03 13:51:29.000000 solverz-0.0.3/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-06-03 13:51:29.000000 solverz-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-03 13:51:29.000000 solverz-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-06-03 13:51:39.846237 solverz-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-06-03 13:51:29.000000 solverz-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.826237 solverz-0.0.3/Solverz/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-03 13:51:39.000000 solverz-0.0.3/Solverz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/make_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/matlab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/matlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/matlab/matlab_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/python/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/python/inline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/inline/inline_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/python/inline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/inline/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/inline/tests/test_inline_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/python/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/module/module_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/module/module_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/python/module/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/module/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/module/test/test_module_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/module/test/test_module_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.830237 solverz-0.0.3/Solverz/code_printer/python/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/code_printer/python/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.834237 solverz-0.0.3/Solverz/equation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/eqn.py
--rw-r--r--   0 runner    (1001) docker     (127)    21900 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/equations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/jac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/param.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.834237 solverz-0.0.3/Solverz/equation/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/test/test_DAE.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/test/test_Param.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/test/test_eqn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/test/test_jac.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/equation/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.834237 solverz-0.0.3/Solverz/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/model/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.834237 solverz-0.0.3/Solverz/num_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/Array.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/custom_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/num_eqn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/numjac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.834237 solverz-0.0.3/Solverz/num_api/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/test/test_Array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/test/test_custom_func.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/num_api/test/test_numjac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.834237 solverz-0.0.3/Solverz/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.838237 solverz-0.0.3/Solverz/solvers/daesolver/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/daesolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/daesolver/beuler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/daesolver/daeic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/daesolver/rodas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/daesolver/trapezoidal.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/daesolver/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/fdesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/laesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.838237 solverz-0.0.3/Solverz/solvers/nlaesolver/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/nlaesolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/nlaesolver/cnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/nlaesolver/lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/nlaesolver/nr.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/nlaesolver/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.838237 solverz-0.0.3/Solverz/solvers/odesolver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/odesolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/odesolver/ode45.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/odesolver/rock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.838237 solverz-0.0.3/Solverz/solvers/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/solvers/test/test_rodas_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.838237 solverz-0.0.3/Solverz/sym_algebra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/matrix_calculus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.842237 solverz-0.0.3/Solverz/sym_algebra/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/test/test_finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/test/test_matrix_calculus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/test/test_num_alg.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/test/test_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/sym_algebra/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.842237 solverz-0.0.3/Solverz/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/utilities/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/utilities/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/utilities/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.842237 solverz-0.0.3/Solverz/utilities/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/utilities/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/utilities/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/utilities/type_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.842237 solverz-0.0.3/Solverz/variable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/variable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/variable/ssymbol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.842237 solverz-0.0.3/Solverz/variable/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/variable/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/variable/test/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-06-03 13:51:29.000000 solverz-0.0.3/Solverz/variable/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.846237 solverz-0.0.3/Solverz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-06-03 13:51:39.000000 solverz-0.0.3/Solverz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-06-03 13:51:39.000000 solverz-0.0.3/Solverz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:51:39.000000 solverz-0.0.3/Solverz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-03 13:51:39.000000 solverz-0.0.3/Solverz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 13:51:39.000000 solverz-0.0.3/Solverz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.842237 solverz-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.842237 solverz-0.0.3/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/ext/convert-svg-to-pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/ext/docscrape.py
--rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/ext/docscrape_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/ext/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.846237 solverz-0.0.3/docs/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.846237 solverz-0.0.3/docs/src/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    68647 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/_static/sympylogo.png
--rw-r--r--   0 runner    (1001) docker     (127)   167361 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/_static/sympylogo_big.png
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/advanced.md
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/gethelp.md
--rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/gettingstart.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.846237 solverz-0.0.3/docs/src/pics/
--rw-r--r--   0 runner    (1001) docker     (127)   191208 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/pics/Hierarchy_of_equations.png
--rw-r--r--   0 runner    (1001) docker     (127)    53578 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/pics/difference_stencil.png
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/pics/res.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.846237 solverz-0.0.3/docs/src/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-03 13:51:29.000000 solverz-0.0.3/docs/src/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-06-03 13:51:29.000000 solverz-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-03 13:51:29.000000 solverz-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-06-03 13:51:29.000000 solverz-0.0.3/res.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:51:39.846237 solverz-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:51:39.846237 solverz-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 13:51:29.000000 solverz-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21963 2024-06-03 13:51:29.000000 solverz-0.0.3/tests/dae_test.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 13:51:29.000000 solverz-0.0.3/tests/test_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-06-03 13:51:29.000000 solverz-0.0.3/tests/test_dae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.247063 solverz-0.0.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.219064 solverz-0.0.3rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.227064 solverz-0.0.3rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/.github/workflows/cookbook-practice.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/.github/workflows/debug github action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/.github/workflows/doc-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-06-03 13:39:07.247063 solverz-0.0.3rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.227064 solverz-0.0.3rc2/Solverz/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-03 13:39:07.000000 solverz-0.0.3rc2/Solverz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.227064 solverz-0.0.3rc2/Solverz/code_printer/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/make_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.227064 solverz-0.0.3rc2/Solverz/code_printer/matlab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/matlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/matlab/matlab_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.227064 solverz-0.0.3rc2/Solverz/code_printer/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.227064 solverz-0.0.3rc2/Solverz/code_printer/python/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/inline/inline_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.227064 solverz-0.0.3rc2/Solverz/code_printer/python/inline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/inline/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/inline/tests/test_inline_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.231063 solverz-0.0.3rc2/Solverz/code_printer/python/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/module/module_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/module/module_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.231063 solverz-0.0.3rc2/Solverz/code_printer/python/module/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/module/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9251 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/module/test/test_module_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/module/test/test_module_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.231063 solverz-0.0.3rc2/Solverz/code_printer/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/code_printer/python/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.231063 solverz-0.0.3rc2/Solverz/equation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/eqn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21900 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/jac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/param.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.231063 solverz-0.0.3rc2/Solverz/equation/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/test/test_DAE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/test/test_Param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/test/test_eqn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/test/test_jac.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/equation/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.231063 solverz-0.0.3rc2/Solverz/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/model/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.235063 solverz-0.0.3rc2/Solverz/num_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/Array.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/custom_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/num_eqn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/numjac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.235063 solverz-0.0.3rc2/Solverz/num_api/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/test/test_Array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/test/test_custom_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/num_api/test/test_numjac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.235063 solverz-0.0.3rc2/Solverz/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.235063 solverz-0.0.3rc2/Solverz/solvers/daesolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/daesolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/daesolver/beuler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/daesolver/daeic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/daesolver/rodas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/daesolver/trapezoidal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/daesolver/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/fdesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/laesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.235063 solverz-0.0.3rc2/Solverz/solvers/nlaesolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/nlaesolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/nlaesolver/cnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/nlaesolver/lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/nlaesolver/nr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/nlaesolver/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/solvers/odesolver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/odesolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/odesolver/ode45.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/odesolver/rock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/solvers/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/solvers/test/test_rodas_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/sym_algebra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/matrix_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/sym_algebra/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/test/test_finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/test/test_matrix_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/test/test_num_alg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/test/test_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/sym_algebra/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/utilities/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/utilities/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/utilities/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/utilities/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/utilities/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/utilities/type_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/variable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/variable/ssymbol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.239063 solverz-0.0.3rc2/Solverz/variable/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/variable/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/variable/test/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/Solverz/variable/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.247063 solverz-0.0.3rc2/Solverz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-06-03 13:39:07.000000 solverz-0.0.3rc2/Solverz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-06-03 13:39:07.000000 solverz-0.0.3rc2/Solverz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 13:39:07.000000 solverz-0.0.3rc2/Solverz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-03 13:39:07.000000 solverz-0.0.3rc2/Solverz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 13:39:07.000000 solverz-0.0.3rc2/Solverz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.243064 solverz-0.0.3rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.243064 solverz-0.0.3rc2/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/ext/convert-svg-to-pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16828 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/ext/docscrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/ext/docscrape_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/ext/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.243064 solverz-0.0.3rc2/docs/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.243064 solverz-0.0.3rc2/docs/src/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    68647 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/_static/sympylogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   167361 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/_static/sympylogo_big.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/gethelp.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14103 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/gettingstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.247063 solverz-0.0.3rc2/docs/src/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)   191208 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/pics/Hierarchy_of_equations.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53578 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/pics/difference_stencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/pics/res.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.247063 solverz-0.0.3rc2/docs/src/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/docs/src/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/res.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 13:39:07.247063 solverz-0.0.3rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 13:39:07.247063 solverz-0.0.3rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21963 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/tests/dae_test.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/tests/test_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-06-03 13:38:59.000000 solverz-0.0.3rc2/tests/test_dae.py
```

### Comparing `solverz-0.0.3/.github/workflows/cookbook-practice.yml` & `solverz-0.0.3rc2/.github/workflows/cookbook-practice.yml`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/.github/workflows/debug github action.yml` & `solverz-0.0.3rc2/.github/workflows/debug github action.yml`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/.github/workflows/doc-deploy.yml` & `solverz-0.0.3rc2/.github/workflows/doc-deploy.yml`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/.github/workflows/publish-to-pypi.yml` & `solverz-0.0.3rc2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/LICENSE` & `solverz-0.0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/PKG-INFO` & `solverz-0.0.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Solverz
-Version: 0.0.3
+Version: 0.0.3rc2
 Summary: A simulation modelling language
 Author-email: Ruizhi Yu <rz.yu@foxmail.com>
 Project-URL: Homepage, https://github.com/smallbunnies/Solverz
 Project-URL: Issues, https://github.com/smallbunnies/Solverz/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `solverz-0.0.3/README.md` & `solverz-0.0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/__init__.py` & `solverz-0.0.3rc2/Solverz/__init__.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/make_module.py` & `solverz-0.0.3rc2/Solverz/code_printer/make_module.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/inline/inline_printer.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/inline/inline_printer.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/inline/tests/test_inline_printer.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/inline/tests/test_inline_printer.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/module/module_generator.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/module/module_generator.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/module/module_printer.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/module/module_printer.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/module/test/test_module_generator.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/module/test/test_module_generator.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/module/test/test_module_printer.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/module/test/test_module_printer.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/tests/test_utilities.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/code_printer/python/utilities.py` & `solverz-0.0.3rc2/Solverz/code_printer/python/utilities.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/eqn.py` & `solverz-0.0.3rc2/Solverz/equation/eqn.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/equations.py` & `solverz-0.0.3rc2/Solverz/equation/equations.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/jac.py` & `solverz-0.0.3rc2/Solverz/equation/jac.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/param.py` & `solverz-0.0.3rc2/Solverz/equation/param.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/test/test_DAE.py` & `solverz-0.0.3rc2/Solverz/equation/test/test_DAE.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/test/test_Param.py` & `solverz-0.0.3rc2/Solverz/equation/test/test_Param.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/test/test_eqn.py` & `solverz-0.0.3rc2/Solverz/equation/test/test_eqn.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/equation/test/test_jac.py` & `solverz-0.0.3rc2/Solverz/equation/test/test_jac.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/model/basic.py` & `solverz-0.0.3rc2/Solverz/model/basic.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/num_api/Array.py` & `solverz-0.0.3rc2/Solverz/num_api/Array.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/num_api/custom_function.py` & `solverz-0.0.3rc2/Solverz/num_api/custom_function.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/num_api/num_eqn.py` & `solverz-0.0.3rc2/Solverz/num_api/num_eqn.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/num_api/numjac.py` & `solverz-0.0.3rc2/Solverz/num_api/numjac.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/num_api/test/test_Array.py` & `solverz-0.0.3rc2/Solverz/num_api/test/test_Array.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/num_api/test/test_custom_func.py` & `solverz-0.0.3rc2/Solverz/num_api/test/test_custom_func.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/num_api/test/test_numjac.py` & `solverz-0.0.3rc2/Solverz/num_api/test/test_numjac.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/daesolver/beuler.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/beuler.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/daesolver/daeic.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/daeic.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/daesolver/rodas.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/rodas.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/daesolver/trapezoidal.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/trapezoidal.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/daesolver/utilities.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/utilities.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/fdesolver.py` & `solverz-0.0.3rc2/Solverz/solvers/fdesolver.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/laesolver.py` & `solverz-0.0.3rc2/Solverz/solvers/laesolver.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/nlaesolver/cnr.py` & `solverz-0.0.3rc2/Solverz/solvers/nlaesolver/cnr.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/nlaesolver/lm.py` & `solverz-0.0.3rc2/Solverz/solvers/nlaesolver/lm.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/nlaesolver/nr.py` & `solverz-0.0.3rc2/Solverz/solvers/nlaesolver/nr.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/odesolver/ode45.py` & `solverz-0.0.3rc2/Solverz/solvers/odesolver/ode45.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/option.py` & `solverz-0.0.3rc2/Solverz/solvers/option.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/parser.py` & `solverz-0.0.3rc2/Solverz/solvers/parser.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/solution.py` & `solverz-0.0.3rc2/Solverz/solvers/solution.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/solvers/test/test_rodas_event.py` & `solverz-0.0.3rc2/Solverz/solvers/test/test_rodas_event.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/sym_algebra/functions.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/functions.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/sym_algebra/matrix_calculus.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/matrix_calculus.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/sym_algebra/symbols.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/symbols.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/sym_algebra/test/test_finite_difference.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/test/test_finite_difference.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/sym_algebra/test/test_matrix_calculus.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/test/test_matrix_calculus.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/sym_algebra/test/test_num_alg.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/test/test_num_alg.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/sym_algebra/transform.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/transform.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/utilities/address.py` & `solverz-0.0.3rc2/Solverz/utilities/address.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/utilities/io.py` & `solverz-0.0.3rc2/Solverz/utilities/io.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/utilities/test/test_address.py` & `solverz-0.0.3rc2/Solverz/utilities/test/test_address.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/utilities/type_checker.py` & `solverz-0.0.3rc2/Solverz/utilities/type_checker.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/variable/ssymbol.py` & `solverz-0.0.3rc2/Solverz/variable/ssymbol.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/variable/test/test_variable.py` & `solverz-0.0.3rc2/Solverz/variable/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz/variable/variables.py` & `solverz-0.0.3rc2/Solverz/variable/variables.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/Solverz.egg-info/PKG-INFO` & `solverz-0.0.3rc2/Solverz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Solverz
-Version: 0.0.3
+Version: 0.0.3rc2
 Summary: A simulation modelling language
 Author-email: Ruizhi Yu <rz.yu@foxmail.com>
 Project-URL: Homepage, https://github.com/smallbunnies/Solverz
 Project-URL: Issues, https://github.com/smallbunnies/Solverz/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `solverz-0.0.3/Solverz.egg-info/SOURCES.txt` & `solverz-0.0.3rc2/Solverz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/Makefile` & `solverz-0.0.3rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/ext/convert-svg-to-pdf.py` & `solverz-0.0.3rc2/docs/ext/convert-svg-to-pdf.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/ext/docscrape.py` & `solverz-0.0.3rc2/docs/ext/docscrape.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/ext/docscrape_sphinx.py` & `solverz-0.0.3rc2/docs/ext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/ext/numpydoc.py` & `solverz-0.0.3rc2/docs/ext/numpydoc.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/make.bat` & `solverz-0.0.3rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/_static/custom.css` & `solverz-0.0.3rc2/docs/src/_static/custom.css`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/_static/sympylogo.png` & `solverz-0.0.3rc2/docs/src/_static/sympylogo.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/_static/sympylogo_big.png` & `solverz-0.0.3rc2/docs/src/_static/sympylogo_big.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/advanced.md` & `solverz-0.0.3rc2/docs/src/advanced.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/conf.py` & `solverz-0.0.3rc2/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/gettingstart.md` & `solverz-0.0.3rc2/docs/src/gettingstart.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/index.rst` & `solverz-0.0.3rc2/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/intro.md` & `solverz-0.0.3rc2/docs/src/intro.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/pics/Hierarchy_of_equations.png` & `solverz-0.0.3rc2/docs/src/pics/Hierarchy_of_equations.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/pics/difference_stencil.png` & `solverz-0.0.3rc2/docs/src/pics/difference_stencil.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/pics/res.png` & `solverz-0.0.3rc2/docs/src/pics/res.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/docs/src/reference/index.rst` & `solverz-0.0.3rc2/docs/src/reference/index.rst`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/pyproject.toml` & `solverz-0.0.3rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/res.png` & `solverz-0.0.3rc2/res.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/tests/dae_test.xlsx` & `solverz-0.0.3rc2/tests/dae_test.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.3/tests/test_dae.py` & `solverz-0.0.3rc2/tests/test_dae.py`

 * *Files identical despite different names*

