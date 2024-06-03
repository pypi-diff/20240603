# Comparing `tmp/solverz-0.0.1rc4.tar.gz` & `tmp/solverz-0.0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "solverz-0.0.3rc2.tar", last modified: Mon Jun  3 13:39:07 2024, max compression
```

## Comparing `solverz-0.0.1rc4.tar` & `solverz-0.0.3rc2.tar`

### file list

```diff
@@ -1,127 +1,168 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/.gitattributes
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/requirements.txt
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/res.png
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/.github/workflows/debug github action.yml
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/.github/workflows/doc-deploy.yml
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/code_printer/__init__.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/code_printer/make_module.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/code_printer/make_pyfunc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/code_printer/matlab_printer.py
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/code_printer/py_printer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/code_printer/test/__init__.py
--rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/code_printer/test/test_py_printer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/__init__.py
--rw-r--r--   0        0        0    17407 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/eqn.py
--rw-r--r--   0        0        0    25834 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/equations.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/param.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/trigger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/test/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/test/test_DAE.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/test/test_Param.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/test/test_eqn.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/equation/test/test_jac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/model/__init__.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/model/basic.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/Array.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/__init__.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/custom_function.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/num_eqn.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/numjac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/test/__init__.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/test/test_Array.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/test/test_custom_func.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/num_api/test/test_numjac.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/__init__.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/fdesolver.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/laesolver.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/option.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/parser.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/solution.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/stats.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/daesolver/__init__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/daesolver/beuler.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/daesolver/daeic.py
--rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/daesolver/rodas.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/daesolver/trapezoidal.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/daesolver/utilities.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/nlaesolver/__init__.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/nlaesolver/cnr.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/nlaesolver/lm.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/nlaesolver/nr.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/nlaesolver/utilities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/odesolver/__init__.py
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/odesolver/ode45.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/odesolver/rock.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/test/__init__.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/solvers/test/test_rodas_event.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/__init__.py
--rw-r--r--   0        0        0    16332 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/functions.py
--rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/matrix_calculus.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/symbols.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/test/__init__.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/test/test_finite_difference.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/test/test_matrix_calculus.py
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/test/test_num_alg.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/sym_algebra/test/test_symbols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/utilities/__init__.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/utilities/address.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/utilities/io.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/utilities/profile.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/utilities/type_checker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/utilities/test/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/utilities/test/test_address.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/variable/__init__.py
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/variable/ssymbol.py
--rw-r--r--   0        0        0     9663 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/variable/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/variable/test/__init__.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/Solverz/variable/test/test_variable.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/Makefile
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/make.bat
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/requirements.txt
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/ext/convert-svg-to-pdf.py
--rw-r--r--   0        0        0    16828 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/ext/docscrape.py
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/ext/docscrape_sphinx.py
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/ext/numpydoc.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/advanced.md
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/conf.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/contributing.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/gethelp.md
--rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/gettingstart.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/index.rst
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/install.md
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/intro.md
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/_static/custom.css
--rw-r--r--   0        0        0    68647 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/_static/sympylogo.png
--rw-r--r--   0        0        0   167361 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/_static/sympylogo_big.png
--rw-r--r--   0        0        0   191208 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/pics/Hierarchy_of_equations.png
--rw-r--r--   0        0        0    53578 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/pics/difference_stencil.png
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/pics/res.png
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/docs/src/reference/index.rst
--rw-r--r--   0        0        0    19896 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/4node3pipe.xlsx
--rw-r--r--   0        0        0    17001 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/4node3pipe_bench.xlsx
--rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/4node3pipe_change_sign.xlsx
--rw-r--r--   0        0        0    15910 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/4node3pipe_change_sign_bench.xlsx
--rw-r--r--   0        0        0    21963 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/dae_test.xlsx
--rw-r--r--   0        0        0    30787 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/dynamic_gas_flow_single_pipe.xlsx
--rw-r--r--   0        0        0    12608 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/ode_test.xlsx
--rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/test_burger.xlsx
--rw-r--r--   0        0        0  1412117 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/test_m3b9.xlsx
--rw-r--r--   0        0        0    41225 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/test_ode45.xlsx
--rw-r--r--   0        0        0  2246743 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/instances/test_sirk.xlsx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/test_0.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/test_dae.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/test_dhspf.py
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/test_dhspf_change_sign.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/test_dyn_gas_flow_single_pipe.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/test_gasflow.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/tests/test_m3b9.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/LICENSE
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/pyproject.toml
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 solverz-0.0.1rc4/PKG-INFO
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

### Comparing `solverz-0.0.1rc4/res.png` & `solverz-0.0.3rc2/docs/src/pics/res.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/.github/workflows/debug github action.yml` & `solverz-0.0.3rc2/.github/workflows/debug github action.yml`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/.github/workflows/doc-deploy.yml` & `solverz-0.0.3rc2/.github/workflows/doc-deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -15,36 +15,37 @@
     runs-on: ubuntu-latest
     name: Build and Deploy Job
     steps:
       - uses: actions/checkout@v3
         with:
           submodules: true
           lfs: false
-      - name: Bulid Docs
+      - name: Deploy Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.11'
           cache: 'pip' # caching pip dependencies
-      - run: |
+      - name: Build Docs
+        run: |
           pip install -r requirements.txt
           cd docs
           pip install -r requirements.txt
           make html
       - name: Deploy
         id: builddeploy
         uses: Azure/static-web-apps-deploy@v1
         with:
           azure_static_web_apps_api_token: ${{ secrets.AZURE_STATIC_WEB_APPS_API_TOKEN_KIND_MUSHROOM_012AD4400 }}
           repo_token: ${{ secrets.GITHUB_TOKEN }} # Used for Github integrations (i.e. PR comments)
           action: "upload"
           ###### Repository/Build Configurations - These values can be configured to match your app requirements. ######
           # For more information regarding Static Web App workflow configurations, please visit: https://aka.ms/swaworkflowconfig
-          app_location: "/" # App source code path
-          api_location: "" # Api source code path - optional
-          output_location: "docs/build/html" # Built app content directory - optional
+          app_location: "docs/build/html" # App source code path
+          output_location: "" # Built app content directory - optional
+          skip_app_build: true
           ###### End of Repository/Build Configurations ######
 
   close_pull_request_job:
     if: github.event_name == 'pull_request' && github.event.action == 'closed'
     runs-on: ubuntu-latest
     name: Close Pull Request Job
     steps:
```

### Comparing `solverz-0.0.1rc4/.github/workflows/publish-to-pypi.yml` & `solverz-0.0.3rc2/.github/workflows/publish-to-pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Publish Python 🐍 distribution 📦 to PyPI
+name: Publish to Pypi
 
 on: push
 
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
```

### Comparing `solverz-0.0.1rc4/Solverz/__init__.py` & `solverz-0.0.3rc2/Solverz/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,12 @@
 from Solverz.equation.equations import AE, FDAE, DAE
 from Solverz.equation.param import Param, IdxParam, TimeSeriesParam
 from Solverz.sym_algebra.symbols import idx, Para, iVar, iAliasVar
 from Solverz.sym_algebra.functions import Sign, Abs, transpose, exp, Diag, Mat_Mul, sin, cos, Min, AntiWindUp, Saturation
 from Solverz.num_api.custom_function import minmod_flag, minmod
 from Solverz.variable.variables import Vars, TimeVars, as_Vars
 from Solverz.solvers import *
-from Solverz.code_printer.make_pyfunc import made_numerical
-from Solverz.code_printer.py_printer import render_modules
-from Solverz.code_printer.make_module import module_printer
+from Solverz.code_printer import made_numerical, module_printer
 from Solverz.utilities.io import save, load, save_result
 from Solverz.utilities.profile import count_time
 from Solverz.variable.ssymbol import Var, AliasVar
 from Solverz.model.basic import Model
```

### Comparing `solverz-0.0.1rc4/Solverz/code_printer/make_module.py` & `solverz-0.0.3rc2/Solverz/code_printer/make_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from Solverz.code_printer.py_printer import render_modules as py_module_renderer
+from Solverz.code_printer.python import py_module_renderer
 from Solverz.equation.equations import AE, FDAE, DAE
 from Solverz.variable.variables import Vars
 
 
 class module_printer:
     def __init__(self,
                  mdl: AE | FDAE | DAE,
```

### Comparing `solverz-0.0.1rc4/Solverz/equation/eqn.py` & `solverz-0.0.3rc2/Solverz/equation/eqn.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from Solverz.sym_algebra.symbols import iVar, Para, IdxVar, idx, IdxPara, iAliasVar, IdxAliasVar
 from Solverz.variable.ssymbol import Var
 from Solverz.sym_algebra.functions import Mat_Mul, Slice, F
 from Solverz.sym_algebra.matrix_calculus import MixedEquationDiff
 from Solverz.sym_algebra.transform import finite_difference, semi_descritize
 from Solverz.num_api.custom_function import numerical_interface
+from Solverz.variable.ssymbol import sSym2Sym
 
 
 def sVar2Var(var: Union[Var, iVar, List[iVar, Var]]) -> Union[iVar, List[iVar]]:
     if isinstance(var, list):
         return [arg.symbol if isinstance(arg, Var) else arg for arg in var]
     else:
         return var.symbol if isinstance(var, Var) else var
@@ -51,15 +52,17 @@
         for symbol_ in list((self.LHS - self.RHS).free_symbols):
             if isinstance(symbol_, (iVar, Para, idx, iAliasVar)):
                 temp_dict[symbol_.name] = symbol_
             elif isinstance(symbol_, (IdxVar, IdxPara, IdxAliasVar)):
                 temp_dict[symbol_.name0] = symbol_.symbol0
                 temp_dict.update(symbol_.SymInIndex)
 
-        return temp_dict
+        # to sort in lexicographic order
+        sorted_dict = {key: temp_dict[key] for key in sorted(temp_dict)}
+        return sorted_dict
 
     def lambdify(self) -> Callable:
         return splambdify(self.SYMBOLS.values(), self.RHS, [numerical_interface, 'numpy'])
 
     def eval(self, *args: Union[np.ndarray]) -> np.ndarray:
         return self.NUM_EQN(*args)
 
@@ -144,16 +147,16 @@
     where $y$ is the state vector.
 
     """
 
     def __init__(self, name: str,
                  f,
                  diff_var: Union[iVar, IdxVar, Var]):
-        super().__init__(name, sVar2Var(f))
-        diff_var = sVar2Var(diff_var)
+        super().__init__(name, sSym2Sym(f))
+        diff_var = sSym2Sym(diff_var)
         self.diff_var = diff_var
         self.LHS = Derivative(diff_var, t)
 
 
 class Pde(Eqn):
     """
     The class of partial differential equations
```

### Comparing `solverz-0.0.1rc4/Solverz/equation/equations.py` & `solverz-0.0.3rc2/Solverz/equation/equations.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from Solverz.equation.eqn import Eqn, Ode, EqnDiff
 from Solverz.equation.param import ParamBase, Param, IdxParam
 from Solverz.sym_algebra.symbols import iVar, idx, IdxVar, Para, iAliasVar
 from Solverz.sym_algebra.functions import Slice
 from Solverz.variable.variables import Vars
 from Solverz.utilities.address import Address, combine_Address
 from Solverz.num_api.Array import Array
+from Solverz.equation.jac import Jac, JacBlock
 
 
 class Equations:
 
     def __init__(self,
                  eqn: Union[List[Eqn], Eqn],
                  name: str = None,
@@ -35,14 +36,16 @@
         self.vsize: int = 0  # size of variables
         self.f_list = []
         self.g_list = []
         self.matrix_container = matrix_container
         self.PARAM: Dict[str, ParamBase] = dict()
         self.triggerable_quantity: Dict[str, str] = dict()
         self.jac_element_address = Address()
+        self.jac: Jac = Jac()
+        self.nstep = 0
 
         if isinstance(eqn, Eqn):
             eqn = [eqn]
 
         for eqn_ in eqn:
             self.add_eqn(eqn_)
 
@@ -54,25 +57,63 @@
         self.a.add(eqn.name)
         if isinstance(eqn, Eqn) and not isinstance(eqn, Ode):
             self.g_list = self.g_list + [eqn.name]
         elif isinstance(eqn, Ode):
             self.f_list = self.f_list + [eqn.name]
 
         for symbol_ in eqn.SYMBOLS.values():
-            if isinstance(symbol_, (Para, iAliasVar)):
+            if isinstance(symbol_, Para):
                 # this is not fully initialize of Parameters, please use param_initializer
-                self.PARAM[symbol_.name] = Param(symbol_.name, value=symbol_.value, dim=symbol_.dim)
+                self.PARAM[symbol_.name] = Param(symbol_.name,
+                                                 value=symbol_.value,
+                                                 dim=symbol_.dim)
+            elif isinstance(symbol_, iAliasVar):
+                self.PARAM[symbol_.name] = Param(symbol_.name,
+                                                 value=symbol_.value,
+                                                 dim=symbol_.dim,
+                                                 is_alias=True)
             elif isinstance(symbol_, idx):
                 self.PARAM[symbol_.name] = IdxParam(symbol_.name, value=symbol_.value)
 
         self.EQNs[eqn.name].derive_derivative()
 
-    def assign_eqn_var_address(self, *xys: Vars):
+    def assign_eqn_var_address(self, *args):
         pass
 
+    def Fy(self, y) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
+        pass
+
+    def FormJac(self, y):
+        self.assign_eqn_var_address(y)
+
+        Fy_list = self.Fy(y)
+        for fy in Fy_list:
+            EqnName = fy[0]
+            EqnAddr = self.a[EqnName]
+            VarName = fy[1]
+            VarAddr = self.var_address[VarName]
+            DiffVar = fy[2].diff_var
+            DeriExpr = fy[2].RHS
+
+            DiffVarEqn = Eqn('DiffVarEqn' + DiffVar.name, DiffVar)
+            args = self.obtain_eqn_args(DiffVarEqn, y, 0)
+            DiffVarValue = Array(DiffVarEqn.NUM_EQN(*args), dim=1)
+
+            # The value of deri can be either matrix, vector, or scalar(number). We cannot reshape it.
+            Value0 = np.array(fy[3])
+
+            jb = JacBlock(EqnName,
+                          EqnAddr,
+                          DiffVar,
+                          DiffVarValue,
+                          VarAddr,
+                          DeriExpr,
+                          Value0)
+            self.jac.add_block(EqnName, DiffVar, jb)
+
     @property
     def eqn_size(self):
         # total size of all the equations
         return np.sum(np.array(list(self.esize.values())))
 
     def is_param_defined(self, param: str) -> bool:
 
@@ -117,103 +158,74 @@
         Evaluate equations
         :param eqn_name:
         :param args:
         :return:
         """
         return Array(self.EQNs[eqn_name].NUM_EQN(*args), dim=1)
 
-    def trigger_param_updater(self, eqn: Eqn, *xys):
+    def trigger_param_updater(self, y):
         # update/initialize triggerable params
-        if len(xys) > 0:
-            for para_name, trigger_var in self.triggerable_quantity.items():
-                trigger_func = self.PARAM[para_name].trigger_fun
-                args = []
-                for var in trigger_var:
-                    var_value = None
-                    if var in self.PARAM:
-                        var_value = self.PARAM[var].v
-                    else:
-                        for y in xys:
-                            if var in y.var_list:
-                                var_value = y[var]
-                    if var_value is None:
-                        raise ValueError(f'Para/iVar {var} not defined')
-                    else:
-                        args.append(var_value)
-                temp = trigger_func(*args)
-                if self.PARAM[para_name].v is None:
-                    self.PARAM[para_name].v = temp
+        for para_name, trigger_var in self.triggerable_quantity.items():
+            trigger_func = self.PARAM[para_name].trigger_fun
+            args = []
+            for var in trigger_var:
+                var_value = None
+                if var in self.PARAM:
+                    var_value = self.PARAM[var].v
+                else:
+                    if var in y.var_list:
+                        var_value = y[var]
+                if var_value is None:
+                    raise ValueError(f'Para/iVar {var} not defined')
                 else:
-                    if type(temp) is not type(self.PARAM[para_name].v):
-                        raise TypeError(
-                            f"The return types of trigger func for param {para_name} must be {type(self.PARAM[para_name].v)}")
+                    args.append(var_value)
+            temp = trigger_func(*args)
+            if self.PARAM[para_name].v is None:
+                self.PARAM[para_name].v = temp
+            else:
+                if type(temp) is not type(self.PARAM[para_name].v):
+                    raise TypeError(
+                        f"The return types of trigger func for param {para_name} must be {type(self.PARAM[para_name].v)}")
 
-    def obtain_eqn_args(self, eqn: Eqn, t=None, *xys: Vars) -> List[np.ndarray]:
+    def obtain_eqn_args(self, eqn: Eqn, y: Vars, t=0) -> List[np.ndarray]:
         """
         Obtain the args of equations
         """
 
-        self.trigger_param_updater(eqn, *xys)
+        self.trigger_param_updater(y)
 
         args = []
         for symbol in eqn.SYMBOLS.values():
             value_obtained = False
             if symbol.name in self.PARAM:
                 temp = self.PARAM[symbol.name].get_v_t(t)
                 if temp is None:
                     raise TypeError(f'Parameter {symbol.name} uninitialized')
                 args.append(temp)
                 value_obtained = True
             else:
-                for y in xys:
-                    if symbol.name in y.var_list:
-                        args.append(y[symbol.name])
-                        value_obtained = True
+                if symbol.name in y.var_list:
+                    args.append(y[symbol.name])
+                    value_obtained = True
             if not value_obtained:
                 raise ValueError(f'Cannot find the values of variable {symbol.name}')
         return args
 
     def eval_diffs(self, eqn_name: str, var_name: str, *args: np.ndarray) -> np.ndarray:
         """
         Evaluate derivative of equations
         :param eqn_name:
         :param var_name:
         :param args:
         :return:
         """
         return self.EQNs[eqn_name].derivatives[var_name].NUM_EQN(*args)
 
-    def parse_address(self, eqn_name, var_name, eqndiff, t=None, *xys):
-        var_idx = eqndiff.var_idx
-        var_idx_func = eqndiff.var_idx_func
-
-        equation_address = self.a.v[eqn_name]
-        if var_idx is None:
-            variable_address = self.var_address.v[var_name]
-        elif isinstance(var_idx, (float, int)):
-            variable_address = self.var_address.v[var_name][var_idx: var_idx + 1]
-        elif isinstance(var_idx, str):
-            variable_address = self.var_address.v[var_name][np.ix_(self.PARAM[var_idx].v.reshape((-1,)))]
-        elif isinstance(var_idx, slice):
-            variable_address = self.var_address.v[var_name][
-                var_idx_func.NUM_EQN(*self.obtain_eqn_args(var_idx_func, t, *xys))]
-        elif isinstance(var_idx, Expr):
-            args = self.obtain_eqn_args(var_idx_func, *xys)
-            variable_address = self.var_address.v[var_name][var_idx_func.NUM_EQN(*args).reshape(-1, )]
-        elif isinstance(var_idx, list):
-            variable_address = self.var_address.v[var_name][var_idx]
-        else:
-            raise TypeError(f"Unsupported variable index {var_idx} for equation {eqn_name}")
-
-        return equation_address, variable_address
-
-    def evalf(self, expr: Expr, t, *xys: Vars) -> np.ndarray:
-        eqn = Eqn('Solverz evalf temporal equation', expr)
-        args = self.obtain_eqn_args(eqn, t, *xys)
-        return eqn.NUM_EQN(*args)
+    def evalf(self, *args) -> np.ndarray:
+        pass
 
 
 class AE(Equations):
 
     def __init__(self,
                  eqn: Union[List[Eqn], Eqn],
                  name: str = None,
@@ -221,82 +233,52 @@
         super().__init__(eqn, name, matrix_container)
 
         # Check if some equation in self.eqn is Eqn.
         # If not, raise error
         if len(self.f_list) > 0:
             raise ValueError(f'Ode found. This object should be DAE!')
 
-    def assign_eqn_var_address(self, *xys: Vars):
+    def assign_eqn_var_address(self, y: Vars):
         """
         ASSIGN ADDRESSES TO EQUATIONS
         """
-        y = xys[0]
 
         temp = 0
         for eqn_name in self.EQNs.keys():
             geval = self.g(y, eqn_name)
             if isinstance(geval, Number):
                 eqn_size = 1
             else:
                 eqn_size = geval.shape[0]
             self.a.update(eqn_name, eqn_size)
             temp = temp + eqn_size
             self.esize[eqn_name] = eqn_size
         self.var_address = y.a
         self.vsize = y.total_size
 
-        # assign dim of derivatives, which is indispensable in Jac printer
-        gy = self.g_y(y)
-        for gy_tuple in gy:
-            eqn_name = gy_tuple[0]
-            var_name = gy_tuple[1]
-            eqndiff = gy_tuple[2]
-            value = gy_tuple[3]
-            if isinstance(value, (np.ndarray, csc_array)):
-                # We use coo_array here because by default when converting to CSR or CSC format,
-                # duplicate (i,j) entries will be summed together.
-                # This facilitates efficient construction of finite element matrices and the like.
-                if value.ndim == 2:  # matrix
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 2
-
-                elif value.ndim == 1 and value.shape[0] != 1:  # vector
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 1
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), value.shape[0])
-                elif value.ndim == 1 and value.shape[0] == 1:  # scalar in np.ndarray for example array([0.0])
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), self.a.size[eqn_name])
-                else:
-                    raise ValueError("Unknown derivative value dimension type!")
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'array'
-            elif isinstance(value, (Number, SymNumber)):
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'Number'
-            else:
-                raise ValueError(f"Unknown derivative data type {type(value)}!")
-
     def g(self, y: Vars, eqn: str = None) -> np.ndarray:
         """
 
         :param y:
         :param eqn:
         :return:
         """
         temp = []
         if not eqn:
             for eqn_name, eqn_ in self.EQNs.items():
-                args = self.obtain_eqn_args(eqn_, None, y)
+                args = self.obtain_eqn_args(eqn_, y)
                 g_eqny = self.eval(eqn_name, *args)
                 g_eqny = g_eqny.toarray() if isinstance(g_eqny, csc_array) else g_eqny
                 temp.append(g_eqny.reshape(-1, ))
             return np.hstack(temp)
         else:
-            args = self.obtain_eqn_args(self.EQNs[eqn], None, y)
+            args = self.obtain_eqn_args(self.EQNs[eqn], y)
             return self.eval(eqn, *args)
 
-    def g_y(self, y: Vars, eqn: List[str] = None, var: List[str] = None) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
+    def gy(self, y: Vars, eqn: List[str] = None, var: List[str] = None) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
         """
         generate Jacobian matrices of Eqn object with respect to var object
         :param y:
         :param eqn:
         :param var:
         :return: List[Tuple[Equation_name, var_name, np.ndarray]]
         """
@@ -308,19 +290,27 @@
         gy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
 
         for eqn_name in eqn:
             eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
             for var_name in var:
                 for key, value in eqn_diffs.items():
                     if var_name == value.diff_var_name:  # f is viewed as f[k]
-                        args = self.obtain_eqn_args(eqn_diffs[key], None, y)
+                        args = self.obtain_eqn_args(eqn_diffs[key], y)
                         temp = self.eval_diffs(eqn_name, key, *args)
                         gy = [*gy, (eqn_name, var_name, eqn_diffs[key], temp)]
         return gy
 
+    def Fy(self, y):
+        return self.gy(y)
+
+    def evalf(self, expr: Expr, y: Vars) -> np.ndarray:
+        eqn = Eqn('Solverz evalf temporal equation', expr)
+        args = self.obtain_eqn_args(eqn, y)
+        return eqn.NUM_EQN(*args)
+
     def __repr__(self):
         if not self.eqn_size:
             return f"Algebraic equation {self.name} with addresses uninitialized"
         else:
             return f"Algebraic equation {self.name} ({self.eqn_size}×{self.vsize})"
 
 
@@ -356,23 +346,28 @@
         self.algebra_num: int = 0  # number of algebraic variables
 
         # Check if some equation in self.eqn is Ode.
         # If not, raise error
         if len(self.f_list) == 0:
             raise ValueError(f'No ODE found. You should initialise AE instead!')
 
-    def assign_eqn_var_address(self, *xys: Vars):
+    def evalf(self, expr: Expr, t, y: Vars) -> np.ndarray:
+        eqn = Eqn('Solverz evalf temporary equation', expr)
+        args = self.obtain_eqn_args(eqn, y, t)
+        return eqn.NUM_EQN(*args)
+
+    def assign_eqn_var_address(self, y: Vars):
         """
         ASSIGN ADDRESSES TO EQUATIONS f and g
         """
 
         temp = 0
         for eqn_name in self.f_list:
-            feval = self.f(None, *xys, eqn=eqn_name)
-            lhs_eval = self.eval_lhs(None, *xys, eqn=eqn_name)
+            feval = self.f(None, y, eqn=eqn_name)
+            lhs_eval = self.eval_lhs(None, y, eqn=eqn_name)
             if isinstance(feval, Number):
                 rhs_size = 1
             else:
                 rhs_size = feval.shape[0]
             if isinstance(lhs_eval, Number):
                 lhs_size = 1
             else:
@@ -381,191 +376,151 @@
             self.a.update(eqn_name, eqn_size)
             temp = temp + eqn_size
             self.esize[eqn_name] = eqn_size
 
         self.state_num = temp
 
         for eqn_name in self.g_list:
-            geval = self.g(None, *xys, eqn=eqn_name)
+            geval = self.g(None, y, eqn=eqn_name)
             if np.max(np.abs(geval)) > 1e-5:
                 warnings.warn(
                     f'Inconsistent initial values for algebraic equation: {eqn_name}, with deviation {np.max(np.abs(geval))}!')
             if isinstance(geval, Number):
                 eqn_size = 1
             else:
                 eqn_size = geval.shape[0]
             self.a.update(eqn_name, eqn_size)
             temp = temp + eqn_size
             self.esize[eqn_name] = eqn_size
 
         self.algebra_num = temp - self.state_num
 
-        if len(xys) == 1:
-            self.var_address = xys[0].a
-            self.vsize = self.var_address.total_size
-        elif len(xys) == 2:
-            x = xys[0]
-            y = xys[1]
-            if x.total_size != self.state_num:
-                raise ValueError("Length of input state variable not compatible with state equations!")
-            if y.total_size != self.algebra_num:
-                raise ValueError("Length of input algebraic variable not compatible with algebraic equations!")
-            self.var_address = combine_Address(x.a, y.a)
-
-            for var_name in self.var_address.v.keys():
-                if var_name not in self.SYMBOLS:
-                    raise ValueError(f"DAE {self.name} has no variable {var_name}")
-
-            self.vsize: int = self.var_address.total_size
-        elif len(xys) > 2:
-            raise ValueError("Accept at most two positional arguments!")
-
-        # assign dim of derivatives, which is indispensable in Jac printer
-        fg_xy = self.f_xy(0, *xys)
-        if len(self.g_list) > 0:
-            fg_xy.extend(self.g_xy(0, *xys))
-        for gy_tuple in fg_xy:
-            eqn_name = gy_tuple[0]
-            var_name = gy_tuple[1]
-            eqndiff = gy_tuple[2]
-            value = gy_tuple[3]
-            if isinstance(value, (np.ndarray, csc_array)):
-                # We use coo_array here because by default when converting to CSR or CSC format,
-                # duplicate (i,j) entries will be summed together.
-                # This facilitates efficient construction of finite element matrices and the like.
-                if value.ndim == 2:  # matrix
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 2
-
-                elif value.ndim == 1 and value.shape[0] != 1:  # vector
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 1
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), value.shape[0])
-                elif value.ndim == 1 and value.shape[0] == 1:  # scalar in np.ndarray for example array([0.0])
-                    self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                    # self.jac_element_address.add((eqn_name, var_name, eqndiff), self.a.size[eqn_name])
-                else:
-                    raise ValueError("Unknown derivative value dimension type!")
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'array'
-            elif isinstance(value, (Number, SymNumber)):
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].dim = 0
-                self.EQNs[eqn_name].derivatives[eqndiff.diff_var.name].v_type = 'Number'
-            else:
-                raise ValueError(f"Unknown derivative data type {type(value)}!")
+        self.var_address = y.a
+        self.vsize = self.var_address.total_size
 
-    def F(self, t, *xys) -> np.ndarray:
+    def F(self, t, y) -> np.ndarray:
         """
         Return [f(t,x,y), g(t,x,y)]
         :param t: time
-        :param xys: Vars
+        :param y: Vars
         :return:
         """
         if len(self.g_list) > 0:
-            return np.concatenate([self.f(t, *xys), self.g(t, *xys)])
+            return np.concatenate([self.f(t, y), self.g(t, y)])
         else:
-            return self.f(t, *xys)
+            return self.f(t, y)
 
-    def f(self, t, *xys, eqn=None) -> np.ndarray:
+    def f(self, t, y, eqn=None) -> np.ndarray:
 
         temp = []
         if eqn:
             if eqn in self.f_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                args = self.obtain_eqn_args(self.EQNs[eqn], y, t)
                 temp.append(self.eval(eqn, *args).reshape(-1, ))
         else:
             for eqn in self.f_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                args = self.obtain_eqn_args(self.EQNs[eqn], y, t)
                 temp.append(self.eval(eqn, *args).reshape(-1, ))
 
         return np.hstack(temp)
 
-    def eval_lhs(self, t, *xys, eqn=None) -> np.ndarray:
+    def eval_lhs(self, t, y, eqn=None) -> np.ndarray:
 
         temp = []
         if eqn:
             if eqn in self.f_list:
-                lhs_eqn = Eqn('lhs_' + eqn, self.EQNs[eqn].diff_var)
-                args = self.obtain_eqn_args(lhs_eqn, t, *xys)
-                temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
+                ode = self.EQNs[eqn]
+                if isinstance(ode, Ode):
+                    lhs_eqn = Eqn('lhs_' + eqn, ode.diff_var)
+                    args = self.obtain_eqn_args(lhs_eqn, y, t)
+                    temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
+                else:
+                    raise TypeError(f"Equation {ode.name} in f_list is not Ode!")
         else:
             for eqn in self.f_list:
-                lhs_eqn = Eqn('lhs_' + eqn, self.EQNs[eqn].diff_var)
-                args = self.obtain_eqn_args(lhs_eqn, t, *xys)
-                temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
+                ode = self.EQNs[eqn]
+                if isinstance(ode, Ode):
+                    lhs_eqn = Eqn('lhs_' + eqn, ode.diff_var)
+                    args = self.obtain_eqn_args(lhs_eqn, y, t)
+                    temp.append(Array(lhs_eqn.NUM_EQN(*args), dim=1))
+                else:
+                    raise TypeError(f"Equation {ode.name} in f_list is not Ode!")
 
         return np.hstack(temp)
 
-    def g(self, t, *xys, eqn=None) -> np.ndarray:
+    def g(self, t, y, eqn=None) -> np.ndarray:
         """
 
         `xys` is either:
           - two arguments, e.g. state vars x, and numerical equation y
           - one argument, e.g. state vars y.
 
         """
 
         if len(self.g_list) == 0:
             raise ValueError(f'No AE found in {self.name}!')
 
         temp = []
         if eqn:
             if eqn in self.g_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                args = self.obtain_eqn_args(self.EQNs[eqn], y, t)
                 temp.append(self.eval(eqn, *args).reshape(-1, ))
         else:
             for eqn in self.g_list:
-                args = self.obtain_eqn_args(self.EQNs[eqn], t, *xys)
+                args = self.obtain_eqn_args(self.EQNs[eqn], y, t)
                 temp.append(self.eval(eqn, *args).reshape(-1, ))
 
         return np.hstack(temp)
 
-    def f_xy(self, t, *xys: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
+    def fy(self, t, y: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
         """
-        generate partial derivatives of f w.r.t. vars in xys
-        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
+        generate partial derivatives of f w.r.t. y
         """
 
-        fxy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
+        fy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
 
-        var: List[str] = list()
-        for xy in xys:
-            var = var + xy.var_list
+        var: List[str] = y.var_list
 
         for eqn_name in self.f_list:
             eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
             for var_name in var:
                 for key, value in eqn_diffs.items():
                     if var_name == value.diff_var_name:
-                        args = self.obtain_eqn_args(eqn_diffs[key], t, *xys)
+                        args = self.obtain_eqn_args(eqn_diffs[key], y, t)
                         temp = self.eval_diffs(eqn_name, key, *args)
-                        fxy = [*fxy, (eqn_name, var_name, eqn_diffs[key], temp)]
-        return fxy
+                        fy = [*fy, (eqn_name, var_name, eqn_diffs[key], temp)]
+        return fy
 
-    def g_xy(self, t, *xys: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
+    def gy(self, t, y: Vars) -> List[Tuple[str, str, EqnDiff, np.ndarray]]:
         """
-        generate partial derivatives of f w.r.t. vars in xys
-        :return: List[Tuple[Equation_name, var_name, np.ndarray]]
+        generate partial derivatives of g w.r.t. y
         """
 
         if len(self.g_list) == 0:
             raise ValueError(f'No AE found in {self.name}!')
 
-        gxy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
+        gy: List[Tuple[str, str, EqnDiff, np.ndarray]] = []
 
-        var: List[str] = list()
-        for xy in xys:
-            var = var + xy.var_list
+        var: List[str] = y.var_list
 
         for eqn_name in self.g_list:
             eqn_diffs: Dict[str, EqnDiff] = self.EQNs[eqn_name].derivatives
             for var_name in var:
                 for key, value in eqn_diffs.items():
                     if var_name == value.diff_var_name:
-                        args = self.obtain_eqn_args(eqn_diffs[key], t, *xys)
+                        args = self.obtain_eqn_args(eqn_diffs[key], y, t)
                         temp = self.eval_diffs(eqn_name, key, *args)
-                        gxy = [*gxy, (eqn_name, var_name, eqn_diffs[key], temp)]
-        return gxy
+                        gy = [*gy, (eqn_name, var_name, eqn_diffs[key], temp)]
+        return gy
+
+    def Fy(self, y):
+        fg_xy = self.fy(0, y)
+        if len(self.g_list) > 0:
+            fg_xy.extend(self.gy(0, y))
+        return fg_xy
 
     @property
     def M(self):
         """
         return the singular mass matrix, M, of dae
         Row of 1 in M corresponds to the differential equation
         Col of 1 in M corresponds to the state variable
@@ -609,15 +564,16 @@
                     else:
                         raise TypeError(f"Unsupported variable index {var_idx} in equation {eqn_name}")
                 else:
                     raise NotImplementedError
                 eqn_address_list = equation_address.tolist()
                 var_address_list = variable_address.tolist()
                 if len(eqn_address_list) != len(var_address_list):
-                    raise ValueError(f"Incompatible eqn address length {len(eqn_address_list)} and variable address length {len(var_address_list)}")
+                    raise ValueError(
+                        f"Incompatible eqn address length {len(eqn_address_list)} and variable address length {len(var_address_list)}")
                 row.extend(eqn_address_list)
                 col.extend(var_address_list)
             else:
                 raise ValueError("Equation in f_list is non-Ode.")
 
         if self.matrix_container == 'scipy':
             return csc_array((np.ones((self.state_num,)), (row, col)), (self.eqn_size, self.vsize))
```

### Comparing `solverz-0.0.1rc4/Solverz/equation/param.py` & `solverz-0.0.3rc2/Solverz/equation/param.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,26 @@
                  name: str,
                  value: Union[np.ndarray, list, Number] = None,
                  triggerable: bool = False,
                  trigger_var: Union[str, List[str]] = None,
                  trigger_fun: Callable = None,
                  dim: int = 1,
                  dtype=float,
-                 sparse=False):
+                 sparse=False,
+                 is_alias=False):
         self.name = name
         self.triggerable = triggerable
         self.trigger_var = [trigger_var] if isinstance(trigger_var, str) else trigger_var
         self.trigger_fun = trigger_fun
         self.dim = dim
         self.dtype = dtype
         self.sparse = sparse
         self.__v = None
         self.v = value
+        self.is_alias = is_alias  # if the Param is an alias var
 
     @property
     def v(self):
         return self.__v
 
     @v.setter
     def v(self, value):
@@ -53,25 +55,27 @@
                  name: str,
                  value: Union[np.ndarray, list, Number] = None,
                  triggerable: bool = False,
                  trigger_var: Union[str, List[str]] = None,
                  trigger_fun: Callable = None,
                  dim: int = 1,
                  dtype=float,
-                 sparse=False
+                 sparse=False,
+                 is_alias=False
                  ):
         ParamBase.__init__(self,
                            name,
                            value,
                            triggerable,
                            trigger_var,
                            trigger_fun,
                            dim,
                            dtype,
-                           sparse)
+                           sparse,
+                           is_alias)
         sSymBasic.__init__(self, name=name, Type='Para', value=value, dim=dim)
 
 
 class IdxParam(ParamBase, sSymBasic):
 
     def __init__(self,
                  name: str,
```

### Comparing `solverz-0.0.1rc4/Solverz/equation/test/test_DAE.py` & `solverz-0.0.3rc2/Solverz/equation/test/test_DAE.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/equation/test/test_Param.py` & `solverz-0.0.3rc2/Solverz/equation/test/test_Param.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/equation/test/test_eqn.py` & `solverz-0.0.3rc2/Solverz/equation/test/test_eqn.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/model/basic.py` & `solverz-0.0.3rc2/Solverz/model/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,13 @@
         array = np.zeros((a.total_size,))
         for var in a.object_list:
             array[a[var]] = self.var_dict[var].value
         y0 = Vars(a, array)
         if eqn_type == 'FDAE':
             for i in range(nstep):
                 eqs.update_param(y0.derive_alias(f'_tag_{i}'))
-        eqs.assign_eqn_var_address(y0)
+        eqs.FormJac(y0)
 
         if eqs.eqn_size != eqs.vsize:
             warnings.warn(f'Equation size {eqs.eqn_size} and variable size {eqs.vsize} not equal!')
 
         return eqs, y0
```

### Comparing `solverz-0.0.1rc4/Solverz/num_api/Array.py` & `solverz-0.0.3rc2/Solverz/num_api/Array.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/num_api/custom_function.py` & `solverz-0.0.3rc2/Solverz/num_api/custom_function.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/num_api/num_eqn.py` & `solverz-0.0.3rc2/Solverz/num_api/num_eqn.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/num_api/numjac.py` & `solverz-0.0.3rc2/Solverz/num_api/numjac.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/num_api/test/test_Array.py` & `solverz-0.0.3rc2/Solverz/num_api/test/test_Array.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/num_api/test/test_custom_func.py` & `solverz-0.0.3rc2/Solverz/num_api/test/test_custom_func.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/num_api/test/test_numjac.py` & `solverz-0.0.3rc2/Solverz/num_api/test/test_numjac.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/fdesolver.py` & `solverz-0.0.3rc2/Solverz/solvers/fdesolver.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/laesolver.py` & `solverz-0.0.3rc2/Solverz/solvers/laesolver.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/option.py` & `solverz-0.0.3rc2/Solverz/solvers/option.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/parser.py` & `solverz-0.0.3rc2/Solverz/solvers/parser.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/solution.py` & `solverz-0.0.3rc2/Solverz/solvers/solution.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/daesolver/beuler.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/beuler.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/daesolver/daeic.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/daeic.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/daesolver/rodas.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/rodas.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/daesolver/trapezoidal.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/trapezoidal.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/daesolver/utilities.py` & `solverz-0.0.3rc2/Solverz/solvers/daesolver/utilities.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/nlaesolver/cnr.py` & `solverz-0.0.3rc2/Solverz/solvers/nlaesolver/cnr.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/nlaesolver/lm.py` & `solverz-0.0.3rc2/Solverz/solvers/nlaesolver/lm.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/nlaesolver/nr.py` & `solverz-0.0.3rc2/Solverz/solvers/nlaesolver/nr.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/odesolver/ode45.py` & `solverz-0.0.3rc2/Solverz/solvers/odesolver/ode45.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/solvers/test/test_rodas_event.py` & `solverz-0.0.3rc2/Solverz/solvers/test/test_rodas_event.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/sym_algebra/functions.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,14 +178,15 @@
     with derivative
 
         .. math::
 
             \frac{\mathrm{d}}{\mathrm{d}x}{\operatorname{Abs}}(x)=\operatorname{Sign}(x).
 
     """
+
     def fdiff(self, argindex=1):
         """
         Get the first derivative of the argument to Abs().
         """
         if argindex == 1:
             return Sign(self.args[0])
         else:
@@ -198,28 +199,30 @@
         return self._numpycode(printer, **kwargs)
 
 
 class exp(UniVarFunc):
     r"""
     The exponential function, $e^x$.
     """
+
     def fdiff(self, argindex=1):
         return exp(*self.args)
 
     def _numpycode(self, printer, **kwargs):
         return r'exp(' + printer._print(self.args[0]) + r')'
 
     def _pythoncode(self, printer, **kwargs):
         return self._numpycode(printer, **kwargs)
 
 
 class sin(UniVarFunc):
     r"""
     The sine function.
     """
+
     def fdiff(self, argindex=1):
         if argindex == 1:
             return Symcos(self.args[0])
         else:
             raise ArgumentIndexError(self, argindex)
 
     def _numpycode(self, printer, **kwargs):
@@ -229,14 +232,15 @@
         return self._numpycode(printer, **kwargs)
 
 
 class cos(UniVarFunc):
     r"""
     The cosine function.
     """
+
     def fdiff(self, argindex=1):
         if argindex == 1:
             return -Symsin(self.args[0])
         else:
             raise ArgumentIndexError(self, argindex)
 
     def _numpycode(self, printer, **kwargs):
@@ -256,14 +260,15 @@
             \begin{cases}
             1&x> 0\\
             0& x==0\\
             -1&x< 0
             \end{cases}
 
     """
+
     def fdiff(self, argindex=1):
         # sign function should be treated as a constant.
         if argindex == 1:
             return 0
         raise ArgumentIndexError(self, argindex)
 
     def _numpycode(self, printer, **kwargs):
@@ -316,14 +321,15 @@
             \operatorname{Saturation}(v, v_\min, v_\max)=
             \begin{cases}
             v_\max&v> v_\max\\
             v& v_\min\leq v\leq v_\max\\
             v_\min&v< v_\min
             \end{cases}
     """
+
     @classmethod
     def eval(cls, v, vmin, vmax):
         return v * In(v, vmin, vmax) + vmax * GreaterThan(v, vmax) + vmin * LessThan(v, vmin)
 
 
 class AntiWindUp(MulVarFunc):
     r"""
@@ -374,14 +380,15 @@
         \begin{split}\min(x,y)=
         \begin{cases}
         x&x\leq y\\
         y& x>y
         \end{cases}\end{split}
 
     """
+
     @classmethod
     def eval(cls, x, y):
         return x * LessThan(x, y) + y * (1 - LessThan(x, y))
 
 
 class In(MulVarFunc):
     """
@@ -413,15 +420,15 @@
     """
 
     def _eval_derivative(self, s):
         return Integer(0)
 
     def _sympystr(self, printer, **kwargs):
         return '(({op1})>({op2}))'.format(op1=printer._print(self.args[0]),
-                                           op2=printer._print(self.args[1]))
+                                          op2=printer._print(self.args[1]))
 
     def _numpycode(self, printer, **kwargs):
         return r'SolGreaterThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
 
     def _lambdacode(self, printer, **kwargs):
         return self._numpycode(printer, **kwargs)
 
@@ -435,15 +442,15 @@
     """
 
     def _eval_derivative(self, s):
         return Integer(0)
 
     def _sympystr(self, printer, **kwargs):
         return '(({op1})<({op2}))'.format(op1=printer._print(self.args[0]),
-                                           op2=printer._print(self.args[1]))
+                                          op2=printer._print(self.args[1]))
 
     def _numpycode(self, printer, **kwargs):
         return r'SolLessThan(' + ', '.join([printer._print(arg, **kwargs) for arg in self.args]) + r')'
 
     def _lambdacode(self, printer, **kwargs):
         return self._numpycode(printer, **kwargs)
 
@@ -521,30 +528,14 @@
 
     @classmethod
     def eval(cls, *args):
         if len(args) > 3:
             raise TypeError(f"minmod takes at most 3 positional arguments but {len(args)} were given!")
 
 
-class zeros(Function):
-    # print zeros(6,6) as zeros((6,6))
-    # or zeros(6,) as zeros((6,))
-    def _numpycode(self, printer, **kwargs):
-        if len(self.args) == 2:
-            temp1 = printer._print(self.args[0])
-            temp2 = printer._print(self.args[1])
-            return r'zeros((' + temp1 + ', ' + temp2 + r'))'
-        elif len(self.args) == 1:
-            temp = printer._print(self.args[0])
-            return r'zeros((' + temp + ', ' + r'))'
-
-    def _pythoncode(self, printer, **kwargs):
-        return self._numpycode(printer, **kwargs)
-
-
 class CSC_array(Function):
 
     @classmethod
     def eval(cls, *args):
         if len(args) != 1:
             raise TypeError(f"CSC_array takes 1 positional arguments but {len(args)} were given!")
```

### Comparing `solverz-0.0.1rc4/Solverz/sym_algebra/matrix_calculus.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/matrix_calculus.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/sym_algebra/symbols.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/symbols.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/sym_algebra/transform.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/transform.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/sym_algebra/test/test_finite_difference.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/test/test_finite_difference.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/sym_algebra/test/test_matrix_calculus.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/test/test_matrix_calculus.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/sym_algebra/test/test_num_alg.py` & `solverz-0.0.3rc2/Solverz/sym_algebra/test/test_num_alg.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/utilities/address.py` & `solverz-0.0.3rc2/Solverz/utilities/address.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/utilities/io.py` & `solverz-0.0.3rc2/Solverz/utilities/io.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/utilities/test/test_address.py` & `solverz-0.0.3rc2/Solverz/utilities/test/test_address.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/variable/ssymbol.py` & `solverz-0.0.3rc2/Solverz/variable/ssymbol.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/variable/variables.py` & `solverz-0.0.3rc2/Solverz/variable/variables.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/Solverz/variable/test/test_variable.py` & `solverz-0.0.3rc2/Solverz/variable/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/Makefile` & `solverz-0.0.3rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/make.bat` & `solverz-0.0.3rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/ext/convert-svg-to-pdf.py` & `solverz-0.0.3rc2/docs/ext/convert-svg-to-pdf.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/ext/docscrape.py` & `solverz-0.0.3rc2/docs/ext/docscrape.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/ext/docscrape_sphinx.py` & `solverz-0.0.3rc2/docs/ext/docscrape_sphinx.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/ext/numpydoc.py` & `solverz-0.0.3rc2/docs/ext/numpydoc.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/advanced.md` & `solverz-0.0.3rc2/docs/src/advanced.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/conf.py` & `solverz-0.0.3rc2/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/gettingstart.md` & `solverz-0.0.3rc2/docs/src/gettingstart.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/index.rst` & `solverz-0.0.3rc2/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/intro.md` & `solverz-0.0.3rc2/docs/src/intro.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/_static/custom.css` & `solverz-0.0.3rc2/docs/src/_static/custom.css`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/_static/sympylogo.png` & `solverz-0.0.3rc2/docs/src/_static/sympylogo.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/_static/sympylogo_big.png` & `solverz-0.0.3rc2/docs/src/_static/sympylogo_big.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/pics/Hierarchy_of_equations.png` & `solverz-0.0.3rc2/docs/src/pics/Hierarchy_of_equations.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/pics/difference_stencil.png` & `solverz-0.0.3rc2/docs/src/pics/difference_stencil.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/pics/res.png` & `solverz-0.0.3rc2/res.png`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/docs/src/reference/index.rst` & `solverz-0.0.3rc2/docs/src/reference/index.rst`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/instances/dae_test.xlsx` & `solverz-0.0.3rc2/tests/dae_test.xlsx`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/tests/test_dae.py` & `solverz-0.0.3rc2/tests/test_dae.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 f = Ode(name='f', f=-x ** 3 + 0.5 * y ** 2, diff_var=x)
 g = Eqn(name='g', eqn=x ** 2 + y ** 2 - 2)
 dae = DAE([f, g])
 
 z = as_Vars([x, y])
 ndae = made_numerical(dae, z)
 
-df = pd.read_excel('instances/dae_test.xlsx',
+df = pd.read_excel('tests/dae_test.xlsx',
                    sheet_name=None,
                    engine='openpyxl'
                    )
 
 sol_rodas = Rodas(ndae,
                   [0, 20],
                   z,
```

### Comparing `solverz-0.0.1rc4/LICENSE` & `solverz-0.0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/README.md` & `solverz-0.0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `solverz-0.0.1rc4/pyproject.toml` & `solverz-0.0.3rc2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=64", "setuptools_scm>=8"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
+version_file = "Solverz/_version.py"
 
 [project]
 name = "Solverz"
-version = "0.0.1rc4"
+dynamic = ["version"]
 dependencies = [
     "sympy>=1.11.1",
     "numba == 0.58.1",
     "numpy>=1.26.3",
     "scipy>=1.12.0",
     "dill >= 0.3.7",
     "pandas>=1.4.2",
     "openpyxl>=3.0.10",
     "matplotlib>=3.5.2",
     "tqdm>=4.64.1",
     "pytest>=7.2.2",
+    "pytest-datadir>=1.5.0",
     "networkx >= 3.1"
 ]
 authors = [
     { name = "Ruizhi Yu", email = "rz.yu@foxmail.com" },
 ]
 description = "A simulation modelling language"
 readme = "README.md"
```

### Comparing `solverz-0.0.1rc4/PKG-INFO` & `solverz-0.0.3rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: Solverz
-Version: 0.0.1rc4
+Version: 0.0.3rc2
 Summary: A simulation modelling language
+Author-email: Ruizhi Yu <rz.yu@foxmail.com>
 Project-URL: Homepage, https://github.com/smallbunnies/Solverz
 Project-URL: Issues, https://github.com/smallbunnies/Solverz/issues
-Author-email: Ruizhi Yu <rz.yu@foxmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
-Requires-Dist: dill>=0.3.7
-Requires-Dist: matplotlib>=3.5.2
-Requires-Dist: networkx>=3.1
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sympy>=1.11.1
 Requires-Dist: numba==0.58.1
 Requires-Dist: numpy>=1.26.3
-Requires-Dist: openpyxl>=3.0.10
-Requires-Dist: pandas>=1.4.2
-Requires-Dist: pytest>=7.2.2
 Requires-Dist: scipy>=1.12.0
-Requires-Dist: sympy>=1.11.1
+Requires-Dist: dill>=0.3.7
+Requires-Dist: pandas>=1.4.2
+Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: matplotlib>=3.5.2
 Requires-Dist: tqdm>=4.64.1
-Description-Content-Type: text/markdown
+Requires-Dist: pytest>=7.2.2
+Requires-Dist: pytest-datadir>=1.5.0
+Requires-Dist: networkx>=3.1
 
 # Overview
 Solverz is an open-source python-based simulation modelling language that provides symbolic interfaces for you to model your equations and can then generate functions or numba-jitted python modules for numerical solutions. 
 
 Solverz supports three types of abstract equation types, that are
 
 - Algebraic Equations (AEs) $0=F(y,p)$
```

