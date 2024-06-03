# Comparing `tmp/inflation-1.0.0.tar.gz` & `tmp/inflation-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inflation-1.0.0.tar", last modified: Thu Mar  2 13:18:43 2023, max compression
+gzip compressed data, was "inflation-2.0.0.tar", last modified: Mon Jun  3 07:58:07 2024, max compression
```

## Comparing `inflation-1.0.0.tar` & `inflation-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 13:18:43.774196 inflation-1.0.0/
--rw-rw-rw-   0        0        0    35149 2023-01-15 08:23:07.000000 inflation-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-15 08:23:07.000000 inflation-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5164 2023-03-02 13:18:43.773198 inflation-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4373 2023-01-15 08:23:07.000000 inflation-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 13:18:43.728194 inflation-1.0.0/inflation/
--rw-rw-rw-   0        0        0    19295 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/InflationProblem.py
--rw-rw-rw-   0        0        0      691 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/__init__.py
--rw-rw-rw-   0        0        0     1325 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/_about.py
--rw-rw-rw-   0        0        0       22 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/_version.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:18:43.758198 inflation-1.0.0/inflation/sdp/
--rw-rw-rw-   0        0        0    93667 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/InflationSDP.py
--rw-rw-rw-   0        0        0        0 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/__init__.py
--rw-rw-rw-   0        0        0    26545 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/fast_npa.py
--rw-rw-rw-   0        0        0    17505 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/monomial_classes.py
--rw-rw-rw-   0        0        0     3949 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/monomial_utils.py
--rw-rw-rw-   0        0        0    10846 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/optimization_utils.py
--rw-rw-rw-   0        0        0    26002 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/quantum_tools.py
--rw-rw-rw-   0        0        0    24473 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/sdp_utils.py
--rw-rw-rw-   0        0        0    13667 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/sdp/writer_utils.py
--rw-rw-rw-   0        0        0      574 2023-01-15 08:23:07.000000 inflation-1.0.0/inflation/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:18:43.738194 inflation-1.0.0/inflation.egg-info/
--rw-rw-rw-   0        0        0     5164 2023-03-02 13:18:43.000000 inflation-1.0.0/inflation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-03-02 13:18:43.000000 inflation-1.0.0/inflation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 13:18:43.000000 inflation-1.0.0/inflation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-02 11:53:48.000000 inflation-1.0.0/inflation.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-03-02 13:18:43.000000 inflation-1.0.0/inflation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-02 13:18:43.000000 inflation-1.0.0/inflation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-02 13:18:43.774196 inflation-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-01-15 08:23:07.000000 inflation-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:18:43.771195 inflation-1.0.0/test/
--rw-rw-rw-   0        0        0     5958 2023-01-15 08:23:07.000000 inflation-1.0.0/test/test_factorization.py
--rw-rw-rw-   0        0        0     6318 2023-01-15 08:23:07.000000 inflation-1.0.0/test/test_functions.py
--rw-rw-rw-   0        0        0     6393 2023-01-15 08:23:07.000000 inflation-1.0.0/test/test_monomial_properties.py
--rw-rw-rw-   0        0        0     1858 2023-01-15 08:23:07.000000 inflation-1.0.0/test/test_optimize.py
--rw-rw-rw-   0        0        0    34502 2023-01-15 08:23:07.000000 inflation-1.0.0/test/test_pipeline.py
--rw-rw-rw-   0        0        0     9371 2023-01-15 08:23:07.000000 inflation-1.0.0/test/test_solvers.py
+drwxrwxr-x   0 apozas    (1000) apozas    (1000)        0 2024-06-03 07:58:07.184822 inflation-2.0.0/
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    35149 2024-03-01 23:04:53.000000 inflation-2.0.0/LICENSE
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)       54 2024-06-03 07:03:20.000000 inflation-2.0.0/MANIFEST.in
+-rw-r--r--   0 apozas    (1000) apozas    (1000)     5694 2024-06-03 07:58:07.184822 inflation-2.0.0/PKG-INFO
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     4690 2024-06-03 07:03:20.000000 inflation-2.0.0/README.md
+drwxrwxr-x   0 apozas    (1000) apozas    (1000)        0 2024-06-03 07:58:07.180822 inflation-2.0.0/inflation/
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    50008 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/InflationProblem.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)      934 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/__init__.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     1325 2024-03-01 23:04:53.000000 inflation-2.0.0/inflation/_about.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)       21 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/_version.py
+drwxrwxr-x   0 apozas    (1000) apozas    (1000)        0 2024-06-03 07:58:07.180822 inflation-2.0.0/inflation/lp/
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    92725 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/lp/InflationLP.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)        0 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/lp/__init__.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    26058 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/lp/lp_utils.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    17964 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/lp/monomial_classes.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     2814 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/lp/numbafied.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     8327 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/lp/writer_utils.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    12832 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/optimization_utils.py
+drwxrwxr-x   0 apozas    (1000) apozas    (1000)        0 2024-06-03 07:58:07.180822 inflation-2.0.0/inflation/sdp/
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)   104917 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/sdp/InflationSDP.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)        0 2024-03-01 23:04:53.000000 inflation-2.0.0/inflation/sdp/__init__.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    28241 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/sdp/fast_npa.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     6304 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/sdp/monomial_classes.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     4113 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/sdp/monomial_utils.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    20387 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/sdp/quantum_tools.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    24938 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/sdp/sdp_utils.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    17165 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/sdp/writer_utils.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     6281 2024-06-03 07:03:20.000000 inflation-2.0.0/inflation/utils.py
+drwxrwxr-x   0 apozas    (1000) apozas    (1000)        0 2024-06-03 07:58:07.180822 inflation-2.0.0/inflation.egg-info/
+-rw-r--r--   0 apozas    (1000) apozas    (1000)     5694 2024-06-03 07:58:07.000000 inflation-2.0.0/inflation.egg-info/PKG-INFO
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)      950 2024-06-03 07:58:07.000000 inflation-2.0.0/inflation.egg-info/SOURCES.txt
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)        1 2024-06-03 07:58:07.000000 inflation-2.0.0/inflation.egg-info/dependency_links.txt
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)        1 2024-03-07 02:35:55.000000 inflation-2.0.0/inflation.egg-info/not-zip-safe
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)      105 2024-06-03 07:58:07.000000 inflation-2.0.0/inflation.egg-info/requires.txt
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)       10 2024-06-03 07:58:07.000000 inflation-2.0.0/inflation.egg-info/top_level.txt
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)       38 2024-06-03 07:58:07.184822 inflation-2.0.0/setup.cfg
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     1244 2024-06-03 07:03:20.000000 inflation-2.0.0/setup.py
+drwxrwxr-x   0 apozas    (1000) apozas    (1000)        0 2024-06-03 07:58:07.180822 inflation-2.0.0/test/
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     5898 2024-06-03 07:03:20.000000 inflation-2.0.0/test/test_factorization.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    18888 2024-06-03 07:03:20.000000 inflation-2.0.0/test/test_functions.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    15872 2024-06-03 07:03:20.000000 inflation-2.0.0/test/test_monomial_properties.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)     1858 2024-03-01 23:04:53.000000 inflation-2.0.0/test/test_optimize.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    56451 2024-06-03 07:03:20.000000 inflation-2.0.0/test/test_pipeline.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    21946 2024-06-03 07:03:20.000000 inflation-2.0.0/test/test_solvers.py
+-rw-rw-r--   0 apozas    (1000) apozas    (1000)    11792 2024-06-03 07:03:20.000000 inflation-2.0.0/test/test_writers.py
```

### Comparing `inflation-1.0.0/LICENSE` & `inflation-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inflation-1.0.0/PKG-INFO` & `inflation-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,132 @@
-Metadata-Version: 2.1
-Name: inflation
-Version: 1.0.0
-Summary: Implementations of the Inflation Technique for Causal Inference
-Home-page: https://github.com/ecboghiu/inflation
-Author: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
-Author-email: cristian.boghiu@icfo.eu, ewolfe@pitp.ca, physics@alexpozas.com
-License: GNU GPL v. 3.0
-Project-URL: Documentation, https://ecboghiu.github.io/inflation/_build/html/index.html
-Project-URL: Source, https://github.com/ecboghiu/inflation
-Project-URL: Issue Tracker, https://github.com/ecboghiu/inflation/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE
-
-[![DOI](https://zenodo.org/badge/500850617.svg)](https://zenodo.org/badge/latestdoi/500850617)
-
-# Inflation
-Inflation is a Python package that implements inflation algorithms for causal inference. In causal inference, the main task is to determine which causal relationships can exist between different observed random variables. Inflation algorithms are a class of techniques designed to solve the causal compatibility problem, that is, test compatibility between some observed data and a given causal relationship.
-
-The first version of this package implements the inflation technique for quantum causal compatibility. For details, see [Physical Review X 11 (2), 021043 (2021)](https://journals.aps.org/prx/abstract/10.1103/PhysRevX.11.021043). The inflation technique for classical causal compatibility will be implemented in a future update.
-
-Examples of use of this package include:
-
-- Feasibility problems and extraction of certificates.
-- Optimization of Bell operators.
-- Optimisation over classical distributions.
-- Standard [NavascuÃ©s-Pironio-AcÃ­n hierarchy](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.010401).
-- Scenarios with partial information.
-
-See the documentation for more details.
-
-## Documentation
-
-* [Latest version](https://ecboghiu.github.io/inflation/).
-
-## Installation
-
-To install the package, run the following command:
-
-```
-pip install inflation
-```
-
-You can also install directly from GitHub with:
-
-```
-pip install git+https://github.com/ecboghiu/inflation.git@main
-```
-
-or download the repository on your computer and run `pip install .` in the repository folder. Install the `devel` branch for the latest features and bugfixes.
-
-Tests are written outside the Python module, therefore they are not installed together with the package. To test the installation, clone the repository and run, in a Unix terminal,
-```python -m unittest -v```
-inside the repository folder.
-
-## Example
-
-The following example shows that the W distribution is incompatible with the triangle scenario with quantum sources by showing that a specific semidefinite programming relaxation is infeasible:
-
-```python
-from inflation import InflationProblem, InflationSDP
-import numpy as np
-
-P_W = np.zeros((2, 2, 2, 1, 1, 1))
-for a, b, c, x, y, z in np.ndindex(*P_W.shape):
-    if a + b + c == 1:
-        P_W[a, b, c, x, y, z] = 1 / 3
-
-triangle = InflationProblem(dag={"rho_AB": ["A", "B"],
-                                 "rho_BC": ["B", "C"],
-                                 "rho_AC": ["A", "C"]},
-                             outcomes_per_party=(2, 2, 2),
-                             settings_per_party=(1, 1, 1),
-                             inflation_level_per_source=(2, 2, 2))
-
-sdp = InflationSDP(triangle, verbose=1)
-sdp.generate_relaxation('npa2')
-sdp.set_distribution(P_W)
-sdp.solve()
-
-print("Problem status:", sdp.status)
-print("Infeasibility certificate:", sdp.certificate_as_probs())
-```
-
-For more information about the theory and other features, please visit the [documentation](https://ecboghiu.github.io/inflation/), and more specifically the [Tutorial](https://ecboghiu.github.io/inflation/_build/html/tutorial.html) and [Examples](https://ecboghiu.github.io/inflation/_build/html/examples.html) pages.
-
-## How to contribute
-
-Contributions are welcome and appreciated. If you want to contribute, you can read the [contribution guidelines](https://github.com/ecboghiu/inflation/blob/main/CONTRIBUTE.md). You can also read the [documentation](https://ecboghiu.github.io/inflation/) to learn more about how the package works.
-
-## License
-
-Inflation is free open-source software released under [GNU GPL v. 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
-
-## Citing Inflation
-
-If you use Inflation in your work, please cite [Inflation's paper](https://www.arxiv.org/abs/2211.04483):
-
-- Emanuel-Cristian Boghiu, Elie Wolfe and Alejandro Pozas-Kerstjens, "Inflation: a Python package for classical and quantum causal compatibility", arXiv:2211.04483
-
-```
-@misc{2211.04483,
-  doi = {10.48550/arXiv.2211.04483},
-  url = {https://arxiv.org/abs/2211.04483},
-  author = {Boghiu, Emanuel-Cristian and Wolfe, Elie and Pozas-Kerstjens, Alejandro},
-  title = {{Inflation}: a {Python} package for classical and quantum causal compatibility},
-  publisher = {arXiv},
-  year = {2022},
-  copyright = {arXiv.org perpetual, non-exclusive license}
-}
-```
+Metadata-Version: 2.1
+Name: inflation
+Version: 2.0.0
+Summary: Implementations of the Inflation Technique for Causal Inference
+Home-page: https://github.com/ecboghiu/inflation
+Author: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
+Author-email: cristian.boghiu@icfo.eu, ewolfe@pitp.ca, physics@alexpozas.com
+License: GNU GPL v. 3.0
+Project-URL: Documentation, https://ecboghiu.github.io/inflation/_build/html/index.html
+Project-URL: Source, https://github.com/ecboghiu/inflation
+Project-URL: Issue Tracker, https://github.com/ecboghiu/inflation/issues
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: mosek>=10
+Requires-Dist: networkx
+Requires-Dist: numba
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: sympy
+Requires-Dist: tqdm
+Provides-Extra: docs
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: m2r2; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx_copybutton; extra == "docs"
+
+[![DOI](https://zenodo.org/badge/500850617.svg)](https://zenodo.org/badge/latestdoi/500850617)
+
+# Inflation
+Inflation is a Python package that implements inflation algorithms for causal inference. In causal inference, the main task is to determine which causal relationships can exist between different observed random variables. Inflation algorithms are a class of techniques designed to solve the causal compatibility problem, that is, test compatibility between some observed data and a given causal relationship.
+
+The first version of this package implements the inflation technique for quantum causal compatibility. For details, see [Physical Review X 11 (2), 021043 (2021)](https://journals.aps.org/prx/abstract/10.1103/PhysRevX.11.021043). The inflation technique for classical causal compatibility will be implemented in a future update.
+
+Examples of use of this package include:
+
+- Feasibility problems and extraction of certificates.
+- Optimization of Bell operators.
+- Optimisation over classical distributions.
+- Standard [Navascués-Pironio-Acín hierarchy](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.010401).
+- Scenarios with partial information.
+- Possibilistic compatibility with a causal network.
+- Estimation of do-conditionals and causal strengths.
+
+See the documentation for more details.
+
+## Documentation
+
+* [Latest version](https://ecboghiu.github.io/inflation/).
+
+## Installation
+
+To install the package, run the following command:
+
+```
+pip install inflation
+```
+
+You can also install directly from GitHub with:
+
+```
+pip install git+https://github.com/ecboghiu/inflation.git@main
+```
+
+or download the repository on your computer and run `pip install .` in the repository folder. Install the `devel` branch for the latest features and bugfixes.
+
+Tests are written outside the Python module, therefore they are not installed together with the package. To test the installation, clone the repository and run, in a Unix terminal,
+```python -m unittest -v```
+inside the repository folder.
+
+## Example
+
+The following example shows that the W distribution is incompatible with the triangle scenario with quantum sources by showing that a specific semidefinite programming relaxation is infeasible:
+
+```python
+from inflation import InflationProblem, InflationSDP
+import numpy as np
+
+P_W = np.zeros((2, 2, 2, 1, 1, 1))
+for a, b, c, x, y, z in np.ndindex(*P_W.shape):
+    if a + b + c == 1:
+        P_W[a, b, c, x, y, z] = 1 / 3
+
+triangle = InflationProblem(dag={"rho_AB": ["A", "B"],
+                                 "rho_BC": ["B", "C"],
+                                 "rho_AC": ["A", "C"]},
+                             outcomes_per_party=(2, 2, 2),
+                             settings_per_party=(1, 1, 1),
+                             inflation_level_per_source=(2, 2, 2))
+
+sdp = InflationSDP(triangle, verbose=1)
+sdp.generate_relaxation('npa2')
+sdp.set_distribution(P_W)
+sdp.solve()
+
+print("Problem status:", sdp.status)
+print("Infeasibility certificate:", sdp.certificate_as_probs())
+```
+
+For more information about the theory and other features, please visit the [documentation](https://ecboghiu.github.io/inflation/), and more specifically the [Tutorial](https://ecboghiu.github.io/inflation/_build/html/tutorial.html) and [Examples](https://ecboghiu.github.io/inflation/_build/html/examples.html) pages.
+
+## How to contribute
+
+Contributions are welcome and appreciated. If you want to contribute, you can read the [contribution guidelines](https://github.com/ecboghiu/inflation/blob/main/CONTRIBUTE.md). You can also read the [documentation](https://ecboghiu.github.io/inflation/) to learn more about how the package works.
+
+## License
+
+Inflation is free open-source software released under [GNU GPL v. 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+## Citing Inflation
+
+If you use Inflation in your work, please cite [Inflation's paper](https://www.arxiv.org/abs/2211.04483):
+
+- Emanuel-Cristian Boghiu, Elie Wolfe and Alejandro Pozas-Kerstjens, "Inflation: a Python package for classical and quantum causal compatibility", Quantum **7**, 996 (2023), arXiv:2211.04483
+
+```
+@article{pythoninflation,
+  doi = {10.22331/q-2023-05-04-996},
+  url = {https://doi.org/10.22331/q-2023-05-04-996},
+  title = {Inflation: a {P}ython library for classical and quantum causal compatibility},
+  author = {Boghiu, Emanuel-Cristian and Wolfe, Elie and Pozas-Kerstjens, Alejandro},
+  journal = {{Quantum}},
+  issn = {2521-327X},
+  publisher = {{Verein zur F{\"{o}}rderung des Open Access Publizierens in den Quantenwissenschaften}},
+  volume = {7},
+  pages = {996},
+  month = may,
+  year = {2023},
+  archivePrefix = {arXiv},
+  eprint = {2211.04483}
+}
+```
```

### Comparing `inflation-1.0.0/README.md` & `inflation-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 Examples of use of this package include:
 
 - Feasibility problems and extraction of certificates.
 - Optimization of Bell operators.
 - Optimisation over classical distributions.
 - Standard [Navascués-Pironio-Acín hierarchy](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.010401).
 - Scenarios with partial information.
+- Possibilistic compatibility with a causal network.
+- Estimation of do-conditionals and causal strengths.
 
 See the documentation for more details.
 
 ## Documentation
 
 * [Latest version](https://ecboghiu.github.io/inflation/).
 
@@ -78,20 +80,26 @@
 
 Inflation is free open-source software released under [GNU GPL v. 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
 
 ## Citing Inflation
 
 If you use Inflation in your work, please cite [Inflation's paper](https://www.arxiv.org/abs/2211.04483):
 
-- Emanuel-Cristian Boghiu, Elie Wolfe and Alejandro Pozas-Kerstjens, "Inflation: a Python package for classical and quantum causal compatibility", arXiv:2211.04483
+- Emanuel-Cristian Boghiu, Elie Wolfe and Alejandro Pozas-Kerstjens, "Inflation: a Python package for classical and quantum causal compatibility", Quantum **7**, 996 (2023), arXiv:2211.04483
 
 ```
-@misc{2211.04483,
-  doi = {10.48550/arXiv.2211.04483},
-  url = {https://arxiv.org/abs/2211.04483},
+@article{pythoninflation,
+  doi = {10.22331/q-2023-05-04-996},
+  url = {https://doi.org/10.22331/q-2023-05-04-996},
+  title = {Inflation: a {P}ython library for classical and quantum causal compatibility},
   author = {Boghiu, Emanuel-Cristian and Wolfe, Elie and Pozas-Kerstjens, Alejandro},
-  title = {{Inflation}: a {Python} package for classical and quantum causal compatibility},
-  publisher = {arXiv},
-  year = {2022},
-  copyright = {arXiv.org perpetual, non-exclusive license}
+  journal = {{Quantum}},
+  issn = {2521-327X},
+  publisher = {{Verein zur F{\"{o}}rderung des Open Access Publizierens in den Quantenwissenschaften}},
+  volume = {7},
+  pages = {996},
+  month = may,
+  year = {2023},
+  archivePrefix = {arXiv},
+  eprint = {2211.04483}
 }
 ```
```

### Comparing `inflation-1.0.0/inflation/__init__.py` & `inflation-2.0.0/inflation/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 ==================
 Provides
  1. A tool for describing causal scenarios and reducing them to network form
     (see the definitions of network and non-network causal scenarios in
     arXiv:1707.06476 and arXiv:1909.10519).
  2. A tool for setting up and solving feasibility and optimization problems
     over probability distributions compatible with quantum causal scenarios.
+ 3. A tool for setting up and solving feasibility and optimization problems
+    over probability distributions compatible with theory-independent and
+    classical causal scenarios
 """
 
 from .InflationProblem import InflationProblem
 from .sdp.InflationSDP import InflationSDP
-from .sdp.optimization_utils import max_within_feasible
+from .lp.InflationLP import InflationLP
+from .optimization_utils import max_within_feasible
 from ._about import about
 from ._version import __version__
 
 __all__ = ["InflationProblem",
            "InflationSDP",
+           "InflationLP",
            "max_within_feasible"]
```

### Comparing `inflation-1.0.0/inflation/_about.py` & `inflation-2.0.0/inflation/_about.py`

 * *Files identical despite different names*

### Comparing `inflation-1.0.0/inflation/sdp/InflationSDP.py` & `inflation-2.0.0/inflation/sdp/InflationSDP.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,113 +1,106 @@
 """
 The module generates the semidefinite program associated to a quantum inflation
 instance (see arXiv:1909.10519).
 
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
 """
-import numpy as np
-import sympy as sp
-
-from collections import Counter, deque
-from functools import reduce
+from collections import Counter, deque, defaultdict
+from functools import reduce, cached_property
 from gc import collect
-from itertools import chain, count, product, permutations, repeat
-from operator import itemgetter
+from itertools import chain, count, product, repeat, combinations
 from numbers import Real
-from scipy.sparse import lil_matrix
-from tqdm import tqdm
+from operator import itemgetter
 from typing import List, Dict, Tuple, Union, Any
 from warnings import warn
 
+import numpy as np
+import sympy as sp
+from scipy.sparse import lil_matrix
+from tqdm import tqdm
+
 from inflation import InflationProblem
-from .fast_npa import (nb_all_commuting_q,
-                       apply_source_perm,
-                       commutation_matrix,
-                       nb_mon_to_lexrepr,
-                       reverse_mon,
-                       to_canonical)
 from .fast_npa import nb_is_knowable as is_knowable
-from .monomial_classes import InternalAtomicMonomial, CompoundMonomial
+from .fast_npa import (reverse_mon,
+                       to_canonical_1d_internal
+                       )
+from .monomial_classes import InternalAtomicMonomialSDP, CompoundMomentSDP
 from .quantum_tools import (apply_inflation_symmetries,
-                            calculate_momentmatrix,
-                            clean_coefficients,
+                            calculate_momentmatrix_1d_internal,
                             construct_normalization_eqs,
-                            expand_moment_normalisation,
                             flatten_symbolic_powers,
-                            format_permutations,
-                            generate_operators,
-                            party_physical_monomials,
-                            reduce_inflation_indices,
-                            to_symbol)
+                            generate_operators
+                            )
 from .sdp_utils import solveSDP_MosekFUSION
 from .writer_utils import (write_to_csv,
                            write_to_mat,
                            write_to_sdpa)
-from ..utils import flatten
-
+from ..lp.numbafied import nb_outer_bitwise_or
+from ..utils import clean_coefficients, partsextractor
 
-class InflationSDP(object):
-    """
-    Class for generating and solving an SDP relaxation for quantum inflation.
 
-    Parameters
-    ----------
-    inflationproblem : InflationProblem
-        Details of the scenario.
-    commuting : bool, optional
-        Whether variables in the problem are going to be commuting (classical
-        problem) or non-commuting (quantum problem). By default ``False``.
-    supports_problem : bool, optional
-        Whether to consider feasibility problems with distributions, or just
-        with the distribution's support. By default ``False``.
-    verbose : int, optional
-        Optional parameter for level of verbose:
-
-            * 0: quiet (default),
-            * 1: monitor level: track program process and show warnings,
-            * 2: debug level: show properties of objects created.
+class InflationSDP:
+    """Class for generating and solving an SDP relaxation for quantum inflation.
     """
     constant_term_name = "constant_term"
 
     def __init__(self,
                  inflationproblem: InflationProblem,
-                 commuting: bool = False,
                  supports_problem: bool = False,
-                 verbose=None) -> None:
-        """Constructor for the InflationSDP class.
+                 include_all_outcomes: bool = False,
+                 commuting: bool = False,
+                 verbose: int = 0) -> None:
+        """
+        Class for generating and solving an SDP relaxation for quantum inflation.
+
+        Parameters
+        ----------
+        inflationproblem : InflationProblem
+            Details of the scenario.
+        supports_problem : bool, optional
+            Whether to consider feasibility problems with distributions, or just
+            with the distribution's support. By default ``False``.
+        verbose : int, optional
+            Optional parameter for level of verbose:
+
+                * 0: quiet (default),
+                * 1: monitor level: track program process and show warnings,
+                * 2: debug level: show properties of objects created.
         """
+        
+        self.problem_type = "sdp"
         self.supports_problem = supports_problem
         if verbose is not None:
             if inflationproblem.verbose > verbose:
                 warn("Overriding the verbosity from InflationProblem")
             self.verbose = verbose
         else:
             self.verbose = inflationproblem.verbose
-        self.commuting = commuting
         self.InflationProblem = inflationproblem
-        self.names = self.InflationProblem.names
+        self.names = inflationproblem.names
         self.names_to_ints = {name: i + 1 for i, name in enumerate(self.names)}
         if self.verbose > 1:
-            print(self.InflationProblem)
+            print(inflationproblem)
 
         self.nr_parties = len(self.names)
-        self.nr_sources = self.InflationProblem.nr_sources
-        self.hypergraph = self.InflationProblem.hypergraph
-        self.inflation_levels = \
-            self.InflationProblem.inflation_level_per_source
-        self.has_children = self.InflationProblem.has_children
-        self.outcome_cardinalities = \
-            self.InflationProblem.outcomes_per_party.copy()
-        if self.supports_problem:
-            # Support problems must not use Collins-Gisin notation
-            self.has_children = np.ones(self.nr_parties, dtype=int)
-        else:
-            self.has_children = self.InflationProblem.has_children
+        self.nr_sources = inflationproblem.nr_sources
+        self.hypergraph = inflationproblem.hypergraph
+        self.inflation_levels = inflationproblem.inflation_level_per_source
+        self.has_children = inflationproblem.has_children
+        self.outcome_cardinalities = inflationproblem.outcomes_per_party.copy()
+        self.has_children = inflationproblem.has_children.copy()
+        if include_all_outcomes or supports_problem:  
+            # HACK to fix detection of incompatible supports. 
+            # (Can be fixed upon adding set_extra_equalities)
+            self.has_children[:] = True
+
+
         self.outcome_cardinalities += self.has_children
-        self.setting_cardinalities = self.InflationProblem.settings_per_party
+        self.setting_cardinalities = inflationproblem.settings_per_party
+        self._quantum_sources = inflationproblem._nonclassical_sources
 
         self.measurements = self._generate_parties()
         if self.verbose > 1:
             print("Number of single operator measurements per party:", end="")
             prefix = " "
             for i, measures in enumerate(self.measurements):
                 counter = count()
@@ -115,55 +108,103 @@
                     chain.from_iterable(measures)),
                           counter),
                       maxlen=0)
                 print(prefix + f"{self.names[i]}={next(counter)}", end="")
                 prefix = ", "
             print()
         self.use_lpi_constraints = False
-        self.network_scenario    = self.InflationProblem.is_network
+        self.network_scenario    = inflationproblem.is_network
         self._is_knowable_q_non_networks = \
-            self.InflationProblem._is_knowable_q_non_networks
-        self.rectify_fake_setting = self.InflationProblem.rectify_fake_setting
-        self.factorize_monomial = self.InflationProblem.factorize_monomial
-
-        self._nr_operators = len(flatten(self.measurements))
-        self._nr_properties = 1 + self.nr_sources + 2
-        self.np_dtype = np.find_common_type([
-            np.min_scalar_type(np.max(self.setting_cardinalities)),
-            np.min_scalar_type(np.max(self.outcome_cardinalities)),
-            np.min_scalar_type(self.nr_parties + 1),
-            np.min_scalar_type(np.max(self.inflation_levels) + 1)], [])
+            inflationproblem._is_knowable_q_non_networks
+        self.rectify_fake_setting = inflationproblem.rectify_fake_setting
+        # self.factorize_monomial_2d = inflationproblem.factorize_monomial_2d
+        self.factorize_moment_1d = inflationproblem.factorize_monomial_1d
+
+        # self._nr_operators = len(flatten(self.measurements))
+        self._nr_properties = inflationproblem._nr_properties
+        self.np_dtype = inflationproblem._np_dtype
+        self._astuples_dtype = inflationproblem._astuples_dtype
         self.identity_operator = np.empty((0, self._nr_properties),
                                           dtype=self.np_dtype)
         self.zero_operator = np.zeros((1, self._nr_properties),
                                       dtype=self.np_dtype)
 
-        # Define default lexicographic order through np.lexsort
-        lexorder = self._interpret_name(flatten(self.measurements))
-        lexorder = np.concatenate((self.zero_operator, lexorder))
-        self._default_lexorder = lexorder[np.lexsort(np.rot90(lexorder))]
+        self._default_lexorder = np.concatenate((self.zero_operator, 
+                                                 inflationproblem._lexorder)
+                                                ).astype(self.np_dtype)
+        self._nr_operators = inflationproblem._nr_operators + 1
+        self.blank_bool_vec = np.zeros(self._nr_operators, dtype=bool)
         self._lexorder = self._default_lexorder.copy()
+        self.op_to_lexrepr_dict = {tuple(op): i for i, op in enumerate(self._lexorder)}
+        self._lexorder_len = len(self._lexorder)
+        self.lexorder_symmetries = \
+            np.pad(inflationproblem.lexorder_symmetries + 1, ((0, 0), (1, 0)))
+
+        self._lexrepr_to_names = \
+            np.hstack((["0"], inflationproblem._lexrepr_to_names))
+        self._lexrepr_to_copy_index_free_names = \
+            np.hstack((["0"], inflationproblem._lexrepr_to_copy_index_free_names))
+        self.op_from_name = {"0": 0}
+        for i, op_names in enumerate(inflationproblem._lexrepr_to_all_names.tolist()):
+            for op_name in op_names:
+                self.op_from_name.setdefault(op_name, i+1)
+        self._lexrepr_to_symbols = \
+            np.hstack(([sp.S.Zero], inflationproblem._lexrepr_to_symbols))
+
+        #Construct orthogonality matrix for recognizing zeros
+        self._orthomat = np.zeros((self._lexorder_len, self._lexorder_len),
+                                  dtype=bool)
+        for ((i, j), (op_i, op_j)) in zip(
+                combinations(range(self._lexorder_len), 2),
+                combinations(self._lexorder, 2)):
+            if (op_i[-1] != op_j[-1] and np.array_equal(op_i[:-1], op_j[:-1])):
+                self._orthomat[i, j] = True
+                self._orthomat[j, i] = True
+        self._orthomat[:, 0] = True
+        self._orthomat[0, :] = True
+
+        # Translating the compatibility matrix of InflationProblem to
+        # a commutativity matrix for InflationSDP.
+        # # InflationProblem has more operators in ._lexorder than InflationSDP
+        # This is because events with the last outcome are included in
+        # InflationProblem. We carefully avoid this by using .mon_to_lexrepr
+        # of InflationProblem on the operators in InflationSDP._lexorder
+        assert np.allclose(self._lexorder[0], self.zero_operator), \
+            "The first element of the lexorder should be the zero operator"
+        self._default_notcomm = \
+            np.pad(inflationproblem._default_notcomm,
+                       ((1, 0), (1, 0)))
 
-        self._default_notcomm = commutation_matrix(self._lexorder,
-                                                   self.commuting)
         self._notcomm = self._default_notcomm.copy()
-        self.all_commuting_q = lambda mon: nb_all_commuting_q(mon,
-                                                              self._lexorder,
-                                                              self._notcomm)
+        self.all_operators_commute = not self._notcomm.any()
+        if commuting:
+            assert self.all_operators_commute, \
+                "You appear to be requesting commuting (classical)" \
+                    + " inflation, \nbut have not specified classical_sources=`all`." \
+                    + "\nNote that the `commuting` keyword argument has been deprecated as of release 2.0.0"
+        if self.all_operators_commute:
+            self.all_commuting_q_2d = lambda mon: True
+            self.all_commuting_q_1d = lambda lexmon: True
+        else:
+            self.all_commuting_q_1d = \
+                lambda lexmon: not self._notcomm[np.ix_(lexmon, lexmon)].any()
+            self.all_commuting_q_2d = \
+                lambda mon: self.all_commuting_q_1d(self.mon_to_lexrepr(mon))
 
-        self.canon_ndarray_from_hash    = dict()
-        self.canonsym_ndarray_from_hash = dict()
+        self.canon_lexmon_from_hash     = dict()
+        self.canonsym_lexmon_from_hash  = dict()
         # These next properties are reset during generate_relaxation, but
         # are needed in init so as to be able to test the Monomial constructor
         # function without generate_relaxation.
         self.atomic_monomial_from_hash  = dict()
         self.monomial_from_atoms        = dict()
         self.monomial_from_name         = dict()
-        self.Zero = self.Monomial(self.zero_operator, idx=0)
-        self.One  = self.Monomial(self.identity_operator, idx=1)
+        self.monomial_from_symbol       = dict()
+        self.Zero = self.Moment_2d(self.zero_operator, idx=0)
+        self.One  = self.Moment_2d(self.identity_operator, idx=1)
         self._relaxation_has_been_generated = False
 
     ###########################################################################
     # MAIN ROUTINES EXPOSED TO THE USER                                       #
     ###########################################################################
     def generate_relaxation(self,
                             column_specification:
@@ -237,157 +278,175 @@
               the measurement operators in ``InflationSDP.measurements``. This
               list needs to have the identity ``sympy.S.One`` as the first
               element.
         """
         self.atomic_monomial_from_hash  = dict()
         self.monomial_from_atoms        = dict()
         self.monomial_from_name         = dict()
-        self.Zero = self.Monomial(self.zero_operator, idx=0)
-        self.One  = self.Monomial(self.identity_operator, idx=1)
+        self.monomial_from_symbol       = dict()
+        self.Zero = self.Moment_2d(self.zero_operator, idx=0)
+        self.One  = self.Moment_2d(self.identity_operator, idx=1)
+        self.Constant_Term = self.One.__copy__()
+        self.Constant_Term.name = self.constant_term_name
+        self.monomial_from_name[self.constant_term_name] = self.Constant_Term
 
-        generating_monomials = self.build_columns(column_specification)
-        # Generate dictionary to indices (used in dealing with symmetries and
-        # column-level equalities)
-        genmon_hash_to_index = {self._from_2dndarray(op): i
-                                for i, op in enumerate(generating_monomials)}
-        # Check for duplicates
-        if len(genmon_hash_to_index) < len(generating_monomials):
-            generating_monomials = [generating_monomials[i]
-                                    for i in genmon_hash_to_index.values()]
-            genmon_hash_to_index = {hash: i for i, hash
-                                    in enumerate(genmon_hash_to_index.keys())}
-            if self.verbose > 0:
-                warn("Duplicates were detected in the list of generating " +
-                     "monomials and automatically removed.")
-        self.genmon_hash_to_index = genmon_hash_to_index
-        self.n_columns            = len(generating_monomials)
-        self.generating_monomials = generating_monomials
-        del generating_monomials, genmon_hash_to_index
+        self.build_columns(column_specification)
         collect()
         if self.verbose > 0:
             print("Number of columns in the moment matrix:", self.n_columns)
 
         # Calculate the moment matrix without the inflation symmetries
-        unsymmetrized_mm, unsymmetrized_corresp = self._build_momentmatrix()
+        unsymmetrized_mm, unsymmetrized_corresp = \
+            self._build_momentmatrix_1d_internal()
         symmetrization_required = np.any(self.inflation_levels - 1)
         additional_var = 0
         if self.verbose > 1:
             extra_msg = (" before symmetrization" if symmetrization_required
                          else "")
             if 0 in unsymmetrized_mm.flat:
                 additional_var = 1
             print("Number of variables" + extra_msg + ":",
                   len(unsymmetrized_corresp) + additional_var)
 
         # Calculate the inflation symmetries
-        self.inflation_symmetries = self._discover_inflation_symmetries()
+        self.columns_symmetries = self._discover_columns_symmetries()
 
         # Apply the inflation symmetries to the moment matrix
         self.momentmatrix, self.orbits, representative_unsym_idxs = \
             apply_inflation_symmetries(unsymmetrized_mm,
-                                       self.inflation_symmetries,
+                                       self.columns_symmetries,
                                        self.verbose)
         self.symmetrized_corresp = \
             {self.orbits[idx]: unsymmetrized_corresp[idx]
              for idx in representative_unsym_idxs.flat if idx >= 1}
-        unsymidx_from_hash = {self._from_2dndarray(mon): idx for (idx, mon) in
-                              unsymmetrized_corresp.items()
-                              if self.all_commuting_q(mon)}
-        for (hash, idx) in unsymidx_from_hash.items():
-            self.canonsym_ndarray_from_hash[hash] = \
-                self.symmetrized_corresp[self.orbits[idx]]
         if self.verbose > 0:
             extra_msg = (" after symmetrization" if symmetrization_required
                          else "")
             print(f"Number of variables{extra_msg}: "
                   + f"{len(self.symmetrized_corresp)+additional_var}")
-        del unsymidx_from_hash, unsymmetrized_mm, unsymmetrized_corresp, \
+        del unsymmetrized_mm, unsymmetrized_corresp, \
             symmetrization_required, additional_var
-        # This is a good time to reclaim memory, as unsymmetrized_mm can be GBs
         collect()
 
         self.momentmatrix_has_a_zero, self.momentmatrix_has_a_one = \
             np.in1d([0, 1], self.momentmatrix.ravel())
 
         # Associate Monomials to the remaining entries. The zero monomial is
         # not stored during calculate_momentmatrix
-        self.compmonomial_from_idx = dict()
+        self.compmoment_from_idx = dict()
         if self.momentmatrix_has_a_zero:
-            self.compmonomial_from_idx[0] = self.Zero
-        for (idx, mon) in tqdm(self.symmetrized_corresp.items(),
+            self.compmoment_from_idx[0] = self.Zero
+        for (idx, lexmon) in tqdm(self.symmetrized_corresp.items(),
                                disable=not self.verbose,
                                desc="Initializing monomials   "):
-            self.compmonomial_from_idx[idx] = self.Monomial(mon, idx)
-        self.first_free_idx = max(self.compmonomial_from_idx.keys()) + 1
-
-        self.monomials = list(self.compmonomial_from_idx.values())
+            self.compmoment_from_idx[idx] = self.Moment_1d(lexmon, idx)
+        self.first_free_idx = max(self.compmoment_from_idx.keys()) + 1
+        self.moments = list(self.compmoment_from_idx.values())
+        self.monomials = list(self.compmoment_from_idx.values())
+        
         assert all(v == 1 for v in Counter(self.monomials).values()), \
             "Multiple indices are being associated to the same monomial"
-        knowable_atoms = set()
-        for mon in self.monomials:
-            knowable_atoms.update(mon.knowable_factors)
-        self.knowable_atoms = [self._monomial_from_atoms([atom])
-                               for atom in knowable_atoms]
-        del knowable_atoms
 
-        _counter = Counter([mon.knowability_status for mon in self.monomials])
+        _counter = Counter([mon.knowability_status for mon in self.moments])
         self.n_knowable           = _counter["Knowable"]
         self.n_something_knowable = _counter["Semi"]
         self.n_unknowable         = _counter["Unknowable"]
         if self.verbose > 1:
-            print(f"The problem has {self.n_knowable} knowable monomials, " +
-                  f"{self.n_something_knowable} semi-knowable monomials, " +
-                  f"and {self.n_unknowable} unknowable monomials.")
+            print(f"The problem has {self.n_knowable} knowable moments, " +
+                  f"{self.n_something_knowable} semi-knowable moments, " +
+                  f"and {self.n_unknowable} unknowable moments.")
 
-        if self.commuting:
-            self.physical_monomials = self.monomials
+        if self.all_operators_commute:
+            self.hermitian_moments = self.moments
         else:
-            self.physical_monomials = [mon for mon in self.monomials
-                                       if mon.is_physical]
+            self.hermitian_moments = [mon for mon in self.moments
+                                      if mon.is_hermitian]
             if self.verbose > 1:
-                print(f"The problem has {len(self.physical_monomials)} " +
-                      "non-negative monomials.")
+                print(f"The problem has {len(self.hermitian_moments)} " +
+                      "non-negative moments.")
 
         # This dictionary useful for certificates_as_probs
         self.names_to_symbols = {mon.name: mon.symbol
-                                 for mon in self.monomials}
+                                 for mon in self.moments}
         self.names_to_symbols[self.constant_term_name] = sp.S.One
 
         # In non-network scenarios we do not use Collins-Gisin notation for
         # some variables, so there exist normalization constraints between them
-        self.moment_equalities = []
+        self.minimal_equalities = []
         if not self.network_scenario or self.supports_problem:
             self.column_level_equalities = self._discover_normalization_eqns()
             self.idx_level_equalities    = construct_normalization_eqs(
                                                 self.column_level_equalities,
                                                 self.momentmatrix,
                                                 self.verbose)
             if self.verbose > 1 and len(self.idx_level_equalities):
                 print("Number of normalization equalities:",
                       len(self.idx_level_equalities))
             for (norm_idx, summation_idxs) in self.idx_level_equalities:
-                eq_dict = {self.compmonomial_from_idx[norm_idx]: 1}
+                eq_dict = {self.compmoment_from_idx[norm_idx]: 1}
                 eq_dict.update(zip(
-                    itemgetter(*summation_idxs)(self.compmonomial_from_idx),
+                    itemgetter(*summation_idxs)(self.compmoment_from_idx),
                     repeat(-1)
                 ))
-                self.moment_equalities.append(eq_dict)
+                self.minimal_equalities.append(eq_dict)
 
-        self.moment_inequalities = []
+        self.minimal_inequalities = []
         self.moment_upperbounds  = dict()
-        self.moment_lowerbounds  = {m: 0. for m in self.physical_monomials}
+        self.moment_lowerbounds  = {m: 0. for m in self.hermitian_moments}
 
-        self._set_lowerbounds(None)
-        self._set_upperbounds(None)
         self.set_objective(None)
         self.set_values(None)
 
         self.maskmatrices = dict()
         self._relaxation_has_been_generated = True
 
+    def set_extra_equalities(self,
+                             extra_equalities: Union[list, None]) -> None:
+        """Set extra equality constraints for the SDP.
+
+        Parameters
+        ----------
+        extra_equalities : Union[list, None]
+            List of additional equality constraints in the form of dictionaries
+            (keys can be instances of `CompoundMonomial`, Symbols, strings, or
+            integers), or SymPy expressions.
+        """
+        self.extra_equalities = []  # reset every time
+        if not extra_equalities or extra_equalities is None:
+            return
+        self.extra_equalities = [self._sanitise_dict(eq)
+                                 for eq in extra_equalities]
+
+    def set_extra_inequalities(self,
+                               extra_inequalities: Union[list, None]) -> None:
+        """Set extra inequality constraints for the SDP.
+
+        Parameters
+        ----------
+        extra_inequalities : Union[list, None]
+            List of additional inequality constraints in the form of
+            dictionaries (keys can be instances of `CompoundMonomial`, Symbols,
+            strings, or integers) or SymPy expressions.
+        """
+        self.extra_inequalities = []  # reset every time
+        if not extra_inequalities or extra_inequalities is None:
+            return
+        self.extra_inequalities = [self._sanitise_dict(ineq)
+                                   for ineq in extra_inequalities]
+
+    @property
+    def moment_equalities(self) -> list[dict]:
+        """All equalities (minimal and extra) as one list of dictionaries."""
+        return self.minimal_equalities + self.extra_equalities
+
+    @property
+    def moment_inequalities(self) -> list[dict]:
+        """All inequalities (minimal and extra) as one list of dictionaries."""
+        return self.minimal_inequalities + self.extra_inequalities
+
     def set_bounds(self,
                    bounds: Union[dict, None],
                    bound_type: str = "up") -> None:
         r"""Set numerical lower or upper bounds on the moments generated in the
         SDP relaxation. The bounds are at the level of the SDP variables,
         and do not take into consideration non-convex constraints. E.g., two
         individual lower bounds, :math:`p_A(0|0) \geq 0.1` and
@@ -407,18 +466,74 @@
 
         Examples
         --------
         >>> set_bounds({"pAB(00|00)": 0.2}, "lo")
         """
         assert bound_type in ["up", "lo"], \
             "The 'bound_type' argument should be either 'up' or 'lo'"
+        if bounds is None:
+            return
+        # Sanitize list of bounds
+        sanitized_bounds = dict()
+        for mon, bound in bounds.items():
+            mon = self._sanitise_moment(mon)
+            if mon not in sanitized_bounds.keys():
+                sanitized_bounds[mon] = bound
+            else:
+                old_bound = sanitized_bounds[mon]
+                assert np.isclose(old_bound, bound), \
+                    (f"Contradiction: Cannot set the same monomial {mon} to " +
+                     "have different upper bounds.")
         if bound_type == "up":
-            self._set_upperbounds(bounds)
+            self._reset_upperbounds()
+            self.moment_upperbounds = sanitized_bounds
         else:
-            self._set_lowerbounds(bounds)
+            self._reset_lowerbounds()
+            self.moment_lowerbounds.update(sanitized_bounds)
+        self._update_bounds(bound_type)
+
+    @cached_property
+    def atomic_factors(self):
+        atoms = set()
+        for mon in self.moments:
+            atoms.update(mon.factors)
+        return sorted(atoms)
+
+    @cached_property
+    def atomic_monomials(self):
+        """Returns the atomic monomials."""
+        return [self._monomial_from_atoms([atom]) for atom in self.atomic_factors]
+
+    @cached_property
+    def atom_from_name(self):
+        """Returns the atomic monomials."""
+        lookup_dict = dict()
+        for atom in self.atomic_factors:
+            lookup_dict[atom.name] = atom
+            lookup_dict[atom.legacy_name] = atom
+        return lookup_dict
+
+    @cached_property
+    def atomic_monomials(self):
+        """Returns the atomic monomials."""
+        atoms = set()
+        for mon in self.moments:
+            atoms.update(mon.factors)
+        return [self._monomial_from_atoms([atom]) for atom in sorted(atoms)]
+
+    @cached_property
+    def knowable_atoms(self):
+        """Returns the knowable atoms."""
+        return [m for m in self.atomic_monomials if m.is_knowable]
+
+    @cached_property
+    def do_conditional_atoms(self):
+        """Returns the atomic monomials which correspond to do conditionals."""
+        return [m for m in self.atomic_monomials if
+                (m.is_do_conditional and not m.is_knowable)]
 
     def set_distribution(self,
                          prob_array: Union[np.ndarray, None],
                          use_lpi_constraints=False,
                          shared_randomness=False) -> None:
         r"""Set numerically all the knowable (and optionally semiknowable)
         moments according to the probability distribution specified.
@@ -463,15 +578,15 @@
         """Set or change the objective function of the polynomial optimization
         problem.
 
         Parameters
         ----------
         objective : Union[sp.core.expr.Expr, dict, None]
             The objective function, either as a combination of sympy symbols,
-            as a dictionary with keys the monomials or their names, and as
+            as a dictionary with keys the moments or their names, and as
             values the corresponding coefficients, or ``None`` for clearing
             a previous objective.
         direction : str, optional
             Direction of the optimization (``"max"``/``"min"``). By default
             ``"max"``.
         """
         assert (not self.supports_problem) or (objective is None), \
@@ -482,62 +597,50 @@
         self._reset_objective()
         if direction == "max":
             self.maximize = True
         else:
             self.maximize = False
         if objective is None:
             return
-        elif isinstance(objective, sp.core.expr.Expr):
-            if objective.free_symbols:
-                objective_raw = sp.expand(objective).as_coefficients_dict()
-                objective_raw = {k: float(v)
-                                 for k, v in objective_raw.items()}
-            else:
-                objective_raw = {self.One: float(objective)}
-            return self.set_objective(objective_raw, direction)
         else:
             if self.use_lpi_constraints and self.verbose > 0:
                 warn("You have the flag `use_lpi_constraints` set to True. Be "
                      + "aware that imposing linearized polynomial constraints "
                      + "will constrain the optimization to distributions with "
                      + "fixed marginals.")
             sign = (1 if self.maximize else -1)
-            objective_dict = {self.One: 0}
-            for mon, coeff in objective.items():
-                if not np.isclose(coeff, 0):
-                    mon = self._sanitise_monomial(mon)
-                    objective_dict[mon] = \
-                        objective_dict.get(mon, 0) + (sign * coeff)
-            self.objective = objective_dict
+            self.objective = {mon: (sign * coeff) for mon, coeff
+                              in self._sanitise_dict(objective).items()}
+            self.objective.setdefault(self.One, 0)
             surprising_objective_terms = {mon for mon in self.objective.keys()
-                                          if mon not in self.monomials}
+                                          if mon not in self.moments}
             assert len(surprising_objective_terms) == 0, \
                 ("When interpreting the objective we have encountered at " +
                  "least one monomial that does not appear in the original " +
                  f"moment matrix:\n\t{surprising_objective_terms}")
             self._update_objective()
 
-    def set_values(self,
-                   values: Union[Dict[Union[CompoundMonomial,
-                                            InternalAtomicMonomial,
+    def update_values(self,
+                   values: Union[Dict[Union[CompoundMomentSDP,
+                                            InternalAtomicMonomialSDP,
                                             sp.core.symbol.Symbol,
                                             str],
                                       Union[float, sp.core.expr.Expr]],
                                  None],
                    use_lpi_constraints: bool = False,
                    only_specified_values: bool = False) -> None:
         """Directly assign numerical values to variables in the moment matrix.
         This is done via a dictionary where keys are the variables to have
         numerical values assigned (either in their operator form, in string
         form, or directly referring to the variable in the moment matrix), and
         the values are the corresponding numerical quantities.
 
         Parameters
         ----------
-        values : Union[None, Dict[Union[CompoundMonomial, InternalAtomicMonomial, sympy.core.symbol.Symbol, str], float]]
+        values : Union[None, Dict[Union[CompoundMomentSDP, InternalAtomicMonomialSDP, sympy.core.symbol.Symbol, str], float]]
             The description of the variables to be assigned numerical values
             and the corresponding values. The keys can be either of the
             Monomial class, symbols or strings (which should be the name of
             some Monomial).
 
         use_lpi_constraints : bool
             Specification whether linearized polynomial constraints (see, e.g.,
@@ -545,96 +648,113 @@
 
         only_specified_values : bool
             Specifies whether one wishes to fix only the variables provided
             (``True``), or also the variables containing products of the
             monomials fixed (``False``). Regardless of this flag, unknowable
             variables can also be fixed.
         """
-        self._reset_values()
-
-        if (values is None) or (len(values) == 0):
-            self._cleanup_after_set_values()
+        if (values is None) or len(values) == 0:
             return
 
+        self._reset_solution()
+
         self.use_lpi_constraints = use_lpi_constraints
 
         if (len(self.objective) > 1) and self.use_lpi_constraints:
             warn("You have an objective function set. Be aware that imposing "
                  + "linearized polynomial constraints will constrain the "
                  + "optimization to distributions with fixed marginals.")
 
-        # It is funny to set values to monomials created from operators that do
+        # It is funny to set values to moments created from operators that do
         # not commute with each other, so we display a warning.
-        non_all_commuting_monomials = set()
-        for mon, value in values.items():
-            mon = self._sanitise_monomial(mon)
-            self.known_moments[mon] = value
-            if (self.verbose > 0) and (not mon.is_all_commuting):
-                non_all_commuting_monomials.add(mon)
-        if (len(non_all_commuting_monomials) >= 1) and (self.verbose > 0):
+        non_all_commuting_moments = set()
+        for moment, value in values.items():
+            try:  # We do this to deal with NaNs (such as in undefined supports)
+                  # in a way that is also compatible with symbolic values.
+                if np.isnan(value):
+                    continue
+            except TypeError:
+                pass
+            moment = self._sanitise_moment(moment)
+            self.known_moments[moment] = value
+            if (self.verbose > 0) and (not moment.is_all_commuting):
+                non_all_commuting_moments.add(moment)
+        if (len(non_all_commuting_moments) >= 1) and (self.verbose > 0):
             warn("When setting values, we encountered at least one monomial " +
                  "with noncommuting operators:\n\t" +
-                 str(non_all_commuting_monomials))
-        del non_all_commuting_monomials
+                 str(non_all_commuting_moments))
+        del non_all_commuting_moments
         if not only_specified_values:
-            atomic_knowns = {mon.knowable_factors[0]: val
+            atomic_knowns = {mon.factors[0]: val
                              for mon, val in self.known_moments.items()
                              if len(mon) == 1}
             atomic_knowns.update({atom.dagger: val
                                   for atom, val in atomic_knowns.items()})
-            monomials_not_present = set(self.known_moments.keys()
-                                        ).difference(self.monomials)
-            for mon in monomials_not_present:
-                del self.known_moments[mon]
+            moments_not_present = set(self.known_moments.keys()
+                                        ).difference(self.moments)
+            for moment in moments_not_present:
+                del self.known_moments[moment]
 
-            # Get the remaining monomials that need assignment
+            # Get the remaining moments that need assignment
             if all(atom.is_knowable for atom in atomic_knowns):
                 if not self.use_lpi_constraints:
-                    remaining_mons = (mon for mon in self.monomials
+                    remaining_mons = (mon for mon in self.moments
                                       if ((not mon.is_atomic)
                                           and mon.is_knowable))
                 else:
-                    remaining_mons = (mon for mon in self.monomials
+                    remaining_mons = (mon for mon in self.moments
                                       if ((not mon.is_atomic)
                                           and mon.knowability_status
                                           in ["Knowable", "Semi"]))
             else:
-                remaining_mons = (mon for mon in self.monomials
+                remaining_mons = (mon for mon in self.moments
                                   if not mon.is_atomic)
             surprising_semiknowns = set()
-            for mon in remaining_mons:
-                if mon not in self.known_moments.keys():
-                    value, unknown_factors, known_status = mon.evaluate(
-                        atomic_knowns,
-                        self.use_lpi_constraints)
-                    if known_status == "Known":
-                        self.known_moments[mon] = value
-                    elif known_status == "Semi":
-                        if self.use_lpi_constraints:
-                            unknown_mon = \
-                                self._monomial_from_atoms(unknown_factors)
-                            self.semiknown_moments[mon] = (value, unknown_mon)
-                            if self.verbose > 0:
-                                if unknown_mon not in self.monomials:
-                                    surprising_semiknowns.add(unknown_mon)
-                    else:
-                        pass
+            for moment in remaining_mons:
+                value, unknown_factors, known_status = moment.evaluate(
+                    atomic_knowns,
+                    self.use_lpi_constraints)
+                if known_status == "Known":
+                    self.known_moments[moment] = value
+                elif known_status == "Semi":
+                    if self.use_lpi_constraints:
+                        unknown_mon = \
+                            self._monomial_from_atoms(unknown_factors)
+                        self.semiknown_moments[moment] = (value, unknown_mon)
+                        if self.verbose > 0:
+                            if unknown_mon not in self.moments:
+                                surprising_semiknowns.add(unknown_mon)
+                else:
+                    pass
             if (len(surprising_semiknowns) >= 1) and (self.verbose > 0):
                 warn("When processing LPI constraints we encountered at " +
                      "least one monomial that does not appear in the " +
                      f"original moment matrix:\n\t{surprising_semiknowns}")
             del atomic_knowns, surprising_semiknowns
         self._cleanup_after_set_values()
 
+    def set_values(self, values, **kwargs):
+        r"""Exactly like update_values, except it resets all known values to zero
+        as an intermediate step
+        """
+        self._reset_values()
+        if (values is None) or len(values) == 0:
+            self._cleanup_after_set_values()
+            return
+        else:
+            self.update_values(values, **kwargs)
+            return
+
     def solve(self,
               interpreter="MOSEKFusion",
               feas_as_optim=False,
-              dualise=True,
+              solve_dual=True,
               solverparameters=None,
-              solver_arguments={}) -> None:
+              solver_arguments={},
+              verbose: int = -1) -> None:
         r"""Call a solver on the SDP relaxation. Upon successful solution, it
         returns the primal and dual objective values along with the solution
         matrices.
 
         Parameters
         ----------
         interpreter : str, optional
@@ -647,61 +767,76 @@
             setting this label to ``True`` solves instead the problem
 
                 :math:`(2) \text{ max }\lambda\text{ such that }
                 \Gamma - \lambda\cdot 1 \succeq 0.`
 
             The correspondence is that the result of (2) is positive if (1) is
             feasible, and negative otherwise. By default ``False``.
-        dualise : bool, optional
+        solve_dual : bool, optional
             Optimize the dual problem (recommended). By default ``True``.
         solverparameters : dict, optional
             Extra parameters to be sent to the solver. By default ``None``.
         solver_arguments : dict, optional
             By default, solve will use the dictionary of SDP keyword arguments
             given by ``_prepare_solver_arguments()``. However, a user may
             manually override these arguments by passing their own here.
+        verbose : int, optional
+            How much information to display to the user. By default, ``-1``
+            (which sets it to ``self.verbose``).
         """
         if not self._relaxation_has_been_generated:
             raise Exception("Relaxation is not generated yet. " +
                             "Call \"InflationSDP.get_relaxation()\" first")
         if feas_as_optim and len(self._processed_objective) > 1:
             warn("You have a non-trivial objective, but set to solve a " +
                  "feasibility problem as optimization. Setting "
                  + "feas_as_optim=False and optimizing the objective...")
             feas_as_optim = False
 
+        real_verbose = self.verbose if verbose == -1 else verbose
+
         args = self._prepare_solver_arguments()
         args.update(solver_arguments)
         args.update({"feas_as_optim": feas_as_optim,
-                     "verbose": self.verbose,
+                     "verbose": real_verbose,
                      "solverparameters": solverparameters,
-                     "solve_dual": dualise})
+                     "solve_dual": solve_dual})
 
         self.solution_object = solveSDP_MosekFUSION(**args)
 
         self.status = self.solution_object["status"]
         if self.status == "feasible":
+            self.success = True
             self.primal_objective = self.solution_object["primal_value"]
             self.objective_value  = self.solution_object["primal_value"]
             self.objective_value *= (1 if self.maximize else -1)
         else:
+            self.success = False
             self.primal_objective = self.status
             self.objective_value  = self.status
         collect()
 
     ###########################################################################
     # PUBLIC ROUTINES RELATED TO THE PROCESSING OF CERTIFICATES               #
     ###########################################################################
-    def certificate_as_probs(self,
-                             clean: bool = True,
-                             chop_tol: float = 1e-10,
-                             round_decimals: int = 3) -> sp.core.add.Add:
-        """Give certificate as symbolic sum of probabilities. The certificate
+    def certificate_as_dict(self,
+                            clean: bool = True,
+                            chop_tol: float = 1e-10,
+                            round_decimals: int = 3) -> dict:
+        """Give certificate as dictionary with monomials as keys and
+        their coefficients in the certificate as the values. The certificate
         of incompatibility is ``cert < 0``.
 
+        If the certificate is evaluated on a point giving a negative value, this
+        guarantees that the compatibility test for the same point is infeasible
+        provided the set of constraints of the program does not change. Warning:
+        when using ``use_lpi_constraints=True`` the set of constraints depends
+        on the specified distribution, thus the certificate is not guaranteed to
+        apply.
+
         Parameters
         ----------
         clean : bool, optional
             If ``True``, eliminate all coefficients that are smaller than
             ``chop_tol``, normalise and round to the number of decimals
             specified by ``round_decimals``. By default ``True``.
         chop_tol : float, optional
@@ -709,44 +844,66 @@
             set to zero. By default ``1e-10``.
         round_decimals : int, optional
             Coefficients that are not set to zero are rounded to the number of
             decimals specified. By default ``3``.
 
         Returns
         -------
-        sympy.core.add.Add
-            The expression of the certificate in terms or probabilities and
+        dict
+            The expression of the certificate in terms of probabilities and
             marginals. The certificate of incompatibility is ``cert < 0``.
         """
         try:
             dual = self.solution_object["dual_certificate"]
         except AttributeError:
             raise Exception("For extracting a certificate you need to solve " +
                             "a problem. Call \"InflationSDP.solve()\" first.")
         if len(self.semiknown_moments) > 0:
             warn("Beware that, because the problem contains linearized " +
                  "polynomial constraints, the certificate is not guaranteed " +
                  "to apply to other distributions.")
-        if clean and not np.allclose(list(dual.values()), 0.):
+        if np.allclose(list(dual.values()), 0.):
+            return dict()
+        if clean:
             dual = clean_coefficients(dual, chop_tol, round_decimals)
+        return {self.monomial_from_name[k]: v for k, v in dual.items()
+                if not self.monomial_from_name[k].is_zero}
+
+    def probs_from_dict(self,
+                        dict_with_monomial_keys: dict) -> sp.core.add.Add:
+        """Converts a monomial dictionary into a SymPy expression.
 
+        Parameters
+        ----------
+        dict_with_monomial_keys : Dict[sympy.Symbol, float]
+            Dictionary with monomials and associated coefficients.
+
+        Returns
+        -------
+        sympy.core.add.Add
+            The expression of the polynomial encoded in the dictionary.
+        """
         polynomial = sp.S.Zero
-        for mon_name, coeff in dual.items():
-            if clean and np.isclose(int(coeff), round(coeff, round_decimals)):
-                coeff = int(coeff)
-            polynomial += coeff * self.names_to_symbols[mon_name]
+        for mon, coeff in self._sanitise_dict(dict_with_monomial_keys).items():
+            polynomial += coeff * mon.symbol
         return polynomial
 
-    def certificate_as_string(self,
-                              clean: bool = True,
-                              chop_tol: float = 1e-10,
-                              round_decimals: int = 3) -> str:
-        """Give the certificate as a string with the notation of the operators
-        in the moment matrix. The expression is in the form such that
-        satisfaction implies incompatibility.
+    def certificate_as_probs(self,
+                             clean: bool = True,
+                             chop_tol: float = 1e-10,
+                             round_decimals: int = 3) -> sp.core.add.Add:
+        """Give certificate as symbolic sum of probabilities. The certificate
+        of incompatibility is ``cert < 0``.
+
+        If the certificate is evaluated on a point giving a negative value, this
+        guarantees that the compatibility test for the same point is infeasible
+        provided the set of constraints of the program does not change. Warning:
+        when using ``use_lpi_constraints=True`` the set of constraints depends
+        on the specified distribution, thus the certificate is not guaranteed to
+        apply.
 
         Parameters
         ----------
         clean : bool, optional
             If ``True``, eliminate all coefficients that are smaller than
             ``chop_tol``, normalise and round to the number of decimals
             specified by ``round_decimals``. By default ``True``.
@@ -755,62 +912,161 @@
             set to zero. By default ``1e-10``.
         round_decimals : int, optional
             Coefficients that are not set to zero are rounded to the number of
             decimals specified. By default ``3``.
 
         Returns
         -------
-        str
-            The certificate in terms of symbols representing the monomials in
-            the moment matrix. The certificate of incompatibility is
-            ``cert < 0``.
+        sympy.core.add.Add
+            The expression of the certificate in terms of probabilities and
+            marginals. The certificate of incompatibility is ``cert < 0``.
         """
-        try:
-            dual = self.solution_object["dual_certificate"]
-        except AttributeError:
-            raise Exception("For extracting a certificate you need to solve " +
-                            "a problem. Call \"InflationSDP.solve()\" first.")
-        if len(self.semiknown_moments) > 0:
-            if self.verbose > 0:
-                warn("Beware that, because the problem contains linearized " +
-                     "polynomial constraints, the certificate is not " +
-                     "guaranteed to apply to other distributions.")
+        return self.probs_from_dict(self.certificate_as_dict(
+            clean=clean,
+            chop_tol=chop_tol,
+            round_decimals=round_decimals))
 
-        if clean and not np.allclose(list(dual.values()), 0.):
-            dual = clean_coefficients(dual, chop_tol, round_decimals)
+    def string_from_dict(self,
+                         dict_with_monomial_keys: dict) -> str:
+        """Converts a monomial dictionary into a string.
 
-        rest_of_dual = dual.copy()
-        constant_value = rest_of_dual.pop(self.constant_term_name, 0)
-        constant_value += rest_of_dual.pop(self.One.name, 0)
+        Parameters
+        ----------
+        dict_with_monomial_keys : Dict[sympy.Symbol, float]
+            Dictionary with monomials and associated coefficients.
+
+        Returns
+        -------
+        str
+            The expression of the certificate in string form.
+        """
+        as_dict = self._sanitise_dict(dict_with_monomial_keys)
+        # Watch out for when "1" is note the same as "constant_term"
+        constant_value = as_dict.pop(self.Constant_Term,
+                                     as_dict.pop(self.One, 0.)
+                                     )
         if constant_value:
-            if clean:
-                cert = "{0:.{prec}f}".format(constant_value,
-                                             prec=round_decimals)
-            else:
-                cert = str(constant_value)
+            polynomial_as_str = str(constant_value)
         else:
-            cert = ""
-        for mon_name, coeff in rest_of_dual.items():
-            if mon_name != "0":
-                cert += "+" if coeff >= 0 else "-"
+            polynomial_as_str = ""
+        for mon, coeff in as_dict.items():
+            if mon.is_zero or np.isclose(np.abs(coeff), 0):
+                continue
+            else:
+                polynomial_as_str += "+" if coeff >= 0 else "-"
                 if np.isclose(abs(coeff), 1):
-                    cert += mon_name
+                    polynomial_as_str += mon.name
                 else:
-                    if clean:
-                        cert += "{0:.{prec}f}*{1}".format(abs(coeff),
-                                                          mon_name,
-                                                          prec=round_decimals)
-                    else:
-                        cert += f"{abs(coeff)}*{mon_name}"
-        cert += " < 0"
-        return cert[1:] if cert[0] == "+" else cert
+                    polynomial_as_str += "{0}*{1}".format(abs(coeff), mon.name)
+        return polynomial_as_str[1:] if polynomial_as_str[
+                                            0] == "+" else polynomial_as_str
+
+    def certificate_as_string(self,
+                              clean: bool = True,
+                              chop_tol: float = 1e-10,
+                              round_decimals: int = 3) -> str:
+        """Give the certificate as a string of a sum of probabilities. The
+        expression is in the form such that its satisfaction implies
+        incompatibility.
+
+        If the certificate is evaluated on a point giving a negative value, this
+        guarantees that the compatibility test for the same point is infeasible
+        provided the set of constraints of the program does not change. Warning:
+        when using ``use_lpi_constraints=True`` the set of constraints depends
+        on the specified distribution, thus the certificate is not guaranteed to
+        apply.
+
+        Parameters
+        ----------
+        clean : bool, optional
+            If ``True``, eliminate all coefficients that are smaller than
+            ``chop_tol``, normalise and round to the number of decimals
+            specified by ``round_decimals``. By default, ``True``.
+        chop_tol : float, optional
+            Coefficients in the dual certificate smaller in absolute value are
+            set to zero. By default, ``1e-10``.
+        round_decimals : int, optional
+            Coefficients that are not set to zero are rounded to the number of
+            decimals specified. By default, ``3``.
+
+        Returns
+        -------
+        str
+            The certificate in terms of probabilities and marginals. The
+            certificate of incompatibility is ``cert < 0``.
+        """
+        return self.string_from_dict(
+            self.certificate_as_dict(
+                clean=clean,
+                chop_tol=chop_tol,
+                round_decimals=round_decimals)) + " < 0"
+
+    def evaluate_polynomial(self, polynomial: dict, prob_array: np.ndarray):
+        """Evaluate the certificate of infeasibility in a target probability
+        distribution. If the evaluation is a negative value, the distribution is
+        not compatible with the causal structure. Warning: when using
+        ``use_lpi_constraints=True`` the set of constraints depends on the
+        specified distribution, thus the certificate is not guaranteed to apply.
+
+        Parameters
+        ----------
+        polynomial : dict
+            A dictionary of monomials with coefficients as values.
+        prob_array : numpy.ndarray
+            Multidimensional array encoding the distribution, which is
+            called as ``prob_array[a,b,c,...,x,y,z,...]`` where
+            :math:`a,b,c,\dots` are outputs and :math:`x,y,z,\dots` are
+            inputs. Note: even if the inputs have cardinality 1 they must
+            be specified, and the corresponding axis dimensions are 1.
+            The parties' outcomes and measurements must appear in the
+            same order as specified by the ``order`` parameter in the
+            ``InflationProblem`` used to instantiate ``InflationLP``.
+
+        Returns
+        -------
+        float
+            The evaluation of the certificate of infeasibility in prob_array.
+        """
+        return sum((atom.compute_marginal(prob_array) * val
+                    for atom, val in self._sanitise_dict(polynomial).items()))
+
+    def evaluate_certificate(self, prob_array: np.ndarray) -> float:
+        """Evaluate the certificate of infeasibility in a target probability
+        distribution. If the evaluation is a negative value, the distribution is
+        not compatible with the causal structure. Warning: when using
+        ``use_lpi_constraints=True`` the set of constraints depends on the
+        specified distribution, thus the certificate is not guaranteed to apply.
+
+        Parameters
+        ----------
+        prob_array : numpy.ndarray
+            Multidimensional array encoding the distribution, which is
+            called as ``prob_array[a,b,c,...,x,y,z,...]`` where
+            :math:`a,b,c,\dots` are outputs and :math:`x,y,z,\dots` are
+            inputs. Note: even if the inputs have cardinality 1 they must
+            be specified, and the corresponding axis dimensions are 1.
+            The parties' outcomes and measurements must appear in the
+            same order as specified by the ``order`` parameter in the
+            ``InflationProblem`` used to instantiate ``InflationLP``.
+
+        Returns
+        -------
+        float
+            The evaluation of the certificate of infeasibility in prob_array.
+        """
+        if self.use_lpi_constraints:
+            warn("You have used LPI constraints to obtain the certificate. " +
+                 "Be aware that, because of that, the certificate may not be " +
+                 "valid for other distributions.")
+        return self.evaluate_polynomial(self.certificate_as_dict(), prob_array)
 
     ###########################################################################
     # OTHER ROUTINES EXPOSED TO THE USER                                      #
     ###########################################################################
+    #TODO: Natively avoid intermediate 2d-representation in build_columns
     def build_columns(self,
                       column_specification: Union[str,
                                                   List[List[int]],
                                                   List[sp.core.symbol.Symbol]],
                       max_monomial_length: int = 0,
                       symbolic: bool = False) -> List[np.ndarray]:
         r"""Creates the objects indexing the columns of the moment matrix from
@@ -830,42 +1086,51 @@
         symbolic: bool, optional
             If ``True``, it returns the columns as a list of sympy symbols
             parsable by `InflationSDP.generate_relaxation()`. By default
             ``False``.
         """
         columns = None
         if type(column_specification) == list:
-            # There are two possibilities: list of lists, or list of symbols
-            if type(column_specification[0]) in {list, np.ndarray}:
+            # There are three possibilities: list of lists, list of arrays 
+            # or list of symbols. If list of lists, then it is the party
+            # block encoding. If it is a list of arrays, then it can be either
+            # monomials in the 2d encoding, or the 1d encoding.
+            if type(column_specification[0]) == list:
+                # This is the standard specification for the helper
+                columns = self._build_cols_from_specs(column_specification)
+            elif type(column_specification[0]) in {np.ndarray}:
                 if len(np.array(column_specification[1]).shape) == 2:
-                    # This is the format that is later parsed by the program
-                    columns = [np.array(mon, dtype=self.np_dtype)
+                    # This is the 2d encoding, convert it to lexicographic repr
+                    columns = [self.mon_to_lexrepr(mon)
                                for mon in column_specification]
                 elif len(np.array(column_specification[1]).shape) == 1:
-                    # This is the standard specification for the helper
-                    columns = self._build_cols_from_specs(column_specification)
+                    # This is the 1d encoding, make sure the dtype is correct
+                    # for compatibility with numba
+                    columns = [np.array(mon, dtype=np.intc)
+                               for mon in column_specification]
                 else:
                     raise Exception("The generating columns are not specified "
                                     + "in a valid format.")
             elif type(column_specification[0]) in [int, sp.core.symbol.Symbol,
                                                    sp.core.power.Pow,
                                                    sp.core.mul.Mul,
                                                    sp.core.numbers.One]:
                 columns = []
                 for col in column_specification:
                     if type(col) in [int, sp.core.numbers.One]:
                         if not np.isclose(float(col), 1):
                             raise Exception(f"Column {col} is just a number. "
                                             + "Please use a valid format.")
                         else:
-                            columns.append(self.identity_operator)
+                            columns.append(np.array([], dtype=np.intc))
                     elif type(col) in [sp.core.symbol.Symbol,
                                        sp.core.power.Pow,
                                        sp.core.mul.Mul]:
-                        columns.append(self._interpret_name(col))
+                        columns.append(self.mon_to_lexrepr(
+                            self._interpret_name(col)))
                     else:
                         raise Exception(f"The column {col} is not specified " +
                                         "in a valid format.")
             else:
                 raise Exception("The generating columns are not specified " +
                                 "in a valid format.")
         elif type(column_specification) == str:
@@ -893,102 +1158,101 @@
                                 else 8)
                 spec    = column_specification[:lengths_init]
                 lengths = column_specification[lengths_init:]
                 if len(lengths) == 0:
                     if spec == "local":
                         raise Exception("Please specify a precise local level")
                     else:
-                        lengths = [min(self.inflation_levels[party])
-                                   for party in self.hypergraph.T]
+                        lengths = [None] * self.nr_parties
                 elif len(lengths) == self.nr_parties:
                     lengths = [int(level) for level in lengths]
                 else:
                     lengths = [int(lengths)] * self.nr_parties
-                max_length = sum(lengths)
-                # Determine maximum length
-                if ((max_monomial_length > 0)
-                        and (max_monomial_length < max_length)):
-                    max_length = max_monomial_length
 
-                party_freqs = sorted((list(pfreq)
-                                      for pfreq in product(
-                                       *[range(level + 1) for level in lengths]
-                                                           )
-                                      if sum(pfreq) <= max_length),
-                                     key=lambda x: (sum(x), [-p for p in x]))
                 if spec == "local":
+                    max_length = sum(lengths)
+                    # Determine maximum length
+                    if ((max_monomial_length > 0)
+                            and (max_monomial_length < max_length)):
+                        max_length = max_monomial_length
+
+                    party_freqs = sorted((list(pfreq)
+                                        for pfreq in product(
+                                        *[range(level + 1) for level in lengths]
+                                                            )
+                                        if sum(pfreq) <= max_length),
+                                        key=lambda x: (sum(x), [-p for p in x]))
                     col_specs = []
                     for pfreq in party_freqs:
                         operators = []
                         for party in range(self.nr_parties):
                             operators += [party] * pfreq[party]
                         col_specs += [operators]
                     columns = self._build_cols_from_specs(col_specs)
                 else:
-                    physical_monomials = []
-                    for freqs in party_freqs:
-                        if freqs == [0] * self.nr_parties:
-                            physical_monomials.append(self.identity_operator)
-                        else:
-                            physmons_per_party = []
-                            for party, freq in enumerate(freqs):
-                                if freq > 0:
-                                    physmons = party_physical_monomials(
-                                        self.hypergraph,
-                                        self.inflation_levels,
-                                        party, freq,
-                                        self.setting_cardinalities,
-                                        self.outcome_cardinalities,
-                                        self._lexorder)
-                                    physmons_per_party.append(physmons)
-                            for monomial_parts in product(
-                                    *physmons_per_party):
-                                physical_monomials.append(
-                                    self._to_canonical_memoized(
-                                        np.concatenate(monomial_parts)))
-                    columns = physical_monomials
+                    physmon_per_party \
+                        = [self.InflationProblem._generate_compatible_monomials_given_party(
+                            party, 
+                            up_to_length=length,
+                            with_last_outcome=self.has_children[party]
+                            )
+                            for length, party in zip(lengths,
+                                                     range(self.nr_parties))
+                            ]
+                    physical_monomials_as_boolvecs = \
+                        reduce(nb_outer_bitwise_or, reversed(physmon_per_party))
+                    columns = sorted(
+                        (np.flatnonzero(boolvec).astype(np.intc) + 1 
+                        for boolvec in physical_monomials_as_boolvecs
+                        if max_monomial_length == 0 or \
+                            (boolvec.sum() <= max_monomial_length)),
+                                    key=lambda x: (len(x), tuple(x)))
             else:
                 raise Exception("I have not understood the format of the "
                                 + "column specification")
         else:
             raise Exception("I have not understood the format of the "
                             + "column specification")
-
-        if not np.array_equal(self._lexorder, self._default_lexorder):
-            res_lexrepr = [nb_mon_to_lexrepr(mon, self._lexorder).tolist()
-                           if (len(mon) or mon.shape[-1] == 1) else []
-                           for mon in columns]
-            sorted_mons = sorted(res_lexrepr, key=lambda x: (len(x), x))
-            columns = [self._lexorder[lexrepr]
-                       if lexrepr != [] else self.identity_operator
-                       for lexrepr in sorted_mons]
-
-        columns = [np.array(col,
-                            dtype=self.np_dtype).reshape((-1,
-                                                          self._nr_properties))
-                   for col in columns]
+        
+        self.generating_monomials_1d = columns
+        self.genmon_1d_to_index = {tuple(lexmon): i for i, lexmon in
+                                   enumerate(self.generating_monomials_1d)}
+        if len(self.genmon_1d_to_index) != len(self.generating_monomials_1d):
+            self.generating_monomials_1d = \
+                sorted(self.generating_monomials_1d, 
+                       key=lambda x: (len(x), tuple(x)))
+            self.genmon_1d_to_index = \
+                {tuple(lexmon): i 
+                 for i, lexmon in enumerate(self.generating_monomials_1d)}
+            warn("The generating set of monomials included duplicate elements.")
+        self.n_columns = len(self.generating_monomials_1d)
+        output = self.generating_monomials_1d
         if symbolic:
-            columns = [to_symbol(col, self.names) for col in columns]
-        return columns
+            output = [reduce(sp.Mul,
+                             self._lexrepr_to_symbols[lexmon],
+                             sp.S.One)
+                      for lexmon in self.generating_monomials_1d ]
+        return output
 
-    def reset(self, which: Union[str, List[str]]) -> None:
+    def reset(self, which: Union[str, List[str]] = "all") -> None:
         """Reset the various user-specifiable objects in the inflation SDP.
 
         Parameters
         ----------
         which : Union[str, List[str]]
             The objects to be reset. It can be fed as a single string or a list
             of them. Options include ``"bounds"``, ``"lowerbounds"``,
             ``"upperbounds"``, ``"objective"``, ``"values"``, and ``"all"``.
         """
         if type(which) == str:
             if which == "all":
-                self.reset(["bounds", "objective", "values"])
+                self.reset(["values", "bounds", "objective"])
             elif which == "bounds":
-                self._reset_bounds()
+                self._reset_lowerbounds()
+                self._reset_upperbounds()
             elif which == "lowerbounds":
                 self._reset_lowerbounds()
             elif which == "upperbounds":
                 self._reset_upperbounds()
             elif which == "objective":
                 self._reset_objective()
             elif which == "values":
@@ -1032,67 +1296,67 @@
             raise Exception("File format not supported. Please choose between "
                             + "the extensions `.csv`, `.dat-s` and `.mat`.")
 
     ###########################################################################
     # ROUTINES RELATED TO CONSTRUCTING COMPOUND MONOMIAL INSTANCES            #
     ###########################################################################
     def _AtomicMonomial(self,
-                        array2d: np.ndarray) -> InternalAtomicMonomial:
-        """Construct an instance of the `InternalAtomicMonomial` class from
-        a 2D array description of a monomial.
+                        lexmon: np.ndarray) -> InternalAtomicMonomialSDP:
+        """Construct an instance of the `InternalAtomicMonomialSDP` class from
+        a 1D array description of a monomial.
 
         See the documentation of the `InternalAtomicMonomial` class for more
         details.
 
         Parameters
         ----------
-        array2d : numpy.ndarray
-            Monomial encoded as a 2D array of integers, where each row encodes
-            one of the operators appearing in the monomial.
+        lexmon : numpy.ndarray
+            Monomial encoded as a 1D array of integers, where integer
+            represents the slots in the lexorder.
 
         Returns
         -------
-        InternalAtomicMonomial
+        InternalAtomicMonomialSDP
             An instance of the `InternalAtomicMonomial` class representing the
             input 2D array monomial.
         """
-        key = self._from_2dndarray(array2d)
+        key = tuple(lexmon)
         try:
             return self.atomic_monomial_from_hash[key]
         except KeyError:
-            repr_array2d = self._to_inflation_repr(array2d)
-            new_key      = self._from_2dndarray(repr_array2d)
+            repr_lexmon = self._to_inflation_repr_1d(lexmon)
+            new_key      = tuple(repr_lexmon)
             try:
                 mon = self.atomic_monomial_from_hash[new_key]
                 self.atomic_monomial_from_hash[key] = mon
                 return mon
             except KeyError:
-                mon = InternalAtomicMonomial(self, repr_array2d)
+                mon = InternalAtomicMonomialSDP(self, repr_lexmon)
                 self.atomic_monomial_from_hash[key]     = mon
                 self.atomic_monomial_from_hash[new_key] = mon
                 return mon
 
-    def Monomial(self, array2d: np.ndarray, idx=-1) -> CompoundMonomial:
-        r"""Create an instance of the `CompoundMonomial` class from a 2D array.
-        An instance of `CompoundMonomial` is a collection of
-        `InternalAtomicMonomial`.
+    def Moment_2d(self, array2d: np.ndarray, idx=-1) -> CompoundMomentSDP:
+        r"""Create an instance of the `CompoundMomentSDP` class from a 2D array.
+        An instance of `CompoundMomentSDP` is a collection of
+        `InternalAtomicMonomialSDP` instances.
 
         Parameters
         ----------
         array2d : numpy.ndarray
             Moment encoded as a 2D array of integers, where each row encodes
             one of the operators appearing in the moment.
         idx : int, optional
-            Assigns an integer index to the resulting monomial, which can be
+            Assigns an integer index to the resulting moment, which can be
             used as an id, by default -1.
 
         Returns
         -------
-        CompoundMonomial
-            The monomial factorised into AtomicMonomials, all brought to
+        CompoundMomentSDP
+            The moment factorised into AtomicMonomials, all brought to
             representative form under inflation symmetries.
 
         Examples
         --------
 
         The moment
         :math:`\langle A^{0,2,1}_{x=2,a=3}C^{2,0,1}_{z=1,c=1}
@@ -1104,115 +1368,109 @@
 
         The resulting monomial, ``InflationSDP.Monomial(m)``, is a collection
         of two ``InternalAtomicMonomial`` s,
         :math:`\langle A^{0,1,1}_{x=2,a=3}C^{1,0,1}_{z=1,c=1}\rangle` and
         :math:`\langle C^{1,0,1}_{z=0,c=0}\rangle`, after factorizing the input
         monomial and reducing the inflation indices of each of the factors.
         """
-        _factors = self.factorize_monomial(array2d, canonical_order=False)
-        list_of_atoms = [self._AtomicMonomial(factor)
+        return self.Moment_1d(self.mon_to_lexrepr(array2d), idx=idx)
+
+    def Moment_1d(self, lexmon: np.ndarray, idx=-1) -> CompoundMomentSDP:
+        r"""Create an instance of the `CompoundMomentSDP` class from a 1D array.
+        An instance of `CompoundMomentSDP` is a collection of
+        `InternalAtomicMonomialSDP` instances.
+
+        Parameters
+        ----------
+        lexmon : numpy.ndarray
+            Moment encoded as a 1D array of integers, indicating positions in
+            the _lexorder.
+        idx : int, optional
+            Assigns an integer index to the resulting moment, which can be
+            used as an id, by default -1.
+
+        Returns
+        -------
+        CompoundMomentSDP
+            The moment factorised into AtomicMonomials, all brought to
+            representative form under inflation symmetries.
+        """
+        # HACK: The lexorder of InflationProblem is different from that 
+        # in InflationSDP!
+        _factors = self.factorize_moment_1d(np.asarray(lexmon, dtype=np.intc)-1,
+                                            canonical_order=False)
+        list_of_atoms = [self._AtomicMonomial(factor + 1)
                          for factor in _factors if len(factor)]
         mon = self._monomial_from_atoms(list_of_atoms)
         mon.attach_idx(idx)
         return mon
 
-    def _conjugate_ndarray(self,
-                           mon: np.ndarray,
+    def _conjugate_lexmon(self,
+                           lexmon: np.ndarray,
                            apply_only_commutations=True) -> np.ndarray:
         """Compute the canonical form of the conjugate of a monomial.
 
         Parameters
         ----------
         mon : numpy.ndarray
-            Input monomial that cannot be further factorised.
+            Input monomial that cannot be further factorised in 1d format
         apply_only_commutations : bool, optional
             If ``True``, skip checking if monomial is zero and if there are
             square projectors.
 
         Returns
         -------
         numpy.ndarray
             The canonical form of the conjugate of the input monomial under
             relabelling through the inflation symmetries.
         """
-        if self.all_commuting_q(mon):
-            return mon
+        if self.all_commuting_q_1d(lexmon):
+            return lexmon
         else:
-            return self._to_inflation_repr(reverse_mon(mon),
-                                           apply_only_commutations)
+            return self._to_inflation_repr_1d(reverse_mon(lexmon),
+                                              apply_only_commutations)
 
     def _construct_mask_matrices(self) -> None:
         """Helper a function to associate each monomial appearing in the moment
         matrix with a unique mask matrix, as this is relevant to expressing an
         SDP in dual form.
         """
         if self._relaxation_has_been_generated:
             if self.n_columns > 0:
                 self.maskmatrices = {
                     mon: lil_matrix(self.momentmatrix == mon.idx)
-                    for mon in tqdm(self.monomials,
+                    for mon in tqdm(self.moments,
                                     disable=not self.verbose,
                                     desc="Assigning mask matrices  ")
                                      }
 
-    def _inflation_orbit_and_rep(self,
-                                 monomial: np.ndarray
-                                 ) -> Tuple[set, np.ndarray]:
-        """Given a monomial as a 2D array, return its representative under
-        inflation symmetries and its orbit. Only source swaps up to the maximum
-        index of the source that appears in the monomials are considered.
-
-        Parameters
-        ----------
-        monomial : numpy.ndarray
-            Monomial as a 2D array.
-
-        Returns
-        -------
-        Tuple[set, numpy.ndarray]
-            The orbit as a set of all monomials explored, and the
-            representative (i.e, the minimum over said set).
-        """
-        inf_levels = monomial[:, 1:-2].max(axis=0)
-        nr_sources = inf_levels.shape[0]
-        all_permutations_per_source = [
-            format_permutations(list(permutations(range(inflevel))))
-            for inflevel in inf_levels.flat]
-        seen_hashes = set()
-        for permutation in product(*all_permutations_per_source):
-            permuted = monomial.copy()
-            for source in range(nr_sources):
-                permuted = apply_source_perm(permuted,
-                                             source,
-                                             permutation[source])
-            permuted = self._to_canonical_memoized(permuted, True)
-            hash     = self._from_2dndarray(permuted)
-            seen_hashes.add(hash)
-            try:
-                representative = self.canonsym_ndarray_from_hash[hash]
-                return seen_hashes, representative
-            except KeyError:
-                pass
-        representative = self._to_2dndarray(min(seen_hashes))
-        return seen_hashes, representative
+    def _inflation_orbit_and_rep_1d(self, lexmon: np.ndarray):
+        permuted_variants = np.take(self.lexorder_symmetries, lexmon, axis=1)
+        permuted_variants = np.unique(permuted_variants, axis=0).astype(int)
+        output_variants = \
+            [tuple(self._to_canonical_memoized_1d(
+                lexmon_variant, apply_only_commutations=True))
+                           for lexmon_variant in permuted_variants]
+        representative = np.array(min(output_variants), dtype=np.intc)
+        return output_variants, representative
 
     def _monomial_from_atoms(self,
-                             atoms: List[InternalAtomicMonomial]
-                             ) -> CompoundMonomial:
+                             atoms: List[InternalAtomicMonomialSDP]
+                             ) -> CompoundMomentSDP:
         """Build an instance of `CompoundMonomial` from a list of instances
         of `InternalAtomicMonomial`.
 
         Parameters
         ----------
-        atoms : List[InternalAtomicMonomial]
+        atoms : List[InternalAtomicMonomialSDP]
             List of instances of `InternalAtomicMonomial`.
 
         Returns
         -------
-        CompoundMonomial
+        CompoundMomentSDP
             A `CompoundMonomial` with atomic factors given by `atoms`.
         """
         list_of_atoms = []
         for factor in atoms:
             if factor.is_zero:
                 list_of_atoms = [factor]
                 break
@@ -1224,162 +1482,143 @@
         conjugate = tuple(sorted(factor.dagger for factor in atoms))
         atoms = min(atoms, conjugate)
         del conjugate
         try:
             mon = self.monomial_from_atoms[atoms]
             return mon
         except KeyError:
-            mon = CompoundMonomial(atoms)
+            mon = CompoundMomentSDP(atoms)
             try:
                 mon.idx = self.first_free_idx
                 self.first_free_idx += 1
             except AttributeError:
                 pass
             self.monomial_from_atoms[atoms]   = mon
             self.monomial_from_name[mon.name] = mon
+            self.monomial_from_name[mon.legacy_name] = mon  # For legacy compatibility!
+            self.monomial_from_symbol[mon.symbol] = mon
             return mon
 
-    def _sanitise_monomial(self, mon: Any) -> CompoundMonomial:
+    def _sanitise_moment(self, moment: Any) -> CompoundMomentSDP:
         """Return a ``CompoundMonomial`` built from ``mon``, where ``mon`` can
         be either the name of a moment as a string, a SymPy variable, a
         monomial encoded as a 2D array, or an integer in case the moment is the
         unit moment or the zero moment.
 
 
         Parameters
         ----------
-        mon : Any
+        moment : Any
             The name of a moment as a string, a SymPy variable with the name of
             a valid moment, a 2D array encoding of a moment or an integer in
             case the moment is the unit moment or the zero moment.
 
         Returns
         -------
-        CompoundMonomial
+        CompoundMomentSDP
             Instance of ``CompoundMonomial`` built from ``mon``.
 
         Raises
         ------
         Exception
             If ``mon`` is the constant monomial, it can only be numbers 0 or 1
         Exception
             If the type of ``mon`` is not supported.
         """
-        if isinstance(mon, CompoundMonomial):
-            return mon
-        elif isinstance(mon, (sp.core.symbol.Symbol,
-                              sp.core.power.Pow,
-                              sp.core.mul.Mul)):
-            symbols = flatten_symbolic_powers(mon)
-            if len(symbols) == 1:
-                try:
-                    return self.monomial_from_name[str(symbols[0])]
-                except KeyError:
-                    pass
-            array = np.concatenate([self._interpret_atomic_string(str(op))
-                                    for op in symbols])
-            return self._sanitise_monomial(array)
-        elif isinstance(mon, (tuple, list, np.ndarray)):
-            array = np.asarray(mon, dtype=self.np_dtype)
+        if isinstance(moment, CompoundMomentSDP):
+            return moment
+        elif isinstance(moment, InternalAtomicMonomialSDP):
+            return self._monomial_from_atoms([moment])
+        elif isinstance(moment, (tuple, list, np.ndarray)):
+            array = np.asarray(moment, dtype=self.np_dtype)
             assert array.ndim == 2, \
                 "The monomial representations must be 2d arrays."
             assert array.shape[-1] == self._nr_properties, \
                 "The input does not conform to the operator specification."
-            canon = self._to_canonical_memoized(array)
-            return self.Monomial(canon)
-        elif isinstance(mon, str):
-            try:
-                return self.monomial_from_name[mon]
-            except KeyError:
-                return self._sanitise_monomial(self._interpret_name(mon))
-        elif isinstance(mon, Real):
-            if np.isclose(float(mon), 1):
+            canon_lexmon = self._to_canonical_memoized_1d(
+                self.mon_to_lexrepr(array))
+            return self.Moment_1d(canon_lexmon)
+        elif isinstance(moment, (str, sp.core.symbol.Expr)):
+            return self._sanitise_moment(self._interpret_name(moment))
+        elif isinstance(moment, Real):
+            if np.isclose(float(moment), 1):
                 return self.One
-            elif np.isclose(float(mon), 0):
+            elif np.isclose(float(moment), 0):
                 return self.Zero
             else:
-                raise Exception(f"Constant monomial {mon} can only be 0 or 1.")
+                raise Exception(f"Constant monomial {moment} can only be 0 or 1.")
         else:
-            raise Exception(f"sanitise_monomial: {mon} is of type " +
-                            f"{type(mon)} and is not supported.")
+            raise Exception(f"sanitise_monomial: {moment} is of type " +
+                            f"{type(moment)} and is not supported.")
 
-    def _to_inflation_repr(self,
-                           mon: np.ndarray,
-                           apply_only_commutations=False) -> np.ndarray:
+    def _sanitise_dict(self, input_dict: Any) -> Dict:
+        if isinstance(input_dict, sp.core.expr.Expr):
+            if input_dict.free_symbols:
+                input_dict_copy = {k: float(v) for k, v in sp.expand(
+                    input_dict).as_coefficients_dict().items()}
+            else:
+                input_dict_copy = dict()
+        else:
+            input_dict_copy = input_dict
+        output_dict = defaultdict(int)
+        for k, v in input_dict_copy.items():
+            if not np.isclose(v, 0):
+                output_dict[self._sanitise_moment(k)] += v
+        return output_dict
+
+    def _to_inflation_repr_1d(self,
+                              lexmon: np.ndarray,
+                              apply_only_commutations=False) -> np.ndarray:
         r"""Apply inflation symmetries to a monomial in order to bring it to
         its canonical form.
 
-        Example: Assume the monomial is :math:`\langle D^{350}_{00}D^{450}_{00}
-        D^{150}_{00}E^{401}_{00}F^{031}_{00}\rangle`. In array form, the
-        information about inflation copies is:
-
-        ::
-
-            [[3 5 0],
-             [4 5 0],
-             [1 5 0],
-             [4 0 1],
-             [0 3 1]]
-
-        For each column the function assigns to the first row index 1. Then,
-        the next different one will be 2, and so on. Therefore, the
-        representative of the monomial above is :math:`\langle D^{110}_{00}
-        D^{210}_{00} D^{310}_{00} E^{201}_{00} F^{021}_{00} \rangle`.
-
         Parameters
         ----------
-        mon : numpy.ndarray
+        lexmon : numpy.ndarray
             Input monomial that cannot be further factorised.
         apply_only_commutations : bool, optional
             If ``True``, skip checking if monomial is zero and if there are
             multiple same projectors that square to just one of them.
 
         Returns
         -------
         numpy.ndarray
             The canonical form of the input monomial under relabelling through
             the inflation symmetries.
         """
-        key = self._from_2dndarray(mon)
-        if len(mon) == 0 or np.array_equiv(mon, 0):
-            self.canonsym_ndarray_from_hash[key] = mon
-            return mon
+        key = tuple(lexmon)
+        if len(lexmon) == 0 or np.array_equiv(lexmon, 0):
+            self.canonsym_lexmon_from_hash[key] = lexmon
+            return lexmon
         else:
             pass
         try:
-            return self.canonsym_ndarray_from_hash[key]
+            return self.canonsym_lexmon_from_hash[key]
         except KeyError:
             pass
-        canonical_mon = self._to_canonical_memoized(mon,
-                                                    apply_only_commutations)
-        canonical_key = self._from_2dndarray(canonical_mon)
+        canonical_mon = self._to_canonical_memoized_1d(lexmon,
+                                                       apply_only_commutations)
+        canonical_key = tuple(canonical_mon)
         try:
-            repr_mon = self.canonsym_ndarray_from_hash[canonical_key]
-            self.canonsym_ndarray_from_hash[key] = repr_mon
+            repr_mon = self.canonsym_lexmon_from_hash[canonical_key]
+            self.canonsym_lexmon_from_hash[key] = repr_mon
             return repr_mon
         except KeyError:
             pass
-        repr_mon = reduce_inflation_indices(mon)
-        repr_key = self._from_2dndarray(repr_mon)
-        try:
-            real_repr_mon = self.canonsym_ndarray_from_hash[repr_key]
-            self.canonsym_ndarray_from_hash[key]           = real_repr_mon
-            self.canonsym_ndarray_from_hash[canonical_key] = real_repr_mon
-            return real_repr_mon
-        except KeyError:
-            pass
-        other_keys, real_repr_mon = self._inflation_orbit_and_rep(repr_mon)
-        other_keys.update({key, canonical_key, repr_key})
+
+        other_keys, real_repr_lexmon = self._inflation_orbit_and_rep_1d(lexmon)
+        other_keys.append(key)
         for key in other_keys:
-            self.canonsym_ndarray_from_hash[key] = real_repr_mon
-        return real_repr_mon
+            self.canonsym_lexmon_from_hash[key] = real_repr_lexmon
+        return real_repr_lexmon
 
     ###########################################################################
     # ROUTINES RELATED TO NAME PARSING                                        #
     ###########################################################################
+    
     def _interpret_name(self,
                         monomial: Union[str, sp.core.symbol.Expr, int]
                         ) -> np.ndarray:
         """Build a 2D array encoding of a monomial which can be passed either
         as a string, as a SymPy expression or as an integer.
 
         Parameters
@@ -1388,24 +1627,31 @@
             Input moment.
 
         Returns
         -------
         numpy.ndarray
             2D array encoding of the input moment.
         """
-        if isinstance(monomial, sp.core.symbol.Expr):
-            factors = [str(factor)
-                       for factor in flatten_symbolic_powers(monomial)]
-        elif str(monomial) == '1':
+        if str(monomial) == '1':
             return self.identity_operator
-        elif isinstance(monomial, tuple) or isinstance(monomial, list):
+        elif isinstance(monomial, str):
+            try:
+                return self.monomial_from_name[monomial]
+            except KeyError:
+                factors = monomial.split("*")
+        elif isinstance(monomial, (tuple, list)):
             factors = [str(factor) for factor in monomial]
+        elif isinstance(monomial, sp.core.symbol.Expr):
+            try:
+                return self.monomial_from_symbol[monomial]
+            except KeyError:
+                factors = [str(factor)
+                           for factor in flatten_symbolic_powers(monomial)]
         else:
-            assert "^" not in monomial, "Cannot interpret exponents."
-            factors = monomial.split("*")
+            raise Exception(f'Cannot interpret monomial with name {monomial} of type {type(monomial)}')
         return np.vstack(tuple(self._interpret_atomic_string(factor_string)
                                for factor_string in factors))
 
     def _interpret_atomic_string(self, factor_string: str) -> np.ndarray:
         """Build a 2D array encoding of a moment that cannot be further
         factorised into products of other moments.
 
@@ -1416,48 +1662,55 @@
             ``"<A_1_1_1_2*B_2_1_3_4>"``.
 
         Returns
         -------
         numpy.ndarray
             2D array encoding of the input atomic moment.
         """
+        try:
+            return self.atom_from_name[factor_string].as_2d_array
+        except (KeyError, AttributeError):
+            pass
         assert ((factor_string[0] == "<" and factor_string[-1] == ">")
+                or (factor_string[0:1] == "P[" and factor_string[-1] == "]")
                 or set(factor_string).isdisjoint(set("| "))), \
             ("Monomial names must be between < > signs, or in conditional " +
-             "probability form.")
-        if factor_string[0] == "<":
-            operators = factor_string[1:-1].split(" ")
+             f"probability form, whereas input received was {factor_string}")
+        if factor_string[-1] in {'>', ')', "]", "}"}:
+            cleaned_factor_string = factor_string[:-1]
+            substrings_to_kill = {"P[", "P(", "p[", "p(", "<"}
+            for substring in substrings_to_kill:
+                cleaned_factor_string = cleaned_factor_string.replace(
+                    substring, '')
+            cleaned_factor_string = cleaned_factor_string.replace(' & ', ' ')
+            operators = cleaned_factor_string.split(" ")
             return np.vstack(tuple(self._interpret_operator_string(op_string)
                                    for op_string in operators))
         else:
             return self._interpret_operator_string(factor_string)[np.newaxis]
 
     def _interpret_operator_string(self, op_string: str) -> np.ndarray:
         """Build a 1D array encoding of an operator passed as a string.
 
         Parameters
         ----------
-        factor_string : str
+        op_string : str
             String representation of an operator, e.g., ``"B_2_1_3_4"``.
 
         Returns
         -------
         numpy.ndarray
             2D array encoding of the operator.
         """
-        components = op_string.split("_")
-        assert len(components) == self._nr_properties, \
-            f"There need to be {self._nr_properties} properties to match " + \
-            "the scenario."
-        components[0] = self.names_to_ints[components[0]]
-        return np.array([int(s) for s in components], dtype=self.np_dtype)
+        return self._lexorder[self.op_from_name[op_string]]
 
     ###########################################################################
     # ROUTINES RELATED TO THE GENERATION OF THE MOMENT MATRIX                 #
     ###########################################################################
+    
     def _build_cols_from_specs(self, col_specs: List[List[int]]) -> List:
         """Build the generating set for the moment matrix taking as input a
         block specified only the number of parties.
 
         For example, with ``col_specs=[[], [0], [2], [0, 2]]`` as input, we
         generate the generating set S={1, A_{inf}_xa, C_{inf'}_zc,
         A_{inf''}_x'a' * C{inf'''}_{z'c'}} where inf, inf', inf'' and inf'''
@@ -1483,137 +1736,142 @@
             # Display col_specs in a readable way
             to_print = []
             for specs in col_specs:
                 to_print.append("1" if specs == []
                                 else "".join([self.names[p] for p in specs]))
             print("Column structure:", "+".join(to_print))
 
+        _zero_lexorder = np.array([0], dtype=np.intc)
         columns      = []
         seen_columns = set()
-        for block in col_specs:
-            if len(block) == 0:
-                columns.append(self.identity_operator)
-                seen_columns.add(self._from_2dndarray(self.identity_operator))
+        for block in tqdm(col_specs, desc="Generating columns  ",
+                          disable=not self.verbose):
+            if block == []:
+                _id = self.mon_to_lexrepr(self.identity_operator)
+                seen_columns.add(tuple(_id))
+                columns += [_id]
             else:
-                meas_ops = []
-                for party in block:
-                    meas_ops.append(flatten(self.measurements[party]))
-                for monomial_factors in product(*meas_ops):
-                    mon   = self._interpret_name(monomial_factors)
-                    canon = self._to_canonical_memoized(mon)
-                    if not np.array_equal(canon, 0):
-                        # If the block is [0, 0], and we have the monomial
-                        # A**2 which simplifies to A, then A could be included
-                        # in the block [0]. We use the convention that [0, 0]
-                        # represents all monomials of length 2 AFTER
-                        # simplifications, so we omit monomials of length 1.
-                        if canon.shape[0] == len(monomial_factors):
-                            key = self._from_2dndarray(canon)
-                            if key not in seen_columns:
-                                seen_columns.add(key)
-                                columns.append(canon)
+                meas_ops = [
+                    np.nonzero(np.logical_and(
+                        self._lexorder[:, 0] == party + 1,
+                        self._lexorder[:, -1] != \
+                            self.outcome_cardinalities[party] - 1))[0]
+                                for party in block]
+                for mon_lexrepr in product(*meas_ops):
+                    canon = self._to_canonical_memoized_1d(mon_lexrepr)
+                    if (not np.array_equal(canon, _zero_lexorder)
+                        and len(canon) == len(block)):
+                        _hash = tuple(canon)
+                        if _hash not in seen_columns:
+                            seen_columns.add(tuple(canon))
+                            columns += [canon]
 
         return columns
 
-    def _build_momentmatrix(self) -> Tuple[np.ndarray, Dict]:
+    def _build_momentmatrix_1d_internal(self) -> Tuple[np.ndarray, Dict]:
         """Wrapper method for building the moment matrix."""
-        problem_arr, canonical_mon_as_bytes_to_idx = \
-            calculate_momentmatrix(self.generating_monomials,
+        problem_arr, canonical_lexmon_to_idx = \
+            calculate_momentmatrix_1d_internal(self.generating_monomials_1d,
                                    self._notcomm,
-                                   self._lexorder,
-                                   commuting=self.commuting,
+                                   self._orthomat,
+                                   commuting=self.all_operators_commute,
                                    verbose=self.verbose)
-        idx_to_canonical_mon = {idx: self._to_2dndarray(mon_as_bytes)
-                                for (mon_as_bytes, idx) in
-                                canonical_mon_as_bytes_to_idx.items()}
-        del canonical_mon_as_bytes_to_idx
-        return problem_arr, idx_to_canonical_mon
+        idx_to_canonical_lexmon = {idx: np.asarray(lexmon, dtype=np.intc)
+                                for (lexmon, idx) in
+                                canonical_lexmon_to_idx.items()}
+        return problem_arr, idx_to_canonical_lexmon
 
     def _discover_normalization_eqns(self) -> List[Tuple[int, List[int]]]:
+        #TODO: Needs major overhaul to efficiently use 1d internal representation
         """Given the generating monomials, infer implicit normalization
         equalities between columns of the moment matrix. Each normalization
         equality is a two element tuple; the first element is an integer
         indicating a particular column of the moment matrix, the second element
         is a list of integers indicating other columns of the moment matrix
         such that the sum of the latter columns is equal to the former column.
 
         Returns
         -------
         List[Tuple[int, List[int]]]
             A list of normalization equalities between columns of the moment
         matrix.
         """
-        skip_party = [not i for i in self.has_children]
+        # skip_party = [not i for i in self.has_children]
+
+        # This will help us identify relevant operators with the last outcome
+        last_outcome_boolmask = np.array(
+            [self.has_children[op[0] - 1] and
+              op[-1] == self.outcome_cardinalities[op[0] - 1] - 2 # TODO -2 is a hack for using fake outcomes
+                                for op in self._lexorder], dtype=bool)
+        
+        # This will allow for easy substitution of operators with the last
+        # outcome with the rest of the operators orthogonal to it
+        lexmon_to_orthogroup = dict()
+        for group in self.InflationProblem._ortho_groups:
+            last_outcome_op = \
+                self.mon_to_lexrepr(np.expand_dims(group[-1], axis=0))[0]
+            lexmon_to_orthogroup[last_outcome_op] = \
+                np.concatenate([self.mon_to_lexrepr(np.expand_dims(m, axis=0))
+                                for m in group], dtype=np.intc)    
+        
         column_level_equalities = []
-        for i, mon in enumerate(self.generating_monomials):
-            eqs = expand_moment_normalisation(mon,
-                                              self.outcome_cardinalities,
-                                              skip_party)
-            for eq in eqs:
-                try:
-                    eq_idxs = [self.genmon_hash_to_index[
-                                                self._from_2dndarray(eq[0])]]
-                    eq_idxs.append([self.genmon_hash_to_index[
-                                    self._from_2dndarray(m)] for m in eq[1]])
-                    column_level_equalities += [tuple(eq_idxs)]
-                except KeyError:
-                    break
+        for i, lexmon in enumerate(self.generating_monomials_1d):
+            last_outcome_ops = last_outcome_boolmask[lexmon]
+            if last_outcome_ops.sum() > 0:
+                eqs = []
+                for i, op in enumerate(lexmon):
+                    if last_outcome_ops[i]:
+                        lhs = np.delete(lexmon, i)  # returns new copy
+                        rhs = np.vstack((lexmon,)*len(lexmon_to_orthogroup[op]))
+                        rhs[:, i] = lexmon_to_orthogroup[op]
+                        eqs += [(lhs, list(rhs))]
+                for eq in eqs:
+                    try:
+                        eq_idxs = [self.genmon_1d_to_index[tuple(eq[0])]]
+                        eq_idxs.append([self.genmon_1d_to_index[tuple(m)]
+                                        for m in eq[1]])
+                        column_level_equalities += [tuple(eq_idxs)]
+                    except KeyError:
+                        break
         return column_level_equalities
 
-    def _discover_inflation_symmetries(self) -> np.ndarray:
+    def _discover_columns_symmetries(self) -> np.ndarray:
         """Calculates all the symmetries and applies them to the set of
         operators used to define the moment matrix. The new set of operators
         is a permutation of the old. The function outputs a list of all
         permutations.
 
         Returns
         -------
         numpy.ndarray[int]
             The list of all permutations of the generating columns implied by
             the inflation symmetries.
         """
-        sources_with_copies = [source for source, inf_level
-                               in enumerate(self.inflation_levels)
-                               if inf_level > 1]
-        if len(sources_with_copies):
-            inflation_symmetries = []
-            identity_perm        = np.arange(self.n_columns, dtype=int)
-            for source in tqdm(sources_with_copies,
-                               disable=not self.verbose,
-                               desc="Calculating symmetries   ",
-                               leave=False,
-                               position=0):
-                one_source_symmetries = [identity_perm]
-                inf_level = self.inflation_levels[source]
-                perms = format_permutations(list(
-                    permutations(range(inf_level)))[1:])
-                permutation_failed = False
-                for permutation in perms:
-                    try:
-                        total_perm = np.empty(self.n_columns, dtype=int)
-                        for i, mon in enumerate(self.generating_monomials):
-                            new_mon = apply_source_perm(mon,
-                                                        source,
-                                                        permutation)
-                            new_mon = self._to_canonical_memoized(new_mon,
-                                                                  True)
-                            total_perm[i] = self.genmon_hash_to_index[
-                                                self._from_2dndarray(new_mon)]
-                        one_source_symmetries.append(total_perm)
-                    except KeyError:
-                        permutation_failed = True
-                inflation_symmetries.append(one_source_symmetries)
-            if permutation_failed and (self.verbose > 0):
-                warn("The generating set is not closed under source swaps."
-                     + " Some symmetries will not be implemented.")
-            inflation_symmetries = [reduce(np.take, perms) for perms in
-                                    product(*inflation_symmetries)]
-            return np.unique(inflation_symmetries[1:], axis=0)
-        else:
-            return np.empty((0, len(self.generating_monomials)), dtype=int)
+        discovered_symmetries = [np.arange(self.n_columns, dtype=int)]
+        permutation_failed = False
+        for inf_sym in self.lexorder_symmetries[1:]:
+            skip_this_one = False
+            try:
+                total_perm = np.empty(self.n_columns, dtype=int)
+                for i, lexmon in enumerate(self.generating_monomials_1d):
+                    new_lexmon = inf_sym[lexmon]
+                    new_lexmon_canon = self._to_canonical_memoized_1d(
+                        new_lexmon,
+                        apply_only_commutations=True)
+                    total_perm[i] \
+                        = self.genmon_1d_to_index[tuple(new_lexmon_canon)]
+            except KeyError:
+                permutation_failed = True
+                skip_this_one = True
+            if not skip_this_one:
+                discovered_symmetries.append(total_perm)
+        if permutation_failed and (self.verbose > 0):
+            warn("The generating set is not closed under source swaps."
+                 + " Some symmetries will not be implemented.")
+        return np.unique(discovered_symmetries, axis=0)[1:]
 
     def _generate_parties(self) -> List[List[List[List[sp.Symbol]]]]:
         """Generates all the party operators in the quantum inflation.
 
         Returns
         -------
         List[List[List[List[sympy.Symbol]]]]
@@ -1634,15 +1892,15 @@
         for pos, [party, ins, outs] in enumerate(zip(parties,
                                                      settings,
                                                      outcomes)):
             party_meas = []
             # Generate all possible copy indices for a party
             all_inflation_indices = product(
                 *[list(range(self.inflation_levels[p_idx]))
-                  for p_idx in np.nonzero(self.hypergraph[:, pos])[0]])
+                  for p_idx in np.flatnonzero(self.hypergraph[:, pos])])
             # Include zeros in the positions of states not feeding the party
             all_indices = []
             for inflation_indices in all_inflation_indices:
                 indices = []
                 i = 0
                 for idx in range(n_states):
                     if self.hypergraph[idx, pos] == 0:
@@ -1666,57 +1924,56 @@
                 party_meas.append(meas)
             measurements.append(party_meas)
         return measurements
 
     ###########################################################################
     # HELPER FUNCTIONS FOR ENSURING CONSISTENCY                               #
     ###########################################################################
+    
     def _cleanup_after_set_values(self) -> None:
         """Helper function to reset or make consistent class attributes after
         setting values."""
         if self.supports_problem:
             # Add lower bounds to monomials inside the support
             nonzero_known_monomials = [mon for
                                        mon, value in self.known_moments.items()
                                        if not np.isclose(value, 0)]
             for mon in nonzero_known_monomials:
-                self._processed_moment_lowerbounds[mon] = 1.
+                self.moment_lowerbounds[mon] = 1.
                 del self.known_moments[mon]
             self.semiknown_moments = dict()
 
-        self._update_lowerbounds()
-        self._update_upperbounds()
+        self._update_bounds("lo")
+        self._update_bounds("up")
         self._update_objective()
         num_nontrivial_known = len(self.known_moments)
         if self.momentmatrix_has_a_zero:
             num_nontrivial_known -= 1
         if self.momentmatrix_has_a_one:
             num_nontrivial_known -= 1
         if self.verbose > 1 and num_nontrivial_known > 0:
             print("Number of variables with fixed numeric value:",
                   len(self.known_moments))
+        if len(self.semiknown_moments):
+            for k in self.known_moments.keys():
+                self.semiknown_moments.pop(k, None)
         num_semiknown = len(self.semiknown_moments)
         if self.verbose > 1 and num_semiknown > 0:
             print(f"Number of semiknown variables: {num_semiknown}")
 
-    def _reset_bounds(self) -> None:
-        """Reset the lists of bounds."""
-        self._reset_lowerbounds()
-        self._reset_upperbounds()
-        collect()
-
     def _reset_lowerbounds(self) -> None:
         """Reset the list of lower bounds."""
         self._reset_solution()
-        self._processed_moment_lowerbounds = dict()
+        self.moment_lowerbounds = {m: 0. for m in self.hermitian_moments}
+        self._update_bounds("lo")
 
     def _reset_upperbounds(self) -> None:
         """Reset the list of upper bounds."""
         self._reset_solution()
-        self._processed_moment_upperbounds = dict()
+        self.moment_upperbounds = dict()
 
     def _reset_objective(self) -> None:
         """Reset the objective function."""
         self._reset_solution()
         self.objective = {self.One: 0.}
         self._processed_objective = self.objective
         self.maximize = True  # Direction of the optimization
@@ -1725,14 +1982,16 @@
         """Reset the known values."""
         self._reset_solution()
         self.known_moments     = dict()
         self.semiknown_moments = dict()
         if self.momentmatrix_has_a_zero:
             self.known_moments[self.Zero] = 0.
         self.known_moments[self.One] = 1.
+        self.extra_equalities = []
+        self.extra_inequalities = []
         collect()
 
     def _update_objective(self) -> None:
         """Process the objective with the information from known_moments
         and semiknown_moments.
         """
         self._processed_objective = self.objective.copy()
@@ -1752,54 +2011,48 @@
             coeff = self._processed_objective[mon]
             for (subs_coeff, subs) in self.semiknown_moments[mon]:
                 self._processed_objective[subs] = \
                     self._processed_objective.get(subs, 0) + coeff * subs_coeff
                 del self._processed_objective[mon]
         collect()
 
-    def _update_lowerbounds(self) -> None:
-        """Helper function to check that lowerbounds are consistent with the
-        specified known values, and to keep only the lowest lowerbounds
-        in case of redundancy.
-        """
-        for mon, lb in self.moment_lowerbounds.items():
-            self._processed_moment_lowerbounds[mon] = \
-                max(self._processed_moment_lowerbounds.get(mon, -np.infty), lb)
-        for mon, value in self.known_moments.items():
-            if isinstance(value, Real):
-                try:
-                    lb = self._processed_moment_lowerbounds[mon]
-                    assert lb <= value, (f"Value {value} assigned for " +
-                                         f"monomial {mon} contradicts the " +
-                                         f"assigned lower bound of {lb}.")
-                    del self._processed_moment_lowerbounds[mon]
-                except KeyError:
-                    pass
-        self.moment_lowerbounds = self._processed_moment_lowerbounds
-
-    def _update_upperbounds(self) -> None:
-        """Helper function to check that upperbounds are consistent with the
+    def _update_bounds(self, typ: str) -> None:
+        """Helper function to check that bounds are consistent with the
         specified known values.
+
+        Parameters
+        ----------
+        typ : str
+            Specification of upper (`"up"`) or lower (`"lo"`) bounds.
         """
+        if typ == "up":
+            bounds = self.moment_upperbounds
+            dir = "upp"
+        elif typ == "lo":
+            bounds = self.moment_lowerbounds
+            dir = "low"
+        else:
+            raise Exception(f"The bound type was {typ}, but it must be " +
+                            "either \"up\" or \"lo\".")
         for mon, value in self.known_moments.items():
             if isinstance(value, Real):
                 try:
-                    ub = self._processed_moment_upperbounds[mon]
-                    assert ub >= value, (f"Value {value} assigned for " +
-                                         f"monomial {mon} contradicts the " +
-                                         f"assigned upper bound of {ub}.")
-                    del self._processed_moment_upperbounds[mon]
+                    b = bounds[mon]
+                    condition = (b >= value) if typ == "up" else (b <= value)
+                    assert condition, (f"Value {value} assigned for " +
+                                       f"monomial {mon} contradicts the " +
+                                       f"assigned {dir}er bound of {b}.")
+                    del bounds[mon]
                 except KeyError:
                     pass
-        self.moment_upperbounds = self._processed_moment_upperbounds
-
 
     ###########################################################################
     # OTHER ROUTINES                                                          #
     ###########################################################################
+    
     def _atomic_knowable_q(self, atomic_monarray: np.ndarray) -> bool:
         """Return ``True`` if the input monomial, encoded as a 2D array,
         can be associated to a knowable value in the scenario, and ``False``
         otherwise.
 
         Parameters
         ----------
@@ -1816,15 +2069,15 @@
         elif self.network_scenario:
             return True
         else:
             return self._is_knowable_q_non_networks(np.take(atomic_monarray,
                                                             [0, -2, -1],
                                                     axis=1))
 
-    def _from_2dndarray(self, array2d: np.ndarray) -> None:
+    def _from_2dndarray(self, array2d: np.ndarray) -> bytes:
         """Obtains the bytes representation of an array. The library uses this
         representation as hashes for the corresponding monomials.
 
         Parameters
         ----------
         array2d : numpy.ndarray
             Monomial encoded as a 2D array.
@@ -1858,45 +2111,45 @@
         Exception
             If the SDP relaxation has not been calculated yet.
         """
         if not self._relaxation_has_been_generated:
             raise Exception("Relaxation is not generated yet. " +
                             "Call \"InflationSDP.get_relaxation()\" first")
 
-        assert set(self.known_moments.keys()).issubset(self.monomials),\
+        assert set(self.known_moments.keys()).issubset(self.moments),\
             ("Error: Tried to assign known values outside of moment matrix: " +
              str(set(self.known_moments.keys()
-                     ).difference(self.monomials)))
+                     ).difference(self.moments)))
         if len(self.maskmatrices) == 0:
             self._construct_mask_matrices()
         solverargs = {"mask_matrices": {mon.name: mask_matrix
                                         for mon, mask_matrix
                                         in self.maskmatrices.items()},
                       "objective": {mon.name: coeff for mon, coeff
                                     in self._processed_objective.items()},
                       "known_vars": {mon.name: val for mon, val
                                      in self.known_moments.items()},
                       "semiknown_vars": {mon.name: (coeff, subs.name)
                                          for mon, (coeff, subs)
                                          in self.semiknown_moments.items()},
                       "equalities": [{mon.name: coeff
                                           for mon, coeff in eq.items()}
-                                         for eq in self.moment_equalities],
+                                     for eq in self.minimal_equalities],
                       "inequalities": [{mon.name: coeff
                                         for mon, coeff in ineq.items()}
-                                       for ineq in self.moment_inequalities]
+                                       for ineq in self.minimal_inequalities]
                       }
         # Add the constant 1 in case of unnormalized problems removed it
         solverargs["known_vars"][self.constant_term_name] = 1.
-        for mon, bnd in self._processed_moment_lowerbounds.items():
+        for mon, bnd in self.moment_lowerbounds.items():
             lb = {mon.name: 1}
             if not np.isclose(bnd, 0):
                 lb[self.constant_term_name] = -bnd
             solverargs["inequalities"].append(lb)
-        for mon, bnd in self._processed_moment_upperbounds.items():
+        for mon, bnd in self.moment_upperbounds.items():
             ub = {mon.name: -1}
             if not np.isclose(bnd, 0):
                 ub[self.constant_term_name] = bnd
             solverargs["inequalities"].append(ub)
         solverargs["mask_matrices"][self.constant_term_name] = lil_matrix(
             (self.n_columns, self.n_columns))
         return solverargs
@@ -1909,67 +2162,14 @@
                           "solution_object"}:
             try:
                 delattr(self, attribute)
             except AttributeError:
                 pass
         self.status = "Not yet solved"
 
-    def _set_upperbounds(self, upperbounds: Union[dict, None]) -> None:
-        """Set upper bounds for variables in the SDP relaxation.
-
-        Parameters
-        ----------
-        upperbounds : Union[dict, None]
-            Dictionary with keys as moments and values as upper bounds. The
-            keys can be either strings, instances of `CompoundMonomial` or
-            moments encoded as 2D arrays.
-        """
-        self._reset_upperbounds()
-        if upperbounds is None:
-            return
-        sanitized_upperbounds = dict()
-        for mon, upperbound in upperbounds.items():
-            mon = self._sanitise_monomial(mon)
-            if mon not in sanitized_upperbounds.keys():
-                sanitized_upperbounds[mon] = upperbound
-            else:
-                old_bound = sanitized_upperbounds[mon]
-                assert np.isclose(old_bound,
-                                  upperbound), \
-                    (f"Contradiction: Cannot set the same monomial {mon} to " +
-                     "have different upper bounds.")
-        self._processed_moment_upperbounds = sanitized_upperbounds
-        self._update_upperbounds()
-
-    def _set_lowerbounds(self, lowerbounds: Union[dict, None]) -> None:
-        """Set lower bounds for variables in the SDP relaxation.
-
-        Parameters
-        ----------
-        upperbounds : Union[dict, None]
-            Dictionary with keys as moments and values as upper bounds. The
-            keys can be either strings, instances of `CompoundMonomial` or
-            moments encoded as 2D arrays.
-        """
-        self._reset_lowerbounds()
-        if lowerbounds is None:
-            return
-        sanitized_lowerbounds = dict()
-        for mon, lowerbound in lowerbounds.items():
-            mon = self._sanitise_monomial(mon)
-            if mon not in sanitized_lowerbounds.keys():
-                sanitized_lowerbounds[mon] = lowerbound
-            else:
-                old_bound = sanitized_lowerbounds[mon]
-                assert np.isclose(old_bound, lowerbound), \
-                    (f"Contradiction: Cannot set the same monomial {mon} to " +
-                     "have different lower bounds.")
-        self._processed_moment_lowerbounds = sanitized_lowerbounds
-        self._update_lowerbounds()
-
     def _to_2dndarray(self, bytestream: bytes) -> np.ndarray:
         """Create a monomial array from its corresponding stream of bytes.
 
         Parameters
         ----------
         bytestream : bytes
             The stream of bytes encoding the monomial.
@@ -2008,13 +2208,85 @@
         try:
             return self.canon_ndarray_from_hash[key]
         except KeyError:
             if len(array2d) == 0 or np.array_equiv(array2d, 0):
                 self.canon_ndarray_from_hash[key] = array2d
                 return array2d
             else:
-                new_array2d = to_canonical(array2d, self._notcomm, self._lexorder,
-                                           self.commuting, apply_only_commutations)
+                lexmon = self.mon_to_lexrepr(array2d)
+                new_lexmon = to_canonical_1d_internal(lexmon,
+                                                       self._notcomm,
+                                                       self._orthomat,
+                                                       self.all_operators_commute,
+                                                       apply_only_commutations)
+                new_array2d = self._lexorder[new_lexmon]
                 new_key = self._from_2dndarray(new_array2d)
                 self.canon_ndarray_from_hash[key]     = new_array2d
                 self.canon_ndarray_from_hash[new_key] = new_array2d
                 return new_array2d
+
+    def _to_canonical_memoized_1d(self,
+                                  lexmon: np.ndarray,
+                                  apply_only_commutations=False) -> np.ndarray:
+        """Cached function to convert a monomial to its canonical form.
+
+        It checks whether the input monomial's canonical form has already been
+        calculated and stored in the ``InflationSDP.canon_ndarray_from_hash``.
+        If not, it calculates it.
+
+        Parameters
+        ----------
+        lexmon : numpy.ndarray
+            Moment encoded as a 1D array.
+        apply_only_commutations : bool, optional
+            If ``True``, skip the removal of projector squares and the test to
+            see if the monomial is equal to zero, by default ``False``.
+
+        Returns
+        -------
+        numpy.ndarray
+            Moment in canonical form as 1D array.
+        """
+        key = tuple(lexmon)
+        try:
+            return self.canon_lexmon_from_hash[key]
+        except KeyError:
+            if len(lexmon) == 0 or np.array_equiv(lexmon, 0):
+                self.canon_lexmon_from_hash[key] = lexmon
+                return lexmon
+            else:
+                new_lexmon = \
+                    to_canonical_1d_internal(
+                        np.asarray(lexmon, dtype=np.int32),
+                        self._notcomm, self._orthomat, 
+                        self.all_operators_commute,
+                        apply_only_commutations=apply_only_commutations)
+                new_key = tuple(new_lexmon)
+                self.canon_lexmon_from_hash[key]     = new_lexmon
+                self.canon_lexmon_from_hash[new_key] = new_lexmon
+                return new_lexmon
+
+    def mon_to_lexrepr(self, mon: np.ndarray) -> np.ndarray:
+        """Convert a monomial from 2D array form to its lexicographic form.
+
+        In the 2D array form, rows represent operators and columns represent
+        properties. In the lexicographic form, each entry represents the index
+        of the operator in the lexicographic order.
+        
+        Example: ``[[1, 0, 1], [2, 0, 0], [1, 1, 0]]``, with 
+        ``lexorder=[[1, 0, 0], [1, 0, 1], [1, 1, 0], [1, 1, 1], [2, 0, 0]]``
+        is converted to ``[1, 4, 2]``.
+
+        Parameters
+        ----------
+        mon : np.ndarray
+            Monomial in 2D array form.
+
+        Returns
+        -------
+        np.ndarray
+            Monomial in the 1D lexicographic form.
+        """
+        template = np.empty(len(mon), dtype=object)
+        template[:] = np.asarray(mon, self.np_dtype).ravel().view(self._astuples_dtype)
+        return np.array(partsextractor(self.op_to_lexrepr_dict, template), dtype=np.intc)
+        # return nb_mon_to_lexrepr(mon, self._lexorder)
```

### Comparing `inflation-1.0.0/inflation/sdp/fast_npa.py` & `inflation-2.0.0/inflation/sdp/fast_npa.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
 This file contains helper functions to manipulate monomials and generate moment
 matrices. The functions in this file can be accelerated by JIT compilation in
 numba.
+
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
 """
 import numpy as np
 
 from typing import List
 
 try:
-    from numba import jit, prange
+    from numba import jit
     from numba.types import bool_, void
     from numba.types import uint8 as uint8_
+    from numba.types import intc as int_
     nopython = True
 except ImportError:
+    print("Warning: NOT using Numba for JIT compilation.")
     def jit(*args, **kwargs):
         return lambda f: f
     bool_    = bool
     nopython = False
-    prange   = range
     uint8_   = np.uint8
+    int_     = np.intc
     void     = None
 
 cache    = True
 if not nopython:
     from scipy.sparse.csgraph import connected_components
     bool_  = bool
     uint8_ = np.uint8
@@ -60,39 +63,14 @@
     >>> dot_mon(mon1, mon2)
     np.array([[4,5,6],[1,2,3],[7,8,9]])
     """
     return np.concatenate((reverse_mon(mon1), mon2))
 
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
-def mon_is_zero(mon: np.ndarray) -> bool_:
-    """Function which checks if a monomial is equivalent to the zero monomial.
-    This is the case if there is a product of two orthogonal projectors, or if
-    the monomial is equal to the canonical zero monomial.
-
-    Parameters
-    ----------
-    mon : numpy.ndarray
-        Input monomial in 2d array format.
-
-    Returns
-    -------
-    bool
-        Whether the monomial evaluates to zero.
-    """
-    if len(mon) >= 1 and not np.any(mon.ravel()):
-        return True
-    for i in range(1, mon.shape[0]):
-        if ((mon[i, -1] != mon[i - 1, -1])
-                and np.array_equal(mon[i, :-1], mon[i - 1, :-1])):
-            return True
-    return False
-
-
-@jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def mon_lexsorted(mon: np.ndarray,
                   lexorder: np.ndarray) -> np.ndarray:
     """Sorts a monomial lexicographically.
 
     Parameters
     ----------
     mon : numpy.ndarray
@@ -133,20 +111,20 @@
     if not nopython:
         return connected_components(adj_mat,
                                     directed=False,
                                     return_labels=True)[-1]
     # See https://stackoverflow.com/a/9112588 for inspiration of the method
     n = len(adj_mat)
     if n <= 1 or adj_mat.all():
-        return np.zeros(n, dtype=np.uint8)
-    component_labels = np.zeros(n, dtype=np.uint8)
+        return np.zeros((n,), dtype=uint8_)
+    component_labels = np.zeros((n,), dtype=uint8_)
     component_counter = 1
     for i in range(n):
         if not component_labels[i]:
-            old_component = np.logical_not(np.ones(n, dtype=np.uint8))
+            old_component = np.logical_not(np.ones((n,), dtype=uint8_))
             new_component = old_component.copy()
             new_component[i] = True
             search_next = np.logical_xor(new_component, old_component)
             while search_next.any():
                 old_component = new_component.copy()
                 new_component = np.logical_or(
                     new_component,
@@ -182,62 +160,14 @@
     for source in monomial.T[1:-2]:
         if len(np.unique(source[np.flatnonzero(source)])) > 1:
             return False
     return True
 
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
-def nb_is_physical(monomial_in: np.ndarray, sandwich_positivity=True) -> bool_:
-    r"""Determines whether a monomial is physical, this is, if it always has a
-    non-negative expectation value.
-
-    This code also supports the detection of "sandwiches", i.e., monomials
-    of the form :math:`\langle \psi | A_1 A_2 A_1 | \psi \rangle` where
-    :math:`A_1` and :math:`A_2` do not commute. In principle we do not know the
-    value of this term. However, note that :math:`A_1` can be absorbed into
-    :math:`| \psi \rangle` forming an unnormalised quantum state
-    :math:`| \psi' \rangle`, thus :math:`\langle\psi'|A_2|\psi'\rangle`.
-    Note that while we know the value :math:`\langle\psi |A_2| \psi\rangle`,
-    we do not know :math:`\langle \psi' | A_2 | \psi' \rangle` because of
-    the unknown normalisation, however we know it must be non-negative,
-    :math:`\langle \psi | A_1 A_2 A_1 | \psi \rangle \geq 0`.
-    This simple example can be extended to various layers of sandwiching.
-
-    Parameters
-    ----------
-    monomial_in : numpy.ndarray
-        Input monomial in 2d array format.
-    sandwich_positivity : bool, optional
-        Whether to consider sandwiching. By default ``True``.
-
-    Returns
-    -------
-    bool
-        Whether the monomial has always non-negative expectation or not.
-    """
-    if len(monomial_in) <= 1:
-        return True
-    if sandwich_positivity:
-        monomial = nb_remove_sandwich(monomial_in)
-        if len(monomial) <= 1:
-            return True
-    else:
-        monomial = monomial_in
-    parties = np.unique(monomial[:, 0])
-    for party in parties:
-        party_monomial = monomial[monomial[:, 0] == party]
-        n = len(party_monomial)
-        if not n == 1:
-            component_labels = nb_monomial_to_components(party_monomial)
-            if np.max(component_labels) + 1 != n:
-                return False
-    return True
-
-
-@jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def nb_lexorder_idx(operator: np.ndarray,
                     lexorder: np.ndarray) -> int:
     """Return the unique integer corresponding to the lexicographic ordering of
     the operator. If ``operator`` is not found in ``lexorder``, no value is
     returned.
 
     Parameters
@@ -252,18 +182,17 @@
     -------
     int
         The index of the operator in the lexorder matrix.
     """
     for i in range(lexorder.shape[0]):
         if np.array_equal(lexorder[i, :], operator):
             return i
-    print("nb_lexorder_idx: Operator not found in lexorder.")
+    return -1
 
-
-@jit(nopython=nopython, cache=cache, forceobj=not nopython, parallel=True)
+@jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def nb_mon_to_lexrepr(mon: np.ndarray,
                       lexorder: np.ndarray) -> np.array:
     """Convert a monomial to its lexicographic representation, in the form of
     an array of integers representing the lexicographic rank of each operator.
 
     Parameters
     ----------
@@ -275,16 +204,16 @@
 
     Returns
     -------
     np.array
         Monomial as array of integers, where each integer is the hash
         of the corresponding operator.
     """
-    lex = np.zeros(mon.shape[0], dtype=lexorder.dtype)
-    for i in prange(mon.shape[0]):
+    lex = np.empty(mon.shape[0], dtype=int_)
+    for i in range(mon.shape[0]):
         lex[i] = nb_lexorder_idx(mon[i], lexorder)
     return lex
 
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def nb_monomial_to_components(monomial: np.ndarray) -> np.ndarray:
     """Wrapper for obtaining the list of disconnected components of a monomial.
@@ -310,20 +239,20 @@
                              [3, 6, 6, 0, 0, 0],
                              [3, 4, 5, 0, 0, 0]])
     >>> factorised = nb_monomial_to_components(monomial)
     [0, 1, 2, 3, 1, 4, 3]
     """
     n = len(monomial)
     if n <= 1:
-        return np.zeros(n, dtype=np.uint8)
+        return np.zeros(n, dtype=uint8_)
     return nb_classify_disconnected_components(nb_overlap_matrix(
         monomial[:, 1:-2]))
 
 
-@jit(nopython=nopython, cache=cache, forceobj=not nopython, parallel=True)
+@jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def nb_overlap_matrix(inflation_indxs: np.ndarray) -> np.ndarray:
     """Given a list of inflation indices for a number of operators, generate
     a boolean matrix whose entries denote whether the supports of the operator
     indexed by the row and of the operator indexed by the column overlap.
 
     Parameters
     ----------
@@ -334,56 +263,97 @@
     -------
     numpy.ndarray
         The "adjacency matrix" whose entries denote whether the supports of the
         operator indexed by the row and of the operator indexed by the column
         overlap.
     """
     n = len(inflation_indxs)
-    adj_mat = np.eye(n, dtype=np.bool_)
-    for i in prange(1, n):
+    adj_mat = np.eye(n, dtype=bool_)
+    for i in range(1, n):
         inf_indices_i = inflation_indxs[i]
         for j in range(i):
             inf_indices_j = inflation_indxs[j]
             if nb_exists_shared_source(inf_indices_i, inf_indices_j):
                 adj_mat[i, j] = True
     adj_mat = np.logical_or(adj_mat, adj_mat.T)
     return adj_mat
 
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
-def nb_remove_sandwich(monomial: np.ndarray) -> np.ndarray:
-    r"""Removes sandwiching/pinching from a monomial. This is, it converts the
-    monomial represented by :math:`U A U^\dagger` into :math:`A`.
+def nb_indices_of_more_than_one_op_per_party_per_factor(monomial: np.ndarray,
+                                                        sandwich_positivity=True) -> np.ndarray:
+    r"""If sandwich_positivity=True, this removes sandwiching/pinching from the
+    monomial. This is, it converts the monomial represented by
+    :math:`U A U^\dagger` into :math:`A`.
+    Regardless, it then factorises the monomial into components, yielding
+    a boolean vector where True indicates an operator which appears in the same
+    factor as another of the same party.
 
     Parameters
     ----------
     monomial : numpy.ndarray
         Input monomial.
+    sandwich_positivity : bool, optional
+        Whether to consider sandwiching. By default ``True``.
 
     Returns
     -------
     numpy.ndarray
         The monomial without sandwiches.
     """
-    picklist = np.logical_not(np.ones(len(monomial), dtype=np.uint8))
+    picklist = np.logical_not(np.ones(len(monomial)))
     parties = np.unique(monomial[:, 0])
     for party in parties:
         indices_for_this_party = np.flatnonzero(monomial[:, 0] == party)
         party_monomial = monomial[indices_for_this_party]
         party_monomial_comp_labels = nb_monomial_to_components(party_monomial)
         for i in range(party_monomial_comp_labels.max() + 1):
             indices_for_this_factor = np.flatnonzero(
                 party_monomial_comp_labels == i)
             factor = party_monomial[indices_for_this_factor]
-            while (len(factor) > 1) and np.array_equal(factor[0], factor[-1]):
-                indices_for_this_factor = indices_for_this_factor[1:-1]
-                factor = factor[1:-1]
-            picklist[indices_for_this_party[indices_for_this_factor]] = True
-    return monomial[picklist]
+            # We now only return factors with more than one operator for a single party!
+            if sandwich_positivity:
+                while len(factor) and np.array_equal(factor[0], factor[-1]):
+                    indices_for_this_factor = indices_for_this_factor[1:-1]
+                    factor = factor[1:-1]
+            if len(factor) > 1:
+                picklist[indices_for_this_party[indices_for_this_factor]] = True
+    return picklist
+
+@jit(nopython=nopython, cache=cache, forceobj=not nopython)
+def nb_is_physical(monomial_in: np.ndarray, sandwich_positivity=True) -> bool_:
+    r"""Determines whether a monomial is physical, this is, if it always has a
+    non-negative expectation value.
 
+    This code also supports the detection of "sandwiches", i.e., monomials
+    of the form :math:`\langle \psi | A_1 A_2 A_1 | \psi \rangle` where
+    :math:`A_1` and :math:`A_2` do not commute. In principle we do not know the
+    value of this term. However, note that :math:`A_1` can be absorbed into
+    :math:`| \psi \rangle` forming an unnormalised quantum state
+    :math:`| \psi' \rangle`, thus :math:`\langle\psi'|A_2|\psi'\rangle`.
+    Note that while we know the value :math:`\langle\psi |A_2| \psi\rangle`,
+    we do not know :math:`\langle \psi' | A_2 | \psi' \rangle` because of
+    the unknown normalisation, however we know it must be non-negative,
+    :math:`\langle \psi | A_1 A_2 A_1 | \psi \rangle \geq 0`.
+    This simple example can be extended to various layers of sandwiching.
+
+    Parameters
+    ----------
+    monomial_in : numpy.ndarray
+        Input monomial in 2d array format.
+    sandwich_positivity : bool, optional
+        Whether to consider sandwiching. By default ``True``.
+
+    Returns
+    -------
+    bool
+        Whether the monomial has always non-negative expectation or not.
+    """
+    return not nb_indices_of_more_than_one_op_per_party_per_factor(
+        monomial_in, sandwich_positivity=sandwich_positivity).any()
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def remove_projector_squares(mon: np.ndarray) -> np.ndarray:
     """Simplify the monomial by removing operator powers. This is because we
     assume projectors, P**2=P. This corresponds to removing duplicates of rows
     which are adjacent.
 
@@ -486,26 +456,35 @@
     new_factors = monomial.copy()
     new_factors[:, 1 + source] = permutation[new_factors[:, 1 + source]]
     return new_factors
 
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def commutation_matrix(lexorder: np.ndarray,
+                       sources_to_check_for_pairwise: np.ndarray,
                        commuting=False) -> np.ndarray:
     """Build a matrix encoding of which operators commute according to the
     function ``nb_operators_commute``. Rows and columns are indexed by
     operators, and each element is a 0 if the operators in the row and in the
     column commute or 1 if they do not.
 
     Parameters
     ----------
     lexorder : numpy.ndarray
         Matrix with rows as operators where the index of the row gives the
         lexicographic order of the operator.
-
+    quantum_sources: numpy.ndarray
+        List of integers denoting the columns that in the 2D array encoding
+        corresponding to inflation indices of quantum sources (as opposed to
+        classical sources). Example: np.array([1, 3]) implies that the 1st
+        and 3rd columns of an operator in 2D array form correspond to inflation
+        indices that act on quantum sources.
+    sources_to_check_for_pairwise: numpy.ndarray
+        A 3-index tensor boolean array which keep track of which pairs of parties
+        have which quantum sources in common via intermediate quantum latents.
     commuting : bool
         Whether all the monomials commute. In such a case, the trivial all-zero
         array is returned.
 
     Returns
     -------
     numpy.ndarray
@@ -514,15 +493,16 @@
         value 0 if they commute.
     """
     notcomm = np.zeros((lexorder.shape[0], lexorder.shape[0]), dtype=bool_)
     if not commuting:
         for i in range(lexorder.shape[0]):
             for j in range(i + 1, lexorder.shape[0]):
                 notcomm[i, j] = not nb_operators_commute(lexorder[i],
-                                                         lexorder[j])
+                                                         lexorder[j],
+                                                         sources_to_check_for_pairwise)
         notcomm = notcomm + notcomm.T
     return notcomm
 
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def nb_all_commuting_q(mon: np.ndarray,
                        lexorder: np.ndarray,
@@ -576,16 +556,14 @@
         common, ``False`` if they do not.
     """
     common_sources = np.logical_and(inf_indices1, inf_indices2)
     if not np.any(common_sources):
         return False
     return not np.subtract(inf_indices1[common_sources],
                            inf_indices2[common_sources]).all()
-
-
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def nb_lexmon_to_canonical(lexmon: np.ndarray,
                            notcomm: np.ndarray) -> np.ndarray:
     """Brings a monomial, input as the indices of the operators in the
     lexicographic ordering, to canonical form with respect to commutations.
 
     Parameters
@@ -598,166 +576,176 @@
         `inflation.sdp.fast_npa.commutation_matrix`.
 
     Returns
     -------
     numpy.ndarray
         Monomial in canonical form with respect to commutations.
     """
-    if lexmon.shape[0] <= 1:
-        return lexmon
-
-    # Take only the rows and columns of notcomm that appear in the monomial,
-    # in the correct order.
-    sub_notcomm = notcomm[lexmon, :][:, lexmon]
-    if not sub_notcomm.any():
-        return np.sort(lexmon)
-    if sub_notcomm.all():
-        return lexmon
-    minimum = lexmon[0]
-    minimum_idx = 0
-    for op in range(1, lexmon.shape[0]):
-        # Find the lowest position where we can move op
-        nc_ops_position = np.where(sub_notcomm[op, :op] == 1)[0]
-        if nc_ops_position.size < 1:
-            if lexmon[op] < minimum:
-                minimum_idx = op
-                minimum     = lexmon[op]
-    if minimum <= lexmon[0]:
-        m1 = np.array([lexmon[minimum_idx]])
-        m2 = np.concatenate((lexmon[:minimum_idx],
-                             lexmon[minimum_idx + 1:]))
-        return np.concatenate((m1, nb_lexmon_to_canonical(m2, notcomm)))
-    else:
-        m1 = np.array([lexmon[0]])
-        m2 = lexmon[1:]
-        return np.concatenate((m1, nb_lexmon_to_canonical(m2, notcomm)))
-
+    result = np.empty((0,), dtype=int_)
+    leftover = lexmon
+    while leftover.shape[0] > 1:
+        lexmon = leftover
+        ########################################################################
+        # A subroutine that splits lexmon into two monomials, m1 and m2,
+        # such that m1 is appended to result, and m2 is the new lexmon for a
+        # new iteration of the while loop.
+        # This subroutine should be defined in a function but numba
+        # gives problems with returning tuples (m1,m2) from functions.
+        if lexmon.shape[0] <= 1:
+            m1, m2 = lexmon, np.empty((0,), dtype=int_)
+        else:
+            # Take only the rows and columns of notcomm that appear in the
+            # monomial, in the correct order.
+            sub_notcomm = notcomm[lexmon, :][:, lexmon]
+            if sub_notcomm.all():
+                m1, m2 = lexmon, np.empty((0,), dtype=int_)
+            elif not sub_notcomm.any():
+                m1, m2 = np.sort(lexmon), np.empty((0,), dtype=int_)
+            else:
+                minimum = lexmon[0]
+                minimum_idx = 0
+                for op in range(1, lexmon.shape[0]):
+                    # Find the lowest position where we can move op
+                    nc_ops_position = np.where(sub_notcomm[op, :op] == 1)[0]
+                    if nc_ops_position.size < 1:
+                        if lexmon[op] < minimum:
+                            minimum_idx = op
+                            minimum     = lexmon[op]
+                if minimum <= lexmon[0]:
+                    m1 = np.array([lexmon[minimum_idx]])
+                    m2 = np.concatenate((lexmon[:minimum_idx],
+                                        lexmon[minimum_idx + 1:]))
+                else:
+                    m1 = np.array([lexmon[0]])
+                    m2 = lexmon[1:]
+        ########################################################################
+        result = np.concatenate((result, m1))
+        leftover = m2
+    # Depending on how the while loop ends, we may have a leftover monomial
+    if leftover.shape[0] != 0:
+        result = np.concatenate((result, leftover))
+    return result
 
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
 def nb_operators_commute(operator1: np.ndarray,
-                         operator2: np.ndarray) -> bool_:
+                         operator2: np.ndarray,
+                         sources_to_check_for_pairwise: np.ndarray
+                         ) -> bool_:
     """Determine if two operators commute. Currently, this only takes into
     account commutation coming from inflation and settings.
 
     Parameters
     ----------
     operator1 : numpy.ndarray
         Operator as an array of integers.
     operator2 : numpy.ndarray
         Operator as an array of integers.
+    sources_to_check_for_pairwise: numpy.ndarray
+        A 3-index tensor boolean array which keep track of which pairs of parties
+        have which quantum or classical sources in common via intermediate latents.
 
     Returns
     -------
     bool
         ``True`` if ``operator1`` and ``operator2`` commute, ``False`` if they
         do not.
 
     Examples
     --------
-    A^11_00 commutes with A^22_00
-    >>> nb_operators_commute(np.array([1, 1, 1, 0, 0]),
-                             np.array([1, 2, 2, 0, 0]))
-    True
-
     A^11_00 does not commute with A^12_00 because they overlap on source 1.
     >>> nb_operators_commute(np.array([1, 1, 1, 0, 0]),
-                             np.array([1, 1, 2, 0, 0]))
+                             np.array([1, 1, 2, 0, 0]),  np.array([[[2,2],[0,0]],[[0,0],[2,2]]))
     False
+    
+    A^11_00 commutes with A^12_00 because source 1 is classical.
+    >>> nb_operators_commute(np.array([1, 1, 1, 0, 0]),
+                             np.array([1, 1, 2, 0, 0]),  np.array([[[1,2],[0,0]],[[0,0],[1,2]]))
+    True
     """
-    if operator1[0] != operator2[0]:  # Different parties
+    # Case 0: Different parties commute
+    party1 = operator1[0] - 1
+    party2 = operator2[0] - 1
+    relevant_sources = sources_to_check_for_pairwise[party1, party2]
+    common_source_positions_all = np.greater_equal(relevant_sources, 1)
+    common_source_positions_quantum = np.greater_equal(relevant_sources, 2)
+
+    # Case 1: no common quantum source TYPE
+    if not common_source_positions_quantum.any():
         return True
-    if np.array_equal(operator1[1:-1], operator2[1:-1]):  # sources & settings
+    # Case 2: yes common quantum source TYPE, but different INDICES across all quantum source
+    sources1 = operator1[1:-2]
+    sources2 = operator2[1:-2]
+    if np.subtract(sources1[common_source_positions_quantum],
+                   sources2[common_source_positions_quantum]).all():
         return True
-    return not nb_exists_shared_source(operator1[1:-2], operator2[1:-2])
-
-
-@jit(nopython=nopython, cache=cache, forceobj=not nopython)
-def order_via_commutation(mon: np.ndarray,
-                          notcomm: np.ndarray,
-                          lexorder: np.ndarray,
-                          commuting=False) -> np.ndarray:
-    """Applies commutations between the operators forming a monomial until
-    finding the smallest lexicographic representation.
-
-    Parameters
-    ----------
-    mon : numpy.ndarray
-        Input monomial in 2D array format.
-    notcomm : numpy.ndarray
-        Matrix of commutation relations. Each operator can be identified by an
-        integer `i` which also doubles as its lexicographic rank. Given two
-        operators with ranks `i`, `j`, ``notcomm[i, j]`` is 1 if the operators
-        do not commute, and 0 if they do.
-    lexorder : numpy.ndarray
-        A matrix where each row is an operator, and the `i`-th row stores
-        the operator with lexicographic rank `i`.
-    commuting : bool, optional
-        Whether all the variables in the problem commute or not. By default
-        ``False``.
-
-    Returns
-    -------
-    numpy.ndarray
-        The monomial in canonical form with respect to some commutation
-        relationships.
-    """
-    mon = np.asarray(mon, dtype=uint8_)
-    if len(mon) <= 1:
-        return mon
-    else:
-        if commuting:
-            mon = mon_lexsorted(mon, lexorder)
-            return mon
-        else:
-            lexmon = nb_mon_to_lexrepr(mon, lexorder)
-            mon = nb_lexmon_to_canonical(lexmon, notcomm)
-            mon = lexorder[mon]
-            return mon
-
+    # Case 3: overlapping quantum source type and index, but not all sources match indices
+    if not np.array_equal(sources1[common_source_positions_all],
+                          sources2[common_source_positions_all]):
+        return False
+    # Case 4: All sources of type common to both operators match indices
+    # # Case 4a: different parties
+    if party1 != party2:
+        return True
+    # Case 4b: Same party (check the settings)
+    return operator1[-2] == operator2[-2]
 
+# Node: cache is set to False because of a bug in numba, which affects
+# nb_lexmon_to_canonical which this function uses
 @jit(nopython=nopython, cache=cache, forceobj=not nopython)
-def to_canonical(mon: np.ndarray,
-                 notcomm: np.ndarray,
-                 lexorder: np.ndarray,
-                 commuting=False,
-                 apply_only_commutations=False) -> np.ndarray:
+def to_canonical_1d_internal(lexmon: np.ndarray,
+                             notcomm: np.ndarray,
+                             orthomat: np.ndarray,
+                             commuting=False,
+                             apply_only_commutations=False) -> np.ndarray:
     """Brings a monomial to canonical form with respect to commutations,
     removing square projectors, and identifying orthogonality.
 
     Parameters
     ----------
-    mon : numpy.ndarray
-        Input monomial in 2D array format.
+    lexmon : numpy.ndarray
+        Input monomial in 1D array format.
     notcomm : numpy.ndarray
         Matrix of commutation relations. Each operator can be identified by an
         integer `i` which also doubles as its lexicographic rank. Given two
         operators with ranks `i`, `j`, ``notcomm[i, j]`` is 1 if the operators
         do not commute, and 0 if they do.
-    lexorder : numpy.ndarray
-        A matrix where each row is an operator, and the `i`-th row stores
-        the operator with lexicographic rank `i`.
+    orthomat : numpy.ndarray
+        Matrix of orthogonality relations. Each operator can be identified by an
+        integer `i` which also doubles as its lexicographic rank. Given two
+        operators with ranks `i`, `j`, ``notcomm[i, j]`` is 1 if the operators
+        are orthogonal, and 0 if they do.
     commuting : bool, optional
         Whether all the variables in the problem commute or not. By default
         ``False``.
     apply_only_commutations : bool, optional
         If ``True``, skip the removal of projector squares and the test to see
         if the monomial is equal to zero. By default ``False``.
 
     Returns
     -------
     numpy.ndarray
         The monomial in canonical form with respect to some commutation
         relationships.
     """
-    mon = np.asarray(mon, dtype=uint8_)
-    if mon.shape[0] <= 1:
-        return mon
+    if len(lexmon) <= 1:
+        return lexmon
     else:
-        mon = order_via_commutation(mon, notcomm, lexorder, commuting)
-        if apply_only_commutations:
-            return mon
+        if commuting:
+            newlexmon = np.sort(lexmon)
         else:
-            mon = remove_projector_squares(mon)
-            if mon_is_zero(mon):
-                return np.asarray(0*mon[:1], dtype=uint8_)
-            else:
-                return mon
+            newlexmon = nb_lexmon_to_canonical(lexmon, notcomm)
+    if apply_only_commutations:
+        return newlexmon
+    else:
+        if lexmon_is_zero(newlexmon, orthomat):
+            newlexmon = np.zeros((1,), dtype=int_)
+        return remove_projector_squares(newlexmon)
+
+
+@jit(nopython=nopython, cache=cache, forceobj=not nopython)
+def lexmon_is_zero(lexmon: np.ndarray, orthomat: np.ndarray) -> bool_:
+    if np.array_equal(lexmon, [0]):
+        return True
+    for i in range(1, lexmon.shape[0]):
+        if orthomat[lexmon[i], lexmon[i-1]]:
+            return True
+    return False
```

### Comparing `inflation-1.0.0/inflation/sdp/monomial_classes.py` & `inflation-2.0.0/inflation/lp/monomial_classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,111 @@
 """
-This file contains classes for defining the monomials inside a moment matrix.
+This file contains classes for defining probabilities of events or expectation
+values of monomials in convex programming relaxations of inflation.
 
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
 """
 import numpy as np
 
-from collections import Counter
+from collections import Counter, defaultdict
 from functools import total_ordering
 from numbers import Real
 from typing import Dict, List, Tuple
+from copy import deepcopy
 
-from .fast_npa import mon_is_zero, nb_remove_sandwich
-from .monomial_utils import (compute_marginal,
-                             name_from_atom_names,
-                             symbol_from_atom_name,
-                             symbol_prod)
+from ..sdp.monomial_utils import (compute_marginal,
+                                  name_from_atom_names,
+                                  symbol_from_atom_name,
+                                  symbol_prod)
+from .numbafied import nb_is_do_conditional as is_do_conditional
 
 
 @total_ordering
 class InternalAtomicMonomial(object):
-    __slots__ = ["as_ndarray",
+    __slots__ = ["as_lexmon",
+                 "as_2d_array",
                  "is_one",
                  "is_zero",
+                 "is_do_conditional",
                  "is_knowable",
-                 "is_all_commuting",
-                 "is_physical",
                  "n_operators",
                  "op_length",
                  "rectified_ndarray",
-                 "sdp"
+                 "context",
+                 "name",
+                 "legacy_name",
+                 "is_all_commuting",
+                 "signature",
+                 "symbol"
                  ]
 
-    def __init__(self, inflation_sdp_instance, array2d: np.ndarray):
+    def __init__(self, inflation_lp_instance, as_1d_vec: np.ndarray):
         r"""This class models a moment
         :math:`\langle Op_1 Op_2\dots Op_n\rangle` on the inflated problem,
         which cannot be decomposed into products of other moments. It is used
         as a building block for the ``CompoundMonomial`` class. It is
-        initialized with a 2D array representing a moment and an an instance of
-        ``InflationSDP``, used for methods that depend on the scenario.
-
-        2D Array encoding
-        -----------------
-        A moment :math:`M=\langle Op_1 Op_2\dots Op_n\rangle` can be specified
-        by a 2D array with `n` rows, one for each operator :math:`Op_k`.
-        Row `k` contains a list of integers which encode information about the
-        operator :math:`Opk`.
-         * The first integer is an index in ``{1,...,nr_parties}``, indicating
-           the party, where `nr_parties` is the number of parties in the DAG.
-         * The second-to-last and last integers encode the setting and the
-           outcome of the operator, respectively.
-         * The remaining positions ``i`` indicate on which copy of the source
-           ``i-1`` (-1 because the first index encodes the party) the operator
-           is acting, with value ``0`` representing no support on the
-           ``i-1``-th source.
-
-        For example, the moment
-        :math:`\langle A^{0,2,1}_{x=2,a=3} C^{2,0,1}_{z=4,c=5}\rangle`, where
-        the complete list of parties is ``["A","B","C"]`` corresponds to the
-        following array:
-
-        >>> m = np.array([[1, 0, 2, 1, 2, 3],
-                          [3, 2, 0, 1, 4, 5]])
+        initialized with a 1D array representing a moment and an instance of
+        ``InflationLP``, used for methods that depend on the scenario.
 
-        Given that this moment is knowable and can be associated with a
-        probability, it is given the name ``"pAC(35|24)"``.
 
         Parameters
         ----------
-        inflation_sdp_instance : InflationSDP
-            An instance of the ``InflationSDP`` class. It is used to access
+        inflation_lp_instance : InflationLP
+            An instance of the ``InflationLP`` class. It is used to access
             methods specific to the inflation problem. E.g., when instantiating
-            an internal atomic moment, the ``InflationSDP`` instance is used to
+            an internal atomic moment, the ``InflationLP`` instance is used to
             check if it already contains such moment.
         array2d : numpy.ndarray
             A moment :math:`\langle Op_1Op_2\dots Op_n\rangle` encoded as a 2D
             array.
         """
-        self.sdp        = inflation_sdp_instance
-        self.as_ndarray = np.asarray(array2d, dtype=self.sdp.np_dtype)
-        self.n_operators, self.op_length = self.as_ndarray.shape
-        assert self.op_length == self.sdp._nr_properties, \
-            ("An AtomicMonomial should be a 2-d array where each row is a list"
-             + f" of integers of length {self.sdp._nr_properties}. The first "
-             + "index corresponds to the party, the last one to the outcome, "
-             + "the second-to-last to the setting, and the rest to the "
-             + "inflation copies.")
-        self.is_zero     = mon_is_zero(self.as_ndarray)
+        self.context = inflation_lp_instance
+        if as_1d_vec.dtype == bool:
+            # self.as_bool_vec = as_1d_vec
+            self.as_lexmon = np.flatnonzero(as_1d_vec).astype(np.intc)
+        else:
+            self.as_lexmon = np.asarray(as_1d_vec, np.intc)
+            # self.as_bool_vec = inflation_lp_instance.blank_bool_vec.copy()
+            # self.as_bool_vec[self.as_lexmon] = True
+
+        self.as_2d_array = inflation_lp_instance._lexorder[self.as_lexmon]
+        self.n_operators = len(self.as_lexmon)
+        self.op_length = inflation_lp_instance._nr_properties
         self.is_one      = (self.n_operators == 0)
-        self.is_knowable = (self.is_zero
-                            or self.is_one
-                            or self.sdp._atomic_knowable_q(self.as_ndarray))
-        self.is_all_commuting = self.sdp.all_commuting_q(self.as_ndarray)
-        if self.is_all_commuting or self.n_operators <= 1:
-            self.is_physical = True
+        # Hack to account for different meanings of the zero position in the lexorder
+        if inflation_lp_instance.problem_type == "lp":
+            self.is_zero = False
+        elif inflation_lp_instance.problem_type == "sdp":
+            self.is_zero = not np.all(self.as_lexmon)
+        else:
+            raise NotImplementedError("InternalAtomicMonomial requires `lp` or `sdp` parent class.")
+        if self.is_one or self.is_zero:
+            self.is_all_commuting = True
+            self.is_do_conditional = True
+            self.is_knowable = True
         else:
-            self.is_physical = self.sdp.all_commuting_q(
-                nb_remove_sandwich(self.as_ndarray))
+            self.is_all_commuting = inflation_lp_instance.all_commuting_q_1d(self.as_lexmon)
+            self.is_do_conditional = is_do_conditional(self.as_2d_array)
+            if self.is_do_conditional and self.is_all_commuting:
+                self.is_knowable = self.context._atomic_knowable_q(self.as_2d_array)
+            else:
+                self.is_knowable = False
         # Save also array with the original setting, not just the effective one
         if self.is_knowable:
             self.rectified_ndarray = np.asarray(
-                self.sdp.rectify_fake_setting(np.take(self.as_ndarray,
-                                                      [0, -2, -1],
-                                                      axis=1)),
+                inflation_lp_instance.rectify_fake_setting(np.take(self.as_2d_array,
+                                                     [0, -2, -1],
+                                                     axis=1)),
                 dtype=int)
 
+        self.name = self._name
+        self.legacy_name = self._raw_name
+        self.signature = self._signature
+        self.symbol = symbol_from_atom_name(self.name)
+
     def __copy__(self):
         """Make a copy of the Monomial"""
         cls = self.__class__
         result = cls.__new__(cls)
         for attr in self.__slots__:
             try:
                 result.__setattr__(attr, self.__getattribute__(attr))
@@ -134,73 +132,76 @@
         return self.__str__()
 
     def __str__(self):
         """Return the name of the Monomial."""
         return self.name
 
     @property
-    def dagger(self):
-        """Returns the adjoint of the Monomial."""
-        conjugate_ndarray   = self.sdp._conjugate_ndarray(self.as_ndarray)
-        conjugate_signature = self.sdp._from_2dndarray(conjugate_ndarray)
-        if conjugate_signature != self.signature:
-            dagger = self.__copy__()
-            dagger.as_ndarray = conjugate_ndarray
-            return dagger
-        else:
-            return self
+    def as_legacy_lexmon(self):
+        return self.as_lexmon
 
     @property
-    def is_hermitian(self):
-        """Whether the atomic monomial is equivalent to its conjugate
-         under inflation symmetries and commutation.
-        """
-        return self == self.dagger
+    def _name(self):
+        if self.is_one:
+            return "1"
+        elif self.is_zero:
+            return "0"
+        if self.is_do_conditional:
+            uncleaned_ops = self.context.InflationProblem._lexrepr_to_dicts[self.as_legacy_lexmon]
+            ambigous_outcome_dict = defaultdict(set)
+            for op in uncleaned_ops.flat:
+                ambigous_outcome_dict[op["Party"]].add(op["Outcome"])
+            parties_with_unambigous_outcomes = [(p, s.pop()) for p, s in ambigous_outcome_dict.items() if len(s)==1]
+            cleaned_ops = [deepcopy(op) for op in uncleaned_ops.flat]
+            for (p, o) in parties_with_unambigous_outcomes:
+                for alt_op in cleaned_ops:
+                    alt_op["Do Values"] = {k: v for k, v in
+                                           alt_op["Do Values"].items()
+                                           if not (k==p and o==v)}
+            list_of_op_names = [self.context.InflationProblem._interpretation_to_name(op, include_copy_indices=False) for op in cleaned_ops]
+        else:
+            list_of_op_names = self.context._lexrepr_to_names[self.as_lexmon]
+        if self.is_all_commuting:
+            return "P[" + " ".join(list_of_op_names) + "]"
+        else:
+            return "<" + " ".join(list_of_op_names) + ">"
 
     @property
-    def name(self):
+    def _raw_name(self):
         """A string representing the monomial. In case of knowable monomials,
         it is of the form ``p(outputs|inputs)``. Otherwise it represents the
         expectation value of the monomial with bracket notation.
         """
         if self.is_one:
             return "1"
         elif self.is_zero:
             return "0"
         elif self.is_knowable:
             # Use notation p(outputs|settings)
             # Convention in numpy monomial format is first party = 1
             party_indices = self.rectified_ndarray[:, 0] - 1
-            parties       = np.take(self.sdp.names, party_indices.tolist())
+            parties       = np.take(self.context.names, party_indices.tolist())
             inputs  = [str(input) for input in self.rectified_ndarray[:, -2]]
             outputs = [str(output) for output in self.rectified_ndarray[:, -1]]
             p_divider = ""
             # We will probably never have more than 1 digit cardinalities,
             # but who knows...
             i_divider = "" if all(len(i) == 1 for i in inputs) else ","
             o_divider = "" if all(len(o) == 1 for o in outputs) else ","
             return ("p" + p_divider.join(parties) +
                     "(" + o_divider.join(outputs) +
                     "|" + i_divider.join(inputs) + ")")
         else:
-            # Use expectation value notation
-            operators = []
-            for op in self.as_ndarray:
-                operators.append("_".join([self.sdp.names[op[0] - 1]]
-                                          + [str(i) for i in op[1:]]))
-            return "<" + " ".join(operators) + ">"
+            return "<" + " ".join(self.context.InflationProblem._lexrepr_to_all_names[
+                self.as_legacy_lexmon, 2]) + ">"
 
     @property
-    def signature(self):
-        return self.sdp._from_2dndarray(self.as_ndarray)
-
-    @property
-    def symbol(self):
-        """Return a sympy Symbol representing the monomial."""
-        return symbol_from_atom_name(self.name)
+    def _signature(self):
+        # return self.as_1d_int_vec.tobytes() #FOR QUANTUM OR NONCOMMUTING CASE!!
+        return (self.n_operators, tuple(self.as_lexmon))
 
     def compute_marginal(self, prob_array: np.ndarray) -> float:
         """Given a probability distribution, compute the numerical value of
         the Monomial.
 
         Parameters
         ----------
@@ -217,101 +218,107 @@
         """
         if self.is_zero:
             return 0.
         else:
             return compute_marginal(prob_array, self.rectified_ndarray)
 
 
-class CompoundMonomial(object):
+class CompoundMoment(object):
     __slots__ = ["as_counter",
                  "factors",
                  "idx",
-                 "is_all_commuting",
                  "is_atomic",
+                 "is_do_conditional",
                  "is_knowable",
-                 "is_physical",
                  "is_one",
                  "is_zero",
                  "knowability_status",
                  "knowable_factors",
-                 "mask_matrix",
                  "n_factors",
                  "n_knowable_factors",
                  "n_operators",
                  "n_unknowable_factors",
                  "name",
+                 "legacy_name",
                  "signature",
-                 "symbol",
-                 "unknowable_factors"
+                 "unknowable_factors",
+                 "as_lexmon",
+                 "internal_type",
+                 "symbol"
                  ]
 
     def __init__(self, monomials: Tuple[InternalAtomicMonomial]):
         r"""This class models moments :math:`\langle Op_1 Op_2\dots Op_n\rangle
         =\langle Op_i\dots\rangle\langle Op_{i'}\dots\rangle` on the inflated
         problem that are products of other moments. It is built from a tuple of
         instances of the ``InternalAtomicMonomial`` class.
 
-        At intialisation, a moment is classified into knowable, semi-knowable
+        At initialisation, a moment is classified into knowable, semi-knowable
         or unknowable based on the knowability of each of the atomic moments
         (which in turn is determined through methods of the
         ``InternalAtomicMonomial`` class). This class also computes names for
         the moment, provides the ability to compare (in)equivalence, and to
         assign numerical values to a moment given a probability distribution.
 
         Parameters
         ----------
         monomials : tuple of InternalAtomicMonomial
             The atomic moments that make up the compound moment.
         """
-        default_factors    = tuple(sorted(monomials))
-        conjugate_factors  = tuple(sorted(factor.dagger
-                                          for factor in monomials))
-        self.factors       = min(default_factors, conjugate_factors)
+        self.factors       = tuple(sorted(monomials))
         self.n_factors     = len(self.factors)
         self.n_operators   = sum(factor.n_operators for factor in self.factors)
         self.is_atomic     = (self.n_factors <= 1)
+        self.is_do_conditional = all(factor.is_do_conditional for factor in self.factors)
         self.is_knowable   = all(factor.is_knowable for factor in self.factors)
-        self.is_all_commuting = all(factor.is_all_commuting
-                                    for factor in self.factors)
+        if self.n_factors == 0:
+            self.as_lexmon = np.empty(0, dtype=np.intc)
+        else:
+            self.as_lexmon     = np.hstack([factor.as_lexmon for factor in self.factors])
+
         knowable_factors   = []
         unknowable_factors = []
-        for factor in self.factors:
+        self.as_counter = Counter(self.factors)
+        for factor, power in self.as_counter.items():
             if factor.is_knowable:
-                knowable_factors.append(factor)
+                knowable_factors.extend([factor] * power)
             else:
-                unknowable_factors.append(factor)
+                unknowable_factors.extend([factor] * power)
         self.knowable_factors     = tuple(knowable_factors)
         self.unknowable_factors   = tuple(unknowable_factors)
         self.n_knowable_factors   = len(self.knowable_factors)
         self.n_unknowable_factors = len(self.unknowable_factors)
         if self.n_unknowable_factors == 0:
             self.knowability_status = "Knowable"
         elif self.n_unknowable_factors == self.n_factors:
             self.knowability_status = "Unknowable"
         else:
             self.knowability_status = "Semi"
-        self.is_zero = any(factor.is_zero for factor in self.factors)
         self.is_one  = (all(factor.is_one for factor in self.factors)
                         or (self.n_factors == 0))
-        self.is_physical = all(factor.is_physical for factor in self.factors)
-        self.as_counter  = Counter(self.factors)
-        self.name        = name_from_atom_names(self._names_of_factors)
-        self.symbol      = symbol_prod(self._symbols_of_factors)
-        self.signature   = tuple(sorted(self.factors))
+        self.is_zero = any(factor.is_zero for factor in self.factors)
+
+        self.name        = name_from_atom_names([factor.name
+                                                 for factor in self.factors])
+        self.legacy_name = name_from_atom_names([factor.legacy_name
+                                                 for factor in self.factors])
+        self.symbol      = symbol_prod([factor.symbol
+                                        for factor in self.factors])
+        self.signature   = self.factors
+        self.internal_type = InternalAtomicMonomial
 
     def __eq__(self, other):
         """Whether the Monomial is equal to the ``other`` Monomial."""
         if isinstance(other, self.__class__):
             return self.as_counter == other.as_counter
-        elif isinstance(other, InternalAtomicMonomial):
+        elif isinstance(other, self.internal_type):
             return (self.n_factors == 1) and other.__eq__(self.factors[0])
         else:
-            assert isinstance(other, self.__class__), \
-                (f"Expected object of class {self.__class__}, received {other}"
-                 + f" of class {type(other)}{list(map(type, other))}.")
+            raise Exception(f"Expected object of class {self.__class__}, received {other}"
+                 + f" of class {type(other)}.")
             return False
 
     def __hash__(self):
         """Return the hash of the Monomial."""
         return hash(self.signature)
 
     def __len__(self):
@@ -322,24 +329,14 @@
         """Return the name of the Monomial."""
         return self.__str__()
 
     def __str__(self):
         """Return the name of the Monomial."""
         return self.name
 
-    @property
-    def _names_of_factors(self):
-        """Return the names of each of the factors in the Monomial."""
-        return [factor.name for factor in self.factors]
-
-    @property
-    def _symbols_of_factors(self):
-        """Generate a sympy Symbol per factor in the Monomial."""
-        return [factor.symbol for factor in self.factors]
-
     def attach_idx(self, idx: int):
         """Assign an index to the Monomial. This is used when generating the
         monomials in a scenario, and identifying them with integers."""
         if idx >= 0:
             self.idx = idx
 
     def compute_marginal(self, prob_array: np.ndarray) -> float:
@@ -398,19 +395,32 @@
         known_value     = 1.
         unknown_counter = Counter()
         for factor, power in self.as_counter.items():
             try:
                 known_value *= (known_monomials[factor] ** power)
             except KeyError:
                 unknown_counter[factor] = power
+        # unknown_factors = sorted(unknown_counter.elements(),
+        #                          key=lambda factor: factor.as_int_vec.tobytes())
         unknown_factors = list(unknown_counter.elements())
         if (len(unknown_factors) == 0):
             known_status = "Known"
         elif ((len(unknown_factors) == self.n_factors)
               or (not use_lpi_constraints)):
             known_status = "Unknown"
         else:
             known_status = "Semi"
             if use_lpi_constraints and isinstance(known_value, Real):
                 if np.isclose(known_value, 0):
                     known_status = "Known"
         return known_value, unknown_factors, known_status
+
+    def __copy__(self):
+        """Make a copy of the CompoundMonomial"""
+        cls = self.__class__
+        result = cls.__new__(cls)
+        for attr in self.__slots__:
+            try:
+                result.__setattr__(attr, self.__getattribute__(attr))
+            except AttributeError:
+                pass
+        return result
```

### Comparing `inflation-1.0.0/inflation/sdp/monomial_utils.py` & `inflation-2.0.0/inflation/sdp/monomial_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This file contains auxiliary functions for the Monomial classes defined in
 monomial_classes.py.
 
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
 """
 import numpy as np
 import sympy
+import re
 
 from collections import Counter
 from typing import List
 
 
 def compute_marginal(prob_array: np.ndarray, atom: np.ndarray) -> float:
     """Given an atomic monomial and a probability distribution ``prob_array``,
@@ -95,15 +96,17 @@
         The corresponding symbol.
     """
     if atomic_name == "1":
         return sympy.S.One
     elif atomic_name == "0":
         return sympy.S.Zero
     else:
-        return sympy.Symbol(atomic_name, commutative=True)
+        new_name = re.sub("_[^=]*=", lambda x:  x.group(0).replace('_','_{').replace('=', '}{=}'), atomic_name)
+        new_name = new_name.replace(' ',',')
+        return sympy.Symbol(new_name, commutative=True)
 
 
 def symbol_prod(atomic_symbols: List[sympy.core.symbol.Symbol]
                 ) -> sympy.core.mul.Mul:
     """Computes the product of a list of sympy symbols.
 
     Parameters
```

### Comparing `inflation-1.0.0/inflation/sdp/optimization_utils.py` & `inflation-2.0.0/inflation/optimization_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 """
 This file contains helper functions to optimize (functions of) symbolic
-variables under the constraint that the InflationSDP instance they implicitly
-define must be feasible. Useful for exploring the set of parametrically-defined
-distribution for which quantum inflation (at specific hierarchy levels) is
+variables under the constraint that the InflationLP or InflationSDP instance
+they implicitly define must be feasible. Useful for exploring the set of
+parametrically-defined distribution for which quantum inflation (at specific
+hierarchy levels) is
+
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
 """
 import numpy as np
 import sympy as sp
 
 from numbers import Real
 from scipy.optimize import bisect, minimize, Bounds
 from sympy.utilities.lambdify import lambdify
-from typing import Callable, Dict, Tuple, Union
+from typing import Dict, Tuple, Union
 
-from inflation import InflationSDP
+from inflation import InflationLP, InflationSDP
 from inflation.sdp.quantum_tools import make_numerical
-from inflation.sdp.monomial_classes import CompoundMonomial
+from inflation.sdp.monomial_classes import CompoundMomentSDP
 
 
-def max_within_feasible(sdp: InflationSDP,
-                        symbolic_values: Dict[CompoundMonomial, Callable],
+def max_within_feasible(program: Union[InflationLP, InflationSDP],
+                        symbolic_values: Dict[CompoundMomentSDP,
+                                              sp.core.expr.Expr],
                         method: str,
                         return_last_certificate=False,
                         **kwargs) -> Union[float,
-                                           Tuple[float, sp.core.add.Add]]:
+                                           Tuple[float, dict]]:
     """Maximize a single real variable within the set of feasible moment
     matrices determined by an ``InflationSDP``. The dependence of the moment
     matrices in the variable is specified by an assignment of monomials in the
     moment matrix to arbitrary expressions of the variable. This is useful for
     finding (bounds for) critical visibilities of distributions beyond which
     they are impossible to generate in a given quantum causal scenario.
 
     Parameters
     ----------
-    sdp : InflationSDP
-        The SDP problem under which to carry the optimization.
-    symbolic_values : Dict[CompoundMonomial, Callable]
+    program : Union[InflationLP, InflationSDP]
+        The problem under which to carry the optimization.
+    symbolic_values : Dict[CompoundMomentSDP, Callable]
         The correspondence between monomials in the SDP problem and symbolic
         expressions depending on the variable to be optimized.
     method : str
         Technique used for optimization. Currently supported: ``"bisection"``
         for bisection algorithms, and ``"dual"`` for exploitation of the
         certificates of infeasibility (typically much fewer iteration steps).
     return_last_certificate : bool, optional
@@ -53,188 +56,217 @@
         options to be passed to the optimization routines (bounds, precision,
         tolerance, ...).
 
     Returns
     -------
     float
         The maximum value that the parameter can take under the set of
-        positive-semidefinite moment matrices. This is the output when
-        ``return_last_certificate=False``.
-    Tuple[float, sympy.core.add.Add]
+        distributions compatible with an inflation (for LPs) or under the set of
+        positive-semidefinite moment matrices (for SDPs). This is the output
+        when ``return_last_certificate=False``.
+    Tuple[float, dict]
         The maximum value that the parameter can take under the set of
-        positive-semidefinite moment matrices, and a corresponding separating
-        surface (a root of the function corresponds to the critical feasible
-        value of the parameter reported). This is the output when
+        distributions compatible with an inflation (for LPs) or under the set of
+        positive-semidefinite moment matrices (for SDPs), and a corresponding
+        separating surface (a root of the function corresponds to the critical
+        feasible value of the parameter reported). This is the output when
         ``return_last_certificate=True``.
     """
     assert method in ["bisection", "dual"], \
         "Unknown optimization method. Please use \"bisection\" or \"dual\"."
     variables = set()
     for expr in symbolic_values.values():
         if not isinstance(expr, Real):
-            variables.update(expr.free_symbols)
+            variables.update(expr.atoms(sp.Symbol))
+    assert len(variables) != 0, \
+        "No variable to be optimized detected"
     assert len(variables) == 1, \
         "Only optimization of a single variable is supported"
     param = variables.pop()
     kwargs.update({"return_last_certificate": return_last_certificate})
 
     if method == "bisection":
-        return _maximize_via_bisect(sdp, symbolic_values, param, **kwargs)
+        return _maximize_via_bisect(program, symbolic_values, param, **kwargs)
     elif method == "dual":
-        return _maximize_via_dual(sdp, symbolic_values, param, **kwargs)
+        return _maximize_via_dual(program, symbolic_values, param, **kwargs)
 
 
 ###############################################################################
 # OPTIMIZATION METHODS                                                        #
 ###############################################################################
-def _maximize_via_bisect(sdp: InflationSDP,
-                         symbolic_values: Dict[CompoundMonomial, Callable],
+def _maximize_via_bisect(program: Union[InflationLP, InflationSDP],
+                         symbolic_values: Dict[CompoundMomentSDP,
+                                               sp.core.expr.Expr],
                          param: sp.core.symbol.Symbol,
                          **kwargs) -> Union[float,
                                             Tuple[float, sp.core.add.Add]]:
     """Implement the maximization of a variable within the feasible set of
-    moment matrices using SciPy's bisection algorithm.
+    distributions using SciPy's bisection algorithm.
 
 
     Parameters
     ----------
-    sdp : InflationSDP
-        The SDP problem under which to carry the optimization.
-    symbolic_values : Dict[CompoundMonomial, Callable]
-        The correspondence between monomials in the SDP problem and symbolic
+    program : Union[InflationLP, InflationSDP]
+        The problem under which to carry the optimization.
+    symbolic_values : Dict[CompoundMomentSDP, Callable]
+        The correspondence between monomials in the problem and symbolic
         expressions depending on the variable to be optimized.
     param : sympy.core.symbol.Symbol
         The variable to be optimized.
 
     **kwargs
-        Additional arguments to ``sdp.set_values()`` and
+        Additional arguments to ``program.set_values()`` and
         ``scipy.optimize.bisect()``.
 
     Returns
     -------
     float
         The maximum value that the parameter can take under the set of
-        positive-semidefinite moment matrices. This is the output when
-        ``return_last_certificate=False``.
+        distributions compatible with an inflation (for LPs) or under the set of
+        positive-semidefinite moment matrices (for SDPs). This is the output
+        when ``return_last_certificate=False``.
     Tuple[float, sympy.core.add.Add]
         The maximum value that the parameter can take under the set of
-        positive-semidefinite moment matrices, and a corresponding separating
-        surface (a root of the function corresponds to the critical feasible
-        value of the parameter reported). This is the output when
+        distributions compatible with an inflation (for LPs) or under the set of
+        positive-semidefinite moment matrices (for SDPs), and a corresponding
+        separating surface (a root of the function corresponds to the critical
+        feasible value of the parameter reported). This is the output when
         ``return_last_certificate=True``.
     """
     bounds         = kwargs.get("bounds", np.array([0.0, 1.0]))
     only_specified = kwargs.get("only_specified_values", False)
     return_last    = kwargs.get("return_last_certificate", False)
+    precision      = kwargs.get("precision", 1e-4)
     use_lpi        = kwargs.get("use_lpi_constraints", False)
     verbose        = kwargs.get("verbose", False)
+    solve_dual     = kwargs.get("solve_dual", True)
+    solverparameters = kwargs.get("solverparameters", None)
     # Prepare bisect kwargs
     bisect_kwargs = {}
     for kwarg in ["args", "rtol", "maxiter", "full_output", "disp"]:
         try:
             bisect_kwargs[kwarg] = kwargs[kwarg]
-        except Exception:
+        except KeyError:
             pass
     try:
         bisect_kwargs["xtol"] = kwargs["xtol"]
-    except Exception:
-        bisect_kwargs["xtol"] = kwargs.get("precision", 1e-4)
+    except KeyError:
+        bisect_kwargs["xtol"] = precision
+
+    discovered_certificates = []
 
     def f(value):
         evaluated_values = make_numerical(symbolic_values, {param: value})
-        sdp.set_values(evaluated_values, use_lpi, only_specified)
-        sdp.solve(feas_as_optim=True)
+        program.set_values(evaluated_values,
+                       use_lpi_constraints=use_lpi,
+                       only_specified_values=only_specified)
+        program.solve(feas_as_optim=True,
+                  solve_dual=solve_dual,
+                  solverparameters=solverparameters)
         if verbose:
             print(f"Parameter = {value:<6.4g}   " +
-                  f"Maximum smallest eigenvalue: {sdp.objective_value:10.4g}")
-        return sdp.objective_value
-    crit_param = bisect(f, bounds[0], bounds[1], **bisect_kwargs)
+                  f"Maximum smallest eigenvalue: {program.objective_value:10.4g}")
+        discovered_certificate = program.certificate_as_dict()
+        if len(discovered_certificate):  # Checking if certificate has any nonzero coefficients
+            discovered_certificates.append((value, discovered_certificate))
+        return program.objective_value+precision/2048
+    crit_param = bisect(f, bounds[0], bounds[1], **bisect_kwargs, full_output=False)
     if return_last:
-        return crit_param, sdp.certificate_as_probs()
+        return crit_param, discovered_certificates[-1][-1]
     else:
         return crit_param
 
 
-def _maximize_via_dual(sdp: InflationSDP,
-                       symbolic_values: Dict[CompoundMonomial, Callable],
+def _maximize_via_dual(program: Union[InflationLP, InflationSDP],
+                       symbolic_values: Dict[CompoundMomentSDP,
+                                             sp.core.expr.Expr],
                        param: sp.core.symbol.Symbol,
                        **kwargs) -> Union[float,
                                           Tuple[float, sp.core.add.Add]]:
     """Implement the maximization of a variable within the feasible set of
-    moment matrices exploiting the certificates of infeasibility. For a given
+    distributions exploiting the certificates of infeasibility. For a given
     value of the parameter, a separating surface that leaves the set of
-    positive-semidefinite moment matrices in its positive side is extracted.
-    The next value of the parameter used is that which evaluates the surface to
-    0.
+    fesible distributions in its positive side is extracted. The next value of
+    the parameter used is that which evaluates the surface to 0.
 
     Parameters
     ----------
-    sdp : InflationSDP
-        The SDP problem under which to carry the optimization.
-    symbolic_values : Dict[CompoundMonomial, Callable]
-        The correspondence between monomials in the SDP problem and symbolic
+    program : Union[InflationLP, InflationSDP]
+        The problem under which to carry the optimization.
+    symbolic_values : Dict[CompoundMomentSDP, Callable]
+        The correspondence between monomials in the problem and symbolic
         expressions depending on the variable to be optimized.
     param : sympy.core.symbol.Symbol
         The variable to be optimized.
 
     **kwargs
-        Additional arguments to ``sdp.set_values()``, bounds of the
+        Additional arguments to ``program.set_values()``, bounds of the
         optimization interval, precision of the optimization, verbosity and
         whether returning the last computed separating surface.
 
     Returns
     -------
     float
         The maximum value that the parameter can take under the set of
-        positive-semidefinite moment matrices. This is the output when
-        ``return_last_certificate=False``.
-    Tuple[float, sympy.core.add.Add]
+        distributions compatible with an inflation (for LPs) or under the set of
+        positive-semidefinite moment matrices (for SDPs). This is the output
+        when ``return_last_certificate=False``.
+    Tuple[float, dict]
         The maximum value that the parameter can take under the set of
-        positive-semidefinite moment matrices, and a corresponding separating
-        surface (a root of the function corresponds to the critical feasible
-        value of the parameter reported). This is the output when
+        distributions compatible with an inflation (for LPs) or under the set of
+        positive-semidefinite moment matrices (for SDPs), and a corresponding
+        separating surface (a root of the function corresponds to the critical
+        feasible value of the parameter reported). This is the output when
         ``return_last_certificate=True``.
     """
     bounds         = kwargs.get("bounds", np.array([0.0, 1.0]))
     only_specified = kwargs.get("only_specified_values", False)
     precision      = kwargs.get("precision", 1e-4)
     return_last    = kwargs.get("return_last_certificate", False)
     use_lpi        = kwargs.get("use_lpi_constraints", False)
     verbose        = kwargs.get("verbose", False)
+    solve_dual     = kwargs.get("solve_dual", True)
+    solverparameters = kwargs.get("solverparameters", None)
 
     symbol_names = {str(key): val for key, val in symbolic_values.items()}
     func_to_minimize = lambdify([param], -param, modules='numpy', cse=True)
     sp_bounds = Bounds(lb=bounds[0], ub=bounds[1])
     x0 = np.array([bounds[0]])
-    new_ub = bounds[1]
+    new_ub = bounds[1]-precision
     old_ub = np.inf
     discovered_certificates = []
     # Get a certificate for a value, find the critical value for it (that which
     # makes the certificate zero), and repeat with this new value
-    while new_ub < old_ub - precision:
+    while new_ub+precision < old_ub:
         old_ub = new_ub
-        evaluated_values = make_numerical(symbolic_values, {param: new_ub})
-        sdp.set_values(evaluated_values, use_lpi, only_specified)
-        sdp.solve(feas_as_optim=True)
-        discovered_certificates.append(sdp.certificate_as_probs())
+        evaluated_values = make_numerical(symbolic_values,
+                                          {param: new_ub+precision})
+        program.set_values(evaluated_values,
+                           use_lpi_constraints=use_lpi,
+                           only_specified_values=only_specified)
+        program.solve(feas_as_optim=True,
+                      solve_dual=solve_dual,
+                      solverparameters=solverparameters)
+
         # The feasible region is where the certificate is positive
         nonneg_expr = sum(symbol_names[var] * coeff
                           for var, coeff in
-                          sdp.solution_object["dual_certificate"].items())
+                          program.solution_object["dual_certificate"].items())
         nonneg_func = lambdify([param],
                                nonneg_expr,
                                modules="numpy",
                                cse=True)
         constraints = {"type": "ineq", "fun": nonneg_func}
         solution = minimize(func_to_minimize, x0,
                             method='SLSQP',
                             bounds=sp_bounds,
                             constraints=constraints,
                             options={'disp': False})
         new_ub = solution['x'][0]
+        discovered_certificates.append((new_ub , program.certificate_as_dict()))
         if verbose:
-            print("Current critical value:", new_ub)
-    crit_param = min(new_ub, old_ub)
+            print(f"Current critical value: {new_ub} (seeded by {old_ub+precision})")
+    crit_param = max(new_ub, old_ub)
     if return_last:
-        return crit_param, discovered_certificates[-1]
+        return crit_param, discovered_certificates[-1][-1]
     else:
         return crit_param
```

### Comparing `inflation-1.0.0/inflation/sdp/quantum_tools.py` & `inflation-2.0.0/inflation/sdp/quantum_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 This file contains helper functions to manipulate monomials and generate moment
 matrices.
+
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
 """
 import numpy as np
 import sympy
 
-from copy import deepcopy
 from itertools import permutations, product, combinations_with_replacement
 from tqdm import tqdm
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Tuple, Union
 
 from .fast_npa import (apply_source_perm,
                        dot_mon,
-                       mon_is_zero,
                        mon_lexsorted,
-                       to_canonical,
+                       to_canonical_1d_internal,
                        to_name)
+from ..utils import format_permutations
 
 
 ###############################################################################
 # FUNCTIONS FOR MONOMIALS                                                     #
 ###############################################################################
+
 def flatten_symbolic_powers(monomial: sympy.core.symbol.Symbol
                             ) -> List[sympy.core.symbol.Symbol]:
     """If we have powers of a monomial, such as A**3, return a list with
     the factors, [A, A, A].
 
     Parameters
     ----------
@@ -37,19 +38,15 @@
     List[sympy.core.symbol.Symbol]
         List of all the symbolic factors, with the powers expanded.
     """
     factors          = monomial.as_ordered_factors()
     factors_expanded = []
     for factor in factors:
         base, exp = factor.as_base_exp()
-        if exp == 1:
-            factors_expanded.append(base)
-        elif exp > 1:
-            for _ in range(exp):
-                factors_expanded.append(base)
+        factors_expanded.extend([base] * exp)
     factors = factors_expanded
     return factors
 
 
 def reduce_inflation_indices(monomial: np.ndarray) -> np.ndarray:
     """Reduce the inflation indices of a monomial as much as possible. This
     procedure might not give the canonical form directly due to commutations.
@@ -72,23 +69,20 @@
                                                 new_mon)).T
     for source in range(nr_sources):
         copies_used = new_mon_padded_transposed[1 + source]
         _, unique_positions = np.unique(copies_used, return_inverse=True)
         new_mon_padded_transposed[1 + source] = unique_positions
     return new_mon_padded_transposed.T[1:]
 
-
-###############################################################################
-# FUNCTIONS FOR MOMENT MATRICES                                               #
-###############################################################################
-def calculate_momentmatrix(cols: List,
-                           notcomm: np.ndarray,
-                           lexorder: np.ndarray,
-                           commuting: bool = False,
-                           verbose: int = 0) -> Tuple[np.ndarray, Dict]:
+def calculate_momentmatrix_1d_internal(cols: List,
+                                       notcomm: np.ndarray,
+                                       orthomat: np.ndarray,
+                                       commuting: bool = False,
+                                       verbose: int = 0
+                                       ) -> Tuple[np.ndarray, Dict]:
     r"""Calculate the moment matrix. The function takes as input the generating
     set :math:`\{M_i\}_i` encoded as a list of monomials. Each monomial is a
     matrix where each row is an operator and the columns specify the operator
     labels/indices. The moment matrix is the inner product between all possible
     pairs of elements from the generating set. The program outputs the moment
     matrix as a 2d array. Entry :math:`(i,j)` of the moment matrix stores the
     index of the monomial that represents the result of the expectation value
@@ -96,21 +90,23 @@
     :math:`\rho` after applying the substitutions. The program returns the
     moment matrix and the dictionary mapping each monomial in string
     representation to its integer representation.
 
     Parameters
     ----------
     cols : List
-        List of numpy.ndarray representing the generating set.
+        List of numpy.ndarray representing the generating set in 1d internal format.
     notcomm : numpy.ndarray
         Matrix of commutation relations, given in the format specified by
-        `inflation.sdp.fast_npa.commutation_matrix`.
-    lexorder : numpy.ndarray
-        Matrix with rows as operators where the index of the row gives
-        the lexicographic order of the operator.
+        `inflation.quantum.fast_npa.commutation_matrix`.
+    orthomat : numpy.ndarray
+        Matrix of orthogonality relations. Each operator can be identified by an
+        integer `i` which also doubles as its lexicographic rank. Given two
+        operators with ranks `i`, `j`, ``notcomm[i, j]`` is 1 if the operators
+        are orthogonal, and 0 if they do.
     commuting : bool, optional
         Whether the variables in the problem commute or not. By default
         ``False``.
     verbose : int, optional
         How much information to print. By default ``0``.
 
     Returns
@@ -121,46 +117,48 @@
         string representation to integer representation.
     """
     nrcols = len(cols)
     canonical_mon_to_idx = dict()
     momentmatrix = np.zeros((nrcols, nrcols), dtype=np.uint32)
     varidx = 1  # We start from 1 because 0 is reserved for 0
     for (i, mon1), (j, mon2) in tqdm(
-                            combinations_with_replacement(enumerate(cols), 2),
-                            disable=not verbose,
-                            desc="Calculating moment matrix",
-                            total=int(nrcols*(nrcols+1)/2),
-                                    ):
-        mon_v1 = to_canonical(dot_mon(mon1, mon2),
-                              notcomm,
-                              lexorder,
-                              commuting=commuting)
-        if not mon_is_zero(mon_v1):
-            if not commuting:
-                mon_v2 = to_canonical(dot_mon(mon2, mon1),
-                                      notcomm,
-                                      lexorder,
-                                      commuting=commuting)
-                mon_hash = min(mon_v1.tobytes(), mon_v2.tobytes())
+            combinations_with_replacement(enumerate(cols), 2),
+            disable=not verbose,
+            desc="Calculating moment matrix",
+            total=int(nrcols * (nrcols + 1) / 2),
+    ):
+        mon_v1 = to_canonical_1d_internal(dot_mon(mon1, mon2),
+                                          notcomm,
+                                          orthomat,
+                                          commuting=commuting,
+                                          apply_only_commutations=False)
+        if np.all(mon_v1):  # a zero indicates equal to zero scalar
+            if len(mon_v1) > 1 and (not commuting):
+                mon_v2 = to_canonical_1d_internal(np.flipud(mon_v1),
+                                                  notcomm,
+                                                  orthomat,
+                                                  commuting=commuting,
+                                                  apply_only_commutations=True)
+                mon_hash = min(tuple(mon_v1), tuple(mon_v2))
             else:
-                mon_hash = mon_v1.tobytes()
+                mon_hash = tuple(mon_v1)
             try:
                 known_varidx = canonical_mon_to_idx[mon_hash]
                 momentmatrix[i, j] = known_varidx
                 momentmatrix[j, i] = known_varidx
             except KeyError:
                 canonical_mon_to_idx[mon_hash] = varidx
                 momentmatrix[i, j] = varidx
                 momentmatrix[j, i] = varidx
                 varidx += 1
     return momentmatrix, canonical_mon_to_idx
 
 
 def to_symbol(mon: np.ndarray,
-              names: np.ndarray,
+              names: Union[np.ndarray, List[str]],
               commutative=False) -> sympy.core.symbol.Symbol:
     """Convert a monomial to a SymPy expression.
 
     Parameters
     ----------
     mon : numpy.ndarray
         Monomial written as a 2D array.
@@ -181,23 +179,24 @@
     A_1_0_1*B_1_1_2
     """
     if isinstance(mon, np.ndarray):
         if mon.shape[0] == 0:
             return sympy.S.One
         res = sympy.S.One
         for mon in mon:
-            name = '_'.join([names[mon[0]-1]] +
+            name = '_'.join([names[mon[0] - 1]] +
                             [str(i) for i in mon.tolist()][1:])
             res *= sympy.Symbol(name, commutative=commutative)
         return res
 
 
 ###############################################################################
 # FUNCTIONS FOR INFLATIONS                                                    #
 ###############################################################################
+
 def apply_inflation_symmetries(momentmatrix: np.ndarray,
                                inflation_symmetries: np.ndarray,
                                verbose: bool = False
                                ) -> Tuple[np.ndarray,
                                           Dict[int, int],
                                           np.ndarray]:
     """Applies the inflation symmetries, in the form of permutations of the
@@ -271,14 +270,15 @@
         if old_indices.min() != 0:
             new_indices += prior_min_value
         orbits = dict(zip(old_indices, new_indices[inversion_tracker]))
         sym_mm = new_indices[inverse]
         return sym_mm, orbits, repr_values
 
 
+# TODO @Cristian add this to InflationSDP
 def commutation_relations(infSDP):
     """Return a user-friendly representation of the commutation relations.
 
     Parameters
     ----------
     infSDP : inflation.InflationSDP
         The SDP object for which the commutation relations are to be extracted.
@@ -380,15 +380,15 @@
     """
     eqs = []
     for k, operator in enumerate(moment):
         party = operator[0] - 1
         # Operators that are involved in normalization equalities are
         # those which are unpacked in non-network scenarios
         if (not skip_party[party]
-            and operator[-1] == outcome_cardinalities[party] - 2):
+                and operator[-1] == outcome_cardinalities[party] - 2):
             operator_2d = np.expand_dims(operator, axis=0)
             prefix = moment[:k]
             suffix = moment[(k + 1):]
             moments = [moment]
             true_cardinality = outcome_cardinalities[party] - 1
             for outcome in range(true_cardinality - 1):
                 variant_operator        = operator_2d.copy()
@@ -399,35 +399,14 @@
                 moments.append(variant_mon)
             if len(moments) == true_cardinality:
                 normalization_mon = np.vstack((prefix, suffix))
                 eqs.append((normalization_mon, moments))
     return eqs
 
 
-def format_permutations(array: np.ndarray) -> np.ndarray:
-    """Permutations of inflation indices must leave the integers 0,
-    corresponding to sources not being measured by the operator, invariant.
-    In order to achieve this, this function shifts a permutation of sources
-    by 1 and prepends it with the integer 0.
-
-    Parameters
-    ----------
-    array : numpy.ndarray
-        2-d array where each row is a permutations.
-
-    Returns
-    -------
-    numpy.ndarray
-        The processed list of permutations.
-    """
-    source_permutation = np.asarray(array) + 1
-    padding = np.zeros((len(source_permutation), 1), dtype=int)
-    return np.hstack((padding, source_permutation))
-
-
 def generate_operators(outs_per_input: List[int],
                        name: str
                        ) -> List[List[List[sympy.core.symbol.Symbol]]]:
     """Generates the list of ``sympy.core.symbol.Symbol`` variables
     representing the measurements for a given party. The variables are treated
     as non-commuting. This code is adapted from `ncpol2sdpa
     <https://github.com/peterwittek/ncpol2sdpa/>`_.
@@ -473,140 +452,17 @@
     """
     lexorder = {}
     for i, op in enumerate(infSDP._lexorder):
         lexorder[sympy.Symbol(to_name([op], infSDP.names),
                               commutative=False)] = i
     return lexorder
 
-
-def party_physical_monomials(hypergraph: np.ndarray,
-                             inflevels: np.ndarray,
-                             party: int,
-                             max_monomial_length: int,
-                             settings_per_party: Tuple[int],
-                             outputs_per_party: Tuple[int],
-                             lexorder: np.ndarray
-                             ) -> List[np.ndarray]:
-    """Generate all possible non-negative monomials for a given party composed
-    of at most ``max_monomial_length`` operators.
-
-    Parameters
-    ----------
-    hypergraph : numpy.ndarray
-         Hypergraph of the scenario.
-    inflevels : np.ndarray
-        The number of copies of each source in the inflated scenario.
-    party : int
-        Party index. NOTE: starting from 0
-    max_monomial_length : int
-        The maximum number of operators in the monomial.
-    settings_per_party : List[int]
-        List containing the cardinality of the input/measurement setting
-        of each party.
-    outputs_per_party : List[int]
-        List containing the cardinality of the output/measurement outcome
-        of each party.
-    lexorder : numpy.ndarray
-        A matrix storing the lexicographic order of operators. If an operator
-        has lexicographic rank `i`, then it is placed at the ``i``-th row of
-        lexorder.
-
-    Returns
-    -------
-    List[numpy.ndarray]
-        An array containing all possible positive monomials of the given
-        length.
-    """
-
-    hypergraph = np.asarray(hypergraph)
-    nr_sources = hypergraph.shape[0]
-
-    relevant_sources = np.flatnonzero(hypergraph[:, party])
-    relevant_inflevels = inflevels[relevant_sources]
-
-    assert max_monomial_length <= min(relevant_inflevels), \
-        ("You cannot have a longer list of commuting operators" +
-         " than the minimum inflation level of said part.")
-
-    # The strategy is building an initial non-negative monomial and apply all
-    # inflation symmetries
-    initial_monomial = np.zeros(
-        (max_monomial_length, 1 + nr_sources + 2), dtype=np.uint16)
-    for mon_idx in range(max_monomial_length):
-        initial_monomial[mon_idx, 0]    = 1 + party
-        initial_monomial[mon_idx, 1:-2] = hypergraph[:, party] * (1 + mon_idx)
-
-    inflation_equivalents = {initial_monomial.tobytes(): initial_monomial}
-
-    all_permutations_per_relevant_source = [
-        format_permutations(list(permutations(range(inflevel))))
-        for inflevel in relevant_inflevels.flat]
-    for permutation in product(*all_permutations_per_relevant_source):
-        permuted = initial_monomial.copy()
-        for perm_idx, source in enumerate(relevant_sources.flat):
-            permuted = mon_lexsorted(apply_source_perm(permuted,
-                                                       source,
-                                                       permutation[perm_idx]),
-                                     lexorder)
-        inflation_equivalents[permuted.tobytes()] = permuted
-    inflation_equivalents = list(inflation_equivalents.values())
-
-    new_monomials = []
-    # Insert all combinations of inputs and outputs
-    for input_slice in product(*[range(settings_per_party[party])
-                                 for _ in range(max_monomial_length)]):
-        for output_slice in product(*[range(outputs_per_party[party] - 1)
-                                      for _ in range(max_monomial_length)]):
-            for new_mon_idx in range(len(inflation_equivalents)):
-                new_monomial = deepcopy(inflation_equivalents[new_mon_idx])
-                for mon_idx in range(max_monomial_length):
-                    new_monomial[mon_idx, -2] = input_slice[mon_idx]
-                    new_monomial[mon_idx, -1] = output_slice[mon_idx]
-                new_monomials.append(new_monomial)
-    return new_monomials
-
-
 ###############################################################################
 # OTHER FUNCTIONS                                                             #
 ###############################################################################
-def clean_coefficients(cert: Dict[str, float],
-                       chop_tol: float = 1e-10,
-                       round_decimals: int = 3) -> Dict:
-    """Clean the list of coefficients in a certificate.
-
-    Parameters
-    ----------
-    cert : Dict[str, float]
-      A dictionary containing as keys the monomials associated to the elements
-      of the certificate and as values the corresponding coefficients.
-    chop_tol : float, optional
-      Coefficients in the dual certificate smaller in absolute value are
-      set to zero. Defaults to ``1e-10``.
-    round_decimals : int, optional
-      Coefficients that are not set to zero are rounded to the number
-      of decimals specified. Defaults to ``3``.
-
-    Returns
-    -------
-    np.ndarray
-      The cleaned-up coefficients.
-    """
-    processed_cert = deepcopy(cert)
-    vars = processed_cert.keys()
-    coeffs = np.asarray(list(processed_cert.values()))
-    # Take the biggest one and make it 1
-    normalising_factor = np.max(np.abs(coeffs[np.abs(coeffs) > chop_tol]))
-    coeffs /= normalising_factor
-    # Set to zero very small coefficients
-    coeffs[np.abs(coeffs) <= chop_tol] = 0
-    # Round
-    coeffs = np.round(coeffs, decimals=round_decimals)
-    return dict(zip(vars, coeffs.flat))
-
-
 def make_numerical(symbolic_expressions: Dict[Any, sympy.core.expr.Expr],
                    symbols_to_values: Dict[sympy.core.symbol.Symbol, float]
                    ) -> Dict[Any, float]:
     """Replace the symbols in the values of a dictionary by the corresponding
     numerical values.
     Parameters
     ----------
```

### Comparing `inflation-1.0.0/inflation/sdp/sdp_utils.py` & `inflation-2.0.0/inflation/sdp/sdp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 This file contains the functions to send the problems to SDP solvers.
+
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe and Alejandro Pozas-Kerstjens
 """
 from __future__ import annotations
 import numpy as np
 
 from copy import deepcopy
 from gc import collect
@@ -15,14 +16,15 @@
 def solveSDP_MosekFUSION(mask_matrices: Dict = None,
                          objective: Dict = None,
                          known_vars: Dict = None,
                          semiknown_vars: Dict = None,
                          inequalities: List[Dict] = None,
                          equalities: List[Dict] = None,
                          solve_dual: bool = True,
+                         default_non_negative: bool = False,
                          feas_as_optim: bool = False,
                          verbose: int = 0,
                          solverparameters: Dict = {},
                          process_constraints: bool = True
                          ) -> Dict[str, Any]:
     r"""Internal function to solve the SDP with the `MOSEK Fusion API
     <https://docs.mosek.com/latest/pythonfusion/index.html>`_.
@@ -111,14 +113,17 @@
     inequalities : list, optional
         List of inequalities encoded as dictionaries of coefficients.
     equalities : list, optional
         List of equalities encoded as dictionaries of coefficients.
     solve_dual : bool, optional
         Whether to solve the dual (True) or primal (False) formulation. By
         default ``True``.
+    default_non_negative: bool, optional
+        Whether to set default primal variables as non-negative (True) or not
+        (False). By default, ``False``.
     feas_as_optim : bool, optional
         Whether to treat feasibility problems, where the objective is,
         constant, as an optimisation problem. By default ``False``.
     verbose : int, optional
         How much information to display to the user. By default ``0``.
     solverparameters : dict, optional
         Dictionary of parameters to pass to the MOSEK solver, see `MOSEK's
@@ -182,19 +187,14 @@
         lam = "lambda"
         while lam in variables:
             lam += "_"
         variables.add(lam)
         Fi[lam] = -1 * eye(mat_dim).tolil()
         var_objective = {lam: 1}
 
-    # Calculate c0, the constant part of the var_objective.
-    c0 = 0. + float(sum([var_objective[x] * known_vars[x]
-                         for x in set(var_objective).intersection(known_vars)])
-                    )
-
     # Calculate F0, the constant part of the matrix variable.
     if mask_matrices:
         F0 = lil_matrix((mat_dim, mat_dim), dtype=float) + \
             sum(known_vars[x] * Fi[x]
                 for x in set(Fi).intersection(known_vars))
 
     if process_constraints:
@@ -222,14 +222,19 @@
 
     else:
         # Just add semiknown constraints as equality constraints.
         for x, (c, x2) in semiknown_vars.items():
             var_equalities.append({x: 1, x2: -c})
             variables.add(x2)
 
+    # Calculate c0, the constant part of the var_objective.
+    c0 = 0. + float(sum([var_objective[x] * known_vars[x]
+                         for x in set(var_objective).intersection(known_vars)])
+                    )
+
     # 'var2index' should be computed after there is no more further modification
     # to 'variables' or any of the constraint or objective dictionaries
     var2index = {x: i for i, x in enumerate(variables)}
 
     # Calculate the matrices A, C and vectors b, d such that
     # Ax + b >= 0, Cx + d == 0.
     A = dok_matrix((len(var_inequalities), len(variables)))
@@ -245,15 +250,14 @@
     d = dok_matrix((len(var_equalities), 1))
     for i, equality in enumerate(var_equalities):
         eq_vars = set(equality)
         for x in eq_vars.difference(known_vars):
             C[i, var2index[x]] = equality[x]
         d[i, 0] = float(sum([equality[x] * known_vars[x]
                              for x in eq_vars.intersection(known_vars)]))
-
     collect()
     if verbose > 1:
         print("Pre-processing took",
               format(perf_counter() - t0, ".4f"),
               "seconds.")
         t0 = perf_counter()
     if verbose > 0:
@@ -268,26 +272,26 @@
                 I = M.variable("I",
                                len(var_inequalities),
                                Domain.greaterThan(0))
                 # It seems MOSEK Fusion API does not allow to pick index i
                 # of an expression (A^T I)_i, so we do it manually row by row.
                 A = A.tocsr()
                 AtI = []  # \sum_j I_j A_ji as i-th entry of AtI
-                for i in range(len(variables)):
-                    slice_ = A[:, i]
+                for var in variables:
+                    slice_ = A[:, var2index[var]]
                     sparse_slice = Matrix.sparse(*slice_.shape,
                                                  *slice_.nonzero(),
                                                  slice_[slice_.nonzero()].A[0])
                     AtI.append(Expr.dot(sparse_slice, I))
             if var_equalities:
                 E = M.variable("E", len(var_equalities), Domain.unbounded())
                 C = C.tocsr()
                 CtI = []  # \sum_j E_j C_ji as i-th entry of CtI
-                for i in range(len(variables)):
-                    slice_ = C[:, i]
+                for var in variables:
+                    slice_ = C[:, var2index[var]]
                     sparse_slice = Matrix.sparse(*slice_.shape,
                                                  *slice_.nonzero(),
                                                  slice_[slice_.nonzero()].A[0])
                     CtI.append(Expr.dot(sparse_slice, E))
 
             # Define and set objective function
             # c0 + Tr Z F0 + I·b + E·d
@@ -314,17 +318,22 @@
                 del d_mosek
 
             M.objective(ObjectiveSense.Minimize, obj_mosek)
 
             # Add constraints
             # ci + Tr Z Fi + \sum_j I_j A_ji + \sum_j E_j C_ji == 0
             ci_constraints = []
+            if default_non_negative:
+                domain = Domain.lessThan(0)
+            else:
+                domain = Domain.equalsTo(0)
             for i, x in enumerate(variables):
                 lhs = 0.0
-                if var_objective and x in var_objective:
+                if var_objective and x in set(var_objective
+                                              ).difference(known_vars):
                     ci  = float(var_objective[x])
                     lhs += ci
                 try:
                     F = Fi.pop(x)
                     lhs = Expr.add(lhs,
                                    Expr.dot(Z,
                                             Matrix.sparse(
@@ -336,36 +345,39 @@
                     pass
                 if var_inequalities:
                     lhs = Expr.add(lhs, AtI[i])
                     AtI[i] = None
                 if var_equalities:
                     lhs = Expr.add(lhs, CtI[i])
                     CtI[i] = None
-                ci_constraints.append(M.constraint(f"c{i}",
-                                                   lhs,
-                                                   Domain.equalsTo(0)))
+                ci_constraints.append(M.constraint(f"c{i}", lhs, domain))
         else:
             # Set up the problem in primal formulation
 
             # Define variables
-            x_mosek = M.variable("x", len(variables), Domain.unbounded())
+            if default_non_negative:
+                domain = Domain.greaterThan(0)
+            else:
+                domain = Domain.unbounded()
+            x_mosek = M.variable("x", len(variables), domain)
 
             if var_inequalities:
                 b_mosek = Matrix.sparse(*b.shape,
                                         *b.nonzero(),
                                         b[b.nonzero()].A[0])
                 A_mosek = Matrix.sparse(*A.shape,
                                         *A.nonzero(),
                                         A[A.nonzero()].A[0])
                 ineq_constraint = M.constraint("Ineq",
                                                Expr.add(Expr.mul(A_mosek,
                                                                  x_mosek),
                                                         b_mosek),
                                                Domain.greaterThan(0))
                 del b_mosek, A_mosek
+
             if var_equalities:
                 d_mosek = Matrix.sparse(*d.shape,
                                         *d.nonzero(),
                                         d[d.nonzero()].A[0])
                 C_mosek = Matrix.sparse(*C.shape,
                                         *C.nonzero(),
                                         C[C.nonzero()].A[0])
```

### Comparing `inflation-1.0.0/inflation/sdp/writer_utils.py` & `inflation-2.0.0/inflation/sdp/writer_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This file contains helper functions to write and export the problems to various
 formats.
+
 @authors: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
 """
 import numpy as np
 
 from copy import deepcopy
 from scipy.io import savemat
 from warnings import warn
@@ -27,34 +28,35 @@
         fourth is a list of equality constraints of the form ``line = 0``.
     """
     matrix = deepcopy(problem.momentmatrix).astype(object)
     ### Process moment matrix
     # Replacer for constants
     constants = {moment.idx: str(value)
                  for moment, value in problem.known_moments.items()}
-    constant_replacer = np.vectorize(lambda x: constants.get(x, x))
     # Replacer for semiknowns
     semiknowns = dict()
     for key, val in problem.semiknown_moments.items():
         val_str = val[1].name.replace(", ", ";")
         semiknowns[key.idx] = f"{val[0]}*{val_str}"
     semiknown_replacer = np.vectorize(lambda x: semiknowns.get(x, str(x)))
     # Replacer for remaining symbols
     monomials = dict()
-    for mon in problem.monomials:
+    for mon in problem.moments:
         monomials[mon.idx] = mon.name.replace(", ", ";")
 
     def replace_known(monom):
         try:
             replacement = monomials.get(float(monom), monom)
         except ValueError:
             replacement = monom
         return replacement
     known_replacer = np.vectorize(replace_known)
-    matrix = constant_replacer(matrix)
+    for ii, row in enumerate(matrix):
+        for jj, col in enumerate(row):
+            matrix[ii, jj] = constants.get(col, col)
     matrix = semiknown_replacer(matrix)
     matrix = np.triu(known_replacer(matrix).astype(object))
 
     ### Process objective
     is_first = True
     try:
         independent_term = float(problem.objective[problem.One])
@@ -93,25 +95,46 @@
                 equality += str(abs(coeff))
             else:
                 if np.isclose(abs(coeff), 1):
                     equality += monom.name
                 else:
                     equality += f"{abs(coeff)}*{monom.name}"
         equalities.append(equality[1:] if equality[0] == "+" else equality)
-    return objective, matrix, bounds.tolist(), equalities
+    
+    ### Process inequalities
+    inequalities = []
+    for ineq in problem.moment_inequalities:
+        inequality = ""
+        for monom, coeff in ineq.items():
+            inequality += "+" if coeff > 0 else "-"
+            if monom == problem.One:
+                inequality += str(abs(coeff))
+            else:
+                if np.isclose(abs(coeff), 1):
+                    inequality += monom.name
+                else:
+                    inequality += f"{abs(coeff)}*{monom.name}"
+        inequalities.append(inequality[1:] if inequality[0] == "+"
+                            else inequality)
+    return objective, matrix, bounds.tolist(), equalities, inequalities
 
 
 def write_to_csv(problem, filename):
-    """Export the problem in a human-readable form in a CSV table.
+    """
+    Export the problem in a human-readable form in a CSV table.
 
-    :param problem: The SDP relaxation to write.
-    :type problem: :class:`inflation.InflationSDP`
-    :type filename: str
+    Parameters
+    ----------
+    problem : :class:`inflation.InflationSDP`
+        The SDP relaxation to write.
+    filename : str
+        The name of the file to write the CSV table to.
     """
-    objective, matrix, bounds, equalities = convert_to_human_readable(problem)
+    objective, matrix, bounds, equalities, inequalities \
+        = convert_to_human_readable(problem)
     f = open(filename, "w")
     f.write("Objective: " + objective + "\n")
     for matrix_line in matrix:
         f.write(
             str(list(matrix_line))[1:-1].replace(" ", "").replace("\'", ""))
         f.write("\n")
     f.write("Bounds:\n")
@@ -119,23 +142,62 @@
     for bound_line in bounds:
         f.write(str(bound_line)[1:-1].replace(" ", ""))
         f.write("\n")
     f.write("\nEqualities (format: line = 0):\n")
     for equality in equalities:
         f.write(equality)
         f.write("\n")
+    f.write("\nInequalities (format: line >= 0):\n")
+    for inequality in inequalities:
+        f.write(inequality)
+        f.write("\n")
     f.close()
 
 
 def write_to_mat(problem, filename):
-    """Export the problem to MATLAB .mat file.
+    """
+    Export the problem to MATLAB .mat file.
 
-    :param problem: The SDP relaxation to write.
-    :type problem: :class:`inflation.InflationSDP`
-    :type filename: str
+    Parameters
+    ----------
+    problem : inflation.InflationSDP
+        The SDP relaxation to write.
+    filename : str
+        The filename of the MATLAB .mat file to be created.
+
+    Notes
+    -----
+    MATLAB does not like 0s, so we shift all values by 1 if the variable 0
+    exists.
+
+    The exported MATLAB .mat file contains the following variables:
+    - moments_idx2name : numpy.ndarray
+        An array containing the indices and names of the moments.
+    - momentmatrix : numpy.ndarray
+        The moment matrix with the offset applied.
+    - objective : list
+        A list of lists containing the indices and coefficients of the objective
+        moments.
+    - known_moments : list
+        A list of lists containing the indices and values of the known moments.
+    - semiknown_moments : numpy.ndarray
+        A 2D array containing the indices, factors, and final indices of the
+        semi-known moments.
+    - moment_lowerbounds : list
+        A list of lists containing the indices and lower bounds of the moments.
+    - moment_upperbounds : list
+        A list of lists containing the indices and upper bounds of the moments.
+    - moment_equalities : list
+        A list of dictionaries representing moment equalities, where each
+        dictionary contains the indices and coefficients of the moments involved
+        in the equality.
+    - moment_inequalities : list
+        A list of dictionaries representing moment inequalities, where each
+        dictionary contains the indices and coefficients of the moments involved
+        in the inequality.
     """
     # MATLAB does not like 0s, so we shift all by 1 if the variable 0 exists
     offset = 1 if problem.momentmatrix_has_a_zero else 0
     final_positions_matrix = problem.momentmatrix + offset
     known_moments = [[mon.idx + offset, val]
                      for mon, val in problem.known_moments.items()]
     semiknown_initial = []
@@ -148,19 +210,19 @@
     semiknown_moments = np.vstack([semiknown_initial,
                                    semiknown_factors,
                                    semiknown_final]).T
     objective   = [[mon.idx + offset, float(coeff)]
                    for mon, coeff in problem.objective.items()
                    if abs(coeff) > 1e-8]
     lowerbounds = [[mon.idx + offset, bnd]
-                   for mon, bnd in problem._processed_moment_lowerbounds.items()]
+                   for mon, bnd in problem.moment_lowerbounds.items()]
     upperbounds = [[mon.idx + offset, bnd]
-                   for mon, bnd in problem._processed_moment_upperbounds.items()]
+                   for mon, bnd in problem.moment_upperbounds.items()]
     names       = np.array([[mon.idx + offset, mon.name]
-                             for mon in problem.monomials], dtype=object)
+                            for mon in problem.moments], dtype=object)
     equalities  = []
     for eq in problem.moment_equalities:
         equality = {'moments': np.array([mon.idx + offset for mon in eq]),
                     'coeffs':  np.array(list(eq.values()))}
         equalities.append(equality)
   
     inequalities  = []
@@ -180,20 +242,33 @@
                    "moment_equalities":   equalities,
                    "moment_inequalities": inequalities
                    }
             )
 
 
 def write_to_sdpa(problem, filename):
-    """Export the problem to a file in .dat-s format. See specifications at
-    http://euler.nmt.edu/~brian/sdplib/FORMAT.
+    """
+    Export the problem to a file in .dat-s format, per as
+    http://euler.nmt.edu/~brian/sdplib/FORMAT
+
+    Parameters
+    ----------
+    problem : inflation.InflationSDP
+        The SDP relaxation to write.
+    filename : str
+        The filename to write the SDP problem to.
 
-    :param problem: The SDP relaxation to write.
-    :type problem: :class:`inflation.InflationSDP`
-    :type filename: str
+    Notes
+    -----
+    This function exports the given SDP relaxation problem to a file in the
+    .dat-s format. The .dat-s format is a specific format used by the SDPA
+    software for semidefinite programming.
+
+    For more information about the .dat-s format, see the specifications at:
+    http://euler.nmt.edu/~brian/sdplib/FORMAT
     """
     # Compute actual number of variables: all in the moment matrix, minus those
     # with known values, minus those that participate in LPI constraints, plus
     # those where the unknown part of the LPI constraint is not in the original
     # moment matrix
     potential_nvars = problem.momentmatrix.max() - 1
     if len(problem.known_moments) == 1:
@@ -301,23 +376,42 @@
     if len(problem.moment_equalities) > 0:
         block += 1
         ii     = 1
         block_size = 2*len(problem.moment_equalities)
         blockstruct.append(str(-block_size))
     for equality in problem.moment_equalities:
         for var, coeff in equality.items():
-            if var != problem.One:
-                var = var_corresp[var.idx]
-                lines.append(f"{var}\t{block}\t{ii}\t{ii}\t{coeff}\n")
-                lines.append(f"{var}\t{block}\t{ii+1}\t{ii+1}\t{-coeff}\n")
-            else:
-                lines.append(f"0\t{block}\t{ii}\t{ii}\t{-coeff}\n")
-                lines.append(f"0\t{block}\t{ii+1}\t{ii+1}\t{coeff}\n")
+            if problem.known_moments.get(var, None) not in [0]:
+                if var != problem.One:
+                    var = var_corresp[var.idx]
+                    lines.append(f"{var}\t{block}\t{ii}\t{ii}\t{coeff}\n")
+                    lines.append(f"{var}\t{block}\t{ii+1}\t{ii+1}\t{-coeff}\n")
+                else:
+                    lines.append(f"0\t{block}\t{ii}\t{ii}\t{-coeff}\n")
+                    lines.append(f"0\t{block}\t{ii+1}\t{ii+1}\t{coeff}\n")
         ii += 2
 
+    # Prepare inequalities
+    if len(problem.moment_inequalities) > 0:
+        block += 1
+        ii = 1
+        block_size = len(problem.moment_inequalities)
+        blockstruct.append(str(-block_size))
+    for inequality in problem.moment_inequalities:
+        sumcoeffs = 0
+        for var, coeff in inequality.items():
+            if problem.known_moments.get(var, None) not in [0]:
+                if var != problem.One:
+                    var = var_corresp[var.idx]
+                    lines.append(f"{var}\t{block}\t{ii}\t{ii}\t{coeff}\n")
+                else:
+                    sumcoeffs += coeff
+        if sumcoeffs != 0:
+            lines.append(f"0\t{block}\t{ii}\t{ii}\t{-sumcoeffs}\n")
+        ii += 2
     file_ = open(filename, "w")
     file_.write("\"file " + filename + " generated by inflation\"\n")
     if abs(objective_constant) > 1e-8:
         file_.write("\"the objective contains a constant term of value "
                     + str(objective_constant) + " that is not included in the "
                     + "program below\"\n")
     file_.write(f"{nvars} = number of vars\n")
```

### Comparing `inflation-1.0.0/inflation.egg-info/PKG-INFO` & `inflation-2.0.0/inflation.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,132 @@
-Metadata-Version: 2.1
-Name: inflation
-Version: 1.0.0
-Summary: Implementations of the Inflation Technique for Causal Inference
-Home-page: https://github.com/ecboghiu/inflation
-Author: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
-Author-email: cristian.boghiu@icfo.eu, ewolfe@pitp.ca, physics@alexpozas.com
-License: GNU GPL v. 3.0
-Project-URL: Documentation, https://ecboghiu.github.io/inflation/_build/html/index.html
-Project-URL: Source, https://github.com/ecboghiu/inflation
-Project-URL: Issue Tracker, https://github.com/ecboghiu/inflation/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE
-
-[![DOI](https://zenodo.org/badge/500850617.svg)](https://zenodo.org/badge/latestdoi/500850617)
-
-# Inflation
-Inflation is a Python package that implements inflation algorithms for causal inference. In causal inference, the main task is to determine which causal relationships can exist between different observed random variables. Inflation algorithms are a class of techniques designed to solve the causal compatibility problem, that is, test compatibility between some observed data and a given causal relationship.
-
-The first version of this package implements the inflation technique for quantum causal compatibility. For details, see [Physical Review X 11 (2), 021043 (2021)](https://journals.aps.org/prx/abstract/10.1103/PhysRevX.11.021043). The inflation technique for classical causal compatibility will be implemented in a future update.
-
-Examples of use of this package include:
-
-- Feasibility problems and extraction of certificates.
-- Optimization of Bell operators.
-- Optimisation over classical distributions.
-- Standard [NavascuÃ©s-Pironio-AcÃ­n hierarchy](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.010401).
-- Scenarios with partial information.
-
-See the documentation for more details.
-
-## Documentation
-
-* [Latest version](https://ecboghiu.github.io/inflation/).
-
-## Installation
-
-To install the package, run the following command:
-
-```
-pip install inflation
-```
-
-You can also install directly from GitHub with:
-
-```
-pip install git+https://github.com/ecboghiu/inflation.git@main
-```
-
-or download the repository on your computer and run `pip install .` in the repository folder. Install the `devel` branch for the latest features and bugfixes.
-
-Tests are written outside the Python module, therefore they are not installed together with the package. To test the installation, clone the repository and run, in a Unix terminal,
-```python -m unittest -v```
-inside the repository folder.
-
-## Example
-
-The following example shows that the W distribution is incompatible with the triangle scenario with quantum sources by showing that a specific semidefinite programming relaxation is infeasible:
-
-```python
-from inflation import InflationProblem, InflationSDP
-import numpy as np
-
-P_W = np.zeros((2, 2, 2, 1, 1, 1))
-for a, b, c, x, y, z in np.ndindex(*P_W.shape):
-    if a + b + c == 1:
-        P_W[a, b, c, x, y, z] = 1 / 3
-
-triangle = InflationProblem(dag={"rho_AB": ["A", "B"],
-                                 "rho_BC": ["B", "C"],
-                                 "rho_AC": ["A", "C"]},
-                             outcomes_per_party=(2, 2, 2),
-                             settings_per_party=(1, 1, 1),
-                             inflation_level_per_source=(2, 2, 2))
-
-sdp = InflationSDP(triangle, verbose=1)
-sdp.generate_relaxation('npa2')
-sdp.set_distribution(P_W)
-sdp.solve()
-
-print("Problem status:", sdp.status)
-print("Infeasibility certificate:", sdp.certificate_as_probs())
-```
-
-For more information about the theory and other features, please visit the [documentation](https://ecboghiu.github.io/inflation/), and more specifically the [Tutorial](https://ecboghiu.github.io/inflation/_build/html/tutorial.html) and [Examples](https://ecboghiu.github.io/inflation/_build/html/examples.html) pages.
-
-## How to contribute
-
-Contributions are welcome and appreciated. If you want to contribute, you can read the [contribution guidelines](https://github.com/ecboghiu/inflation/blob/main/CONTRIBUTE.md). You can also read the [documentation](https://ecboghiu.github.io/inflation/) to learn more about how the package works.
-
-## License
-
-Inflation is free open-source software released under [GNU GPL v. 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
-
-## Citing Inflation
-
-If you use Inflation in your work, please cite [Inflation's paper](https://www.arxiv.org/abs/2211.04483):
-
-- Emanuel-Cristian Boghiu, Elie Wolfe and Alejandro Pozas-Kerstjens, "Inflation: a Python package for classical and quantum causal compatibility", arXiv:2211.04483
-
-```
-@misc{2211.04483,
-  doi = {10.48550/arXiv.2211.04483},
-  url = {https://arxiv.org/abs/2211.04483},
-  author = {Boghiu, Emanuel-Cristian and Wolfe, Elie and Pozas-Kerstjens, Alejandro},
-  title = {{Inflation}: a {Python} package for classical and quantum causal compatibility},
-  publisher = {arXiv},
-  year = {2022},
-  copyright = {arXiv.org perpetual, non-exclusive license}
-}
-```
+Metadata-Version: 2.1
+Name: inflation
+Version: 2.0.0
+Summary: Implementations of the Inflation Technique for Causal Inference
+Home-page: https://github.com/ecboghiu/inflation
+Author: Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens
+Author-email: cristian.boghiu@icfo.eu, ewolfe@pitp.ca, physics@alexpozas.com
+License: GNU GPL v. 3.0
+Project-URL: Documentation, https://ecboghiu.github.io/inflation/_build/html/index.html
+Project-URL: Source, https://github.com/ecboghiu/inflation
+Project-URL: Issue Tracker, https://github.com/ecboghiu/inflation/issues
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: mosek>=10
+Requires-Dist: networkx
+Requires-Dist: numba
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: sympy
+Requires-Dist: tqdm
+Provides-Extra: docs
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: m2r2; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx_copybutton; extra == "docs"
+
+[![DOI](https://zenodo.org/badge/500850617.svg)](https://zenodo.org/badge/latestdoi/500850617)
+
+# Inflation
+Inflation is a Python package that implements inflation algorithms for causal inference. In causal inference, the main task is to determine which causal relationships can exist between different observed random variables. Inflation algorithms are a class of techniques designed to solve the causal compatibility problem, that is, test compatibility between some observed data and a given causal relationship.
+
+The first version of this package implements the inflation technique for quantum causal compatibility. For details, see [Physical Review X 11 (2), 021043 (2021)](https://journals.aps.org/prx/abstract/10.1103/PhysRevX.11.021043). The inflation technique for classical causal compatibility will be implemented in a future update.
+
+Examples of use of this package include:
+
+- Feasibility problems and extraction of certificates.
+- Optimization of Bell operators.
+- Optimisation over classical distributions.
+- Standard [Navascués-Pironio-Acín hierarchy](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.010401).
+- Scenarios with partial information.
+- Possibilistic compatibility with a causal network.
+- Estimation of do-conditionals and causal strengths.
+
+See the documentation for more details.
+
+## Documentation
+
+* [Latest version](https://ecboghiu.github.io/inflation/).
+
+## Installation
+
+To install the package, run the following command:
+
+```
+pip install inflation
+```
+
+You can also install directly from GitHub with:
+
+```
+pip install git+https://github.com/ecboghiu/inflation.git@main
+```
+
+or download the repository on your computer and run `pip install .` in the repository folder. Install the `devel` branch for the latest features and bugfixes.
+
+Tests are written outside the Python module, therefore they are not installed together with the package. To test the installation, clone the repository and run, in a Unix terminal,
+```python -m unittest -v```
+inside the repository folder.
+
+## Example
+
+The following example shows that the W distribution is incompatible with the triangle scenario with quantum sources by showing that a specific semidefinite programming relaxation is infeasible:
+
+```python
+from inflation import InflationProblem, InflationSDP
+import numpy as np
+
+P_W = np.zeros((2, 2, 2, 1, 1, 1))
+for a, b, c, x, y, z in np.ndindex(*P_W.shape):
+    if a + b + c == 1:
+        P_W[a, b, c, x, y, z] = 1 / 3
+
+triangle = InflationProblem(dag={"rho_AB": ["A", "B"],
+                                 "rho_BC": ["B", "C"],
+                                 "rho_AC": ["A", "C"]},
+                             outcomes_per_party=(2, 2, 2),
+                             settings_per_party=(1, 1, 1),
+                             inflation_level_per_source=(2, 2, 2))
+
+sdp = InflationSDP(triangle, verbose=1)
+sdp.generate_relaxation('npa2')
+sdp.set_distribution(P_W)
+sdp.solve()
+
+print("Problem status:", sdp.status)
+print("Infeasibility certificate:", sdp.certificate_as_probs())
+```
+
+For more information about the theory and other features, please visit the [documentation](https://ecboghiu.github.io/inflation/), and more specifically the [Tutorial](https://ecboghiu.github.io/inflation/_build/html/tutorial.html) and [Examples](https://ecboghiu.github.io/inflation/_build/html/examples.html) pages.
+
+## How to contribute
+
+Contributions are welcome and appreciated. If you want to contribute, you can read the [contribution guidelines](https://github.com/ecboghiu/inflation/blob/main/CONTRIBUTE.md). You can also read the [documentation](https://ecboghiu.github.io/inflation/) to learn more about how the package works.
+
+## License
+
+Inflation is free open-source software released under [GNU GPL v. 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+## Citing Inflation
+
+If you use Inflation in your work, please cite [Inflation's paper](https://www.arxiv.org/abs/2211.04483):
+
+- Emanuel-Cristian Boghiu, Elie Wolfe and Alejandro Pozas-Kerstjens, "Inflation: a Python package for classical and quantum causal compatibility", Quantum **7**, 996 (2023), arXiv:2211.04483
+
+```
+@article{pythoninflation,
+  doi = {10.22331/q-2023-05-04-996},
+  url = {https://doi.org/10.22331/q-2023-05-04-996},
+  title = {Inflation: a {P}ython library for classical and quantum causal compatibility},
+  author = {Boghiu, Emanuel-Cristian and Wolfe, Elie and Pozas-Kerstjens, Alejandro},
+  journal = {{Quantum}},
+  issn = {2521-327X},
+  publisher = {{Verein zur F{\"{o}}rderung des Open Access Publizierens in den Quantenwissenschaften}},
+  volume = {7},
+  pages = {996},
+  month = may,
+  year = {2023},
+  archivePrefix = {arXiv},
+  eprint = {2211.04483}
+}
+```
```

### Comparing `inflation-1.0.0/inflation.egg-info/SOURCES.txt` & `inflation-2.0.0/inflation.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 MANIFEST.in
 README.md
 setup.py
 inflation/InflationProblem.py
 inflation/__init__.py
 inflation/_about.py
 inflation/_version.py
+inflation/optimization_utils.py
 inflation/utils.py
 inflation.egg-info/PKG-INFO
 inflation.egg-info/SOURCES.txt
 inflation.egg-info/dependency_links.txt
 inflation.egg-info/not-zip-safe
 inflation.egg-info/requires.txt
 inflation.egg-info/top_level.txt
+inflation/lp/InflationLP.py
+inflation/lp/__init__.py
+inflation/lp/lp_utils.py
+inflation/lp/monomial_classes.py
+inflation/lp/numbafied.py
+inflation/lp/writer_utils.py
 inflation/sdp/InflationSDP.py
 inflation/sdp/__init__.py
 inflation/sdp/fast_npa.py
 inflation/sdp/monomial_classes.py
 inflation/sdp/monomial_utils.py
-inflation/sdp/optimization_utils.py
 inflation/sdp/quantum_tools.py
 inflation/sdp/sdp_utils.py
 inflation/sdp/writer_utils.py
 test/test_factorization.py
 test/test_functions.py
 test/test_monomial_properties.py
 test/test_optimize.py
 test/test_pipeline.py
-test/test_solvers.py
+test/test_solvers.py
+test/test_writers.py
```

### Comparing `inflation-1.0.0/setup.py` & `inflation-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 with open('inflation/_version.py') as f:
     exec(f.read())
 
 setup(
     name="inflation",
     version=__version__,
-    install_requires=["numpy", "sympy", "scipy", "numba", "mosek", "tqdm"],
+    install_requires=["mosek>=10", "networkx", "numba", "numpy",
+                      "scipy", "sympy", "tqdm"],
     extras_require={
         "docs": ["nbsphinx", "m2r2", "sphinx_rtd_theme", "sphinx_copybutton"]
     },
     author="Emanuel-Cristian Boghiu, Elie Wolfe, Alejandro Pozas-Kerstjens",
     author_email="cristian.boghiu@icfo.eu, ewolfe@pitp.ca, physics@alexpozas.com",
     description="Implementations of the Inflation Technique for Causal Inference",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     packages=find_packages(exclude=["test", "doc*", "example*"]),
     license="GNU GPL v. 3.0",
     url="https://github.com/ecboghiu/inflation",
     project_urls={"Documentation": "https://ecboghiu.github.io/inflation/_build/html/index.html",
                   "Source": "https://github.com/ecboghiu/inflation",
                   "Issue Tracker": "https://github.com/ecboghiu/inflation/issues"},
     zip_safe=False,  # To avoid problems with Numba, https://github.com/numba/numba/issues/4908
```

### Comparing `inflation-1.0.0/test/test_factorization.py` & `inflation-2.0.0/test/test_factorization.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,22 @@
         monomial = np.array([[1, 0, 1, 1, 0, 0],
                              [2, 1, 0, 2, 0, 0],
                              [1, 0, 3, 3, 0, 0],
                              [3, 3, 5, 0, 0, 0],
                              [3, 1, 4, 0, 0, 0],
                              [3, 6, 6, 0, 0, 0],
                              [3, 4, 5, 0, 0, 0]])
-        factorised = prob.factorize_monomial(monomial, canonical_order=True)
-        correct    = np.array([np.array([[1, 0, 1, 1, 0, 0]]),
-                               np.array([[1, 0, 3, 3, 0, 0]]),
-                               np.array([[2, 1, 0, 2, 0, 0],
-                                         [3, 1, 4, 0, 0, 0]]),
-                               np.array([[3, 3, 5, 0, 0, 0],
-                                         [3, 4, 5, 0, 0, 0]]),
-                               np.array([[3, 6, 6, 0, 0, 0]])], dtype=object)
+        factorised = prob.factorize_monomial_2d(monomial, canonical_order=True)
+        correct    = [np.array([[1, 0, 1, 1, 0, 0]]),
+                      np.array([[1, 0, 3, 3, 0, 0]]),
+                      np.array([[2, 1, 0, 2, 0, 0],
+                                [3, 1, 4, 0, 0, 0]]),
+                      np.array([[3, 3, 5, 0, 0, 0],
+                                [3, 4, 5, 0, 0, 0]]),
+                      np.array([[3, 6, 6, 0, 0, 0]])]
 
         self.assertEqual(len(correct), len(factorised),
                          "The factorization is not finding all factors.")
         for idx in range(len(correct)):
             self.assertTrue(np.allclose(correct[idx], factorised[idx]),
                             "The factors found are not in canonical form.")
 
@@ -48,15 +48,15 @@
                              [2, 1, 2, 0, 0],
                              [3, 3, 4, 0, 0],
                              [3, 1, 1, 0, 0],
                              [3, 4, 3, 1, 0],
                              [4, 0, 3, 1, 0],
                              [4, 0, 2, 1, 0],
                              [4, 0, 1, 1, 0]])
-        factorised = prob.factorize_monomial(monomial)
+        factorised = prob.factorize_monomial_2d(monomial)
         correct    = np.array([np.array([[1, 1, 0, 1, 0],
                                          [1, 1, 0, 0, 0],
                                          [2, 1, 1, 0, 0],
                                          [2, 1, 2, 0, 0],
                                          [3, 1, 1, 0, 0],
                                          [4, 0, 2, 1, 0],
                                          [4, 0, 1, 1, 0]]),
@@ -75,44 +75,44 @@
         # (because A and C are not causally connected). This should be taken
         # into account because A1C1 = A1C2 in the bilocal scenario
         # Input and output are set to 0 because they are irrelevant.
         prob = InflationProblem(dag={"h1": ["v1", "v2"],
                                      "h2": ["v2", "v3"]},
                                 outcomes_per_party=[2, 2, 2],
                                 inflation_level_per_source=[2, 2])
-        A1C1 = np.array([[0, 1, 0, 0, 0],
-                         [2, 0, 1, 0, 0]])
-        A1C2 = np.array([[0, 1, 0, 0, 0],
-                         [2, 0, 2, 0, 0]])
+        A1C1 = np.array([[1, 1, 0, 0, 0],
+                         [3, 0, 1, 0, 0]])
+        A1C2 = np.array([[1, 1, 0, 0, 0],
+                         [3, 0, 2, 0, 0]])
 
-        self.assertEqual(len(prob.factorize_monomial(A1C1)),
-                         len(prob.factorize_monomial(A1C2)),
+        self.assertEqual(len(prob.factorize_monomial_2d(A1C1)),
+                         len(prob.factorize_monomial_2d(A1C2)),
                          "Causally independent parties are being treated "
                          + "different depending on the copy indices.")
 
     def test_unfactorizable(self):
         prob = InflationProblem(dag={"h1": ["v2", "v3"],
                                      "h2": ["v1", "v2"],
                                      "h3": ["v1", "v3"]},
                                 outcomes_per_party=[2, 2, 2],
                                 inflation_level_per_source=[2, 2, 2])
         # monomial = < A^011_00 * B^101_00 * C^120_00 >
         monomial = np.array([[1, 0, 1, 1, 0, 0],
                              [2, 1, 1, 0, 0, 0],
                              [3, 1, 0, 2, 0, 0]])
-        factorised = prob.factorize_monomial(monomial)
+        factorised = prob.factorize_monomial_2d(monomial)
 
         self.assertEqual(monomial.tolist(), factorised[0].tolist(),
                          "Non-factorizable monomials are being factorized.")
 
     def test_unfactorizable_NC(self):
         # monomial = < A_00 * A_10 * A_00 >
         prob = InflationProblem(outcomes_per_party=[2],
                                 settings_per_party=[2])
         monomial = np.array([[1, 1, 0, 0],
                              [1, 1, 1, 0],
                              [1, 1, 0, 0]])
-        factorised = prob.factorize_monomial(monomial)
+        factorised = prob.factorize_monomial_2d(monomial)
 
         self.assertEqual(monomial.tolist(), factorised[0].tolist(),
                          "Non-factorizable, non-commutative monomials are "
                          + "being reordered as if they were commutative.")
```

### Comparing `inflation-1.0.0/test/test_optimize.py` & `inflation-2.0.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `inflation-1.0.0/test/test_pipeline.py` & `inflation-2.0.0/test/test_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import unittest
 import numpy as np
 import warnings
+from itertools import product
 
-from inflation import InflationProblem, InflationSDP
+from inflation import InflationProblem, InflationSDP, InflationLP
 
 bilocalDAG = {"h1": ["A", "B"], "h2": ["B", "C"]}
 bilocality = InflationProblem(dag=bilocalDAG,
                               settings_per_party=[1, 1, 1],
                               outcomes_per_party=[2, 2, 2],
                               inflation_level_per_source=[2, 2])
+bilocality_c = InflationProblem(dag=bilocalDAG,
+                                settings_per_party=[1, 1, 1],
+                                outcomes_per_party=[2, 2, 2],
+                                inflation_level_per_source=[2, 2],
+                                classical_sources="all")
 bilocalSDP = InflationSDP(bilocality)
 
 trivial = InflationProblem({"h": ["v"]},
                            outcomes_per_party=[2],
                            settings_per_party=[2],
                            inflation_level_per_source=[2]
                            )
+trivial_c = InflationProblem({"h": ["v"]},
+                           outcomes_per_party=[2],
+                           settings_per_party=[2],
+                           inflation_level_per_source=[2],
+                           classical_sources="all"
+                           )
 
 
 class TestMonomialGeneration(unittest.TestCase):
-    bilocalSDP_commuting = InflationSDP(bilocality, commuting=True)
+    bilocalSDP_commuting = InflationSDP(bilocality_c)
     # Column structure for the NPA level 2 in a tripartite scenario
     col_structure = [[],
                      [0], [1], [2],
                      [0, 0], [0, 1], [0, 2], [1, 1], [1, 2], [2, 2]]
     # Monomials for the NPA level 2 in the bilocality scenario
     meas = bilocalSDP.measurements
     A_1_0_0_0 = meas[0][0][0][0]
@@ -45,15 +57,16 @@
             B_2_1_0_0*B_1_1_0_0, B_2_1_0_0*B_2_2_0_0, B_2_2_0_0*B_1_2_0_0,
             B_2_2_0_0*B_2_1_0_0, B_1_1_0_0*C_0_1_0_0, B_1_1_0_0*C_0_2_0_0,
             B_1_2_0_0*C_0_1_0_0, B_1_2_0_0*C_0_2_0_0, B_2_1_0_0*C_0_1_0_0,
             B_2_1_0_0*C_0_2_0_0, B_2_2_0_0*C_0_1_0_0, B_2_2_0_0*C_0_2_0_0,
             C_0_1_0_0*C_0_2_0_0]
     actual_cols = []
     for col in cols:
-        actual_cols.append(bilocalSDP._interpret_name(col))
+        actual_cols.append(bilocalSDP.mon_to_lexrepr(bilocalSDP._interpret_name(col)))
+    actual_cols_2d = [bilocalSDP._lexorder[lexmon] for lexmon in actual_cols]
 
     def test_generating_columns_c(self):
         truth = 37
         columns = self.bilocalSDP_commuting.build_columns(self.col_structure)
         self.assertEqual(len(columns), truth,
                          "With commuting variables, there are  " +
                          str(len(columns)) + " columns but " + str(truth) +
@@ -64,15 +77,15 @@
         columns = bilocalSDP.build_columns(self.col_structure)
         self.assertEqual(len(columns), truth,
                          "With noncommuting variables, there are  " +
                          str(len(columns)) + " columns but " + str(truth) +
                          " were expected.")
 
     def test_generation_from_columns(self):
-        columns = bilocalSDP.build_columns(self.actual_cols)
+        columns = bilocalSDP.build_columns(self.actual_cols_2d)
         areequal = all(np.array_equal(r[0].T, np.array(r[1]).T)
                        for r in zip(columns, self.actual_cols))
         self.assertTrue(areequal, "The direct copying of columns is failing.")
 
     def test_generation_from_lol(self):
         columns = bilocalSDP.build_columns(self.col_structure)
         areequal = all(np.array_equal(r[0].T, np.array(r[1]).T)
@@ -83,147 +96,196 @@
     def test_generation_from_str(self):
         columns = bilocalSDP.build_columns("npa2")
         areequal = all(np.array_equal(r[0].T, np.array(r[1]).T)
                        for r in zip(columns, self.actual_cols))
         self.assertTrue(areequal,
                         "Parsing NPA levels with string description fails.")
         columns = bilocalSDP.build_columns("local2", max_monomial_length=2)
-        diff = set(bilocalSDP._from_2dndarray(col) for col in columns
+        diff = set(tuple(col) for col in columns
                    ).difference(
-                       set(bilocalSDP._from_2dndarray(col)
+                       set(tuple(col)
                            for col in self.actual_cols))
         self.assertTrue(len(diff) == 0,
                         "Parsing local levels with string description fails.")
         columns = bilocalSDP.build_columns("local221", max_monomial_length=2)
-        diff = set(bilocalSDP._from_2dndarray(col) for col in columns
+        diff = set(tuple(col) for col in columns
                    ).difference(
-                       set(bilocalSDP._from_2dndarray(col)
+                       set(tuple(col)
                            for col in self.actual_cols[:-1]))
         self.assertTrue(len(diff) == 0,
                         "Parsing local levels with individual string " +
                         "descriptions fails.")
         columns = bilocalSDP.build_columns("physical2",
                                            max_monomial_length=2)
         physical = (self.actual_cols[:22] + [self.actual_cols[24]]
                     + [self.actual_cols[26]] + self.actual_cols[32:])
-        diff = set(bilocalSDP._from_2dndarray(col) for col in columns
+        diff = set(tuple(col) for col in columns
                    ).difference(
-                       set(bilocalSDP._from_2dndarray(col)
+                       set(tuple(col)
                            for col in physical))
         self.assertTrue(len(diff) == 0,
                         "Parsing physical levels with global string " +
                         "description fails.")
         columns = bilocalSDP.build_columns("physical", max_monomial_length=2)
-        diff = set(bilocalSDP._from_2dndarray(col) for col in columns
+        diff = set(tuple(col) for col in columns
                    ).difference(
-                       set(bilocalSDP._from_2dndarray(col)
+                       set(tuple(col)
                            for col in physical))
         self.assertTrue(len(diff) == 0,
                         "Parsing physical levels without further " +
                         "description fails.")
         columns = bilocalSDP.build_columns("physical121",
                                            max_monomial_length=2)
-        diff = set(bilocalSDP._from_2dndarray(col) for col in columns
+        diff = set(tuple(col) for col in columns
                    ).difference(
-                       set(bilocalSDP._from_2dndarray(col)
+                       set(tuple(col)
                            for col in (self.actual_cols[:9]
                                        + self.actual_cols[10:22]
                                        + [self.actual_cols[24]]
                                        + [self.actual_cols[26]]
                                        + self.actual_cols[32:-1])))
         self.assertTrue(len(diff) == 0,
                         "Parsing physical levels with individual string " +
                         "descriptions fails.")
 
     def test_generation_with_identities(self):
         oneParty = InflationSDP(InflationProblem({"h": ["v"]}, [2], [2], [1]))
         columns  = oneParty.build_columns([[], [0, 0]])
-        truth    = [[],
-                    [[1, 1, 0, 0], [1, 1, 1, 0]],
-                    [[1, 1, 1, 0], [1, 1, 0, 0]]]
-        truth    = [np.array(mon) for mon in truth]
+        truth    = [np.array([[1, 1, 0, 0], [1, 1, 1, 0]]),
+                    np.array([[1, 1, 1, 0], [1, 1, 0, 0]])]
+        truth    = [np.empty((0,4), dtype=int)] + [oneParty.mon_to_lexrepr(mon) 
+                                                   for mon in truth]
         self.assertTrue(len(columns) == len(truth),
                         "Generating columns with identities is not producing "
                         + "the correct number of columns.")
         areequal = all(np.array_equiv(r[0].T, np.array(r[1]).T)
                        for r in zip(columns, truth))
         self.assertTrue(areequal,
                         "The column generation is not capable of handling " +
-                        "monomials that reduce to the identity")
+                        "monomials that reduce to the identity" +
+                        f"\ngot: {columns} \nexpected: {truth}")
 
 
 class TestReset(unittest.TestCase):
     sdp = InflationSDP(trivial)
     sdp.generate_relaxation("npa1")
+    physical_bounds = {m: 0. for m in sdp.hermitian_moments}
+    del physical_bounds[sdp.One]
 
     def prepare_objects(self, infSDP):
         var1 = infSDP.measurements[0][0][0][0]
         var2 = infSDP.measurements[0][0][1][0]
         infSDP.set_objective(var1, "max")
         infSDP.set_bounds({var1*var2: 0.9}, "up")
         infSDP.set_bounds({var1*var2: 0.1}, "lo")
         infSDP.set_values({var2: 0.5})
 
     def test_reset_all(self):
         self.prepare_objects(self.sdp)
         self.sdp.reset("all")
-        self.assertTrue(len(self.sdp._processed_moment_lowerbounds) == 0,
-                        "Resetting lower bounds fails.")
-        self.assertTrue(len(self.sdp._processed_moment_upperbounds) == 0,
-                        "Resetting upper bounds fails.")
+        self.assertEqual(self.sdp.moment_lowerbounds,
+                         self.physical_bounds,
+                         "Resetting lower bounds fails.")
+        self.assertEqual(self.sdp.moment_upperbounds, dict(),
+                         "Resetting processed upper bounds fails.")
         self.assertEqual(self.sdp.objective, {self.sdp.One: 0.},
                          "Resetting the objective function fails.")
-        self.assertTrue(len(self.sdp.semiknown_moments) == 0,
-                        "Resetting the known values fails to empty " +
-                        "semiknown_moments.")
+        self.assertEqual(self.sdp.semiknown_moments, dict(),
+                         "Resetting the known values fails to empty " +
+                         "semiknown_moments.")
         self.assertEqual(self.sdp.known_moments, {self.sdp.One: 1.},
                          "Resetting the known values fails to empty " +
                          "known_moments.")
 
     def test_reset_bounds(self):
         self.prepare_objects(self.sdp)
+        correct = {key: val for key, val in self.physical_bounds.items()
+                   if key not in self.sdp.known_moments}
         self.sdp.reset("bounds")
-        self.assertTrue(len(self.sdp._processed_moment_lowerbounds) == 0,
-                        "Resetting lower bounds fails.")
-        self.assertTrue(len(self.sdp._processed_moment_upperbounds) == 0,
-                        "Resetting upper bounds fails.")
+        self.assertEqual(self.sdp.moment_lowerbounds,
+                         correct,
+                         "Resetting lower bounds fails.")
+        self.assertEqual(self.sdp.moment_upperbounds, dict(),
+                         "Resetting upper bounds fails.")
+        self.assertTrue(len(self.sdp.objective) == 2,
+                        "Resetting the bounds resets the objective function.")
+        self.assertTrue(len(self.sdp.known_moments) == 3,
+                        "Resetting the bounds resets the known moments.")
 
     def test_reset_some(self):
         self.prepare_objects(self.sdp)
         self.sdp.reset(["objective", "values"])
         self.assertEqual(self.sdp.objective, {self.sdp.One: 0.},
                          "Resetting the objective function fails.")
-        self.assertTrue(len(self.sdp.semiknown_moments) == 0,
+        self.assertEqual(self.sdp.semiknown_moments, dict(),
                         "Resetting the known values fails to empty " +
                         "semiknown_moments.")
         self.assertEqual(self.sdp.known_moments, {self.sdp.One: 1.},
                          "Resetting the known values fails to empty " +
                          "known_moments.")
-        self.assertEqual(self.sdp.objective, {self.sdp.One: 0.},
-                         "Resetting the objective function fails.")
-        self.assertTrue(len(self.sdp._processed_moment_lowerbounds) == 4,
+        self.assertTrue(len(self.sdp.moment_lowerbounds) == 4,
                         "Lower bounds are being reset when they should not.")
-        self.assertTrue(len(self.sdp._processed_moment_upperbounds) == 1,
+        self.assertTrue(len(self.sdp.moment_upperbounds) == 1,
                         "Upper bounds are being reset when they should not.")
 
     def test_reset_objective(self):
         self.prepare_objects(self.sdp)
         self.sdp.reset("objective")
         self.assertEqual(self.sdp.objective, {self.sdp.One: 0.},
                          "Resetting the objective function fails.")
+        self.assertTrue(len(self.sdp.known_moments) == 3,
+                        "Resetting the objective resets the known moments.")
+        self.assertTrue(len(self.sdp.moment_lowerbounds) == 4,
+                        "Resetting the objective resets the lower bounds.")
+        self.assertTrue(len(self.sdp.moment_upperbounds) == 1,
+                        "Resetting the objective resets the upper bounds.")
 
     def test_reset_values(self):
         self.prepare_objects(self.sdp)
         self.sdp.reset("values")
-        self.assertTrue(len(self.sdp.semiknown_moments) == 0,
-                        "Resetting the known values fails to empty " +
-                        "semiknown_moments.")
+        self.assertEqual(self.sdp.semiknown_moments, dict(),
+                         "Resetting the known values fails to empty " +
+                         "semiknown_moments.")
         self.assertEqual(self.sdp.known_moments, {self.sdp.One: 1.},
                          "Resetting the known values fails to empty " +
                          "known_moments.")
+        self.assertTrue(len(self.sdp.moment_lowerbounds) == 4,
+                        "Resetting the objective resets the lower bounds.")
+        self.assertTrue(len(self.sdp.moment_upperbounds) == 1,
+                        "Resetting the objective resets the upper bounds.")
+        self.assertTrue(len(self.sdp.objective) == 2,
+                        "Resetting the bounds resets the objective function.")
+
+
+class TestResetLP(unittest.TestCase):
+    lp = InflationLP(trivial_c, nonfanout=False)
+    lp._generate_lp()
+
+    def setUp(self) -> None:
+        var1 = "P[v_0=0 v_1=0]"
+        var2 = "pv(0|1)"
+        self.lp.set_objective({var1: 1}, "max")
+        self.lp.set_bounds({var1: 0.9}, "up")
+        self.lp.set_bounds({var1: 0.1}, "lo")
+        self.lp.set_values({var2: 0.5})
+
+    def test_reset_all(self):
+        self.lp.reset("all")
+        self.assertEqual(self.lp.moment_lowerbounds, dict(),
+                         "Resetting lower bounds failed.")
+        self.assertEqual(self.lp.moment_upperbounds, dict(),
+                         "Resetting upper bounds failed.")
+        self.assertEqual(self.lp.objective, dict(),
+                         "Resetting objective failed.")
+        self.assertEqual(self.lp.semiknown_moments, dict(),
+                         "Resetting known values failed to empty "
+                         "semiknown_moments.")
+        self.assertEqual(self.lp.known_moments, {self.lp.One: 1.},
+                         "Resetting known values failed to empty "
+                         "known_moments.")
 
 
 class TestSDPOutput(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         warnings.simplefilter("ignore", category=DeprecationWarning)
         warnings.simplefilter("ignore", category=UserWarning)
@@ -239,28 +301,48 @@
                         dist[a, b, c, 0, 0, 0] = (1-v)/8
         return dist
 
     bellScenario = InflationProblem({"Lambda": ["A", "B"]},
                                     outcomes_per_party=[2, 2],
                                     settings_per_party=[2, 2],
                                     inflation_level_per_source=[1])
+    bellScenario_c = InflationProblem({"Lambda": ["A", "B"]},
+                                      outcomes_per_party=[2, 2],
+                                      settings_per_party=[2, 2],
+                                      inflation_level_per_source=[1],
+                                      classical_sources='all')
 
     cutInflation = InflationProblem({"lambda": ["a", "b"],
                                      "mu": ["b", "c"],
                                      "sigma": ["a", "c"]},
                                     outcomes_per_party=[2, 2, 2],
                                     settings_per_party=[1, 1, 1],
                                     inflation_level_per_source=[2, 1, 1])
 
+    cutInflation_c = InflationProblem({"lambda": ["a", "b"],
+                                       "mu": ["b", "c"],
+                                       "sigma": ["a", "c"]},
+                                      outcomes_per_party=[2, 2, 2],
+                                      settings_per_party=[1, 1, 1],
+                                      inflation_level_per_source=[2, 1, 1],
+                                      classical_sources="all")
+
     instrumental = InflationProblem({"U_AB": ["A", "B"],
                                      "A": ["B"]},
                                     outcomes_per_party=(2, 2),
                                     settings_per_party=(3, 1),
                                     inflation_level_per_source=(1,),
                                     order=("A", "B"))
+    instrumental_c = InflationProblem({"U_AB": ["A", "B"],
+                                       "A": ["B"]},
+                                      outcomes_per_party=(2, 2),
+                                      settings_per_party=(3, 1),
+                                      inflation_level_per_source=(1,),
+                                      order=("A", "B"),
+                                      classical_sources='all')
 
     incompatible_dist = np.array([[[[0.5], [0.5], [0.0]],
                                    [[0.0], [0.0], [0.5]]],
                                   [[[0.0], [0.5], [0.0]],
                                    [[0.5], [0.0], [0.5]]]], dtype=float)
 
     def test_bounds(self):
@@ -284,15 +366,15 @@
                         "Setting upper bounds to monomials is failing. The " +
                         f"result obtained for [min x s.t. x >= {lb}] is " +
                         f"{sdp.objective_value}.")
 
     def test_CHSH(self):
         sdp = InflationSDP(self.bellScenario)
         sdp.generate_relaxation("npa1")
-        self.assertEqual(len(sdp.generating_monomials), 5,
+        self.assertEqual(sdp.n_columns, 5,
                          "The number of generating columns is not correct.")
         self.assertEqual(sdp.n_knowable, 8 + 1,  # only '1' is included here.
                          "The count of knowable moments is wrong.")
         self.assertEqual(sdp.n_unknowable, 2,
                          "The count of unknowable moments is wrong.")
         meas = sdp.measurements
         A0 = 2*meas[0][0][0][0] - 1
@@ -338,15 +420,15 @@
                                      "A": ["B", "C", "D"]},
                                 outcomes_per_party=(2, 2, 2, 2),
                                 settings_per_party=(1, 1, 1, 1),
                                 inflation_level_per_source=(1, 1, 1),
                                 order=("A", "B", "C", "D"))
         sdp = InflationSDP(prob)
         sdp.generate_relaxation("npa2")
-        equalities = sdp.moment_equalities
+        equalities = sdp.minimal_equalities
 
         self.assertEqual(len(equalities), 738,
                          "Failing to obtain the correct number of implicit " +
                          "equalities in a non-network scenario.")
 
         # TODO: When we add support for user-specifiable equalities, modify
         # this test to only check implicit equalities.
@@ -357,67 +439,89 @@
 
         self.assertTrue(all(sdp.Zero.name not in equality.keys()
                             for equality in equalities),
                         "Some implicit equalities are wrongly assigning " +
                         "coefficients to the zero monomial.")
 
     def test_GHZ_commuting(self):
-        sdp = InflationSDP(self.cutInflation, commuting=True)
+        sdp = InflationSDP(self.cutInflation_c)
         sdp.generate_relaxation("local1")
-        self.assertEqual(len(sdp.generating_monomials), 18,
+        self.assertEqual(sdp.n_columns, 18,
                          "The number of generating columns is not correct.")
         self.assertEqual(sdp.n_knowable, 8 + 1,  # only '1' is included here.
                          "The count of knowable moments is wrong.")
         self.assertEqual(sdp.n_unknowable, 11,
                          "The count of unknowable moments is wrong.")
 
         sdp.set_distribution(self.GHZ(0.5 + 1e-2))
         sdp.solve()
         self.assertEqual(sdp.status, "infeasible",
                          "The commuting SDP is not identifying incompatible " +
                          "distributions.")
+        lp_fanout = InflationLP(self.cutInflation_c, nonfanout=False)
+        lp_fanout.set_distribution(self.GHZ(0.5 + 1e-2))
+        lp_fanout.solve()
+        self.assertEqual(lp_fanout.success, False,
+                         "The fanout LP is not identifying incompatible " +
+                         "distributions.")
+        lp_nonfanout = InflationLP(self.cutInflation_c, nonfanout=True)
+        lp_nonfanout.set_distribution(self.GHZ(0.5 + 1e-2))
+        lp_nonfanout.solve()
+        self.assertEqual(lp_nonfanout.success, False,
+                         "The nonfanout LP is not identifying incompatible " +
+                         "distributions.")
         sdp.solve(feas_as_optim=True)
         self.assertTrue(sdp.primal_objective <= 0,
                         "The commuting SDP with feasibility as optimization " +
                         "is not identifying incompatible distributions.")
         sdp.set_distribution(self.GHZ(0.5 - 1e-2))
         sdp.solve()
         self.assertEqual(sdp.status, "feasible",
                          "The commuting SDP is not recognizing compatible " +
                          "distributions.")
+        lp_fanout.set_distribution(self.GHZ(0.5 - 1e-2))
+        lp_fanout.solve()
+        self.assertEqual(lp_fanout.success, True,
+                         "The fanout LP is not recognizing compatible " +
+                         "distributions.")
+        lp_nonfanout.set_distribution(self.GHZ(0.5 - 1e-2))
+        lp_nonfanout.solve()
+        self.assertEqual(lp_nonfanout.success, True,
+                         "The nonfanout LP is not identifying incompatible " +
+                         "distributions.")
         sdp.solve(feas_as_optim=True)
         self.assertTrue(sdp.primal_objective >= 0,
                         "The commuting SDP with feasibility as optimization " +
                         "is not recognizing compatible distributions.")
 
     def test_GHZ_NC(self):
         sdp = InflationSDP(self.cutInflation)
         sdp.generate_relaxation("local1")
-        self.assertEqual(len(sdp.generating_monomials), 18,
+        self.assertEqual(sdp.n_columns, 18,
                          "The number of generating columns is not correct.")
         self.assertEqual(sdp.n_knowable, 8 + 1,  # only '1' is included here.
                          "The count of knowable moments is wrong.")
         self.assertEqual(sdp.n_unknowable, 13,
                          "The count of unknowable moments is wrong.")
 
         sdp.set_distribution(self.GHZ(0.5 + 1e-2))
-        self.assertTrue(np.isclose(sdp.known_moments[sdp.monomials[8]],
-                        (0.5+1e-2)/2 + (0.5-1e-2)/8),
+        self.assertTrue(np.isclose(sdp.known_moments[sdp.moments[8]],
+                                   (0.5+1e-2) / 2 + (0.5-1e-2) / 8),
                         "Setting the distribution is failing.")
         sdp.solve()
         self.assertTrue(sdp.status in ["infeasible", "unknown"],
                         "The non-commuting SDP is not identifying " +
                         "incompatible distributions.")
         sdp.solve(feas_as_optim=True)
         self.assertTrue(sdp.primal_objective <= 0,
                         "The NC SDP with feasibility as optimization is not " +
                         "identifying incompatible distributions.")
         sdp.set_distribution(self.GHZ(0.5 - 1e-2))
-        self.assertTrue(np.isclose(sdp.known_moments[sdp.monomials[8]],
-                        (0.5-1e-2)/2 + (0.5+1e-2)/8),
+        self.assertTrue(np.isclose(sdp.known_moments[sdp.moments[8]],
+                                   (0.5-1e-2) / 2 + (0.5+1e-2) / 8),
                         "Re-setting the distribution is failing.")
         sdp.solve()
         self.assertEqual(sdp.status, "feasible",
                          "The non-commuting SDP is not recognizing " +
                          "compatible distributions.")
         sdp.solve(feas_as_optim=True)
         self.assertTrue(sdp.primal_objective >= 0,
@@ -466,20 +570,20 @@
         self.assertTrue(np.isclose(sdp.objective_value, 0.0640776),
                         "Optimization of a simple SDP with LPI-like " +
                         "constraints is not obtaining the correct known value."
                         )
 
     def test_lpi_bounds(self):
         sdp  = InflationSDP(trivial)
-        cols = [[],
-                [[1, 2, 0, 0],
-                 [1, 2, 1, 0]],
-                [[1, 1, 0, 0],
+        cols = [np.array([]),
+                np.array([[1, 2, 0, 0],
+                 [1, 2, 1, 0]]),
+                np.array([[1, 1, 0, 0],
                  [1, 2, 0, 0],
-                 [1, 2, 1, 0]]]
+                 [1, 2, 1, 0]])]
         sdp.generate_relaxation(cols)
         sdp.set_distribution(np.ones((2, 1)) / 2,
                              use_lpi_constraints=True)
 
         self.assertGreaterEqual(len(sdp.semiknown_moments), 1,
                                 "Failing to identify semiknowns.")
 
@@ -487,24 +591,24 @@
                             for val in sdp.semiknown_moments.values()),
                         "Semiknown moments need to be of the form " +
                         "mon_index1 = (number<=1) * mon_index2, this is " +
                         "failing.")
 
     def test_new_indices(self):
         sdp  = InflationSDP(trivial)
-        cols = [[],
-                [[1, 1, 0, 0],
-                 [1, 2, 0, 0],
-                 [1, 2, 1, 0]]]
+        cols = [np.array([]),
+                np.array([[1, 1, 0, 0],
+                          [1, 2, 0, 0],
+                          [1, 2, 1, 0]])]
         sdp.generate_relaxation(cols)
         sdp.set_distribution(np.ones((2, 1)) / 2,
                              use_lpi_constraints=True)
         new_mon_indices = np.array([semi[1][1].idx
                                     for semi in sdp.semiknown_moments.items()])
-        self.assertTrue(np.all(new_mon_indices > len(sdp.monomials)),
+        self.assertTrue(np.all(new_mon_indices > len(sdp.moments)),
                         "The new unknown monomials that appear when applying" +
                         " LPI constraints are not assigned correct indices.")
 
     def test_supports(self):
         sdp = InflationSDP(self.bellScenario, supports_problem=True)
         sdp.generate_relaxation("local1")
         pr_support = np.zeros((2, 2, 2, 2))
@@ -520,14 +624,88 @@
         sdp.set_distribution(compatible_support)
         sdp.solve(feas_as_optim=False)
         self.assertEqual(sdp.status, "feasible",
                          "A feasible support for the Bell scenario is not " +
                          "being recognized as such.")
 
 
+class TestLPOutput(unittest.TestCase):
+    def test_bounds(self):
+        ub = 0.8
+        lb = 0.2
+        very_trivial = InflationProblem({"a": ["b"]}, outcomes_per_party=[2])
+        lp = InflationLP(very_trivial)
+        operator = np.asarray(lp.monomials).flatten()[1]
+        with self.subTest(msg="Setting upper bound"):
+            lp.set_objective({operator: 1}, "max")
+            lp.set_bounds({operator: ub}, "up")
+            lp.solve()
+            self.assertAlmostEqual(
+                lp.objective_value, ub,
+                msg=f"Setting upper bounds to monomials failed. The result "
+                    f"obtained for {{max x s.t. x <= {ub}}} is "
+                    f"{lp.objective_value}.")
+        with self.subTest(msg="Setting lower bound"):
+            lp.set_objective({operator: 1}, "min")
+            lp.set_bounds({operator: lb}, "lo")
+            lp.solve()
+            self.assertAlmostEqual(
+                lp.objective_value, lb,
+                msg=f"Setting lower bounds to monomials failed. The result "
+                    f"obtained for {{min x s.t. x >= {lb}}} is "
+                    f"{lp.objective_value}.")
+
+    def test_instrumental(self):
+        lp = InflationLP(TestSDPOutput.instrumental_c, nonfanout=False)
+        with self.subTest(msg="Infeasible Bonet's inequality"):
+            lp.set_distribution(TestSDPOutput.incompatible_dist)
+            lp.solve(feas_as_optim=False)
+            self.assertTrue(lp.status in ["prim_infeas_cer", "dual_infeas_cer",
+                                          "unknown"],
+                            "Failed to detect the infeasibility of the "
+                            "distribution that maximally violates Bonet's "
+                            "inequality.")
+        with self.subTest(msg="Infeasible normalization"):
+            unnormalized_dist = np.ones((2, 2, 3, 1), dtype=float)
+            lp.set_distribution(unnormalized_dist)
+            lp.solve(feas_as_optim=False)
+            self.assertTrue(lp.status in ["prim_infeas_cer", "dual_infeas_cer",
+                                          "unknown"],
+                            "Failed to detect the infeasibility of a "
+                            "distribution that violates normalization.")
+        with self.subTest(msg="Feasible instrumental"):
+            compatible_dist = unnormalized_dist / 4
+            lp.set_distribution(compatible_dist)
+            lp.solve(feas_as_optim=False)
+            self.assertEqual(lp.status, "optimal",
+                             "A feasible distribution for the instrumental "
+                             "scenario is not being recognized as such.")
+
+    def test_supports(self):
+        lp = InflationLP(TestSDPOutput.bellScenario_c, supports_problem=True,
+                         nonfanout=False)
+        with self.subTest(msg="Incompatible support"):
+            pr_support = np.zeros((2, 2, 2, 2))
+            for a, b, x, y in np.ndindex(*pr_support.shape):
+                if x*y == (a + b) % 2:
+                    pr_support[a, b, x, y] = np.random.randn()
+            lp.set_distribution(pr_support)
+            lp.solve(feas_as_optim=False)
+            self.assertIn(lp.status, ["prim_infeas_cer", "dual_infeas_cer"],
+                          "Failed to detect the infeasibility of a support "
+                          "known to be incompatible.")
+        with self.subTest(msg="Compatible support"):
+            compatible_support = np.ones((2, 2, 2, 2), dtype=float)
+            lp.set_distribution(compatible_support)
+            lp.solve(feas_as_optim=False)
+            self.assertEqual(lp.status, "optimal",
+                             "A feasible support for the Bell scenario was "
+                             "not recognized as such.")
+
+
 class TestSymmetries(unittest.TestCase):
     def test_apply_symmetries(self):
         from inflation.sdp.quantum_tools import \
                                                 apply_inflation_symmetries
         G = np.array([[0,  1,  2,  3,  4,  5],
                       [6,  7,  8,  9, 10, 11],
                       [12, 13, 14, 15, 16, 17],
@@ -555,63 +733,58 @@
                         "Orbits dictionary is not correct.")
         repr_values_good = np.array([0,  1,  2,  4,  6,  7,  8,  9, 10,
                                      12, 13, 14, 15, 16, 24, 25, 26, 28, 29])
         self.assertTrue(np.allclose(repr_values, repr_values_good),
                         "Representatives mapping is not correct.")
 
     def test_commutations_after_symmetrization(self):
-        scenario = InflationSDP(trivial, commuting=True)
-        col_structure = [[],
-                         [[1, 2, 0, 0], [1, 2, 1, 0]],
-                         [[1, 1, 0, 0], [1, 2, 0, 0]],
-                         [[1, 1, 1, 0], [1, 2, 0, 0]],
-                         [[1, 1, 0, 0], [1, 2, 1, 0]],
-                         [[1, 1, 1, 0], [1, 2, 1, 0]],
-                         [[1, 1, 0, 0], [1, 1, 1, 0]]]
+        scenario = InflationSDP(trivial_c)
+        col_structure = [np.array([]),
+                         np.array([[1, 2, 0, 0], [1, 2, 1, 0]]),
+                         np.array([[1, 1, 0, 0], [1, 2, 0, 0]]),
+                         np.array([[1, 1, 1, 0], [1, 2, 0, 0]]),
+                         np.array([[1, 1, 0, 0], [1, 2, 1, 0]]),
+                         np.array([[1, 1, 1, 0], [1, 2, 1, 0]]),
+                         np.array([[1, 1, 0, 0], [1, 1, 1, 0]])]
 
         scenario.generate_relaxation(col_structure)
-        self.assertTrue(np.array_equal(scenario.inflation_symmetries,
+        self.assertTrue(np.array_equal(scenario.columns_symmetries,
                                        [[0, 6, 2, 4, 3, 5, 1]]),
                         "The commutation relations of different copies are " +
                         "not applied properly after inflation symmetries.")
 
     def test_detected_symmetries(self):
-        cols = bilocalSDP.build_columns('local1')
-        bilocalSDP.generating_monomials = cols
-        bilocalSDP.n_columns = len(cols)
-        bilocalSDP.genmon_hash_to_index = {
-                                bilocalSDP._from_2dndarray(op): i
-                                for i, op in enumerate(cols)}
-        syms = bilocalSDP._discover_inflation_symmetries()
+        bilocalSDP.build_columns('local1')
+        syms = bilocalSDP._discover_columns_symmetries()
         # Make it a set so the order doesn't matter
         syms = set(tuple(s) for s in syms)
         # I simply copied the output at a time when we understand the code
         # to be working; this test simply detects if the code changes
-        syms_good = set(((0, 1, 2, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14,
-                          13, 16, 15, 18, 17, 20, 19, 24, 23, 22, 21, 28,
-                          27, 26, 25, 32, 31, 30, 29, 36, 35, 34, 33, 40,
-                          39, 38, 37, 44, 43, 42, 41),
-                         (0, 2, 1, 5, 6, 3, 4, 7, 8, 15, 16, 13, 14, 11,
-                          12, 9, 10, 19, 20, 17, 18, 25, 26, 27, 28, 21,
-                          22, 23, 24, 41, 42, 43, 44, 37, 38, 39, 40, 33,
-                          34, 35, 36, 29, 30, 31, 32),
-                         (0, 2, 1, 6, 5, 4, 3, 8, 7, 16, 15, 14, 13, 12,
-                          11, 10, 9, 20, 19, 18, 17, 28, 27, 26, 25, 24,
-                          23, 22, 21, 44, 43, 42, 41, 40, 39, 38, 37, 36,
-                          35, 34, 33, 32, 31, 30, 29)))
+        syms_good = {(0, 1, 2, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14,
+                      13, 16, 15, 18, 17, 20, 19, 24, 23, 22, 21, 28,
+                      27, 26, 25, 32, 31, 30, 29, 36, 35, 34, 33, 40,
+                      39, 38, 37, 44, 43, 42, 41),
+                     (0, 2, 1, 5, 6, 3, 4, 7, 8, 15, 16, 13, 14, 11,
+                      12, 9, 10, 19, 20, 17, 18, 25, 26, 27, 28, 21,
+                      22, 23, 24, 41, 42, 43, 44, 37, 38, 39, 40, 33,
+                      34, 35, 36, 29, 30, 31, 32),
+                     (0, 2, 1, 6, 5, 4, 3, 8, 7, 16, 15, 14, 13, 12,
+                      11, 10, 9, 20, 19, 18, 17, 28, 27, 26, 25, 24,
+                      23, 22, 21, 44, 43, 42, 41, 40, 39, 38, 37, 36,
+                      35, 34, 33, 32, 31, 30, 29)}
         self.assertEqual(syms, syms_good, "The symmetries are not being " +
                                           "detected correctly.")
 
 
 class TestConstraintGeneration(unittest.TestCase):
     def test_norm_eqs_mon2index_mapping(self):
         sdp = InflationSDP(InflationProblem({'r': ['A']}, (3,), (3,), (3,)))
         sdp.generate_relaxation('npa2')
-        for i, mon in enumerate(sdp.generating_monomials):
-            self.assertTrue(i == sdp.genmon_hash_to_index[mon.tobytes()],
+        for i, lexmon in enumerate(sdp.generating_monomials_1d):
+            self.assertTrue(i == sdp.genmon_1d_to_index[tuple(lexmon)],
                             "Monomials in the generating list must be mapped "
                             + "to their index in the list under "
                             + "InflationSDP.genmon_hash_to_index for "
                             + "InflationSDP._discover_normalization_eqns() "
                             + "to work correctly.")
 
     def test_norm_eqs_expansion(self):
@@ -677,7 +850,302 @@
                     (7, [6, 8]),
                     (9, [1, 10]),
                     (1, [9, 11])]
         self.assertEqual(out,
                          out_good,
                          "Column equalities are not being " +
                          "properly lifted to moment inequalities.")
+
+
+class TestPipelineLP(unittest.TestCase):
+    def _monomial_generation(self, **args):
+        with self.subTest(msg="Testing monomial generation"):
+            raw_n_columns = args["scenario"].raw_n_columns
+            truth = args["truth_columns"]
+            self.assertEqual(raw_n_columns, truth,
+                             f"There are {raw_n_columns} columns but {truth} "
+                             f"were expected.")
+
+    def _equalities(self, **args):
+        with self.subTest(msg="Testing equalities"):
+            equalities = args["scenario"].moment_equalities
+            truth = args["truth_eq"]
+            self.assertEqual(len(equalities), truth,
+                             f"There are {len(equalities)} equalities but "
+                             f"{truth} were expected.")
+            self.assertTrue(all(set(equality.values()) == {-1, 1}
+                                for equality in equalities),
+                            "Some implicit equalities lack a nontrivial "
+                            "left-hand or right-hand side.")
+
+    def _test_a_visibility(self, **args):
+        lp = args["scenario"]
+        dist_func = args["dist_func"]
+        dist_name = args["dist_name"]
+        crit_cutoff = args["crit_cutoff"]
+        with self.subTest(msg="Testing GHZ, incompatible distribution"):
+            lp.set_distribution(dist_func(crit_cutoff + 1e-2))
+            lp.solve()
+            self.assertIn(lp.status, ["prim_infeas_cer", "dual_infeas_cer",
+                                      "unknown"],
+                          "The LP did not identify the incompatible "
+                          "distribution.")
+        with self.subTest(msg=f"Testing {dist_name}, incompatible distribution, "
+                              "feasibility as optimization"):
+            lp.solve(feas_as_optim=True)
+            self.assertTrue(lp.primal_objective <= 0,
+                            "The LP with feasibility as optimization did not "
+                            "identify the incompatible distribution.")
+        with self.subTest(msg=f"Testing {dist_name}, compatible distribution"):
+            lp.set_distribution(dist_func(crit_cutoff - 1e-2))
+            lp.solve()
+            self.assertEqual(lp.status, "optimal",
+                             "The LP did not recognize the compatible "
+                             "distribution.")
+        with self.subTest(msg=f"Testing {dist_name}, compatible distribution, "
+                              "feasibility as optimization"):
+            # self.skipTest("Feasibility as optimization not working for "
+            #               "compatible distributions?")
+            lp.solve(feas_as_optim=True)
+            self.assertTrue(lp.primal_objective >= -1e-6,
+                            "The LP with feasibility as optimization did not "
+                            "recognize the compatible distribution.")
+
+    def _run(self, **args):
+        self._monomial_generation(**args)
+        self._equalities(**args)
+        self._test_a_visibility(**args)
+
+
+class TestInstrumental(TestPipelineLP):
+    instrumental = InflationProblem({"U_AB": ["A", "B"],
+                                     "A": ["B"]},
+                                    outcomes_per_party=(2, 2),
+                                    settings_per_party=(2, 1),
+                                    inflation_level_per_source=(1,),
+                                    order=("A", "B"))
+    instrumental_c = InflationProblem({"U_AB": ["A", "B"],
+                                       "A": ["B"]},
+                                      outcomes_per_party=(2, 2),
+                                      settings_per_party=(2, 1),
+                                      inflation_level_per_source=(1,),
+                                      order=("A", "B"),
+                                      classical_sources='all')
+
+    def p_Pearl_Violating(self, v):
+        dist = np.full((2, 2, 2, 1), (1 - v) / 4)
+        dist[0, 0, 0, 0] = dist[0, 1, 1, 0] = v + (1 - v) / 4
+        return dist
+
+    def test_instrumental_fanout(self):
+        inst = InflationLP(self.instrumental_c, nonfanout=False)
+        args = {"scenario": inst,
+                "truth_columns": 36,
+                "truth_eq": 20,
+                "dist_func": self.p_Pearl_Violating,
+                "dist_name": "Instrumental noisy e-sep violating",
+                "crit_cutoff": 1/3}
+        self._run(**args)
+
+    def test_instrumental_nonfanout(self):
+        inst = InflationLP(self.instrumental, nonfanout=True)
+        args = {"scenario": inst,
+                "truth_columns": 15,
+                "truth_eq": 6,
+                "dist_func": self.p_Pearl_Violating,
+                "dist_name": "Instrumental noisy e-sep violating",
+                "crit_cutoff": 1/3}
+        self._run(**args)
+
+
+class TestBell(TestPipelineLP):
+    bellScenario = InflationProblem({"Lambda": ["A", "B"]},
+                                    outcomes_per_party=[2, 2],
+                                    settings_per_party=[2, 2],
+                                    inflation_level_per_source=[1])
+    bellScenario_c = InflationProblem({"Lambda": ["A", "B"]},
+                                      outcomes_per_party=[2, 2],
+                                      settings_per_party=[2, 2],
+                                      inflation_level_per_source=[1],
+                                      classical_sources='all')
+
+    def _CHSH(self, **args):
+        lp = args["scenario"]
+        truth = args["truth_obj"]
+        lp.set_objective({1: 2.0,
+                          "pA(0|0)": -4.0,
+                          "pB(0|0)": -4.0,
+                          "pAB(00|11)": -4.0,
+                          "pAB(00|00)": 4.0,
+                          "pAB(00|01)": 4.0,
+                          "pAB(00|10)": 4.0}, "max")
+        with self.subTest(msg="Testing max CHSH"):
+            lp.solve()
+            self.assertAlmostEqual(lp.objective_value, truth,
+                                   msg=f"The LP is not recovering max(CHSH) = "
+                                       f"{truth}.")
+        # Biased CHSH?
+
+    def p_Signalling_to_Bob(self, v):
+        dist = np.full((2, 2, 2, 2), (1 - v) / 4)
+        dist[0, 0, 0, 0] = dist[0, 1, 1, 0] = v + (1 - v) / 4
+        return dist
+
+    def test_bell_fanout(self):
+        bell = InflationLP(self.bellScenario_c, nonfanout=False)
+        args = {"scenario": bell,
+                "truth_columns": 16,
+                "truth_obj": 2,
+                "truth_eq": 0,
+                "dist_func": self.p_Signalling_to_Bob,
+                "dist_name": "Noisy Signalling to Bob",
+                "crit_cutoff": 0.2}
+        self._run(**args)
+        # self._CHSH(**args)
+
+    def test_bell_nonfanout(self):
+        bell = InflationLP(self.bellScenario, nonfanout=True)
+        args = {"scenario": bell,
+                "truth_columns": 9,
+                "truth_obj": 2,
+                "truth_eq": 0,
+                "dist_func": self.p_Signalling_to_Bob,
+                "dist_name": "Noisy Signalling to Bob",
+                "crit_cutoff": 0.2}
+        self._run(**args)
+        # self._CHSH(**args)
+
+
+class TestTriangle(TestPipelineLP):
+    triangle = InflationProblem({"lambda": ["a", "b"],
+                                 "mu": ["b", "c"],
+                                 "sigma": ["a", "c"]},
+                                outcomes_per_party=[2, 2, 2],
+                                settings_per_party=[1, 1, 1],
+                                inflation_level_per_source=[1, 1, 1],
+                                order=['a', 'b', 'c'])
+
+    def GHZ(self, v):
+        dist = np.zeros((2, 2, 2, 1, 1, 1))
+        dist[0, 0, 0] = dist[1, 1, 1] = 1 / 2
+        return v * dist + (1 - v) / 8
+
+    def test_triangle_fanout(self):
+        triangle = InflationLP(self.triangle, nonfanout=False)
+        args = {"scenario": triangle,
+                "truth_columns": 8,
+                "truth_eq": 0,
+                "dist_func": self.GHZ,
+                "dist_name": "Noisy GHZ",
+                "crit_cutoff": 1}
+        self._run(**args)
+
+    def test_triangle_nonfanout(self):
+        triangle = InflationLP(self.triangle, nonfanout=True)
+        args = {"scenario": triangle,
+                "truth_columns": 8,
+                "truth_eq": 0,
+                "dist_func": self.GHZ,
+                "dist_name": "Noisy GHZ",
+                "crit_cutoff": 1}
+        self._run(**args)
+
+
+class TestEvans(TestPipelineLP):
+    evans = InflationProblem({"U_AB": ["A", "B"],
+                              "U_BC": ["B", "C"],
+                              "B": ["A", "C"]},
+                             outcomes_per_party=(2, 2, 2),
+                             settings_per_party=(1, 1, 1),
+                             inflation_level_per_source=(1, 1),
+                             order=("A", "B", "C"))
+    evans_c = InflationProblem({"U_AB": ["A", "B"],
+                                "U_BC": ["B", "C"],
+                                "B": ["A", "C"]},
+                               outcomes_per_party=(2, 2, 2),
+                               settings_per_party=(1, 1, 1),
+                               inflation_level_per_source=(1, 1),
+                               order=("A", "B", "C"),
+                               classical_sources='all')
+
+    def p_Evans_esep_violating(self, v):
+        dist = np.zeros((2, 2, 2, 1, 1, 1))
+        for x, y, z in product(range(2), repeat=3):
+            dist[x, y, z] = (1 + v * (-1) ** (x + y + y * z)) / 8
+        return dist
+
+    def test_evans_fanout(self):
+        evans = InflationLP(self.evans_c, nonfanout=False)
+        args = {"scenario": evans,
+                "truth_columns": 48,
+                "truth_eq": 16,
+                "dist_func": self.p_Evans_esep_violating,
+                "dist_name": "Noisy Evans Incompatible",
+                "crit_cutoff": 1}
+        self._run(**args)
+
+    def test_evans_nonfanout(self):
+        evans = InflationLP(self.evans, nonfanout=True)
+        args = {"scenario": evans,
+                "truth_columns": 27,
+                "truth_eq": 9,
+                "dist_func": self.p_Evans_esep_violating,
+                "dist_name": "Noisy Evans Incompatible",
+                "crit_cutoff": 1}
+        self._run(**args)
+        
+
+class TestFullNN(TestPipelineLP):
+    scenario = InflationProblem({'lambda': ['A', 'B'],
+                                     'NS': ['B', 'C']},
+                                [2, 4, 2], [3, 1, 3], 
+                                inflation_level_per_source=[1, 2],
+                                classical_sources=['lambda'],)
+
+    def _prob_EJM(self, v, theta=0):
+        p_bell = np.expand_dims((0, 1, -1, 0), axis=1)/np.sqrt(2)
+        rho_v = v * p_bell @ p_bell.conj().T + (1 - v) * np.eye(4)/4
+        sigmax = np.array([[0, 1], [1, 0]])
+        sigmay = np.array([[0, -1j], [1j, 0]])
+        sigmaz = np.array([[1, 0], [0, -1]])
+        A = [[np.expand_dims(v, axis=1) @ np.expand_dims(v, axis=1).conj().T 
+                for v in reversed(np.linalg.eigh(op)[1].T)] 
+                for op in [sigmax, sigmay, sigmaz]]
+        C = [[np.expand_dims(v, axis=1) @ np.expand_dims(v, axis=1).conj().T 
+                for v in reversed(np.linalg.eigh(op)[1].T)] 
+                for op in [sigmax, sigmay, sigmaz]]
+        r_plus = (1 + np.exp(1j*theta))/np.sqrt(2)
+        r_minus = (1 - np.exp(1j*theta))/np.sqrt(2)
+        e00 = np.expand_dims([1, 0, 0, 0], axis=1)
+        e01 = np.expand_dims([0, 1, 0, 0], axis=1)
+        e10 = np.expand_dims([0, 0, 1, 0], axis=1)
+        e11 = np.expand_dims([0, 0, 0, 1], axis=1)
+        psi1 = 1/2 * (np.exp(-1j*np.pi/4)*e00 - r_plus * e01 
+                        - r_minus * e10 + np.exp(-3/4*np.pi*1j)*e11)
+        psi2 = 1/2 * (np.exp(1j*np.pi/4)*e00 + r_minus * e01 
+                        + r_plus * e10 + np.exp(3/4*np.pi*1j)*e11)
+        psi3 = 1/2 * (np.exp(-1j*np.pi*3/4)*e00 + r_minus * e01 
+                        + r_plus * e10 + np.exp(-1/4*np.pi*1j)*e11)
+        psi4 = 1/2 * (np.exp(1j*np.pi*3/4)*e00 - r_plus * e01 
+                        - r_minus * e10 + np.exp(np.pi*1j/4)*e11)
+        B = [ [psi @ psi.conj().T for psi in [psi1, psi2, psi3, psi4] ]]
+        
+        p = np.zeros((2, 4, 2, 3, 1, 3))
+        state = np.kron(rho_v, rho_v)
+        for a, b, c, x, y, z in np.ndindex(p.shape):
+            mmnt = np.kron(np.kron(A[x][a], B[y][b]), C[z][c])
+            p[a, b, c, x, y, z] = np.real(np.trace(state @ mmnt))
+        return p
+    
+    def test_fullnetworknonlocality_3partite_line(self):
+        lp = InflationLP(self.scenario, nonfanout=True)
+        
+        best_theta = np.arccos(np.sqrt(5) / 3)
+        v_for_best_theta = 2 / np.sqrt(5)
+        
+        args = {"scenario": lp,
+                "truth_columns": 2048,
+                "truth_eq": 0,
+                "dist_func": lambda x: self._prob_EJM(x, theta=best_theta),
+                "dist_name": "Noisy EJM",
+                "crit_cutoff": v_for_best_theta}
+        self._run(**args)
```

