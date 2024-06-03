# Comparing `tmp/cetpy-0.1.0b5.tar.gz` & `tmp/cetpy-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cetpy-0.1.0b5.tar", last modified: Mon Nov 20 12:17:38 2023, max compression
+gzip compressed data, was "cetpy-0.1.0b6.tar", last modified: Mon Jun  3 14:01:04 2024, max compression
```

## Comparing `cetpy-0.1.0b5.tar` & `cetpy-0.1.0b6.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.509264 cetpy-0.1.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-11-20 12:17:38.509264 cetpy-0.1.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.501264 cetpy-0.1.0b5/cetpy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.501264 cetpy-0.1.0b5/cetpy/CaseTools/
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/CaseTools/FilterFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14701 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/CaseTools/_CaseGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/CaseTools/_CaseRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)    70206 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/CaseTools/_DataSet.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/CaseTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.501264 cetpy-0.1.0b5/cetpy/Configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    13851 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Configuration/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Configuration/_ModuleManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Configuration/_Session.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Configuration/default_config_parameters.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Configuration/default_session_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.501264 cetpy-0.1.0b5/cetpy/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.501264 cetpy-0.1.0b5/cetpy/Modules/Fluid/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Fluid/_FluidCoolProp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Fluid/_FluidSkeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Fluid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.505264 cetpy-0.1.0b5/cetpy/Modules/FluidBlock/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_CompressibleFluidBlock.py
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_FluidBlock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_FluidPort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_GenericFluidBlock.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/FluidBlock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.505264 cetpy-0.1.0b5/cetpy/Modules/Material/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Material/_MaterialGiven.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Material/_MaterialSkeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Material/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.505264 cetpy-0.1.0b5/cetpy/Modules/Report/
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Report/_Report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Report/_ReportPort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Report/_ReportSolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.505264 cetpy-0.1.0b5/cetpy/Modules/Solver/
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Solver/_ContinuousFlowSolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Solver/_Solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Solver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.505264 cetpy-0.1.0b5/cetpy/Modules/SysML/
--rw-r--r--   0 runner    (1001) docker     (127)    16288 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/_Block.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/_ContinuousPort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/_FlowProperty.py
--rw-r--r--   0 runner    (1001) docker     (127)    10884 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/_PartProperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/_Port.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/_ProxyProperty.py
--rw-r--r--   0 runner    (1001) docker     (127)    36102 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/_ValueProperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/SysML/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.505264 cetpy-0.1.0b5/cetpy/Modules/Utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Utilities/InputValidation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Utilities/Labelling.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/Modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.509264 cetpy-0.1.0b5/cetpy/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.509264 cetpy-0.1.0b5/cetpy/tests/TestModules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.509264 cetpy-0.1.0b5/cetpy/tests/TestModules/TestSysML/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/tests/TestModules/TestSysML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/tests/TestModules/TestSysML/test_Block.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/tests/TestModules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/cetpy/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:17:38.501264 cetpy-0.1.0b5/cetpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-11-20 12:17:38.000000 cetpy-0.1.0b5/cetpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-11-20 12:17:38.000000 cetpy-0.1.0b5/cetpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 12:17:38.000000 cetpy-0.1.0b5/cetpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-20 12:17:38.000000 cetpy-0.1.0b5/cetpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-20 12:17:38.000000 cetpy-0.1.0b5/cetpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-20 12:17:38.509264 cetpy-0.1.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-11-20 12:17:14.000000 cetpy-0.1.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.389395 cetpy-0.1.0b6/cetpy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.389395 cetpy-0.1.0b6/cetpy/CaseTools/
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/CaseTools/FilterFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/CaseTools/RegressionDataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/CaseTools/_CaseGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/CaseTools/_CaseRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56607 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/CaseTools/_DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/CaseTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.389395 cetpy-0.1.0b6/cetpy/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Configuration/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Configuration/_ModuleManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Configuration/_Session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Configuration/default_config_parameters.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Configuration/default_session_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.389395 cetpy-0.1.0b6/cetpy/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.393395 cetpy-0.1.0b6/cetpy/Modules/Fluid/
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Fluid/_FluidCoolProp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Fluid/_FluidSkeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Fluid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.393395 cetpy-0.1.0b6/cetpy/Modules/FluidBlock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_CompressibleFluidBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_FluidBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_FluidPort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_GenericFluidBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/FluidBlock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.393395 cetpy-0.1.0b6/cetpy/Modules/Material/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Material/_MaterialGiven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Material/_MaterialSkeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Material/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.393395 cetpy-0.1.0b6/cetpy/Modules/Report/
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Report/_Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Report/_ReportPort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Report/_ReportSolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.393395 cetpy-0.1.0b6/cetpy/Modules/Solver/
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Solver/_ContinuousFlowSolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Solver/_Solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Solver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/cetpy/Modules/SysML/
+-rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/_Block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/_ContinuousPort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/_FlowProperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/_PartProperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/_Port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/_ProxyProperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36102 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/_ValueProperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/SysML/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/cetpy/Modules/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Utilities/InputValidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Utilities/Labelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/Modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/cetpy/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/cetpy/tests/TestModules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/cetpy/tests/TestModules/TestSysML/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/tests/TestModules/TestSysML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/tests/TestModules/TestSysML/test_Block.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/tests/TestModules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/cetpy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/cetpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-06-03 14:01:04.000000 cetpy-0.1.0b6/cetpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-06-03 14:01:04.000000 cetpy-0.1.0b6/cetpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:01:04.000000 cetpy-0.1.0b6/cetpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-03 14:01:04.000000 cetpy-0.1.0b6/cetpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 14:01:04.000000 cetpy-0.1.0b6/cetpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-03 14:01:04.397395 cetpy-0.1.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-06-03 14:01:00.000000 cetpy-0.1.0b6/setup.py
```

### Comparing `cetpy-0.1.0b5/LICENSE.txt` & `cetpy-0.1.0b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/PKG-INFO` & `cetpy-0.1.0b6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cetpy
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Congruent Engineering Toolbox
 Home-page: https://github.com/CongruentEngineeringToolbox/cetpy
 Author: CET developers
 Keywords: engineering,system engineering,congruent engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,17 +16,14 @@
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: CoolProp
 Requires-Dist: tomli
-Requires-Dist: keras
-Requires-Dist: keras-tuner
-Requires-Dist: tensorflow
 Requires-Dist: tabulate
 Requires-Dist: smt
 Requires-Dist: pytest
 Requires-Dist: matplotlib
 Requires-Dist: statsmodels
 Requires-Dist: scikit-learn
```

### Comparing `cetpy-0.1.0b5/cetpy/CaseTools/FilterFunctions.py` & `cetpy-0.1.0b6/cetpy/CaseTools/FilterFunctions.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/CaseTools/_CaseGenerator.py` & `cetpy-0.1.0b6/cetpy/CaseTools/_CaseGenerator.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/CaseTools/_CaseRunner.py` & `cetpy-0.1.0b6/cetpy/CaseTools/_CaseRunner.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/CaseTools/_DataSet.py` & `cetpy-0.1.0b6/cetpy/CaseTools/_DataSet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 """
 DataSet
 =======
 
-This file defines a wrapper around a pandas DataFrame to add further
-convenient analysis using the knowledge of the cetpy Iterator of its system.
+This file defines a wrapper around a pandas DataFrame to add further convenient analysis using the knowledge of the
+cetpy Iterator of its system.
 """
 from __future__ import annotations
 
 from os.path import isdir, dirname
-from typing import List, Dict, Iterable, Tuple, Sequence, Any
+from typing import List, Dict, Iterable, Tuple, Sequence
 import numpy as np
 import pandas as pd
 import pickle
 from copy import deepcopy
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 import statsmodels.api as sm
-from statsmodels.regression.linear_model import OLS, RegressionResults
-from sklearn.ensemble import RandomForestRegressor
-from sklearn.neural_network import MLPRegressor
-import keras
-from keras import backend as K
-import keras_tuner
 
 from cetpy.Modules.SysML import Block, ValueProperty, value_property
 
-from cetpy.CaseTools.FilterFunctions import apply_filter, \
-    drop_no_variance_columns, apply_one_hot_encoding
-from cetpy.Modules.Utilities.Labelling import round_sig_figs, \
-    floor_sig_figs, ceil_sig_figs, unit_2_latex, name_2_unit, name_2_axis_label
+from cetpy.CaseTools.FilterFunctions import apply_filter, drop_no_variance_columns, apply_one_hot_encoding
+from cetpy.Modules.Utilities.Labelling import round_sig_figs, floor_sig_figs, ceil_sig_figs, unit_2_latex, \
+    name_2_unit, name_2_axis_label
 
 
-binary_color_maps = ['Greys', 'Purples', 'Blues', 'Greens', 'Oranges', 'Reds',
-                     'YlOrBr', 'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu',
-                     'GnBu', 'PuBu', 'YlGnBu', 'PuBuGn', 'BuGn', 'YlGn'] * 3
+binary_color_maps = ['Greys', 'Purples', 'Blues', 'Greens', 'Oranges', 'Reds', 'YlOrBr', 'YlOrRd', 'OrRd', 'PuRd',
+                     'RdPu', 'BuPu', 'GnBu', 'PuBu', 'YlGnBu', 'PuBuGn', 'BuGn', 'YlGn'] * 3
 
 
 def get_numerical_correlation_threshold(threshold: str | float) -> float:
-    """Return float threshold for correlation label. Return float if a float
-    is passed."""
+    """Return float threshold for correlation label. Return float if a float is passed."""
     if isinstance(threshold, float):
         return threshold
     else:
         match threshold:
             case 'perfect':
                 return 0.98
             case 'high':
@@ -53,36 +44,30 @@
             case 'low':
                 return 0.02
             case _:
                 return 0.
 
 
 class DataSet(Block):
-    """Congruent Engineering Toolbox DataSet, a wrapper around a pandas
-    DataFrame with additional analysis functionality."""
+    """Congruent Engineering Toolbox DataSet, a wrapper around a pandas DataFrame with additional analysis
+    functionality."""
 
     drop_errors = ValueProperty(permissible_types_list=bool)
     drop_no_variance = ValueProperty(permissible_types_list=bool)
     one_hot_encoding = ValueProperty(permissible_types_list=bool)
-    filter_list = ValueProperty(
-        permissible_types_list=[str, list, type(None)])
-    error_filter = ValueProperty(
-        permissible_types_list=[str, list, type(None)])
-    input_df = ValueProperty(
-        permissible_types_list=[pd.DataFrame, type(None)])
-    units = ValueProperty(
-        permissible_types_list=[dict, type(None)])
-    axis_labels = ValueProperty(
-        permissible_types_list=[dict, type(None)])
-    last_input_column = ValueProperty(
-        permissible_types_list=[str, type(None)])
+    filter_list = ValueProperty(permissible_types_list=[str, list, type(None)])
+    error_filter = ValueProperty(permissible_types_list=[str, list, type(None)])
+    input_df = ValueProperty(permissible_types_list=[pd.DataFrame, type(None)])
+    units = ValueProperty(permissible_types_list=[dict, type(None)])
+    axis_labels = ValueProperty(permissible_types_list=[dict, type(None)])
+    last_input_column = ValueProperty(permissible_types_list=[str, type(None)])
 
     __init_parameters__ = Block.__init_parameters__.copy() + [
-        'drop_errors', 'drop_no_variance', 'one_hot_encoding', 'filter_list',
-        'error_filter', 'input_df', 'units', 'axis_labels', 'last_input_column'
+        'drop_errors', 'drop_no_variance', 'one_hot_encoding', 'filter_list', 'error_filter', 'input_df', 'units',
+        'axis_labels', 'last_input_column'
     ]
 
     _reset_dict = Block._reset_dict.copy()
     _reset_dict.update({'_output_df': None})
 
     def __init__(self,
                  raw_df: pd.DataFrame,
@@ -109,37 +94,32 @@
             axis_labels=axis_labels,
             last_input_column=last_input_column,
             **kwargs)
         self.raw_df = raw_df
         if units is None or axis_labels is None:
             names = [s.split('.')[-1] for s in raw_df.columns]
             if units is None:
-                self.units = {col: name_2_unit(name)
-                              for col, name in zip(raw_df.columns, names)}
+                self.units = {col: name_2_unit(name) for col, name in zip(raw_df.columns, names)}
             if axis_labels is None:
-                self.axis_labels = {
-                    col: name_2_axis_label(name)
-                    for col, name in zip(raw_df.columns, names)}
+                self.axis_labels = {col: name_2_axis_label(name) for col, name in zip(raw_df.columns, names)}
 
     @value_property(input_permissible=True,
                     permissible_types_list=[str, type(None)])
     def last_input_column(self) -> str:
         """Return key of last input column.
 
-        Can be supplied manually, if None is provided, the column is
-        evaluated automatically based on the structure of the cetpy Case
-        Runner.
+        Can be supplied manually, if None is provided, the column is evaluated automatically based on the structure
+        of the cetpy CaseRunner.
         """
         df = self.raw_df
         try:
             idx_solved = df.columns.get_loc('solved') - 1
         except AttributeError:
-            raise ValueError('The last input column of the dataframe could '
-                             'not be evaluated automatically. Please set the '
-                             'column manually with DataSet.last_input_column')
+            raise ValueError('The last input column of the dataframe could not be evaluated automatically. Please set '
+                             'the column manually with DataSet.last_input_column')
         return df.columns[idx_solved]
 
     @property
     def __idx_last_input_column_raw__(self) -> int:
         """Return index of last input column of raw dataframe."""
         return self.raw_df.columns.get_loc(self.last_input_column)
 
@@ -149,18 +129,17 @@
         return self.df.columns.get_loc(self.last_input_column)
 
     # region DataFrames
     @value_property(permissible_types_list=pd.DataFrame)
     def raw_df(self) -> pd.DataFrame:
         """Unprocessed dataset as a pandas Dataframe.
 
-        The dataframe should first have the input columns, then the output
-        columns. If the dataframe still contains the original solved or
-        error related columns, the separation can be detected automatically.
-        Otherwise, a last_input_column value will need to be specified.
+        The dataframe should first have the input columns, then the output columns. If the dataframe still contains
+        the original solved or error related columns, the separation can be detected automatically. Otherwise,
+        a last_input_column value will need to be specified.
 
         See Also
         --------
         DataSet.df
         """
         return self._df_raw.copy()  # Protect original
 
@@ -168,16 +147,15 @@
     def raw_df(self, val: pd.DataFrame) -> None:
         self._df_raw = val
 
     @property
     def df_errors(self) -> pd.DataFrame:
         """Dataframe of only cases with errors.
 
-        Includes both detected errors and those selected by the custom error
-        filter.
+        Includes both detected errors and those selected by the custom error filter.
 
         See Also
         --------
         DataSet.df_no_errors
         DataSet.df
         """
         df = self.raw_df
@@ -198,24 +176,22 @@
 
         See Also
         --------
         DataSet.df_errors
         DataSet.df
         """
         return self.raw_df.drop(index=self.df_errors.index,
-                                columns=['errored', 'error_class',
-                                         'error_message', 'error_location'],
+                                columns=['errored', 'error_class', 'error_message', 'error_location'],
                                 errors='ignore')
 
     @property
     def df(self) -> pd.DataFrame:
         """DataFrame with all enabled processing functions applied.
 
-        Processed dataframe is stored for performance. This can be reset
-        with the DataSet.reset() function.
+        Processed dataframe is stored for performance. This can be reset with the DataSet.reset() function.
 
         Filters are applied in the following order:
             1. Drop Errors (including custom error filter)
             2. Filter List
             3. Drop No Variance
 
         See Also
@@ -237,26 +213,24 @@
             if self.drop_no_variance:
                 df = drop_no_variance_columns(df)
 
             # Dropping columns with no variance can drop the detected
             # transition input column. Verify and re-detect if necessary.
             if self.last_input_column not in df.columns:
                 self._output_last_input_column = [
-                    col for col in df.columns
-                    if col in list(self.raw_df.keys())][-1]
+                    col for col in df.columns if col in list(self.raw_df.keys())][-1]
 
             if self.one_hot_encoding:
                 # One-Hot Encoding appends the newly created columns at the
                 # end. The application function splits the dataframe into
                 # inputs and outputs and applies the encoding separately in
                 # order to maintain separation. Given new columns are
                 # appended, the last column of the inputs needs to be
                 # reevaluated.
-                df_input = pd.get_dummies(
-                    df.loc[:, :self.last_input_column])
+                df_input = pd.get_dummies(df.loc[:, :self.last_input_column])
                 self._output_last_input_column = df_input.columns[-1]
                 df = apply_one_hot_encoding(df, df_input.columns)
 
             self._output_df = df
         return self._output_df
 
     # region Keys
@@ -334,212 +308,178 @@
 
         See Also
         --------
         DataSet.last_input_column
         DataSet.output_keys
         DataSet.input_keys_raw
         """
-        return list(self.raw_df.select_dtypes(
-            exclude=['bool_', 'number']).columns)
+        return list(self.raw_df.select_dtypes(exclude=['bool_', 'number']).columns)
     # endregion
 
     def get_df_custom_level(self, idx_start_filter: int = None,
                             idx_end_filter: int = None,
                             drop_errors: bool = None,
                             drop_no_variance: bool = None) -> pd.DataFrame:
         """Return dataframe with custom processing level.
 
         Parameters
         ----------
         idx_start_filter: optional, default = None
-            Start index of the filter list. If this index is higher than the
-            length of the filter list, a copy of the original dataframe is
-            returned.
+            Start index of the filter list. If this index is higher than the length of the filter list, a copy of the
+            original dataframe is returned.
 
         idx_end_filter: optional, default = None
-            End index of the filter list. If this index is higher than the
-            length of the filter list, the list is returned until the end.
-            if this index is smaller than the start index, just the
-            filter at the start index is applied.
+            End index of the filter list. If this index is higher than the length of the filter list, the list is
+            returned until the end. if this index is smaller than the start index, just the filter at the start index is
+            applied.
 
         drop_errors: optional, default = None
-            Bool flag whether to drop errors from the dataframe. Also drops
-            error related columns. If set to None, the DataSet instance
-            default value is used.
+            Bool flag whether to drop errors from the dataframe. Also drops error related columns. If set to None,
+            the DataSet instance default value is used.
 
         drop_no_variance: optional, default = None
-            Bool flag whether to drop columns with no variance from the
-            dataframe. If set to None, the DataSet instance default value is
-            used.
+            Bool flag whether to drop columns with no variance from the dataframe. If set to None, the DataSet
+            instance default value is used.
 
         Returns
         -------
         pd.DataFrame
-            Processed dataframe from the raw dataframe with the chosen
-            filters applied.
+            Processed dataframe from the raw dataframe with the chosen filters applied.
         """
         if drop_errors or (drop_errors is None and self.drop_errors):
             df = self.df_no_errors
         else:
             df = self.raw_df
 
         # Slice Filter
         filter_list = self.filter_list
-        if (idx_start_filter is None and idx_end_filter is None
-                or isinstance(filter_list, str)):
+        if idx_start_filter is None and idx_end_filter is None or isinstance(filter_list, str):
             pass
         else:
             filter_list = filter_list[idx_start_filter: idx_end_filter]
 
         df = apply_filter(df, filter_list, join_and=True)
 
-        if drop_no_variance or (
-                drop_no_variance is None and self.drop_no_variance):
+        if drop_no_variance or (drop_no_variance is None and self.drop_no_variance):
             df = drop_no_variance_columns(df)
 
         if self.one_hot_encoding:
             df = apply_one_hot_encoding(df, self.input_keys_raw)
         return df
 
-    def get_dfs_filter_levels(self, stacked: bool = True
-                              ) -> Dict[str, pd.DataFrame]:
-        """Return list of dataframes corresponding to the raw, no errors (if
-        DataSet.drop_errors is True), and subsequently each cumulative filter
-        level.
+    def get_dfs_filter_levels(self, stacked: bool = True) -> Dict[str, pd.DataFrame]:
+        """Return list of dataframes corresponding to the raw, no errors (if DataSet.drop_errors is True),
+        and subsequently each cumulative filter level.
 
         Useful to analyse scope, validity, and detail changes with filtering.
 
         Parameters
         ----------
         stacked: optional, default = True
-            Bool flag whether to stack filters. E.g. show the incremental
-            improvement of the full filter set (True) or the impact of the
-            individual filters on the original dataset (False).
+            Bool flag whether to stack filters. E.g. show the incremental improvement of the full filter set (True)
+            or the impact of the individual filters on the original dataset (False).
         """
         # Go through custom level function, to match no variance and
         # one-hot-encoding post-processing.
         dfs = {'raw': self.get_df_custom_level(None, 0, False, None)}
         if self.drop_errors:
             dfs['no_errors'] = self.get_df_custom_level(None, 0, True, None)
         idx_start = None
         for i in range(len(self.filter_list)):
-            dfs[self.filter_list[i]] = self.get_df_custom_level(
-                idx_start, i + 1, None, None)
+            dfs[self.filter_list[i]] = self.get_df_custom_level(idx_start, i + 1, None, None)
             if not stacked:
                 idx_start = i + 1
         return dfs
 
     def get_split_dataset(self, split_key: str,
                           split_set: None | int | np.ndarray = None,
                           maintain_raw: bool = None
                           ) -> List[DataSet]:
         """Return list of datasets split along a specified key.
 
         Parameters
         ----------
         split_key
-            Dataframe column key to split the dataset. If this is a
-            categorical key and one-hot-encoding is enabled, both pre- and
-            post-encoding keys are supported.
+            Dataframe column key to split the dataset. If this is a categorical key and one-hot-encoding is enabled,
+            both pre- and post-encoding keys are supported.
 
         split_set: optional, default = None
-            A definition of the set to be created. If the split_key is a
-            categorical value. This property is ignored, and a subset for
-            each categorical value is created. If the split_key is a
-            continuous property, the split_set can either be an integer,
-            in which case the integer describes the amount of sets to split
-            the continuous variable into. Alternatively the set can be a 1d
-            numpy array where a set is created from each value to the next of
-            the split_key data.
+            A definition of the set to be created. If the split_key is a categorical value. This property is ignored,
+            and a subset for each categorical value is created. If the split_key is a continuous property,
+            the split_set can either be an integer, in which case the integer describes the amount of sets to split
+            the continuous variable into. Alternatively the set can be a 1d numpy array where a set is created from
+            each value to the next of the split_key data.
 
         maintain_raw: optional, default = None
-            Bool flag whether the new dataset should maintain the full depth to
-            the raw dataframe. This can sometimes be easier for categorical
-            filtering with one-hot encoding. Otherwise, it is recommendable
-            to drop the already filtered rows to improve performance. When
-            set to None, attempts False, if the split_key is categorical
-            then True.
+            Bool flag whether the new dataset should maintain the full depth to the raw dataframe. This can sometimes
+            be easier for categorical filtering with one-hot encoding. Otherwise, it is recommendable to drop the
+            already filtered rows to improve performance. When set to None, attempts False, if the split_key is
+            categorical then True.
 
         Notes
         -----
         if the split_set of a continuous variable is defined as an integer.
-        The created sets are automatically rounded to sensible s
+        The created sets are automatically rounded to sensible significant figure.
         """
         if maintain_raw is None:
             maintain_raw = split_key not in self.df.columns
         if maintain_raw:
             if split_key not in self.raw_df.columns:
-                raise KeyError("Split key not in raw dataframe, consider "
-                               "setting maintain_raw to False or applying "
+                raise KeyError("Split key not in raw dataframe, consider setting maintain_raw to False or applying "
                                "one-hot-encoding on the raw dataset.")
             split_data = self.raw_df.loc[:, split_key]
         else:
             if split_key not in self.df.columns:
-                raise KeyError("Split key not in processed dataframe, "
-                               "consider setting maintain_raw to True or "
-                               "adjusting the categorical split key to a "
-                               "specific post one-hot-encoding category.")
+                raise KeyError("Split key not in processed dataframe, consider setting maintain_raw to True or "
+                               "adjusting the categorical split key to a specific post one-hot-encoding category.")
             split_data = self.df.loc[:, split_key]
 
         datasets = []
-        if (split_data.nunique() in [1, 2]
-                and not isinstance(split_data.iloc[0], str)):
+        if split_data.nunique() in [1, 2] and not isinstance(split_data.iloc[0], str):
             # Binary Data
-            ds_0 = self.subset(split_key + ' == '
-                               + str(np.unique(split_data)[0]),
-                               maintain_raw=maintain_raw)
-            ds_1 = self.subset(split_key + ' != '
-                               + str(np.unique(split_data)[0]),
-                               maintain_raw=maintain_raw)
+            ds_0 = self.subset(split_key + ' == ' + str(np.unique(split_data)[0]), maintain_raw=maintain_raw)
+            ds_1 = self.subset(split_key + ' != ' + str(np.unique(split_data)[0]), maintain_raw=maintain_raw)
             datasets = [ds_0, ds_1]
         elif split_key in self.keys_categorical:
             # Categorical Data
             for val in np.unique(split_data):
-                datasets += [self.subset(split_key + ' == "' + val + '"',
-                                         maintain_raw=maintain_raw)]
+                datasets += [self.subset(split_key + ' == "' + val + '"', maintain_raw=maintain_raw)]
         else:
             # Numerical Data
             limit_data = self.df.loc[:, split_key]
             if isinstance(split_set, int):
                 sig_figs = int(np.ceil(np.log10(split_set)) + 1)
                 split_set_new = np.linspace(
                     floor_sig_figs(limit_data.min(), sig_figs),
                     ceil_sig_figs(limit_data.max(), sig_figs), split_set + 1)
                 # Round to sig fig in the center as well.
                 for i in range(1, len(split_set_new) - 1):
-                    split_set_new[i] = round_sig_figs(
-                        split_set_new[i], sig_figs)
+                    split_set_new[i] = round_sig_figs(split_set_new[i], sig_figs)
                 split_set = split_set_new
             for i in range(len(split_set) - 1):
                 datasets += [self.subset(
-                    str(split_set[i]) + " <= " + split_key
-                    + " <= " + str(split_set[i + 1]),
-                    maintain_raw=maintain_raw)]
+                    str(split_set[i]) + " <= " + split_key + " <= " + str(split_set[i + 1]), maintain_raw=maintain_raw)]
 
         return datasets
 
-    def subset(self, new_filter: None | str | List[str] = None,
-               maintain_raw: bool = False) -> DataSet:
-        """Return a further dataset utilising the current processed
-        dataframe as its base dataframe. Disables one-hot encoding and drop
-        errors on the new subset if raw is not maintained. These actions only
-        need to be performed once.
+    def subset(self, new_filter: None | str | List[str] = None, maintain_raw: bool = False) -> DataSet:
+        """Return a further dataset utilising the current processed dataframe as its base dataframe. Disables one-hot
+        encoding and drop errors on the new subset if raw is not maintained. These actions only need to be performed
+        once.
 
         Parameters
         ----------
         new_filter: optional, default = None
-            Filter to define the sub-set. Can be none, just to match the
-            current dataset, a string for a single filter, or a list of
-            strings for multiple filters.
+            Filter to define the sub-set. Can be none, just to match the current dataset, a string for a single
+            filter, or a list of strings for multiple filters.
 
         maintain_raw: optional, default = False
-            Bool flag whether the new dataset should maintain the full depth to
-            the raw dataframe. This can sometimes be easier for categorical
-            filtering with one-hot encoding. Otherwise, it is recommendable
-            to drop the already filtered rows to improve performance.
+            Bool flag whether the new dataset should maintain the full depth to the raw dataframe. This can sometimes
+            be easier for categorical filtering with one-hot encoding. Otherwise, it is recommendable to drop the
+            already filtered rows to improve performance.
         """
         subset = self.copy()
 
         # Base subset on own processed dataset.
         if maintain_raw:
             if new_filter is not None:
                 if isinstance(new_filter, list):
@@ -558,257 +498,24 @@
             # Clear already applied filters.
             subset.filter_list = new_filter
 
         return subset
     # endregion
 
     # region Extensions
-    def get_model_xy(self, output_key: str,
-                     input_keys: str | List[str] | None = None,
+    def get_model_xy(self, output_key: str, input_keys: str | List[str] | None = None,
                      add_constant: bool = True) -> (np.ndarray, np.ndarray):
-        """Return prepared X, y values of the dataset for input into a
-        regression model."""
+        """Return prepared X, y values of the dataset for input into a regression model."""
         if input_keys is None:
             input_keys = self.input_keys
         x = self.df.loc[:, input_keys].astype(float)
         if add_constant:
             x = sm.add_constant(x)
         y = self.df.loc[:, output_key]
         return x, y
-
-    def get_ols(self, output_key: str,
-                input_keys: str | List[str] | None = None,
-                add_constant: bool = True) -> RegressionResults:
-        """Return Ordinary Least Squares (OLS) model of the dataset."""
-        x, y = self.get_model_xy(output_key, input_keys, add_constant)
-        return OLS(y, x).fit()
-
-    def get_random_forest_regressor(
-            self, output_key: str,
-            input_keys: str | List[str] | None = None,
-            add_constant: bool = True, **kwargs) -> RandomForestRegressor:
-        """Return Scikit-Learn Random Forest Regressor of the dataset."""
-        regressor = RandomForestRegressor(**kwargs)
-        regressor.fit(*self.get_model_xy(output_key, input_keys, add_constant))
-        return regressor
-
-    def get_mlp_regressor(
-            self, output_key: str,
-            input_keys: str | List[str] | None = None,
-            add_constant: bool = True, **kwargs) -> MLPRegressor:
-        """Return Scikit-Learn MLP Neural Network Regressor of the dataset."""
-        regressor = MLPRegressor(**kwargs)
-        regressor.fit(*self.get_model_xy(output_key, input_keys, add_constant))
-        return regressor
-
-    @staticmethod
-    def __get_compiled_keras_regressor__(
-            n_output_dim: int,
-            normalizer: keras.layers.Normalization,
-            out_denormalizer: keras.layers.Normalization,
-            n_hidden_layers: int,
-            dense_layer_units: int,
-            dense_activation: str = 'relu6',
-            learning_rate: float = 1e-2,
-            loss: str = 'mean_squared_error') -> keras.Model:
-        """Get Tensorflow Keras regressor."""
-        K.clear_session()
-        model = keras.Sequential([
-            normalizer,
-            *[keras.layers.Dense(dense_layer_units,
-                                 activation=dense_activation,
-                                 name='dense_' + str(n))
-              for n in range(n_hidden_layers)],
-            keras.layers.Dense(n_output_dim, name='dense_output'),
-            out_denormalizer
-        ])
-        model.compile(
-            optimizer=keras.optimizers.Adam(learning_rate=learning_rate),
-            loss=loss)
-
-        return model
-
-    @staticmethod
-    def __get_keras_normalizers__(
-            X: np.ndarray | pd.DataFrame, y: np.ndarray | pd.DataFrame
-            ) -> (keras.layers.Normalization, keras.layers.Normalization):
-        """Return keras normalisation and de-normalisation layers for deep
-        neural networks."""
-        # Normalize to mean 0, variance 1
-        normalizer = keras.layers.Normalization(name='normalizer')
-        normalizer.adapt(np.asarray(X).astype(float))
-        # De-Normalize from mean 0, variance 1
-        de_normalizer = keras.layers.Normalization(invert=True,
-                                                   name='de-normalizer')
-        if len(X.shape) == 2:
-            normalizer.adapt(np.asarray(X).astype(float))
-        else:
-            normalizer.adapt(np.atleast_2d(X).T.astype(float))
-        if len(y.shape) == 2:
-            de_normalizer.adapt(np.asarray(y).astype(float))
-        else:
-            de_normalizer.adapt(np.atleast_2d(y).T.astype(float))
-        return normalizer, de_normalizer
-
-    def get_keras_regressor(
-            self, output_key: str,
-            input_keys: str | List[str] | None = None,
-            add_constant: bool = True,
-            test_size: float = 0.1,
-            n_hidden_layers: int = None,
-            dense_units: int = None,
-            batch_size: int = None,
-            epochs: int = None,
-            ** kwargs) -> (keras.Model, Any):
-        """Get Tensorflow Keras regressor."""
-        X, y = self.get_model_xy(output_key, input_keys, add_constant)
-        n_input_dim = X.shape[1]
-        try:
-            n_output_dim = y.shape[1]
-        except IndexError:
-            n_output_dim = 1
-        if n_hidden_layers is None:
-            n_hidden_layers = 2
-        if dense_units is None:
-            dense_units = int(2 ** (np.ceil(np.log2(n_input_dim)) + 2))
-        if batch_size is None:
-            batch_size = X.shape[0]
-        if epochs is None:
-            epochs = 500
-
-        normalizer, de_normaliser = self.__get_keras_normalizers__(X, y)
-
-        model = self.__get_compiled_keras_regressor__(
-            n_output_dim, normalizer, de_normaliser,
-            n_hidden_layers, dense_units,
-            dense_activation=kwargs.get('dense_activation', 'relu6'),
-            learning_rate=kwargs.get('learning_rate', 1e-2),
-            loss=kwargs.get('loss', 'mean_squared_error')
-        )
-
-        callbacks = [
-            keras.callbacks.EarlyStopping(monitor='val_loss', patience=10,
-                                          restore_best_weights=True)]
-
-        history = model.fit(X, y, batch_size=batch_size, epochs=epochs,
-                            validation_split=test_size, callbacks=callbacks)
-
-        return model, history
-
-    def get_keras_regressor_optimized(
-            self, output_key: str,
-            input_keys: str | List[str] | None = None,
-            add_constant: bool = True,
-            test_size: float = 0.1,
-            batch_size: int = None,
-            optimization_epochs: int = None,
-            final_epochs: int = None,
-            tuner_model: str = 'bayesian',
-            n_hidden_layers: List[int] | int | None = None,
-            dense_units: List[int] | int | None = None,
-            dense_activation: List[str] | str | None = None,
-            learning_rate: List[float] | float | None = None,
-            **kwargs) -> keras.Model:
-        """Get Tensorflow Keras regressor."""
-        X, y = self.get_model_xy(output_key, input_keys, add_constant)
-        try:
-            n_output_dim = y.shape[1]
-        except IndexError:
-            n_output_dim = 1
-        if batch_size is None:
-            batch_size = X.shape[0]
-        if optimization_epochs is None:
-            optimization_epochs = 100
-        if final_epochs is None:
-            final_epochs = 500
-        if n_hidden_layers is None:
-            n_hidden_layers = [1, 4, 1]
-        if dense_units is None:
-            dense_units = [16, 1024, 16]
-        if dense_activation is None:
-            dense_activation = ['relu6', 'tanh']
-        if learning_rate is None:
-            learning_rate = [1e-4, 0.25]
-
-        normalizer, de_normaliser = self.__get_keras_normalizers__(X, y)
-
-        def build_model(hp):
-            if isinstance(n_hidden_layers, list):
-                n_layers = hp.Int(
-                    'n_hidden_layers', min_value=n_hidden_layers[0],
-                    max_value=n_hidden_layers[1], step=n_hidden_layers[2])
-            else:
-                n_layers = n_hidden_layers
-            if isinstance(dense_units, list):
-                units = hp.Int(
-                    'dense_units', min_value=dense_units[0],
-                    max_value=dense_units[1], step=dense_units[2])
-            else:
-                units = dense_units
-            if isinstance(dense_activation, list):
-                activation = hp.Choice(
-                    'dense_activation', values=dense_units)
-            else:
-                activation = dense_activation
-            if isinstance(learning_rate, list):
-                l_rate = hp.Float(
-                    'learning_rate', min_value=learning_rate[0],
-                    max_value=learning_rate[1])
-            else:
-                l_rate = learning_rate
-
-            return self.__get_compiled_keras_regressor__(
-                n_output_dim, normalizer, de_normaliser, n_layers, units,
-                dense_activation=activation,
-                learning_rate=l_rate,
-                loss=kwargs.get('loss', 'mean_squared_error')
-            )
-
-        callbacks = [
-            keras.callbacks.EarlyStopping(monitor='val_loss', patience=10,
-                                          restore_best_weights=True)]
-
-        if tuner_model == 'bayesian':
-            tuner = keras_tuner.tuners.BayesianOptimization(
-                build_model,
-                objective=keras_tuner.Objective('val_loss', direction="min"),
-                max_trials=kwargs.get('max_trials', 200),
-                overwrite=True)
-
-            tuner.search(X, y, batch_size=batch_size,
-                         epochs=optimization_epochs,
-                         validation_split=test_size,
-                         callbacks=callbacks)
-
-        elif tuner_model == 'hyperband':
-            tuner = keras_tuner.tuners.Hyperband(
-                build_model,
-                objective='val_loss',
-                max_epochs=optimization_epochs,
-                executions_per_trial=kwargs.get('executions_per_trial', 2),
-                overwrite=True)
-
-            tuner.search(X, y, batch_size=batch_size,
-                         validation_split=test_size,
-                         callbacks=callbacks)
-        else:
-            raise ValueError("Unrecognised tuner_model, must be 'bayesian' "
-                             "or 'hyperband'.")
-
-        model = tuner.get_best_models(num_models=2)[0]
-
-        if final_epochs > optimization_epochs:
-            # Recreate the callbacks to ensure they can be deep-copied.
-            callbacks = [keras.callbacks.EarlyStopping(
-                monitor='val_loss', patience=10, restore_best_weights=True)]
-
-            model.fit(X, y, batch_size=batch_size,  epochs=final_epochs,
-                      validation_split=test_size, callbacks=callbacks)
-
-        return model
     # endregion
 
     # region Saving
     def copy(self) -> DataSet:
         """Return a copy of the DataSet using the copy package."""
         return deepcopy(self)
 
@@ -834,376 +541,324 @@
         --------
         DataSet.df
         """
         return self.df.shape[0]
 
     @property
     def n_cases_fraction(self) -> float:
-        """Return fraction of cases selected post filtering compared to
-        original dataframe.
+        """Return fraction of cases selected post filtering compared to original dataframe.
 
         See Also
         --------
         DataSet.df
         DataSet.raw_df
         """
         return self.n_cases / self.raw_df.shape[0]
 
     @property
     def n_errors(self) -> int:
-        """Return number of cases with recognised errors. Includes the
-        custom error filter.
+        """Return number of cases with recognised errors. Includes the custom error filter.
 
         See Also
         --------
         DataSet.df_errors
         """
         return self.df_errors.shape[0]
 
     @property
     def n_errors_fraction(self) -> float:
-        """Return fraction of cases with recognised errors compared to
-        original dataframe.
+        """Return fraction of cases with recognised errors compared to original dataframe.
 
         See Also
         --------
         DataSet.df_errors
         DataSet.raw_df
         """
         return self.n_errors / self.raw_df.shape[0]
     # endregion
 
     # region Correlations
     def corr(self, key: str = None, sort: bool = True,
-             split_input_output: bool = False,
-             alternate_df: pd.DataFrame = None) -> pd.DataFrame:
-        """Return Pearson correlation coefficient matrix for the filtered
-        dataframe or for a selected key therein. The matrix is optionally
-        sorted in descending order.
+             split_input_output: bool = False, alternate_df: pd.DataFrame = None) -> pd.DataFrame:
+        """Return Pearson correlation coefficient matrix for the filtered dataframe or for a selected key therein.
+        The matrix is optionally sorted in descending order.
 
         Degree of correlation:
             - Perfect: |C| ~ 1
             - High degree: 0.5 <= |C| < 1
             - Moderate degree: 0.3 <= |C| < 0.5
             - Low degree: 0 < |C| < 0.3
             - No correlation: |C| ~ 0
 
         Parameters
         ----------
         key: optional, default = None
-            Input or output key to down-select correlation matrix. If the
-            default none is passed, the full matrix is returned.
+            Input or output key to down-select correlation matrix. If the default none is passed, the full matrix is
+            returned.
 
         sort: optional, default = True
-            Bool flag whether to sort the down-selected matrix by absolute
-            descending order. If no key is passed, this option is ignored.
+            Bool flag whether to sort the down-selected matrix by absolute descending order. If no key is passed,
+            this option is ignored.
 
         split_input_output: optional, default = False
-            Bool flag whether to format the resulting symmetrical matrix to
-            split input and output columns. If set to True, rows are the
-            model inputs, and columns are the model outputs. If examining a
-            model as a black box, this may be preferable to reduce clutter.
+            Bool flag whether to format the resulting symmetrical matrix to split input and output columns. If set to
+            True, rows are the model inputs, and columns are the model outputs. If examining a model as a black box,
+            this may be preferable to reduce clutter.
 
         alternate_df: optional, default = None
-            An alternate dataframe to use for the analysis. If None is
-            passed, the main dataframe is used. This functionality is used
-            for example by the filter analysis functions. Please note,
-            the dataframe is still split with the main input and output keys.
+            An alternate dataframe to use for the analysis. If None is passed, the main dataframe is used. This
+            functionality is used for example by the filter analysis functions. Please note, the dataframe is still
+            split with the main input and output keys.
 
         Returns
         -------
         pd.DataFrame
             Correlation matrix.
         """
         if alternate_df is None:
             df = self.df
         else:
             df = alternate_df
         corr = df.corr()
         if split_input_output:
-            corr.drop(columns=self.input_keys, index=self.output_keys,
-                      inplace=True)
+            corr.drop(columns=self.input_keys, index=self.output_keys, inplace=True)
         if key is not None:
             if key in self.input_keys:
                 corr = corr.loc[key, :]
             else:
                 corr = corr.loc[:, key]
             if sort:
                 # Don't use in-place due to some pandas weirdness
                 corr = corr.sort_values(ascending=False, key=abs)
         return corr
 
-    def get_significant_keys(self, key: str,
-                             threshold: str | float = 'high',
-                             alternate_df: pd.DataFrame = None
+    def get_significant_keys(self, key: str, threshold: str | float = 'high', alternate_df: pd.DataFrame = None
                              ) -> List[str]:
-        """Return list of columns whose Pearson correlation coefficient is
-        above the given threshold for a given input key.
+        """Return list of columns whose Pearson correlation coefficient is above the given threshold for a given
+        input key.
 
         Degree of correlation:
             - Perfect: |C| ~ 1, here defined as 0.98 <= |C| < 1
             - High degree: 0.5 <= |C| < 1
             - Moderate degree: 0.3 <= |C| < 0.5
             - Low degree: 0 < |C| < 0.3, here defined as 0.02 <= |C| < 0.3
             - No correlation: |C| ~ 0, here defined as 0 <= |C| < 0.02
 
         Parameters
         ----------
         key
-            Input or output key for which the significant keys should be
-            identified.
+            Input or output key for which the significant keys should be identified.
 
         threshold: optional, default = 'high'
             Threshold above which a correlation is deemed significant.
 
         alternate_df: optional, default = None
-            An alternate dataframe to use for the analysis. If None is
-            passed, the main dataframe is used. This functionality is used
-            for example by the filter analysis functions. Please note,
-            the dataframe is still split with the main input and output keys.
+            An alternate dataframe to use for the analysis. If None is passed, the main dataframe is used. This
+            functionality is used for example by the filter analysis functions. Please note, the dataframe is still
+            split with the main input and output keys.
 
         See Also
         --------
         DataSet.corr
 
         Notes
         -----
         Pearson Correlation coefficient is suitable for linear relationships.
         """
         threshold = get_numerical_correlation_threshold(threshold)
-        corr = self.corr(key=key, sort=True, split_input_output=False,
-                         alternate_df=alternate_df)
+        corr = self.corr(key=key, sort=True, split_input_output=False, alternate_df=alternate_df)
         sig_keys = corr.index[corr.abs() >= threshold]
         return sig_keys[sig_keys != key]
 
-    def correlation_count_analysis(self, key: str,
-                                   alternate_df: pd.DataFrame = None
-                                   ) -> pd.Series:
-        """Return dataframe of correlation counts at various thresholds for
-        requested key. Notably each threshold does not contain the entries
-        of higher levels.
+    def correlation_count_analysis(self, key: str, alternate_df: pd.DataFrame = None) -> pd.Series:
+        """Return dataframe of correlation counts at various thresholds for requested key. Notably each threshold
+        does not contain the entries of higher levels.
 
         Parameters
         ----------
         key
             Input or output key for which the analysis should be conducted.
 
         alternate_df: optional, default = None
-            An alternate dataframe to use for the analysis. If None is
-            passed, the main dataframe is used. This functionality is used
-            for example by the filter analysis functions. Please note,
-            the dataframe is still split with the main input and output keys.
+            An alternate dataframe to use for the analysis. If None is passed, the main dataframe is used. This
+            functionality is used for example by the filter analysis functions. Please note, the dataframe is still
+            split with the main input and output keys.
 
         Returns
         -------
         pd.Series
-            Pandas Dataframe with the input columns as rows and the
-            thresholds perfect, high, moderate, low, and total as columns.
+            Pandas Dataframe with the input columns as rows and the thresholds perfect, high, moderate, low,
+            and total as columns.
         """
         df = pd.Series(dtype=int)
         for threshold in ['perfect', 'high', 'moderate', 'low']:
-            df.loc[threshold] = len(self.get_significant_keys(
-                key, threshold, alternate_df=alternate_df))
+            df.loc[threshold] = len(self.get_significant_keys(key, threshold, alternate_df=alternate_df))
         df.name = key
         df.loc['total'] = df.low.copy()
         # Subtract higher levels
         df.low -= df.moderate
         df.moderate -= df.high
         df.high -= df.perfect
         return df.astype(int)
 
-    def input_correlation_count_analysis(self,
-                                         alternate_df: pd.DataFrame = None
-                                         ) -> pd.DataFrame:
-        """Return dataframe of correlation counts at various thresholds for
-        each input key. Notably each threshold does not contain the entries
-        of higher levels.
+    def input_correlation_count_analysis(self, alternate_df: pd.DataFrame = None) -> pd.DataFrame:
+        """Return dataframe of correlation counts at various thresholds for each input key. Notably each threshold
+        does not contain the entries of higher levels.
 
         Parameters
         ----------
         alternate_df: optional, default = None
-            An alternate dataframe to use for the analysis. If None is
-            passed, the main dataframe is used. This functionality is used
-            for example by the filter analysis functions. Please note,
-            the dataframe is still split with the main input and output keys.
+            An alternate dataframe to use for the analysis. If None is passed, the main dataframe is used. This
+            functionality is used for example by the filter analysis functions. Please note, the dataframe is still
+            split with the main input and output keys.
 
         Returns
         -------
         pd.DataFrame
-            Pandas Dataframe with the input columns as rows and the
-            thresholds perfect, high, moderate, low, and total as columns.
+            Pandas Dataframe with the input columns as rows and the thresholds perfect, high, moderate, low,
+            and total as columns.
 
         See Also
         --------
         DataSet.correlation_count_analysis
         """
         df = pd.DataFrame()
         for key in self.input_keys:
-            df = pd.concat((df, self.correlation_count_analysis(
-                key, alternate_df=alternate_df)), axis=1)
+            df = pd.concat((df, self.correlation_count_analysis(key, alternate_df=alternate_df)), axis=1)
         return df.T
 
     # endregion
 
     # region Filter Analysis
-    def correlation_count_filter_progression(self, key: str,
-                                             stacked: bool = True
-                                             ) -> pd.DataFrame:
-        """Evaluate how each filter level affects the progression of
-        correlations on a specific input or output key.
+    def correlation_count_filter_progression(self, key: str, stacked: bool = True) -> pd.DataFrame:
+        """Evaluate how each filter level affects the progression of correlations on a specific input or output key.
 
         Parameters
         ----------
         key
             Input or output key for which the analysis should be conducted.
 
         stacked: optional, default = True
-            Bool flag whether to stack filters. E.g. show the incremental
-            improvement of the full filter set (True) or the impact of the
-            individual filters on the original dataset (False).
+            Bool flag whether to stack filters. E.g. show the incremental improvement of the full filter set (True)
+            or the impact of the individual filters on the original dataset (False).
 
         Returns
         -------
         pd.DataFrame
-            Pandas DataFrame with the rows representing each filter level
-            and the columns representing the thresholds.
+            Pandas DataFrame with the rows representing each filter level and the columns representing the thresholds.
         """
         df = pd.DataFrame(dtype=int)
         dfs = self.get_dfs_filter_levels(stacked=stacked)
         for level, value in dfs.items():
-            df_new = self.correlation_count_analysis(key,
-                                                     alternate_df=value)
+            df_new = self.correlation_count_analysis(key, alternate_df=value)
             df_new.name = level
             df = pd.concat((df, df_new), axis=1)
         return df
 
-    def get_case_count_with_filter_level(self, stacked: bool = True,
-                                         normed: bool = False) -> dict:
-        """Return dictionary with filter levels and number of cases in the
-        dataset.
+    def get_case_count_with_filter_level(self, stacked: bool = True, normed: bool = False) -> dict:
+        """Return dictionary with filter levels and number of cases in the dataset.
 
         Parameters
         ----------
         stacked: optional, default = True
-            Bool flag whether to stack filters. E.g. show the incremental
-            improvement of the full filter set (True) or the impact of the
-            individual filters on the original dataset (False).
+            Bool flag whether to stack filters. E.g. show the incremental improvement of the full filter set (True)
+            or the impact of the individual filters on the original dataset (False).
 
         normed: optional, default = False
-            Bool flag whether the values should be normalised against the
-            size of the initial dataset.
+            Bool flag whether the values should be normalised against the size of the initial dataset.
         """
         case_counts = {}
         dfs = self.get_dfs_filter_levels(stacked=stacked)
         for level, value in dfs.items():
             case_counts[level] = value.shape[0]
             if normed:
                 case_counts[level] /= list(case_counts.values())[0]
         return case_counts
 
-    def get_filter_reduction_degrees(self, individual: bool = False,
-                                     stacked: bool = True) -> dict:
+    def get_filter_reduction_degrees(self, individual: bool = False, stacked: bool = True) -> dict:
         """Get reduction degree of each filter level.
 
         Parameters
         ----------
         individual: optional, default = False
-            Bool flag whether the reduction level of each filter should be
-            evaluated individually relative to the raw data frame or to a
-            previous reduction (select using the stacked parameter).
+            Bool flag whether the reduction level of each filter should be evaluated individually relative to the raw
+            data frame or to a previous reduction (select using the stacked parameter).
 
         stacked: optional, default = True
-            Bool flag whether to stack filters. E.g. show the incremental
-            improvement of the full filter set (True) or the impact of the
-            individual filters on the original dataset (False). Note,
-            the original dataset already includes the no_errors correction.
-            If this is not desired, set individual to True.
+            Bool flag whether to stack filters. E.g. show the incremental improvement of the full filter set (True)
+            or the impact of the individual filters on the original dataset (False). Note, the original dataset
+            already includes the no_errors correction. If this is not desired, set individual to True.
         """
         reductions = {}
         raw_df = self.raw_df
         n_no_errors = n_raw = raw_df.shape[0]
         if self.drop_errors:
             n_no_errors = self.df_no_errors.shape[0]
             reductions['no_errors'] = n_no_errors / n_raw
         if individual:
             for s_filter in self.filter_list:
-                reductions[s_filter] = \
-                    raw_df.query(s_filter).shape[0] / n_raw
+                reductions[s_filter] = raw_df.query(s_filter).shape[0] / n_raw
         else:
             dfs = self.get_dfs_filter_levels(stacked=stacked)
-            if len(dfs) > 2 or (
-                    len(dfs) > 1 and list(dfs.keys())[1] != 'no_errors'):
+            if len(dfs) > 2 or (len(dfs) > 1 and list(dfs.keys())[1] != 'no_errors'):
                 n_last = n_no_errors
                 for level, df in dfs.items():
                     if level in ['raw', 'no_errors']:
                         continue
                     reductions[level] = df.shape[0] / n_last
                     if stacked:
                         n_last = df.shape[0]
 
         return reductions
 
-    def get_filter_describes(self, key: str, stacked: bool = True
-                             ) -> pd.DataFrame:
-        """Get dataframe of pandas describe for each filter level in respect to
-        a specific column key.
+    def get_filter_describes(self, key: str, stacked: bool = True) -> pd.DataFrame:
+        """Get dataframe of pandas describe for each filter level in respect to a specific column key.
 
         Parameters
         ----------
         key
             Evaluation key on which pd.Describe is called.
 
         stacked: optional, default = True
-            Bool flag whether to stack filters. E.g. show the incremental
-            impact of the full filter set (True) or the impact of the
-            individual filters on the original dataset (False). Note,
-            the original dataset already includes the no_errors correction.
+            Bool flag whether to stack filters. E.g. show the incremental impact of the full filter set (True) or the
+            impact of the individual filters on the original dataset (False). Note, the original dataset already
+            includes the no_errors correction.
         """
         dfs = self.get_dfs_filter_levels(stacked=stacked)
         describes = pd.DataFrame()
         for level, df in dfs.items():
             describe = df.loc[:, key].describe()
             describe.name = level
             describes = pd.concat((describes, describe), axis=1)
         return describes
     # endregion
     # endregion
 
     # region Visualisation
-    def plot_input_correlation_count_analysis(self, stacked: bool = False,
-                                              ax: plt.Axes = None,
-                                              title: str = None
-                                              ) -> plt.Figure:
-        """Plot a bar-graph of the correlation threshold counts for input
-        parameters."""
+    def plot_input_correlation_count_analysis(self, stacked: bool = False, ax: plt.Axes = None,
+                                              title: str = None) -> plt.Figure:
+        """Plot a bar-graph of the correlation threshold counts for input parameters."""
         df = self.input_correlation_count_analysis()
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = None
 
         x_axis = np.arange(len(df.index))
 
         if stacked:
             ax.bar(x_axis, df.low, label='low', color='r')
-            ax.bar(x_axis, df.moderate, bottom=df.low,
-                   label='moderate', color='orange')
-            ax.bar(x_axis, df.high, bottom=df.low + df.moderate,
-                   label='high', color='g')
-            ax.bar(x_axis, df.perfect,
-                   bottom=df.low + df.moderate + df.high,
-                   label='perfect', color='b')
+            ax.bar(x_axis, df.moderate, bottom=df.low, label='moderate', color='orange')
+            ax.bar(x_axis, df.high, bottom=df.low + df.moderate, label='high', color='g')
+            ax.bar(x_axis, df.perfect, bottom=df.low + df.moderate + df.high, label='perfect', color='b')
         else:
             ax.bar(x_axis + 0.3, df.low, 0.2, label='low', color='r')
-            ax.bar(x_axis + 0.1, df.moderate, 0.2,
-                   label='moderate', color='orange')
-            ax.bar(x_axis - 0.1, df.high, 0.2,
-                   label='high', color='g')
-            ax.bar(x_axis - 0.3, df.perfect, 0.2,
-                   label='perfect', color='b')
+            ax.bar(x_axis + 0.1, df.moderate, 0.2, label='moderate', color='orange')
+            ax.bar(x_axis - 0.1, df.high, 0.2, label='high', color='g')
+            ax.bar(x_axis - 0.3, df.perfect, 0.2, label='perfect', color='b')
 
         ax.set_xticks(x_axis, df.index, rotation=45, ha="right")
         if title is None:
             ax.set_title("Input Correlation Thresholds")
         else:
             ax.set_title(title)
         ax.legend(title='Threshold')
@@ -1214,18 +869,16 @@
 
     def plot_significant_keys(self, key: str,
                               split_input_output: bool = True,
                               threshold: str | float = 'low',
                               ax: plt.Axes = None, absolute: bool = True,
                               title: str = None, y_label: str = None
                               ) -> plt.Figure:
-        """Plot a bar-graph of the correlation coefficients of relevant
-        keys for a given input key."""
-        df = self.corr(key=key, sort=True,
-                       split_input_output=split_input_output)
+        """Plot a bar-graph of the correlation coefficients of relevant keys for a given input key."""
+        df = self.corr(key=key, sort=True, split_input_output=split_input_output)
         threshold = get_numerical_correlation_threshold(threshold)
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = None
 
         df = df[df.abs() > threshold]
@@ -1235,16 +888,15 @@
             df = df.abs()
 
         ax.bar(x_axis, df)
 
         ax.set_xticks(x_axis, df.index, rotation=45, ha="right")
         ax.set_ylim(0, 1)
         if title is None:
-            ax.set_title(f"{key.title().replace('_', ' ')} - "
-                         f"Significant Correlations")
+            ax.set_title(f"{key.title().replace('_', ' ')} - Significant Correlations")
         elif title == 'empty':
             pass
         else:
             ax.set_title(title)
 
         if y_label == 'empty':
             ax.set_yticks([0, 0.2, 0.4, 0.6, 0.8, 1.0], [])
@@ -1255,50 +907,43 @@
         else:
             ax.set_ylabel('Correlation Coefficient, -')
         ax.grid()
         if fig is not None:
             fig.tight_layout()
         return fig
 
-    def plot_correlation_count_filter_progression(self, key: str,
-                                                  ax: plt.Axes = None
-                                                  ) -> plt.Figure:
+    def plot_correlation_count_filter_progression(self, key: str, ax: plt.Axes = None) -> plt.Figure:
         """Plot a bar-graph of the correlation threshold counts for input
         parameters."""
         df = self.correlation_count_filter_progression(key)
         df.drop(index='total', inplace=True)
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = None
 
         x_axis = np.arange(len(df.columns))
 
-        ax.stackplot(x_axis, df[::-1], baseline='zero',
-                     labels=df.index[::-1],
-                     colors=['r', 'orange', 'g', 'b'])
+        ax.stackplot(x_axis, df[::-1], baseline='zero', labels=df.index[::-1], colors=['r', 'orange', 'g', 'b'])
 
         ax.set_xticks(x_axis, df.columns, rotation=45, ha="right")
         ax.set_title(f"{key}Input Correlation Thresholds")
         handles, labels = ax.get_legend_handles_labels()
-        ax.legend(handles[::-1], labels[::-1],
-                  title='Threshold', loc='upper left')
+        ax.legend(handles[::-1], labels[::-1], title='Threshold', loc='upper left')
         plt.grid()
         plt.tight_layout()
         return fig
 
     def plot_case_counts_with_filter_levels(self, stacked: bool = True,
                                             normed: bool = False,
                                             y_scale: str = 'linear',
                                             ax: plt.Axes = None
                                             ) -> plt.Figure:
         """Plot line plot as number of cases decreases with filter levels."""
-        case_counts = self.get_case_count_with_filter_level(
-            stacked=stacked,
-            normed=normed)
+        case_counts = self.get_case_count_with_filter_level(stacked=stacked, normed=normed)
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = None
 
         x_axis = np.arange(len(case_counts))
 
@@ -1307,38 +952,34 @@
         ax.set_xticks(x_axis, case_counts.keys(), rotation=45, ha="right")
         ax.set_yscale(y_scale)
         ax.set_title("Case Counts with Filter Levels")
         plt.grid()
         plt.tight_layout()
         return fig
 
-    def plot_filter_reduction_degree(self, individual: bool = False,
-                                     stacked: bool = True,
+    def plot_filter_reduction_degree(self, individual: bool = False, stacked: bool = True,
                                      ax: plt.Axes = None) -> plt.Figure:
         """Plot line plot as number of cases decreases with filter levels."""
-        reduction_degrees = self.get_filter_reduction_degrees(
-            individual=individual, stacked=stacked)
+        reduction_degrees = self.get_filter_reduction_degrees(individual=individual, stacked=stacked)
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = None
 
         x_axis = np.arange(len(reduction_degrees))
 
         ax.bar(x_axis, reduction_degrees.values())
 
-        ax.set_xticks(x_axis, reduction_degrees.keys(),
-                      rotation=45, ha="right")
+        ax.set_xticks(x_axis, reduction_degrees.keys(), rotation=45, ha="right")
         ax.set_title("Filter Reduction Degrees")
         plt.grid()
         plt.tight_layout()
         return fig
 
-    def plot_filter_progression_box_plots(self, key: str,
-                                          stacked: bool = True,
+    def plot_filter_progression_box_plots(self, key: str, stacked: bool = True,
                                           ax: plt.Axes = None) -> plt.Figure:
         """Plot line plot as number of cases decreases with filter levels.
 
         Nan values are removed from the raw dataframe if needed.
         """
         dfs = self.get_dfs_filter_levels(stacked)
         if ax is None:
@@ -1349,16 +990,15 @@
         x_axis = np.arange(1, len(dfs) + 1)
         y_values = [df.loc[:, key] for df in dfs.values()]
         if list(dfs.keys())[0] == 'raw':
             y_values[0].dropna(inplace=True)
         ax.boxplot(y_values, labels=dfs.keys())
 
         ax.set_xticks(x_axis, dfs.keys(), rotation=45, ha="right")
-        ax.set_title(key.title().replace('_', ' ')
-                     + "Filter Distribution Impact")
+        ax.set_title(key.title().replace('_', ' ') + "Filter Distribution Impact")
         plt.grid()
         plt.tight_layout()
         return fig
 
     def plot_2d(self, key_x: str, keys_y: str | List[str],
                 key_categorical: str = None, key_size: str = None,
                 key_color: str = None, size_adj_factor: float = 1.0,
@@ -1382,16 +1022,15 @@
         key_categorical: optional, default = None
             Categorical key to split the plotting over. E.g. fuel.
 
         key_size: optional, default = None
             Marker size value key
 
         key_color: optional, default = None
-            Marker color value key. If a categorical key is given,
-            each color gets a monotone color gradient.
+            Marker color value key. If a categorical key is given, each color gets a monotone color gradient.
 
         size_adj_factor: optional, default = 1.0
             Linear scaling factor on the marker size if a key_size is given.
 
         ax: optional, default = None
             Optionally pass an existing Axes to plot to same figure.
 
@@ -1404,37 +1043,33 @@
         y_label: optional, default = None
             Manually set y-axis label
 
         legend_kwargs: optional, default = None
             Dictionary of keyword argument to pass to the legend command.
 
         alternate_df: optional, default = None
-            An alternate dataframe to use as source. If None is
-            passed, the main dataframe is used. This functionality is used
-            for example by the filter analysis functions. Please note,
-            the dataframe is still interpreted with the stored unit and
-            axis_label dataframes.
+            An alternate dataframe to use as source. If None is passed, the main dataframe is used. This
+            functionality is used for example by the filter analysis functions. Please note, the dataframe is still
+            interpreted with the stored unit and axis_label dataframes.
 
         plot_raw: optional, default = False
-            Bool flag whether the raw data should be plotted beneath the
-            target date. Data is plotted in grey.
+            Bool flag whether the raw data should be plotted beneath the target date. Data is plotted in grey.
 
         plot_errors: optional, default = False
-            Bool flag whether the error data should be plotted beneath the
-            target date. Data is plotted in red.
+            Bool flag whether the error data should be plotted beneath the target date. Data is plotted in red.
 
         plot_only_errors: optional, default = False
             Bool flag whether only the error data should be plotted.
 
         plot_kwargs: Optional
             Plot keyword arguments passed to the plotting function.
 
         kwargs: Optional
-            Keyword arguments used for additional plot adjustment,
-            e.g. disabling the color bar with colorbar=False, xlim, clim, ylim
+            Keyword arguments used for additional plot adjustment, e.g. disabling the color bar with colorbar=False,
+            xlim, clim, ylim
 
         See Also
         --------
         plt.Figure
         plt.scatter
         """
         if legend_kwargs is None:
@@ -1463,116 +1098,91 @@
         if ax is None:
             fig, ax = plt.subplots()
         else:
             fig = None
         ax.grid()
 
         if plot_raw and not plot_only_errors:
-            ax.scatter(self.raw_df[key_x], self.raw_df[key_y_single],
-                       c='grey', **plot_kwargs, label='raw')
+            ax.scatter(self.raw_df[key_x], self.raw_df[key_y_single], c='grey', **plot_kwargs, label='raw')
         if plot_errors:
-            ax.scatter(self.df_errors[key_x], self.df_errors[key_y_single],
-                       c='red', **plot_kwargs, label='errors')
+            ax.scatter(self.df_errors[key_x], self.df_errors[key_y_single], c='red', **plot_kwargs, label='errors')
         if plot_only_errors:
             try:
                 df_errors = alternate_df['df_errors']
                 df_raw = alternate_df['df_raw']
             except (KeyError, TypeError):
                 df_errors = self.df_errors
                 df_raw = self.raw_df
             error_filter = self.error_filter
             if error_filter is not None and error_filter != []:
-                df_errors_filter = apply_filter(df_raw, error_filter,
-                                                join_and=False)
-                df_errors_detected = df_errors.drop(
-                    index=df_errors_filter.index, errors='ignore')
+                df_errors_filter = apply_filter(df_raw, error_filter, join_and=False)
+                df_errors_detected = df_errors.drop(index=df_errors_filter.index, errors='ignore')
             else:
                 df_errors_filter = pd.DataFrame(columns=df_errors.columns)
                 df_errors_detected = df_errors.copy()
-            ax.scatter(df_errors_detected[key_x],
-                       df_errors_detected[key_y_single],
+            ax.scatter(df_errors_detected[key_x], df_errors_detected[key_y_single],
                        c='red', **plot_kwargs, label='Detected')
             if error_filter is not None and error_filter != []:
-                ax.scatter(df_errors_filter[key_x],
-                           df_errors_filter[key_y_single],
+                ax.scatter(df_errors_filter[key_x], df_errors_filter[key_y_single],
                            c='tab:orange', **plot_kwargs, label='Filter')
 
         for key in keys_y_plotting:
             if plot_only_errors:
                 break  # Don't plot anything else
 
             if key_categorical is None:
                 if key_size is None and key_color is None:
-                    ax.scatter(df[key_x], df[key], label=key,
-                               **plot_kwargs)
+                    ax.scatter(df[key_x], df[key], label=key, **plot_kwargs)
                 elif key_size is None:
-                    ax.scatter(df[key_x], df[key], c=df[key_color],
-                               cmap='jet',
-                               label=key, **plot_kwargs)
+                    ax.scatter(df[key_x], df[key], c=df[key_color], cmap='jet', label=key, **plot_kwargs)
                 elif key_color is None:
-                    ax.scatter(df[key_x], df[key],
-                               s=df[key_size] * size_adj_factor,
-                               label=key, **plot_kwargs)
+                    ax.scatter(df[key_x], df[key], s=df[key_size] * size_adj_factor, label=key, **plot_kwargs)
                 else:
-                    ax.scatter(df[key_x], df[key],
-                               s=df[key_size] * size_adj_factor,
-                               c=df[key_color],
+                    ax.scatter(df[key_x], df[key], s=df[key_size] * size_adj_factor, c=df[key_color],
                                cmap='jet', label=key, **plot_kwargs)
             else:
                 keys_categorical = df.columns[
                     df.columns.str.contains(key_categorical)]
                 for i_k, key_cat in enumerate(keys_categorical):
                     sub_df = df[df.loc[:, key_cat] == 1]
                     label_str = key_cat.replace(key_categorical + '_', '')
                     c_map = binary_color_maps[i_k + 2]
                     if key_size is None and key_color is None:
-                        ax.scatter(sub_df[key_x], sub_df[key],
-                                   label=label_str, **plot_kwargs)
+                        ax.scatter(sub_df[key_x], sub_df[key], label=label_str, **plot_kwargs)
                     elif key_size is None:
-                        ax.scatter(sub_df[key_x], sub_df[key],
-                                   c=sub_df[key_color], cmap=c_map,
+                        ax.scatter(sub_df[key_x], sub_df[key], c=sub_df[key_color], cmap=c_map,
                                    label=label_str, **plot_kwargs)
                     elif key_color is None:
-                        ax.scatter(sub_df[key_x], sub_df[key],
-                                   s=sub_df[key_size] * size_adj_factor,
+                        ax.scatter(sub_df[key_x], sub_df[key], s=sub_df[key_size] * size_adj_factor,
                                    label=label_str, **plot_kwargs)
                     else:
-                        ax.scatter(sub_df[key_x], sub_df[key],
-                                   s=sub_df[key_size] * size_adj_factor,
-                                   c=sub_df[key_color],
-                                   label=label_str, cmap=c_map,
-                                   **plot_kwargs)
-
-        if ((not isinstance(keys_y, str) or key_categorical is not None)
-                and not plot_only_errors):
-            if key_categorical is not None and 'title' not in \
-                    legend_kwargs.keys():
-                legend_kwargs['title'] = key_categorical.title().replace(
-                    '_', ' ')
+                        ax.scatter(sub_df[key_x], sub_df[key], s=sub_df[key_size] * size_adj_factor,
+                                   c=sub_df[key_color], label=label_str, cmap=c_map, **plot_kwargs)
+
+        if (not isinstance(keys_y, str) or key_categorical is not None) and not plot_only_errors:
+            if key_categorical is not None and 'title' not in legend_kwargs.keys():
+                legend_kwargs['title'] = key_categorical.title().replace('_', ' ')
             legend_1 = ax.legend(**legend_kwargs)
         elif plot_only_errors:
             if 'title' not in legend_kwargs.keys():
                 legend_kwargs['title'] = "Error Source"
             legend_1 = ax.legend(**legend_kwargs)
         else:
             legend_1 = None
 
         if x_label is None:
-            ax.set_xlabel(self.axis_labels[key_x] + ", "
-                          + unit_2_latex(self.units[key_x]))
+            ax.set_xlabel(self.axis_labels[key_x] + ", " + unit_2_latex(self.units[key_x]))
         else:
             ax.set_xlabel(x_label)
         if y_label is None:
-            ax.set_ylabel(self.axis_labels[key_y_single] + ", "
-                          + unit_2_latex(self.units[key_y_single]))
+            ax.set_ylabel(self.axis_labels[key_y_single] + ", " + unit_2_latex(self.units[key_y_single]))
         else:
             ax.set_ylabel(y_label)
 
-        if (key_color is not None and kwargs.get('colorbar', True)
-                and not plot_only_errors):
+        if key_color is not None and kwargs.get('colorbar', True) and not plot_only_errors:
             # Color bar location
             divider = make_axes_locatable(ax)
             cax = divider.append_axes("right", size="5%", pad=0.15)
 
             # Colormap
             if key_categorical is None:
                 cmap = mpl.cm.jet
@@ -1580,29 +1190,24 @@
                 cmap = mpl.cm.binary
             if kwargs.get('clim', False):
                 clim = kwargs.get('clim')
             else:
                 clim = [df[key_color].min(), df[key_color].max()]
             norm = mpl.colors.Normalize(clim[0], clim[1])
 
-            cbar = plt.colorbar(
-                mpl.cm.ScalarMappable(norm=norm, cmap=cmap),
-                cax=cax)
-            cbar.set_label(self.axis_labels[key_color] + ", "
-                           + unit_2_latex(self.units[key_color]))
+            cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap), cax=cax)
+            cbar.set_label(self.axis_labels[key_color] + ", " + unit_2_latex(self.units[key_color]))
 
         if key_size is not None and not plot_only_errors:
             sizes = np.round(np.linspace(df[key_size].min(),
                                          df[key_size].max(), 3))
-            labels = ["{:4.2g}".format(s) for s in sizes]
+            labels = ["{:.3g}".format(s) for s in sizes]
 
-            points = [ax.scatter([], [], s=s * size_adj_factor,
-                                 c='gray') for s in sizes]
-            ax.legend(points, labels, scatterpoints=1,
-                      title=key_size.title().replace('_', ' '), loc=7)
+            points = [ax.scatter([], [], s=s * size_adj_factor, c='gray') for s in sizes]
+            ax.legend(points, labels, scatterpoints=1, title=key_size.title().replace('_', ' '), loc=7)
             if legend_1 is not None:
                 ax.add_artist(legend_1)  # Re-add original legend.
 
         if kwargs.get('xlim', False):
             ax.set_xlim(*kwargs.get('xlim'))
         if kwargs.get('ylim', False):
             ax.set_ylim(*kwargs.get('ylim'))
@@ -1624,16 +1229,15 @@
             ax: plt.Axes = None, title: str = None, x_label: str = None,
             y_label: str = None, legend_kwargs: dict = None,
             plot_raw: bool = False, plot_errors: bool = False,
             plot_only_errors: bool = False,
             plot_kwargs: dict = None, **kwargs
     ) -> (plt.Figure, Tuple[Tuple[plt.Axes]], List[DataSet]):
         """Plot a collection of 2d line plot for an x and y value property set.
-        Key value proposition of the function is the alignment of plots and
-        unification of axis limits.
+        Key value proposition of the function is the alignment of plots and unification of axis limits.
 
         Parameters
         ----------
         key_x
             X-axis value key
 
         keys_y
@@ -1642,29 +1246,26 @@
         key_categorical: optional, default = None
             Categorical key to split the plotting over. E.g. fuel.
 
         key_size: optional, default = None
             Marker size value key
 
         key_color: optional, default = None
-            Marker color value key. If a categorical key is given,
-            each color gets a monotone color gradient.
+            Marker color value key. If a categorical key is given, each color gets a monotone color gradient.
 
         size_adj_factor: optional, default = 1.0
             Linear scaling factor on the marker size if a key_size is given.
 
         key_multiplot: optional, default = None
             Key to differentiate dataset for each sub-plot
 
         multiplot_set: optional, default = None
-            Differentiation of the multiplot key. This is optional if
-            key_multiplot is None or is a categorical value. In this case,
-            as many plots are created as there are values. If the
-            key_multiplot data is continuous, the multiplot_set can be an
-            integer, which defines how many plots are created or a vector
+            Differentiation of the multiplot key. This is optional if key_multiplot is None or is a categorical
+            value. In this case, as many plots are created as there are values. If the key_multiplot data is
+            continuous, the multiplot_set can be an integer, which defines how many plots are created or a vector
             array which more closely defines
 
         ax: optional, default = None
             Optionally pass an existing Axes to plot to same figure.
 
         title: optional, default = None
             Manually set plot title.
@@ -1675,115 +1276,94 @@
         y_label: optional, default = None
             Manually set y-axis label
 
         legend_kwargs: optional, default = None
             Dictionary of keyword argument to pass to the legend command.
 
         plot_raw: optional, default = False
-            Bool flag whether the raw data should be plotted beneath the
-            target date. Data is plotted in grey.
+            Bool flag whether the raw data should be plotted beneath the target date. Data is plotted in grey.
 
         plot_errors: optional, default = False
-            Bool flag whether the error data should be plotted beneath the
-            target date. Data is plotted in red.
+            Bool flag whether the error data should be plotted beneath the target date. Data is plotted in red.
 
         plot_only_errors: optional, default = False
             Bool flag whether only the error data should be plotted.
 
         plot_kwargs: Optional
             Plot key word arguments passed to the plotting function.
 
         kwargs: Optional
-            Keyword arguments used for additional plot adjustment,
-            e.g. disabling the color bar with colorbar=False, xlim, clim, ylim
+            Keyword arguments used for additional plot adjustment, e.g. disabling the color bar with colorbar=False,
+            xlim, clim, ylim
 
         See Also
         --------
         DataSet.plot_2d
         """
         if key_multiplot is None:
             fig, axes = self.plot_2d(
-                key_x, keys_y, key_categorical, key_size, key_color,
-                size_adj_factor, ax, title, x_label, y_label,
-                legend_kwargs,
-                None, plot_raw, plot_errors, plot_only_errors,
-                plot_kwargs, **kwargs)
+                key_x, keys_y, key_categorical, key_size, key_color, size_adj_factor, ax, title, x_label, y_label,
+                legend_kwargs, None, plot_raw, plot_errors, plot_only_errors, plot_kwargs, **kwargs)
             datasets = [self]
         else:
             if plot_kwargs is None:
                 plot_kwargs = {}
 
             datasets = self.get_split_dataset(key_multiplot, multiplot_set)
             n_plots = len(datasets)
 
             n_plots_minor = int(np.floor(np.sqrt(n_plots)))
             n_plots_major = int(np.ceil(n_plots / n_plots_minor))
             fig, axes = plt.subplots(n_plots_minor, n_plots_major)
 
             axes_1d = axes.reshape(-1)
             df = self.df
-            xlim = kwargs.get('xlim', [df.loc[:, key_x].min(),
-                                       df.loc[:, key_x].max()])
-            ylim = kwargs.get('ylim', [df.loc[:, keys_y].min(),
-                                       df.loc[:, keys_y].max()])
+            xlim = kwargs.get('xlim', [df.loc[:, key_x].min(), df.loc[:, key_x].max()])
+            ylim = kwargs.get('ylim', [df.loc[:, keys_y].min(), df.loc[:, keys_y].max()])
             if kwargs.get('clim', None) is None:
                 if key_color is not None:
-                    clim = [df.loc[:, key_color].min(),
-                            df.loc[:, key_color].max()]
+                    clim = [df.loc[:, key_color].min(), df.loc[:, key_color].max()]
                     norm = mpl.colors.Normalize(clim[0], clim[1])
                 else:
                     clim = False
                     norm = None
             else:
                 clim = kwargs.get('clim')
                 norm = mpl.colors.Normalize(clim[0], clim[1])
-            kwargs.update({'xlim': xlim, 'ylim': ylim, 'clim': clim,
-                           'colorbar': False})
+            kwargs.update({'xlim': xlim, 'ylim': ylim, 'clim': clim, 'colorbar': False})
             plot_kwargs.update({'norm': norm})
 
             for i in range(n_plots):
                 if plot_only_errors:
-                    # Assumes the subset filter was added last in line.
-                    # Typically true.
-                    alternate_df = {
-                        'df_errors': datasets[i].df_errors.query(
-                            datasets[i].filter_list[-1]),
-                        'df_raw': datasets[i].raw_df.query(
-                            datasets[i].filter_list[-1])}
+                    # Assumes the subset filter was added last in line. Typically true.
+                    alternate_df = {'df_errors': datasets[i].df_errors.query(datasets[i].filter_list[-1]),
+                                    'df_raw': datasets[i].raw_df.query(datasets[i].filter_list[-1])}
                 else:
                     alternate_df = datasets[i].df
 
                 # Simplify title for categorical splits
                 if isinstance(datasets[i].filter_list, list):
                     sub_title = datasets[i].filter_list[-1]
                 else:
                     sub_title = datasets[i].filter_list
-                sub_cat = [k for k in self.keys_categorical
-                           if k + " == " in sub_title]
+                sub_cat = [k for k in self.keys_categorical if k + " == " in sub_title]
                 if len(sub_cat) > 0:
-                    sub_title = sub_title.replace(
-                        sub_cat[0] + " == ", "").replace('"', '')
+                    sub_title = sub_title.replace(sub_cat[0] + " == ", "").replace('"', '')
 
-                self.plot_2d(key_x, keys_y, key_categorical, key_size,
-                             key_color, size_adj_factor, axes_1d[i],
-                             sub_title, x_label, y_label,
-                             legend_kwargs, alternate_df, plot_raw,
-                             plot_errors, plot_only_errors,
-                             plot_kwargs, **kwargs)
+                self.plot_2d(key_x, keys_y, key_categorical, key_size, key_color, size_adj_factor, axes_1d[i],
+                             sub_title, x_label, y_label, legend_kwargs, alternate_df, plot_raw, plot_errors,
+                             plot_only_errors, plot_kwargs, **kwargs)
 
             if title is not None:
                 plt.suptitle(title)
 
             fig.tight_layout()  # Before color bar
 
             if key_color is not None:
                 if key_categorical is None:
                     cmap = mpl.cm.jet
                 else:
                     cmap = mpl.cm.binary
-                cbar = plt.colorbar(
-                    mpl.cm.ScalarMappable(norm=norm, cmap=cmap),
-                    ax=axes.ravel().tolist(), shrink=0.95)
-                cbar.set_label(self.axis_labels[key_color] + ", "
-                               + unit_2_latex(self.units[key_color]))
+                cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap), ax=axes.ravel().tolist(), shrink=0.95)
+                cbar.set_label(self.axis_labels[key_color] + ", " + unit_2_latex(self.units[key_color]))
         return fig, axes, datasets
     # endregion
```

### Comparing `cetpy-0.1.0b5/cetpy/Configuration/_ConfigurationManager.py` & `cetpy-0.1.0b6/cetpy/Configuration/_ConfigurationManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 """
 Configuration Manager
 =====================
 
-This file defines a Configuration Manager for CET. The manager handles the
-interface to the .toml config files, layering of config files,
-and traceability.
+This file defines a Configuration Manager for CET. The manager handles the interface to the .toml config files,
+layering of config files, and traceability.
 """
 
 from os import listdir
 from os.path import join, isdir, isfile, abspath, dirname
 from typing import List
 import pandas as pd
 import numpy as np
 import pickle
 import tomli
 
 import cetpy
 import cetpy.Configuration
 
 
-def get_absolute_path(file_path: str, additional_locations: List[str] = None
-                      ) -> str:
+def get_absolute_path(file_path: str, additional_locations: List[str] = None) -> str:
     """Return absolute path of a file within the CET config structure.
 
-    A valid absolute path is prioritised above all else. Second the
-    additional locations in order of occurrence, and lastly the CET config
-    locations from cetpy.Configurations in order of occurrence.
+    A valid absolute path is prioritised above all else. Second the additional locations in order of occurrence,
+    and lastly the CET config locations from cetpy.Configurations in order of occurrence.
     """
-    if file_path[-5:] != '.toml':
-        file_path = file_path + '.toml'
     if isfile(abspath(file_path)):
         return abspath(file_path)
     else:
-        for location in (additional_locations +
-                         cetpy.Configuration.config_locations):
+        for location in (additional_locations + cetpy.Configuration.config_locations):
             abs_path = join(location, file_path)
             if isfile(abs_path):
                 return abs_path
 
 
+def get_absolute_config_path(file_path: str, additional_locations: List[str] = None) -> str:
+    """Return absolute path of a config file within the CET config structure.
+
+    Adds .toml to file path if not already present.
+
+    See Also
+    --------
+    get_absolute_path: independent of file ending
+    """
+    if file_path[-5:] != '.toml':
+        file_path = file_path + '.toml'
+    return get_absolute_config_path(file_path, additional_locations=additional_locations)
+
+
 def load_config(file_path: str) -> dict:
     """Return dictionary fitting to a TOML file at the specified location."""
     try:
         with open(file_path, "rb") as f:
             return tomli.load(f)
     except tomli.TOMLDecodeError:
         return {}  # Empty config.
@@ -52,18 +60,17 @@
                      ) -> dict:
     """Parse a config dictionary to load numpy, pickle, or csv files."""
     if additional_locations is None:
         additional_locations = []
     out = config.copy()
     for key in out.keys():
         if isinstance(out[key], dict) and 'file' in out[key].keys():
-            match out[key]['file'][-3:]:
-                case 'csv':
-                    out[key] = pd.read_csv(get_absolute_path(
-                        out[key]['file'], additional_locations))
+            match out[key]['file'][-4:]:
+                case '.csv':
+                    out[key] = pd.read_csv(get_absolute_path(out[key]['file'], additional_locations))
                 case '.pkl':
                     with open(out[key]['file'], "rb") as f:
                         out[key] = pickle.load(f)
                 case '.txt':
                     out[key] = np.loadtxt(out[key]['file'])
                 case _:
                     pass
@@ -71,25 +78,22 @@
             out[key] = interpret_config(out[key], additional_locations)
         elif isinstance(out[key], str) and out[key] in ['none', 'None']:
             out[key] = None
     return out
 
 
 def get_parameter_dict() -> dict:
-    """Return parameter dict incorporating all possible parameters
-    across all model elements."""
-    out = load_config(
-        join(dirname(__file__), 'default_config_parameters.toml'))
+    """Return parameter dict incorporating all possible parameters across all model elements."""
+    out = load_config(join(dirname(__file__), 'default_config_parameters.toml'))
 
     def load_parameters_from_dir(file_path: str) -> dict:
         target_dict = {}
         for item in listdir(file_path):
             if isdir(join(file_path, item)):
-                sub_dict = load_parameters_from_dir(
-                    join(file_path, item))
+                sub_dict = load_parameters_from_dir(join(file_path, item))
                 if len(sub_dict) > 0:
                     target_dict[item.lower()] = sub_dict
             if isfile(join(file_path, item)) and item[-5:] == '.toml':
                 target_dict.update(load_config(join(file_path, item)))
         return target_dict
 
     for loc in cetpy.Configuration.module_locations:
@@ -105,26 +109,25 @@
             out[key] = value['default']
         elif isinstance(value, dict):
             out[key] = get_default_dict(value)
     return out
 
 
 def get_config_keys(config: dict) -> List[str]:
-    """Return list of all value keys in the config, split by a dot,
-    as would be the case in a config file."""
+    """Return list of all value keys in the config, split by a dot, as would be the case in a config file."""
     keys = list(config.keys())
     for key, val in config.items():
         if isinstance(val, dict):
             keys += [key + '.' + k for k in get_config_keys(val)]
     return keys
 
 
 def get_parameter(config: dict, key: str | List[str]):
-    """Return the parameter value from a config dictionary using either the
-    chained name (table headers split by a '.') or a list of keys."""
+    """Return the parameter value from a config dictionary using either the chained name
+    (table headers split by a '.') or a list of keys."""
     if isinstance(key, str):
         key = key.split('.')
     val = config[key[0]]
     if len(key) > 1:
         return get_parameter(val, key[1:])
     else:
         return val
@@ -150,73 +153,65 @@
     elif isinstance(value, str):
         return "'" + value + "'"
     elif isinstance(value, list):
         return "[" + ",".join([format_value_to_toml(v) for v in value]) + "]"
     elif isinstance(value, dict):
         return "{" + ",".join([f"{k} = {v}" for k, v in value.items()]) + "}"
     else:
-        raise ValueError(
-            f"Value type could not be converted to toml: {type(value)}")
+        raise ValueError(f"Value type could not be converted to toml: {type(value)}")
 
 
 def format_config_key(key: str, value, parameter_entry: dict) -> List[str]:
     """Format the table header of a config file"""
     value = format_value_to_toml(value)
     lines = [key + ' = ' + value]
     match parameter_entry.get('type', None), parameter_entry.get('unit', None):
         case None, None:
             pass
         case _, None:
             lines += ["(" + parameter_entry['type'] + ")"]
         case None, _:
             lines += ["[" + parameter_entry['unit'] + "]"]
         case _, _:
-            lines += ["(" + parameter_entry['type'] + ") ["
-                      + parameter_entry['unit'] + "]"]
+            lines += ["(" + parameter_entry['type'] + ") [" + parameter_entry['unit'] + "]"]
         case _:
             pass
 
     lines += [parameter_entry['description']]
     return lines
 
 
-def format_toml_body_text(default_dict: dict, parameter_dict: dict,
-                          table_master_level: list = None) -> List[str]:
+def format_toml_body_text(default_dict: dict, parameter_dict: dict, table_master_level: list = None) -> List[str]:
     """Format the body text of a TOML config file."""
     if table_master_level is None:
         table_master_level = []
     lines = []
 
-    keys_values = [key for key, value in default_dict.items()
-                   if not isinstance(value, dict)]
-    keys_sub_keys = [key for key in default_dict.keys() if key not in
-                     keys_values]
+    keys_values = [key for key, value in default_dict.items() if not isinstance(value, dict)]
+    keys_sub_keys = [key for key in default_dict.keys() if key not in keys_values]
     for key in keys_values:
-        lines += format_config_key(
-            key, default_dict[key], parameter_dict[key])
+        lines += format_config_key(key, default_dict[key], parameter_dict[key])
     lines += ["\n\n"]
 
     for key in keys_sub_keys:
         table_sub_level = table_master_level + [key]
         lines += format_config_table_header(table_sub_level)
         parameter_sub_dict = parameter_dict[key]
         default_sub_dict = default_dict[key]
-        lines += format_toml_body_text(default_sub_dict, parameter_sub_dict,
-                                       table_sub_level)
+        lines += format_toml_body_text(default_sub_dict, parameter_sub_dict, table_sub_level)
     return lines
 
 
 class ConfigurationManager:
     """CET Config Manger for loading, layering, and tracing configs."""
 
     __slots__ = ['_parameter_dict', '_config', '_configs', '_config_keys',
                  '_directory', '_session_config_name']
 
-    def __init__(self, directory: str | None = None,
-                 session_config: str | None = None) -> None:
+    def __init__(self, directory: str | None = None, session_config: str | None = None) -> None:
         self._parameter_dict = {}
         self._config = {}
         self._configs = {}
         self._config_keys = []
         self.session_config_name = session_config
         self.directory = directory
 
@@ -290,77 +285,67 @@
     def __get_config__(self, file_path: str) -> dict:
         """Return dictionary fitting to a TOML file at the specified location
         while finding a relevant config in the CET config structure."""
         abs_path = self.__get_abs_path__(file_path)
         if abs_path is not None:
             return load_config(abs_path)
         else:
-            raise ValueError(f"Config File could not be found. "
-                             f"Config Path: {file_path}")
+            raise ValueError(f"Config File could not be found. Config Path: {file_path}")
 
-    def __load_config_amendment__(self, config: dict,
-                                  config_dict: dict = None,
-                                  allow_user_directory: bool = True
-                                  ) -> dict:
+    def __load_config_amendment__(self, config: dict, config_dict: dict = None,
+                                  allow_user_directory: bool = True) -> dict:
         """Overload a config with its stated amendments."""
         config_in = config.copy()
         if 'config_amendment' in config.keys():
             config_amendment = config_in['config_amendment']
             if not isinstance(config_amendment, list):
                 config_amendment = [config_amendment]
             for cam in config_amendment:
                 if allow_user_directory:
                     config_add = self.__get_config__(cam)
                 else:
-                    config_add = load_config(get_absolute_path(cam))
-                # Add config to list first, to preserve initial state
-                # and prioritisation.
+                    config_add = load_config(get_absolute_config_path(cam))
+                # Add config to list first, to preserve initial state and prioritisation.
                 if config_dict is not None:
                     config_dict[cam] = config_add.copy()
-                config_add = self.__load_config_amendment__(
-                    config_add, config_dict, allow_user_directory)
+                config_add = self.__load_config_amendment__(config_add, config_dict, allow_user_directory)
                 config_add.update(config_in)  # Prioritise config_in
                 config_in = config_add
             config_in.pop('config_amendment', None)
         return config_in
 
     def load(self) -> None:
         """Load the configuration at the specified directory."""
         # Always start from zero for a clean load.
         # region Default Config
         config = self.default_dict_raw
         self._configs = {'default': config.copy()}
-        self._config = self.__load_config_amendment__(
-            config, self._configs, False)
+        self._config = self.__load_config_amendment__(config, self._configs, False)
         # endregion
 
         # region Session Config
         if self.directory is not None:
             config = self.__get_config__(self.session_config_name)
             self._configs['session'] = config.copy()
-            self._config.update(self.__load_config_amendment__(
-                config, self._configs, True))
+            self._config.update(self.__load_config_amendment__(config, self._configs, True))
 
         self._config = interpret_config(self._config, [self.directory])
         # endregion
 
         self._config_keys = get_config_keys(self.config)
 
     def write_session_config_template(self, file_path: str = None) -> None:
-        """Write template for the session config. The session config
-        documents the available options with all installed modules, units,
-        acceptable inputs, and parameter descriptions."""
+        """Write template for the session config. The session config documents the available options with all
+        installed modules, units, acceptable inputs, and parameter descriptions."""
         directory = self.directory
         if directory is None and file_path is None:
-            raise ValueError("The config manager needs a defined directory "
-                             "to write the session config template.")
+            raise ValueError("The config manager needs a defined directory to write the session config template.")
         if file_path is None and isfile(
                 join(directory, 'session_config.toml')):
-            raise FileExistsError("Session config already exists. Delete "
-                                  "this file first before writing again.")
+            raise FileExistsError("Session config already exists. Delete this file first before writing again.")
         if file_path is None:
             file_path = join(directory, 'session_config.toml'),
 
         # region Write Text
         lines = format_config_header(
             "Congruent Engineering Toolbox Session Config")
         lines += format_toml_body_text(
```

### Comparing `cetpy-0.1.0b5/cetpy/Configuration/_ModuleManager.py` & `cetpy-0.1.0b6/cetpy/Configuration/_ModuleManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 """
 Module Manager
 ==============
 
-This file defines function to aggregate a list of modules used in cetpy and
-extension modules. It pulls from the cetpy.Configuration module_location
-list and aggregates all modules deriving from the base SysML Block class.
+This file defines function to aggregate a list of modules used in cetpy and extension modules. It pulls from the
+cetpy.Configuration module_location list and aggregates all modules deriving from the base SysML Block class.
 """
 import sys
 import pkgutil
 import os.path
 from types import ModuleType
 from typing import Dict
+import numpy as np
 
 
 import cetpy
 import cetpy.Configuration
 from cetpy.Modules.SysML import Block
 
 
 def get_module(name: str) -> cetpy.Modules.SysML.Block:
-    """Find and return a module based on its base name from the blocks in
-    the module locations of the cetpy configuration."""
+    """Find and return a module based on its base name from the blocks in the module locations of the cetpy
+    configuration."""
     return cetpy.Configuration.module_dict[name]
 
 
 def generate_block_class_list() -> Dict[str, Block]:
-    """Return dictionary of all Block derived classes in across cetpy and
-    extension modules."""
+    """Return dictionary of all Block derived classes in across cetpy and extension modules."""
     blocks = {}
     for location in cetpy.Configuration.module_locations:
         location = os.path.abspath(location)
-        # The issue here is that the location, while on the OS path, can be
-        # n-levels deep in this path. So we must strip out the overlap
-        # between the path entry and the module locations. Finally, we must
-        # swap out the directory separators for '.' package separators.
-        overlap = [p for p in sys.path if p in location and p != ''][-1]
-        location_new = location.replace(overlap, '').replace(
-            os.path.sep, '.')[1:]
+        # The issue here is that the location, while on the OS path, can be n-levels deep in this path. So we must
+        # strip out the overlap between the path entry and the module locations. Finally, we must swap out the
+        # directory separators for '.' package separators.
+        overlaps = [p for p in sys.path if p in location and p != '']
+        if len(overlaps) == 1:
+            overlap = overlaps[-1]
+        else:
+            idx = np.argmax([len(o) for o in overlaps])
+            overlap = overlaps[idx]
+        location_new = location.replace(overlap, '').replace(os.path.sep, '.')[1:]
 
         module_instance = get_submodule_instance(location_new)
 
-        # Verify that the correct module was loaded, also important for
-        # security.
+        # Verify that the correct module was loaded, also important for security.
         if module_instance.__path__[0] != location:
-            raise ValueError(f"The path match failed on the module locations. "
-                             f"The desired import path was {location}, "
-                             f"the attempted match resulted in "
-                             f"{module_instance.__path__[0]}.")
+            raise ValueError(f"The path match failed on the module locations. The desired import path was {location}, "
+                             f"the attempted match resulted in {module_instance.__path__[0]}.")
 
         blocks.update(get_module_recursive_classes(module_instance))
     return blocks
 
 
 def get_module_recursive_classes(ref_module: ModuleType) -> Dict[str, Block]:
     """Return dictionary of name and type of all classes in a module.
@@ -69,19 +68,17 @@
     for c in module_dict:
         if isinstance(module_dict[c], type) and Block in module_dict[c].mro():
             blocks.update({c: module_dict[c]})
     return blocks
 
 
 def get_submodules(ref_module: ModuleType) -> Dict[str, ModuleType]:
-    """Return dictionary of name and Module Instance of all submodules of a
-    module."""
+    """Return dictionary of name and Module Instance of all submodules of a module."""
     mod_list = list([
-        i for i in pkgutil.iter_modules(ref_module.__path__,
-                                        prefix=ref_module.__name__ + '.')
+        i for i in pkgutil.iter_modules(ref_module.__path__, prefix=ref_module.__name__ + '.')
         if i.ispkg])
     modules = {}
     for submodule in mod_list:
         submodule_instance = get_submodule_instance(submodule.name)
         modules.update({submodule.name: submodule_instance})
 
     return modules
```

### Comparing `cetpy-0.1.0b5/cetpy/Configuration/_Session.py` & `cetpy-0.1.0b6/cetpy/Configuration/_Session.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Configuration/__init__.py` & `cetpy-0.1.0b6/cetpy/Configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from os.path import dirname, join
 
 from cetpy.Configuration._ConfigurationManager import ConfigurationManager
 from cetpy.Configuration._Session import Session
-from cetpy.Configuration._ModuleManager import \
-    generate_block_class_list, get_module
+from cetpy.Configuration._ModuleManager import generate_block_class_list, get_module
 
 config_locations = [join(dirname(__file__), 'Configurations')]
 module_locations = [join(dirname(__file__), '..', 'Modules')]
 module_dict = {}
 
 
 def refresh_module_dict() -> None:
```

### Comparing `cetpy-0.1.0b5/cetpy/Configuration/default_session_config.toml` & `cetpy-0.1.0b6/cetpy/Configuration/default_session_config.toml`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Fluid/_FluidCoolProp.py` & `cetpy-0.1.0b6/cetpy/Modules/Fluid/_FluidCoolProp.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Fluid/_FluidSkeleton.py` & `cetpy-0.1.0b6/cetpy/Modules/Fluid/_FluidSkeleton.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_CompressibleFluidBlock.py` & `cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_CompressibleFluidBlock.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_FluidBlock.py` & `cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_FluidBlock.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_FluidPort.py` & `cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_FluidPort.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/FluidBlock/_GenericFluidBlock.py` & `cetpy-0.1.0b6/cetpy/Modules/FluidBlock/_GenericFluidBlock.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Material/_MaterialGiven.py` & `cetpy-0.1.0b6/cetpy/Modules/Material/_MaterialGiven.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Material/_MaterialSkeleton.py` & `cetpy-0.1.0b6/cetpy/Modules/Material/_MaterialSkeleton.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Report/_Report.py` & `cetpy-0.1.0b6/cetpy/Modules/Report/_Report.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Report/_ReportPort.py` & `cetpy-0.1.0b6/cetpy/Modules/Report/_ReportPort.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Report/_ReportSolver.py` & `cetpy-0.1.0b6/cetpy/Modules/Report/_ReportSolver.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Solver/_ContinuousFlowSolver.py` & `cetpy-0.1.0b6/cetpy/Modules/Solver/_ContinuousFlowSolver.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Solver/_Solver.py` & `cetpy-0.1.0b6/cetpy/Modules/Solver/_Solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Generic Decentralised Solver
 ============================
 
-This file specifies the base Solver class which defines the base structure
-of the decentralised solver architecture.
+This file specifies the base Solver class which defines the base structure of the decentralised solver architecture.
 """
 
 from __future__ import annotations
 
 from typing import List, Any, Dict
 from copy import deepcopy
+from time import perf_counter
 
 from cetpy.Modules.SysML import ValuePrinter
 from cetpy.Modules.Report import ReportSolver
 
 
 class Solver:
     """Decentralised Solver of the Congruent Engineering Toolbox."""
 
-    __slots__ = ['_recalculate', '_calculating', '_hold', '_resetting',
-                 '_parent', '_tolerance', 'report', '_last_input']
+    __slots__ = ['_recalculate', '_calculating', '_hold', '_resetting', '_parent', '_tolerance', 'report',
+                 '_last_input']
 
     print = ValuePrinter()
 
     input_keys: List[str] = []
     convergence_keys: List[str] = []
     _reset_dict: Dict[str, Any] = {}
 
@@ -44,14 +44,19 @@
     # region System References
     @property
     def name(self) -> str:
         """Solver name."""
         return type(self).__name__
 
     @property
+    def long_name(self) -> str:
+        """Solver name with owning block name."""
+        return self.parent.name_display + ' ' + self.name
+
+    @property
     def parent(self):
         """Solver owner block."""
         return self._parent
 
     @parent.setter
     def parent(self, val) -> None:
         val_initial = self._parent
@@ -108,55 +113,49 @@
 
     def __deep_getattr__(self, name: str) -> Any:
         """Get value from block or its parts, solvers, and ports."""
         if '.' not in name:
             return self.__getattribute__(name)
         else:
             name_split = name.split('.')
-            return self.__getattribute__(name_split[0]).__deep_getattr__(
-                '.'.join(name_split[1:]))
+            return self.__getattribute__(name_split[0]).__deep_getattr__('.'.join(name_split[1:]))
 
     def __deep_setattr__(self, name: str, val: Any) -> None:
         """Set value on block or its parts, solvers, and ports."""
         if '.' not in name:
             return self.__setattr__(name, val)
         else:
             name_split = name.split('.')
-            self.__getattribute__(name_split[0]).__deep_setattr__(
-                '.'.join(name_split[1:]), val)
+            self.__getattribute__(name_split[0]).__deep_setattr__('.'.join(name_split[1:]), val)
 
     def __deep_get_vp__(self, name: str) -> Any:
         """Get value property from block or its parts, solvers, and ports."""
         if '.' not in name:
             return getattr(type(self), name)
         else:
             name_split = name.split('.')
-            return self.__getattribute__(name_split[0]).__deep_get_vp__(
-                '.'.join(name_split[1:]))
+            return self.__getattribute__(name_split[0]).__deep_get_vp__('.'.join(name_split[1:]))
     # endregion
 
     # region Solver Flags
     @property
     def solved(self) -> bool:
         """Return bool if the solver is solved.
 
-        If the recalculate flag is True and input keys are specified the
-        function further calls Solver.necessary to perform an additional
-        check if a resolve is actually necessary using the last stored solve
-        input parameters.
+        If the recalculate flag is True and input keys are specified the function further calls Solver.necessary to
+        perform an additional check if a resolve is actually necessary using the last stored solve input parameters.
         """
         return not self._recalculate or not self.necessary
 
     # region Necessity Test
     @property
     def necessary(self) -> bool:
-        """Return bool if a rerun in necessary. If no input keys are
-        specified, the function always returns True as it cannot verify the
-        inputs are still the same. The solved check still prioritises the
-        recalculate flag set by the post_solver."""
+        """Return bool if a rerun in necessary. If no input keys are specified, the function always returns True as
+        it cannot verify the inputs are still the same. The solved check still prioritises the recalculate flag set
+        by the post_solver."""
         input_keys = self.input_keys
         last_input = self._last_input
         if len(input_keys) == 0 or len(last_input) == 0:
             return True
         for val_last, key in zip(last_input, input_keys):
             vp = self.__deep_get_vp__(key)
             val_new = self.__deep_getattr__(key)
@@ -169,23 +168,21 @@
 
     def __get_input__(self) -> list:
         """Pull and return all current input properties."""
         return [self.__deep_getattr__(k) for k in self.input_keys]
 
     def __get_input_sensitivity__(self) -> List[float]:
         """Pull and return all current input properties."""
-        return [self.__deep_get_vp__(k).necessity_test
-                for k in self.input_keys]
+        return [self.__deep_get_vp__(k).necessity_test for k in self.input_keys]
 
     def _write_last_input(self) -> None:
         """Write current input properties to _last_input attribute.
 
-        This function is called as part of the pre-run. It's recommended
-        that if the solver is recursive, the function is also called once at
-        the start of every solver loop.
+        This function is called as part of the pre-run. It's recommended that if the solver is recursive,
+        the function is also called once at the start of every solver loop.
         """
         self._last_input = self.__get_input__()
     # endregion
 
     @property
     def calculating(self) -> bool:
         """Return bool if the solver is currently running."""
@@ -194,17 +191,16 @@
     @property
     def solved_calculating(self) -> bool:
         """Return bool if the solver is solved or currently running."""
         return self.solved or self.calculating
 
     @property
     def hold(self) -> bool:
-        """Current hold status. Hold enables an additional user input to
-        enable and disable the automatic run of individual solvers. The hold is
-        stored as an integer enabling nested holds throughout the system.
+        """Current hold status. Hold enables an additional user input to enable and disable the automatic run of
+        individual solvers. The hold is stored as an integer enabling nested holds throughout the system.
 
         See Also
         --------
         Solver.raise_hold
         Solver.lower_hold
         """
         return bool(self._hold)
@@ -219,23 +215,29 @@
 
     def lower_hold(self) -> None:
         """Lower the hold level by one."""
         self._hold += 1
 
     def force_solve(self) -> None:
         """Run the solver, regardless of the current solver state."""
-        self._solve()
-        # ToDo: Add timing and logging.
+        if self.parent.__detailed_debug__:
+            name = self.long_name
+            logger = self.parent.__logger__
+            logger.debug(f"Starting {name}.")
+            t1 = perf_counter()
+            self._solve()
+            logger.debug(f"Finished {name} in {perf_counter() - t1} s.")
+        else:
+            self._solve()
 
     def solve(self) -> None:
         """Run the solver if necessary and allowed.
 
-        The solver will run if the solver is not already solved, the
-        solver is not currently already running, and the solver does not
-        currently have an enabled hold condition.
+        The solver will run if the solver is not already solved, the solver is not currently already running,
+        and the solver does not currently have an enabled hold condition.
         """
         if not self.solved_calculating and not self.hold:
             self.force_solve()
     # endregion
 
     # region Solver Functions
     def _pre_solve(self) -> None:
@@ -249,16 +251,15 @@
 
     def _post_solve(self) -> None:
         """Conduct standardised post-run of the solver."""
         self._calculating = False
         self._recalculate = False
 
     def _solve(self) -> None:
-        """Private solve function combining the pre-, core-, and post-solve
-        functions."""
+        """Private solve function combining the pre-, core-, and post-solve functions."""
         self._pre_solve()
         self._solve_function()
         self._post_solve()
     # endregion
 
     # region Input Properties
     @property
```

### Comparing `cetpy-0.1.0b5/cetpy/Modules/SysML/_Block.py` & `cetpy-0.1.0b6/cetpy/Modules/SysML/_Block.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,62 +22,53 @@
 from cetpy.Modules.Solver import Solver
 from cetpy.Modules.Report import Report
 
 
 class Block:
     """SysML Block element.
 
-    This is the basic system block of SysML. It can contain parts,
-    themselves Blocks. It can contain ports, which handle interfaces to
-    other elements. The block can also contain references to solvers,
-    which are a product of cetpy, not SysML, that handle a decentralised
-    solver architecture for any slow computations.
-
-    This base class contains functions that handle initialisation, loading
-    from config files and keyword arguments, attach a session logger,
-    and create sub parts according to model definitions.
+    This is the basic system block of SysML. It can contain parts, themselves Blocks. It can contain ports,
+    which handle interfaces to other elements. The block can also contain references to solvers, which are a product
+    of cetpy, not SysML, that handle a decentralised solver architecture for any slow computations.
+
+    This base class contains functions that handle initialisation, loading from config files and keyword arguments,
+    attach a session logger, and create sub parts according to model definitions.
     """
 
-    __slots__ = ['_resetting', 'name', 'abbreviation', '_parent',
-                 '_tolerance', '_logger',
-                 'parts', 'ports', 'requirements', 'solvers',
-                 '_get_init_parameters', '__init_kwargs__', '__dict__']
+    __slots__ = ['_resetting', 'name', 'abbreviation', '_parent', '_tolerance', '_logger', 'parts', 'ports',
+                 'requirements', 'solvers', '_get_init_parameters', '__init_kwargs__', '__dict__']
 
     __init_parameters__: List[str] = []
     __init_parts__: List[str] = []
     _reset_dict: Dict[str, Any] = {}
     _hard_reset_dict: Dict[str, Any] = {}
     __fixed_parameters__: List[str] = []
     __default_parameters__: Dict[str, Any] = {}
     _bool_parent_reset = True
+    __detailed_debug__ = False
 
     print = ValuePrinter()
 
     def __init__(self, name: str, abbreviation: str = None,
                  parent: Block = None, tolerance: float = None, **kwargs
                  ) -> None:
         """Initialise a Block instance.
 
         Parameters
         ----------
         name
-            A name for the block, used for visualizations, reports,
-            and other user output.
+            A name for the block, used for visualizations, reports, and other user output.
         abbreviation: optional
-            A shortened abbreviation of the name that can also be used for
-            output functions where a long-name would be a prohibitive
-            identifier. If none is given, the block predicts a sensible
-            abbreviation.
+            A shortened abbreviation of the name that can also be used for output functions where a long-name would
+            be a prohibitive identifier. If none is given, the block predicts a sensible abbreviation.
         parent: optional
-            Another block, which is to contain this block as a part. The
-            bidirectional connection is made automatically.
+            Another block, which is to contain this block as a part. The bidirectional connection is made automatically.
         tolerance: optional
-            A general tolerance for the block, its solvers, ports,
-            and parts. If None is provided, takes the tolerance of the
-            parent if available or from the active session configuration.
+            A general tolerance for the block, its solvers, ports, and parts. If None is provided, takes the
+            tolerance of the parent if available or from the active session configuration.
         """
         # region Logging
         if cetpy.active_session is not None:
             self._logger = cetpy.active_session.logger
         else:
             self._logger = None
         # endregion
@@ -125,39 +116,35 @@
         type_name = str(type(self))
 
         parameter_strings = [
             '.'.join(parent_names[i:]) for i in range(-len(parent_names), 0)
             ] + [
             '.'.join(class_names[i:]) for i in range(-len(class_names), 0)
             ] + [
-            '.'.join(type_name[
-                     type_name.find('Modules') + 8:-2].split('.')[:-2]).lower()
+            '.'.join(type_name[type_name.find('Modules') + 8:-2].split('.')[:-2]).lower()
         ]
 
         config_keys = cetpy.active_session.config_manager.config_keys
 
         def get_key_strings(key_in: str) -> List[str]:
             """Return joined parameter strings with the key attached.
 
             Strings are sorted in order of complexity.
             """
             return [ps + '.' + key_in for ps in parameter_strings] + [key_in]
 
         def get_key_in_kwargs(key_in: str) -> List[str]:
-            """Return joined key strings which are present in the keyword
-            arguments."""
+            """Return joined key strings which are present in the keyword arguments."""
             key_strings = get_key_strings(key_in)
-            return [k.replace('.', '_') for k in key_strings
-                    if k.replace('.', '_') in kwargs.keys()]
+            return [k.replace('.', '_') for k in key_strings if k.replace('.', '_') in kwargs.keys()]
 
         def get_key_in_config(key_in: str) -> List[str]:
             """Return joined key strings which are present in the configs."""
             key_strings = get_key_strings(key_in)
-            return [k.replace('.', '_') for k in key_strings
-                    if k.replace('.', '_') in config_keys]
+            return [k.replace('.', '_') for k in key_strings if k.replace('.', '_') in config_keys]
 
         def parameter(key_in: str):
             """Return parameter setting for a given key with prioritisation.
 
             Source Prioritisation:
             1. kwargs
             2. session config
@@ -176,60 +163,53 @@
 
                 1. mandalore.concordia.radius
                 2. concordia.radius
                 3. Planet.Moon.radius
                 4. Moon.radius
                 5. radius
 
-            Please note, for comparison all '.' separators are
-            replaced by '_'.
+            Please note, for comparison all '.' separators are replaced by '_'.
             """
             in_kwargs = get_key_in_kwargs(key_in)
             in_config = get_key_in_config(key_in)
             if len(in_kwargs) > 0:
                 key_load = in_kwargs[0]
                 source = 'kwargs'
                 val = kwargs.get(key_load)
             elif len(in_config) > 0:
                 key_load = in_config[0]
                 source = 'config'
                 val = session.parameter(key_load)
             else:
                 return None
             if isinstance(val, str | float | int | None):
-                self._logger.log(
-                    15,
-                    f"{key_in} loaded as {key_load} from {source}: {str(val)}")
+                self._logger.log(15, f"{key_in} loaded as {key_load} from {source}: {str(val)}")
             else:
-                self._logger.log(
-                    15, f"{key_in} loaded as {key_load} from {source}")
+                self._logger.log(15, f"{key_in} loaded as {key_load} from {source}")
             return val
         self._get_init_parameters = parameter
         self.__init_kwargs__ = kwargs
         cls = type(self)
 
         self._resetting = True  # Avoid unnecessary resets.
         for key in self.__init_parameters__:
             getattr(cls, key).__set__(self, parameter(key))
         self._resetting = False
 
         # Check default parameters before running the determination tests.
         for key, value in self.__default_parameters__.items():
             vp = getattr(cls, key)
             d_test = vp.determination_test
-            if ((d_test is not None and d_test.under_determined(self))
-                    or (d_test is None and not vp.fixed(self))):
+            if (d_test is not None and d_test.under_determined(self)) or (d_test is None and not vp.fixed(self)):
                 vp.__set__(self, value)
 
-        # Determination test is disabled on initial initialisation as the
-        # parameters are initialised in sequence, and it would fail regardless
-        # on the first parameters.
+        # Determination test is disabled on initial initialisation as the parameters are initialised in sequence,
+        # and it would fail regardless on the first parameters.
         d_tests = []
-        for key in [k for k in self.__init_parameters__
-                    if getattr(type(self), k).determination_test is not None]:
+        for key in [k for k in self.__init_parameters__ if getattr(type(self), k).determination_test is not None]:
             d_test = getattr(cls, key).determination_test
             if d_test not in d_tests:
                 d_tests += [d_test]
                 d_test.test(self)
         # endregion
 
         # region Part Initialisation
@@ -273,49 +253,45 @@
 
     def __deep_getattr__(self, name: str) -> Any:
         """Get value from block or its parts, solvers, and ports."""
         if '.' not in name:
             return self.__getattribute__(name)
         else:
             name_split = name.split('.')
-            return self.__getattribute__(name_split[0]).__deep_getattr__(
-                '.'.join(name_split[1:]))
+            return self.__getattribute__(name_split[0]).__deep_getattr__('.'.join(name_split[1:]))
 
     def __deep_setattr__(self, name: str, val: Any) -> None:
         """Set value on block or its parts, solvers, and ports."""
         if '.' not in name:
             return self.__setattr__(name, val)
         else:
             name_split = name.split('.')
-            self.__getattribute__(name_split[0]).__deep_setattr__(
-                '.'.join(name_split[1:]), val)
+            self.__getattribute__(name_split[0]).__deep_setattr__('.'.join(name_split[1:]), val)
 
     def __deep_get_vp__(self, name: str) -> Any:
         """Get value property from block or its parts, solvers, and ports."""
         if '.' not in name:
             return getattr(type(self), name)
         else:
             name_split = name.split('.')
-            return self.__getattribute__(name_split[0]).__deep_get_vp__(
-                '.'.join(name_split[1:]))
+            return self.__getattribute__(name_split[0]).__deep_get_vp__('.'.join(name_split[1:]))
 
     def __call__(self, *args, **kwargs) -> None:
         return self.report()
 
     @property
     def logger(self) -> logging.Logger:
         """Return the appropriate logger for the block."""
         return self._logger
     # endregion
 
     # region Solver Functions
     # region Reset
     def reset(self, parent_reset: bool = None) -> None:
-        """Tell the instance and sub-blocks to resolve before the next
-        value output."""
+        """Tell the instance and sub-blocks to resolve before the next value output."""
         if not self._resetting:
             self._resetting = True
             # reset all subcomponents while not calling the instances own reset
             for s in self.solvers:
                 s.reset(parent_reset=False)
             for p in self.parts:
                 p.reset(parent_reset=False)
@@ -329,25 +305,24 @@
                 parent_reset = self._bool_parent_reset
             if parent_reset and self.parent is not None:
                 self.parent.reset()
 
             self._resetting = False
 
     def reset_self(self) -> None:
-        """Reset own reset parameters without calling any changes on
-        attached blocks, ports, solvers."""
+        """Reset own reset parameters without calling any changes on attached blocks, ports, solvers."""
         # Reset all local attributes to the desired reset value
         for key, val in self._reset_dict.items():
             self.__setattr__(key, val)
 
     def hard_reset(self, convergence_reset: bool = False) -> None:
         """Reset all blocks including solver flags and intermediate values.
 
-        This should only be used to get the program unstuck as it undermines
-        recursion stops and deletes any progress made.
+        This should only be used to get the program unstuck as it undermines recursion stops and deletes any progress
+        made.
         """
         self._resetting = True  # Set True while resetting parts
         for key, val in self._hard_reset_dict.items():
             self.__setattr__(key, val)
         for solver in self.solvers:
             solver.hard_reset(convergence_reset)
         for p in self.parts:
@@ -356,23 +331,21 @@
         self.reset()
     # endregion
 
     # region Solve
     @property
     def solved_self(self) -> bool:
         """Return bool if the block and its solvers are solved."""
-        return True and (len(self.solvers) == 0
-                         or all([s.solved for s in self.solvers]))
+        return True and (len(self.solvers) == 0 or all([s.solved for s in self.solvers]))
 
     @property
     def solved(self) -> bool:
         """Return bool if the block, its solvers, and its contained blocks
         are solved."""
-        return self.solved_self and (len(self.parts) == 0
-                                     or all([p.solved for p in self.parts]))
+        return self.solved_self and (len(self.parts) == 0 or all([p.solved for p in self.parts]))
 
     def solve_self(self) -> None:
         """Solve the block and its solvers."""
         [s.solve() for s in self.solvers]
 
     def solve(self) -> None:
         """Solve the block, its solvers, and its parts."""
@@ -380,38 +353,32 @@
         [p.solve() for p in self.parts]
     # endregion
 
     # region Fixed
     @property
     def fixed_self(self) -> bool:
         """Bool if this block, regardless of its parts is fixed."""
-        return all([getattr(type(self), vp).fixed(self)
-                    for vp in self.__fixed_parameters__])
+        return all([getattr(type(self), vp).fixed(self) for vp in self.__fixed_parameters__])
 
     @fixed_self.setter
     def fixed_self(self, val: bool) -> None:
         if val:
-            vp_not_fixed = [getattr(type(self), vp)
-                            for vp in self.__fixed_parameters__
+            vp_not_fixed = [getattr(type(self), vp) for vp in self.__fixed_parameters__
                             if not getattr(type(self), vp).fixed(self)]
 
-            # First get all values to not retrigger a solve after every setting
+            # First get all values to not re-trigger a solve after every setting
             values = [vp.__get__(self) for vp in vp_not_fixed]
-            [vp.__set_converging_value__(self, value)
-             for vp, value in zip(vp_not_fixed, values)]
+            [vp.__set_converging_value__(self, value) for vp, value in zip(vp_not_fixed, values)]
         else:
             val_dict = {}
             for vp in self.__fixed_parameters__:
                 if getattr(type(self), vp).determination_test is not None:
-                    vp_free = getattr(
-                        type(self), vp).determination_test.vp_free(self)
-                    if (len(vp_free) == 1 and
-                            vp_free[0] not in self.__fixed_parameters__):
-                        val_dict.update({
-                            vp_free[0]: self.__getattribute__(vp_free[0])})
+                    vp_free = getattr(type(self), vp).determination_test.vp_free(self)
+                    if len(vp_free) == 1 and vp_free[0] not in self.__fixed_parameters__:
+                        val_dict.update({vp_free[0]: self.__getattribute__(vp_free[0])})
 
             for key, val in val_dict.items():
                 self.__setattr__(key, val)
 
     @property
     def fixed(self) -> bool:
         """Bool if block and parts are fixed."""
```

### Comparing `cetpy-0.1.0b5/cetpy/Modules/SysML/_ContinuousPort.py` & `cetpy-0.1.0b6/cetpy/Modules/SysML/_ContinuousPort.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/SysML/_FlowProperty.py` & `cetpy-0.1.0b6/cetpy/Modules/SysML/_FlowProperty.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/SysML/_PartProperty.py` & `cetpy-0.1.0b6/cetpy/Modules/SysML/_PartProperty.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/SysML/_Port.py` & `cetpy-0.1.0b6/cetpy/Modules/SysML/_Port.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/SysML/_ProxyProperty.py` & `cetpy-0.1.0b6/cetpy/Modules/SysML/_ProxyProperty.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/SysML/_ValueProperty.py` & `cetpy-0.1.0b6/cetpy/Modules/SysML/_ValueProperty.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Utilities/InputValidation.py` & `cetpy-0.1.0b6/cetpy/Modules/Utilities/InputValidation.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/Modules/Utilities/Labelling.py` & `cetpy-0.1.0b6/cetpy/Modules/Utilities/Labelling.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy/tests/TestModules/TestSysML/test_Block.py` & `cetpy-0.1.0b6/cetpy/tests/TestModules/TestSysML/test_Block.py`

 * *Files identical despite different names*

### Comparing `cetpy-0.1.0b5/cetpy.egg-info/PKG-INFO` & `cetpy-0.1.0b6/cetpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cetpy
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: Congruent Engineering Toolbox
 Home-page: https://github.com/CongruentEngineeringToolbox/cetpy
 Author: CET developers
 Keywords: engineering,system engineering,congruent engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -16,17 +16,14 @@
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: CoolProp
 Requires-Dist: tomli
-Requires-Dist: keras
-Requires-Dist: keras-tuner
-Requires-Dist: tensorflow
 Requires-Dist: tabulate
 Requires-Dist: smt
 Requires-Dist: pytest
 Requires-Dist: matplotlib
 Requires-Dist: statsmodels
 Requires-Dist: scikit-learn
```

### Comparing `cetpy-0.1.0b5/cetpy.egg-info/SOURCES.txt` & `cetpy-0.1.0b6/cetpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 cetpy/__init__.py
 cetpy.egg-info/PKG-INFO
 cetpy.egg-info/SOURCES.txt
 cetpy.egg-info/dependency_links.txt
 cetpy.egg-info/requires.txt
 cetpy.egg-info/top_level.txt
 cetpy/CaseTools/FilterFunctions.py
+cetpy/CaseTools/RegressionDataSet.py
 cetpy/CaseTools/_CaseGenerator.py
 cetpy/CaseTools/_CaseRunner.py
 cetpy/CaseTools/_DataSet.py
 cetpy/CaseTools/__init__.py
 cetpy/Configuration/_ConfigurationManager.py
 cetpy/Configuration/_ModuleManager.py
 cetpy/Configuration/_Session.py
```

### Comparing `cetpy-0.1.0b5/setup.py` & `cetpy-0.1.0b6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='cetpy',
-    version='0.1.0b5',
+    version='0.1.0b6',
     description='Congruent Engineering Toolbox',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CongruentEngineeringToolbox/cetpy",
     author='CET developers',
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
@@ -29,17 +29,14 @@
     include_package_data=True,
     python_requires=">=3.10, <4",
     install_requires=[
         'numpy',
         'pandas',
         'CoolProp',
         'tomli',
-        'keras',
-        'keras-tuner',
-        'tensorflow',
         'tabulate',
         'smt',
         'pytest',
         'matplotlib',
         'statsmodels',
         'scikit-learn'
     ],
```

