# Comparing `tmp/simulab-0.0.2.tar.gz` & `tmp/simulab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulab-0.0.2.tar", max compression
+gzip compressed data, was "simulab-0.0.3.tar", max compression
```

## Comparing `simulab-0.0.2.tar` & `simulab-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1080 2024-06-02 23:00:24.778733 simulab-0.0.2/LICENSE
--rw-r--r--   0        0        0     2198 2024-06-02 23:00:24.778733 simulab-0.0.2/README.md
--rw-r--r--   0        0        0     2184 2024-06-02 23:00:24.778733 simulab-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/abstract/__init__.py
--rw-r--r--   0        0        0     1709 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/abstract/agent.py
--rw-r--r--   0        0        0     7676 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/abstract/model.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/__init__.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/condensation/__init__.py
--rw-r--r--   0        0        0     2387 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/condensation/model.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/game_of_life/__init__.py
--rw-r--r--   0        0        0     1536 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/game_of_life/model.py
--rw-r--r--   0        0        0     5021 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/game_of_life/seeds.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/__init__.py
--rw-r--r--   0        0        0     3679 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/agent.py
--rw-r--r--   0        0        0      634 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/formulas.py
--rw-r--r--   0        0        0     4608 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/real_state_market/model.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/schelling/__init__.py
--rw-r--r--   0        0        0     2221 2024-06-02 23:00:24.782733 simulab-0.0.2/src/models/computational/schelling/model.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/__init__.py
--rw-r--r--   0        0        0     1312 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/equilibrium_criterion.py
--rw-r--r--   0        0        0     1801 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/experiment.py
--rw-r--r--   0        0        0     1909 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/lattice.py
--rw-r--r--   0        0        0     1494 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/neighborhood.py
--rw-r--r--   0        0        0     2079 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/core/runner.py
--rw-r--r--   0        0        0        0 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/__init__.py
--rw-r--r--   0        0        0     3576 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/animated_lattice.py
--rw-r--r--   0        0        0     5438 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/final_grid.py
--rw-r--r--   0        0        0     3041 2024-06-02 23:00:24.782733 simulab-0.0.2/src/simulation/plotters/numerical_series.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 simulab-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-06-03 00:25:50.491140 simulab-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2198 2024-06-03 00:25:50.491140 simulab-0.0.3/README.md
+-rw-r--r--   0        0        0     2192 2024-06-03 00:25:50.495140 simulab-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/abstract/__init__.py
+-rw-r--r--   0        0        0     1709 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/abstract/agent.py
+-rw-r--r--   0        0        0     7692 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/abstract/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/condensation/__init__.py
+-rw-r--r--   0        0        0     2395 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/condensation/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/game_of_life/__init__.py
+-rw-r--r--   0        0        0     1548 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/game_of_life/model.py
+-rw-r--r--   0        0        0     5025 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/game_of_life/seeds.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/__init__.py
+-rw-r--r--   0        0        0     3691 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/agent.py
+-rw-r--r--   0        0        0      634 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/formulas.py
+-rw-r--r--   0        0        0     4628 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/real_state_market/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/schelling/__init__.py
+-rw-r--r--   0        0        0     2229 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/models/computational/schelling/model.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/simulation/core/__init__.py
+-rw-r--r--   0        0        0     1312 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/simulation/core/equilibrium_criterion.py
+-rw-r--r--   0        0        0     1801 2024-06-03 00:25:50.495140 simulab-0.0.3/simulab/simulation/core/experiment.py
+-rw-r--r--   0        0        0     1909 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/core/lattice.py
+-rw-r--r--   0        0        0     1494 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/core/neighborhood.py
+-rw-r--r--   0        0        0     2091 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/core/runner.py
+-rw-r--r--   0        0        0        0 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/__init__.py
+-rw-r--r--   0        0        0     3580 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/animated_lattice.py
+-rw-r--r--   0        0        0     5442 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/final_grid.py
+-rw-r--r--   0        0        0     3045 2024-06-03 00:25:50.499140 simulab-0.0.3/simulab/simulation/plotters/numerical_series.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 simulab-0.0.3/PKG-INFO
```

### Comparing `simulab-0.0.2/LICENSE` & `simulab-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/README.md` & `simulab-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/pyproject.toml` & `simulab-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "simulab"
-version = "0.0.2"
+version = "0.0.3"
 description = "Simple simulation framework, created during a course of the Discrete Events Simulation Laboratory, from the University of Buenos Aires (https://modsimu.exp.dc.uba.ar/sed/)"
 authors = ["Armando Ezequiel Puerta <armando.ezequiel.puerta@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
-packages = [{include = "src"}]
-include = [{ path = "src" }]
+packages = [{include = "simulab"}]
+include = [{ path = "simulab" }]
 exclude = ["docs", "tests"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `simulab-0.0.2/src/models/abstract/agent.py` & `simulab-0.0.3/simulab/models/abstract/agent.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/src/models/abstract/model.py` & `simulab-0.0.3/simulab/models/abstract/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from copy import deepcopy
 from functools import partial
 from typing import Any, Callable, Dict, List, Tuple, Type, Union
 
 import networkx as nx
 import numpy as np
 
-from src.models.abstract.agent import Agent
-from src.simulation.core.equilibrium_criterion import AbstractCriterion
-from src.simulation.core.lattice import Lattice
-from src.simulation.core.neighborhood import Neighborhood, VonNeumann
+from simulab.models.abstract.agent import Agent
+from simulab.simulation.core.equilibrium_criterion import AbstractCriterion
+from simulab.simulation.core.lattice import Lattice
+from simulab.simulation.core.neighborhood import Neighborhood, VonNeumann
 
 
 class AbstractLatticeModel(ABC):
     def __init__(
         self,
         length: int,
         configuration: Lattice | np.ndarray | None = None,
```

### Comparing `simulab-0.0.2/src/models/computational/condensation/model.py` & `simulab-0.0.3/simulab/models/computational/condensation/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, cast
 
 import networkx as nx
 
-from src.models.abstract.model import AbstractLatticeModel, as_series
-from src.simulation.core.lattice import Lattice
+from simulab.models.abstract.model import AbstractLatticeModel, as_series
+from simulab.simulation.core.lattice import Lattice
 
 
 class Condensation(AbstractLatticeModel):
     CONDENSES = 1
     EVAPORATES = 0
 
     def __init__(  # type: ignore[no-untyped-def]
```

### Comparing `simulab-0.0.2/src/models/computational/game_of_life/model.py` & `simulab-0.0.3/simulab/models/computational/game_of_life/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, cast
 
-from src.models.abstract.model import AbstractLatticeModel, as_series
-from src.models.computational.game_of_life.seeds import Seed
-from src.simulation.core.lattice import Lattice
+from simulab.models.abstract.model import AbstractLatticeModel, as_series
+from simulab.models.computational.game_of_life.seeds import Seed
+from simulab.simulation.core.lattice import Lattice
 
 
 class GameOfLife(AbstractLatticeModel):
     ALIVE = 1
     DEAD = 0
 
     def __init__(self, seeds: List[Seed], *args, **kwargs):  # type: ignore[no-untyped-def]
```

### Comparing `simulab-0.0.2/src/models/computational/game_of_life/seeds.py` & `simulab-0.0.3/simulab/models/computational/game_of_life/seeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 
 import numpy as np
 
-from src.simulation.core.lattice import Lattice
+from simulab.simulation.core.lattice import Lattice
 
 
 class Seed(ABC):
     def __init__(self, i: int, j: int) -> None:
         self.i = i
         self.j = j
```

### Comparing `simulab-0.0.2/src/models/computational/real_state_market/agent.py` & `simulab-0.0.3/simulab/models/computational/real_state_market/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple
 
-from src.models.abstract.agent import Agent
-from src.models.abstract.model import AbstractLatticeModel
-from src.simulation.core.lattice import Lattice
+from simulab.models.abstract.agent import Agent
+from simulab.models.abstract.model import AbstractLatticeModel
+from simulab.simulation.core.lattice import Lattice
 
 
 class Transfer:
     def __init__(
         self,
         payer: "RealStateAgent",
         to_pay: float,
```

### Comparing `simulab-0.0.2/src/models/computational/real_state_market/formulas.py` & `simulab-0.0.3/simulab/models/computational/real_state_market/formulas.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/src/models/computational/real_state_market/model.py` & `simulab-0.0.3/simulab/models/computational/real_state_market/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 from typing import cast as typing_cast
 
-from src.models.abstract.agent import Agent
-from src.models.abstract.model import AbstractLatticeModel, as_series, as_series_with
-from src.models.computational.real_state_market.agent import RealStateAgent
-from src.models.computational.real_state_market.formulas import PriceFormula, UtilityFormula
-from src.simulation.core.lattice import Lattice
+from simulab.models.abstract.agent import Agent
+from simulab.models.abstract.model import AbstractLatticeModel, as_series, as_series_with
+from simulab.models.computational.real_state_market.agent import RealStateAgent
+from simulab.models.computational.real_state_market.formulas import PriceFormula, UtilityFormula
+from simulab.simulation.core.lattice import Lattice
 
 
 class RealStateMarket(AbstractLatticeModel):
     def __init__(  # type: ignore[no-untyped-def]
         self,
         alpha: float = 0.5,
         A: float = 1 / 16,
```

### Comparing `simulab-0.0.2/src/models/computational/schelling/model.py` & `simulab-0.0.3/simulab/models/computational/schelling/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
-from src.models.abstract.model import AbstractLatticeModel, as_series, as_series_with
-from src.simulation.core.lattice import Lattice
+from simulab.models.abstract.model import AbstractLatticeModel, as_series, as_series_with
+from simulab.simulation.core.lattice import Lattice
 
 
 class Schelling(AbstractLatticeModel):
     def __init__(  # type: ignore[no-untyped-def]
         self,
         tolerance: int,
         *args,
```

### Comparing `simulab-0.0.2/src/simulation/core/equilibrium_criterion.py` & `simulab-0.0.3/simulab/simulation/core/equilibrium_criterion.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/src/simulation/core/experiment.py` & `simulab-0.0.3/simulab/simulation/core/experiment.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/src/simulation/core/lattice.py` & `simulab-0.0.3/simulab/simulation/core/lattice.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/src/simulation/core/neighborhood.py` & `simulab-0.0.3/simulab/simulation/core/neighborhood.py`

 * *Files identical despite different names*

### Comparing `simulab-0.0.2/src/simulation/core/runner.py` & `simulab-0.0.3/simulab/simulation/core/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Tuple, Type
 
-from src.models.abstract.model import AbstractLatticeModel
-from src.simulation.core.equilibrium_criterion import AbstractCriterion
-from src.simulation.core.experiment import ExperimentParametersSet
+from simulab.models.abstract.model import AbstractLatticeModel
+from simulab.simulation.core.equilibrium_criterion import AbstractCriterion
+from simulab.simulation.core.experiment import ExperimentParametersSet
 
 
 class Execute:
     def __init__(self, *series_names: Tuple[str, ...], times: int = 1) -> None:
         self.series_names: Tuple[str] = series_names  # type: ignore[assignment]
         self.times: int = times
```

### Comparing `simulab-0.0.2/src/simulation/plotters/animated_lattice.py` & `simulab-0.0.3/simulab/simulation/plotters/animated_lattice.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List
 
 import plotly.graph_objs as go
 
-from src.simulation.core.runner import Runner
+from simulab.simulation.core.runner import Runner
 
 
 class AnimatedLatticeSeries:
     @classmethod
     def show_up(
         cls,
         series_name: str,
```

### Comparing `simulab-0.0.2/src/simulation/plotters/final_grid.py` & `simulab-0.0.3/simulab/simulation/plotters/final_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Set
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from src.simulation.core.runner import Runner
+from simulab.simulation.core.runner import Runner
 
 
 class FinalGridSeries:
     @classmethod
     def show_up(
         cls,
         series_name: str,
```

### Comparing `simulab-0.0.2/src/simulation/plotters/numerical_series.py` & `simulab-0.0.3/simulab/simulation/plotters/numerical_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import plotly.graph_objects as go
 
-from src.simulation.core.runner import Runner
+from simulab.simulation.core.runner import Runner
 
 
 class NumericalSeries:
     @classmethod
     def show_up(
         cls,
         series_name: str,
```

### Comparing `simulab-0.0.2/PKG-INFO` & `simulab-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simulab
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple simulation framework, created during a course of the Discrete Events Simulation Laboratory, from the University of Buenos Aires (https://modsimu.exp.dc.uba.ar/sed/)
 Home-page: https://github.com/EzequielPuerta/simulab
 License: MIT
 Author: Armando Ezequiel Puerta
 Author-email: armando.ezequiel.puerta@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

