# Comparing `tmp/muttfuzz-0.9.2-py3-none-any.whl.zip` & `tmp/muttfuzz-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 11418 bytes, number of entries: 8
+Zip file size: 11422 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     6027 b- defN 24-Jun-03 14:58 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx    12331 b- defN 24-Jun-03 14:54 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx    12333 b- defN 24-Jun-03 15:01 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     7957 b- defN 24-Jun-03 14:54 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 14:58 muttfuzz-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 14:58 muttfuzz-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-Jun-03 14:58 muttfuzz-0.9.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Jun-03 14:58 muttfuzz-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-Jun-03 14:58 muttfuzz-0.9.2.dist-info/RECORD
-8 files, 34041 bytes uncompressed, 10334 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     6941 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-Jun-03 15:01 muttfuzz-0.9.3.dist-info/RECORD
+8 files, 34043 bytes uncompressed, 10338 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.9.2.dist-info/METADATA
+Filename: muttfuzz-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.9.2.dist-info/WHEEL
+Filename: muttfuzz-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.9.2.dist-info/entry_points.txt
+Filename: muttfuzz-0.9.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.9.2.dist-info/top_level.txt
+Filename: muttfuzz-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.9.2.dist-info/RECORD
+Filename: muttfuzz-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzzutil.py

```diff
@@ -101,15 +101,15 @@
                       skip_default_avoid=False):
     print("*" * 80)
     print("STARTING MUTTFUZZ")
     print()
     executable_code = mutate.get_code(executable)
 
     if not skip_default_avoid:
-        avoid_mutating.extend("LLVMFuzzOneInput", "printf")
+        avoid_mutating.extend(["LLVMFuzzOneInput", "printf"])
 
     visited_mutants = {}
 
     if score:
         if not avoid_repeats:
             print("WARNING: SCORE ESTIMATION WITHOUT --avoid_repeats WILL REPEAT SAMPLES")
         mutants_run = 0.0
```

## Comparing `muttfuzz-0.9.2.dist-info/METADATA` & `muttfuzz-0.9.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.9.2
+Version: 0.9.3
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.9.2.dist-info/RECORD` & `muttfuzz-0.9.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=7euY5JapFLUThuduCALYMN8zC7prqckNfFde68Brg0A,6027
-muttfuzz/fuzzutil.py,sha256=522K8Ft4R7mRuiwa97TFSGYYnqWzvJ7UDn2F82Q4TQc,12331
+muttfuzz/fuzzutil.py,sha256=kjYQ5QlNTA6JwWH4988skUsDZ7TwL4kpjXP8FMBvBDw,12333
 muttfuzz/mutate.py,sha256=LuEn-n39SAkYmcqbk86Z7_PR1aiIE2n0q7H9hW1e5n0,7957
-muttfuzz-0.9.2.dist-info/METADATA,sha256=x5cOUzLHO1s2f_yNCLHsi9hH5ZntuhOfoaN9_IwmX7Q,6941
-muttfuzz-0.9.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.9.2.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.9.2.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.9.2.dist-info/RECORD,,
+muttfuzz-0.9.3.dist-info/METADATA,sha256=RVR1OyX8fML9tQwXxgw91hS8QPZ8XTtF6DYEOGJq0ao,6941
+muttfuzz-0.9.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.9.3.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.9.3.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.9.3.dist-info/RECORD,,
```

