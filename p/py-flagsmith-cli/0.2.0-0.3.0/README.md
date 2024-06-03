# Comparing `tmp/py_flagsmith_cli-0.2.0.tar.gz` & `tmp/py_flagsmith_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_flagsmith_cli-0.2.0.tar", last modified: Sun Jun  2 14:22:31 2024, max compression
+gzip compressed data, was "py_flagsmith_cli-0.3.0.tar", last modified: Sun Jun  2 15:19:32 2024, max compression
```

## Comparing `py_flagsmith_cli-0.2.0.tar` & `py_flagsmith_cli-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      213 2024-06-02 14:20:29.346214 py_flagsmith_cli-0.2.0/README.md
--rw-r--r--   0        0        0       53 2024-06-02 14:22:06.045023 py_flagsmith_cli-0.2.0/py_flagsmith_cli/__init__.py
--rw-r--r--   0        0        0       59 2024-06-01 11:42:10.260550 py_flagsmith_cli-0.2.0/py_flagsmith_cli/__main__.py
--rw-r--r--   0        0        0      355 2024-06-02 12:54:28.594925 py_flagsmith_cli-0.2.0/py_flagsmith_cli/cli.py
--rw-r--r--   0        0        0     6142 2024-06-02 13:18:10.560202 py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/get.py
--rw-r--r--   0        0        0     1313 2024-06-02 13:44:01.399153 py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/showenv.py
--rw-r--r--   0        0        0      159 2024-06-02 12:42:46.510348 py_flagsmith_cli-0.2.0/py_flagsmith_cli/constant.py
--rw-r--r--   0        0        0      883 2024-06-02 13:18:14.121680 py_flagsmith_cli-0.2.0/py_flagsmith_cli/utils.py
--rw-r--r--   0        0        0     1323 2024-06-02 14:22:31.029557 py_flagsmith_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1891 2024-06-01 11:43:03.803849 py_flagsmith_cli-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 13:32:57.627945 py_flagsmith_cli-0.2.0/tests/clis/__init__.py
--rw-r--r--   0        0        0     7660 2024-06-02 13:26:03.552719 py_flagsmith_cli-0.2.0/tests/clis/test_get.py
--rw-r--r--   0        0        0     1740 2024-06-02 13:47:26.108567 py_flagsmith_cli-0.2.0/tests/clis/test_showenv.py
--rw-r--r--   0        0        0       42 2024-06-01 13:29:14.438520 py_flagsmith_cli-0.2.0/tests/mockdata/__init__.py
--rw-r--r--   0        0        0     1011 2024-06-01 13:28:13.395307 py_flagsmith_cli-0.2.0/tests/mockdata/clis/get.py
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 py_flagsmith_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-06-02 15:19:20.948972 py_flagsmith_cli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7124 2024-06-02 15:19:20.966188 py_flagsmith_cli-0.3.0/README.md
+-rw-r--r--   0        0        0       52 2024-06-02 15:19:20.978373 py_flagsmith_cli-0.3.0/py_flagsmith_cli/__init__.py
+-rw-r--r--   0        0        0       59 2024-06-01 11:42:10.260550 py_flagsmith_cli-0.3.0/py_flagsmith_cli/__main__.py
+-rw-r--r--   0        0        0      351 2024-06-02 15:19:20.967888 py_flagsmith_cli-0.3.0/py_flagsmith_cli/cli.py
+-rw-r--r--   0        0        0     6455 2024-06-02 15:19:20.968531 py_flagsmith_cli-0.3.0/py_flagsmith_cli/clis/get.py
+-rw-r--r--   0        0        0     1389 2024-06-02 15:19:20.969054 py_flagsmith_cli-0.3.0/py_flagsmith_cli/clis/showenv.py
+-rw-r--r--   0        0        0      159 2024-06-02 12:42:46.510348 py_flagsmith_cli-0.3.0/py_flagsmith_cli/constant.py
+-rw-r--r--   0        0        0      883 2024-06-02 13:18:14.121680 py_flagsmith_cli-0.3.0/py_flagsmith_cli/utils.py
+-rw-r--r--   0        0        0     1337 2024-06-02 15:19:32.911102 py_flagsmith_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1891 2024-06-01 11:43:03.803849 py_flagsmith_cli-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 13:32:57.627945 py_flagsmith_cli-0.3.0/tests/clis/__init__.py
+-rw-r--r--   0        0        0     7681 2024-06-02 15:19:20.969985 py_flagsmith_cli-0.3.0/tests/clis/test_get.py
+-rw-r--r--   0        0        0     1740 2024-06-02 15:19:20.970511 py_flagsmith_cli-0.3.0/tests/clis/test_showenv.py
+-rw-r--r--   0        0        0       42 2024-06-01 13:29:14.438520 py_flagsmith_cli-0.3.0/tests/mockdata/__init__.py
+-rw-r--r--   0        0        0     1011 2024-06-01 13:28:13.395307 py_flagsmith_cli-0.3.0/tests/mockdata/clis/get.py
+-rw-r--r--   0        0        0     7752 1970-01-01 00:00:00.000000 py_flagsmith_cli-0.3.0/PKG-INFO
```

### Comparing `py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/get.py` & `py_flagsmith_cli-0.3.0/py_flagsmith_cli/clis/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 from enum import Enum
 from typing import Any, Dict, List
 
-from click import FileError
 import requests
 import typer
+from click import FileError
 
 from py_flagsmith_cli.constant import FLAGSMITH_ENVIRONMENT, FLAGSMITH_HOST
 from py_flagsmith_cli.utils import exit_error
 
 SMITH_HOST = os.getenv(FLAGSMITH_HOST, "https://edge.api.flagsmith.com")
 SMITH_API_ENDPOINT = f"{SMITH_HOST}/api/v1/"
 DEFAULT_OUTPUT = "./flagsmith.json"
@@ -123,30 +123,46 @@
         "--api",
         "-a",
         help="The API URL to fetch the feature flags from", metavar="<text>"
     ),
     identity: str = typer.Option(
         None, "--identity", "-i", help="The identity for which to fetch feature flags", metavar="<text>"
     ),
-    pretty: bool = typer.Option(
-        True, "--no-pretty", "-np", help="Prettify the output JSON", is_flag=True, metavar="<flag>"
+    no_pretty: bool = typer.Option(
+        False, "--no-pretty", "-np", help="Do not prettify the output JSON", is_flag=True, metavar="<flag>"
     ),
     entity: str = typer.Option(
         EntityEnum.flags,
         "--entity",
         "-e",
         help="""The entity to fetch, this will either be the flags or an environment document used for Local Evaluation Mode.
         Refer to https://docs.flagsmith.com/clients/server-side.""",
         metavar="<text>",
         show_choices=True,
         case_sensitive=False,
     ),
 ):
     """
     Retrieve flagsmith features from the Flagsmith API and output them to file.
+
+    \b
+    EXAMPLES
+    $ pysmith get <ENVIRONMENT_API_KEY>
+
+    $ FLAGSMITH_ENVIRONMENT=x pysmith get
+
+    $ pysmith get -e environment
+
+    $ pysmith get -o ./my-file.json
+
+    $ pysmith get -a https://flagsmith.example.com/api/v1/
+
+    $ pysmith get -i flagsmith_identity
+
+    $ pysmith get -np
     """
     if not environment:
         exit_error(
             "A flagsmith environment was not specified, run pysmith get --help for more usage."
         )
 
     is_document = entity == "environment"
@@ -162,18 +178,18 @@
     api_url = api or SMITH_API_ENDPOINT
 
     if is_document:
         data = get_by_environment(api_url, environment)
     else:
         data = get_by_identity(api_url, environment, identity)
 
-    if pretty:
-        output_data = json.dumps(data, indent=2)
-    else:
+    if no_pretty:
         output_data = json.dumps(data)
+    else:
+        output_data = json.dumps(data, indent=2)
     if output:
         try:
             with open(output, "w") as f:
                 f.write(output_data)
         except Exception:
             raise FileError(output)
         typer.echo(f"Output saved to {typer.style(output, fg=typer.colors.GREEN)}")
```

### Comparing `py_flagsmith_cli-0.2.0/py_flagsmith_cli/clis/showenv.py` & `py_flagsmith_cli-0.3.0/py_flagsmith_cli/clis/showenv.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 
 from py_flagsmith_cli.constant import FLAGSMITH_ENVIRONMENT, FLAGSMITH_HOST
 
 
 def entry():
     """
     Show the current flagsmith environment setup. Including environment id and api host.
+    
+    \b
+    EXAMPLES:
+
+    $ pysmith showenv
+    Current flagsmith env setup>>>
+    flagsmith environment ID: <environment-id>
+    flagsmith host: <api-host>
     """
     smith_env: Union[str, None] = os.getenv(FLAGSMITH_ENVIRONMENT)
-    print("??????????????????", smith_env)
     if not smith_env:
         typer.echo("No environment set yet.")
         typer.echo(
             f"""You have two ways to set the environment: 
 1. Set the environment variable {typer.style(FLAGSMITH_ENVIRONMENT, fg=typer.colors.GREEN)} to your environment key.
     eg: `export {FLAGSMITH_ENVIRONMENT}=<your-flagsmith-environment>` in the CLI \
 or in your {typer.style('~/.bashrc', fg=typer.colors.GREEN)} or {typer.style('~/.zshrc', fg=typer.colors.GREEN)}
 2. Set variable {typer.style(FLAGSMITH_ENVIRONMENT, fg=typer.colors.GREEN)} \
 in {typer.style('.env', fg=typer.colors.GREEN)} current directory."""
         )
         raise typer.Exit()
     smith_host: Union[str, None] = os.getenv(FLAGSMITH_HOST)
-    print('?????????????????', smith_host)
     typer.echo(
         f"""Current flagsmith env setup>>>
 flagsmith environment ID: {typer.style(smith_env, fg=typer.colors.GREEN)}
 flagsmith host: {typer.style(smith_host, fg=typer.colors.GREEN)}
 """
     )
```

### Comparing `py_flagsmith_cli-0.2.0/py_flagsmith_cli/utils.py` & `py_flagsmith_cli-0.3.0/py_flagsmith_cli/utils.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.2.0/pyproject.toml` & `py_flagsmith_cli-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
+version = "0.3.0"
 name = "py-flagsmith-cli"
-dynamic = []
 description = "flagsmith-cli Python Implementation."
 authors = [
     { name = "belingud", email = "im.victor@qq.com" },
 ]
 dependencies = [
     "typer>=0.12.3",
     "requests>=2.32.3",
@@ -16,15 +16,14 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 pysmith = "py_flagsmith_cli.cli:app"
 
@@ -62,8 +61,9 @@
 
 [tool.pdm.dev-dependencies]
 dev = [
     "tox-pdm>=0.7.2",
     "pytest>=8.2.1",
     "isort>=5.13.2",
     "mock>=5.1.0",
+    "bump2version>=1.0.1",
 ]
```

### Comparing `py_flagsmith_cli-0.2.0/tests/__init__.py` & `py_flagsmith_cli-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `py_flagsmith_cli-0.2.0/tests/clis/test_get.py` & `py_flagsmith_cli-0.3.0/tests/clis/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-import pytest
 from unittest import TestCase, mock
-from unittest.mock import MagicMock, patch, Mock, mock_open
+from unittest.mock import MagicMock, Mock, mock_open, patch
+
+import pytest
 import typer
+from click.exceptions import Exit
 from typer.testing import CliRunner
 
 from py_flagsmith_cli.cli import app
-from py_flagsmith_cli.clis.get import (
-    get_by_environment,
-    get_by_identity,
-    SMITH_API_ENDPOINT,
-    NO_ENVIRONMENT_MSG,
-)
+from py_flagsmith_cli.clis.get import (NO_ENVIRONMENT_MSG, SMITH_API_ENDPOINT,
+                                       get_by_environment, get_by_identity)
 
-from click.exceptions import Exit
 from ..mockdata import mock_get_by_identity
 
 
 class TestGetByIdentity(TestCase):
     @patch("py_flagsmith_cli.clis.get.requests.get")
     def test_get_by_identity_success(self, mock_get):
         # 模拟API返回数据
```

### Comparing `py_flagsmith_cli-0.2.0/tests/clis/test_showenv.py` & `py_flagsmith_cli-0.3.0/tests/clis/test_showenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import unittest
-from unittest.mock import patch, MagicMock
+from unittest.mock import MagicMock, patch
+
 import typer
 from typer.testing import CliRunner
 
 from py_flagsmith_cli.cli import app
 from py_flagsmith_cli.constant import FLAGSMITH_ENVIRONMENT
 
-
 runner = CliRunner()
 app = app
 
 
 @patch("os.getenv")
 @patch("typer.echo")
 @patch("typer.Exit")
```

### Comparing `py_flagsmith_cli-0.2.0/tests/mockdata/clis/get.py` & `py_flagsmith_cli-0.3.0/tests/mockdata/clis/get.py`

 * *Files identical despite different names*

