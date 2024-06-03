# Comparing `tmp/itemloaders-1.3.0.tar.gz` & `tmp/itemloaders-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itemloaders-1.3.0.tar", last modified: Thu May 30 11:09:35 2024, max compression
+gzip compressed data, was "itemloaders-1.3.1.tar", last modified: Mon Jun  3 12:25:04 2024, max compression
```

## Comparing `itemloaders-1.3.0.tar` & `itemloaders-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.991864 itemloaders-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-30 11:09:20.000000 itemloaders-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 11:09:20.000000 itemloaders-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-30 11:09:35.991864 itemloaders-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-30 11:09:20.000000 itemloaders-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.987864 itemloaders-1.3.0/itemloaders/
--rw-r--r--   0 runner    (1001) docker     (127)    22988 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-30 11:09:20.000000 itemloaders-1.3.0/itemloaders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.991864 itemloaders-1.3.0/itemloaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 11:09:35.000000 itemloaders-1.3.0/itemloaders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 11:09:35.991864 itemloaders-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 11:09:20.000000 itemloaders-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:09:35.991864 itemloaders-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_base_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_loader_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_nested_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_nested_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_output_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_select_jmes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_selector_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-30 11:09:20.000000 itemloaders-1.3.0/tests/test_utils_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:25:04.413739 itemloaders-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-06-03 12:24:50.000000 itemloaders-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 12:24:50.000000 itemloaders-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-06-03 12:25:04.413739 itemloaders-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-06-03 12:24:50.000000 itemloaders-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:25:04.413739 itemloaders-1.3.1/itemloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    23048 2024-06-03 12:24:50.000000 itemloaders-1.3.1/itemloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-06-03 12:24:50.000000 itemloaders-1.3.1/itemloaders/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-06-03 12:24:50.000000 itemloaders-1.3.1/itemloaders/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 12:24:50.000000 itemloaders-1.3.1/itemloaders/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-06-03 12:24:50.000000 itemloaders-1.3.1/itemloaders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:25:04.413739 itemloaders-1.3.1/itemloaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-06-03 12:25:04.000000 itemloaders-1.3.1/itemloaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-03 12:25:04.000000 itemloaders-1.3.1/itemloaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:25:04.000000 itemloaders-1.3.1/itemloaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:25:04.000000 itemloaders-1.3.1/itemloaders.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-03 12:25:04.000000 itemloaders-1.3.1/itemloaders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-03 12:25:04.000000 itemloaders-1.3.1/itemloaders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-06-03 12:25:04.417739 itemloaders-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-06-03 12:24:50.000000 itemloaders-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:25:04.413739 itemloaders-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17800 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_base_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_loader_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_nested_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_nested_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_output_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_select_jmes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_selector_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-06-03 12:24:50.000000 itemloaders-1.3.1/tests/test_utils_python.py
```

### Comparing `itemloaders-1.3.0/LICENSE` & `itemloaders-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/PKG-INFO` & `itemloaders-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.3.0
+Version: 1.3.1
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.3.0 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.3.1 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `itemloaders-1.3.0/README.rst` & `itemloaders-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/itemloaders/__init__.py` & `itemloaders-1.3.1/itemloaders/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,30 +159,30 @@
         Create a nested loader with an xpath selector.
         The supplied selector is applied relative to selector associated
         with this :class:`ItemLoader`. The nested loader shares the item
         with the parent :class:`ItemLoader` so calls to :meth:`add_xpath`,
         :meth:`add_value`, :meth:`replace_value`, etc. will behave as expected.
         """
         self._check_selector_method()
-        assert self.selector
+        assert self.selector is not None
         selector = self.selector.xpath(xpath)
         context.update(selector=selector)
         subloader = self.__class__(item=self.item, parent=self, **context)
         return subloader
 
     def nested_css(self, css: str, **context: Any) -> Self:
         """
         Create a nested loader with a css selector.
         The supplied selector is applied relative to selector associated
         with this :class:`ItemLoader`. The nested loader shares the item
         with the parent :class:`ItemLoader` so calls to :meth:`add_xpath`,
         :meth:`add_value`, :meth:`replace_value`, etc. will behave as expected.
         """
         self._check_selector_method()
-        assert self.selector
+        assert self.selector is not None
         selector = self.selector.css(css)
         context.update(selector=selector)
         subloader = self.__class__(item=self.item, parent=self, **context)
         return subloader
 
     def add_value(
         self,
@@ -469,15 +469,15 @@
         values = self._get_xpathvalues(xpath, **kw)
         return self.get_value(values, *processors, re=re, **kw)
 
     def _get_xpathvalues(
         self, xpaths: Union[str, Iterable[str]], **kw: Any
     ) -> List[Any]:
         self._check_selector_method()
-        assert self.selector
+        assert self.selector is not None
         xpaths = arg_to_iter(xpaths)
         return flatten(self.selector.xpath(xpath, **kw).getall() for xpath in xpaths)
 
     def add_css(
         self,
         field_name: Optional[str],
         css: Union[str, Iterable[str]],
@@ -554,15 +554,15 @@
             loader.get_css('p#price', TakeFirst(), re='the price is (.*)')
         """
         values = self._get_cssvalues(css)
         return self.get_value(values, *processors, re=re, **kw)
 
     def _get_cssvalues(self, csss: Union[str, Iterable[str]]) -> List[Any]:
         self._check_selector_method()
-        assert self.selector
+        assert self.selector is not None
         csss = arg_to_iter(csss)
         return flatten(self.selector.css(css).getall() for css in csss)
 
     def add_jmes(
         self,
         field_name: Optional[str],
         jmes: str,
@@ -637,14 +637,14 @@
             loader.get_jmes('price', TakeFirst(), re='the price is (.*)')
         """
         values = self._get_jmesvalues(jmes)
         return self.get_value(values, *processors, re=re, **kw)
 
     def _get_jmesvalues(self, jmess: Union[str, Iterable[str]]) -> List[Any]:
         self._check_selector_method()
-        assert self.selector
+        assert self.selector is not None
         jmess = arg_to_iter(jmess)
         if not hasattr(self.selector, "jmespath"):
             raise AttributeError(
                 "Please install parsel >= 1.8.1 to get jmespath support"
             )
         return flatten(self.selector.jmespath(jmes).getall() for jmes in jmess)
```

### Comparing `itemloaders-1.3.0/itemloaders/common.py` & `itemloaders-1.3.1/itemloaders/common.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/itemloaders/processors.py` & `itemloaders-1.3.1/itemloaders/processors.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/itemloaders/utils.py` & `itemloaders-1.3.1/itemloaders/utils.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/itemloaders.egg-info/PKG-INFO` & `itemloaders-1.3.1/itemloaders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itemloaders
-Version: 1.3.0
+Version: 1.3.1
 Summary: Base library for scrapy's ItemLoader
 Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte
 Author-email: opensource@zyte.com
 License: BSD
 Project-URL: Documentation, https://itemloaders.readthedocs.io/
 Project-URL: Source, https://github.com/scrapy/itemloaders
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: itemloaders Version: 1.3.0 Summary: Base library
+Metadata-Version: 2.1 Name: itemloaders Version: 1.3.1 Summary: Base library
 for scrapy's ItemLoader Home-page: https://github.com/scrapy/itemloaders
 Author: Zyte Author-email: opensource@zyte.com License: BSD Project-URL:
 Documentation, https://itemloaders.readthedocs.io/ Project-URL: Source, https:/
 /github.com/scrapy/itemloaders Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `itemloaders-1.3.0/itemloaders.egg-info/SOURCES.txt` & `itemloaders-1.3.1/itemloaders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/setup.py` & `itemloaders-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="itemloaders",
-    version="1.3.0",
+    version="1.3.1",
     url="https://github.com/scrapy/itemloaders",
     project_urls={
         "Documentation": "https://itemloaders.readthedocs.io/",
         "Source": "https://github.com/scrapy/itemloaders",
     },
     description="Base library for scrapy's ItemLoader",
     long_description=long_description,
```

### Comparing `itemloaders-1.3.0/tests/test_base_loader.py` & `itemloaders-1.3.1/tests/test_base_loader.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_loader_initialization.py` & `itemloaders-1.3.1/tests/test_loader_initialization.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_nested_items.py` & `itemloaders-1.3.1/tests/test_nested_items.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_nested_loader.py` & `itemloaders-1.3.1/tests/test_nested_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,7 +113,17 @@
         assert item is loader.item
         assert item is nl1.item
         assert item is nl2.item
 
         self.assertEqual(item["name"], ["marta"])
         self.assertEqual(item["url"], ["http://www.scrapy.org"])
         self.assertEqual(item["image"], ["/images/logo.png"])
+
+    def test_nested_empty_selector(self):
+        loader = ItemLoader(selector=self.selector)
+        nested_xpath = loader.nested_xpath("//bar")
+        assert isinstance(nested_xpath, ItemLoader)
+        nested_xpath.add_xpath("foo", "./foo")
+
+        nested_css = loader.nested_css("bar")
+        assert isinstance(nested_css, ItemLoader)
+        nested_css.add_css("foo", "foo")
```

### Comparing `itemloaders-1.3.0/tests/test_output_processor.py` & `itemloaders-1.3.1/tests/test_output_processor.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_processors.py` & `itemloaders-1.3.1/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_select_jmes.py` & `itemloaders-1.3.1/tests/test_select_jmes.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_selector_loader.py` & `itemloaders-1.3.1/tests/test_selector_loader.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_utils_misc.py` & `itemloaders-1.3.1/tests/test_utils_misc.py`

 * *Files identical despite different names*

### Comparing `itemloaders-1.3.0/tests/test_utils_python.py` & `itemloaders-1.3.1/tests/test_utils_python.py`

 * *Files identical despite different names*

