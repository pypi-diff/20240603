# Comparing `tmp/process_plot-0.2.1.tar.gz` & `tmp/process_plot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process_plot-0.2.1.tar", last modified: Tue Sep 21 14:15:27 2021, max compression
+gzip compressed data, was "process_plot-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `process_plot-0.2.1.tar` & `process_plot-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 14:15:27.523805 process_plot-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-09-21 14:15:23.000000 process_plot-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-21 14:15:23.000000 process_plot-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2021-09-21 14:15:27.527805 process_plot-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2021-09-21 14:15:23.000000 process_plot-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 14:15:27.523805 process_plot-0.2.1/process_plot/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-09-21 14:15:23.000000 process_plot-0.2.1/process_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-09-21 14:15:23.000000 process_plot-0.2.1/process_plot/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6325 2021-09-21 14:15:23.000000 process_plot-0.2.1/process_plot/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-21 14:15:27.523805 process_plot-0.2.1/process_plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2021-09-21 14:15:27.000000 process_plot-0.2.1/process_plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-09-21 14:15:27.000000 process_plot-0.2.1/process_plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-21 14:15:27.000000 process_plot-0.2.1/process_plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-09-21 14:15:27.000000 process_plot-0.2.1/process_plot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-09-21 14:15:27.000000 process_plot-0.2.1/process_plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-21 14:15:27.000000 process_plot-0.2.1/process_plot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-09-21 14:15:23.000000 process_plot-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-09-21 14:15:27.527805 process_plot-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-21 14:15:23.000000 process_plot-0.2.1/setup.py
+-rw-r--r--   0        0        0       66 2024-06-03 10:47:46.314247 process_plot-0.3.0/.gitattributes
+-rw-r--r--   0        0        0      598 2024-06-03 10:47:46.314247 process_plot-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1964 2024-06-03 10:47:46.314247 process_plot-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1328 2024-06-03 10:47:46.314247 process_plot-0.3.0/.gitignore
+-rw-r--r--   0        0        0      294 2024-06-03 10:47:46.314247 process_plot-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1069 2024-06-03 10:47:46.314247 process_plot-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2798 2024-06-03 10:47:46.314247 process_plot-0.3.0/README.md
+-rw-r--r--   0        0        0    25559 2024-06-03 10:47:46.314247 process_plot-0.3.0/example.png
+-rw-r--r--   0        0        0      121 2024-06-03 10:47:46.314247 process_plot-0.3.0/process_plot/__init__.py
+-rw-r--r--   0        0        0     5665 2024-06-03 10:47:46.314247 process_plot-0.3.0/process_plot/api.py
+-rw-r--r--   0        0        0     6327 2024-06-03 10:47:46.314247 process_plot-0.3.0/process_plot/cli.py
+-rw-r--r--   0        0        0     1684 2024-06-03 10:47:46.314247 process_plot-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1707 2024-06-03 10:47:46.314247 process_plot-0.3.0/tests/test_basic.py
+-rw-r--r--   0        0        0      123 2024-06-03 10:47:46.314247 process_plot-0.3.0/tox.ini
+-rw-r--r--   0        0        0     3648 1970-01-01 00:00:00.000000 process_plot-0.3.0/PKG-INFO
```

### Comparing `process_plot-0.2.1/LICENSE` & `process_plot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `process_plot-0.2.1/PKG-INFO` & `process_plot-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,98 @@
 Metadata-Version: 2.1
 Name: process_plot
-Version: 0.2.1
+Version: 0.3.0
 Summary: Create plots of memory usage for a process.
-Home-page: https://github.com/chrisjsewell/process-plot
-Author: Chris Sewell
-License: MIT
-Description: # process-plot
-        
-        [![Build Status][ci-badge]][ci-link]
-        [![codecov.io][cov-badge]][cov-link]
-        [![PyPI version][pypi-badge]][pypi-link]
-        
-        Create plots of resource usage for a process (memory, CPU, etc).
-        
-        Process statistics are polled at a set interval, in a cross-platform manner (i.e. supports Linux, OSX and Windows).
-        
-        ## Usage
-        
-        Install the package with [pip](https://pip.pypa.io) or [pipx](https://github.com/pypa/pipx):
-        
-        ```console
-        $ pipx install process-plot
-        ```
-        
-        then run:
-        
-        ```console
-        $ pplot exec -i 0.1 "sleep 1"
-        PPLOT INFO: Output files will be written to: /user/pplot_out, with basename: 20210921125420
-        PPLOT INFO: Running process as PID: 5379
-        PPLOT INFO: Total run time: 0 hour(s), 00 minute(s), 01.034680 second(s)
-        PPLOT INFO: Plotting results to: pplot_out/20210921125420.png
-        PPLOT SUCCESS!
-        ```
-        
-        You will then find the output files in `/user/pplot_out`, with a plot for the process like:
-        
-        ![example plot](example.png)
-        
-        Additional options are available:
-        
-        ```console
-        $ pplot exec --help
-        Usage: pplot exec [OPTIONS] COMMAND
-        
-          Execute a command and profile it.
-        
-        Options:
-          -i, --interval FLOAT            Polling interval (seconds)
-          -t, --timeout FLOAT             Timeout process (seconds)
-          -c, --command-output [hide|screen|file]
-                                          Mode for stdout/stderr of command  [default:
-                                          file]
-          -o, --outfolder DIRECTORY       Folder path for output files
-          -n, --basename TEXT             Basename for output files (defaults to
-                                          datetime)
-          -p, --plot-cols [memory_rss|memory_vms|cpu_percent|cpu_time_user|cpu_time_sys|threads_num|files_num]
-                                          Columns to plot (comma-delimited)  [default:
-                                          memory_rss,cpu_percent]
-          --title TEXT                    Plot title (defaults to command)
-          --grid / --no-grid              Add grid to plots  [default: grid]
-          -sw, --size-width FLOAT         Width of plot in cm
-          -sh, --size-height FLOAT        Height of plot in cm
-          -f, --format [png|pdf|svg]      Plot file format
-          -v, --verbose                   Increase verbosity  [x>=0]
-          -q, --quiet                     Quiet mode
-          --help                          Show this message and exit.
-        ```
-        
-        ## Acknowledgements
-        
-        Initially adapted from: <https://github.com/jeetsukumaran/Syrupy>
-        
-        [ci-badge]: https://github.com/chrisjsewell/process-plot/workflows/CI/badge.svg?branch=main
-        [ci-link]: https://github.com/chrisjsewell/process-plot/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
-        [cov-badge]: https://codecov.io/gh/chrisjsewell/process-plot/branch/main/graph/badge.svg
-        [cov-link]: https://codecov.io/gh/chrisjsewell/process-plot
-        [pypi-badge]: https://img.shields.io/pypi/v/process-plot.svg
-        [pypi-link]: https://pypi.org/project/process-plot
-        
 Keywords: memory,profiling
-Platform: UNKNOWN
+Author: Chris Sewell
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: click~=8.0
+Requires-Dist: matplotlib~=3.4
+Requires-Dist: pandas~=2.2
+Requires-Dist: psutil~=5.8
+Requires-Dist: pyyaml
+Requires-Dist: coverage ; extra == "tests"
+Requires-Dist: pytest ; extra == "tests"
+Requires-Dist: pytest-cov ; extra == "tests"
+Requires-Dist: pytest-timeout ; extra == "tests"
+Project-URL: Homepage, https://github.com/chrisjsewell/process-plot
 Provides-Extra: tests
+
+# process-plot
+
+[![Build Status][ci-badge]][ci-link]
+[![codecov.io][cov-badge]][cov-link]
+[![PyPI version][pypi-badge]][pypi-link]
+
+Create plots of resource usage for a process (memory, CPU, etc).
+
+Process statistics are polled at a set interval, in a cross-platform manner (i.e. supports Linux, OSX and Windows).
+
+## Usage
+
+Install the package with [pip](https://pip.pypa.io) or [pipx](https://github.com/pypa/pipx):
+
+```console
+$ pipx install process-plot
+```
+
+then run:
+
+```console
+$ pplot exec -i 0.1 "sleep 1"
+PPLOT INFO: Output files will be written to: /user/pplot_out, with basename: 20210921125420
+PPLOT INFO: Running process as PID: 5379
+PPLOT INFO: Total run time: 0 hour(s), 00 minute(s), 01.034680 second(s)
+PPLOT INFO: Plotting results to: pplot_out/20210921125420.png
+PPLOT SUCCESS!
+```
+
+You will then find the output files in `/user/pplot_out`, with a plot for the process like:
+
+![example plot](example.png)
+
+Additional options are available:
+
+```console
+$ pplot exec --help
+Usage: pplot exec [OPTIONS] COMMAND
+
+  Execute a command and profile it.
+
+Options:
+  -i, --interval FLOAT            Polling interval (seconds)
+  -t, --timeout FLOAT             Timeout process (seconds)
+  -c, --command-output [hide|screen|file]
+                                  Mode for stdout/stderr of command  [default:
+                                  file]
+  -o, --outfolder DIRECTORY       Folder path for output files
+  -n, --basename TEXT             Basename for output files (defaults to
+                                  datetime)
+  -p, --plot-cols [memory_rss|memory_vms|cpu_percent|cpu_time_user|cpu_time_sys|threads_num|files_num]
+                                  Columns to plot (comma-delimited)  [default:
+                                  memory_rss,cpu_percent]
+  --title TEXT                    Plot title (defaults to command)
+  --grid / --no-grid              Add grid to plots  [default: grid]
+  -sw, --size-width FLOAT         Width of plot in cm
+  -sh, --size-height FLOAT        Height of plot in cm
+  -f, --format [png|pdf|svg]      Plot file format
+  -v, --verbose                   Increase verbosity  [x>=0]
+  -q, --quiet                     Quiet mode
+  --help                          Show this message and exit.
+```
+
+## Acknowledgements
+
+Initially adapted from: <https://github.com/jeetsukumaran/Syrupy>
+
+[ci-badge]: https://github.com/chrisjsewell/process-plot/workflows/CI/badge.svg?branch=main
+[ci-link]: https://github.com/chrisjsewell/process-plot/actions?query=workflow%3ACI+branch%3Amain+event%3Apush
+[cov-badge]: https://codecov.io/gh/chrisjsewell/process-plot/branch/main/graph/badge.svg
+[cov-link]: https://codecov.io/gh/chrisjsewell/process-plot
+[pypi-badge]: https://img.shields.io/pypi/v/process-plot.svg
+[pypi-link]: https://pypi.org/project/process-plot
+
```

### Comparing `process_plot-0.2.1/README.md` & `process_plot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `process_plot-0.2.1/process_plot/api.py` & `process_plot-0.3.0/process_plot/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Code for profiling a process."""
+
+from collections.abc import Sequence
 import os
-import time
 from os import PathLike
-from typing import Optional, Sequence, TextIO, Union
+import time
+from typing import Optional, TextIO, Union
 
 import psutil
 
 POSIX = os.name == "posix"
 WINDOWS = os.name == "nt"
 
 COLUMNS_DESCRIPT = (
@@ -20,15 +22,15 @@
     ("threads_num", "Number of threads currently used"),
     ("memory_rss_bytes", "Resident Set Size; the non-swapped physical memory used"),
     ("memory_vms_bytes", "Virtual Memory Size: the virtual memory used"),
     ("files_num", "Number of file descriptors (POSIX) or handles (Windows) used"),
 )
 
 
-def profile_process(  # noqa: C901
+def profile_process(
     pid: int,
     *,
     poll_interval: Union[int, float] = 1,
     max_iterations: Optional[int] = None,
     output_stream: Optional[TextIO] = None,
     flush_output: bool = False,
     headers: bool = True,
@@ -59,15 +61,14 @@
         output_stream.write(output_separator.join(col_headers) + "\n")
         if flush_output:
             output_stream.flush()
 
     iteration = 0
     proc = psutil.Process(pid)
     while True:
-
         iteration += 1
 
         elapsed_time = time.time() - proc.create_time()
         try:
             if not proc.is_running() or proc.status() == "zombie":
                 raise psutil.NoSuchProcess(proc.pid)
             data = proc.as_dict(
```

### Comparing `process_plot-0.2.1/process_plot/cli.py` & `process_plot-0.3.0/process_plot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """The commandline interface."""
+
+from contextlib import nullcontext
+from datetime import datetime
 import os
+from pathlib import Path
 import shlex
 import subprocess
 import sys
 import time
-from contextlib import nullcontext
-from datetime import datetime
-from pathlib import Path
 
 import click
 import yaml
 
 from . import __version__
 from .api import COLUMNS_DESCRIPT, PLOT_YLABELS, plot_result, profile_process
 
@@ -47,15 +48,15 @@
 )
 def main(
     context_settings={  # noqa: B006
         "help_option_names": (
             "-h",
             "--help",
         )
-    }
+    },
 ):
     """CLI to profile a process's memory/CPU usage and plot it."""
 
 
 @main.command("exec")
 @click.argument("command")
 @click.option(
```

