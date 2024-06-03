# Comparing `tmp/awktutorial-1.0.0.tar.gz` & `tmp/awktutorial-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, from Unix
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `awktutorial-1.0.0.tar` & `awktutorial-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,27 @@
-drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-04-29 04:01:42.000000 awktutorial-1.0.0/
-drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-04-29 04:01:05.000000 awktutorial-1.0.0/src/
-drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-04-29 04:01:05.000000 awktutorial-1.0.0/src/awktutorial/
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      520 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/awk_tutorial.css
-drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-04-29 04:01:05.000000 awktutorial-1.0.0/src/awktutorial/example_files/
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)       40 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/c1.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)       34 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/greeting.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)       39 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/c2.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      155 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/marks.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)       57 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/purchases.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      119 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/uniform.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)        8 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/dept.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)       79 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/table.txt
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      174 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/example_files/items.csv
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)        0 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/__init__.py
-drwxrwxr-x   0 sundeep   (1000) sundeep   (1000)        0 2024-04-29 04:01:05.000000 awktutorial-1.0.0/src/awktutorial/tutorial/
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     2018 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_05.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1399 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_03.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      578 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_10.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      423 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_02.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1399 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_09.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      934 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_06.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     2472 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_00.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1551 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_07.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1039 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_04.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1057 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_01.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     2447 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/tutorial/awk_08.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     5344 2020-02-02 00:00:00.000000 awktutorial-1.0.0/src/awktutorial/awk_tutorial.py
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      714 2020-02-02 00:00:00.000000 awktutorial-1.0.0/pyproject.toml
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)      507 2020-02-02 00:00:00.000000 awktutorial-1.0.0/README.md
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1072 2020-02-02 00:00:00.000000 awktutorial-1.0.0/LICENSE
--rw-r--r--   0 sundeep   (1000) sundeep   (1000)     1086 2024-04-29 04:01:42.000000 awktutorial-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/awk_tutorial.css
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/awk_tutorial.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/c1.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/c2.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/dept.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/greeting.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/items.csv
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/marks.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/purchases.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/table.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/example_files/uniform.txt
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_00.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_01.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_02.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_03.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_04.md
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_05.md
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_06.md
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_07.md
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_08.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_09.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 awktutorial-1.1.0/src/awktutorial/tutorial/awk_10.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 awktutorial-1.1.0/LICENSE
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awktutorial-1.1.0/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 awktutorial-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 awktutorial-1.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `awktutorial-1.0.0/src/awktutorial/awk_tutorial.css` & `awktutorial-1.1.0/src/awktutorial/awk_tutorial.css`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_05.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_05.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_03.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_03.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_10.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_10.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_09.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_09.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_06.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_06.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_00.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_00.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_07.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_07.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_04.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_04.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_01.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_01.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/tutorial/awk_08.md` & `awktutorial-1.1.0/src/awktutorial/tutorial/awk_08.md`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/src/awktutorial/awk_tutorial.py` & `awktutorial-1.1.0/src/awktutorial/awk_tutorial.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 
 SCRIPT_DIR = Path(__file__).parent.resolve()
 
 class AwkTutorialApp(App):
     CSS_PATH = SCRIPT_DIR.joinpath('awk_tutorial.css')
     BINDINGS = [
-        Binding('ctrl+p', 'previous', 'Prev', show=True),
+        Binding('ctrl+p', 'previous', 'Previous', show=True),
         Binding('ctrl+n', 'next', 'Next', show=True),
         Binding('ctrl+r', 'reset', 'Reset', show=True),
         ('ctrl+t', 'toggle_theme', 'Theme'),
         ('ctrl+q', 'app.quit', 'Quit'),
     ]
 
     def __init__(self):
@@ -64,52 +64,53 @@
                 self.i_cmd.styles.background = 'lightgray'
             else:
                 self.l_cmd_output.update(self.trim(result.stdout))
                 self.l_cmd_output_style('gray', 'Output', '')
 
     def setup_tutorial(self):
         self.v_tutorial.remove()
-        self.v_tutorial = VerticalScroll()
         block = False
         s = ''
         cnt = 0
         self.i_cmds = []
         self.l_cmd_outputs = []
+        tt_widgets = []
         with open(self.tutorial_files[self.idx]) as f:
             title = f'[b]({self.idx+1}/{self.max_idx+1}) {next(f)[2:-1]}'
             self.l_title.update(title)
             for line in f:
                 if line.startswith('```'):
                     if block:
-                        codeblock = Vertical(classes='codeblock')
+                        cb_widgets = []
                         for c in s.splitlines():
                             if c.startswith('#'):
-                                codeblock.mount(Label(c, classes='comment'))
+                                cb_widgets.append(Label(c, classes='comment'))
                             elif c.startswith('$ '):
                                 self.i_cmd = Input(classes='input',
                                                    name=str(cnt))
                                 self.l_cmd_output = Label(classes='cmd_output',
                                                           markup=False)
-                                codeblock.mount(self.i_cmd)
-                                codeblock.mount(self.l_cmd_output)
+                                cb_widgets.append(self.i_cmd)
+                                cb_widgets.append(self.l_cmd_output)
                                 self.i_cmds.append(self.i_cmd)
                                 self.l_cmd_outputs.append(self.l_cmd_output)
                                 self.set_cmd(c[2:])
                                 if cnt == 0:
                                     self.i_cmd.focus()
                                 cnt += 1
-                        self.v_tutorial.mount(codeblock)
+                        tt_widgets.append(Vertical(*cb_widgets, classes='codeblock'))
                     else:
-                        self.v_tutorial.mount(Markdown(s))
+                        tt_widgets.append(Markdown(s))
                     s = ''
                     block ^= True
                     continue
                 s += line
             if s:
-                self.v_tutorial.mount(Markdown(s))
+                tt_widgets.append(Markdown(s))
+        self.v_tutorial = VerticalScroll(*tt_widgets)
         self.v_main.mount(self.v_tutorial)
 
     def set_cmd(self, cmd):
         self.i_cmd.value = cmd
         self.i_cmd.cursor_position = len(cmd)
         self.process_user_cmd()
```

### Comparing `awktutorial-1.0.0/pyproject.toml` & `awktutorial-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "awktutorial"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "brief tour of the GNU awk command"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.57.1",
+  "textual>=0.63.6",
 ]
 
 [project.scripts]
 awktutorial = "awktutorial.awk_tutorial:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/AwkTutorial"
```

### Comparing `awktutorial-1.0.0/LICENSE` & `awktutorial-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awktutorial-1.0.0/PKG-INFO` & `awktutorial-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: awktutorial
-Version: 1.0.0
+Version: 1.1.0
 Summary: brief tour of the GNU awk command
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/AwkTutorial
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: textual>=0.57.1
+Requires-Dist: textual>=0.63.6
 Description-Content-Type: text/markdown
 
 # Awk Tutorial
 
 This interactive tutorial aims to give a brief tour of the `GNU awk` command.
 
 # Screenshot
```

