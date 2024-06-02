# Comparing `tmp/language_practice-0.2.0.tar.gz` & `tmp/language_practice-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language_practice-0.2.0.tar", last modified: Mon May 27 23:39:20 2024, max compression
+gzip compressed data, was "language_practice-0.2.1.tar", last modified: Sun Jun  2 23:05:41 2024, max compression
```

## Comparing `language_practice-0.2.0.tar` & `language_practice-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.558908 language_practice-0.2.0/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1500 2024-05-27 14:47:16.000000 language_practice-0.2.0/LICENSE
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4160 2024-05-27 23:39:20.558908 language_practice-0.2.0/PKG-INFO
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3721 2024-05-27 23:33:58.000000 language_practice-0.2.0/README.md
--rwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)     1539 2024-05-27 23:33:58.000000 language_practice-0.2.0/language-practice
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.557908 language_practice-0.2.0/language_practice/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/__init__.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      895 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/cache.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4050 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/repetition.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     5805 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/terminal.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3245 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/toml.py
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.558908 language_practice-0.2.0/language_practice/web/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     2165 2024-05-27 23:33:58.000000 language_practice-0.2.0/language_practice/web/__init__.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1007 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/fr.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      748 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/ru.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      798 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/shared.py
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      434 2024-05-27 14:47:16.000000 language_practice-0.2.0/language_practice/web/uk.py
-drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 23:39:20.558908 language_practice-0.2.0/language_practice.egg-info/
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4160 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/PKG-INFO
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      553 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/SOURCES.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        1 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/dependency_links.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       41 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/requires.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       18 2024-05-27 23:39:20.000000 language_practice-0.2.0/language_practice.egg-info/top_level.txt
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      549 2024-05-27 23:39:20.559908 language_practice-0.2.0/setup.cfg
--rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       38 2024-05-27 14:47:16.000000 language_practice-0.2.0/setup.py
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-06-02 23:05:41.972655 language_practice-0.2.1/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1500 2024-05-27 14:47:16.000000 language_practice-0.2.1/LICENSE
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4160 2024-06-02 23:05:41.972655 language_practice-0.2.1/PKG-INFO
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3721 2024-05-27 23:33:58.000000 language_practice-0.2.1/README.md
+-rwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)     1539 2024-05-27 23:33:58.000000 language_practice-0.2.1/language-practice
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-06-02 23:05:41.970656 language_practice-0.2.1/language_practice/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-05-27 14:47:16.000000 language_practice-0.2.1/language_practice/__init__.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      895 2024-06-02 22:58:14.000000 language_practice-0.2.1/language_practice/cache.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4050 2024-06-02 22:58:19.000000 language_practice-0.2.1/language_practice/repetition.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     5855 2024-06-02 23:02:38.000000 language_practice-0.2.1/language_practice/terminal.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     3245 2024-05-27 23:33:58.000000 language_practice-0.2.1/language_practice/toml.py
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-06-02 23:05:41.971655 language_practice-0.2.1/language_practice/web/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     2165 2024-05-27 23:33:58.000000 language_practice-0.2.1/language_practice/web/__init__.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     1007 2024-05-27 14:47:16.000000 language_practice-0.2.1/language_practice/web/fr.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      748 2024-05-27 14:47:16.000000 language_practice-0.2.1/language_practice/web/ru.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      798 2024-05-27 14:47:16.000000 language_practice-0.2.1/language_practice/web/shared.py
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      434 2024-05-27 14:47:16.000000 language_practice-0.2.1/language_practice/web/uk.py
+drwxr-xr-x   0 jbaublitz  (1000) jbaublitz  (1000)        0 2024-06-02 23:05:41.971655 language_practice-0.2.1/language_practice.egg-info/
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)     4160 2024-06-02 23:05:41.000000 language_practice-0.2.1/language_practice.egg-info/PKG-INFO
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      553 2024-06-02 23:05:41.000000 language_practice-0.2.1/language_practice.egg-info/SOURCES.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)        1 2024-06-02 23:05:41.000000 language_practice-0.2.1/language_practice.egg-info/dependency_links.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       41 2024-06-02 23:05:41.000000 language_practice-0.2.1/language_practice.egg-info/requires.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       18 2024-06-02 23:05:41.000000 language_practice-0.2.1/language_practice.egg-info/top_level.txt
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)      549 2024-06-02 23:05:41.973656 language_practice-0.2.1/setup.cfg
+-rw-r--r--   0 jbaublitz  (1000) jbaublitz  (1000)       38 2024-05-27 14:47:16.000000 language_practice-0.2.1/setup.py
```

### Comparing `language_practice-0.2.0/LICENSE` & `language_practice-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/PKG-INFO` & `language_practice-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: language-practice
-Version: 0.2.0
+Version: 0.2.1
 Summary: Flashcard app with support for downloading inflection tables
 Home-page: https://github.com/jbaublitz/language-practice
 Author: John Baublitz
 Author-email: "john.m.baublitz@gmail.com"
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `language_practice-0.2.0/README.md` & `language_practice-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language-practice` & `language_practice-0.2.1/language-practice`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice/cache.py` & `language_practice-0.2.1/language_practice/cache.py`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice/repetition.py` & `language_practice-0.2.1/language_practice/repetition.py`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice/terminal.py` & `language_practice-0.2.1/language_practice/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,31 @@
                 ],
             )
             name = "directory"
         else:
             if not word_path.endswith(".toml"):
                 raise RuntimeError("Word file needs to be a TOML file")
 
-            (name, _) = os.path.splitext(word_path)
             self.words = TomlConfig(word_path)
+            (name, _) = os.path.splitext(os.path.basename(word_path))
+            directory = os.path.dirname(word_path)
 
-        repetition_path = f"{name}-repetition.json"
-        cache_path = f"{name}-cache.json"
+        repetition_path = f"{directory}/{name}-repetition.json"
+        cache_path = f"{directory}/{name}-cache.json"
 
         if reset:
             try:
                 os.remove(repetition_path)
                 os.remove(cache_path)
             except FileNotFoundError:
                 pass
 
         self.settings = termios.tcgetattr(sys.stdin.fileno())
 
         self.cache = Cache(cache_path)
-        self.words = TomlConfig(word_path)
         self.lang = self.words.get_lang()
         self.repetition = Repetition(repetition_path, self.words.get_words())
 
         current_word = self.repetition.peek()
         self.current_entry = self.words[current_word]
 
     async def startup(self):
```

### Comparing `language_practice-0.2.0/language_practice/toml.py` & `language_practice-0.2.1/language_practice/toml.py`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice/web/__init__.py` & `language_practice-0.2.1/language_practice/web/__init__.py`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice/web/fr.py` & `language_practice-0.2.1/language_practice/web/fr.py`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice/web/ru.py` & `language_practice-0.2.1/language_practice/web/ru.py`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice/web/shared.py` & `language_practice-0.2.1/language_practice/web/shared.py`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/language_practice.egg-info/PKG-INFO` & `language_practice-0.2.1/language_practice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: language-practice
-Version: 0.2.0
+Version: 0.2.1
 Summary: Flashcard app with support for downloading inflection tables
 Home-page: https://github.com/jbaublitz/language-practice
 Author: John Baublitz
 Author-email: "john.m.baublitz@gmail.com"
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `language_practice-0.2.0/language_practice.egg-info/SOURCES.txt` & `language_practice-0.2.1/language_practice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `language_practice-0.2.0/setup.cfg` & `language_practice-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 author = John Baublitz
 author_email = "john.m.baublitz@gmail.com"
 url = https://github.com/jbaublitz/language-practice
 description = Flashcard app with support for downloading inflection tables
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
-version = 0.2.0
+version = 0.2.1
 
 [options]
 install_requires = 
 	aiohttp
 	beautifulsoup4
 	requests
 	tabulate
```

