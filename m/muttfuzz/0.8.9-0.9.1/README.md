# Comparing `tmp/muttfuzz-0.8.9-py3-none-any.whl.zip` & `tmp/muttfuzz-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10607 bytes, number of entries: 8
--rw-r--r--  2.0 unx     5184 b- defN 24-May-30 15:09 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx    11881 b- defN 24-May-30 15:09 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     6630 b- defN 24-May-30 15:09 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/RECORD
-8 files, 31421 bytes uncompressed, 9523 bytes compressed:  69.7%
+Zip file size: 11421 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     6027 b- defN 24-Jun-03 14:54 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx    12331 b- defN 24-Jun-03 14:54 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx     7957 b- defN 24-Jun-03 14:54 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 14:54 muttfuzz-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 14:54 muttfuzz-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-Jun-03 14:54 muttfuzz-0.9.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Jun-03 14:54 muttfuzz-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-Jun-03 14:54 muttfuzz-0.9.1.dist-info/RECORD
+8 files, 34041 bytes uncompressed, 10337 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.8.9.dist-info/METADATA
+Filename: muttfuzz-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.8.9.dist-info/WHEEL
+Filename: muttfuzz-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.8.9.dist-info/entry_points.txt
+Filename: muttfuzz-0.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.8.9.dist-info/top_level.txt
+Filename: muttfuzz-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.8.9.dist-info/RECORD
+Filename: muttfuzz-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -40,17 +40,25 @@
     parser.add_argument('--post_mutant_timeout', type=float, default=2.0,
                         help='timeout for post-mutant command')
     parser.add_argument('--status_cmd', type=str, default="",
                         help='command to execute to show fuzzing stats')
     parser.add_argument('--order', type=int, default=1,
                         help='mutation order (default 1)')
     parser.add_argument('-s', '--score', action='store_true',
-                        help="compute a mutation score, instead of fuzzing.")
+                        help='compute a mutation score, instead of fuzzing.')
+    parser.add_argument('--avoid_repeats', action='store_true',
+                        help='avoid using the same mutant multiple times, if possible')
+    parser.add_argument('--repeat_retries', type=int, default=20,
+                        help='number of times to retry to avoid a repeat mutant (default 20)')
     parser.add_argument('--save_mutants', type=str, default="",
                         help='directory in which to save generated mutants/checks; no saving if not provided or empty')
+    parser.add_argument('-v', '--verbose', action='store_true',
+                        help='more verbose fuzzing, with command outputs')
+    parser.add_arugment('--skip_default_avoid', action='store_true',
+                        help='do not use the default list of sections to skip (e.g. printf)')
 
     parsed_args = parser.parse_args(sys.argv[1:])
     return (parsed_args, parser)
 
 
 def make_config(pargs):
     """
@@ -84,15 +92,19 @@
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.post_mutant_timeout,
                                    config.status_cmd,
                                    config.order,
                                    config.score,
-                                   config.save_mutants)
+                                   config.avoid_repeats,
+                                   config.repeat_retries,
+                                   config.save_mutants,
+                                   config.verbose,
+                                   config.skip_default_avoid)
     except IndexError:
         print("Target binary seems to have no jumps, so mutation will not do anything!")
 
 
 
 if __name__ == "__main__":
     main()
```

## muttfuzz/fuzzutil.py

```diff
@@ -31,45 +31,58 @@
     # We do this because it could still be busy if fuzzer hasn't shut down yet
     with open("/tmp/restore_executable", 'wb') as f:
         f.write(executable_code)
     os.rename("/tmp/restore_executable", executable)
     subprocess.check_call(['chmod', '+x', executable])
 
 
-def silent_run_with_timeout(cmd, timeout):
+def silent_run_with_timeout(cmd, timeout, verbose):
+    # Allow functions instead of commands, for use as a library from a script
+    if verbose:
+        print("*" * 30)
+    if callable(cmd):
+        try:
+            if verbose:
+                print("CALLING FUNCTION", cmd)
+            with time_limit(timeout):
+                return cmd()
+        except TimeoutException:
+            print("ABORTED WITH TIMEOUT")
+            return 1 # non-zero return code may be interpreted as failure/crash/timeout
     dnull = open(os.devnull, 'w')
-    print("*" * 80)
-    print("EXECUTING", cmd)
+    if verbose:
+        print("EXECUTING", cmd)
     start_P = time.time()
     try:
         with open("cmd_errors.txt", 'w') as cmd_errors:
             P = subprocess.Popen(cmd, shell=True, preexec_fn=os.setsid,
                                  stdout=dnull, stderr=cmd_errors)
             while (P.poll() is None) and ((time.time() - start_P) < timeout):
                 time.sleep(min(0.5, timeout / 10.0)) # Allow for small timeouts
             if P.poll() is None:
                 os.killpg(os.getpgid(P.pid), signal.SIGTERM)
         with open("cmd_errors.txt", 'r') as cmd_errors:
             try:
                 cmd_errors_out = cmd_errors.read()
             except:
                 cmd_errors_out = "ERROR READING OUTPUT"
-        if len(cmd_errors_out) > 0:
+        if verbose and len(cmd_errors_out) > 0:
             print("OUTPUT (TRUNCATED TO LAST 20 LINES):")
             print("\n".join(cmd_errors_out.split("\n")[-20:]))
     finally:
         if P.poll() is None:
             print("KILLING SUBPROCESS DUE TO TIMEOUT")
             os.killpg(os.getpgid(P.pid), signal.SIGTERM)
-    print("COMPLETE IN", round(time.time() - start_P, 2), "SECONDS")
-    print("*" * 80)
+    if verbose:
+        print("COMPLETE IN", round(time.time() - start_P, 2), "SECONDS")
+        print("*" * 30)
 
     return P.returncode
 
-
+# all _cmd arguments can also be Python functions
 def fuzz_with_mutants(fuzzer_cmd, executable, budget, time_per_mutant, fraction_mutant,
                       only_mutate=[],
                       avoid_mutating=[],
                       reachability_check_cmd="",
                       reachability_check_timeout=2.0,
                       prune_mutant_cmd="",
                       prune_mutant_timeout=2.0,
@@ -77,101 +90,155 @@
                       initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
                       post_mutant_timeout=2.0,
                       status_cmd="",
                       order=1,
                       score=False,
-                      save_mutants=""):
+                      avoid_repeats=False,
+                      repeat_retries=20,
+                      save_mutants="",
+                      verbose=False,
+                      skip_default_avoid=False):
+    print("*" * 80)
+    print("STARTING MUTTFUZZ")
+    print()
     executable_code = mutate.get_code(executable)
+
+    if not skip_default_avoid:
+        avoid_mutating.extend("LLVMFuzzOneInput", "printf")
+
+    visited_mutants = {}
+
+    if score:
+        if not avoid_repeats:
+            print("WARNING: SCORE ESTIMATION WITHOUT --avoid_repeats WILL REPEAT SAMPLES")
+        mutants_run = 0.0
+        mutants_killed = 0.0
+        fraction_mutant = 1.0 # No final fuzz for mutation score estimation!
+        section_score = {}
+
+    print("READ EXECUTABLE WITH", len(executable_code), "BYTES")
     executable_jumps = mutate.get_jumps(executable, only_mutate, avoid_mutating)
-    print("FOUND", len(executable_jumps), "JUMPS")
+    print("FOUND", len(executable_jumps), "MUTABLE JUMPS IN EXECUTABLE")
     print("JUMPS BY SECTION:")
     section_jumps = {}
-    for jump in executable_jumps:
+    for loc in executable_jumps:
+        jump = executable_jumps[loc]
         if jump["section_name"] not in section_jumps:
-            section_jumps[jump["section_name"]] = [jump]
+            section_jumps[jump["section_name"]] = [(loc, jump)]
         else:
-            section_jumps[jump["section_name"]].append(jump)
+            section_jumps[jump["section_name"]].append((loc, jump))
+    if reachability_check_cmd != "":
+        section_coverage = {}
     for section in section_jumps:
         print(section, len(section_jumps[section]))
+        if reachability_check_cmd != "":
+            section_coverage[section] = (0.0, 0.0)
+        if score:
+            section_score[section] = (0.0, 0.0)
     print()
     start_fuzz = time.time()
-    mutant_no = 1
+    mutant_no = 0
     try:
         if initial_fuzz_cmd != "":
             print("=" * 10,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
             print("RUNNING INITIAL FUZZING...")
-            silent_run_with_timeout(initial_fuzz_cmd, initial_budget)
+            silent_run_with_timeout(initial_fuzz_cmd, initial_budget, verbose)
             if status_cmd != "":
                 print("INITIAL STATUS:")
                 subprocess.call(status_cmd, shell=True)
             if post_initial_cmd != "":
                 subprocess.call(post_initial_cmd, shell=True)
 
         if reachability_check_cmd != "":
             reachability_filename = "/tmp/reachability_executable"
             reachability_checks = 0.0
             reachability_hits = 0.0
         else:
             reachability_filename = ""
-        if score:
-            mutants_run = 0.0
-            mutants_killed = 0.0
-            fraction_mutant = 1.0 # No final fuzz for mutation score estimation!
         while ((time.time() - start_fuzz) - initial_budget) < (budget * fraction_mutant):
-            print("=" * 10,
+            mutant_no += 1
+            print()
+            print()
+            print()
+            print("=" * 30,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
-                  "=" * 10)
+                  "=" * 30)
             print(round(time.time() - start_fuzz, 2),
                   "ELAPSED: GENERATING MUTANT #" + str(mutant_no))
-            mutant_no += 1
             # make a new mutant of the executable; rename avoids hitting a busy executable
-            mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable", order=order,
-                               reachability_filename=reachability_filename, save_mutants=save_mutants,
-                               save_count = mutant_no)
+            sections = mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable",
+                                          order=order, reachability_filename=reachability_filename,
+                                          save_mutants=save_mutants, save_count=mutant_no,
+                                          avoid_repeats=avoid_repeats, repeat_retries=repeat_retries,
+                                          visited_mutants=visited_mutants)
             mutant_ok = True
             if reachability_check_cmd != "":
-                print("CHECKING REACHABILITY")
+                if verbose:
+                    print()
+                    print("=" * 40)
+                    print("CHECKING REACHABILITY")
                 reachability_checks += 1.0
                 os.rename(reachability_filename, executable)
                 subprocess.check_call(['chmod', '+x', executable])
                 r = silent_run_with_timeout(reachability_check_cmd, reachability_check_timeout)
                 restore_executable(executable, executable_code)
                 if r == 0:
                     print("MUTANT IS NOT REACHABLE (RETURN CODE 0)")
                     mutant_ok = False
                 else:
                     reachability_hits += 1.0
+                for section in sections:
+                    (hits, total) = section_coverage[section]
+                    if r == 0:
+                        section_coverage[section] = (hits, total + 1)
+                    else:
+                        section_coverage[section] = (hits + 1, total + 1)
+                    (hits, total) = section_coverage[section]
+                    print(section + ":", str(round((hits / total) * 100.0, 2)) + "% COVERAGE")
                 print ("RUNNING COVERAGE ESTIMATE OVER", int(reachability_checks), "MUTANTS:",
                        str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
             if mutant_ok:
                 os.rename("/tmp/new_executable", executable)
                 subprocess.check_call(['chmod', '+x', executable])
                 if prune_mutant_cmd != "":
-                    print("PRUNING MUTANT...")
+                    if verbose:
+                        print()
+                        print("=" * 40)
+                        print("PRUNING MUTANT...")
                     r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
                     if r != 0:
-                        print("CHECK FAILED WITH RETURN CODE", r)
+                        print("PRUNING CHECK FAILED WITH RETURN CODE", r)
                         mutant_ok = False
             if mutant_ok:
+                print()
                 print("FUZZING MUTANT...")
                 start_run = time.time()
                 r = silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
                 if score:
                     mutants_run += 1
                     if (r != 0):
                         mutants_killed += 1
                         print ("** MUTANT KILLED **")
                     else:
                         print ("** MUTANT NOT KILLED **")
+                    for section in sections:
+                        (kills, total) = section_score[section]
+                        if r == 0:
+                            section_score[section] = (kills, total + 1)
+                        else:
+                            section_score[section] = (kills + 1, total + 1)
+                        (kills, total) = section_score[section]
+                        print(section + ":", str(round((kills / total) * 100.0, 2)) + "% MUTATION SCORE")
                     print ("RUNNING MUTATION SCORE ON", int(mutants_run), "MUTANTS:",
                            str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
+
                 print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
                 if post_mutant_cmd != "":
                     restore_executable(executable, executable_code) # Might need original for post
                     print("RUNNING POST-MUTANT COMMAND")
                     silent_run_with_timeout(post_mutant_cmd, post_mutant_timeout)
                 if status_cmd != "":
                     restore_executable(executable, executable_code) # Might need for status
@@ -182,87 +249,35 @@
         print(round(time.time() - start_fuzz, 2), "ELAPSED: STARTING FINAL FUZZ")
         restore_executable(executable, executable_code)
         silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz))
         print("COMPLETED ALL FUZZING AFTER", round(time.time() - start_fuzz, 2), "SECONDS")
         if status_cmd != "":
             print("FINAL STATUS:")
             subprocess.call(status_cmd, shell=True)
+
         if reachability_check_cmd != "":
-            print ("FINAL COVERAGE ESTIMATE OVER", int(reachability_checks), "MUTANTS:",
+            for section in section_coverage:
+                (hits, total) = section_coverage[section]
+                if total > 0:
+                    print(section + ":", str(round((hits / total) * 100.0, 2)) + "% COVERAGE")
+                else:
+                    print(section + ": NO COVERAGE CHECKS")
+            print("FINAL COVERAGE ESTIMATE OVER", int(reachability_checks), "MUTANTS:",
                    str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
+
         if score:
-            print ("FINAL MUTATION SCORE OVER", int(mutants_run), "MUTANTS:",
-                    str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
+            for section in section_score:
+                (kills, total) = section_score[section]
+                if total > 0:
+                    print(section + ":", str(round((kills / total) * 100.0, 2)) + "% MUTATION SCORE")
+                else:
+                    print(section + ": NO MUTANTS EXECUTED")
+            if mutants_run > 0:
+                print("FINAL MUTATION SCORE OVER", int(mutants_run), "MUTANTS:",
+                        str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
+            else:
+                print("NO MUTANTS EXECUTED!")
             print ("NOTE:  MUTANTS MAY BE REDUNDANT")
-    finally:
-        # always restore the original binary!
-        restore_executable(executable, executable_code)
 
-# Currently this is not used, and is not updated to match all changes to the API!
-# It should work, but it does not support everything the command line does
-def fuzz_with_mutants_via_function(fuzzer_fn, executable, budget,
-                                   time_per_mutant, fraction_mutant,
-                                   initial_fn=None, initial_budget=0,
-                                   post_initial_fn=None,
-                                   post_mutant_fn=None,
-                                   status_fn=None, order=1):
-    executable_code = mutate.get_code(executable)
-    executable_jumps = mutate.get_jumps(executable)
-    start_fuzz = time.time()
-    mutant_no = 1
-    try:
-        if initial_fn is not None:
-            print("=" * 10,
-                  datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
-                  "=" * 10)
-            print("RUNNING INITIAL FUZZING...")
-            try:
-                with time_limit(initial_budget):
-                    initial_fn()
-            except TimeoutException:
-                pass
-            if status_fn is not None:
-                print("INITIAL STATUS:")
-                status_fn()
-            if post_initial_fn is not None:
-                post_initial_fn()
-
-        while ((time.time() - start_fuzz) - initial_budget) < (budget * fraction_mutant):
-            print("=" * 10,
-                  datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
-                  "=" * 10)
-            print(round(time.time() - start_fuzz, 2),
-                  "ELAPSED: GENERATING MUTANT #" + str(mutant_no))
-            mutant_no += 1
-            # make a new mutant of the executable; rename avoids hitting a busy executable
-            mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable", order=order)
-            os.rename("/tmp/new_executable", executable)
-            subprocess.check_call(['chmod', '+x', executable])
-            print("FUZZING MUTANT...")
-            start_run = time.time()
-            try:
-                with time_limit(time_per_mutant):
-                    fuzzer_fn()
-            except TimeoutException:
-                pass
-            print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
-            if post_mutant_fn is not None:
-                post_mutant_fn()
-            if status_fn is not None:
-                print("STATUS:")
-                status_fn()
-
-        print(datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'))
-        print(round(time.time() - start_fuzz, 2), "ELAPSED: STARTING FINAL FUZZ")
-        restore_executable(executable, executable_code)
-        try:
-            with time_limit(int(budget - (time.time() - start_fuzz))):
-                fuzzer_fn()
-        except TimeoutException:
-            pass
-        print("COMPLETED ALL FUZZING AFTER", round(time.time() - start_fuzz, 2), "SECONDS")
-        if status_fn is not None:
-            print("FINAL STATUS:")
-            status_fn()
     finally:
         # always restore the original binary!
         restore_executable(executable, executable_code)
```

## muttfuzz/mutate.py

```diff
@@ -8,15 +8,17 @@
 SHORT_FLIP = dict(zip(map(lambda x: x[0], SHORT_JUMPS[:-1]), SHORT_OPPOSITES))
 NEAR_JUMPS = list(map(bytes.fromhex, ["0F 84", "0F 85", "0F 8C", "0F 8D", "0F 8E", "0F 8F", "90 E9"]))
 NEAR_NAMES = dict(zip(NEAR_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 NEAR_OPPOSITES = list(map(bytes.fromhex, ["0F 85", "0F 84", "0F 8D", "0F 8C", "0F 8F", "0F 8E"]))
 NEAR_FLIP = dict(zip(map(lambda x: x[1], NEAR_JUMPS[:-1]), NEAR_OPPOSITES))
 
 NOP = bytes.fromhex("90") # Needed to erase a jump
+NOP_OP = NOP[0]
 HALT = bytes.fromhex("F4") # Needed for reachability check
+HALT_OP = HALT[0]
 
 # known markers for fuzzer/compiler injected instrumentation/etc.
 INST_SET = ["__afl", "__asan", "__ubsan", "__sanitizer", "__lsan", "__sancov", "AFL_"]
 INST_SET.extend(["DeepState", "deepstate"])
 
 def get_jumps(filename, only_mutate=[], avoid_mutating=[]):
     jumps = {}
@@ -91,49 +93,63 @@
             return NEAR_JUMPS[-1]
         return random.choice(list(filter(lambda j: j[1] != hexdata[1], NEAR_JUMPS[:-1])))
     else:
         if random.random() <= P_DC_JMP:
             return SHORT_JUMPS[-1]
         return random.choice(list(filter(lambda j: j[0] != hexdata[0], SHORT_JUMPS[:-1])))
 
-def pick_and_change(jumps):
-    loc = random.choice(list(jumps.keys()))
-    jump = jumps[loc]
-    changed = different_jump(jump["hexdata"])
+def pick_and_change(jumps, avoid_repeats=False, repeat_retries=20, visited_mutants={}):
+    done = False
+    tries = 0
+    while not done:
+        tries += 1
+        loc = random.choice(list(jumps.keys()))
+        jump = jumps[loc]
+        changed = different_jump(jump["hexdata"])
+        if (not avoid_repeats) or ((loc, changed) not in visited_mutants):
+            done = True
+        if tries >= repeat_retries:
+            print("WARNING: HAD TO USE REPEAT MUTANT DUE TO RUNNING OUT OF RETRIES")
+            break
+    if avoid_repeats:
+        visited_mutants[(loc, changed)] = True
+
     print("MUTATING JUMP IN", jump["section_name"], "WITH ORIGINAL OPCODE", jump["opcode"])
     print("ORIGINAL CODE:", jump["code"])
     if changed in SHORT_NAMES:
         print("CHANGING TO", SHORT_NAMES[changed])
     elif changed in NEAR_NAMES:
         print("CHANGING TO", NEAR_NAMES[changed])
     else:
         print("CHANGING TO NOPS")
     full_change = bytearray(jump["hexdata"]) # lets us write the correct set of NOPs for HALT insertion
     for i in range(len(changed)):
         full_change[i] = changed[i]
-    return (loc, changed)
+    return (jump["section_name"], loc, changed)
 
 def get_code(filename):
     with open(filename, "rb") as f:
         return bytearray(f.read())
 
-def mutant_from(code, jumps, order=1):
+def mutant_from(code, jumps, order=1, avoid_repeats=False, repeat_retries=20, visited_mutants={}):
+    sections = []
     new_code = bytearray(code)
     reach_code = bytearray(code)
     for i in range(order): # allows higher-order mutants, though can undo mutations
-        (loc, new_data) = pick_and_change(jumps)
+        (section, loc, new_data) = pick_and_change(jumps, avoid_repeats, repeat_retries, visited_mutants)
+        sections.append(section)
         for offset in range(0, len(new_data)):
             if offset == 0:
-                reach_code[loc + offset] = HALT[0]
+                reach_code[loc + offset] = HALT_OP
             else:
-                reach_code[loc + offset] = NOP[0]
+                reach_code[loc + offset] = NOP_OP
             new_code[loc + offset] = new_data[offset]
-    return (new_code, reach_code)
+    return (sections, new_code, reach_code)
 
-def mutant(filename, order=1, avoid_mutating=[]):
+def mutant(filename, order=1, avoid_mutating=[], avoid_repeats=False, repeat_retries=20, visited_mutants={}):
     return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
 
 def write_files(mutant, reach, new_filename, reachability_filename="", save_mutants="", save_count=0):
     with open(new_filename, "wb") as f:
         f.write(mutant)
     if save_mutants != "":
         with open(save_mutants + "/mutant_" + str(save_count), "wb") as f:
@@ -141,14 +157,21 @@
     if reachability_filename != "":
         with open(reachability_filename, "wb") as f:
             f.write(reach)
         if save_mutants != "":
             with open(save_mutants + "/reach_" + str(save_count), "wb") as f:
                 f.write(reach)
 
-def mutate_from(code, jumps, new_filename, order=1, reachability_filename="", save_mutants="", save_count=0):
-    (m, r) = mutant_from(code, jumps, order=order)
-    write_files(m, r, new_filename, reachability_filename, save_mutants, save_count)
-
-def mutate(filename, new_filename, order=1, avoid_mutating=[], reachability_filename="", save_mutants="", save_count=0):
-    (m, r) = mutant(filename, order=order, avoid_mutating=avoid_mutating)
-    write_files(m, r, new_filename, reachability_filename, save_mutants, save_count)
+def mutate_from(code, jumps, new_filename, order=1, reachability_filename="", save_mutants="", save_count=0,
+                avoid_repeats=False, repeat_retries=20, visited_mutants={}):
+    (sections, new_mutant, new_reach) = mutant_from(code, jumps, order=order, avoid_repeats=avoid_repeats,
+                                            repeat_retries=repeat_retries, visited_mutants=visited_mutants)
+    write_files(new_mutant, new_reach, new_filename, reachability_filename, save_mutants, save_count)
+    return sections
+
+def mutate(filename, new_filename, order=1, avoid_mutating=[], reachability_filename="", save_mutants="",
+           save_count=0, avoid_repeats=False, repeat_retries=20, visited_mutants={}):
+    (sections, new_mutant, new_reach) = mutant(filename, order=order, avoid_mutating=avoid_mutating,
+                                       avoid_repeats=avoid_repeats, repeat_retries=repeat_retries,
+                                       visited_mutants=visited_mutants)
+    write_files(new_mutant, new_reach, new_filename, reachability_filename, save_mutants, save_count)
+    return sections
```

## Comparing `muttfuzz-0.8.9.dist-info/METADATA` & `muttfuzz-0.9.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.8.9
+Version: 0.9.1
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.8.9.dist-info/RECORD` & `muttfuzz-0.9.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=EzlOxvZC5DmVaTccduzTez3xy6qMMV45KsEpNrqYAho,5184
-muttfuzz/fuzzutil.py,sha256=u9cIlIVVn_wjDQuE61eIvxcY1HBqpjPLBq7EY8ZrwqY,11881
-muttfuzz/mutate.py,sha256=-tBQqRM3sRiUnrJzyfgRkgSixXuNPJ-YaonvUAq0Pqc,6630
-muttfuzz-0.8.9.dist-info/METADATA,sha256=u2xCqTGgMVHmvNrnRsOxuwuXK_GhsCx_1P-u0Uu9OME,6941
-muttfuzz-0.8.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.8.9.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.8.9.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.8.9.dist-info/RECORD,,
+muttfuzz/fuzz.py,sha256=2lMymF60tKmAx_wPt-DcwknoKL46VZnXsIJGaUFk2vo,6027
+muttfuzz/fuzzutil.py,sha256=522K8Ft4R7mRuiwa97TFSGYYnqWzvJ7UDn2F82Q4TQc,12331
+muttfuzz/mutate.py,sha256=LuEn-n39SAkYmcqbk86Z7_PR1aiIE2n0q7H9hW1e5n0,7957
+muttfuzz-0.9.1.dist-info/METADATA,sha256=x1M6EocjdYJh6OCp0bp1kgjMlBgcy5HeZoR56u8FTu0,6941
+muttfuzz-0.9.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.9.1.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.9.1.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.9.1.dist-info/RECORD,,
```

