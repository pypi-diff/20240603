# Comparing `tmp/lang-1.0.4.tar.gz` & `tmp/lang-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lang-1.0.4.tar", last modified: Fri Jan  8 16:26:47 2016, max compression
+gzip compressed data, was "dist/lang-1.0.5.tar", last modified: Fri Jan  8 16:35:00 2016, max compression
```

## Comparing `lang-1.0.4.tar` & `lang-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 amit       (501) staff       (20)        0 2016-01-08 16:26:47.000000 lang-1.0.4/
-drwxr-xr-x   0 amit       (501) staff       (20)        0 2016-01-08 16:26:47.000000 lang-1.0.4/lang/
--rw-r--r--   0 amit       (501) staff       (20)       18 2016-01-05 20:48:23.000000 lang-1.0.4/lang/__init__.py
--rw-r--r--   0 amit       (501) staff       (20)      287 2016-01-08 14:21:35.000000 lang-1.0.4/lang/abstract.py
--rw-r--r--   0 amit       (501) staff       (20)    12141 2016-01-06 00:02:20.000000 lang-1.0.4/lang/access.py
--rw-r--r--   0 amit       (501) staff       (20)      791 2016-01-08 16:25:41.000000 lang-1.0.4/lang/exceptions.py
--rw-r--r--   0 amit       (501) staff       (20)      548 2016-01-08 15:16:55.000000 lang-1.0.4/lang/experimental.py
--rw-r--r--   0 amit       (501) staff       (20)      319 2016-01-08 15:16:43.000000 lang-1.0.4/lang/final.py
--rw-r--r--   0 amit       (501) staff       (20)     1809 2016-01-08 14:21:46.000000 lang-1.0.4/lang/interface.py
-drwxr-xr-x   0 amit       (501) staff       (20)        0 2016-01-08 16:26:47.000000 lang-1.0.4/lang.egg-info/
--rw-r--r--   0 amit       (501) staff       (20)        1 2016-01-08 16:26:46.000000 lang-1.0.4/lang.egg-info/dependency_links.txt
--rw-r--r--   0 amit       (501) staff       (20)     4463 2016-01-08 16:26:46.000000 lang-1.0.4/lang.egg-info/PKG-INFO
--rw-r--r--   0 amit       (501) staff       (20)      241 2016-01-08 16:26:46.000000 lang-1.0.4/lang.egg-info/SOURCES.txt
--rw-r--r--   0 amit       (501) staff       (20)        5 2016-01-08 16:26:46.000000 lang-1.0.4/lang.egg-info/top_level.txt
--rw-r--r--   0 amit       (501) staff       (20)     4463 2016-01-08 16:26:47.000000 lang-1.0.4/PKG-INFO
--rw-r--r--   0 amit       (501) staff       (20)       59 2016-01-08 16:26:47.000000 lang-1.0.4/setup.cfg
--rw-r--r--   0 amit       (501) staff       (20)     1847 2016-01-08 16:22:28.000000 lang-1.0.4/setup.py
+drwxr-xr-x   0 amit       (501) staff       (20)        0 2016-01-08 16:35:00.000000 lang-1.0.5/
+drwxr-xr-x   0 amit       (501) staff       (20)        0 2016-01-08 16:35:00.000000 lang-1.0.5/lang/
+-rw-r--r--   0 amit       (501) staff       (20)       18 2016-01-05 20:48:23.000000 lang-1.0.5/lang/__init__.py
+-rw-r--r--   0 amit       (501) staff       (20)      288 2016-01-08 16:33:18.000000 lang-1.0.5/lang/abstract.py
+-rw-r--r--   0 amit       (501) staff       (20)    12141 2016-01-06 00:02:20.000000 lang-1.0.5/lang/access.py
+-rw-r--r--   0 amit       (501) staff       (20)      793 2016-01-08 16:33:18.000000 lang-1.0.5/lang/exceptions.py
+-rw-r--r--   0 amit       (501) staff       (20)      548 2016-01-08 15:16:55.000000 lang-1.0.5/lang/experimental.py
+-rw-r--r--   0 amit       (501) staff       (20)      415 2016-01-08 16:33:52.000000 lang-1.0.5/lang/final.py
+-rw-r--r--   0 amit       (501) staff       (20)     1809 2016-01-08 14:21:46.000000 lang-1.0.5/lang/interface.py
+drwxr-xr-x   0 amit       (501) staff       (20)        0 2016-01-08 16:35:00.000000 lang-1.0.5/lang.egg-info/
+-rw-r--r--   0 amit       (501) staff       (20)        1 2016-01-08 16:34:59.000000 lang-1.0.5/lang.egg-info/dependency_links.txt
+-rw-r--r--   0 amit       (501) staff       (20)     4490 2016-01-08 16:34:59.000000 lang-1.0.5/lang.egg-info/PKG-INFO
+-rw-r--r--   0 amit       (501) staff       (20)      241 2016-01-08 16:34:59.000000 lang-1.0.5/lang.egg-info/SOURCES.txt
+-rw-r--r--   0 amit       (501) staff       (20)        5 2016-01-08 16:34:59.000000 lang-1.0.5/lang.egg-info/top_level.txt
+-rw-r--r--   0 amit       (501) staff       (20)     4490 2016-01-08 16:35:00.000000 lang-1.0.5/PKG-INFO
+-rw-r--r--   0 amit       (501) staff       (20)       59 2016-01-08 16:35:00.000000 lang-1.0.5/setup.cfg
+-rw-r--r--   0 amit       (501) staff       (20)     1847 2016-01-08 16:34:48.000000 lang-1.0.5/setup.py
```

### Comparing `lang-1.0.4/lang/access.py` & `lang-1.0.5/lang/access.py`

 * *Files identical despite different names*

### Comparing `lang-1.0.4/lang/exceptions.py` & `lang-1.0.5/lang/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 class ProtectedMemberAccessException(LangException):
     MESSAGE = 'You cannot access a member of a class, that is a protected member not from inside the class.'
 
 
 class BadInterfaceImplementationException(LangException):
     MESSAGE = 'A class that was declared as an interface, had function implementations.'
 
+
 class FinalClassSubclassedException(LangException):
-    MESSAGE = 'Type is not a final class and cannot be subclassed'
+    MESSAGE = 'Type is not a final class and cannot be subclassed'
```

### Comparing `lang-1.0.4/lang/experimental.py` & `lang-1.0.5/lang/experimental.py`

 * *Files identical despite different names*

### Comparing `lang-1.0.4/lang/interface.py` & `lang-1.0.5/lang/interface.py`

 * *Files identical despite different names*

### Comparing `lang-1.0.4/lang.egg-info/PKG-INFO` & `lang-1.0.5/lang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lang
-Version: 1.0.4
+Version: 1.0.5
 Summary: Module for enforcing language constraints in Python
 Home-page: https://github.com/amitassaraf/lang
 Author: Amit Assaraf
 Author-email: soit48@gmail.com
 License: APACHE
 Description: Lang - Python Language Constraints
         =============================
@@ -64,14 +64,15 @@
         	    def size(self):
         		    ...
         
         		@size.setter
         		def size(self):
         			...
         **Interface Classes**
+        
         An interface is a class that can only implement function signatures and class members.
         
             class IBox(Interface):
         	    # or __metaclass__ = EnforceInterfaceMeta
         	    DEFAULT_HEIGHT = 10
         	    
         	    def size(self):
@@ -79,28 +80,30 @@
         		    
         		def calculate_volume(self):
         			pass
         			
         If a function is implemented that it's source is not only 'pass' then an exception is thrown.
         
         **Abstract Classes**
+        
         This exists already in python  (abc module) so I just wrapped it to be in the same package.
         
             class Box(Abstract): 
         	    # or __metaclass__ = EnforceAbstractMeta
         	    
         	    @abstract_method
         	    def i_am_abstract(self):
         		    ...
         		
         		@abstract_property
         		def size(self):
         			...
         
         **Final Classes**
+        
         Final classes are classes that cannot be subclassed
         
             class TheBestBox(object):
         	    __metaclass__ = FinalClassMeta
         
         Installation
         ----------------
```

### Comparing `lang-1.0.4/PKG-INFO` & `lang-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lang
-Version: 1.0.4
+Version: 1.0.5
 Summary: Module for enforcing language constraints in Python
 Home-page: https://github.com/amitassaraf/lang
 Author: Amit Assaraf
 Author-email: soit48@gmail.com
 License: APACHE
 Description: Lang - Python Language Constraints
         =============================
@@ -64,14 +64,15 @@
         	    def size(self):
         		    ...
         
         		@size.setter
         		def size(self):
         			...
         **Interface Classes**
+        
         An interface is a class that can only implement function signatures and class members.
         
             class IBox(Interface):
         	    # or __metaclass__ = EnforceInterfaceMeta
         	    DEFAULT_HEIGHT = 10
         	    
         	    def size(self):
@@ -79,28 +80,30 @@
         		    
         		def calculate_volume(self):
         			pass
         			
         If a function is implemented that it's source is not only 'pass' then an exception is thrown.
         
         **Abstract Classes**
+        
         This exists already in python  (abc module) so I just wrapped it to be in the same package.
         
             class Box(Abstract): 
         	    # or __metaclass__ = EnforceAbstractMeta
         	    
         	    @abstract_method
         	    def i_am_abstract(self):
         		    ...
         		
         		@abstract_property
         		def size(self):
         			...
         
         **Final Classes**
+        
         Final classes are classes that cannot be subclassed
         
             class TheBestBox(object):
         	    __metaclass__ = FinalClassMeta
         
         Installation
         ----------------
```

### Comparing `lang-1.0.4/setup.py` & `lang-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, '..', 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lang',
-    version='1.0.4',
+    version='1.0.5',
     description='Module for enforcing language constraints in Python',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/amitassaraf/lang',
 
     # Author details
```

