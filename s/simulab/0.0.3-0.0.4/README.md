# Comparing `tmp/simulab-0.0.3.tar.gz` & `tmp/simulab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulab-0.0.3.tar", max compression
+gzip compressed data, was "simulab-0.0.4.tar", max compression
```

## Comparing `simulab-0.0.3.tar` & `simulab-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1080 2024-06-03 00:25:50.491140 simulab-0.0.3/LICENSE
--rw-r--r--   0        0        0     2198 2024-06-03 00:25:50.491140 simulab-0.0.3/README.md
--rw-r--r--   0        0        0     2192 2024-06-03 00:25:50.495140 simulab-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/__init__.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/abstract/__init__.py
--rw-r--r--   0        0        0     1709 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/abstract/agent.py
--rw-r--r--   0        0        0     7692 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/abstract/model.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/__init__.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/condensation/__init__.py
--rw-r--r--   0        0        0     2395 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/condensation/model.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/game_of_life/__init__.py
--rw-r--r--   0        0        0     1548 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/game_of_life/model.py
--rw-r--r--   0        0        0     5025 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/game_of_life/seeds.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/__init__.py
--rw-r--r--   0        0        0     3691 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/agent.py
--rw-r--r--   0        0        0      634 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/formulas.py
--rw-r--r--   0        0        0     4628 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/model.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/schelling/__init__.py
--rw-r--r--   0        0        0     2229 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/schelling/model.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/simulation/core/__init__.py
--rw-r--r--   0        0        0     1312 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/simulation/core/equilibrium_criterion.py
--rw-r--r--   0        0        0     1801 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/simulation/core/experiment.py
--rw-r--r--   0        0        0     1909 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/core/lattice.py
--rw-r--r--   0        0        0     1494 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/core/neighborhood.py
--rw-r--r--   0        0        0     2091 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/core/runner.py
--rw-r--r--   0        0        0        0 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/__init__.py
--rw-r--r--   0        0        0     3580 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/animated_lattice.py
--rw-r--r--   0        0        0     5442 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/final_grid.py
--rw-r--r--   0        0        0     3045 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/numerical_series.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 simulab-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-06-03 01:00:45.516773 simulab-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2211 2024-06-03 01:00:45.516773 simulab-0.0.4/README.md
+-rw-r--r--   0        0        0     2192 2024-06-03 01:00:45.520773 simulab-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.520773 simulab-0.0.4/simulab/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.520773 simulab-0.0.4/simulab/models/abstract/__init__.py
+-rw-r--r--   0        0        0     1709 2024-06-03 01:00:45.520773 simulab-0.0.4/simulab/models/abstract/agent.py
+-rw-r--r--   0        0        0     7692 2024-06-03 01:00:45.520773 simulab-0.0.4/simulab/models/abstract/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.520773 simulab-0.0.4/simulab/models/computational/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/condensation/__init__.py
+-rw-r--r--   0        0        0     2395 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/condensation/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/game_of_life/__init__.py
+-rw-r--r--   0        0        0     1548 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/game_of_life/model.py
+-rw-r--r--   0        0        0     5025 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/game_of_life/seeds.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/real_state_market/__init__.py
+-rw-r--r--   0        0        0     3691 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/real_state_market/agent.py
+-rw-r--r--   0        0        0      634 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/real_state_market/formulas.py
+-rw-r--r--   0        0        0     4628 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/real_state_market/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/schelling/__init__.py
+-rw-r--r--   0        0        0     2229 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/models/computational/schelling/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/core/__init__.py
+-rw-r--r--   0        0        0     1312 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/core/equilibrium_criterion.py
+-rw-r--r--   0        0        0     1801 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/core/experiment.py
+-rw-r--r--   0        0        0     1909 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/core/lattice.py
+-rw-r--r--   0        0        0     1494 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/core/neighborhood.py
+-rw-r--r--   0        0        0     2091 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/core/runner.py
+-rw-r--r--   0        0        0        0 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/plotters/__init__.py
+-rw-r--r--   0        0        0     3580 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/plotters/animated_lattice.py
+-rw-r--r--   0        0        0     5442 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/plotters/final_grid.py
+-rw-r--r--   0        0        0     3045 2024-06-03 01:00:45.524773 simulab-0.0.4/simulab/simulation/plotters/numerical_series.py
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 simulab-0.0.4/PKG-INFO
```

### Comparing `simulab-0.0.3/LICENSE` & `simulab-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/README.md` & `simulab-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [![Codecov](https://img.shields.io/codecov/c/gh/EzequielPuerta/simulab?label=Codecov&logo=codecov&logoColor=white)](https://codecov.io/gh/EzequielPuerta/simulab)
 
 > [!WARNING]
 > #### This framework is a WIP
 
 ## Jupyter Notebooks
 
-On ***[this](https://github.com/EzequielPuerta-University/modelado_y_simulacion_de_sistemas_complejos)*** repository you can find some Jupyter Notebooks that use this framework. It's a set of models seen on some optional subject of my university career at the University of Buenos Aires.
+On ***[this](https://github.com/EzequielPuerta-University/modelado_y_simulacion_de_sistemas_complejos)*** repository you can find some Jupyter Notebooks (in Spanish) that use this framework. It's a set of models seen on some optional subject of my university career at the University of Buenos Aires.
 
 ## Framework explained
 
 * Models included
     * [Abstract](docs/abstract.md)
     * [Computationals](docs/computational.md)
         * [Schelling's Segregation](docs/computational.md#schellings-segregation)
```

### Comparing `simulab-0.0.3/pyproject.toml` & `simulab-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simulab"
-version = "0.0.3"
+version = "0.0.4"
 description = "Simple simulation framework, created during a course of the Discrete Events Simulation Laboratory, from the University of Buenos Aires (https://modsimu.exp.dc.uba.ar/sed/)"
 authors = ["Armando Ezequiel Puerta <armando.ezequiel.puerta@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "simulab"}]
 include = [{ path = "simulab" }]
 exclude = ["docs", "tests"]
```

### Comparing `simulab-0.0.3/simulab/models/abstract/agent.py` & `simulab-0.0.4/simulab/models/abstract/agent.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/abstract/model.py` & `simulab-0.0.4/simulab/models/abstract/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/computational/condensation/model.py` & `simulab-0.0.4/simulab/models/computational/condensation/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/computational/game_of_life/model.py` & `simulab-0.0.4/simulab/models/computational/game_of_life/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/computational/game_of_life/seeds.py` & `simulab-0.0.4/simulab/models/computational/game_of_life/seeds.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/computational/real_state_market/agent.py` & `simulab-0.0.4/simulab/models/computational/real_state_market/agent.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/computational/real_state_market/formulas.py` & `simulab-0.0.4/simulab/models/computational/real_state_market/formulas.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/computational/real_state_market/model.py` & `simulab-0.0.4/simulab/models/computational/real_state_market/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/models/computational/schelling/model.py` & `simulab-0.0.4/simulab/models/computational/schelling/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/core/equilibrium_criterion.py` & `simulab-0.0.4/simulab/simulation/core/equilibrium_criterion.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/core/experiment.py` & `simulab-0.0.4/simulab/simulation/core/experiment.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/core/lattice.py` & `simulab-0.0.4/simulab/simulation/core/lattice.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/core/neighborhood.py` & `simulab-0.0.4/simulab/simulation/core/neighborhood.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/core/runner.py` & `simulab-0.0.4/simulab/simulation/core/runner.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/plotters/animated_lattice.py` & `simulab-0.0.4/simulab/simulation/plotters/animated_lattice.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/plotters/final_grid.py` & `simulab-0.0.4/simulab/simulation/plotters/final_grid.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/simulab/simulation/plotters/numerical_series.py` & `simulab-0.0.4/simulab/simulation/plotters/numerical_series.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.3/PKG-INFO` & `simulab-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple simulation framework, created during a course of the Discrete Events Simulation Laboratory, from the University of Buenos Aires (https://modsimu.exp.dc.uba.ar/sed/)
 Home-page: https://github.com/EzequielPuerta/simulab
 License: MIT
 Author: Armando Ezequiel Puerta
 Author-email: armando.ezequiel.puerta@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 [![Codecov](https://img.shields.io/codecov/c/gh/EzequielPuerta/simulab?label=Codecov&logo=codecov&logoColor=white)](https://codecov.io/gh/EzequielPuerta/simulab)
 
 > [!WARNING]
 > #### This framework is a WIP
 
 ## Jupyter Notebooks
 
-On ***[this](https://github.com/EzequielPuerta-University/modelado_y_simulacion_de_sistemas_complejos)*** repository you can find some Jupyter Notebooks that use this framework. It's a set of models seen on some optional subject of my university career at the University of Buenos Aires.
+On ***[this](https://github.com/EzequielPuerta-University/modelado_y_simulacion_de_sistemas_complejos)*** repository you can find some Jupyter Notebooks (in Spanish) that use this framework. It's a set of models seen on some optional subject of my university career at the University of Buenos Aires.
 
 ## Framework explained
 
 * Models included
     * [Abstract](docs/abstract.md)
     * [Computationals](docs/computational.md)
         * [Schelling's Segregation](docs/computational.md#schellings-segregation)
```

