# Comparing `tmp/bipsea-0.3.0.tar.gz` & `tmp/bipsea-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipsea-0.3.0.tar", last modified: Mon Jun  3 04:27:47 2024, max compression
+gzip compressed data, was "bipsea-0.3.1.tar", last modified: Mon Jun  3 05:29:40 2024, max compression
```

## Comparing `bipsea-0.3.0.tar` & `bipsea-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.157576 bipsea-0.3.0/
--rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.3.0/LICENSE.md
--rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-03 04:27:47.157374 bipsea-0.3.0/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)    11170 2024-06-03 04:27:37.000000 bipsea-0.3.0/README.md
--rw-r--r--   0 akarve     (501) staff       (20)       38 2024-06-03 04:27:47.157618 bipsea-0.3.0/setup.cfg
--rw-r--r--   0 akarve     (501) staff       (20)     1285 2024-06-01 03:17:12.000000 bipsea-0.3.0/setup.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.154015 bipsea-0.3.0/src/
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.155528 bipsea-0.3.0/src/bipsea/
--rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.3.0/src/bipsea/__init__.py
--rw-r--r--   0 akarve     (501) staff       (20)     8024 2024-06-01 14:56:06.000000 bipsea-0.3.0/src/bipsea/bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.3.0/src/bipsea/bip32types.py
--rw-r--r--   0 akarve     (501) staff       (20)     4734 2024-06-03 04:27:37.000000 bipsea-0.3.0/src/bipsea/bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     6838 2024-06-02 02:04:57.000000 bipsea-0.3.0/src/bipsea/bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     8047 2024-06-03 04:27:37.000000 bipsea-0.3.0/src/bipsea/bipsea.py
--rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.3.0/src/bipsea/english.txt
--rw-r--r--   0 akarve     (501) staff       (20)     1763 2024-06-03 04:27:37.000000 bipsea-0.3.0/src/bipsea/util.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.157167 bipsea-0.3.0/src/bipsea.egg-info/
--rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)      503 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/SOURCES.txt
--rw-r--r--   0 akarve     (501) staff       (20)        1 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/dependency_links.txt
--rw-r--r--   0 akarve     (501) staff       (20)       45 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/entry_points.txt
--rw-r--r--   0 akarve     (501) staff       (20)       26 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/requires.txt
--rw-r--r--   0 akarve     (501) staff       (20)        7 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/top_level.txt
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.156978 bipsea-0.3.0/tests/
--rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-06-03 01:47:51.000000 bipsea-0.3.0/tests/test_bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3038 2024-06-03 04:27:37.000000 bipsea-0.3.0/tests/test_bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     5010 2024-06-01 01:30:56.000000 bipsea-0.3.0/tests/test_bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     7752 2024-06-03 04:27:37.000000 bipsea-0.3.0/tests/test_cli.py
--rw-r--r--   0 akarve     (501) staff       (20)     1102 2024-06-02 02:04:57.000000 bipsea-0.3.0/tests/test_util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 05:29:40.050161 bipsea-0.3.1/
+-rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.3.1/LICENSE.md
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-03 05:29:40.049950 bipsea-0.3.1/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)    11170 2024-06-03 04:27:37.000000 bipsea-0.3.1/README.md
+-rw-r--r--   0 akarve     (501) staff       (20)       38 2024-06-03 05:29:40.050214 bipsea-0.3.1/setup.cfg
+-rw-r--r--   0 akarve     (501) staff       (20)     1285 2024-06-01 03:17:12.000000 bipsea-0.3.1/setup.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 05:29:40.046557 bipsea-0.3.1/src/
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 05:29:40.048190 bipsea-0.3.1/src/bipsea/
+-rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.3.1/src/bipsea/__init__.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8024 2024-06-01 14:56:06.000000 bipsea-0.3.1/src/bipsea/bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.3.1/src/bipsea/bip32types.py
+-rw-r--r--   0 akarve     (501) staff       (20)     4734 2024-06-03 04:27:37.000000 bipsea-0.3.1/src/bipsea/bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     6838 2024-06-02 02:04:57.000000 bipsea-0.3.1/src/bipsea/bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8004 2024-06-03 05:29:05.000000 bipsea-0.3.1/src/bipsea/bipsea.py
+-rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.3.1/src/bipsea/english.txt
+-rw-r--r--   0 akarve     (501) staff       (20)     1856 2024-06-03 05:29:05.000000 bipsea-0.3.1/src/bipsea/util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 05:29:40.049740 bipsea-0.3.1/src/bipsea.egg-info/
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-03 05:29:40.000000 bipsea-0.3.1/src/bipsea.egg-info/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)      503 2024-06-03 05:29:40.000000 bipsea-0.3.1/src/bipsea.egg-info/SOURCES.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        1 2024-06-03 05:29:40.000000 bipsea-0.3.1/src/bipsea.egg-info/dependency_links.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       45 2024-06-03 05:29:40.000000 bipsea-0.3.1/src/bipsea.egg-info/entry_points.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       26 2024-06-03 05:29:40.000000 bipsea-0.3.1/src/bipsea.egg-info/requires.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        7 2024-06-03 05:29:40.000000 bipsea-0.3.1/src/bipsea.egg-info/top_level.txt
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 05:29:40.049579 bipsea-0.3.1/tests/
+-rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-06-03 01:47:51.000000 bipsea-0.3.1/tests/test_bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3038 2024-06-03 04:27:37.000000 bipsea-0.3.1/tests/test_bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     5010 2024-06-01 01:30:56.000000 bipsea-0.3.1/tests/test_bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7684 2024-06-03 05:29:05.000000 bipsea-0.3.1/tests/test_cli.py
+-rw-r--r--   0 akarve     (501) staff       (20)      969 2024-06-03 05:29:05.000000 bipsea-0.3.1/tests/test_util.py
```

### Comparing `bipsea-0.3.0/LICENSE.md` & `bipsea-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/PKG-INFO` & `bipsea-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.3.0/README.md` & `bipsea-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/setup.py` & `bipsea-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/src/bipsea/bip32.py` & `bipsea-0.3.1/src/bipsea/bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/src/bipsea/bip32types.py` & `bipsea-0.3.1/src/bipsea/bip32types.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/src/bipsea/bip39.py` & `bipsea-0.3.1/src/bipsea/bip39.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/src/bipsea/bip85.py` & `bipsea-0.3.1/src/bipsea/bip85.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/src/bipsea/bipsea.py` & `bipsea-0.3.1/src/bipsea/bipsea.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,28 +102,28 @@
 )
 def bip39_cmd(from_, input, to, number, passphrase, pretty, strict):
     number = int(number)
     input = input.strip() if input else input
     if (from_ == "rand" and input) or (from_ != "rand" and not input):
         raise click.BadOptionUsage(
             option_name="--from",
-            message="`--from words|str` requires `--input STRING`, `--from rand` forbids `--input`",
+            message="`--from words` requires `--input STRING`, `--from rand` forbids `--input`",
         )
     if from_ == "words":
         if to == "words":
             raise click.BadOptionUsage(
                 option_name="--to",
                 message="`--to words` incompatible with `--from words`",
             )
         words = normalize_list(re.split(r"\s+", input), lower=True)
         if strict:
             if not verify_seed_words("english", words):
-                raise click.BadOptionUsage(
-                    option_name="--input",
-                    message=f"Non BIP-39 words from `--input` ({' '.join(words)}) or bad BIP-39 checksum",
+                raise click.BadParameter(
+                    f"Non BIP-39 words from `--input` ({' '.join(words)}) or bad BIP-39 checksum",
+                    param_hint="--input",
                 )
         else:
             # TODO bipsea seed -f words -u "$(cat README.md)" --not-strict
             # has negative entropy :(
             implied = relative_entropy(normalize_str(input, lower=True), ASCII_INPUTS)
             if implied < MIN_REL_ENTROPY:
                 click.secho(
@@ -152,15 +152,14 @@
                 message="`--pretty` has no effect with `--to xprv`",
             )
         # TODO: we do the entropy measure for not-strict against the string
         # but that's not what we pass in here. here we pass in split on \s+
         # for compatibility with foreign languages but is it really what we should
         # do for the general case of arbitrary secrets?
         # if so then not space is not that significant... :/
-        logger.error(words)
         seed = to_master_seed(words, passphrase)
         prv = to_master_key(seed, mainnet=to == "xprv", private=True)
 
         click.echo(prv)
 
 
 cli.add_command(bip39_cmd)
```

### Comparing `bipsea-0.3.0/src/bipsea/english.txt` & `bipsea-0.3.1/src/bipsea/english.txt`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/src/bipsea/util.py` & `bipsea-0.3.1/src/bipsea/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import binascii
 import logging
 import math
 import random
 import string
 from collections import Counter
-from typing import List
+from typing import List, Sequence
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __app_name__ = "bipsea"
 
 LOGGER = __app_name__
 MIN_REL_ENTROPY = 0.51  # somewhat magic heuristic
 
 ASCII_INPUTS = set(string.printable.lower())
 FORMAT = "utf-8"
@@ -27,20 +27,22 @@
 
 def to_hex_string(data: bytes) -> str:
     return binascii.hexlify(data).decode("utf-8")
 
 
 def shannon_entropy(input: List[str], cardinality: int) -> float:
     counts = Counter(input)
-    probs = {char: count / cardinality for char, count in counts.items()}
+    total = sum(counts.values())
+    probs = {char: count / total for char, count in counts.items()}
 
     return -sum(prob * math.log(prob, 2) for prob in probs.values())
 
 
-def relative_entropy(input: List[str], universe: set):
+def relative_entropy(input: Sequence, universe: set) -> float:
+    # TODO: check if characters out of universe
     ideal = math.log(len(universe), 2)
     actual = shannon_entropy(input, len(universe))
 
     return actual / ideal
 
 
 def contains_only_ascii(lst: List[str]):
```

### Comparing `bipsea-0.3.0/src/bipsea.egg-info/PKG-INFO` & `bipsea-0.3.1/src/bipsea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.3.0/tests/test_bip32.py` & `bipsea-0.3.1/tests/test_bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/tests/test_bip39.py` & `bipsea-0.3.1/tests/test_bip39.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/tests/test_bip85.py` & `bipsea-0.3.1/tests/test_bip85.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.3.0/tests/test_cli.py` & `bipsea-0.3.1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,14 @@
 @pytest.mark.parametrize("n", N_WORDS_ALLOWED)
 def test_seed_command_from_rand(runner, n):
     for style in ("--not-pretty", "--pretty"):
         cmd = ["seed", "-t", "words", "-n", str(n), "-f", "rand"]
         cmd.append(style)
         result = runner.invoke(cli, cmd)
         output = result.output.strip()
-        logger.debug(style)
-        logger.debug(output.split(" "))
         split_on = "\n" if style == "--pretty" else " "
         assert len(output.split(split_on)) == int(n)
         assert result.exit_code == 0
 
 
 def test_seed_command_from_str(runner):
     lengths = {"short": 5, "enough": 42}
```

### Comparing `bipsea-0.3.0/tests/test_util.py` & `bipsea-0.3.1/tests/test_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,17 @@
         shannon_entropy(universe, len(universe)), math.log(len(universe), 2)
     )
 
 
 def test_relative_entropy():
     deck = deck_52()
     shuffled = shuffle(list(deck))
-    # order doesn't matter
-    assert math.isclose(relative_entropy(shuffled, deck), relative_entropy(deck, deck))
-    # cutting universe in half yields a relative entropy of about 1/2
-    assert math.isclose(relative_entropy(deck[:26], set(deck)), 0.5)
-    assert math.isclose(relative_entropy(deck[:13], set(deck)), 0.25)
+    # order doesn't matter and the deck's relative entropy is close to 1
+    assert math.isclose(relative_entropy(shuffled, deck), 1)
+    assert math.isclose(1, relative_entropy(deck, deck))
 
 
 def test_contains_only_ascii():
     universe = "".join(ASCII_INPUTS)
     assert contains_only_ascii(universe)
     with pytest.raises(ValueError):
         contains_only_ascii(universe + "ñ")
```

