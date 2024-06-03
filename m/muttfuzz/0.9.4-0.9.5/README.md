# Comparing `tmp/muttfuzz-0.9.4-py3-none-any.whl.zip` & `tmp/muttfuzz-0.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11426 bytes, number of entries: 8
+Zip file size: 11463 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     6027 b- defN 24-Jun-03 14:58 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx    12378 b- defN 24-Jun-03 15:03 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx    12775 b- defN 24-Jun-03 15:30 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     7957 b- defN 24-Jun-03 14:54 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/RECORD
-8 files, 34088 bytes uncompressed, 10342 bytes compressed:  69.7%
+-rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 15:30 muttfuzz-0.9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 15:30 muttfuzz-0.9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-Jun-03 15:30 muttfuzz-0.9.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Jun-03 15:30 muttfuzz-0.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-Jun-03 15:30 muttfuzz-0.9.5.dist-info/RECORD
+8 files, 34485 bytes uncompressed, 10379 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.9.4.dist-info/METADATA
+Filename: muttfuzz-0.9.5.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.9.4.dist-info/WHEEL
+Filename: muttfuzz-0.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.9.4.dist-info/entry_points.txt
+Filename: muttfuzz-0.9.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.9.4.dist-info/top_level.txt
+Filename: muttfuzz-0.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.9.4.dist-info/RECORD
+Filename: muttfuzz-0.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzzutil.py

```diff
@@ -96,15 +96,15 @@
                       score=False,
                       avoid_repeats=False,
                       repeat_retries=20,
                       save_mutants="",
                       verbose=False,
                       skip_default_avoid=False):
     print("*" * 80)
-    print("STARTING MUTTFUZZ")
+    print("STARTING MUTTFUZZ WITH BUDGET", budget, "SECONDS")
     print()
     executable_code = mutate.get_code(executable)
 
     if not skip_default_avoid:
         avoid_mutating.extend(["LLVMFuzzOneInput", "printf"])
 
     visited_mutants = {}
@@ -257,27 +257,36 @@
         if reachability_check_cmd != "":
             for section in section_coverage:
                 (hits, total) = section_coverage[section]
                 if total > 0:
                     print(section + ":", str(round((hits / total) * 100.0, 2)) + "% COVERAGE")
                 else:
                     print(section + ": NO COVERAGE CHECKS")
-            print("FINAL COVERAGE ESTIMATE OVER", int(reachability_checks), "MUTANTS:",
-                   str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
 
         if score:
             for section in section_score:
                 (kills, total) = section_score[section]
                 if total > 0:
                     print(section + ":", str(round((kills / total) * 100.0, 2)) + "% MUTATION SCORE")
                 else:
-                    print(section + ": NO MUTANTS EXECUTED")
+                    if verbose:
+                        print(section + ": NO MUTANTS EXECUTED")
             if mutants_run > 0:
                 print("FINAL MUTATION SCORE OVER", int(mutants_run), "MUTANTS:",
                         str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
             else:
                 print("NO MUTANTS EXECUTED!")
             print ("NOTE:  MUTANTS MAY BE REDUNDANT")
 
+        if reachability_check_cmd != "":
+            print("FINAL COVERAGE ESTIMATE OVER", int(reachability_checks), "MUTANTS:",
+                  str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
+        if score:
+            if mutants_run > 0:
+                print("FINAL MUTATION SCORE OVER", int(mutants_run), "EXECUTED MUTANTS:",
+                        str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
+            else:
+                print("NO MUTANTS EXECUTED!")
+
     finally:
         # always restore the original binary!
         restore_executable(executable, executable_code)
```

## Comparing `muttfuzz-0.9.4.dist-info/METADATA` & `muttfuzz-0.9.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.9.4
+Version: 0.9.5
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

