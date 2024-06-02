# Comparing `tmp/cycle_plotter-0.0.1rc1.tar.gz` & `tmp/cycle_plotter-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycle_plotter-0.0.1rc1.tar", last modified: Sun Jun  2 22:19:06 2024, max compression
+gzip compressed data, was "cycle_plotter-0.0.1rc2.tar", last modified: Sun Jun  2 22:47:10 2024, max compression
```

## Comparing `cycle_plotter-0.0.1rc1.tar` & `cycle_plotter-0.0.1rc2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-06-02 22:19:06.000000 cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-02 22:19:06.000000 cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:19:06.000000 cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 22:19:06.000000 cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 22:19:06.000000 cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 22:19:06.000000 cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.980056 cycle_plotter-0.0.1rc1/cycleplotter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.980056 cycle_plotter-0.0.1rc1/cycleplotter/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/entities/cycle_duration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.980056 cycle_plotter-0.0.1rc1/cycleplotter/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.980056 cycle_plotter-0.0.1rc1/cycleplotter/infrastructure/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/infrastructure/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/infrastructure/files/opener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.980056 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.980056 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.980056 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/applehealth.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/withingshealthmate.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/cycleplotter/usecases/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/cycle_dates_to_durations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/cycleplotter/usecases/cycledataparser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/cycledataparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/cycledataparser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/extract_cycle_durations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/cycleplotter/usecases/plotter/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/plotter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/cycleplotter/usecases/plotter/plot_cycle_durations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:19:06.984056 cycle_plotter-0.0.1rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/tests/test_extract_cycle_durations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-06-02 22:19:03.000000 cycle_plotter-0.0.1rc1/tests/test_plot_cycle_durations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.142188 cycle_plotter-0.0.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-06-02 22:47:10.142188 cycle_plotter-0.0.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.142188 cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-06-02 22:47:10.000000 cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-02 22:47:10.000000 cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 22:47:10.000000 cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 22:47:10.000000 cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 22:47:10.000000 cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 22:47:10.000000 cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/entities/cycle_duration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/infrastructure/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/infrastructure/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/infrastructure/files/opener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/applehealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/withingshealthmate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/usecases/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/cycle_dates_to_durations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/usecases/cycledataparser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/cycledataparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/cycledataparser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/extract_cycle_durations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/cycleplotter/usecases/plotter/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/plotter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/cycleplotter/usecases/plotter/plot_cycle_durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 22:47:10.142188 cycle_plotter-0.0.1rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 22:47:10.138188 cycle_plotter-0.0.1rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/tests/test_extract_cycle_durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-06-02 22:47:06.000000 cycle_plotter-0.0.1rc2/tests/test_plot_cycle_durations.py
```

### Comparing `cycle_plotter-0.0.1rc1/LICENSE` & `cycle_plotter-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/PKG-INFO` & `cycle_plotter-0.0.1rc2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycle-plotter
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Command line tool to plot a graph of cycles exported from Apple Health or Withings Health Mate.
 Author-email: Carmen Alvarez <carmen@rmen.ca>
 License: MIT License
         
         Copyright (c) 2024 Carmen Alvarez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,21 +55,21 @@
 
 ### Sample graphs
 
 The datasets for these graphs were generated by ChatGPT. They don't corespond to any real person.
 
 #### Regular cycles
 Cycles covering a period of 6 months, with little variation in cycle length.
-<img src="docs/regular.png" >
+<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/regular.png" >
 
 #### Pregnancy
 Cycles covering a period of just over one year, with a pregnancy during that time.
 |`--axis x` | `--axis y` | `--axis both` (default) |
 |---|---|---|
-|<img src="docs/pregnancy-x.png" > |<img src="docs/pregnancy-y.png" > |<img src="docs/pregnancy-both.png" >|
+|<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/pregnancy-x.png" > |<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/pregnancy-y.png" > |<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/pregnancy-both.png" >|
 
 ## Usage
 
 Run the program with the `--help` argument to see the full usage.
 
 ```
 % python -m cycleplotter.main --help
@@ -119,28 +119,8 @@
 Export a pdf of data from Withings Health Mate, using short arguments:
 ```shell
 python -m cycleplotter.main -i ~/Downloads/data_ABC_1717249954.zip  -o /tmp/cyclegraph.pdf -s withings
 ```
 
 ## How to get the health data files
 
-### Apple health
-* Open Apple Health.
-* Click on "Browse".
-* Click on your avatar on the top right.
-* Scroll down to the end of the screen. Click on "Export All Health Data".
-* Click "Export".
-* Wait a few moments while the dialog "Preparing" appears.
-* Select an app to share the data to yourself (by email for example).
-
-<img src="docs/apple-export.png">
-
-### Withings Health Mate
-* Open Withings Health Mate.
-* Click on your avatar on the top left.
-* Click on the settings icon.
-* Click on "Export All Health Data".
-* Click "Start my archive"
-* You will receive an email from Withings with a link to download the archive.
-
-<img src="docs/withings-export.png">
-
+See the steps [here](https://github.com/caarmen/cycle-plotter/blob/main/docs/healthdatafiles.md).
```

### Comparing `cycle_plotter-0.0.1rc1/README.md` & `cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,49 @@
+Metadata-Version: 2.1
+Name: cycle-plotter
+Version: 0.0.1rc2
+Summary: Command line tool to plot a graph of cycles exported from Apple Health or Withings Health Mate.
+Author-email: Carmen Alvarez <carmen@rmen.ca>
+License: MIT License
+        
+        Copyright (c) 2024 Carmen Alvarez
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Repository, https://github.com/caarmen/cycle-plotter
+Project-URL: Changelog, https://github.com/caarmen/cycle-plotter/releases
+Keywords: cli,health
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Framework :: Matplotlib
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: defusedxml
+Requires-Dist: matplotlib
+
 ## Cycle Plotter
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/caarmen/cycle-plotter/check.yml)
 ![GitHub License](https://img.shields.io/github/license/caarmen/cycle-plotter)
 ![GitHub top language](https://img.shields.io/github/languages/top/caarmen/cycle-plotter)
 ![GitHub last commit](https://img.shields.io/github/last-commit/caarmen/cycle-plotter)
 
@@ -13,21 +55,21 @@
 
 ### Sample graphs
 
 The datasets for these graphs were generated by ChatGPT. They don't corespond to any real person.
 
 #### Regular cycles
 Cycles covering a period of 6 months, with little variation in cycle length.
-<img src="docs/regular.png" >
+<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/regular.png" >
 
 #### Pregnancy
 Cycles covering a period of just over one year, with a pregnancy during that time.
 |`--axis x` | `--axis y` | `--axis both` (default) |
 |---|---|---|
-|<img src="docs/pregnancy-x.png" > |<img src="docs/pregnancy-y.png" > |<img src="docs/pregnancy-both.png" >|
+|<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/pregnancy-x.png" > |<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/pregnancy-y.png" > |<img src="https://raw.githubusercontent.com/caarmen/cycle-plotter/main/docs/pregnancy-both.png" >|
 
 ## Usage
 
 Run the program with the `--help` argument to see the full usage.
 
 ```
 % python -m cycleplotter.main --help
@@ -77,28 +119,8 @@
 Export a pdf of data from Withings Health Mate, using short arguments:
 ```shell
 python -m cycleplotter.main -i ~/Downloads/data_ABC_1717249954.zip  -o /tmp/cyclegraph.pdf -s withings
 ```
 
 ## How to get the health data files
 
-### Apple health
-* Open Apple Health.
-* Click on "Browse".
-* Click on your avatar on the top right.
-* Scroll down to the end of the screen. Click on "Export All Health Data".
-* Click "Export".
-* Wait a few moments while the dialog "Preparing" appears.
-* Select an app to share the data to yourself (by email for example).
-
-<img src="docs/apple-export.png">
-
-### Withings Health Mate
-* Open Withings Health Mate.
-* Click on your avatar on the top left.
-* Click on the settings icon.
-* Click on "Export All Health Data".
-* Click "Start my archive"
-* You will receive an email from Withings with a link to download the archive.
-
-<img src="docs/withings-export.png">
-
+See the steps [here](https://github.com/caarmen/cycle-plotter/blob/main/docs/healthdatafiles.md).
```

### Comparing `cycle_plotter-0.0.1rc1/cycle_plotter.egg-info/SOURCES.txt` & `cycle_plotter-0.0.1rc2/cycle_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cli/argparser.py` & `cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cli/argparser.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/applehealth.py` & `cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/applehealth.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/factory.py` & `cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/factory.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/cycleplotter/interfaceadapters/cycledataparser/withingshealthmate.py` & `cycle_plotter-0.0.1rc2/cycleplotter/interfaceadapters/cycledataparser/withingshealthmate.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/cycleplotter/main.py` & `cycle_plotter-0.0.1rc2/cycleplotter/main.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/cycleplotter/usecases/cycle_dates_to_durations.py` & `cycle_plotter-0.0.1rc2/cycleplotter/usecases/cycle_dates_to_durations.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/cycleplotter/usecases/plotter/plot_cycle_durations.py` & `cycle_plotter-0.0.1rc2/cycleplotter/usecases/plotter/plot_cycle_durations.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/pyproject.toml` & `cycle_plotter-0.0.1rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cycle-plotter"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 dependencies = [
   "defusedxml",
   "matplotlib",
 ]
 requires-python = ">=3.11"
 authors = [
   {name = "Carmen Alvarez", email = "carmen@rmen.ca"},
```

### Comparing `cycle_plotter-0.0.1rc1/tests/test_extract_cycle_durations.py` & `cycle_plotter-0.0.1rc2/tests/test_extract_cycle_durations.py`

 * *Files identical despite different names*

### Comparing `cycle_plotter-0.0.1rc1/tests/test_plot_cycle_durations.py` & `cycle_plotter-0.0.1rc2/tests/test_plot_cycle_durations.py`

 * *Files identical despite different names*

