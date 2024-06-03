# Comparing `tmp/aiven_client-4.1.1.tar.gz` & `tmp/aiven_client-4.2.0.tar.gz`

## Comparing `aiven_client-4.1.1.tar` & `aiven_client-4.2.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.flake8
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.git-blame-ignore-revs
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 aiven_client-4.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aiven_client-4.1.1/DEVELOPMENT.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 aiven_client-4.1.1/MANIFEST.in
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiven_client-4.1.1/Makefile
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 aiven_client-4.1.1/SECURITY.md
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven-client.spec
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aiven_client-4.1.1/mypy.ini
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/ISSUE_TEMPLATE/01_question.md
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/ISSUE_TEMPLATE/02_bug.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/ISSUE_TEMPLATE/03_feature.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.github/workflows/sync-main-and-master.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/__main__.py
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/argx.py
--rw-r--r--   0        0        0   241298 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/cli.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/cliarg.py
--rw-r--r--   0        0        0   104842 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/client.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/common.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/envdefault.py
--rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/pretty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/py.typed
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/session.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/speller.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/units.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/version.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/connection_info/__init__.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/connection_info/_utils.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/connection_info/common.py
--rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/connection_info/kafka.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/connection_info/pg.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 aiven_client-4.1.1/aiven/client/connection_info/redis.py
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 aiven_client-4.1.1/scripts/avn
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/test_argx.py
--rw-r--r--   0        0        0    57734 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/test_cli.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/test_cliarg.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/test_client.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/test_pretty.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/test_session.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiven_client-4.1.1/tests/test_speller.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aiven_client-4.1.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 aiven_client-4.1.1/LICENSE
--rw-r--r--   0        0        0    15431 2020-02-02 00:00:00.000000 aiven_client-4.1.1/README.rst
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 aiven_client-4.1.1/pyproject.toml
--rw-r--r--   0        0        0    16920 2020-02-02 00:00:00.000000 aiven_client-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.flake8
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 aiven_client-4.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aiven_client-4.2.0/DEVELOPMENT.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 aiven_client-4.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiven_client-4.2.0/Makefile
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 aiven_client-4.2.0/SECURITY.md
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven-client.spec
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aiven_client-4.2.0/mypy.ini
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/ISSUE_TEMPLATE/01_question.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/ISSUE_TEMPLATE/02_bug.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/ISSUE_TEMPLATE/03_feature.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.github/workflows/sync-main-and-master.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/__main__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/_typing.py
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/argx.py
+-rw-r--r--   0        0        0   241298 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/cli.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/cliarg.py
+-rw-r--r--   0        0        0   106196 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/client.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/common.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/envdefault.py
+-rw-r--r--   0        0        0     8106 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/pretty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/py.typed
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/session.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/speller.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/units.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/version.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/connection_info/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/connection_info/_utils.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/connection_info/common.py
+-rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/connection_info/kafka.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/connection_info/pg.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 aiven_client-4.2.0/aiven/client/connection_info/redis.py
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 aiven_client-4.2.0/scripts/avn
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/test_argx.py
+-rw-r--r--   0        0        0    57734 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/test_cliarg.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/test_client.py
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/test_pretty.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/test_session.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiven_client-4.2.0/tests/test_speller.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aiven_client-4.2.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 aiven_client-4.2.0/LICENSE
+-rw-r--r--   0        0        0    15431 2020-02-02 00:00:00.000000 aiven_client-4.2.0/README.rst
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 aiven_client-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16920 2020-02-02 00:00:00.000000 aiven_client-4.2.0/PKG-INFO
```

### Comparing `aiven_client-4.1.1/CODE_OF_CONDUCT.md` & `aiven_client-4.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/Makefile` & `aiven_client-4.2.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-short_ver = 4.1.1
+short_ver = 4.2.0
 release = 1
 PYTHON ?= python3
 PYTHON_DIRS = aiven tests
 
 test: pytest
 lint: ruff flake8 mypy
```

### Comparing `aiven_client-4.1.1/SECURITY.md` & `aiven_client-4.2.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven-client.spec` & `aiven_client-4.2.0/aiven-client.spec`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/mypy.ini` & `aiven_client-4.2.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/.github/CONTRIBUTING.md` & `aiven_client-4.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/.github/workflows/build.yaml` & `aiven_client-4.2.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/.github/workflows/codeql-analysis.yml` & `aiven_client-4.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/.github/workflows/publish-pypi.yaml` & `aiven_client-4.2.0/.github/workflows/publish-pypi.yaml`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/argx.py` & `aiven_client-4.2.0/aiven/client/argx.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/cli.py` & `aiven_client-4.2.0/aiven/client/cli.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/cliarg.py` & `aiven_client-4.2.0/aiven/client/cliarg.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     help="Tag to add or replace into topic metadata",
 )
 arg.untag = arg(
     "--untag", dest="topic_option_untag", metavar="KEY", action="append", help="Tag to delete from topic metadata"
 )
 arg.service_name = arg("service_name", help="Service name")
 arg.service_name_mandatory = arg("service_name", help="Service name", required=True)
-arg.service_type = arg("-t", "--service-type", help="Type of service (see 'service list-types')")
+arg.service_type = arg("-t", "--service-type", help="Type of service (see 'service types')")
 arg.static_ip_id = arg("static_ip_id", help="Static IP address ID")
 arg.ns_name = arg("ns_name", help="Namespace name")
 arg.ns_type = arg("--ns-type", help="Namespace type ('aggregated' or 'unaggregated')", required=True)
 arg.ns_retention_mandatory = arg(
     "--ns-retention", help="Namespace retention period (written like 30m/25h etc)", required=True
 )
 arg.ns_retention = arg("--ns-retention", help="Namespace retention period (written like 30m/25h etc)", required=False)
```

### Comparing `aiven_client-4.1.1/aiven/client/client.py` & `aiven_client-4.2.0/aiven/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 # Copyright 2015, Aiven, https://aiven.io/
 #
 # This file is under the Apache License, Version 2.0.
 # See the file `LICENSE` for details.
 from __future__ import annotations
 
+from ._typing import assert_never
 from .common import UNDEFINED
 from .session import get_requests_session
 from http import HTTPStatus
 from requests import Response
 from requests_toolbelt import MultipartEncoder  # type: ignore
-from typing import Any, BinaryIO, Callable, Collection, Mapping, Sequence, TypedDict
+from typing import (
+    Any,
+    BinaryIO,
+    Callable,
+    Collection,
+    Final,
+    Literal,
+    Mapping,
+    NamedTuple,
+    Sequence,
+    TYPE_CHECKING,
+    TypedDict,
+)
 from urllib.parse import quote
 
+import datetime
 import json
 import logging
 import re
 import requests
 import time
 import warnings
 
 try:
     from .version import __version__
 except ImportError:
     __version__ = "UNKNOWN"
 
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
 UNCHANGED = object()  # used as a sentinel value
 
 
 class Error(Exception):
     """Request error"""
 
     def __init__(self, response: Response, status: int = 520) -> None:
@@ -41,26 +58,56 @@
 
 
 class Tag(TypedDict):
     key: str
     value: str
 
 
+HTTPMethod: TypeAlias = Literal[
+    "CONNECT",
+    "DELETE",
+    "GET",
+    "HEAD",
+    "OPTIONS",
+    "PATCH",
+    "POST",
+    "PUT",
+    "TRACE",
+]
+
+
+class RetrySpec(NamedTuple):
+    attempts: int = 3
+    # Retry GET operations by default
+    http_methods: tuple[HTTPMethod, ...] = ("GET",)
+    sleep: datetime.timedelta = datetime.timedelta(milliseconds=200)
+
+
 class AivenClientBase:
     """Aiven Client with low-level HTTP operations"""
 
-    def __init__(self, base_url: str, show_http: bool = False, request_timeout: int | None = None) -> None:
+    NO_RETRY: Final = RetrySpec(attempts=1)
+    DEFAULT_RETRY: Final = RetrySpec()
+
+    def __init__(
+        self,
+        base_url: str,
+        show_http: bool = False,
+        request_timeout: int | None = None,
+        default_retry_spec: RetrySpec = DEFAULT_RETRY,
+    ) -> None:
         self.log = logging.getLogger("AivenClient")
         self.auth_token: str | None = None
         self.base_url = base_url
         self.log.debug("using %r", self.base_url)
         self.session = get_requests_session(timeout=request_timeout)
         self.http_log = logging.getLogger("aiven_http")
         self.init_http_logging(show_http)
         self.api_prefix = "/v1"
+        self.default_retry_spec: Final = default_retry_spec
 
     def init_http_logging(self, show_http: bool) -> None:
         http_handler = logging.StreamHandler()
         http_handler.setFormatter(logging.Formatter("%(message)s"))
         self.http_log.addHandler(http_handler)
         self.http_log.propagate = False
         self.http_log.setLevel(logging.INFO)
@@ -137,29 +184,42 @@
         """HTTP PUT"""
         return self._execute(self.session.put, "PUT", path, body, params)
 
     def delete(self, path: str = "", body: Any = None, params: Any = None) -> Response:
         """HTTP DELETE"""
         return self._execute(self.session.delete, "DELETE", path, body, params)
 
+    def _get_retry_spec(
+        self,
+        op: Callable[..., Response],
+        argument: int | RetrySpec | None,
+    ) -> RetrySpec:
+        if argument is None:
+            if op.__name__.upper() in self.default_retry_spec.http_methods:
+                return self.default_retry_spec
+            else:
+                return self.NO_RETRY
+        elif isinstance(argument, int):
+            return self.default_retry_spec._replace(attempts=argument)
+        elif isinstance(argument, RetrySpec):
+            return argument
+        else:
+            assert_never(argument)
+
     def verify(
         self,
         op: Callable[..., Response],
         path: str,
         body: Any = None,
         params: Any = None,
         result_key: str | None = None,
-        retry: int | None = None,
+        retry: int | RetrySpec | None = None,
     ) -> Any:
-        # Retry GET operations by default
-        if retry is None and op == self.get:
-            attempts = 3
-        else:
-            attempts = 1 + (retry or 0)
-
+        retry_spec = self._get_retry_spec(op, retry)
+        attempts = retry_spec.attempts
         path = self.api_prefix + path
 
         while attempts:
             attempts -= 1
             try:
                 if body is not None:
                     response = op(path=path, body=body, params=params)
@@ -173,15 +233,15 @@
                     "%s %s failed: %s: %s; retrying in 0.2 seconds, %s attempts left",
                     op.__name__.upper(),
                     path,
                     ex.__class__.__name__,
                     ex,
                     attempts,
                 )
-                time.sleep(0.2)
+                time.sleep(retry_spec.sleep.total_seconds())
 
         return self._process_response(response=response, op=op, path=path, result_key=result_key)
 
     @staticmethod
     def build_path(*parts: str) -> str:
         return "/" + "/".join(quote(part, safe="") for part in parts)
```

### Comparing `aiven_client-4.1.1/aiven/client/envdefault.py` & `aiven_client-4.2.0/aiven/client/envdefault.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/pretty.py` & `aiven_client-4.2.0/aiven/client/pretty.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/session.py` & `aiven_client-4.2.0/aiven/client/session.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/speller.py` & `aiven_client-4.2.0/aiven/client/speller.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/connection_info/_utils.py` & `aiven_client-4.2.0/aiven/client/connection_info/_utils.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/connection_info/common.py` & `aiven_client-4.2.0/aiven/client/connection_info/common.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/connection_info/kafka.py` & `aiven_client-4.2.0/aiven/client/connection_info/kafka.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/connection_info/pg.py` & `aiven_client-4.2.0/aiven/client/connection_info/pg.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/aiven/client/connection_info/redis.py` & `aiven_client-4.2.0/aiven/client/connection_info/redis.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/tests/test_argx.py` & `aiven_client-4.2.0/tests/test_argx.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/tests/test_cli.py` & `aiven_client-4.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/tests/test_cliarg.py` & `aiven_client-4.2.0/tests/test_cliarg.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/tests/test_pretty.py` & `aiven_client-4.2.0/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/tests/test_session.py` & `aiven_client-4.2.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/tests/test_speller.py` & `aiven_client-4.2.0/tests/test_speller.py`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/LICENSE` & `aiven_client-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/README.rst` & `aiven_client-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/pyproject.toml` & `aiven_client-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiven_client-4.1.1/PKG-INFO` & `aiven_client-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aiven-client
-Version: 4.1.1
+Version: 4.2.0
 Summary: Aiven.io client library / command-line client
 Project-URL: Homepage, https://github.com/aiven/aiven-client
 Project-URL: Bug Tracker, https://github.com/aiven/aiven-client/issues
 Project-URL: Documentation, https://docs.aiven.io/docs/tools/cli
 Author-email: Aiven <support@aiven.io>
 License: Apache License 2.0
 License-File: LICENSE
```

