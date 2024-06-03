# Comparing `tmp/sedexercises-1.0.1.tar.gz` & `tmp/sedexercises-1.1.0.tar.gz`

## Comparing `sedexercises-1.0.1.tar` & `sedexercises-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/__init__.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/app_guide.md
--rw-r--r--   0        0        0    28754 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/questions.json
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sed_exercises.css
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sed_exercises.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/user_progress.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/addr.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/anchors.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/blocks.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/broken.txt
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/code.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/copyright.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/f1.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/f2.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/f3.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/f4.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/f5.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/f6.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/fields.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/headers.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/hex.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/nul_separated
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/nums.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/para.txt
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/patterns.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/purchases.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/replace.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/sample.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sedexercises-1.0.1/src/sedexercises/sample_input/text.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sedexercises-1.0.1/LICENSE
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 sedexercises-1.0.1/README.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 sedexercises-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 sedexercises-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/__init__.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/app_guide.md
+-rw-r--r--   0        0        0    28754 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/questions.json
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sed_exercises.css
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sed_exercises.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/user_progress.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/addr.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/anchors.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/blocks.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/broken.txt
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/code.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/copyright.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/f1.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/f2.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/f3.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/f4.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/f5.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/f6.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/fields.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/headers.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/hex.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/nul_separated
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/nums.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/para.txt
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/patterns.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/purchases.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/replace.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/sample.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sedexercises-1.1.0/src/sedexercises/sample_input/text.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sedexercises-1.1.0/LICENSE
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 sedexercises-1.1.0/README.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 sedexercises-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 sedexercises-1.1.0/PKG-INFO
```

### Comparing `sedexercises-1.0.1/src/sedexercises/app_guide.md` & `sedexercises-1.1.0/src/sedexercises/app_guide.md`

 * *Files identical despite different names*

### Comparing `sedexercises-1.0.1/src/sedexercises/questions.json` & `sedexercises-1.1.0/src/sedexercises/questions.json`

 * *Files identical despite different names*

### Comparing `sedexercises-1.0.1/src/sedexercises/sed_exercises.css` & `sedexercises-1.1.0/src/sedexercises/sed_exercises.css`

 * *Files identical despite different names*

### Comparing `sedexercises-1.0.1/src/sedexercises/sed_exercises.py` & `sedexercises-1.1.0/src/sedexercises/sed_exercises.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 SCRIPT_DIR = Path(__file__).parent.resolve()
 
 class SedExercisesApp(App):
     CSS_PATH = SCRIPT_DIR.joinpath('sed_exercises.css')
     BINDINGS = [
         Binding('ctrl+s', 'show_solution', 'Solution', show=True),
-        Binding('ctrl+p', 'previous', 'Prev', show=True),
+        Binding('ctrl+p', 'previous', 'Previous', show=True),
         Binding('ctrl+n', 'next', 'Next', show=True),
         Binding('f1', 'app_guide', 'App Guide', show=False),
         Binding('f2', 'sed_exercises', 'Sed Exercises', show=False),
         Binding('f3', 'directory', 'Directory', show=False),
         ('ctrl+t', 'toggle_theme', 'Theme'),
         ('ctrl+q', 'app.quit', 'Quit'),
     ]
@@ -132,34 +132,34 @@
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
-            self.h_ip_op = Horizontal(v_op, classes='container')
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

### Comparing `sedexercises-1.0.1/src/sedexercises/sample_input/patterns.txt` & `sedexercises-1.1.0/src/sedexercises/sample_input/patterns.txt`

 * *Files identical despite different names*

### Comparing `sedexercises-1.0.1/LICENSE` & `sedexercises-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sedexercises-1.0.1/README.md` & `sedexercises-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sedexercises-1.0.1/pyproject.toml` & `sedexercises-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "sedexercises"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "50+ exercises for GNU sed"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.45.1",
+  "textual>=0.63.6",
 ]
 
 [project.scripts]
 sedexercises = "sedexercises.sed_exercises:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/SedExercises"
```

### Comparing `sedexercises-1.0.1/PKG-INFO` & `sedexercises-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sedexercises
-Version: 1.0.1
+Version: 1.1.0
 Summary: 50+ exercises for GNU sed
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/SedExercises
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: textual>=0.45.1
+Requires-Dist: textual>=0.63.6
 Description-Content-Type: text/markdown
 
 # Sed Exercises
 
 This TUI application includes 50+ questions meant to be solved using `GNU sed`. Some exercises will require you to combine `sed` with other standard commands such as `tac`, `wc` and `tr`.
 
 > **Note:** This application is intended to be run in a Linux-like environment. You might still be able to solve the exercises on other platforms, but I do not know if that'll work.
```

