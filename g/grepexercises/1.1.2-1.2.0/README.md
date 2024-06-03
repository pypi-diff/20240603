# Comparing `tmp/grepexercises-1.1.2.tar.gz` & `tmp/grepexercises-1.2.0.tar.gz`

## Comparing `grepexercises-1.1.2.tar` & `grepexercises-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/__init__.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/app_guide.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/grep_exercises.css
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/grep_exercises.py
--rw-r--r--   0        0        0    33176 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/questions.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/user_progress.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/.hidden
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/code.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/colors_1
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/colors_2.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/lines.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/nul_separated
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/patterns.txt
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/pcre.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/regex_terms.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/sample.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/substitute.sh
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/terms.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/backups/color list.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/backups/dot_files/.bash_aliases
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/backups/dot_files/.inputrc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/projects/python/hello.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-1.1.2/src/grepexercises/sample_input/projects/shell/hello.sh
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grepexercises-1.1.2/LICENSE
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 grepexercises-1.1.2/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 grepexercises-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 grepexercises-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/__init__.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/app_guide.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/grep_exercises.css
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/grep_exercises.py
+-rw-r--r--   0        0        0    33176 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/questions.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/user_progress.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/.hidden
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/code.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/colors_1
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/colors_2.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/lines.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/nul_separated
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/patterns.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/pcre.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/regex_terms.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/sample.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/substitute.sh
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/terms.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/backups/color list.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/backups/dot_files/.bash_aliases
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/backups/dot_files/.inputrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/projects/python/hello.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-1.2.0/src/grepexercises/sample_input/projects/shell/hello.sh
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grepexercises-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 grepexercises-1.2.0/README.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 grepexercises-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 grepexercises-1.2.0/PKG-INFO
```

### Comparing `grepexercises-1.1.2/src/grepexercises/app_guide.md` & `grepexercises-1.2.0/src/grepexercises/app_guide.md`

 * *Files identical despite different names*

### Comparing `grepexercises-1.1.2/src/grepexercises/grep_exercises.css` & `grepexercises-1.2.0/src/grepexercises/grep_exercises.css`

 * *Files identical despite different names*

### Comparing `grepexercises-1.1.2/src/grepexercises/grep_exercises.py` & `grepexercises-1.2.0/src/grepexercises/grep_exercises.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 SCRIPT_DIR = Path(__file__).parent.resolve()
 
 class GrepExercisesApp(App):
     CSS_PATH = SCRIPT_DIR.joinpath('grep_exercises.css')
     BINDINGS = [
         Binding('ctrl+s', 'show_solution', 'Solution', show=True),
-        Binding('ctrl+p', 'previous', 'Prev', show=True),
+        Binding('ctrl+p', 'previous', 'Previous', show=True),
         Binding('ctrl+n', 'next', 'Next', show=True),
         Binding('f1', 'app_guide', 'App Guide', show=False),
         Binding('f2', 'grep_exercises', 'Grep Exercises', show=False),
         Binding('f3', 'directory', 'Directory', show=False),
         ('ctrl+t', 'toggle_theme', 'Theme'),
         ('ctrl+q', 'app.quit', 'Quit'),
     ]
@@ -146,34 +146,34 @@
         self.solved = False
         self.l_question.update(
                 Markdown(f'(Q:{self.q_idx+1}/{self.q_max_idx+1}) ' +
                          self.questions[self.q_idx]['question']))
         self.ref_solution = self.questions[self.q_idx]['ref_solution']
 
         self.h_ip_op.remove()
-        v_ip = Vertical(classes='ip_op_container')
-        v_op = Vertical(classes='ip_op_container')
         ip_files = self.questions[self.q_idx]['ip_file']
-        if ip_files:
-            self.h_ip_op = Horizontal(v_ip, v_op, classes='container')
-        else:
-            self.h_ip_op = v_op
-        self.v_exercises.mount(self.h_ip_op)
-
+        v_ip_widgets = []
         for ip_file in ip_files:
             with open(ip_file, encoding='ascii') as f:
                 ip_txt = self.trim(f.read())
             l_ip = Label(ip_txt, classes='ip_op', markup=False)
             l_ip.border_title = ip_file
-            v_ip.mount(l_ip)
+            v_ip_widgets.append(l_ip)
 
         self.op_txt = self.trim(self.questions[self.q_idx]['op_file'])
         l_op = Label(self.op_txt, classes='ip_op', markup=False)
         l_op.border_title = 'Expected output'
-        v_op.mount(l_op)
+
+        v_ip = Vertical(*v_ip_widgets, classes='ip_op_container')
+        v_op = Vertical(l_op, classes='ip_op_container')
+        if ip_files:
+            self.h_ip_op = Horizontal(v_ip, v_op, classes='container')
+        else:
+            self.h_ip_op = v_op
+        self.v_exercises.mount(self.h_ip_op)
 
         if self.q_idx in self.user_progress:
             self.set_cmd(self.user_progress[self.q_idx][0])
         else:
             self.i_cmd.value = ''
             self.i_cmd.styles.background = 'lightgray'
             self.l_cmd_output.update('')
```

### Comparing `grepexercises-1.1.2/src/grepexercises/questions.json` & `grepexercises-1.2.0/src/grepexercises/questions.json`

 * *Files identical despite different names*

### Comparing `grepexercises-1.1.2/src/grepexercises/sample_input/patterns.txt` & `grepexercises-1.2.0/src/grepexercises/sample_input/patterns.txt`

 * *Files identical despite different names*

### Comparing `grepexercises-1.1.2/LICENSE` & `grepexercises-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grepexercises-1.1.2/README.md` & `grepexercises-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `grepexercises-1.1.2/pyproject.toml` & `grepexercises-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "grepexercises"
-version = "1.1.2"
+version = "1.2.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "50+ exercises for GNU grep (or alternatives like ripgrep)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.46.0",
+  "textual>=0.63.6",
 ]
 
 [project.scripts]
 grepexercises = "grepexercises.grep_exercises:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/GrepExercises"
```

### Comparing `grepexercises-1.1.2/PKG-INFO` & `grepexercises-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: grepexercises
-Version: 1.1.2
+Version: 1.2.0
 Summary: 50+ exercises for GNU grep (or alternatives like ripgrep)
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/GrepExercises
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: textual>=0.46.0
+Requires-Dist: textual>=0.63.6
 Description-Content-Type: text/markdown
 
 # Grep Exercises
 
 This TUI application includes 50+ questions meant to be solved using `GNU grep` (or alternate implementations like `ripgrep`). Some exercises will require you to combine `grep` with other standard commands such as `cat`, `wc` and `find`.
 
 > **Note:** This application is intended to be run in a Linux-like environment. You might still be able to solve the exercises on other platforms, but I do not know if that'll work.
```

