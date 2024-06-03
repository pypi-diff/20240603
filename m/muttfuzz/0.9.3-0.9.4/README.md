# Comparing `tmp/muttfuzz-0.9.3-py3-none-any.whl.zip` & `tmp/muttfuzz-0.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11422 bytes, number of entries: 8
+Zip file size: 11426 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     6027 b- defN 24-Jun-03 14:58 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx    12333 b- defN 24-Jun-03 15:01 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx    12378 b- defN 24-Jun-03 15:03 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     7957 b- defN 24-Jun-03 14:54 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/RECORD
-8 files, 34043 bytes uncompressed, 10338 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-Jun-03 15:03 muttfuzz-0.9.4.dist-info/RECORD
+8 files, 34088 bytes uncompressed, 10342 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.9.3.dist-info/METADATA
+Filename: muttfuzz-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.9.3.dist-info/WHEEL
+Filename: muttfuzz-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.9.3.dist-info/entry_points.txt
+Filename: muttfuzz-0.9.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.9.3.dist-info/top_level.txt
+Filename: muttfuzz-0.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.9.3.dist-info/RECORD
+Filename: muttfuzz-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzzutil.py

```diff
@@ -179,15 +179,15 @@
                 if verbose:
                     print()
                     print("=" * 40)
                     print("CHECKING REACHABILITY")
                 reachability_checks += 1.0
                 os.rename(reachability_filename, executable)
                 subprocess.check_call(['chmod', '+x', executable])
-                r = silent_run_with_timeout(reachability_check_cmd, reachability_check_timeout)
+                r = silent_run_with_timeout(reachability_check_cmd, reachability_check_timeout, verbose)
                 restore_executable(executable, executable_code)
                 if r == 0:
                     print("MUTANT IS NOT REACHABLE (RETURN CODE 0)")
                     mutant_ok = False
                 else:
                     reachability_hits += 1.0
                 for section in sections:
@@ -204,23 +204,23 @@
                 os.rename("/tmp/new_executable", executable)
                 subprocess.check_call(['chmod', '+x', executable])
                 if prune_mutant_cmd != "":
                     if verbose:
                         print()
                         print("=" * 40)
                         print("PRUNING MUTANT...")
-                    r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
+                    r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout, verbose)
                     if r != 0:
                         print("PRUNING CHECK FAILED WITH RETURN CODE", r)
                         mutant_ok = False
             if mutant_ok:
                 print()
                 print("FUZZING MUTANT...")
                 start_run = time.time()
-                r = silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
+                r = silent_run_with_timeout(fuzzer_cmd, time_per_mutant, verbose)
                 if score:
                     mutants_run += 1
                     if (r != 0):
                         mutants_killed += 1
                         print ("** MUTANT KILLED **")
                     else:
                         print ("** MUTANT NOT KILLED **")
@@ -235,24 +235,24 @@
                     print ("RUNNING MUTATION SCORE ON", int(mutants_run), "MUTANTS:",
                            str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
 
                 print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
                 if post_mutant_cmd != "":
                     restore_executable(executable, executable_code) # Might need original for post
                     print("RUNNING POST-MUTANT COMMAND")
-                    silent_run_with_timeout(post_mutant_cmd, post_mutant_timeout)
+                    silent_run_with_timeout(post_mutant_cmd, post_mutant_timeout, verbose)
                 if status_cmd != "":
                     restore_executable(executable, executable_code) # Might need for status
                     print("STATUS:")
                     subprocess.call(status_cmd, shell=True)
 
         print(datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'))
         print(round(time.time() - start_fuzz, 2), "ELAPSED: STARTING FINAL FUZZ")
         restore_executable(executable, executable_code)
-        silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz))
+        silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz), verbose)
         print("COMPLETED ALL FUZZING AFTER", round(time.time() - start_fuzz, 2), "SECONDS")
         if status_cmd != "":
             print("FINAL STATUS:")
             subprocess.call(status_cmd, shell=True)
 
         if reachability_check_cmd != "":
             for section in section_coverage:
```

## Comparing `muttfuzz-0.9.3.dist-info/METADATA` & `muttfuzz-0.9.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.9.3
+Version: 0.9.4
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.9.3.dist-info/RECORD` & `muttfuzz-0.9.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=7euY5JapFLUThuduCALYMN8zC7prqckNfFde68Brg0A,6027
-muttfuzz/fuzzutil.py,sha256=kjYQ5QlNTA6JwWH4988skUsDZ7TwL4kpjXP8FMBvBDw,12333
+muttfuzz/fuzzutil.py,sha256=NvhE3B9b14ITZPEp0mrn_lqjzQ3pn2OJHPNvm9jnA-c,12378
 muttfuzz/mutate.py,sha256=LuEn-n39SAkYmcqbk86Z7_PR1aiIE2n0q7H9hW1e5n0,7957
-muttfuzz-0.9.3.dist-info/METADATA,sha256=RVR1OyX8fML9tQwXxgw91hS8QPZ8XTtF6DYEOGJq0ao,6941
-muttfuzz-0.9.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.9.3.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.9.3.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.9.3.dist-info/RECORD,,
+muttfuzz-0.9.4.dist-info/METADATA,sha256=0NDDQKpR_A2IETDTabZ2ONBTe6oF9sCOU-e-7QVqD4U,6941
+muttfuzz-0.9.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.9.4.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.9.4.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.9.4.dist-info/RECORD,,
```

