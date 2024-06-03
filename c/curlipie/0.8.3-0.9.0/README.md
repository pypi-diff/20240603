# Comparing `tmp/curlipie-0.8.3.tar.gz` & `tmp/curlipie-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curlipie-0.8.3.tar", max compression
+gzip compressed data, was "curlipie-0.9.0.tar", max compression
```

## Comparing `curlipie-0.8.3.tar` & `curlipie-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0     4919 2021-06-21 14:10:41.688164 curlipie-0.8.3/README.rst
--rw-r--r--   0        0        0      195 2020-01-31 17:27:15.053324 curlipie-0.8.3/curlipie/__init__.py
--rw-r--r--   0        0        0      670 2021-08-09 04:10:19.998234 curlipie-0.8.3/curlipie/compat.py
--rw-r--r--   0        0        0     7761 2021-08-09 04:10:34.838340 curlipie-0.8.3/curlipie/curly.py
--rw-r--r--   0        0        0     5327 2021-08-12 06:07:48.814384 curlipie-0.8.3/curlipie/pie.py
--rw-r--r--   0        0        0     1306 2021-08-12 06:11:58.170375 curlipie-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     6265 2021-08-12 06:12:57.728433 curlipie-0.8.3/setup.py
--rw-r--r--   0        0        0     6481 2021-08-12 06:12:57.728889 curlipie-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     4975 2024-06-02 04:17:46.994984 curlipie-0.9.0/README.rst
+-rw-r--r--   0        0        0      195 2020-01-31 17:27:15.000000 curlipie-0.9.0/curlipie/__init__.py
+-rw-r--r--   0        0        0     7747 2024-06-03 10:58:53.665057 curlipie-0.9.0/curlipie/curly.py
+-rw-r--r--   0        0        0     5288 2024-06-03 11:03:45.946993 curlipie-0.9.0/curlipie/pie.py
+-rw-r--r--   0        0        0     1956 2024-06-03 11:12:35.534600 curlipie-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6405 1970-01-01 00:00:00.000000 curlipie-0.9.0/PKG-INFO
```

### Comparing `curlipie-0.8.3/README.rst` & `curlipie-0.9.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ========
 CurliPie
 ========
 
-.. image:: https://madewithlove.vercel.app/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d
+.. image:: https://madewithlove.open-api.vn/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d
 .. image:: https://badgen.net/pypi/v/curlipie
    :target: https://pypi.org/project/curlipie
 
 Python library to convert `cURL`_ command to `HTTPie`_.
 
 It will convert
 
@@ -83,45 +83,45 @@
 
 
 Online tool
 -----------
 
 CurliPie is not very usable if it stays in library form, so I made an online tool for you to use it quickly:
 
-https://curlipie.vercel.app
+https://curlipie.open-api.vn
 
 The site also provide HTTP API for you to develop a client for it.
 
 
 Development
 -----------
 
 This repo contains three components:
 
 - Python library ``curlipie``. This is the one `published`_ to PyPI.
 
-- An API server built with `FastAPI`_, playing role of backend for `curlipie.vercel.app`_.
+- An API server built with `FastAPI`_, playing role of backend for `curlipie.open-api.vn`_.
 
-- A minimal frontend app built with `AlpineJS`_ and `TailwindCSS`_.
+- A minimal frontend app built with `AlpineJS`_ and `UnoCSS`_ (with `TailwindCSS`_ style).
 
 - Python dependencies are managed with `Poetry`_.
 
 To try running on localhost:
 
 - Run backend with:
 
   .. code-block:: sh
 
     uvicorn api.main:app
 
-- The front-end are just static files, served by backend also, so you can access it via http://localhost:8000/. But because TailwindCSS is configured to strip unused CSS classes, you may need to rerun this command, inside *frontend-dev* folder, to keep your classes:
+- The front-end are just static files, served by backend also, so you can access it via http://localhost:8000/. The CSS is generated depending on which CSS classes are used. To generate CSS file, install `Bun`_, then run the command:
 
   .. code-block:: sh
 
-    yarn build-tailwind
+    ./tools/generate-css.sh
 
 
 Unit test:
 
     .. code-block:: sh
 
         pytest
@@ -139,13 +139,15 @@
 .. |shlex| replace:: ``shlex``
 .. _shlex: https://docs.python.org/3/library/shlex.html
 .. |argparse| replace:: ``argparse``
 .. _argparse: https://docs.python.org/3/library/argparse.html
 .. _go_tutorial: https://gobyexample.com/command-line-flags
 .. _published: https://pypi.org/project/curlipie/
 .. _fastapi: https://github.com/tiangolo/fastapi
-.. _curlipie.vercel.app: https://curlipie.vercel.app/
+.. _curlipie.open-api.vn: https://curlipie.open-api.vn/
 .. _vuejs: https://vuejs.org/
 .. _alpinejs: https://github.com/alpinejs/alpine
+.. _unocss: https://unocss.dev/
 .. _tailwindcss: https://tailwindcss.com
+.. _bun: https://bun.css
 .. _poetry: https://python-poetry.org/
 .. _author: https://quan.hoabinh.vn
```

### Comparing `curlipie-0.8.3/curlipie/curly.py` & `curlipie-0.9.0/curlipie/curly.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import collections.abc
 from typing import List, Optional, Tuple
 from dataclasses import dataclass, field
 from collections import OrderedDict, deque
 from urllib.parse import parse_qsl
 
 import yarl
+import orjson
 from tap import Tap
 from logbook import Logger
 from kiss_headers import parse_it, get_polymorphic, ContentType, BasicAuthorization
 from kiss_headers import Headers, Header
 from http_constants.headers import HttpHeaders as HH
 
-from .compat import json_load, JSONDecodeError
 
 
 logger = Logger(__name__)
 
 
 @dataclass
 class DataArgParseResult:
@@ -185,16 +185,16 @@
         errors.append('@filename syntax (without field name) is not supported')
         return DataArgParseResult(data, errors)
     if string.startswith('='):
         errors.append('=content syntax (without field name) is not supported')
         return DataArgParseResult(data, errors)
     # Maybe JSON?
     try:
-        jsdata = json_load(string)
-    except JSONDecodeError:
+        jsdata = orjson.loads(string.encode())
+    except orjson.JSONDecodeError:
         # Not JSON
         errors.append('Cannot guess post data format')
         return DataArgParseResult(data, errors)
     if isinstance(jsdata, collections.abc.Mapping):
         data = list(jsdata.items())
         return DataArgParseResult(data, errors)
     errors.append('JSON content does not represent an object')
```

### Comparing `curlipie-0.8.3/curlipie/pie.py` & `curlipie-0.9.0/curlipie/pie.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import re
 import shlex
 import logging
 from shlex import quote
 from collections import deque
 from typing import List
 
+import orjson
 from first import first
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from http_constants.headers import HttpHeaders as HH
-from .compat import json_dump
 from .curly import CURLArgumentParser
 
 
 REGEX_SINGLE_OPT = re.compile(r'-\w$')
 REGEX_SHELL_LINEBREAK = re.compile(r'\\\s+')
 logger = logging.getLogger(__name__)
+EXAMPLE = {'httpie': 'http -fa admin:xxx quan.hoabinh.vn/api/users name=meow', 'errors': []}
 
 
 class ConversionResult(BaseModel):
+    model_config = ConfigDict(json_schema_extra={'example': EXAMPLE})
     httpie: str
     errors: List[str] = []
 
-    class Config:
-        schema_extra = {
-            'example': {
-                'httpie': 'http -fa admin:xxx quan.hoabinh.vn/api/users name=meow',
-                'errors': []
-            }
-        }
-
 
 def join_previous_arg(cmds: List[str], name: str):
     prev_arg = cmds[-1]
     if REGEX_SINGLE_OPT.match(prev_arg):
         cmds[-1] += name
     else:
         cmds.append(f'-{name}')
 
 
 def clean_curl(cmd: str):
-    ''' Remove slash-escaped newlines and normal newlines from curl command.'''
+    """Remove slash-escaped newlines and normal newlines from curl command."""
     stripped = REGEX_SHELL_LINEBREAK.sub(' ', cmd)
     return ' '.join(stripped.splitlines())
 
 
 def curl_to_httpie(cmd: str, long_option: bool = False) -> ConversionResult:
     # The cmd can be multiline string, with escape symbols, shlex doesn't support it, so
     # we should convert it to one-line first.
@@ -140,17 +134,17 @@
         if isinstance(v, bool):
             js_bool = str(v).lower()
             cmds.append(f'{qp}:={js_bool}' if not args.get else f'{qp}=={str(v)}')
             continue
         try:
             qv = quote(v)
             cmds.append(f'{qp}={qv}' if not args.get else f'{qp}=={qv}')
-        except TypeError:     # v is not string, normally after parsed from JSON
+        except TypeError:  # v is not string, normally after parsed from JSON
             if isinstance(v, (list, dict)):
-                v = quote(json_dump(v))
+                v = quote(orjson.dumps(v).decode())
             cmds.append(f'{qp}:={v}' if not args.get else f'{qp}=={quote(str(v))}')
     if args.data_binary:
         fn = first(v for v in args.data_binary if v and v.startswith('@'))
         if fn:
             # Strip @
             fn = fn[1:]
             cmds.append(f'@{quote(fn)}')
```

### Comparing `curlipie-0.8.3/pyproject.toml` & `curlipie-0.9.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "curlipie"
-version = "0.8.3"
+version = "0.9.0"
 description = "Library to convert cURL command line to HTTPie"
 authors = ["Nguyễn Hồng Quân <ng.hong.quan@gmail.com>"]
 maintainers = [
     "Nguyễn Hồng Quân <ng.hong.quan@gmail.com>"
 ]
 license = "MPL-2.0"
 readme = "README.rst"
@@ -15,32 +15,72 @@
     "Environment :: Web Environment",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 keywords = ["api", "http", "curl", "httpie", "cli", "conversion"]
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
-multidict = "^4.7.4"
-yarl = "^1.4.2"
-orjson = { version = "^2.2.0", markers = "python_version >= '3.7'" }
+python = "^3.11"
+multidict = "^6.0.5"
+yarl = "^1.9.4"
+orjson = "^3.10.3"
 first = "^2.0.2"
-python-rapidjson = { version = "^0.9.1", markers = "python_version ~= '3.6'" }
-http-constants = "^0.4.0"
-logbook = "^1.5.3"
-single-version = "^1.5.1"
-kiss-headers = "^2.3.0"
-pydantic = "^1.8.2"
-Jinja2 = "^3.0.1"
-typed-argument-parser = "^1.7.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-devtools = "^0.5.1"
-pytest-flake8 = "^1.0.4"
-fastapi = "^0.65.2"
-uvicorn = "^0.14.0"
-aiofiles = "^0.7.0"
+http-constants = "^0.5.0"
+logbook = "^1.7.0.post0"
+single-version = "^1.6.0"
+kiss-headers = "^2.4.3"
+pydantic = "^2.7.2"
+typed-argument-parser = "^1.10.0"
+pydantic-settings = "^2.2.1"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.1"
+devtools = "^0.12.2"
+fastapi = "^0.111.0"
+aiofiles = "^23.2.1"
+ruff = "^0.4.7"
+uvicorn = "^0.30.1"
+jinja2 = "^3.1.4"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = ["tests", "curlipie"]
+
+[tool.ruff]
+line-length = 120
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+target-version = "py312"
+
+[tool.ruff.lint]
+# Enable Pyflakes `E` and `F` codes by default.
+select = ["E", "F"]
+ignore = []
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+[tool.ruff.format]
+quote-style = "single"
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `curlipie-0.8.3/setup.py` & `curlipie-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,189 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: curlipie
+Version: 0.9.0
+Summary: Library to convert cURL command line to HTTPie
+Home-page: https://github.com/hongquan/CurliPie.git
+License: MPL-2.0
+Keywords: api,http,curl,httpie,cli,conversion
+Author: Nguyễn Hồng Quân
+Author-email: ng.hong.quan@gmail.com
+Maintainer: Nguyễn Hồng Quân
+Maintainer-email: ng.hong.quan@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: first (>=2.0.2,<3.0.0)
+Requires-Dist: http-constants (>=0.5.0,<0.6.0)
+Requires-Dist: kiss-headers (>=2.4.3,<3.0.0)
+Requires-Dist: logbook (>=1.7.0.post0,<2.0.0)
+Requires-Dist: multidict (>=6.0.5,<7.0.0)
+Requires-Dist: orjson (>=3.10.3,<4.0.0)
+Requires-Dist: pydantic (>=2.7.2,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: single-version (>=1.6.0,<2.0.0)
+Requires-Dist: typed-argument-parser (>=1.10.0,<2.0.0)
+Requires-Dist: yarl (>=1.9.4,<2.0.0)
+Project-URL: Repository, https://github.com/hongquan/CurliPie.git
+Description-Content-Type: text/x-rst
 
-packages = \
-['curlipie']
+========
+CurliPie
+========
 
-package_data = \
-{'': ['*']}
+.. image:: https://madewithlove.open-api.vn/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d
+.. image:: https://badgen.net/pypi/v/curlipie
+   :target: https://pypi.org/project/curlipie
 
-install_requires = \
-['Jinja2>=3.0.1,<4.0.0',
- 'first>=2.0.2,<3.0.0',
- 'http-constants>=0.4.0,<0.5.0',
- 'kiss-headers>=2.3.0,<3.0.0',
- 'logbook>=1.5.3,<2.0.0',
- 'multidict>=4.7.4,<5.0.0',
- 'pydantic>=1.8.2,<2.0.0',
- 'single-version>=1.5.1,<2.0.0',
- 'typed-argument-parser>=1.7.0,<2.0.0',
- 'yarl>=1.4.2,<2.0.0']
-
-extras_require = \
-{':python_version >= "3.7"': ['orjson>=2.2.0,<3.0.0'],
- ':python_version ~= "3.6"': ['python-rapidjson>=0.9.1,<0.10.0']}
-
-setup_kwargs = {
-    'name': 'curlipie',
-    'version': '0.8.3',
-    'description': 'Library to convert cURL command line to HTTPie',
-    'long_description': '========\nCurliPie\n========\n\n.. image:: https://madewithlove.vercel.app/vn?heart=true&colorA=%23ffcd00&colorB=%23da251d\n.. image:: https://badgen.net/pypi/v/curlipie\n   :target: https://pypi.org/project/curlipie\n\nPython library to convert `cURL`_ command to `HTTPie`_.\n\nIt will convert\n\n.. code-block:: sh\n\n    curl -d name=admin -d shoesize=12 -d color=green&food=wet http://quan.hoabinh.vn\n\nto\n\n.. code-block:: sh\n\n    http -f http://quan.hoabinh.vn name=admin shoesize=12 color=green food=wet\n\n\nMotivation\n----------\n\nThis library was born when I joined a project with a team of non-Linux, non-Python developers. Because the project didn\'t have proper documentation, the other team often shared API usage example to me in form of cURL command, generated from their daily-used Postman. Those cURL commands are usually ugly, like this:\n\n\n.. code-block:: sh\n\n    curl --location --request POST \'http://app-staging.dev/api\' \\\n    --header \'Content-Type: application/json\' \\\n    --data-raw \'{\n        "userId": "abc-xyz",\n        "planAmount": 50000,\n        "isPromotion": false,\n        "createdAt": "2019-12-13 10:00:00"\n    }\'\n\nI am more comfortable with HTTPie (shorter syntax, has highlighting and is a Python application), so I often converted it to HTTPie:\n\n.. code-block:: sh\n\n    http -F app-staging.dev/api userId=abc-xyz planAmount:=50000 isPromotion:=false createdAt=\'2019-12-13 10:00:00\'\n\nThough Postman can generate HTTPie, it does result in even uglier command:\n\n.. code-block:: sh\n\n    printf \'{\n        "userId": "abc-xyz",\n        "planAmount": 50000,\n        "isPromotion": false,\n        "createdAt": "2019-12-13 10:00:00"\n    }\'| http  --follow --timeout 3600 POST app-staging.dev/api \\\n    Content-Type:\'application/json\'\n\nInitially, I had to do conversion manually and quickly got tired from it. I tried to find a conversion tool but failed. There is an online tool `curl2httpie.online`_, but it failed with above example. So I decide to write my own tool.\n\nI don\'t bother to help fix the online tool above, because it is written in Go. The rich ecosystem of Python, with these built-in libraries, enable me to finish the job fast:\n\n- |shlex|_: Help parse the command line in form of shell language, handle the string escaping, quoting for me.\n- |argparse|_: Help parse cURL options and arguments. Note that, cURL arguments syntax follow GNU style, which is common in Linux (and Python) world but not popular in Go world (see `this tutorial <go_tutorial_>`_), so it feels more natural with Python.\n\n\nUsage\n-----\n\n.. code-block:: python\n\n    >>> from curlipie import curl_to_httpie\n\n    >>> curl = """curl -XPUT elastic.dev/movies/_doc/1 -d \'{"director": "Burton, Tim", "year": 1996, "title": "Mars Attacks!"}\' -H \'Content-Type: application/json\'"""\n\n    >>> curl_to_httpie(curl)\n    ConversionResult(httpie="http PUT elastic.dev/movies/_doc/1 director=\'Burton, Tim\' year:=1996 title=\'Mars Attacks!\'", errors=[])\n\n    >>> result = curl_to_httpie(curl)\n\n    >>> result.httpie\n    "http PUT elastic.dev/movies/_doc/1 director=\'Burton, Tim\' year:=1996 title=\'Mars Attacks!\'"\n\n\nOnline tool\n-----------\n\nCurliPie is not very usable if it stays in library form, so I made an online tool for you to use it quickly:\n\nhttps://curlipie.vercel.app\n\nThe site also provide HTTP API for you to develop a client for it.\n\n\nDevelopment\n-----------\n\nThis repo contains three components:\n\n- Python library ``curlipie``. This is the one `published`_ to PyPI.\n\n- An API server built with `FastAPI`_, playing role of backend for `curlipie.vercel.app`_.\n\n- A minimal frontend app built with `AlpineJS`_ and `TailwindCSS`_.\n\n- Python dependencies are managed with `Poetry`_.\n\nTo try running on localhost:\n\n- Run backend with:\n\n  .. code-block:: sh\n\n    uvicorn api.main:app\n\n- The front-end are just static files, served by backend also, so you can access it via http://localhost:8000/. But because TailwindCSS is configured to strip unused CSS classes, you may need to rerun this command, inside *frontend-dev* folder, to keep your classes:\n\n  .. code-block:: sh\n\n    yarn build-tailwind\n\n\nUnit test:\n\n    .. code-block:: sh\n\n        pytest\n\n\nCredit\n------\n\nBrought to you by `Nguyễn Hồng Quân <author_>`_.\n\n\n.. _cURL: https://curl.haxx.se\n.. _HTTPie: https://httpie.org\n.. _curl2httpie.online: https://curl2httpie.online/\n.. |shlex| replace:: ``shlex``\n.. _shlex: https://docs.python.org/3/library/shlex.html\n.. |argparse| replace:: ``argparse``\n.. _argparse: https://docs.python.org/3/library/argparse.html\n.. _go_tutorial: https://gobyexample.com/command-line-flags\n.. _published: https://pypi.org/project/curlipie/\n.. _fastapi: https://github.com/tiangolo/fastapi\n.. _curlipie.vercel.app: https://curlipie.vercel.app/\n.. _vuejs: https://vuejs.org/\n.. _alpinejs: https://github.com/alpinejs/alpine\n.. _tailwindcss: https://tailwindcss.com\n.. _poetry: https://python-poetry.org/\n.. _author: https://quan.hoabinh.vn\n',
-    'author': 'Nguyễn Hồng Quân',
-    'author_email': 'ng.hong.quan@gmail.com',
-    'maintainer': 'Nguyễn Hồng Quân',
-    'maintainer_email': 'ng.hong.quan@gmail.com',
-    'url': 'https://github.com/hongquan/CurliPie.git',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6.1,<4.0.0',
-}
+Python library to convert `cURL`_ command to `HTTPie`_.
 
+It will convert
+
+.. code-block:: sh
+
+    curl -d name=admin -d shoesize=12 -d color=green&food=wet http://quan.hoabinh.vn
+
+to
+
+.. code-block:: sh
+
+    http -f http://quan.hoabinh.vn name=admin shoesize=12 color=green food=wet
+
+
+Motivation
+----------
+
+This library was born when I joined a project with a team of non-Linux, non-Python developers. Because the project didn't have proper documentation, the other team often shared API usage example to me in form of cURL command, generated from their daily-used Postman. Those cURL commands are usually ugly, like this:
+
+
+.. code-block:: sh
+
+    curl --location --request POST 'http://app-staging.dev/api' \
+    --header 'Content-Type: application/json' \
+    --data-raw '{
+        "userId": "abc-xyz",
+        "planAmount": 50000,
+        "isPromotion": false,
+        "createdAt": "2019-12-13 10:00:00"
+    }'
+
+I am more comfortable with HTTPie (shorter syntax, has highlighting and is a Python application), so I often converted it to HTTPie:
+
+.. code-block:: sh
+
+    http -F app-staging.dev/api userId=abc-xyz planAmount:=50000 isPromotion:=false createdAt='2019-12-13 10:00:00'
+
+Though Postman can generate HTTPie, it does result in even uglier command:
+
+.. code-block:: sh
+
+    printf '{
+        "userId": "abc-xyz",
+        "planAmount": 50000,
+        "isPromotion": false,
+        "createdAt": "2019-12-13 10:00:00"
+    }'| http  --follow --timeout 3600 POST app-staging.dev/api \
+    Content-Type:'application/json'
+
+Initially, I had to do conversion manually and quickly got tired from it. I tried to find a conversion tool but failed. There is an online tool `curl2httpie.online`_, but it failed with above example. So I decide to write my own tool.
+
+I don't bother to help fix the online tool above, because it is written in Go. The rich ecosystem of Python, with these built-in libraries, enable me to finish the job fast:
+
+- |shlex|_: Help parse the command line in form of shell language, handle the string escaping, quoting for me.
+- |argparse|_: Help parse cURL options and arguments. Note that, cURL arguments syntax follow GNU style, which is common in Linux (and Python) world but not popular in Go world (see `this tutorial <go_tutorial_>`_), so it feels more natural with Python.
+
+
+Usage
+-----
+
+.. code-block:: python
+
+    >>> from curlipie import curl_to_httpie
+
+    >>> curl = """curl -XPUT elastic.dev/movies/_doc/1 -d '{"director": "Burton, Tim", "year": 1996, "title": "Mars Attacks!"}' -H 'Content-Type: application/json'"""
+
+    >>> curl_to_httpie(curl)
+    ConversionResult(httpie="http PUT elastic.dev/movies/_doc/1 director='Burton, Tim' year:=1996 title='Mars Attacks!'", errors=[])
+
+    >>> result = curl_to_httpie(curl)
+
+    >>> result.httpie
+    "http PUT elastic.dev/movies/_doc/1 director='Burton, Tim' year:=1996 title='Mars Attacks!'"
+
+
+Online tool
+-----------
+
+CurliPie is not very usable if it stays in library form, so I made an online tool for you to use it quickly:
+
+https://curlipie.open-api.vn
+
+The site also provide HTTP API for you to develop a client for it.
+
+
+Development
+-----------
+
+This repo contains three components:
+
+- Python library ``curlipie``. This is the one `published`_ to PyPI.
+
+- An API server built with `FastAPI`_, playing role of backend for `curlipie.open-api.vn`_.
+
+- A minimal frontend app built with `AlpineJS`_ and `UnoCSS`_ (with `TailwindCSS`_ style).
+
+- Python dependencies are managed with `Poetry`_.
+
+To try running on localhost:
+
+- Run backend with:
+
+  .. code-block:: sh
+
+    uvicorn api.main:app
+
+- The front-end are just static files, served by backend also, so you can access it via http://localhost:8000/. The CSS is generated depending on which CSS classes are used. To generate CSS file, install `Bun`_, then run the command:
+
+  .. code-block:: sh
+
+    ./tools/generate-css.sh
+
+
+Unit test:
+
+    .. code-block:: sh
+
+        pytest
+
+
+Credit
+------
+
+Brought to you by `Nguyễn Hồng Quân <author_>`_.
+
+
+.. _cURL: https://curl.haxx.se
+.. _HTTPie: https://httpie.org
+.. _curl2httpie.online: https://curl2httpie.online/
+.. |shlex| replace:: ``shlex``
+.. _shlex: https://docs.python.org/3/library/shlex.html
+.. |argparse| replace:: ``argparse``
+.. _argparse: https://docs.python.org/3/library/argparse.html
+.. _go_tutorial: https://gobyexample.com/command-line-flags
+.. _published: https://pypi.org/project/curlipie/
+.. _fastapi: https://github.com/tiangolo/fastapi
+.. _curlipie.open-api.vn: https://curlipie.open-api.vn/
+.. _vuejs: https://vuejs.org/
+.. _alpinejs: https://github.com/alpinejs/alpine
+.. _unocss: https://unocss.dev/
+.. _tailwindcss: https://tailwindcss.com
+.. _bun: https://bun.css
+.. _poetry: https://python-poetry.org/
+.. _author: https://quan.hoabinh.vn
 
-setup(**setup_kwargs)
```

