# Comparing `tmp/evalidate-2.0.2.tar.gz` & `tmp/evalidate-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalidate-2.0.2.tar", last modified: Sat Jul  8 07:56:22 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `evalidate-2.0.2.tar` & `evalidate-2.0.3.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-07-08 07:56:22.914012 evalidate-2.0.2/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12326 2023-07-08 07:56:22.914012 evalidate-2.0.2/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)     9540 2023-06-22 14:53:25.000000 evalidate-2.0.2/README.md
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-07-08 07:56:22.914012 evalidate-2.0.2/evalidate/
--rwxr-xr-x   0 xenon     (1000) xenon     (1000)     4091 2023-07-08 07:54:46.000000 evalidate-2.0.2/evalidate/__init__.py
--rw-r--r--   0 xenon     (1000) xenon     (1000)     2506 2023-06-21 21:43:38.000000 evalidate-2.0.2/evalidate/security.py
-drwxr-xr-x   0 xenon     (1000) xenon     (1000)        0 2023-07-08 07:56:22.914012 evalidate-2.0.2/evalidate.egg-info/
--rw-r--r--   0 xenon     (1000) xenon     (1000)    12326 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/PKG-INFO
--rw-r--r--   0 xenon     (1000) xenon     (1000)      226 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/SOURCES.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/dependency_links.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)        1 2022-08-10 17:45:22.000000 evalidate-2.0.2/evalidate.egg-info/not-zip-safe
--rw-r--r--   0 xenon     (1000) xenon     (1000)       10 2023-07-08 07:56:22.000000 evalidate-2.0.2/evalidate.egg-info/top_level.txt
--rw-r--r--   0 xenon     (1000) xenon     (1000)       38 2023-07-08 07:56:22.914012 evalidate-2.0.2/setup.cfg
--rw-r--r--   0 xenon     (1000) xenon     (1000)     1077 2023-06-15 17:42:59.000000 evalidate-2.0.2/setup.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 evalidate-2.0.3/NOTES
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 evalidate-2.0.3/setup.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 evalidate-2.0.3/x.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 evalidate-2.0.3/xx.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 evalidate-2.0.3/xx2.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 evalidate-2.0.3/xx3.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 evalidate-2.0.3/y.py
+-rwxr-xr-x   0        0        0     2231 2020-02-02 00:00:00.000000 evalidate-2.0.3/benchmark/benchmark.py
+-rwxr-xr-x   0        0        0     4134 2020-02-02 00:00:00.000000 evalidate-2.0.3/evalidate/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 evalidate-2.0.3/evalidate/credits.txt
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 evalidate-2.0.3/evalidate/security.py
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 evalidate-2.0.3/examples/basic.py
+-rwxr-xr-x   0        0        0      673 2020-02-02 00:00:00.000000 evalidate-2.0.3/examples/products.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 evalidate-2.0.3/tests/test_exc.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 evalidate-2.0.3/tests/test_expr.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 evalidate-2.0.3/tests/test_feature.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 evalidate-2.0.3/tests/test_jailbreak.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 evalidate-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 evalidate-2.0.3/LICENSE
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 evalidate-2.0.3/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 evalidate-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 evalidate-2.0.3/PKG-INFO
```

### Comparing `evalidate-2.0.2/PKG-INFO` & `evalidate-2.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,292 +1,289 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: evalidate
-Version: 2.0.2
+Version: 2.0.3
 Summary: Validation and secure evaluation of untrusted python expressions
-Home-page: http://github.com/yaroslaff/evalidate
-Author: Yaroslav Polyakov
-Author-email: xenon@sysattack.com
-License: MIT
-Description: ﻿# Evalidate
-        Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
-        
-        ## Upgrade warning
-        Version 2.0 is backward incompatible with older versions. `safeeval()` and `evalidate()` methods are removed, and EvalMode class is introduced.
-        
-        See [upgrade example in ticket](https://github.com/yaroslaff/evalidate/issues/5) or use older (any before 2.0.0, e.g. [v1.1.0](https://pypi.org/project/evalidate/1.1.0/)) if you have old code and do not want to upgrade. But upgrading is easy, so please consider this option.
-        
-        ## Purpose
-        Originally it's developed for filtering complex data structures e.g. 
-        
-        Find cheap smartphones available for sale:
-        ```python
-        category="smartphones" and price<300 and stock>0
-        ```
-        
-        But also, it can be used for other expressions, e.g. arithmetical, like
-        ```python
-        a+b-100
-        ```
-        
-        Evalidate is fastest among all (known to me) secure eval pythong modules.
-        
-        ## Install
-        
-        ```shell
-        pip3 install evalidate
-        ```
-            
-        ## Security
-        
-        Built-in python features such as compile() or eval() are quite powerful to run any kind of user-supplied code, but could be insecure if used code is malicious like `os.system("rm -rf /")`. Evalidate works on whitelist principle, allowing code only if it consist only of safe operations (based on authors views about what is safe and what is not, your mileage may vary - but you can supply your list of safe operations)
-        
-        
-        ## TL;DR. Just give me safe eval!
-        ```python       
-        from evalidate import Expr, EvalException
-        
-        src = 'a + 40 > b'
-        # src = "__import__('os').system('clear')"
-        
-        try:
-            print(Expr(src).eval({'a':10, 'b':42}))
-        except EvalException as e:
-            print(e)
-        ```
-        
-        Gives output: `True`
-        
-        In case of dangerous code (uncomment second src line to test):
-          
-        output will be: `ERR: Operation type Call is not allowed`
-        
-        
-        ## Exceptions
-        Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
-        inherit from base exception class `EvalException`.
-        
-        ## Configure validation
-        Evalidate is very flexible, depending on security model, same code can either pass validation or raise exception.
-        
-        EvalModel is security model class for eval - lists of allowed AST nodes, function calls, attributes and dict of imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
-        
-        You can create custom empty model (and extend it later):
-        ~~~python
-        my_model = evalidate.EvalModel()
-        ~~~
-        
-        (nothing is allowed by default, even `1+2` will not be considered safe)
-        
-        or you may start from `base_eval_mode` and extend it:
-        ~~~python
-        from evalidate import Expr, base_eval_model
-        
-        my_model = base_eval_model.clone()
-        my_model.nodes.append('Mult')
-        
-        Expr('2*2', model=my_model).eval()
-        ~~~
-        
-        To enable `int()` function, need to allow `'Call'` node and add this function to list of allowed function:
-        
-        ~~~python
-        my_model.nodes.append('Call')
-        my_model.allowed_functions.append('int')
-        
-        Expr('int(36.6)', model=my_model).eval()
-        ~~~
-        
-        Or, to call attributes:
-        ~~~python
-        m = base_eval_model.clone()
-        m.nodes.extend(['Call', 'Attribute'])
-        m.attributes.append('startswith')
-        
-        src = '"abcdef".startswith("abc")'
-        r = evalidate.Expr(src, model=m).eval()
-        ~~~
-        
-        But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
-        
-        
-        ### Exporting my functions to eval code
-        ~~~python
-        def one():
-          return 1
-        
-        m = base_eval_model.clone()
-        m.nodes.append('Call')
-        Expr('one()', model=m).eval()
-        ~~~
-        
-        ## Improve speed by using native eval() with validated code
-        Evalidate is very fast, but it's still takes CPU cycles... If you want to achieve maximal possible speed, you can use python native [eval](https://docs.python.org/3/library/functions.html#eval) with this kind of code:
-        
-        ~~~python
-        from evalidate import Expr
-        
-        d = dict(a=1, b=2)
-        expr = Expr('a+b')
-        eval(expr.code, None, d) # <-- native python eval, will run at eval() speed
-        ~~~
-        
-        This is as secure as expr.eval(), because `expr.code` is already validated to be secure.
-        
-        Difference is very little: execution of `expr.code` can throw any exception, while `expr.eval()` can throw only ExecutionException. Also, if you want to export your functions to eval, you should do this manually. 
-        
-        ## Limitations
-        
-        evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) to get [AST node](https://docs.python.org/3/library/ast.html#node-classes) to validate it.
-        
-        >Warning
-        >
-        >It is possible to crash the Python interpreter with a sufficiently large/complex string due to stack depth limitations in Python’s AST compiler. 
-        
-        In my test, works well with 200 nested int(): `int(int(.... int(1)...))` but not with 201. Source code is 1000+ characters. But even if evalidate will get such code, it will just raise `CompilationException`.
-        
-        
-        ### evalidate.security.test_security()
-        Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (nodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
-        
-        This code will never print (I hope).
-        ~~~python
-        from evalidate.security import test_security
-        
-        test_security() or print("default rules are vulnerable!")
-        ~~~
-        
-        But this will fail because nodes/funcs leads to successful validation for attack (suppose you do not want anyone to call `int()`)
-        ~~~python
-        from evalidate.security import test_security
-        
-        attacks = ['int(1)']
-        
-        test_security(attacks, addnodes=['Call'], funcs=['int'], verbose=True)
-        ~~~
-        
-        It will print:
-        ~~~
-        Testing attack code:
-        int(1)
-        Problem! Attack passed validation without exception!
-        Code:
-        int(1)
-        ~~~
-        
-        
-        
-        
-        ## Example
-        
-        ### Filtering by user-supplied condition ###
-        
-        This is code of `examples/products.py`. Expression is validated and compiled once and executed (as byte-code, very fast) many times, so filtering is both fast and secure.
-        
-        
-        ~~~python
-        #!/usr/bin/env python3
-        
-        import requests
-        from evalidate import Expr, ValidationException, CompilationException, ExecutionException
-        import json
-        import sys
-        
-        data = requests.get('https://dummyjson.com/products?limit=100').json()
-        
-        try:
-            src = sys.argv[1]
-        except IndexError:
-            src = 'True'
-        
-        try:
-            expr = Expr(src)
-        except (ValidationException, CompilationException) as e:
-            print(e)
-            sys.exit(1)
-        
-        c=0
-        for p in data['products']:
-            # print(p)
-            try:
-                r = expr.eval(p)
-                if r:
-                    print(json.dumps(p, indent=2))
-                    c+=1
-            except ExecutionException as e:
-                print("Runtime exception:", e)
-        print("# {} products matches".format(c))
-        ~~~
-        
-        ~~~shell
-        # print all 100 products
-        ./products.py
-        
-        # Only cheap products, 8 matches
-        ./products.py 'price<20'
-        
-        # smartphones (5)
-        ./products.py 'category=="smartphones"'
-        
-        # good smartphones
-        ./products.py 'category=="smartphones" and rating>4.5'
-        
-        # cheap smartphones
-        ./products.py 'category=="smartphones" and price<300'
-        ~~~
-                                               
-        
-        ## Similar projects and benchmark
-        
-        [asteval](https://newville.github.io/asteval/)
-        
-        While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
-        - asteval is much slower (evalidate can be used at speed of eval() python bytecode)
-        - user can provide source code which runs very long time and consumes many resources 
-        
-        
-        [simpleeval](https://github.com/danthedeckie/simpleeval)
-        Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is few times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
-        
-        evalidate is good to run same expression against different data.
-        
-        ## Benchmarking
-        We use `benchmark/benchmark.py` in this repository.
-        We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
-        
-        ~~~
-        Products: 1000000 items
-        evalidate_raw_eval(): 0.266s
-        evalidate_eval(): 0.326s
-        test_simpleeval(): 1.824s
-        test_asteval(): 26.106s
-        ~~~
-        
-        As you see, evalidate is few times faster then simpleeval and both are much faster then asteval.
-        
-        Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. (Benchmark code must assume expression as unknown in advance and untrusted)
-        
-        
-        ## Read about eval() risks
-        
-        - https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
-        - https://netsec.expert/posts/breaking-python3-eval-protections/
-        - https://realpython.com/python-eval-function/
-        
-        Note: realpython article shows example with nice short method of validation source (using `code.co_names`), 
-        but it's vulnerable, it passes "bomb" from Ned Batchelder article (bomb has empty `co_names` tuple) and crash interpreter. Evalidate can block this code and similar bombs (unless you will intentionally configure evalidate to pass specific bomb code. Yes, with evalidate it is hard to shoot yourself in the foot, but it is possible if you will try hard).
-        
-        ## More info
-        
-        Want more info? Check source code of module, it's very short and simple, easy to modify
-        
-        ## Contact
-        
-        Write me: yaroslaff at gmail.com
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/yaroslaff/evalidate
+Project-URL: Issues, https://github.com/yaroslaff/evalidate/issues
+Author-email: Yaroslav Polyakov <yaroslaff@gmail.com>
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Classifier: Topic :: Security
-Classifier: Topic :: Software Development :: Interpreters
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+﻿# Evalidate
+Evalidate is simple python module for safe and very fast eval()'uating user-supplied (possible malicious) python expressions.
+
+## Upgrade warning
+Version 2.0 is backward incompatible with older versions. `safeeval()` and `evalidate()` methods are removed, and EvalMode class is introduced.
+
+See [upgrade example in ticket](https://github.com/yaroslaff/evalidate/issues/5) or use older (any before 2.0.0, e.g. [v1.1.0](https://pypi.org/project/evalidate/1.1.0/)) if you have old code and do not want to upgrade. But upgrading is easy, so please consider this option.
+
+## Purpose
+Originally it's developed for filtering complex data structures e.g. 
+
+Find cheap smartphones available for sale:
+```python
+category="smartphones" and price<300 and stock>0
+```
+
+But also, it can be used for other expressions, e.g. arithmetical, like
+```python
+a+b-100
+```
+
+Evalidate is fastest among all (known to me) secure eval pythong modules.
+
+## Install
+
+```shell
+pip3 install evalidate
+```
+    
+## Security
+
+Built-in python features such as compile() or eval() are quite powerful to run any kind of user-supplied code, but could be insecure if used code is malicious like `os.system("rm -rf /")`. Evalidate works on whitelist principle, allowing code only if it consist only of safe operations (based on authors views about what is safe and what is not, your mileage may vary - but you can supply your list of safe operations)
+
+
+## TL;DR. Just give me safe eval!
+```python       
+from evalidate import Expr, EvalException
+
+src = 'a + 40 > b'
+# src = "__import__('os').system('clear')"
+
+try:
+    print(Expr(src).eval({'a':10, 'b':42}))
+except EvalException as e:
+    print(e)
+```
+
+Gives output: `True`
+
+In case of dangerous code (uncomment second src line to test):
+  
+output will be: `ERR: Operation type Call is not allowed`
+
+
+## Exceptions
+Evalidate throws exceptions `CompilationException`, `ValidationException`, `ExecutionException`. All of them
+inherit from base exception class `EvalException`.
+
+## Configure validation
+Evalidate is very flexible, depending on security model, same code can either pass validation or raise exception.
+
+EvalModel is security model class for eval - lists of allowed AST nodes, function calls, attributes and dict of imported functions. There is built-in model `base_eval_model` with basic operations allowed (which are safe from authors point of view).
+
+You can create custom empty model (and extend it later):
+~~~python
+my_model = evalidate.EvalModel()
+~~~
+
+(nothing is allowed by default, even `1+2` will not be considered safe)
+
+or you may start from `base_eval_mode` and extend it:
+~~~python
+from evalidate import Expr, base_eval_model
+
+my_model = base_eval_model.clone()
+my_model.nodes.append('Mult')
+
+Expr('2*2', model=my_model).eval()
+~~~
+
+To enable `int()` function, need to allow `'Call'` node and add this function to list of allowed function:
+
+~~~python
+my_model.nodes.append('Call')
+my_model.allowed_functions.append('int')
+
+Expr('int(36.6)', model=my_model).eval()
+~~~
+
+Or, to call attributes:
+~~~python
+m = base_eval_model.clone()
+m.nodes.extend(['Call', 'Attribute'])
+m.attributes.append('startswith')
+
+src = '"abcdef".startswith("abc")'
+r = evalidate.Expr(src, model=m).eval()
+~~~
+
+But even with this settings, exploiting it with expression like `__builtins__["eval"](1)` will fail (good!).
+
+
+### Exporting my functions to eval code
+~~~python
+def one():
+  return 1
+
+m = base_eval_model.clone()
+m.nodes.append('Call')
+Expr('one()', model=m).eval()
+~~~
+
+## Improve speed by using native eval() with validated code
+Evalidate is very fast, but it's still takes CPU cycles... If you want to achieve maximal possible speed, you can use python native [eval](https://docs.python.org/3/library/functions.html#eval) with this kind of code:
+
+~~~python
+from evalidate import Expr
+
+d = dict(a=1, b=2)
+expr = Expr('a+b')
+eval(expr.code, None, d) # <-- native python eval, will run at eval() speed
+~~~
+
+This is as secure as expr.eval(), because `expr.code` is already validated to be secure.
+
+Difference is very little: execution of `expr.code` can throw any exception, while `expr.eval()` can throw only ExecutionException. Also, if you want to export your functions to eval, you should do this manually. 
+
+## Limitations
+
+evalidate uses [ast.parse()](https://docs.python.org/3/library/ast.html#ast.parse) to get [AST node](https://docs.python.org/3/library/ast.html#node-classes) to validate it.
+
+>Warning
+>
+>It is possible to crash the Python interpreter with a sufficiently large/complex string due to stack depth limitations in Python’s AST compiler. 
+
+In my test, works well with 200 nested int(): `int(int(.... int(1)...))` but not with 201. Source code is 1000+ characters. But even if evalidate will get such code, it will just raise `CompilationException`.
+
+
+### evalidate.security.test_security()
+Evalidate is very flexible and it's possible to shoot yourself in foot if you will try hard. `test_security()` checks your configuration (nodes, funcs, attrs) against given list of possible attack code or against built-in list of attacks. `test_security()` returns True if everything is OK (all attacks raised ValidationException) or False if something passed.
+
+This code will never print (I hope).
+~~~python
+from evalidate.security import test_security
+
+test_security() or print("default rules are vulnerable!")
+~~~
+
+But this will fail because nodes/funcs leads to successful validation for attack (suppose you do not want anyone to call `int()`)
+~~~python
+from evalidate.security import test_security
+
+attacks = ['int(1)']
+
+test_security(attacks, addnodes=['Call'], funcs=['int'], verbose=True)
+~~~
+
+It will print:
+~~~
+Testing attack code:
+int(1)
+Problem! Attack passed validation without exception!
+Code:
+int(1)
+~~~
+
+
+
+
+## Example
+
+### Filtering by user-supplied condition ###
+
+This is code of `examples/products.py`. Expression is validated and compiled once and executed (as byte-code, very fast) many times, so filtering is both fast and secure.
+
+
+~~~python
+#!/usr/bin/env python3
+
+import requests
+from evalidate import Expr, ValidationException, CompilationException, ExecutionException
+import json
+import sys
+
+data = requests.get('https://dummyjson.com/products?limit=100').json()
+
+try:
+    src = sys.argv[1]
+except IndexError:
+    src = 'True'
+
+try:
+    expr = Expr(src)
+except (ValidationException, CompilationException) as e:
+    print(e)
+    sys.exit(1)
+
+c=0
+for p in data['products']:
+    # print(p)
+    try:
+        r = expr.eval(p)
+        if r:
+            print(json.dumps(p, indent=2))
+            c+=1
+    except ExecutionException as e:
+        print("Runtime exception:", e)
+print("# {} products matches".format(c))
+~~~
+
+~~~shell
+# print all 100 products
+./products.py
+
+# Only cheap products, 8 matches
+./products.py 'price<20'
+
+# smartphones (5)
+./products.py 'category=="smartphones"'
+
+# good smartphones
+./products.py 'category=="smartphones" and rating>4.5'
+
+# cheap smartphones
+./products.py 'category=="smartphones" and price<300'
+~~~
+                                       
+
+## Similar projects and benchmark
+
+[asteval](https://newville.github.io/asteval/)
+
+While asteval can compute much more complex code (define functions, use python math libraries) it has drawbacks:
+- asteval is much slower (evalidate can be used at speed of eval() python bytecode)
+- user can provide source code which runs very long time and consumes many resources 
+
+
+[simpleeval](https://github.com/danthedeckie/simpleeval)
+Very similar project, using AST approach too and optimized to re-evaluate pre-parsed expressions. But parsed expressions are stored as more high-level [ast.Expr](https://docs.python.org/3/library/ast.html#ast.Expr) type and this approach is few times slower, while evalidate uses python native `code` type and evaluation itself goes at speed of python eval()
+
+evalidate is good to run same expression against different data.
+
+## Benchmarking
+We use `benchmark/benchmark.py` in this repository.
+We prepare list of 1 million of products (actually, we take just 100 products sample, but repeat it 10 000 times to get 1 million), and then filter it, finding only specific products on "untrusted user-supplied expression" (`price < 20` in this case)
+
+~~~
+Products: 1000000 items
+evalidate_raw_eval(): 0.266s
+evalidate_eval(): 0.326s
+test_simpleeval(): 1.824s
+test_asteval(): 26.106s
+~~~
+
+As you see, evalidate is few times faster then simpleeval and both are much faster then asteval.
+
+Maybe my test is not perfectly optimized (I'm not expert with simpleeval/asteval), if you can suggest better filtering sample code (which produces faster result), I will include it. (Benchmark code must assume expression as unknown in advance and untrusted)
+
+
+## Read about eval() risks
+
+- https://nedbatchelder.com/blog/201206/eval_really_is_dangerous.html
+- https://netsec.expert/posts/breaking-python3-eval-protections/
+- https://realpython.com/python-eval-function/
+
+Note: realpython article shows example with nice short method of validation source (using `code.co_names`), 
+but it's vulnerable, it passes "bomb" from Ned Batchelder article (bomb has empty `co_names` tuple) and crash interpreter. Evalidate can block this code and similar bombs (unless you will intentionally configure evalidate to pass specific bomb code. Yes, with evalidate it is hard to shoot yourself in the foot, but it is possible if you will try hard).
+
+## More info
+
+Want more info? Check source code of module, it's very short and simple, easy to modify
+
+## Contact
+
+Write me: yaroslaff at gmail.com
```

### Comparing `evalidate-2.0.2/README.md` & `evalidate-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `evalidate-2.0.2/evalidate/__init__.py` & `evalidate-2.0.3/evalidate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Safe user-supplied python expression evaluation."""
 
 import ast
 import dataclasses
 from typing import Callable
 
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 
 
 class EvalException(Exception):
     pass
 
 
 class ValidationException(EvalException):
@@ -30,15 +30,15 @@
         super().__init__(exc)
         self.exc = exc
 
 
 @dataclasses.dataclass
 class EvalModel:
     """ eval security model """
-    nodes: list
+    nodes: list = dataclasses.field(default_factory=list)
     allowed_functions: list = dataclasses.field(default_factory=list)
     imported_functions: dict = dataclasses.field(default_factory=dict)
     attributes: list = dataclasses.field(default_factory=list)
 
     def clone(self):
         return EvalModel(**dataclasses.asdict(self))
 
@@ -105,14 +105,15 @@
 )
 
 mult_eval_model = base_eval_model.clone()
 mult_eval_model.nodes.append('Mul')
 
 class Expr():
     def __init__(self, expr, model=None, filename=None):
+
         self.expr = expr
         self.model = model or base_eval_model
 
         try:
             self.node = ast.parse(self.expr, '<usercode>', 'eval')
         except SyntaxError as e:
             raise CompilationException(e)
```

### Comparing `evalidate-2.0.2/evalidate/security.py` & `evalidate-2.0.3/evalidate/security.py`

 * *Files identical despite different names*

### Comparing `evalidate-2.0.2/setup.py` & `evalidate-2.0.3/setup.py`

 * *Files identical despite different names*

