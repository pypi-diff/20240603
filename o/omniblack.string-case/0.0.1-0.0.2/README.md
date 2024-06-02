# Comparing `tmp/omniblack.string_case-0.0.1.tar.gz` & `tmp/omniblack.string_case-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniblack.string_case-0.0.1.tar", last modified: Thu May 16 00:14:17 2024, max compression
+gzip compressed data, was "omniblack.string_case-0.0.2.tar", last modified: Sun Jun  2 22:04:59 2024, max compression
```

## Comparing `omniblack.string_case-0.0.1.tar` & `omniblack.string_case-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-16 00:14:17.907068 omniblack.string_case-0.0.1/
--rw-r--r--   0 terryp    (1000) terryp    (1000)    11358 2023-02-07 20:02:33.000000 omniblack.string_case-0.0.1/LICENSE.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       27 2024-05-12 00:19:11.000000 omniblack.string_case-0.0.1/MANIFEST.in
--rw-r--r--   0 terryp    (1000) terryp    (1000)    13365 2024-05-16 00:14:17.907068 omniblack.string_case-0.0.1/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)       49 2024-05-05 19:38:31.000000 omniblack.string_case-0.0.1/package_config.yaml
--rw-r--r--   0 terryp    (1000) terryp    (1000)      624 2024-05-12 00:19:11.000000 omniblack.string_case-0.0.1/pyproject.toml
--rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-05-16 00:14:17.907068 omniblack.string_case-0.0.1/setup.cfg
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-16 00:14:17.904068 omniblack.string_case-0.0.1/src/
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-16 00:14:17.904068 omniblack.string_case-0.0.1/src/omniblack/
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-16 00:14:17.906068 omniblack.string_case-0.0.1/src/omniblack/string_case/
--rw-r--r--   0 terryp    (1000) terryp    (1000)     1737 2024-05-16 00:14:07.000000 omniblack.string_case-0.0.1/src/omniblack/string_case/__init__.py
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-16 00:14:17.906068 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/
--rw-r--r--   0 terryp    (1000) terryp    (1000)    13365 2024-05-16 00:14:17.000000 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/PKG-INFO
--rw-r--r--   0 terryp    (1000) terryp    (1000)      481 2024-05-16 00:14:17.000000 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/SOURCES.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-05-16 00:14:17.000000 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/dependency_links.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       55 2024-05-16 00:14:17.000000 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/omniblack_package.json
--rw-r--r--   0 terryp    (1000) terryp    (1000)       49 2024-04-02 00:08:32.000000 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/omniblack_package.yaml
--rw-r--r--   0 terryp    (1000) terryp    (1000)       33 2024-05-16 00:14:17.000000 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/requires.txt
--rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-05-16 00:14:17.000000 omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/top_level.txt
-drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-05-16 00:14:17.907068 omniblack.string_case-0.0.1/test/
--rw-r--r--   0 terryp    (1000) terryp    (1000)     1619 2024-05-05 19:38:31.000000 omniblack.string_case-0.0.1/test/test_string_case.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:59.463147 omniblack.string_case-0.0.2/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    11358 2023-02-07 20:02:33.000000 omniblack.string_case-0.0.2/LICENSE.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       27 2024-05-31 22:48:12.000000 omniblack.string_case-0.0.2/MANIFEST.in
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    13365 2024-06-02 22:04:59.462146 omniblack.string_case-0.0.2/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       49 2024-05-31 22:48:12.000000 omniblack.string_case-0.0.2/package_config.yaml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      624 2024-06-02 22:01:35.000000 omniblack.string_case-0.0.2/pyproject.toml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       38 2024-06-02 22:04:59.463147 omniblack.string_case-0.0.2/setup.cfg
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:59.458146 omniblack.string_case-0.0.2/src/
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:59.459146 omniblack.string_case-0.0.2/src/omniblack/
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:59.461146 omniblack.string_case-0.0.2/src/omniblack/string_case/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)     1809 2024-05-31 22:48:12.000000 omniblack.string_case-0.0.2/src/omniblack/string_case/__init__.py
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:59.461146 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)    13365 2024-06-02 22:04:59.000000 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/PKG-INFO
+-rw-r--r--   0 terryp    (1000) terryp    (1000)      481 2024-06-02 22:04:59.000000 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/SOURCES.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)        1 2024-06-02 22:04:59.000000 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/dependency_links.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       55 2024-06-02 22:04:59.000000 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/omniblack_package.json
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       49 2024-04-02 00:08:32.000000 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/omniblack_package.yaml
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       33 2024-06-02 22:04:59.000000 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/requires.txt
+-rw-r--r--   0 terryp    (1000) terryp    (1000)       10 2024-06-02 22:04:59.000000 omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/top_level.txt
+drwxr-xr-x   0 terryp    (1000) terryp    (1000)        0 2024-06-02 22:04:59.462146 omniblack.string_case-0.0.2/test/
+-rw-r--r--   0 terryp    (1000) terryp    (1000)     1970 2024-05-31 22:48:12.000000 omniblack.string_case-0.0.2/test/test_string_case.py
```

### Comparing `omniblack.string_case-0.0.1/LICENSE.txt` & `omniblack.string_case-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omniblack.string_case-0.0.1/PKG-INFO` & `omniblack.string_case-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.string_case
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Terry Patterson <Terryp@wegrok.net>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `omniblack.string_case-0.0.1/pyproject.toml` & `omniblack.string_case-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='omniblack.string_case'
-version='0.0.1'
+version='0.0.2'
 
 dependencies = [
     'omniblack.utils'
 ]
 
 [project.license]
 id = "Apache-2.0"
```

### Comparing `omniblack.string_case-0.0.1/src/omniblack/string_case/__init__.py` & `omniblack.string_case-0.0.2/src/omniblack/string_case/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import auto
-from omniblack.utils import Enum
+
 from public import public
 
+from omniblack.utils import Enum
+
 try:
     from regex import compile
     unicode_re = True
 except ImportError:
     from re import compile
     unicode_re = False
 
@@ -18,30 +20,34 @@
     word_pattern = compile(r'[\. \-_]+|(?<=[a-z])(?=[A-Z])')
 
 public(word_pattern=word_pattern)
 
 
 @public
 def words(string):
-    yield from word_pattern.split(string)
+    yield from (
+        word
+        for word in word_pattern.split(string)
+        if word
+    )
 
 
 @public
 class Cases(Enum):
     Camel = auto(), 'Camel'
     CapKebab = auto(), 'CapKebab'
     CapSnake = auto(), 'CapSnake'
     Kebab = auto(), 'Kebab'
     Pascal = auto(), 'Pascal'
     Snake = auto(), 'Snake'
     Title = auto(), 'Title'
 
     Cobol = CapKebab
 
-    def __init__(self, value, name):
+    def __init__(self, _value, name):
         self.cap_boundary = name in {'Camel', 'Pascal', 'Title'}
         self.cap_first = name in {'Pascal', 'Title'}
         self.cap_all = name in {'CapSnake', 'CapKebab'}
 
         match name:
             case 'Snake' | 'CapSnake':
                 self.seperator = '_'
@@ -57,13 +63,13 @@
             return word.title()
         elif self.cap_all:
             return word.upper()
         else:
             return word.lower()
 
     def to(self, string):
-        words = [
+        found_words = [
             self.handle_word(word, index == 0)
             for index, word in enumerate(words(string))
         ]
 
-        return self.seperator.join(words)
+        return self.seperator.join(found_words)
```

### Comparing `omniblack.string_case-0.0.1/src/omniblack.string_case.egg-info/PKG-INFO` & `omniblack.string_case-0.0.2/src/omniblack.string_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniblack.string-case
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Terry Patterson <Terryp@wegrok.net>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `omniblack.string_case-0.0.1/test/test_string_case.py` & `omniblack.string_case-0.0.2/test/test_string_case.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from omniblack.string_case import Cases
+from omniblack.string_case import Cases, words
 
 
 class Base:
     def test_from_kebab(self):
         assert self.case.to('test-test') == self.result
 
     def test_from_snake(self):
@@ -22,41 +22,64 @@
 
     def test_mixed_seperator(self):
         assert self.case.to('test.-_test') == self.result
 
     def test_mixed_case(self):
         assert self.case.to('testTest_test-Test') == self.long_result
 
+    def test_start_boundary(self):
+        assert self.case.to('__test_test') == self.result
+
+
 class TestToKebabCase(Base):
     case = Cases.Kebab
     result = 'test-test'
     long_result = 'test-test-test-test'
 
+
 class TestToCapKebabCase(Base):
     case = Cases.CapKebab
     result = 'TEST-TEST'
     long_result = 'TEST-TEST-TEST-TEST'
 
+
 class TestToSnakeCase(Base):
     case = Cases.Snake
     result = 'test_test'
     long_result = 'test_test_test_test'
 
+
 class TestToCapSnakeCase(Base):
     case = Cases.CapSnake
     result = 'TEST_TEST'
     long_result = 'TEST_TEST_TEST_TEST'
 
+
 class TestToCamelCase(Base):
     case = Cases.Camel
     result = 'testTest'
     long_result = 'testTestTestTest'
 
+
 class TestToPascalCase(Base):
     case = Cases.Pascal
     result = 'TestTest'
     long_result = 'TestTestTestTest'
 
+
 class TestToTitleCase(Base):
     case = Cases.Title
     result = 'Test Test'
     long_result = 'Test Test Test Test'
+
+
+def assert_words(_words):
+    _words = words(_words)
+    assert _words
+    for word in _words:
+        assert word
+        assert '_' not in word
+
+
+def test_words_ignore_empty():
+    assert_words('__test_test')
+    assert_words('__slots__')
```

