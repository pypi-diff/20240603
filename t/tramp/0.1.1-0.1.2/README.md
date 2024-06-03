# Comparing `tmp/tramp-0.1.1.tar.gz` & `tmp/tramp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tramp-0.1.1.tar", max compression
+gzip compressed data, was "tramp-0.1.2.tar", max compression
```

## Comparing `tramp-0.1.1.tar` & `tramp-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       35 2024-05-30 23:33:01.796806 tramp-0.1.1/README.md
--rw-r--r--   0        0        0      311 2024-05-30 23:32:44.295223 tramp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      371 2024-05-30 23:23:56.025236 tramp-0.1.1/tramp/containers.py
--rw-r--r--   0        0        0     1717 2024-05-30 23:12:32.270826 tramp-0.1.1/tramp/optionals.py
--rw-r--r--   0        0        0     2641 2024-05-30 23:50:30.714838 tramp-0.1.1/tramp/results.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 tramp-0.1.1/setup.py
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 tramp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-05-30 23:33:01.796806 tramp-0.1.2/README.md
+-rw-r--r--   0        0        0      311 2024-06-03 13:04:29.397544 tramp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-05-30 23:23:56.025236 tramp-0.1.2/tramp/containers.py
+-rw-r--r--   0        0        0     1721 2024-06-03 13:04:29.398586 tramp-0.1.2/tramp/optionals.py
+-rw-r--r--   0        0        0     2641 2024-05-30 23:50:30.714838 tramp-0.1.2/tramp/results.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 tramp-0.1.2/setup.py
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 tramp-0.1.2/PKG-INFO
```

### Comparing `tramp-0.1.1/tramp/optionals.py` & `tramp-0.1.2/tramp/optionals.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 
 
 class OptionalException(Exception):
     """Base exception for errors raised by an Optional object."""
 
 
 class OptionalTypeCannotBeInstantiated(OptionalException):
-    """Raised when attempting to instantiate an Optional type that is not a value type."""
+    """Raised when attempting to instantiate an Optional type that is not a type of Some."""
 
 
 class OptionalHasNoValueException(OptionalException):
     """Raised when an Optional object has no value."""
 
 
 class Optional(Generic[V]):
-    Value: "Type[Optional[V]]"
+    Some: "Type[Optional[V]]"
     Nothing: "Optional[V]"
 
     def __new__(cls, *_):
         if cls is Optional:
             raise OptionalTypeCannotBeInstantiated(
                 "You cannot instantiate the base Optional type."
             )
 
         return super().__new__(cls)
 
     @property
     def value(self) -> V | NoReturn:
         raise OptionalHasNoValueException(
-            "You cannot Optional directly, you must use either Optional.Value or Optional.Nothing"
+            "You cannot access Optional directly, you must use either Optional.Some or Optional.Nothing"
         )
 
     def value_or(self, default: V) -> V:
         return self.value
 
     def __bool__(self):
         return False
 
 
-class Value(Optional):
+class Some(Optional):
     __match_args__ = ("value",)
 
     def __init__(self, value: V):
         self._value = value
 
     @property
     def value(self) -> V:
@@ -66,9 +66,9 @@
     def value(self) -> NoReturn:
         raise OptionalHasNoValueException("No value was set, this is Nothing")
 
     def value_or(self, default: V) -> V:
         return default
 
 
-Optional.Value = Value
+Optional.Some = Some
 Optional.Nothing = Nothing()
```

### Comparing `tramp-0.1.1/tramp/results.py` & `tramp-0.1.2/tramp/results.py`

 * *Files identical despite different names*

### Comparing `tramp-0.1.1/setup.py` & `tramp-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['tramp']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'tramp',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'No idea but we have a result type!',
     'long_description': 'No idea but we have a result type!\n',
     'author': 'Zech Zimmerman',
     'author_email': 'hi@zech.codes',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

