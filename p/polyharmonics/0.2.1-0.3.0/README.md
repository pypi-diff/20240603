# Comparing `tmp/polyharmonics-0.2.1.tar.gz` & `tmp/polyharmonics-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyharmonics-0.2.1.tar", max compression
+gzip compressed data, was "polyharmonics-0.3.0.tar", max compression
```

## Comparing `polyharmonics-0.2.1.tar` & `polyharmonics-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0     1466 2024-04-16 13:33:46.000000 polyharmonics-0.2.1/LICENSE
--rwxr-xr-x   0        0        0     5766 2024-05-06 13:47:41.571445 polyharmonics-0.2.1/README.md
--rwxr-xr-x   0        0        0      459 2024-05-04 15:40:05.000000 polyharmonics-0.2.1/polyharmonics/__init__.py
--rwxr-xr-x   0        0        0     1075 2024-05-06 13:28:42.421280 polyharmonics-0.2.1/polyharmonics/__main__.py
--rwxr-xr-x   0        0        0     7357 2024-05-10 19:01:36.870299 polyharmonics-0.2.1/polyharmonics/associated_legendre_functions.py
--rwxr-xr-x   0        0        0      209 2024-05-06 13:28:42.418277 polyharmonics-0.2.1/polyharmonics/cli/__init__.py
--rwxr-xr-x   0        0        0     5707 2024-05-06 13:28:42.427725 polyharmonics-0.2.1/polyharmonics/cli/associated_legendre_cmd.py
--rwxr-xr-x   0        0        0      190 2024-05-06 13:28:42.418225 polyharmonics-0.2.1/polyharmonics/cli/benchmark/__init__.py
--rwxr-xr-x   0        0        0    13006 2024-05-06 13:41:16.581886 polyharmonics-0.2.1/polyharmonics/cli/benchmark/associated_legendre_bench.py
--rwxr-xr-x   0        0        0     5553 2024-05-06 13:41:16.580068 polyharmonics-0.2.1/polyharmonics/cli/benchmark/legendre_bench.py
--rwxr-xr-x   0        0        0      650 2024-05-06 13:28:42.421780 polyharmonics-0.2.1/polyharmonics/cli/benchmark_cmd.py
--rwxr-xr-x   0        0        0      183 2024-05-04 16:25:21.000000 polyharmonics-0.2.1/polyharmonics/cli/colors.py
--rwxr-xr-x   0        0        0     3456 2024-05-06 13:28:42.423962 polyharmonics-0.2.1/polyharmonics/cli/legendre_cmd.py
--rwxr-xr-x   0        0        0     4957 2024-05-06 13:37:17.743809 polyharmonics-0.2.1/polyharmonics/legendre_polynomials.py
--rwxr-xr-x   0        0        0     3462 2024-05-10 18:59:45.448988 polyharmonics-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7296 1970-01-01 00:00:00.000000 polyharmonics-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1466 2024-05-28 09:53:16.724673 polyharmonics-0.3.0/LICENSE
+-rwxr-xr-x   0        0        0     5448 2024-05-28 09:53:16.726662 polyharmonics-0.3.0/README.md
+-rwxr-xr-x   0        0        0      459 2024-05-28 09:53:16.734155 polyharmonics-0.3.0/polyharmonics/__init__.py
+-rwxr-xr-x   0        0        0     1075 2024-05-28 09:53:16.735045 polyharmonics-0.3.0/polyharmonics/__main__.py
+-rwxr-xr-x   0        0        0    10151 2024-06-02 23:31:37.850882 polyharmonics-0.3.0/polyharmonics/associated_legendre_functions.py
+-rwxr-xr-x   0        0        0      209 2024-05-06 13:28:42.418277 polyharmonics-0.3.0/polyharmonics/cli/__init__.py
+-rwxr-xr-x   0        0        0     5531 2024-06-02 23:16:32.408114 polyharmonics-0.3.0/polyharmonics/cli/associated_legendre_cmd.py
+-rwxr-xr-x   0        0        0      190 2024-05-06 13:28:42.418225 polyharmonics-0.3.0/polyharmonics/cli/benchmark/__init__.py
+-rwxr-xr-x   0        0        0     7982 2024-06-02 23:28:49.471530 polyharmonics-0.3.0/polyharmonics/cli/benchmark/associated_legendre_bench.py
+-rwxr-xr-x   0        0        0     7405 2024-06-02 23:31:37.849910 polyharmonics-0.3.0/polyharmonics/cli/benchmark/legendre_bench.py
+-rwxr-xr-x   0        0        0      650 2024-05-06 13:28:42.421780 polyharmonics-0.3.0/polyharmonics/cli/benchmark_cmd.py
+-rwxr-xr-x   0        0        0      183 2024-05-04 16:25:21.000000 polyharmonics-0.3.0/polyharmonics/cli/colors.py
+-rwxr-xr-x   0        0        0     3739 2024-06-02 23:11:24.165368 polyharmonics-0.3.0/polyharmonics/cli/legendre_cmd.py
+-rwxr-xr-x   0        0        0     5913 2024-06-02 11:25:26.857381 polyharmonics-0.3.0/polyharmonics/legendre_polynomials.py
+-rwxr-xr-x   0        0        0     3421 2024-06-02 23:35:25.549472 polyharmonics-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6926 1970-01-01 00:00:00.000000 polyharmonics-0.3.0/PKG-INFO
```

### Comparing `polyharmonics-0.2.1/LICENSE` & `polyharmonics-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.1/README.md` & `polyharmonics-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -93,33 +93,14 @@
 
 > Note: `check-codestyle` uses `ruff` and `darglint` library
 
 </p>
 </details>
 
 <details>
-<summary>Code security</summary>
-<p>
-
-> If this command is not selected during installation, it cannnot be used.
-
-```bash
-make check-safety
-```
-
-This command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.
-
-```bash
-make check-safety
-```
-
-</p>
-</details>
-
-<details>
 <summary>Tests with coverage badges</summary>
 <p>
 
 Run `pytest`
 
 ```bash
 make test
```

### Comparing `polyharmonics-0.2.1/polyharmonics/__main__.py` & `polyharmonics-0.3.0/polyharmonics/__main__.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.1/polyharmonics/cli/associated_legendre_cmd.py` & `polyharmonics-0.3.0/polyharmonics/cli/associated_legendre_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         "-p",
         "--polar",
         case_sensitive=False,
         help="Calculate the function(s) with polar coordinates.",
     ),
     evaluate: str = typer.Option(
         None,
-        "-x",
         "--eval",
         case_sensitive=False,
         help="""Print the function(s) evaluated on the given numbers.
         Either a number or a comma-separated list of numbers.""",
     ),
     color: Optional[Color] = typer.Option(
         Color.white,
@@ -58,14 +57,19 @@
         "--time",
         case_sensitive=False,
         help="Display the time taken to calculate the function(s).",
     ),
 ) -> None:
     """Calculate and print the associated Legendre function(s)."""
 
+    if print_latex and evaluate:
+        raise typer.BadParameter(
+            "Cannot use both '--print_latex' and '--eval' at the same time."
+        )
+
     # Convert the input to two lists of integers
     try:
         n_values = []
         m_values = []
         for value in nm.split(","):
             n, m = value.split(":")
             if n is None or m is None or n == "" or m == "":
@@ -95,65 +99,62 @@
                 "x must either be a number or a list of numbers separated by commas."
             )
 
     if display_time:
         t_start = time()
 
     # Calculate the Associated Legendre function(s)
+
     with console.status(
         status=(
             "[yellow1]Calculating associated Legendre functions.[/]"
             if len(n_values) > 1
             else "[yellow1]Calculating associated Legendre function.[/]"
         ),
         spinner="dots",
     ):
-        result: List[Expr] = [
-            associated_legendre(i, j, polar=polar) for i, j in zip(n_values, m_values)
-        ]
+        if x_values:
+            result: List[List[float]] = [
+                [associated_legendre(i, j, polar=polar, eval=x) for x in x_values]
+                for i, j in zip(n_values, m_values)
+            ]
+        else:
+            result: List[Expr] = [
+                associated_legendre(i, j, polar=polar) for i, j in zip(n_values, m_values)
+            ]
 
     if display_time:
         t_end = time()
         console.print(
             f"[bold green1]Done! [/][bold]Time taken: {t_end - t_start:.6f} seconds[/]\n"  # noqa: E501
         )
 
     for n, m, fun in zip(n_values, m_values, result):
         if print_latex:
             if polar:
-                console.print(f"[bold {color}]P_{n}^{m}(x) = {latex(fun)}[/]\n")
-            else:
                 console.print(f"[bold {color}]P_{n}^{m}(cos(θ)) = {latex(fun)}[/]\n")
+            else:
+                console.print(f"[bold {color}]P_{n}^{m}(x) = {latex(fun)}[/]\n")
+        elif x_values:
+            for i, x in enumerate(x_values):
+                if polar:
+                    console.print(
+                        f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}(cos({x})) = {fun[i]}[/]\n"  # noqa: E501
+                    )
+                else:
+                    console.print(
+                        f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}({x}) = {fun[i]}[/]\n"  # noqa: E501
+                    )
         else:
             if polar:
                 console.print(
                     f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}(cos(θ)) = [/]"  # noqa: E501
                 )
             else:
                 console.print(
                     f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}(x) = [/]"  # noqa: E501
                 )
             console.print(
                 f"[bold {color}] {pretty(fun)}[/]\n",
             )
-        if x_values:
-            for x in x_values:
-                if abs(x) != 1:
-                    if polar:
-                        console.print(
-                            f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}({x}) = {fun.subs(th, acos(x))}[/]\n"  # noqa: E501
-                        )
-                    else:
-                        console.print(
-                            f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}({x}) = {fun.subs(X, x)}[/]\n"  # noqa: E501
-                        )
-                else:
-                    if polar:
-                        console.print(
-                            f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}({x}) = {limit(fun, th, acos(x))}[/]\n"  # noqa: E501
-                        )
-                    else:
-                        console.print(
-                            f"[bold {color}]P{str(n).translate(SUB)}{str(m).translate(SUP)}({x}) = {limit(fun, X, x)}[/]\n"  # noqa: E501
-                        )
 
     raise typer.Exit()
```

### Comparing `polyharmonics-0.2.1/polyharmonics/cli/benchmark/legendre_bench.py` & `polyharmonics-0.3.0/polyharmonics/cli/benchmark/legendre_bench.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import time
+from csv import writer
 from multiprocessing import Process
 
 import typer
-from prettytable import PrettyTable
 from rich.console import Console
 from rich.status import Status
+from tabulate import tabulate
 
 from polyharmonics.legendre_polynomials import (
     legendre_def,
+    legendre_exp,
     legendre_rec,
     legendre_store,
 )
 
 SUB = str.maketrans("0123456789", "₀₁₂₃₄₅₆₇₈₉")
 console = Console()
 
@@ -19,14 +21,20 @@
 def legendre_bench_command(
     n: str = typer.Argument(
         ...,
         help="""Calculate the Legendre polynomials from 0 to the given degree.
         An integer or a comma-separated list of integers.""",
         metavar="DEGREE",
     ),
+    eval: float = typer.Option(
+        None,
+        "--eval",
+        case_sensitive=False,
+        help="Evaluate the polynomials on the given number.",
+    ),
     max_time: float = typer.Option(
         60.0,
         "--max-time",
         case_sensitive=False,
         help="Maximum execution time in seconds for each calculation. Default is 60 seconds.",  # noqa: E501
     ),
     csv: str = typer.Option(
@@ -49,65 +57,80 @@
     except ValueError:
         raise typer.BadParameter(
             "n must be an integer or a comma-separated list of integers."  # noqa: E501
         )
 
     with console.status(status="", spinner="dots") as status:
         status: Status
-        table = PrettyTable()
-        n_tests = 4
-        table.field_names = [
+        table = []
+        n_tests = 5
+        headers = [
             "N",
             "Definition w storage",
             "Definition w/o storage",
             "Recursion w storage",
             "Recursion w/o storage",
+            "Expression",
         ]
 
         # List for each test to indicate if it timed out
         timed_out = [False for _ in range(n_tests)]
         for i in n_values:
             # List of tests to run for each n of n_values
             tests = [
                 {
                     "fun": calculate_legendre,
-                    "args": (i, True, True),
+                    "args": (i, eval, True, True),
                     "text": (
-                        "Calculating all Legendre polynomials "
-                        f"from P{str(0).translate(SUB)}(x) to P{str(i).translate(SUB)}(x) "
+                        f"{'Calculating' if eval is None else 'Evaluating'} all Legendre polynomials "  # noqa: E501
+                        f"from P{str(0).translate(SUB)}({'x' if eval is None else eval}) "
+                        f"to P{str(i).translate(SUB)}({'x' if eval is None else eval}) "
                         "with definition and storage."
                     ),
                 },
                 {
                     "fun": calculate_legendre,
-                    "args": (i, True, False),
+                    "args": (i, eval, True, False),
                     "text": (
-                        "Calculating all Legendre polynomials "
-                        f"from P{str(0).translate(SUB)}(x) to P{str(i).translate(SUB)}(x) "
+                        f"{'Calculating' if eval is None else 'Evaluating'} all Legendre polynomials "  # noqa: E501
+                        f"from P{str(0).translate(SUB)}({'x' if eval is None else eval}) "
+                        f"to P{str(i).translate(SUB)}({'x' if eval is None else eval}) "
                         "with definition but no storage."
                     ),
                 },
                 {
                     "fun": calculate_legendre,
-                    "args": (i, False, True),
+                    "args": (i, eval, False, True),
                     "text": (
-                        "Calculating all Legendre polynomials "
-                        f"from P{str(0).translate(SUB)}(x) to P{str(i).translate(SUB)}(x) "
+                        f"{'Calculating' if eval is None else 'Evaluating'} all Legendre polynomials "  # noqa: E501
+                        f"from P{str(0).translate(SUB)}({'x' if eval is None else eval}) "
+                        f"to P{str(i).translate(SUB)}({'x' if eval is None else eval}) "
                         "with recursion and storage."
                     ),
                 },
                 {
                     "fun": calculate_legendre,
-                    "args": (i, False, False),
+                    "args": (i, eval, False, False),
                     "text": (
-                        "Calculating all Legendre polynomials "
-                        f"from P{str(0).translate(SUB)}(x) to P{str(i).translate(SUB)}(x) "
+                        f"{'Calculating' if eval is None else 'Evaluating'} all Legendre polynomials "  # noqa: E501
+                        f"from P{str(0).translate(SUB)}({'x' if eval is None else eval}) "
+                        f"to P{str(i).translate(SUB)}({'x' if eval is None else eval}) "
                         "with recursion but no storage."
                     ),
                 },
+                {
+                    "fun": calculate_legendre_exp,
+                    "args": (i, eval),
+                    "text": (
+                        f"{'Calculating' if eval is None else 'Evaluating'} all Legendre polynomials "  # noqa: E501
+                        f"from P{str(0).translate(SUB)}({'x' if eval is None else eval}) "
+                        f"to P{str(i).translate(SUB)}({'x' if eval is None else eval}) "
+                        "with the expression."
+                    ),
+                },
             ]
             assert len(tests) == n_tests
             row = [i]
             for n_test, test in enumerate(tests):
                 status.update(f"[yellow1]{test['text']}[/]")
                 if timed_out[n_test]:
                     row.append("TIMEOUT")
@@ -119,32 +142,50 @@
                         if time.time() - t_start > max_time:
                             legendre_calc.terminate()
                             row.append("TIMEOUT")
                             timed_out[n_test] = True
                             break
 
                     if len(row) == n_test + 1:
-                        row.append(time.time() - t_start)
+                        row.append(round(time.time() - t_start, 6))
 
-            table.add_row(row)
+            table.append(row)
 
     if csv is None:
-        console.print("[bold green]LEGENDRE POLYNOMIALS UP TO N[/]")
-        console.print(table)
+        console.print(
+            "[bold green]LEGENDRE POLYNOMIALS UP TO N[/]"
+            + f"[bold green] EVALUATED ON x = {eval}[/]"
+            if eval is not None
+            else ""
+        )
+        console.print(
+            tabulate(
+                table,
+                headers,
+                tablefmt="fancy_grid",
+                maxheadercolwidths=[None] + [12 for _ in range(n_tests)],
+            )
+        )
     else:
-        # Open the file in binary mode to avoid having multiple newlines
-        with open(csv + ".csv", "wb") as f:
-            f.write(table.get_csv_string().encode("utf-8"))
+        with open(csv + ".csv", "w") as f:
+            csv_writer = writer(f)
+            csv_writer.writerow(headers)
+            for row in table:
+                csv_writer.writerow(row)
 
     raise typer.Exit()
 
 
-def calculate_legendre(n: int, use_legendre_def: bool, store: bool):
+def calculate_legendre(n: int, eval: float | None, use_legendre_def: bool, store: bool):
     if store:
         # Reset the store to avoid following calculations to be faster than expected
         legendre_store.reset(definition=use_legendre_def, recursion=not use_legendre_def)
-    values = range(n + 1)
-    for i in values:
+    for i in range(n + 1):
         if use_legendre_def:
-            legendre_def(i, store=store)
+            legendre_def(i, eval=eval, store=store)
         else:
-            legendre_rec(i, store=store)
+            legendre_rec(i, eval=eval, store=store)
+
+
+def calculate_legendre_exp(n: int, eval: float | None):
+    for i in range(n + 1):
+        legendre_exp(i, eval=eval)
```

### Comparing `polyharmonics-0.2.1/polyharmonics/cli/benchmark_cmd.py` & `polyharmonics-0.3.0/polyharmonics/cli/benchmark_cmd.py`

 * *Files identical despite different names*

### Comparing `polyharmonics-0.2.1/polyharmonics/cli/legendre_cmd.py` & `polyharmonics-0.3.0/polyharmonics/cli/legendre_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from time import time
 from typing import List, Optional
 
 import typer
 from rich.console import Console
-from sympy import Expr, Symbol, latex, pretty
+from sympy import Expr, latex, pretty
 
 from polyharmonics import legendre
 
 from .colors import Color
 
 SUB = str.maketrans("0123456789", "₀₁₂₃₄₅₆₇₈₉")
-X = Symbol("x")
 console = Console()
 
 
 def legendre_command(
     n: str = typer.Argument(
         ...,
         help="""The degree of the polynomial(s).
@@ -26,15 +25,14 @@
         "-l",
         "--latex",
         case_sensitive=False,
         help="Print the polynomial(s) in LaTeX format.",
     ),
     evaluate: str = typer.Option(
         None,
-        "-x",
         "--eval",
         case_sensitive=False,
         help="""Print the polynomial(s) evaluated on the given numbers.
         Either a number or a comma-separated list of numbers.""",
     ),
     color: Optional[Color] = typer.Option(
         Color.white,
@@ -49,14 +47,19 @@
         "--time",
         case_sensitive=False,
         help="Display the time taken to calculate the function(s).",
     ),
 ) -> None:
     """Calculate and print the Legendre polynomial(s)."""
 
+    if print_latex and evaluate:
+        raise typer.BadParameter(
+            "Cannot use both '--print_latex' and '--eval' at the same time."
+        )
+
     # Convert the input to a list of integers
     try:
         n_values = [int(value) for value in n.split(",")]
         if any(i < 0 for i in n_values):
             raise typer.BadParameter("All integers must be greater or equal to 0.")
     except ValueError:
         raise typer.BadParameter(
@@ -85,28 +88,33 @@
         status=(
             "[yellow1]Calculating Legendre polynomials.[/]"
             if len(n_values) > 1
             else "[yellow1]Calculating Legendre polynomial.[/]"
         ),
         spinner="dots",
     ):
-        result: List[Expr] = [legendre(i) for i in n_values]
+        if x_values:
+            result: List[List[float]] = [
+                [legendre(i, x) for x in x_values] for i in n_values
+            ]
+        else:
+            result: List[Expr] = [legendre(i) for i in n_values]
 
     if display_time:
         t_end = time()
         console.print(
             f"[bold green1]Done! [/][bold]Time taken: {t_end - t_start:.6f} seconds[/]\n"  # noqa: E501
         )
 
     for n, pol in zip(n_values, result):
         if print_latex:
             console.print(f"[bold {color}]P_{n}(x) = {latex(pol)}[/]\n")
+        elif x_values:
+            for i, x in enumerate(x_values):
+                console.print(
+                    f"[bold {color}]P{str(n).translate(SUB)}({x}) = {pol[i]}[/]\n"
+                )
         else:
             console.print(f"[bold {color}]P{str(n).translate(SUB)}(x) = [/]")
             console.print(f"[bold {color}] {pretty(pol)}[/]\n")
-        if x_values:
-            for x in x_values:
-                console.print(
-                    f"[bold {color}]P{str(n).translate(SUB)}({x}) = {pol.subs(X, x)}[/]\n"  # noqa: E501
-                )
 
     raise typer.Exit()
```

### Comparing `polyharmonics-0.2.1/pyproject.toml` & `polyharmonics-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polyharmonics"
-version = "0.2.1"
+version = "0.3.0"
 description = "Ortogonal polynomials in the unit sphere"
 readme = "README.md"
 authors = [
   "Iván Salido Cobo <isalidocobo@gmail.com>",
 ]
 license = "BSD-3-Clause"
 repository = "https://github.com/ComicIvans/polyharmonics"
@@ -35,39 +35,39 @@
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Scientific/Engineering :: Mathematics",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "polyharmonics" = "polyharmonics.__main__:app"
 
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 matplotlib = "^3.8.4"
 sympy = "^1.12"
 rich = "^13.7.1"
 typer = "^0.12.3"
 numpy = "^1.26.4"
-prettytable = "^3.10.0"
+tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.1.1"
+pytest = "^8.2.1"
 pytest-html = "^4.1.1"
 pytest-cov = "^5.0.0"
 bandit = "^1.7.1"
 ruff = "^0.4.1"
-pre-commit = "^3.5.0"
+pre-commit = "^3.7.1"
 coverage = "^7.4.4"
 coverage-badge = "^1.1.0"
 
 
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/settings/
@@ -77,15 +77,14 @@
 # https://beta.ruff.rs/docs/rules/
 lint.select = ["E", "W", "F", "I"]
 lint.extend-select = ["I"]
 lint.ignore = ["F401"]
 
 # Exclude a variety of commonly ignored directories.
 respect-gitignore = true
-lint.ignore-init-module-imports = true
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".git-rewrite",
     ".hg",
```

### Comparing `polyharmonics-0.2.1/PKG-INFO` & `polyharmonics-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: polyharmonics
-Version: 0.2.1
+Version: 0.3.0
 Summary: Ortogonal polynomials in the unit sphere
 Home-page: https://github.com/ComicIvans/polyharmonics
 License: BSD-3-Clause
 Keywords: python,polynomials,unit sphere,orthogonal polynomials,mathematics,math,legendre polynomials,associated legendre functions,spherical harmonics
 Author: Iván Salido Cobo
 Author-email: isalidocobo@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: prettytable (>=3.10.0,<4.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sympy (>=1.12,<2.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Repository, https://github.com/ComicIvans/polyharmonics
 Description-Content-Type: text/markdown
 
 # Polyharmonics
 
 <div align="center">
@@ -126,33 +125,14 @@
 
 > Note: `check-codestyle` uses `ruff` and `darglint` library
 
 </p>
 </details>
 
 <details>
-<summary>Code security</summary>
-<p>
-
-> If this command is not selected during installation, it cannnot be used.
-
-```bash
-make check-safety
-```
-
-This command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.
-
-```bash
-make check-safety
-```
-
-</p>
-</details>
-
-<details>
 <summary>Tests with coverage badges</summary>
 <p>
 
 Run `pytest`
 
 ```bash
 make test
```

