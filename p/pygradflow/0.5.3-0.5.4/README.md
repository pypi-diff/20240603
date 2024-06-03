# Comparing `tmp/pygradflow-0.5.3.tar.gz` & `tmp/pygradflow-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.5.3.tar", max compression
+gzip compressed data, was "pygradflow-0.5.4.tar", max compression
```

## Comparing `pygradflow-0.5.3.tar` & `pygradflow-0.5.4.tar`

### file list

```diff
@@ -1,55 +1,57 @@
--rw-r--r--   0        0        0    10847 2024-05-28 11:53:18.096126 pygradflow-0.5.3/LICENSE
--rw-r--r--   0        0        0      984 2024-05-28 11:53:18.096126 pygradflow-0.5.3/README.md
--rw-r--r--   0        0        0        0 2024-05-28 11:53:18.096126 pygradflow-0.5.3/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-28 11:53:18.096126 pygradflow-0.5.3/pygradflow/active_set.py
--rw-r--r--   0        0        0     1016 2024-05-28 11:53:18.096126 pygradflow-0.5.3/pygradflow/callbacks.py
--rw-r--r--   0        0        0     4417 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/controller.py
--rw-r--r--   0        0        0     2431 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     9840 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/display.py
--rw-r--r--   0        0        0     6359 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/eval.py
--rw-r--r--   0        0        0     7472 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/implicit_func.py
--rw-r--r--   0        0        0        0 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/integration/__init__.py
--rw-r--r--   0        0        0     1173 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/integration/events.py
--rw-r--r--   0        0        0     3634 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/integration/flow.py
--rw-r--r--   0        0        0    16999 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/integration/integration_solver.py
--rw-r--r--   0        0        0     4330 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/integration/problem_switches.py
--rw-r--r--   0        0        0     3458 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/integration/restricted_flow.py
--rw-r--r--   0        0        0     6092 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/log.py
--rw-r--r--   0        0        0     9309 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/newton.py
--rw-r--r--   0        0        0     6017 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/py.typed
--rw-r--r--   0        0        0     1872 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/result.py
--rw-r--r--   0        0        0     4746 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      708 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2157 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/runners/mps_runner.py
--rw-r--r--   0        0        0     2015 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     8600 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     7406 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/scale.py
--rw-r--r--   0        0        0    12377 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/solver.py
--rw-r--r--   0        0        0     1738 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/status.py
--rw-r--r--   0        0        0     1284 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4274 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     7831 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     3416 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/box_solver.py
--rw-r--r--   0        0        0     2710 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3101 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7326 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2691 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2476 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4713 2024-05-28 11:53:18.100126 pygradflow-0.5.3/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2917 2024-05-28 11:53:18.104126 pygradflow-0.5.3/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4024 2024-05-28 11:53:18.104126 pygradflow-0.5.3/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      492 2024-05-28 11:53:18.104126 pygradflow-0.5.3/pygradflow/timer.py
--rw-r--r--   0        0        0     3009 2024-05-28 11:53:18.104126 pygradflow-0.5.3/pygradflow/transform.py
--rw-r--r--   0        0        0     1043 2024-05-28 11:53:18.104126 pygradflow-0.5.3/pygradflow/util.py
--rw-r--r--   0        0        0     1171 2024-05-28 11:53:18.104126 pygradflow-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1941 1970-01-01 00:00:00.000000 pygradflow-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-06-03 12:41:51.019786 pygradflow-0.5.4/LICENSE
+-rw-r--r--   0        0        0      984 2024-06-03 12:41:51.019786 pygradflow-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/active_set.py
+-rw-r--r--   0        0        0     1016 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/callbacks.py
+-rw-r--r--   0        0        0     4417 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/controller.py
+-rw-r--r--   0        0        0     2431 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     9840 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/display.py
+-rw-r--r--   0        0        0     6359 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/eval.py
+-rw-r--r--   0        0        0     7472 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/integration/__init__.py
+-rw-r--r--   0        0        0     1173 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/integration/events.py
+-rw-r--r--   0        0        0     3634 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/integration/flow.py
+-rw-r--r--   0        0        0    16999 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/integration/integration_solver.py
+-rw-r--r--   0        0        0     4330 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/integration/problem_switches.py
+-rw-r--r--   0        0        0     3458 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/integration/restricted_flow.py
+-rw-r--r--   0        0        0     6092 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/log.py
+-rw-r--r--   0        0        0     9323 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/newton.py
+-rw-r--r--   0        0        0     6017 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/py.typed
+-rw-r--r--   0        0        0     1872 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/result.py
+-rw-r--r--   0        0        0     4746 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      708 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2157 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/runners/mps_runner.py
+-rw-r--r--   0        0        0     2015 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     8600 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     7406 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/scale.py
+-rw-r--r--   0        0        0    11944 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/solver.py
+-rw-r--r--   0        0        0     1738 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/status.py
+-rw-r--r--   0        0        0     7819 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     3416 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/step/box_solver.py
+-rw-r--r--   0        0        0     2710 2024-06-03 12:41:51.019786 pygradflow-0.5.4/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2523 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2178 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0      635 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2732 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     1183 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/newton_control.py
+-rw-r--r--   0        0        0     7314 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2106 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     1210 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/solver/__init__.py
+-rw-r--r--   0        0        0     4265 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/solver/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     3092 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/solver/extended_step_solver.py
+-rw-r--r--   0        0        0     2677 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/solver/scaled_step_solver.py
+-rw-r--r--   0        0        0     2467 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/solver/standard_step_solver.py
+-rw-r--r--   0        0        0     2947 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/solver/step_solver.py
+-rw-r--r--   0        0        0     4015 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/solver/symmetric_step_solver.py
+-rw-r--r--   0        0        0     4570 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0      164 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/step/step_solver_error.py
+-rw-r--r--   0        0        0      492 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/timer.py
+-rw-r--r--   0        0        0     3009 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/transform.py
+-rw-r--r--   0        0        0     1043 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pygradflow/util.py
+-rw-r--r--   0        0        0     1171 2024-06-03 12:41:51.023786 pygradflow-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1941 1970-01-01 00:00:00.000000 pygradflow-0.5.4/PKG-INFO
```

### Comparing `pygradflow-0.5.3/LICENSE` & `pygradflow-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/README.md` & `pygradflow-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/active_set.py` & `pygradflow-0.5.4/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/callbacks.py` & `pygradflow-0.5.4/pygradflow/callbacks.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/cons_problem.py` & `pygradflow-0.5.4/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/controller.py` & `pygradflow-0.5.4/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/deriv_check.py` & `pygradflow-0.5.4/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/display.py` & `pygradflow-0.5.4/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/eval.py` & `pygradflow-0.5.4/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/implicit_func.py` & `pygradflow-0.5.4/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/integration/events.py` & `pygradflow-0.5.4/pygradflow/integration/events.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/integration/flow.py` & `pygradflow-0.5.4/pygradflow/integration/flow.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/integration/integration_solver.py` & `pygradflow-0.5.4/pygradflow/integration/integration_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/integration/problem_switches.py` & `pygradflow-0.5.4/pygradflow/integration/problem_switches.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/integration/restricted_flow.py` & `pygradflow-0.5.4/pygradflow/integration/restricted_flow.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/iterate.py` & `pygradflow-0.5.4/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/newton.py` & `pygradflow-0.5.4/pygradflow/newton.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import numpy as np
 import scipy as sp
 
 from pygradflow.iterate import Iterate
 from pygradflow.log import logger as lgg
 from pygradflow.params import NewtonType, Params
 from pygradflow.problem import Problem
-from pygradflow.step import step_solver
-from pygradflow.step.step_solver import StepResult, StepSolver
+from pygradflow.step.solver import step_solver
+from pygradflow.step.solver.step_solver import StepResult, StepSolver
 
 logger = lgg.getChild("newton")
 
 
 class NewtonMethod(abc.ABC):
     def __init__(
         self, problem: Problem, orig_iterate: Iterate, dt: float, rho: float
```

### Comparing `pygradflow-0.5.3/pygradflow/params.py` & `pygradflow-0.5.4/pygradflow/params.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/penalty.py` & `pygradflow-0.5.4/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/problem.py` & `pygradflow-0.5.4/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/result.py` & `pygradflow-0.5.4/pygradflow/result.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/runners/cutest_runner.py` & `pygradflow-0.5.4/pygradflow/runners/cutest_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/runners/instance.py` & `pygradflow-0.5.4/pygradflow/runners/instance.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/runners/mps_runner.py` & `pygradflow-0.5.4/pygradflow/runners/mps_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/runners/qplib_runner.py` & `pygradflow-0.5.4/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/runners/runner.py` & `pygradflow-0.5.4/pygradflow/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/scale.py` & `pygradflow-0.5.4/pygradflow/scale.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/solver.py` & `pygradflow-0.5.4/pygradflow/solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import numpy as np
 
 from pygradflow.callbacks import Callbacks, CallbackType
 from pygradflow.display import Format, StateData, print_problem_stats, solver_display
 from pygradflow.iterate import Iterate
 from pygradflow.log import logger
-from pygradflow.newton import newton_method
 from pygradflow.params import Params
 from pygradflow.penalty import penalty_strategy
 from pygradflow.problem import Problem
 from pygradflow.result import SolverResult
 from pygradflow.status import SolverStatus
 from pygradflow.step.step_control import (
     StepController,
@@ -88,30 +87,17 @@
         self,
         controller: StepController,
         iterate: Iterate,
         dt: float,
         display: bool,
         timer: Timer,
     ) -> StepControlResult:
-        problem = self.problem
-        params = self.params
-        assert self.rho != -1.0
 
-        method = newton_method(problem, params, iterate, dt, self.rho)
-
-        def next_steps():
-            curr_iterate = iterate
-            while True:
-                next_step = method.step(curr_iterate)
-                yield next_step
-                curr_iterate = next_step.iterate
-
-        return controller.compute_step(
-            iterate, self.rho, dt, next_steps(), display, timer
-        )
+        assert self.rho != -1.0
+        return controller.compute_step(iterate, self.rho, dt, display, timer)
 
     def _deriv_check(self, x: np.ndarray, y: np.ndarray) -> None:
         from pygradflow.deriv_check import deriv_check
         from pygradflow.params import DerivCheck
 
         eval = self.evaluator
         params = self.params
```

### Comparing `pygradflow-0.5.3/pygradflow/status.py` & `pygradflow-0.5.4/pygradflow/status.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/step/__init__.py` & `pygradflow-0.5.4/pygradflow/step/solver/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params, StepSolverType
 from pygradflow.problem import Problem
-from pygradflow.step.asymmetric_step_solver import AsymmetricStepSolver
-from pygradflow.step.extended_step_solver import ExtendedStepSolver
-from pygradflow.step.standard_step_solver import StandardStepSolver
-from pygradflow.step.step_solver import StepSolver
-from pygradflow.step.symmetric_step_solver import SymmetricStepSolver
+
+from .asymmetric_step_solver import AsymmetricStepSolver
+from .extended_step_solver import ExtendedStepSolver
+from .standard_step_solver import StandardStepSolver
+from .step_solver import StepSolver
+from .symmetric_step_solver import SymmetricStepSolver
 
 
 def step_solver(
     problem: Problem, params: Params, iterate: Iterate, dt: float, rho: float
 ) -> StepSolver:
     assert dt > 0.0
     assert rho > 0.0
```

### Comparing `pygradflow-0.5.3/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.5.4/pygradflow/step/solver/asymmetric_step_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import numpy as np
 import scipy as sp
 
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params
 from pygradflow.problem import Problem
 from pygradflow.step.linear_solver import LinearSolverError
-from pygradflow.step.scaled_step_solver import ScaledStepSolver
-from pygradflow.step.step_control import StepSolverError
+from pygradflow.step.step_solver_error import StepSolverError
+
+from .scaled_step_solver import ScaledStepSolver
 
 
 class AsymmetricStepSolver(ScaledStepSolver):
     def __init__(
         self,
         problem: Problem,
         params: Params,
```

### Comparing `pygradflow-0.5.3/pygradflow/step/box_control.py` & `pygradflow-0.5.4/pygradflow/step/box_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             return solve_box_constrained(
                 iterate.x, objective, gradient, hessian, problem.var_lb, problem.var_ub
             )
         except BoxSolverError as e:
             raise StepSolverError("Box-constrained solver failed to converge") from e
 
     def step(
-        self, iterate, rho: float, dt: float, next_steps, display: bool, timer
+        self, iterate, rho: float, dt: float, display: bool, timer
     ) -> StepControlResult:
 
         lamb = 1.0 / dt
 
         problem = self.problem
         params = self.params
```

### Comparing `pygradflow-0.5.3/pygradflow/step/box_solver.py` & `pygradflow-0.5.4/pygradflow/step/box_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/step/cond_estimate.py` & `pygradflow-0.5.4/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.5.4/pygradflow/step/distance_ratio_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import numpy as np
 
 from pygradflow.controller import ControllerSettings, LogController
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.log import logger
 from pygradflow.params import Params
 from pygradflow.problem import Problem
-from pygradflow.step.step_control import StepController, StepControlResult
+from pygradflow.step.newton_control import NewtonController
+from pygradflow.step.step_control import StepControlResult
 
 
-class DistanceRatioController(StepController):
+class DistanceRatioController(NewtonController):
     def __init__(self, problem: Problem, params: Params) -> None:
         super().__init__(problem, params)
         settings = ControllerSettings.from_params(params)
         self.controller = LogController(settings, params.theta_ref)
 
-    def step(self, iterate, rho, dt, next_steps, display, timer):
+    def step(self, iterate, rho, dt, display, timer):
         assert dt > 0.0
         lamb = 1.0 / dt
 
         problem = self.problem
         params = self.params
 
+        next_steps = self.newton_steps(iterate, rho, dt)
+
         func = ImplicitFunc(problem, iterate, dt)
 
         mid_step = next(next_steps)
         mid_iterate = mid_step.iterate
 
         self.display_step(0, mid_step)
```

### Comparing `pygradflow-0.5.3/pygradflow/step/exact_control.py` & `pygradflow-0.5.4/pygradflow/step/exact_control.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import numpy as np
 
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.log import logger
-from pygradflow.step.step_control import (
-    StepController,
-    StepControlResult,
-    StepSolverError,
-)
+from pygradflow.step.newton_control import NewtonController
+from pygradflow.step.step_control import StepControlResult
+from pygradflow.step.step_solver_error import StepSolverError
 
 
-class ExactController(StepController):
+class ExactController(NewtonController):
     def __init__(self, problem, params, max_num_it=10, rate_bound=0.5):
         super().__init__(problem, params)
         self.max_num_it = max_num_it
         self.rate_bound = rate_bound
 
-    def step(self, iterate, rho, dt, next_steps, display, timer):
+    def step(self, iterate, rho, dt, display, timer):
         assert dt > 0.0
         lamb = 1.0 / dt
 
         func = ImplicitFunc(self.problem, iterate, dt)
 
         def func_val(iterate):
             return np.linalg.norm(func.value_at(iterate, rho))
 
         curr_func_val = func_val(iterate)
 
+        next_steps = self.newton_steps(iterate, rho, dt)
+
         rcond = None
         active_set = None
 
         for i in range(self.max_num_it):
             next_step = next(next_steps)
             next_iterate = next_step.iterate
             active_set = next_step.active_set
```

### Comparing `pygradflow-0.5.3/pygradflow/step/extended_step_solver.py` & `pygradflow-0.5.4/pygradflow/step/solver/extended_step_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import scipy as sp
 
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params
 from pygradflow.problem import Problem
 from pygradflow.step.linear_solver import LinearSolverError
-from pygradflow.step.scaled_step_solver import ScaledStepSolver
-from pygradflow.step.step_control import StepSolverError
+from pygradflow.step.step_solver_error import StepSolverError
+
+from .scaled_step_solver import ScaledStepSolver
 
 
 class ExtendedStepSolver(ScaledStepSolver):
     """
     Extended step solver. Computes Newton step based on the
     scaled implicit function and a modified formulation in
     order to improve condition and sparsity.
```

### Comparing `pygradflow-0.5.3/pygradflow/step/linear_solver.py` & `pygradflow-0.5.4/pygradflow/step/linear_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from abc import ABC, abstractmethod
+
 import numpy as np
 import scipy as sp
 from numpy import ndarray
 
 from pygradflow.log import logger
 from pygradflow.params import LinearSolverType
 
@@ -12,15 +14,17 @@
     matrix is (near) singular. The solver attempts to recover by
     reducing the step size
     """
 
     pass
 
 
-class LinearSolver:
+class LinearSolver(ABC):
+
+    @abstractmethod
     def solve(self, b: ndarray, trans: bool = False) -> ndarray:
         raise NotImplementedError()
 
 
 class MINRESSolver(LinearSolver):
     def __init__(self, mat):
         self.mat = mat
```

### Comparing `pygradflow-0.5.3/pygradflow/step/opti_control.py` & `pygradflow-0.5.4/pygradflow/step/opti_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         x = z[: self.prob_num_vars]
         y = info["mult_g"]
 
         return (x, y)
 
 
 class OptimizingController(StepController):
-    def step(self, iterate, rho, dt, next_steps, display, timer) -> StepControlResult:
+    def step(self, iterate, rho, dt, display, timer) -> StepControlResult:
 
         problem = self.problem
         params = self.params
 
         lamb = 1.0 / dt
         implicit_problem = ImplicitProblem(iterate, lamb, rho)
         (x, y) = implicit_problem.solve(timer=timer)
```

### Comparing `pygradflow-0.5.3/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.5.4/pygradflow/step/residuum_ratio_control.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import numpy as np
 
 from pygradflow.controller import ControllerSettings, LogController
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.log import logger
 from pygradflow.params import Params
 from pygradflow.problem import Problem
-from pygradflow.step.step_control import StepController, StepControlResult
+from pygradflow.step.newton_control import NewtonController
+from pygradflow.step.step_control import StepControlResult
 
 
-class ResiduumRatioController(StepController):
+class ResiduumRatioController(NewtonController):
     def __init__(self, problem: Problem, params: Params) -> None:
         settings = ControllerSettings.from_params(params)
         self.controller = LogController(settings, params.theta_ref)
         super().__init__(problem, params)
 
-    def step(self, iterate, rho, dt, next_steps, display, timer):
+    def step(self, iterate, rho, dt, display, timer):
         assert dt > 0.0
         lamb = 1.0 / dt
 
         problem = self.problem
         params = self.params
 
+        next_steps = self.newton_steps(iterate, rho, dt)
+
         func = ImplicitFunc(problem, iterate, dt)
 
         mid_step = next(next_steps)
         mid_iterate = mid_step.iterate
 
         mid_norm = np.linalg.norm(func.value_at(mid_iterate, rho))
```

### Comparing `pygradflow-0.5.3/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.5.4/pygradflow/step/solver/scaled_step_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import numpy as np
 import scipy as sp
 
 from pygradflow.implicit_func import ScaledImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params
 from pygradflow.problem import Problem
-from pygradflow.step.step_solver import StepResult, StepSolver
+
+from .step_solver import StepResult, StepSolver
 
 
 class ScaledStepSolver(StepSolver):
     def __init__(
         self,
         problem: Problem,
         params: Params,
```

### Comparing `pygradflow-0.5.3/pygradflow/step/standard_step_solver.py` & `pygradflow-0.5.4/pygradflow/step/solver/standard_step_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import numpy as np
 
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params
 from pygradflow.problem import Problem
 from pygradflow.step.linear_solver import LinearSolverError
-from pygradflow.step.step_control import StepSolverError
-from pygradflow.step.step_solver import StepResult, StepSolver
+from pygradflow.step.step_solver_error import StepSolverError
+
+from .step_solver import StepResult, StepSolver
 
 
 class StandardStepSolver(StepSolver):
     """
     Standard Newton step solver. Computes the step based on the
     value and derivative of the implicit function.
     """
```

### Comparing `pygradflow-0.5.3/pygradflow/step/step_control.py` & `pygradflow-0.5.4/pygradflow/step/step_control.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 import abc
 import logging
-from typing import Iterator, Optional
+from typing import Optional
 
 import numpy as np
 
 from pygradflow.display import StateData, inner_display
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.log import logger
 from pygradflow.params import Params, StepControlType
 from pygradflow.problem import Problem
-from pygradflow.step.step_solver import StepResult
+from pygradflow.step.solver.step_solver import StepResult
+from pygradflow.step.step_solver_error import StepSolverError
 from pygradflow.timer import Timer
 
 
-class StepSolverError(Exception):
-    """
-    Error signaling that the step solver failed, e.g. because the
-    Newton matrix is (near) singular.
-    """
-
-    pass
-
-
 class StepControlResult:
     def __init__(
         self,
         iterate: Iterate,
         lamb: float,
         active_set,
         rcond: Optional[float],
@@ -59,53 +51,55 @@
 
     @abc.abstractmethod
     def step(
         self,
         iterate: Iterate,
         rho: float,
         dt: float,
-        next_steps: Iterator[StepResult],
         display: bool,
         timer: Timer,
     ) -> StepControlResult:
         raise NotImplementedError()
 
     def update_stepsize_after_fail(self, lamb: float) -> float:
         return 2.0 * lamb
 
     def compute_step(
         self,
         iterate: Iterate,
         rho: float,
         dt: float,
-        next_steps: Iterator[StepResult],
         display: bool,
         timer: Timer,
     ) -> StepControlResult:
         """
         Computes next step using the step method, handling
         linear algebra errors by reducing the step size.
         """
+
+        def fail_result():
+            lamb = 1.0 / dt
+            lamb = self.update_stepsize_after_fail(lamb)
+            return StepControlResult(iterate, lamb, None, None, False)
+
         try:
             self.display = None
             if display:
 
                 def res_func(next_iterate):
                     func = ImplicitFunc(self.problem, iterate, dt)
                     return np.linalg.norm(func.value_at(next_iterate, rho))
 
                 self.res_func = res_func
                 self.display = inner_display(self.problem, self.params)
                 logger.debug("     %s", self.display.header)
-            return self.step(iterate, rho, dt, next_steps, display, timer)
+            return self.step(iterate, rho, dt, display, timer)
         except StepSolverError as e:
-            logger.debug("Linear solver error during step computation: %s", e)
-            lamb = 1.0 / dt
-            lamb = self.update_stepsize_after_fail(lamb)
-            return StepControlResult(iterate, lamb, None, None, False)
+            logger.debug("Step solver error during step computation: %s", e)
+            return fail_result()
 
     def display_step(self, iteration, step):
         level = logger.getEffectiveLevel()
         if not self.display or level > logging.DEBUG:
             return
 
         iterate = step.iterate
```

### Comparing `pygradflow-0.5.3/pygradflow/step/step_solver.py` & `pygradflow-0.5.4/pygradflow/step/solver/step_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,23 +63,23 @@
 
     @property
     def hess(self) -> sp.sparse.spmatrix:
         assert self._hess is not None
         return cast(sp.sparse.spmatrix, self._hess)
 
     def linear_solver(self, mat: sp.sparse.spmatrix) -> LinearSolver:
-        from .linear_solver import linear_solver
+        from pygradflow.step.linear_solver import linear_solver
 
         solver_type = self.params.linear_solver_type
         return linear_solver(mat, solver_type)
 
     def estimate_rcond(
         self, mat: sp.sparse.spmatrix, solver: LinearSolver
     ) -> Optional[float]:
-        from .cond_estimate import ConditionEstimator
+        from pygradflow.step.cond_estimate import ConditionEstimator
 
         estimator = ConditionEstimator(mat, solver, self.params)
         rcond = None
 
         try:
             rcond = estimator.estimate_rcond()
         except LinearSolverError:
```

### Comparing `pygradflow-0.5.3/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.5.4/pygradflow/step/solver/symmetric_step_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import scipy as sp
 
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params
 from pygradflow.problem import Problem
 from pygradflow.step.linear_solver import LinearSolverError
-from pygradflow.step.scaled_step_solver import ScaledStepSolver
-from pygradflow.step.step_control import StepSolverError
+from pygradflow.step.step_solver_error import StepSolverError
+
+from .scaled_step_solver import ScaledStepSolver
 
 
 class SymmetricStepSolver(ScaledStepSolver):
     def __init__(
         self,
         problem: Problem,
         params: Params,
```

### Comparing `pygradflow-0.5.3/pygradflow/transform.py` & `pygradflow-0.5.4/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pygradflow/util.py` & `pygradflow-0.5.4/pygradflow/util.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.5.3/pyproject.toml` & `pygradflow-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.5.3"
+version = "0.5.4"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
```

### Comparing `pygradflow-0.5.3/PKG-INFO` & `pygradflow-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.5.3
+Version: 0.5.4
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

