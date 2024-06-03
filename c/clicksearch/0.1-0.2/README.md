# Comparing `tmp/clicksearch-0.1.tar.gz` & `tmp/clicksearch-0.2.tar.gz`

## Comparing `clicksearch-0.1.tar` & `clicksearch-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 clicksearch-0.1/Makefile
--rw-r--r--   0        0        0    49915 2020-02-02 00:00:00.000000 clicksearch-0.1/clicksearch.py
--rw-r--r--   0        0        0   674899 2020-02-02 00:00:00.000000 clicksearch-0.1/sample.data
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 clicksearch-0.1/test.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 clicksearch-0.1/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 clicksearch-0.1/LICENSE
--rw-r--r--   0        0        0    30638 2020-02-02 00:00:00.000000 clicksearch-0.1/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 clicksearch-0.1/pyproject.toml
--rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 clicksearch-0.1/PKG-INFO
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 clicksearch-0.2/Makefile
+-rw-r--r--   0        0        0    50063 2020-02-02 00:00:00.000000 clicksearch-0.2/clicksearch.py
+-rw-r--r--   0        0        0   674899 2020-02-02 00:00:00.000000 clicksearch-0.2/sample.data
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 clicksearch-0.2/test.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 clicksearch-0.2/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 clicksearch-0.2/LICENSE
+-rw-r--r--   0        0        0    31425 2020-02-02 00:00:00.000000 clicksearch-0.2/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 clicksearch-0.2/pyproject.toml
+-rw-r--r--   0        0        0    33195 2020-02-02 00:00:00.000000 clicksearch-0.2/PKG-INFO
```

### Comparing `clicksearch-0.1/Makefile` & `clicksearch-0.2/Makefile`

 * *Files identical despite different names*

### Comparing `clicksearch-0.1/clicksearch.py` & `clicksearch-0.2/clicksearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -757,14 +757,15 @@
         typename: str | None = None,
         verbosity: int | None = 0,
         unlabeled: bool | object = Undefined,
         brief_format: str | None = None,
         implied: str | None = None,
         styles: dict | None = None,
         redirect_args: bool = False,
+        prefetch: Callable | None = None,
     ):
         self.default = default
         self.inclusive = inclusive
         self.skip_filters = skip_filters
         self.keyname = keyname
         self.optname = optname
         self.optalias = optalias
@@ -773,14 +774,15 @@
         self.typename = typename
         self.verbosity = verbosity
         self.unlabeled = unlabeled
         self.brief_format = brief_format
         self.implied = implied
         self.styles = styles
         self.redirect_args = redirect_args
+        self.prefetch = prefetch
 
         # Set when assigned to a model
         self.model: type[ModelBase] = None  # type: ignore
         self.fieldfilteroptions: list[ClickSearchOption] = []
 
     def __set_name__(self, owner: type[ModelBase], name: str):
         """
@@ -870,14 +872,16 @@
         * If `item` has no value for this field and `default` is given, then
           `default` is returned instead. Otherwise a `MissingField` exception
           is raised.
         * If this field has overloaded the `validate` method, it may raise an
           exception if the value cannot be converted by that method.
         """
         try:
+            if self.prefetch:
+                item = self.prefetch(item)
             value = item[self.keyname]
             if self.is_missing(value) and value != default:
                 raise MissingField(f"Value missing: {self.keyname}")
         except KeyError:
             if default is MissingField:
                 if self.default is MissingField:
                     raise MissingField(f"Value missing: {self.keyname}")
```

### Comparing `clicksearch-0.1/sample.data` & `clicksearch-0.2/sample.data`

 * *Files identical despite different names*

### Comparing `clicksearch-0.1/test.py` & `clicksearch-0.2/test.py`

 * *Files identical despite different names*

### Comparing `clicksearch-0.1/.gitignore` & `clicksearch-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `clicksearch-0.1/LICENSE` & `clicksearch-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clicksearch-0.1/README.md` & `clicksearch-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1269,10 +1269,37 @@
 Title: Sales Representative
 Gender: Male
 Salary: 2700
 
 Total count: 1
 ```
 
+#### `prefetch`
+
+Optional `Callable` that can potentially alter an `item` before `fetch` gets the field's value from it. Raise `MissingField` exception to skip the item.
+
+```python
+def can_have_salary(item):
+    if item["gender"] == "Male":
+        raise MissingField("Sorry boys!")
+    return item
+
+class Employee(ModelBase):
+    name = Text(redirect_args=True)
+    title = Text(inclusive=True)
+    gender = Choice(["Female", "Male", "Other"], inclusive=True, default="Other")
+    salary = Number(prefetch=can_have_salary)
+```
+
+```pycon
+>>> Employee.cli('', reader=employees)
+Alice Anderson: Sales Director. Female. Salary 4200.
+Bob Balderson: Sales Representative. Male.
+Charlotte Carlson: Sales Representative. Female. Salary 2200.
+Totoro: Company Mascot. Other.
+
+Total count: 4
+```
+
 #### `styles`
 
 Set the styles with which to display values of this field, as passed on to [click.style](https://click.palletsprojects.com/en/latest/api/#click.style).
```

### Comparing `clicksearch-0.1/pyproject.toml` & `clicksearch-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clicksearch"
-version = "0.1"
+version = "0.2"
 description = "Framework for CLI applications that filter data streams"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["click"]
 authors = [
   {name = "Petter Nyström", email = "jimorie@gmail.com" }
```

### Comparing `clicksearch-0.1/PKG-INFO` & `clicksearch-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: clicksearch
-Version: 0.1
+Version: 0.2
 Summary: Framework for CLI applications that filter data streams
 Project-URL: Homepage, https://github.com/jimorie/clicksearch
 Author-email: Petter Nyström <jimorie@gmail.com>
 Maintainer-email: Petter Nyström <jimorie@gmail.com>
 License: Copyright 2023 Petter Nyström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -1296,10 +1296,37 @@
 Title: Sales Representative
 Gender: Male
 Salary: 2700
 
 Total count: 1
 ```
 
+#### `prefetch`
+
+Optional `Callable` that can potentially alter an `item` before `fetch` gets the field's value from it. Raise `MissingField` exception to skip the item.
+
+```python
+def can_have_salary(item):
+    if item["gender"] == "Male":
+        raise MissingField("Sorry boys!")
+    return item
+
+class Employee(ModelBase):
+    name = Text(redirect_args=True)
+    title = Text(inclusive=True)
+    gender = Choice(["Female", "Male", "Other"], inclusive=True, default="Other")
+    salary = Number(prefetch=can_have_salary)
+```
+
+```pycon
+>>> Employee.cli('', reader=employees)
+Alice Anderson: Sales Director. Female. Salary 4200.
+Bob Balderson: Sales Representative. Male.
+Charlotte Carlson: Sales Representative. Female. Salary 2200.
+Totoro: Company Mascot. Other.
+
+Total count: 4
+```
+
 #### `styles`
 
 Set the styles with which to display values of this field, as passed on to [click.style](https://click.palletsprojects.com/en/latest/api/#click.style).
```

