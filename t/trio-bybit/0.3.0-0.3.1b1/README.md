# Comparing `tmp/trio_bybit-0.3.0.tar.gz` & `tmp/trio_bybit-0.3.1b1.tar.gz`

## Comparing `trio_bybit-0.3.0.tar` & `trio_bybit-0.3.1b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/keypair.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/pkcs8.key
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/pytest.ini
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/tests/test_async_client.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/tests/test_rsa.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/trio_bybit/__init__.py
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/trio_bybit/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/trio_bybit/enums.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/trio_bybit/helpers.py
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/README.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 trio_bybit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/keypair.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/pkcs8.key
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/pytest.ini
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/tests/test_async_client.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/tests/test_rsa.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/tests/test_streams.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/README.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/pyproject.toml
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 trio_bybit-0.3.1b1/PKG-INFO
```

### Comparing `trio_bybit-0.3.0/keypair.pem` & `trio_bybit-0.3.1b1/keypair.pem`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/pkcs8.key` & `trio_bybit-0.3.1b1/pkcs8.key`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/test.py` & `trio_bybit-0.3.1b1/test.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/tests/test_async_client.py` & `trio_bybit-0.3.1b1/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/tests/test_rsa.py` & `trio_bybit-0.3.1b1/tests/test_rsa.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/tests/test_streams.py` & `trio_bybit-0.3.1b1/tests/test_streams.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,84 +19,82 @@
         "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
     }
     await socket.subscribe(unsub)
 
 
 async def test_public_stream():
     socket = BybitSocketManager()
-    async with socket.connect():
-        subscription = {
-            "op": "subscribe",
-            "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
-        }
-        await socket.subscribe(subscription)
-
-        with trio.move_on_after(12):
+    with trio.move_on_after(12):
+        async with socket.connect():
+            subscription = {
+                "op": "subscribe",
+                "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
+            }
+            await socket.subscribe(subscription)
             async with trio.open_nursery() as nursery:
                 nursery.start_soon(pub_stream_check, socket)
                 await trio.sleep(10)
                 nursery.start_soon(pub_unsub, socket)
 
 
 async def test_public_linear_stream():
     socket = BybitSocketManager(endpoint="linear")
-    async with socket.connect():
-        subscription = {
-            "op": "subscribe",
-            "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
-        }
-        await socket.subscribe(subscription)
-
-        count = 0
-        async for msg in socket.get_next_message():
-            count += 1
-            if msg.get("topic") == "orderbook.1.BTCUSDT":
-                assert "topic" in msg
-                assert "type" in msg
-                assert "data" in msg
-                assert "s" in msg["data"]
-                assert "a" in msg["data"]
-                assert "b" in msg["data"]
-            elif msg.get("topic") == "publicTrade.BTCUSDT":
-                assert "topic" in msg
-                assert "type" in msg
-                assert "data" in msg
-                assert "S" in msg["data"][0]
-                assert "v" in msg["data"][0]
-                assert "p" in msg["data"][0]
-            if count >= 5000:
-                break
+    with trio.move_on_after(30):
+        async with socket.connect():
+            subscription = {
+                "op": "subscribe",
+                "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
+            }
+            await socket.subscribe(subscription)
+
+            async for msg in socket.get_next_message():
+                if msg.get("topic") == "orderbook.1.BTCUSDT":
+                    assert "topic" in msg
+                    assert "type" in msg
+                    assert "data" in msg
+                    assert "s" in msg["data"]
+                    assert "a" in msg["data"]
+                    assert "b" in msg["data"]
+                elif msg.get("topic") == "publicTrade.BTCUSDT":
+                    assert "topic" in msg
+                    assert "type" in msg
+                    assert "data" in msg
+                    assert "S" in msg["data"][0]
+                    assert "v" in msg["data"][0]
+                    assert "p" in msg["data"][0]
 
 
 async def test_private_stream():
     socket = BybitSocketManager(
         endpoint="private",
         api_key=os.getenv("BYBIT_API_KEY"),
         api_secret=os.getenv("BYBIT_API_SECRET"),
     )
-    async with socket.connect():
-        subscription = {
-            "op": "subscribe",
-            "args": ["order"],
-        }
-        await socket.subscribe(subscription)
+    with trio.move_on_after(100):
+        async with socket.connect():
+            subscription = {
+                "op": "subscribe",
+                "args": ["order"],
+            }
+            await socket.subscribe(subscription)
 
-        async for msg in socket.get_next_message():
-            print(msg)
+            async for msg in socket.get_next_message():
+                print(msg)
 
 
 async def test_private_stream_by_rsa_sig():
     socket = BybitSocketManager(
         endpoint="private",
         api_key=os.getenv("BYBIT_RSA_API_KEY"),
         api_secret=os.getenv("BYBIT_RSA_PRIVATE_KEY_PATH"),
         sign_style="RSA",
     )
-    async with socket.connect():
-        subscription = {
-            "op": "subscribe",
-            "args": ["order"],
-        }
-        await socket.subscribe(subscription)
+    with trio.move_on_after(100):
+        async with socket.connect():
+            subscription = {
+                "op": "subscribe",
+                "args": ["order"],
+            }
+            await socket.subscribe(subscription)
 
-        async for msg in socket.get_next_message():
-            print(msg)
+            async for msg in socket.get_next_message():
+                print(msg)
```

### Comparing `trio_bybit-0.3.0/trio_bybit/client.py` & `trio_bybit-0.3.1b1/trio_bybit/client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/trio_bybit/exceptions.py` & `trio_bybit-0.3.1b1/trio_bybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/trio_bybit/helpers.py` & `trio_bybit-0.3.1b1/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/.gitignore` & `trio_bybit-0.3.1b1/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/LICENSE` & `trio_bybit-0.3.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/README.md` & `trio_bybit-0.3.1b1/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.3.0/pyproject.toml` & `trio_bybit-0.3.1b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trio-bybit"
-version = "0.3.0"
+version = "0.3.1b1"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.1",
     "httpx[http2]>=0.27.0",
```

### Comparing `trio_bybit-0.3.0/PKG-INFO` & `trio_bybit-0.3.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.3.0
+Version: 0.3.1b1
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
```

