# Comparing `tmp/web3research-0.0.1.tar.gz` & `tmp/web3research-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "web3research-0.0.2.tar", max compression
```

## Comparing `web3research-0.0.1.tar` & `web3research-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 web3research-0.0.1/Makefile
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 web3research-0.0.1/tests/test_ethereum.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/__init__.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/web3research.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/db/__init__.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/db/provider.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/eth/__init__.py
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/eth/base.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/eth/defi.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/eth/market.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/eth/resolve.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/eth/token.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/eth/wallet.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/evm/__init__.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/evm/decoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 web3research-0.0.1/web3research/tron/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 web3research-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 web3research-0.0.1/LICENSE
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 web3research-0.0.1/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 web3research-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 web3research-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-24 09:49:55.886128 web3research-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1350 2024-05-27 14:08:39.433799 web3research-0.0.2/README.md
+-rw-r--r--   0        0        0      924 2024-06-03 11:03:44.305954 web3research-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-24 09:49:55.886128 web3research-0.0.2/web3research/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-24 09:49:55.886128 web3research-0.0.2/web3research/db/__init__.py
+-rw-r--r--   0        0        0     3627 2024-06-03 10:17:12.366801 web3research-0.0.2/web3research/db/provider.py
+-rw-r--r--   0        0        0       35 2024-05-24 09:49:55.886128 web3research-0.0.2/web3research/eth/__init__.py
+-rw-r--r--   0        0        0     6797 2024-06-02 13:40:44.633418 web3research-0.0.2/web3research/eth/base.py
+-rw-r--r--   0        0        0      168 2024-05-24 09:49:55.896128 web3research-0.0.2/web3research/eth/defi.py
+-rw-r--r--   0        0        0      140 2024-05-25 08:02:30.906042 web3research-0.0.2/web3research/eth/market.py
+-rw-r--r--   0        0        0      143 2024-05-24 09:49:55.896128 web3research-0.0.2/web3research/eth/resolve.py
+-rw-r--r--   0        0        0      174 2024-05-24 09:49:55.896128 web3research-0.0.2/web3research/eth/token.py
+-rw-r--r--   0        0        0      142 2024-05-24 09:49:55.896128 web3research-0.0.2/web3research/eth/wallet.py
+-rw-r--r--   0        0        0       22 2024-05-24 09:49:55.896128 web3research-0.0.2/web3research/evm/__init__.py
+-rw-r--r--   0        0        0     1684 2024-05-24 09:49:55.896128 web3research-0.0.2/web3research/evm/decoder.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:49:55.896128 web3research-0.0.2/web3research/tron/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:19:41.479375 web3research-0.0.2/web3research/tron/base.py
+-rw-r--r--   0        0        0     1677 2024-06-03 10:07:20.936963 web3research-0.0.2/web3research/web3research.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 web3research-0.0.2/PKG-INFO
```

### Comparing `web3research-0.0.1/web3research/web3research.py` & `web3research-0.0.2/web3research/web3research.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 import base64
 from io import BytesIO
 import json
 import os
+from typing import Any, Dict, Optional
 from web3research.eth import EthereumProvider
 
 
 class Web3Research:
-    def __init__(self, api_token) -> None:
-        self.eth = EthereumProvider(api_token)
+    def __init__(
+        self,
+        api_token: str,
+        backend: Optional[str] = None,
+        database: str = "ethereum",
+        settings: Optional[Dict[str, Any]] = None,
+        generic_args: Optional[Dict[str, Any]] = None,
+        **kwargs
+    ) -> None:
+        self.eth = EthereumProvider(
+            api_token=api_token,
+            backend=backend,
+            database=database,
+            settings=settings,
+            generic_args=generic_args,
+            **kwargs,
+        )
 
     def install(self):
         # Set this _before_ importing matplotlib
         os.environ["MPLBACKEND"] = "AGG"
 
     def plotly(self, plot):
         # Encode to a base64 str
@@ -29,18 +45,14 @@
         # Write to stdout
         print(img)
         plt.clf()
 
     def table(self, table_element_list):
         print("data:w3r/table;json," + json.dumps(table_element_list))
 
-    def install(self):
-        # Set this _before_ importing matplotlib
-        os.environ["MPLBACKEND"] = "AGG"
-
     def image(self, plt):
         buf = BytesIO()
         plt.savefig(buf, format="png")
         buf.seek(0)
         # Encode to a base64 str
         img = "data:image/png;base64," + base64.b64encode(buf.read()).decode("utf-8")
         # Write to stdout
```

### Comparing `web3research-0.0.1/web3research/evm/decoder.py` & `web3research-0.0.2/web3research/evm/decoder.py`

 * *Files identical despite different names*

### Comparing `web3research-0.0.1/LICENSE` & `web3research-0.0.2/LICENSE`

 * *Files identical despite different names*

