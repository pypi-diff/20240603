# Comparing `tmp/ferncrypter-1.2-py3-none-any.whl.zip` & `tmp/ferncrypter-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4284 bytes, number of entries: 6
--rwxrwxr-x  2.0 unx     6782 b- defN 24-May-31 10:16 ferncrypter-1.2.data/scripts/ferncrypter
--rw-rw-r--  2.0 unx     1073 b- defN 24-May-31 10:16 ferncrypter-1.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1334 b- defN 24-May-31 10:16 ferncrypter-1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-31 10:16 ferncrypter-1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-May-31 10:16 ferncrypter-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      492 b- defN 24-May-31 10:16 ferncrypter-1.2.dist-info/RECORD
-6 files, 9774 bytes uncompressed, 3388 bytes compressed:  65.3%
+Zip file size: 4294 bytes, number of entries: 6
+-rwxrwxr-x  2.0 unx     6791 b- defN 24-Jun-03 05:56 ferncrypter-1.3.data/scripts/ferncrypter
+-rw-rw-r--  2.0 unx     1073 b- defN 24-Jun-03 05:56 ferncrypter-1.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1334 b- defN 24-Jun-03 05:56 ferncrypter-1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Jun-03 05:56 ferncrypter-1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-Jun-03 05:56 ferncrypter-1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      492 b- defN 24-Jun-03 05:56 ferncrypter-1.3.dist-info/RECORD
+6 files, 9783 bytes uncompressed, 3398 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: ferncrypter-1.2.data/scripts/ferncrypter
+Filename: ferncrypter-1.3.data/scripts/ferncrypter
 Comment: 
 
-Filename: ferncrypter-1.2.dist-info/LICENSE
+Filename: ferncrypter-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: ferncrypter-1.2.dist-info/METADATA
+Filename: ferncrypter-1.3.dist-info/METADATA
 Comment: 
 
-Filename: ferncrypter-1.2.dist-info/WHEEL
+Filename: ferncrypter-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: ferncrypter-1.2.dist-info/top_level.txt
+Filename: ferncrypter-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ferncrypter-1.2.dist-info/RECORD
+Filename: ferncrypter-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ferncrypter-1.2.data/scripts/ferncrypter` & `ferncrypter-1.3.data/scripts/ferncrypter`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         "-k",
         "--key",
         action="store",
         dest="key",
         default=0,
         help="specify key file or key",
     )
-    # parser.add_argument("")
     return [
         (parser.parse_args().environment),
         (parser.parse_args().decrypt),
         (parser.parse_args().key),
     ]
 
 
@@ -136,14 +135,15 @@
 
 def decrypt(key, env_file):
     print("Decrypting...")
     message = open_read(env_file, "rb")
     fernet = Fernet(key)
     try:
         message = fernet.decrypt(message).decode()
+        print("Decryption Successful")
     except Exception:
         print("Decryption failed")
         quit()
     return message
 
 
 def decrypt_open(key, env_file):
```

## Comparing `ferncrypter-1.2.dist-info/LICENSE` & `ferncrypter-1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ferncrypter-1.2.dist-info/METADATA` & `ferncrypter-1.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferncrypter
-Version: 1.2
+Version: 1.3
 Summary: A utility to encrypt and decrypt env variables
 Home-page: https://github.com/abhiramsreekumar
 Author: Abhiram Sreekumar
 Author-email: ferncrypter@randomsasi.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

