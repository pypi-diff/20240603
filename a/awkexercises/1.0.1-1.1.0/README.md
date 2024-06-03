# Comparing `tmp/awkexercises-1.0.1.tar.gz` & `tmp/awkexercises-1.1.0.tar.gz`

## Comparing `awkexercises-1.0.1.tar` & `awkexercises-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/__init__.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/app_guide.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/awk_exercises.css
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/awk_exercises.py
--rw-r--r--   0        0        0    40771 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/questions.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/user_progress.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/addr.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/anchors.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/brackets.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/broken.txt
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/concat.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/copyright.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/criteria.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f1.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f10.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f11.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f2.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f3.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f4.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f5.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f6.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f7.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f8.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/f9.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/fields.txt
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/files.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/fw.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/hex.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/ip.txt
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/items.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/jumbled.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/lines.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/match_words.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/mixed_fs.txt
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/names.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/nums.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/nums1.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/odd.txt
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/patterns.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/quoted.txt
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/result.csv
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/sample.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/scores.csv
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/secrets.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/sum.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/table.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/twos.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 awkexercises-1.0.1/src/awkexercises/sample_input/varying_fields.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 awkexercises-1.0.1/LICENSE
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 awkexercises-1.0.1/README.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 awkexercises-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 awkexercises-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/__init__.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/app_guide.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/awk_exercises.css
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/awk_exercises.py
+-rw-r--r--   0        0        0    40771 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/questions.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/user_progress.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/addr.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/anchors.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/brackets.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/broken.txt
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/concat.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/copyright.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/criteria.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f1.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f10.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f11.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f2.txt
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f3.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f4.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f5.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f6.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f7.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f8.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/f9.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/fields.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/files.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/fw.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/hex.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/ip.txt
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/items.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/jumbled.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/lines.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/match_words.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/mixed_fs.txt
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/names.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/nums.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/nums1.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/odd.txt
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/patterns.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/quoted.txt
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/result.csv
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/sample.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/scores.csv
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/secrets.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/sum.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/table.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/twos.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 awkexercises-1.1.0/src/awkexercises/sample_input/varying_fields.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 awkexercises-1.1.0/LICENSE
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 awkexercises-1.1.0/README.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 awkexercises-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 awkexercises-1.1.0/PKG-INFO
```

### Comparing `awkexercises-1.0.1/src/awkexercises/app_guide.md` & `awkexercises-1.1.0/src/awkexercises/app_guide.md`

 * *Files identical despite different names*

### Comparing `awkexercises-1.0.1/src/awkexercises/awk_exercises.css` & `awkexercises-1.1.0/src/awkexercises/awk_exercises.css`

 * *Files identical despite different names*

### Comparing `awkexercises-1.0.1/src/awkexercises/awk_exercises.py` & `awkexercises-1.1.0/src/awkexercises/awk_exercises.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 SCRIPT_DIR = Path(__file__).parent.resolve()
 
 class AwkExercisesApp(App):
     CSS_PATH = SCRIPT_DIR.joinpath('awk_exercises.css')
     BINDINGS = [
         Binding('ctrl+s', 'show_solution', 'Solution', show=True),
-        Binding('ctrl+p', 'previous', 'Prev', show=True),
+        Binding('ctrl+p', 'previous', 'Previous', show=True),
         Binding('ctrl+n', 'next', 'Next', show=True),
         Binding('f1', 'app_guide', 'App Guide', show=False),
         Binding('f2', 'awk_exercises', 'Awk Exercises', show=False),
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

### Comparing `awkexercises-1.0.1/src/awkexercises/questions.json` & `awkexercises-1.1.0/src/awkexercises/questions.json`

 * *Files identical despite different names*

### Comparing `awkexercises-1.0.1/src/awkexercises/sample_input/patterns.txt` & `awkexercises-1.1.0/src/awkexercises/sample_input/patterns.txt`

 * *Files identical despite different names*

### Comparing `awkexercises-1.0.1/LICENSE` & `awkexercises-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awkexercises-1.0.1/README.md` & `awkexercises-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `awkexercises-1.0.1/pyproject.toml` & `awkexercises-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "awkexercises"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "80+ exercises for GNU awk"
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
 awkexercises = "awkexercises.awk_exercises:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/AwkExercises"
```

### Comparing `awkexercises-1.0.1/PKG-INFO` & `awkexercises-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: awkexercises
-Version: 1.0.1
+Version: 1.1.0
 Summary: 80+ exercises for GNU awk
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/AwkExercises
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
 
 # Awk Exercises
 
 This TUI application includes 80+ questions meant to be solved using `GNU awk`. Some exercises will require you to combine `awk` with other CLI tools such as `tac`.
 
 > **Note:** This application is intended to be run in a Linux-like environment. You might still be able to solve the exercises on other platforms, but I do not know if that'll work.
```

