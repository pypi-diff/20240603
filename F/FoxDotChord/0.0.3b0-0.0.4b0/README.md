# Comparing `tmp/foxdotchord-0.0.3b0.tar.gz` & `tmp/foxdotchord-0.0.4b0.tar.gz`

## Comparing `foxdotchord-0.0.3b0.tar` & `foxdotchord-0.0.4b0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 foxdotchord-0.0.3b0/FoxDotChord/__init__.py
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 foxdotchord-0.0.3b0/FoxDotChord/_chord.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 foxdotchord-0.0.3b0/.gitignore
--rw-r--r--   0        0        0    35075 2020-02-02 00:00:00.000000 foxdotchord-0.0.3b0/LICENSE
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 foxdotchord-0.0.3b0/README.md
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 foxdotchord-0.0.3b0/pyproject.toml
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 foxdotchord-0.0.3b0/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 foxdotchord-0.0.4b0/FoxDotChord/__init__.py
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 foxdotchord-0.0.4b0/FoxDotChord/_chord.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 foxdotchord-0.0.4b0/.gitignore
+-rw-r--r--   0        0        0    35075 2020-02-02 00:00:00.000000 foxdotchord-0.0.4b0/LICENSE
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 foxdotchord-0.0.4b0/README.md
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 foxdotchord-0.0.4b0/pyproject.toml
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 foxdotchord-0.0.4b0/PKG-INFO
```

### Comparing `foxdotchord-0.0.3b0/FoxDotChord/_chord.py` & `foxdotchord-0.0.4b0/FoxDotChord/_chord.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         False
         >>> Chord('Ebsus').is_sus
         True
         >>> Chord('Ebsus4').is_sus
         True
         >>> Chord('Eb4').is_sus
         False
-        >>> Chord('Eb#3').is_sus
+        >>> Chord('Eb3#').is_sus
         False
 
         Returns
         -------
         bool:
             `True` if the chord is suspended otherwise `False`.
         """
@@ -246,15 +246,15 @@
 
         Examples
         --------
         >>> Chord('C')
         Chord('C')
         """
         if not (
-            result := re.search(r'(^(?P<tone>[A-G]){1}[b#]?)', self.chord)
+            result := re.search(r'(^(?P<tone>[A-G]{1}[b#]?))', self.chord)
         ):
             raise ChordException(
                 f'Tonic inválid: "{self.chord:.1}" from chord "{self.chord}"',
             )
         return Note(result.group('tone')) + self.tone
 
     @property
@@ -276,26 +276,26 @@
     @property
     def subdominant(self) -> TNote:
         """Subdominant IV."""
         if (
             re.search(r'(sus)2', self.chord)
             or (
                 not re.search(r'4', self.chord)
-                and not re.search(r'(sus)([\+#]3|4)?', self.chord)
+                and not re.search(r'(sus)(3[\+#]|4)?', self.chord)
             )
         ):
             return None
         return self.tonic + 5
 
     @property
     def dominant(self) -> TNote:
         """Dominant V."""
-        if re.search(r'[\+#]5', self.chord):
+        if re.search(r'5[\+#]', self.chord):
             return self.tonic + 8
-        if re.search(r'[\-b]5', self.chord) or self.is_dim:
+        if re.search(r'5[\-b]', self.chord) or self.is_dim:
             return self.tonic + 6
         return self.tonic + 7
 
     @property
     def submediant(self) -> TNote:
         """Submediant VI."""
         if re.search(r'6', self.chord):
@@ -308,37 +308,37 @@
             return self.tonic + 11
         if re.search(r'7', self.chord):
             return self.tonic + 10
 
     @property
     def ninth(self) -> TNote:
         """Ninth IX."""
-        if re.search(r'[\+\#]9', self.chord):
+        if re.search(r'9[\+\#]', self.chord):
             return self.tonic + 15
-        if re.search(r'[\-b]9', self.chord):
+        if re.search(r'9[\-b]', self.chord):
             return self.tonic + 13
         if re.search(r'9', self.chord):
             return self.tonic + 14
 
     @property
     def eleventh(self) -> TNote:
         """Eleventh XI."""
-        if re.search(r'[\+#]11', self.chord):
+        if re.search(r'11[\+#]', self.chord):
             return self.tonic + 18
-        if re.search(r'[\-b]11', self.chord):
+        if re.search(r'11[\-b]', self.chord):
             return self.tonic + 16
         if re.search(r'11', self.chord):
             return self.tonic + 17
 
     @property
     def thirteenth(self) -> TNote:
         """Thirteenth XIII."""
-        if re.search(r'[\+#]13', self.chord):
+        if re.search(r'13[\+#]', self.chord):
             return self.tonic + 22
-        if re.search(r'[\-b]13', self.chord):
+        if re.search(r'13[\-b]', self.chord):
             return self.tonic + 20
         if re.search(r'13', self.chord):
             return self.tonic + 21
 
 
 class __chords__:  # noqa: N801
     """
```

### Comparing `foxdotchord-0.0.3b0/.gitignore` & `foxdotchord-0.0.4b0/.gitignore`

 * *Files identical despite different names*

### Comparing `foxdotchord-0.0.3b0/LICENSE` & `foxdotchord-0.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxdotchord-0.0.3b0/README.md` & `foxdotchord-0.0.4b0/README.md`

 * *Files identical despite different names*

### Comparing `foxdotchord-0.0.3b0/pyproject.toml` & `foxdotchord-0.0.4b0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FoxDotChord"
 description = "Chords for use in FoxDot"
-version = "0.0.3b0"
+version = "0.0.4b0"
 authors = [{ name = "taconi", email = "igor.taconi@protonmail.com" }]
 maintainers = [{ name = "taconi", email = "igor.taconi@protonmail.com" }]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords = ["FoxDot", "foxdot", "chord"]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
@@ -46,29 +46,30 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["FoxDotChord/"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
-[tool.hatch.envs.test]
+[tool.hatch.envs.hatch-test]
 dependencies = [
   "pytest>=8.0.2",
   "pytest-clarity>=1.0.1",
   "pytest-cov>=4.1.0",
+  "pytest-sugar>=1.0.0",
   "FoxDot @ git+https://gitlab.com/iShapeNoise/foxdot",
 ]
 
-[tool.hatch.envs.test.scripts]
-test = """
-pytest --cov=FoxDotChord/ --doctest-modules
-coverage report
-"""
+[tool.hatch.envs.hatch-test.scripts]
+run = [
+  "pytest --cov=FoxDotChord/ --doctest-modules {args}",
+  "coverage report",
+]
 
-[[tool.hatch.envs.test.matrix]]
+[[tool.hatch.envs.hatch-test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.pytest.ini_options]
 addopts = "-vv --diff-symbols --cache-clear --cov-report html --cov-config pyproject.toml"
 filterwarnings = ["ignore::DeprecationWarning"]
 
 [tool.coverage.run]
```

### Comparing `foxdotchord-0.0.3b0/PKG-INFO` & `foxdotchord-0.0.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoxDotChord
-Version: 0.0.3b0
+Version: 0.0.4b0
 Summary: Chords for use in FoxDot
 Project-URL: Homepage, https://codeberg.com/taconi/FoxDotChord
 Project-URL: Documentation, https://foxdotchord.readthedocs.io
 Project-URL: Repository, https://codeberg.com/taconi/FoxDotChord
 Project-URL: Contributor Guide, https://foxdotchord.readthedocs.io/contributing
 Project-URL: Issue tracker, https://codeberg.com/taconi/FoxDotChord/issues
 Author-email: taconi <igor.taconi@protonmail.com>
```

