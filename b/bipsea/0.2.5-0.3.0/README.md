# Comparing `tmp/bipsea-0.2.5.tar.gz` & `tmp/bipsea-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipsea-0.2.5.tar", last modified: Sun Jun  2 02:05:03 2024, max compression
+gzip compressed data, was "bipsea-0.3.0.tar", last modified: Mon Jun  3 04:27:47 2024, max compression
```

## Comparing `bipsea-0.2.5.tar` & `bipsea-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-02 02:05:03.261945 bipsea-0.2.5/
--rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.2.5/LICENSE.md
--rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-02 02:05:03.261739 bipsea-0.2.5/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)    10798 2024-06-02 02:04:57.000000 bipsea-0.2.5/README.md
--rw-r--r--   0 akarve     (501) staff       (20)       38 2024-06-02 02:05:03.261987 bipsea-0.2.5/setup.cfg
--rw-r--r--   0 akarve     (501) staff       (20)     1285 2024-06-01 03:17:12.000000 bipsea-0.2.5/setup.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-02 02:05:03.258647 bipsea-0.2.5/src/
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-02 02:05:03.260121 bipsea-0.2.5/src/bipsea/
--rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.2.5/src/bipsea/__init__.py
--rw-r--r--   0 akarve     (501) staff       (20)     8024 2024-06-01 14:56:06.000000 bipsea-0.2.5/src/bipsea/bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.2.5/src/bipsea/bip32types.py
--rw-r--r--   0 akarve     (501) staff       (20)     4700 2024-06-02 02:04:57.000000 bipsea-0.2.5/src/bipsea/bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     6838 2024-06-02 02:04:57.000000 bipsea-0.2.5/src/bipsea/bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     7861 2024-06-02 02:04:57.000000 bipsea-0.2.5/src/bipsea/bipsea.py
--rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.2.5/src/bipsea/english.txt
--rw-r--r--   0 akarve     (501) staff       (20)     2242 2024-06-02 02:04:57.000000 bipsea-0.2.5/src/bipsea/util.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-02 02:05:03.261550 bipsea-0.2.5/src/bipsea.egg-info/
--rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-02 02:05:03.000000 bipsea-0.2.5/src/bipsea.egg-info/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)      503 2024-06-02 02:05:03.000000 bipsea-0.2.5/src/bipsea.egg-info/SOURCES.txt
--rw-r--r--   0 akarve     (501) staff       (20)        1 2024-06-02 02:05:03.000000 bipsea-0.2.5/src/bipsea.egg-info/dependency_links.txt
--rw-r--r--   0 akarve     (501) staff       (20)       45 2024-06-02 02:05:03.000000 bipsea-0.2.5/src/bipsea.egg-info/entry_points.txt
--rw-r--r--   0 akarve     (501) staff       (20)       26 2024-06-02 02:05:03.000000 bipsea-0.2.5/src/bipsea.egg-info/requires.txt
--rw-r--r--   0 akarve     (501) staff       (20)        7 2024-06-02 02:05:03.000000 bipsea-0.2.5/src/bipsea.egg-info/top_level.txt
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-02 02:05:03.261390 bipsea-0.2.5/tests/
--rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-05-26 22:36:53.000000 bipsea-0.2.5/tests/test_bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     3138 2024-06-01 01:30:56.000000 bipsea-0.2.5/tests/test_bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     5010 2024-06-01 01:30:56.000000 bipsea-0.2.5/tests/test_bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     7357 2024-06-02 02:04:57.000000 bipsea-0.2.5/tests/test_cli.py
--rw-r--r--   0 akarve     (501) staff       (20)     1102 2024-06-02 02:04:57.000000 bipsea-0.2.5/tests/test_util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.157576 bipsea-0.3.0/
+-rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.3.0/LICENSE.md
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-03 04:27:47.157374 bipsea-0.3.0/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)    11170 2024-06-03 04:27:37.000000 bipsea-0.3.0/README.md
+-rw-r--r--   0 akarve     (501) staff       (20)       38 2024-06-03 04:27:47.157618 bipsea-0.3.0/setup.cfg
+-rw-r--r--   0 akarve     (501) staff       (20)     1285 2024-06-01 03:17:12.000000 bipsea-0.3.0/setup.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.154015 bipsea-0.3.0/src/
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.155528 bipsea-0.3.0/src/bipsea/
+-rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 22:08:44.000000 bipsea-0.3.0/src/bipsea/__init__.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8024 2024-06-01 14:56:06.000000 bipsea-0.3.0/src/bipsea/bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 22:08:44.000000 bipsea-0.3.0/src/bipsea/bip32types.py
+-rw-r--r--   0 akarve     (501) staff       (20)     4734 2024-06-03 04:27:37.000000 bipsea-0.3.0/src/bipsea/bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     6838 2024-06-02 02:04:57.000000 bipsea-0.3.0/src/bipsea/bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8047 2024-06-03 04:27:37.000000 bipsea-0.3.0/src/bipsea/bipsea.py
+-rw-r--r--   0 akarve     (501) staff       (20)    13116 2024-05-26 22:39:38.000000 bipsea-0.3.0/src/bipsea/english.txt
+-rw-r--r--   0 akarve     (501) staff       (20)     1763 2024-06-03 04:27:37.000000 bipsea-0.3.0/src/bipsea/util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.157167 bipsea-0.3.0/src/bipsea.egg-info/
+-rw-r--r--   0 akarve     (501) staff       (20)      778 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)      503 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/SOURCES.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        1 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/dependency_links.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       45 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/entry_points.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       26 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/requires.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        7 2024-06-03 04:27:47.000000 bipsea-0.3.0/src/bipsea.egg-info/top_level.txt
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-06-03 04:27:47.156978 bipsea-0.3.0/tests/
+-rw-r--r--   0 akarve     (501) staff       (20)     1319 2024-06-03 01:47:51.000000 bipsea-0.3.0/tests/test_bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3038 2024-06-03 04:27:37.000000 bipsea-0.3.0/tests/test_bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     5010 2024-06-01 01:30:56.000000 bipsea-0.3.0/tests/test_bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7752 2024-06-03 04:27:37.000000 bipsea-0.3.0/tests/test_cli.py
+-rw-r--r--   0 akarve     (501) staff       (20)     1102 2024-06-02 02:04:57.000000 bipsea-0.3.0/tests/test_util.py
```

### Comparing `bipsea-0.2.5/LICENSE.md` & `bipsea-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/PKG-INFO` & `bipsea-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.2.5
+Version: 0.3.0
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.2.5/README.md` & `bipsea-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 and more. Consider dedicated cold hardware that runs [Tails](https://tails.net),
 never has network access, and disables
 [Intel Management Engine](https://support.system76.com/articles/intel-me/)
 and other possible backdoors.
 
 # How is this useful?
 
-BIP-85 is the foundation enables you to protect and store a _single_ master secret
+BIP-85 enables you to protect and store a _single_ master secret
 that can derive _millions of independent, multi-purpose secrets_. 
 
 BIP-85 offers the following benefits:
 
 * The security of numerous independent passwords with the operational efficiency
 of a single master password. (The master secret can be multi-factor.)
 * Uses Bitcoin's well-tested hierarchical deterministic wallet
 tree (including primitives like ECDSA and hardened children)
-* Can generate millions of new Bitcoin wallet seed words and master keys
+* Can generate millions of new mnemonic seed words and master keys
 * Can generate millions of new passwords from a single master root key
 (as an extended private key (xprv)
 and a short derivation path.
 
 Unlike a password manager, which protects many secrets with one hot secret,
 BIP-85 _derives_ many secrets from one protected secret. Therefore you only need
 to back up the derivation paths and the services they are for. You do not need to
@@ -53,15 +53,15 @@
 > for more.
 
 
 General secrets keychain with semantic derivation paths
 
 # How does it work?
 
-The root of your BIP-85 password tree is a standard Bitcoin master private key (xprv).
+The root of your BIP-85 password tree is an extended master private key (xprv).
 
 > In general, you _should not use a wallet seed with funds in it_.
 > In any case, fresh seeds are free and easy to generate with bipsea.
 
 The master key is then derived according to BIP-32 hierarchical deterministic
 wallets with a clever twist:
 the derivation path includes a purpose code (`83696968'`) followed by an _application_
@@ -150,26 +150,32 @@
 
 ```
 bipsea seed -f words -u "airport letter idea forget broccoli prefer panda food delay struggle ridge salute above want dinner"
 ```
     xprv9s21ZrQH143K3YwuXcacSSghcUfrrEyj9hTHU3a2gmr6SzPBaxmuTgKGBWtFdnnCjwGYMkU7mLvxba8FFPGLQUMvyACZTEdSCJ8uBwh5Aqs
 
 
-`--strict` ensures that the input words are from the BIP-39 list and have
-a valid checksum.
+The default switch `--strict` ensures that the input words are from the BIP-39
+list and have a valid checksum.
 
 
 ## xprv from dice rolls (or any string)
 
 ```
-bipsea seed -f str -u "123456123456123456"
+bipsea seed -f words -u "123456123456123456" --not-strict
 ```
 
     Warning: Relative entropy of input seems low (0.18). Consider more complex --input.
-    xprv9s21ZrQH143K2Sxhvzbx2vvjLxPB2tJyfh5hm7ags5UWbKRHbm7x1wyCnqN4sdGTqxbq5tJJc3vV4vd51er6WgUiUC7ma1nKtfYRNTYaCeE
+    xprv9s21ZrQH143K34TY441MbRNwzpXPfkXenXeh9VgnC74Asy19YMC1uwvxCBb1z339w8DC1P7GD5GzJPsRXMwsMcygYaG7wZwVstpVhhZR6gK
+
+You can even load the input from a file.
+
+```
+bipsea seed -f words -u "$(cat README.md)" --not-strict
+```
 
 If you are now thinking, _I could use any string to derive a master key_,
 then you're ready to learn about BIP-85 with `bipsea entropy`.
 
 > **Do not get cute and derive valuable keys or secrets from short
 > strings**. You can only stretch entropy so far.
 > **Weak entropy in, weak entropy out**.
@@ -197,33 +203,36 @@
 ```
 bipsea seed -f words -u "load kitchen smooth mass blood happy kidney orbit used process lady sudden" | bipsea entropy -n 12
 ```
     medal air cube edit offer pair source promote wrap pretty rare when
 
 Append `-i 1` (the next index above the default of `-i 0`) for new words.
 
+```
+bipsea seed -f words -u "load kitchen smooth mass blood happy kidney orbit used process lady sudden" | bipsea entropy -n 12 -i 1
+```
+
     run sea prison modify december any pottery melody aspect hero loan gown
 
 And so on for millions of possible child indexes.
 
 
 ### base64 password
 
 ```
-bipsea seed -f str -u "satoshi nakamoto" | bipsea entropy -a base85 -n 10
+bipsea seed -f words -u "satoshi nakamoto" --not-strict | bipsea entropy -a base85 -n 10
 ```
-    &TP4v7gJrH
+    pdHd=DQk9z
 
 Increment the child index for a unique fresh secret.
 
 ```
-bipsea seed -f words -i "123456123456123456" | bipsea entropy -a base85 -n 10 -i 1
+bipsea seed -f words -u "satoshi nakamoto" --not-strict | bipsea entropy -a base85 -n 10 -i 1
 ```
-
-    JP!jWK@S14
+    W>SGVF(=V6
 
 You can pipe in an existing xprv.
 
 ```
 echo "$XPRV" | bipsea entropy -a base85 -n 10
 ```
 
@@ -283,20 +292,22 @@
 ```
 
 See [Makefile](./Makefile) for more commands.
 
 
 # References
 
-1. [BIP-32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki)
-hierarchical deterministic wallets
-1. [BIP-85](https://github.com/bitcoin/bips/blob/master/bip-0085.mediawiki)
-generalized cryptographic entropy
+1. [BIP-32](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki) hierarchical deterministic wallets
+
+1. [BIP-39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki) mnemonic seed words
+
 1. [BIP-44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki)
 generalized BIP-32 paths
 
+1. [BIP-85](https://github.com/bitcoin/bips/blob/master/bip-0085.mediawiki) generalized cryptographic entropy
+
 
 # TODO
 
 * [ ] Investigate switch to secure ECDSA libs with constant-time programming and
 side-channel resistance.
     * [ ] https://cryptography.io/en/latest/
```

### Comparing `bipsea-0.2.5/setup.py` & `bipsea-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/src/bipsea/bip32.py` & `bipsea-0.3.0/src/bipsea/bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/src/bipsea/bip32types.py` & `bipsea-0.3.0/src/bipsea/bip32types.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/src/bipsea/bip39.py` & `bipsea-0.3.0/src/bipsea/bip39.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,17 @@
 
 def normalize_list(words: List[str], lower=False):
     """lower() then nfkd()"""
     return [normalize_str(w, lower) for w in words]
 
 
 def to_master_seed(mnemonic: List[str], passphrase, iterations=2048):
-    """converts english mnemonics to all lower case"""
+    """apply pbkdf2"""
+    # TODO: it's not just english
+    # TODO always lower really?
     mnemonic_nfkd = " ".join(normalize_list(mnemonic, lower=True)).encode("utf-8")
     salt_nfkd = normalize_str("mnemonic" + passphrase).encode("utf-8")
 
     return pbkdf2_hmac(
         hash_name="sha512",
         password=mnemonic_nfkd,
         salt=salt_nfkd,
```

### Comparing `bipsea-0.2.5/src/bipsea/bip85.py` & `bipsea-0.3.0/src/bipsea/bip85.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/src/bipsea/bipsea.py` & `bipsea-0.3.0/src/bipsea/bipsea.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     __version__,
     relative_entropy,
     to_hex_string,
 )
 
 SEED_FROM_VALUES = [
     "rand",
-    "str",
     "words",
 ]
 SEED_TO_VALUES = [
     "words",
     "tprv",
     "xprv",
 ]
@@ -86,84 +85,86 @@
     "-n",
     "--number",
     default="24",
     type=click.Choice(N_WORDS_ALLOWED_STR),
 )
 @click.option("-p", "--passphrase", default="")
 @click.option(
-    "--pretty", is_flag=True, default=False, help="Number and separate seed words"
+    "--pretty/--not-pretty",
+    is_flag=True,
+    default=False,
+    help="Number and newline seed words",
 )
 @click.option(
     "--strict/--not-strict",
     is_flag=True,
     default=True,
     help="Require BIP-39 English words & valid checksum from `--input`",
 )
 def bip39_cmd(from_, input, to, number, passphrase, pretty, strict):
-    if input:
-        input = input.strip()
     number = int(number)
+    input = input.strip() if input else input
     if (from_ == "rand" and input) or (from_ != "rand" and not input):
         raise click.BadOptionUsage(
             option_name="--from",
             message="`--from words|str` requires `--input STRING`, `--from rand` forbids `--input`",
         )
     if from_ == "words":
-        words = normalize_list(re.split(r"\s+", input), lower=True)
-        if strict and not verify_seed_words("english", words):
-            raise click.BadOptionUsage(
-                option_name="--input",
-                message=f"Non BIP-39 words from `--input` ({' '.join(words)}) or bad BIP-39 checksum",
-            )
-    elif from_ in ("str", "rand"):
-        if not strict:
+        if to == "words":
             raise click.BadOptionUsage(
-                option_name="--not-strict",
-                message=f"`--not-strict` requires `--from rand|str`",
+                option_name="--to",
+                message="`--to words` incompatible with `--from words`",
             )
-        if from_ == "str":
-            words = normalize_list(list(input), lower=True)
-            # TODO: this is not the right universe?
-            implied = relative_entropy(words, ASCII_INPUTS)
+        words = normalize_list(re.split(r"\s+", input), lower=True)
+        if strict:
+            if not verify_seed_words("english", words):
+                raise click.BadOptionUsage(
+                    option_name="--input",
+                    message=f"Non BIP-39 words from `--input` ({' '.join(words)}) or bad BIP-39 checksum",
+                )
+        else:
+            # TODO bipsea seed -f words -u "$(cat README.md)" --not-strict
+            # has negative entropy :(
+            implied = relative_entropy(normalize_str(input, lower=True), ASCII_INPUTS)
             if implied < MIN_REL_ENTROPY:
                 click.secho(
                     (
                         f"Warning: Relative entropy of input seems low ({implied:.2f})."
                         " Consider more complex --input."
                     ),
                     fg="yellow",
                     err=True,
                 )
-            entropy = to_master_seed(words, passphrase)
-        else:  # from_ == "rand":
-            entropy = None
-            words = entropy_to_words(n_words=number, user_entropy=entropy)
+    else:  # from_ == rand
+        entropy = None
+        words = entropy_to_words(number, entropy)
+
     if to == "words":
-        if from_ == "words":
-            raise click.BadOptionUsage(
-                option_name="--to",
-                message="`--to words` incompatible with `--from words`",
-            )
-        output = " ".join(words)
         if pretty:
             output = "\n".join(f"{i+1}) {w}" for i, w in enumerate(words))
+        else:
+            output = " ".join(words)
 
         click.echo(output)
-
-    elif to in ("tprv", "xprv"):
+    else:  # to == xprv | tprv
         if pretty:
             raise click.BadOptionUsage(
                 option_name="pretty",
                 message="`--pretty` has no effect with `--to xprv`",
             )
-        mainnet = to == "xprv"
+        # TODO: we do the entropy measure for not-strict against the string
+        # but that's not what we pass in here. here we pass in split on \s+
+        # for compatibility with foreign languages but is it really what we should
+        # do for the general case of arbitrary secrets?
+        # if so then not space is not that significant... :/
+        logger.error(words)
         seed = to_master_seed(words, passphrase)
-        kprv = to_master_key(seed, mainnet=mainnet, private=True)
+        prv = to_master_key(seed, mainnet=to == "xprv", private=True)
 
-        click.echo(kprv)
+        click.echo(prv)
 
 
 cli.add_command(bip39_cmd)
 
 
 @click.command(name="entropy", help="Derive secrets according to BIP-85")
 @click.option(
@@ -201,14 +202,15 @@
 )
 def bip85_cmd(application, number, index, special, input):
     if not input:
         stdin, _, _ = select.select([sys.stdin], [], [], TIMEOUT)
         if stdin:
             lines = sys.stdin.readlines()
             if lines:
+                # get just the last line because there might be a warning above
                 prv = lines[-1].strip()
             else:
                 no_prv()
         else:
             no_prv()
     else:
         prv = input
```

### Comparing `bipsea-0.2.5/src/bipsea/english.txt` & `bipsea-0.3.0/src/bipsea/english.txt`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/src/bipsea/util.py` & `bipsea-0.3.0/src/bipsea/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 
 import binascii
 import logging
 import math
 import random
 import string
 from collections import Counter
-from hashlib import pbkdf2_hmac
-from typing import List, Sequence
-from unicodedata import normalize as unicode_normalize
+from typing import List
 
-__version__ = "0.2.5"
+__version__ = "0.3.0"
 __app_name__ = "bipsea"
 
 LOGGER = __app_name__
 MIN_REL_ENTROPY = 0.51  # somewhat magic heuristic
 
 ASCII_INPUTS = set(string.printable.lower())
 FORMAT = "utf-8"
@@ -27,29 +25,14 @@
 logger = logging.getLogger(LOGGER)
 
 
 def to_hex_string(data: bytes) -> str:
     return binascii.hexlify(data).decode("utf-8")
 
 
-def pbkdf2(
-    mnemonic: str, passphrase: str, iterations: int = 2048, hash_name: str = "sha512"
-) -> bytes:
-    return pbkdf2_hmac(
-        hash_name=hash_name,
-        password=normalize(mnemonic),
-        salt=normalize("mnemonic" + passphrase),
-        iterations=iterations,
-    )
-
-
-def normalize(input: str) -> str:
-    return unicode_normalize(NFKD, input).encode(FORMAT)
-
-
 def shannon_entropy(input: List[str], cardinality: int) -> float:
     counts = Counter(input)
     probs = {char: count / cardinality for char, count in counts.items()}
 
     return -sum(prob * math.log(prob, 2) for prob in probs.values())
```

### Comparing `bipsea-0.2.5/src/bipsea.egg-info/PKG-INFO` & `bipsea-0.3.0/src/bipsea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.2.5
+Version: 0.3.0
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
 Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `bipsea-0.2.5/tests/test_bip32.py` & `bipsea-0.3.0/tests/test_bip32.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/tests/test_bip39.py` & `bipsea-0.3.0/tests/test_bip39.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     WORDS_FILE_HASH,
     entropy_to_words,
     to_master_seed,
     verify_seed_words,
 )
 from bipsea.util import LOGGER
 
+MNEMONIC_12 = "noodle life devote warm sponsor truck ship safe race noble royal proof"
+
 logger = logging.getLogger(LOGGER)
 
 
 @pytest.mark.parametrize(
     "language, vectors", VECTORS.items(), ids=[l for l in VECTORS.keys()]
 )
 def test_vectors(language, vectors):
@@ -31,33 +33,27 @@
         expected_seed = bytes.fromhex(seed)
         expected_words = re.split(r"\s", mnemonic)
         computed_seed = to_master_seed(expected_words, passphrase="TREZOR")
         assert expected_seed == computed_seed
         assert computed_seed != to_master_seed(expected_words, passphrase="TREZOr")
         computed_xprv = to_master_key(expected_seed, mainnet=True, private=True)
         assert str(computed_xprv) == xprv
-        if language == "english":
-            assert verify_seed_words(language, expected_words)
 
 
 def test_meta():
     """Computed BIP-39 table with ENT, CS, ENT+CS"""
     for k, v in N_WORDS_META.items():
         assert (v["entropy_bits"] % 32) == 0, "Entropy bits must be a multiple of 32"
         assert (
             v["checksum_bits"] == v["entropy_bits"] // 32
         ), "Unexpected mismatch between checksum and entropy sizes"
 
 
 def test_verify_checksum():
-    correct = (
-        "noodle life devote warm sponsor truck ship safe race noble royal proof".split(
-            " "
-        )
-    )
+    correct = MNEMONIC_12.split(" ")
     assert verify_seed_words("english", correct)
     assert not verify_seed_words("english", correct[:-1])
     assert not verify_seed_words("english", correct[:-1] + ["mix"])
 
 
 @pytest.mark.parametrize(
     "language, vectors", VECTORS.items(), ids=[l for l in VECTORS.keys()]
@@ -72,19 +68,19 @@
                 warnings.simplefilter("ignore")
             computed_words = entropy_to_words(
                 len(expected_words), user_entropy=entropy_bytes
             )
             assert expected_words == computed_words
             assert verify_seed_words("english", computed_words)
         else:
-            pytest.skip(f"{language} not supported")
+            pytest.skip(f"{language} generation not supported")
 
 
 @pytest.mark.network
-def test_words_in_bip39_wordlist():
+def test_words_against_github():
     """make sure we match github"""
     url = "https://raw.githubusercontent.com/bitcoin/bips/master/bip-0039/english.txt"
     response = requests.get(url)
     wordlist = response.text.split()
     assert all(is_normalized("NFKD", w) for w in wordlist)
     assert len(wordlist) == N_MNEMONICS
     response_hash = hashlib.sha256(response.content).hexdigest()
```

### Comparing `bipsea-0.2.5/tests/test_bip85.py` & `bipsea-0.3.0/tests/test_bip85.py`

 * *Files identical despite different names*

### Comparing `bipsea-0.2.5/tests/test_cli.py` & `bipsea-0.3.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import random
-import string
 
 import pytest
 from click.testing import CliRunner
 from data.bip39_vectors import VECTORS
 from data.bip85_vectors import BIP39, HEX, PWD_BASE85, WIF
 
 from bipsea.bipsea import N_WORDS_ALLOWED, cli
@@ -23,17 +22,16 @@
 @pytest.fixture
 def runner():
     return CliRunner()
 
 
 @pytest.mark.parametrize("language, vectors", VECTORS.items())
 def test_seed_command_to_actual_seed(runner, language, vectors):
-    for vector in vectors:
+    for vector in vectors[:1]:  # for speed since test_bip39 already covers all
         _, mnemonic, _, xprv = vector
-
         for upper in (True, False):
             # prove that case doesn't matter
             mnemonic = mnemonic.upper() if upper else mnemonic
             result = runner.invoke(
                 cli,
                 [
                     "seed",
@@ -45,96 +43,105 @@
                     mnemonic,
                     "-p",
                     "TREZOR",
                     "--strict" if language == "english" else "--not-strict",
                 ],
             )
             assert result.exit_code == 0
-            assert result.output.strip() == xprv
+            # we might get an entropy warning for foreign languages
+            # so just look at the last line
+            last = result.output.strip().split("\n")[-1]
+            assert last == xprv
 
 
 @pytest.mark.parametrize("language, vectors", VECTORS.items())
 def test_seed_option_sensitivity(runner, language, vectors):
     """prove that meaningful passphrase mnemonic changes change the xprv
     (but white space after the mnemonic doesn't)"""
-    for vector in vectors[:1]:  # one vector per language for faster tests
+    for vector in vectors[:1]:  # one vector per language for speed
         _, mnemonic, _, xprv = vector
         strictness = ["--strict"] if language == "english" else ["--not-strict"]
         change_passphrase = runner.invoke(
             cli,
             ["seed", "-t", "xprv", "-f", "words", "-u", mnemonic, "-p", "TrEZOR"]
             + strictness,
         )
         assert change_passphrase.exit_code == 0
-        assert change_passphrase.output.strip() != xprv
+        result_xprv = change_passphrase.output.strip().split("\n")[-1]
+        assert result_xprv != xprv
 
         for suffix in ("", ".", " \t\n "):
             mnemonic_ = mnemonic + suffix
             cmd = ["seed", "-f", "words", "-u", mnemonic_, "-p", "TREZOR"] + strictness
             result = runner.invoke(cli, cmd)
             if suffix == ".":
                 if language == "english":
                     assert result.exit_code != 0
                     assert "BIP-39" in result.output
             else:
                 assert result.exit_code == 0
-                assert result.output.strip() == xprv
+                result_xprv = result.output.strip().split("\n")[-1]
+                assert result_xprv == xprv
 
     if language == "english":
         testnet = runner.invoke(
             cli, ["seed", "-t", "tprv", "-f", "words", "-u", MNEMONIC_12] + strictness
         )
         assert testnet.exit_code == 0
-        tprv = testnet.output.strip()
+        tprv = testnet.output.strip().split("\n")[-1]
         assert tprv != xprv
         assert tprv.startswith("tprv")
 
 
 @pytest.mark.parametrize("n", N_WORDS_ALLOWED)
 def test_seed_command_from_rand(runner, n):
-    cmd = ["seed", "-t", "words", "-n", str(n), "-f", "rand"]
-    result = runner.invoke(cli, cmd)
-    assert len(result.output.split()) == int(n)
-    assert result.exit_code == 0
+    for style in ("--not-pretty", "--pretty"):
+        cmd = ["seed", "-t", "words", "-n", str(n), "-f", "rand"]
+        cmd.append(style)
+        result = runner.invoke(cli, cmd)
+        output = result.output.strip()
+        logger.debug(style)
+        logger.debug(output.split(" "))
+        split_on = "\n" if style == "--pretty" else " "
+        assert len(output.split(split_on)) == int(n)
+        assert result.exit_code == 0
 
 
 def test_seed_command_from_str(runner):
     lengths = {"short": 5, "enough": 42}
-    base = ["seed", "-t", "xprv"]
+    base = ["seed", "-t", "xprv", "--not-strict"]
     for k, v in lengths.items():
-        cmd = base + ["-f", "str", "-u", gen_custom_seed_words(v, 0)]
+        cmd = base + ["-f", "words", "-u", gen_custom_seed_words(v, 0)]
         result = runner.invoke(cli, cmd)
         assert result.exit_code == 0
         if k == "short":
             assert "Warning" in result.output
         else:
             assert "Warning" not in result.output
-        bad_cmd = base + ["-f", "words", "-u", gen_custom_seed_words(v, 0)]
-        bad_result = runner.invoke(cli, bad_cmd)
-        assert bad_result.exit_code != 0
-        assert "BIP-39" in bad_result.output
 
 
 def gen_custom_seed_words(length: int, seed: int):
     """non bip-39 seeds"""
     random.seed(seed)
-    custom = "".join(random.choice("".join(ASCII_INPUTS)) for _ in range(length))
+    custom = "".join(
+        random.choice("".join(sorted(list(ASCII_INPUTS)))) for _ in range(length)
+    )
 
     return custom
 
 
 def test_seed_from_and_to_words(runner):
     result = runner.invoke(cli, ["seed", "--from", "words", "--to", "words"])
     assert result.exit_code != 0
     assert "--input" in result.output
     assert "--from rand" in result.output
 
 
 def test_seed_bad_n(runner):
-    result = runner.invoke(cli, ["seed", "--from", "words", "-n", "45"])
+    result = runner.invoke(cli, ["seed", "--from", "words", "-n", "11"])
     assert result.exit_code != 0
     assert "--number" in result.output
 
 
 def test_seed_bad_from(runner):
     result = runner.invoke(cli, ["seed", "--from", "baz"])
     assert result.exit_code != 0
```

### Comparing `bipsea-0.2.5/tests/test_util.py` & `bipsea-0.3.0/tests/test_util.py`

 * *Files identical despite different names*

