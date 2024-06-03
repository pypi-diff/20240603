# Comparing `tmp/simulab-0.0.1.tar.gz` & `tmp/simulab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulab-0.0.1.tar", max compression
+gzip compressed data, was "simulab-0.0.2.tar", max compression
```

## Comparing `simulab-0.0.1.tar` & `simulab-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1080 2024-06-02 22:32:12.840483 simulab-0.0.1/LICENSE
--rw-r--r--   0        0        0     2198 2024-06-02 22:32:12.840483 simulab-0.0.1/README.md
--rw-r--r--   0        0        0     2165 2024-06-02 22:32:12.844483 simulab-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/__init__.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/abstract/__init__.py
--rw-r--r--   0        0        0     1709 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/abstract/agent.py
--rw-r--r--   0        0        0     7676 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/abstract/model.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/__init__.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/condensation/__init__.py
--rw-r--r--   0        0        0     2387 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/condensation/model.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/game_of_life/__init__.py
--rw-r--r--   0        0        0     1536 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/game_of_life/model.py
--rw-r--r--   0        0        0     5021 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/game_of_life/seeds.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/real_state_market/__init__.py
--rw-r--r--   0        0        0     3679 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/real_state_market/agent.py
--rw-r--r--   0        0        0      634 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/real_state_market/formulas.py
--rw-r--r--   0        0        0     4608 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/real_state_market/model.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/schelling/__init__.py
--rw-r--r--   0        0        0     2221 2024-06-02 22:32:12.844483 simulab-0.0.1/src/models/computational/schelling/model.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/core/__init__.py
--rw-r--r--   0        0        0     1312 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/core/equilibrium_criterion.py
--rw-r--r--   0        0        0     1801 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/core/experiment.py
--rw-r--r--   0        0        0     1909 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/core/lattice.py
--rw-r--r--   0        0        0     1494 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/core/neighborhood.py
--rw-r--r--   0        0        0     2079 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/core/runner.py
--rw-r--r--   0        0        0        0 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/plotters/__init__.py
--rw-r--r--   0        0        0     3576 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/plotters/animated_lattice.py
--rw-r--r--   0        0        0     5438 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/plotters/final_grid.py
--rw-r--r--   0        0        0     3041 2024-06-02 22:32:12.844483 simulab-0.0.1/src/simulation/plotters/numerical_series.py
--rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 simulab-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-06-02 23:00:24.778733 simulab-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2198 2024-06-02 23:00:24.778733 simulab-0.0.2/README.md
+-rw-r--r--   0        0        0     2184 2024-06-02 23:00:24.778733 simulab-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/abstract/__init__.py
+-rw-r--r--   0        0        0     1709 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/abstract/agent.py
+-rw-r--r--   0        0        0     7676 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/abstract/model.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/condensation/__init__.py
+-rw-r--r--   0        0        0     2387 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/condensation/model.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/game_of_life/__init__.py
+-rw-r--r--   0        0        0     1536 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/game_of_life/model.py
+-rw-r--r--   0        0        0     5021 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/game_of_life/seeds.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/__init__.py
+-rw-r--r--   0        0        0     3679 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/agent.py
+-rw-r--r--   0        0        0      634 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/formulas.py
+-rw-r--r--   0        0        0     4608 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/model.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/schelling/__init__.py
+-rw-r--r--   0        0        0     2221 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/schelling/model.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/__init__.py
+-rw-r--r--   0        0        0     1312 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/equilibrium_criterion.py
+-rw-r--r--   0        0        0     1801 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/experiment.py
+-rw-r--r--   0        0        0     1909 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/lattice.py
+-rw-r--r--   0        0        0     1494 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/neighborhood.py
+-rw-r--r--   0        0        0     2079 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/runner.py
+-rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/__init__.py
+-rw-r--r--   0        0        0     3576 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/animated_lattice.py
+-rw-r--r--   0        0        0     5438 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/final_grid.py
+-rw-r--r--   0        0        0     3041 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/numerical_series.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 simulab-0.0.2/PKG-INFO
```

### Comparing `simulab-0.0.1/LICENSE` & `simulab-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/README.md` & `simulab-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/pyproject.toml` & `simulab-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simulab"
-version = "0.0.1"
+version = "0.0.2"
 description = "Simple simulation framework, created during a course of the Discrete Events Simulation Laboratory, from the University of Buenos Aires (https://modsimu.exp.dc.uba.ar/sed/)"
 authors = ["Armando Ezequiel Puerta <armando.ezequiel.puerta@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "src"}]
 include = [{ path = "src" }]
 exclude = ["docs", "tests"]
@@ -19,14 +19,15 @@
 repository = "https://github.com/EzequielPuerta/simulab"
 documentation = "https://github.com/EzequielPuerta/simulab"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
 networkx = "^3.3"
+plotly = "^5.22.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^5.0.0"
 pre-commit = "^3.7.1"
 flake8 = "^7.0.0"
 mypy = "^1.10.0"
```

### Comparing `simulab-0.0.1/src/models/abstract/agent.py` & `simulab-0.0.2/src/models/abstract/agent.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/abstract/model.py` & `simulab-0.0.2/src/models/abstract/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/computational/condensation/model.py` & `simulab-0.0.2/src/models/computational/condensation/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/computational/game_of_life/model.py` & `simulab-0.0.2/src/models/computational/game_of_life/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/computational/game_of_life/seeds.py` & `simulab-0.0.2/src/models/computational/game_of_life/seeds.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/computational/real_state_market/agent.py` & `simulab-0.0.2/src/models/computational/real_state_market/agent.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/computational/real_state_market/formulas.py` & `simulab-0.0.2/src/models/computational/real_state_market/formulas.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/computational/real_state_market/model.py` & `simulab-0.0.2/src/models/computational/real_state_market/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/models/computational/schelling/model.py` & `simulab-0.0.2/src/models/computational/schelling/model.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/core/equilibrium_criterion.py` & `simulab-0.0.2/src/simulation/core/equilibrium_criterion.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/core/experiment.py` & `simulab-0.0.2/src/simulation/core/experiment.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/core/lattice.py` & `simulab-0.0.2/src/simulation/core/lattice.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/core/neighborhood.py` & `simulab-0.0.2/src/simulation/core/neighborhood.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/core/runner.py` & `simulab-0.0.2/src/simulation/core/runner.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/plotters/animated_lattice.py` & `simulab-0.0.2/src/simulation/plotters/animated_lattice.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/plotters/final_grid.py` & `simulab-0.0.2/src/simulation/plotters/final_grid.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/src/simulation/plotters/numerical_series.py` & `simulab-0.0.2/src/simulation/plotters/numerical_series.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.1/PKG-INFO` & `simulab-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple simulation framework, created during a course of the Discrete Events Simulation Laboratory, from the University of Buenos Aires (https://modsimu.exp.dc.uba.ar/sed/)
 Home-page: https://github.com/EzequielPuerta/simulab
 License: MIT
 Author: Armando Ezequiel Puerta
 Author-email: armando.ezequiel.puerta@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: plotly (>=5.22.0,<6.0.0)
 Project-URL: Bug Tracker, https://github.com/EzequielPuerta/simulab/issues
 Project-URL: Documentation, https://github.com/EzequielPuerta/simulab
 Project-URL: Repository, https://github.com/EzequielPuerta/simulab
 Description-Content-Type: text/markdown
 
 # SimuLab
```

