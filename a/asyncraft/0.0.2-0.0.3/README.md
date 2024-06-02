# Comparing `tmp/asyncraft-0.0.2.tar.gz` & `tmp/asyncraft-0.0.3.tar.gz`

## Comparing `asyncraft-0.0.2.tar` & `asyncraft-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 asyncraft-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 asyncraft-0.0.2/examples/example_ping.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 asyncraft-0.0.2/examples/example_queue.py
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 asyncraft-0.0.2/src/asyncraft/__init__.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 asyncraft-0.0.2/src/asyncraft/broker.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 asyncraft-0.0.2/src/asyncraft/handler.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 asyncraft-0.0.2/src/asyncraft/message.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 asyncraft-0.0.2/src/asyncraft/pool.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 asyncraft-0.0.2/src/asyncraft/queues.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 asyncraft-0.0.2/tests/test_asyncraft.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 asyncraft-0.0.2/tests/test_pool.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 asyncraft-0.0.2/tests/test_queue.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 asyncraft-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 asyncraft-0.0.2/LICENSE
--rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 asyncraft-0.0.2/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 asyncraft-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 asyncraft-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 asyncraft-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 asyncraft-0.0.3/examples/example_ping.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 asyncraft-0.0.3/examples/example_queue.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 asyncraft-0.0.3/src/asyncraft/__init__.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 asyncraft-0.0.3/src/asyncraft/broker.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 asyncraft-0.0.3/src/asyncraft/handler.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 asyncraft-0.0.3/src/asyncraft/message.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 asyncraft-0.0.3/src/asyncraft/pool.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 asyncraft-0.0.3/src/asyncraft/queues.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 asyncraft-0.0.3/tests/test_asyncraft.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 asyncraft-0.0.3/tests/test_pool.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 asyncraft-0.0.3/tests/test_queue.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 asyncraft-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 asyncraft-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 asyncraft-0.0.3/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 asyncraft-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6780 2020-02-02 00:00:00.000000 asyncraft-0.0.3/PKG-INFO
```

### Comparing `asyncraft-0.0.2/.github/workflows/python-package.yml` & `asyncraft-0.0.3/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with pytest
       run: |
-        pytest
+        pytest -W ignore::RuntimeWarning
   build_package:
       name: Build distribution 📦
       runs-on: ubuntu-latest
       
 
       steps:
       - uses: actions/checkout@v4
```

### Comparing `asyncraft-0.0.2/examples/example_ping.py` & `asyncraft-0.0.3/examples/example_ping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """This example demonstrates how to use the asyncraft library to create a simple ping-pong system."""
 import asyncio
 import time
 import asyncraft
 
 
-@asyncraft.asyncraft_handler("Ping", keys=["Ping"])
+@asyncraft.asyncraft_handler(keys=["Ping"])
 def ping_handler_function(message):
     """This is a sync handler that will respond to the Pong handler. It will be executed in a separate thread."""
     print(f"Received {message.key} with value {message.value}")
     time.sleep(1)
     return asyncraft.Message("Pong", message.value + 1)
 
 
-@asyncraft.asyncraft_handler("Pong", keys=["Pong"])
+@asyncraft.asyncraft_handler(keys=["Pong"])
 async def pong_handler_function(message):
     """This is an async handler that will respond to the Ping handler. It will be executed in the event loop."""
     print(f"Received {message.key} with value {message.value}")
     await asyncio.sleep(1)
     return asyncraft.Message("Ping", message.value + 1)
```

### Comparing `asyncraft-0.0.2/examples/example_queue.py` & `asyncraft-0.0.3/examples/example_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,10 +43,10 @@
         async_producer(),
         asyncio.to_thread(reader, queue),
         asyncio.to_thread(producer)
     )
 
 
 if __name__ == "__main__":
-    queue = MessageQueue("queue1", ["Key", "Key1"])
+    queue = MessageQueue(["Key", "Key1"])
     asyncraft.register_queue(queue)
     asyncraft.start(main())
```

### Comparing `asyncraft-0.0.2/src/asyncraft/broker.py` & `asyncraft-0.0.3/src/asyncraft/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from asyncraft.message import Message, KeyType
 from asyncraft.handler import AsyncHandler, SyncHandler, AbstractHandler
 from asyncraft.pool import AbstractPool, Pool
 
 
 class AbstractBroker:
     loop: asyncio.AbstractEventLoop
+    pool: AbstractPool
 
     def broadcast_message(self, message: Message) -> None:
         """Broadcast a message to all handlers. Is thread safe."""
         raise NotImplementedError
 
     def get_next_free_identifier(self, prefix: Union[str, None] = None) -> str:
         """Get the next free identifier"""
```

### Comparing `asyncraft-0.0.2/src/asyncraft/handler.py` & `asyncraft-0.0.3/src/asyncraft/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from asyncraft.message import Message, KeyType
 
 
 class AbstractHandler:
     handler_type: Literal["Sync", "Async"]
 
-    def __init__(self, identifier: str, keys: List[KeyType], callback: Callable[[Message], Any] = None):
+    def __init__(self, keys: List[KeyType], callback: Callable[[Message], Any] = None,identifier: str = None):
         self.keys = keys
         self.callback = callback
         self.identifier = identifier
 
 
 class SyncHandler(AbstractHandler):
     handler_type = "Sync"
```

### Comparing `asyncraft-0.0.2/src/asyncraft/pool.py` & `asyncraft-0.0.3/src/asyncraft/pool.py`

 * *Files identical despite different names*

### Comparing `asyncraft-0.0.2/src/asyncraft/queues.py` & `asyncraft-0.0.3/src/asyncraft/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     async def async_get(self, blocking=True) -> Union[Message, None]:
         """Get a message from the queue asynchronously."""
         raise NotImplementedError
 
 
 class MessageQueue(AbstractMessageQueue):
-    def __init__(self, identifier: str, keys: List[KeyType], max_items: int = -1,
-                 eviction_policy: Literal["FIFO"] = "FIFO"):
+    def __init__(self, keys: List[KeyType], max_items: int = -1,
+                 eviction_policy: Literal["FIFO"] = "FIFO",identifier: str = None):
         self.identifier = identifier
         self.queue: List[Message] = []
         self.keys = keys
         self.max_items = max_items
         self.eviction_policy = eviction_policy
         self.get_semaphore = threading.Semaphore(0)
         self.access_semaphore = threading.Semaphore(1)
```

### Comparing `asyncraft-0.0.2/tests/test_asyncraft.py` & `asyncraft-0.0.3/tests/test_asyncraft.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncraft
 from asyncraft.message import Message
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_asyncraft():
-    asyncraft.reset()
+    asyncraft.init()
 
     received_sleep_async = False
     received_sleep_sync = False
     call_count = 0
 
     async def call_back_value_async(message):
         await asyncio.sleep(1)
@@ -25,59 +25,61 @@
         nonlocal received_sleep_sync
         nonlocal call_count
         received_sleep_sync = True
         call_count += 1
         time.sleep(1)
         return Message("Key2", "Calling async")
 
-    asyncraft.register_handler(asyncraft.SyncHandler("1", keys=["Key1", "Key3"],
+    asyncraft.register_handler(asyncraft.SyncHandler(keys=["Key1", "Key3"],
                                                      callback=call_back_value_sync)
                                )
 
-    asyncraft.register_handler(asyncraft.AsyncHandler("2", keys=["Key2"],
+    asyncraft.register_handler(asyncraft.AsyncHandler(keys=["Key2"],
                                                       callback=call_back_value_async)
                                )
 
     async def main():
         asyncraft.broadcast(Message(("Key1", "Key3"), "Calling sync"))
         await asyncio.sleep(0.5)
         assert received_sleep_sync
         assert not received_sleep_async
         await asyncio.sleep(2)
     gb = asyncraft._global_broker
     asyncraft.start(main())
     assert received_sleep_sync
     assert received_sleep_async
     assert call_count == 1
+    asyncraft.shutdown()
 
 
 def test_asyncraft_cal_and_wait():
-    asyncraft.reset()
+    asyncraft.init()
     called = 0
 
-    @asyncraft.asyncraft_handler("2", keys=["Key2"])
+    @asyncraft.asyncraft_handler(keys=["Key2"])
     async def call_back_value_async(message: Message):
         assert message.key == "Key2"
         assert message.value == "Calling async"
         nonlocal called
         called += 1
         return Message("Key4", "Sleep Finished!")
 
-    @asyncraft.asyncraft_handler("1", keys=["Key1"])
+    @asyncraft.asyncraft_handler(keys=["Key1"])
     def call_back_value_sync(message: Message):
         assert message.key == "Key1"
         assert message.value == "Calling sync"
         nonlocal called
         called += 1
         return Message("Key3", "Calling async")
 
     async def main():
         nonlocal called
-        message = await asyncraft.broadcast_and_wait(Message(("Key1"), "Calling sync"), ["Key3"])
+        message = await asyncraft.broadcast_and_wait(Message("Key1", "Calling sync"), ["Key3"])
         assert message.key == "Key3"
         assert message.value == "Calling async"
-        message = await asyncraft.broadcast_and_wait(Message(("Key2"), "Calling async"), ["Key4"])
+        message = await asyncraft.broadcast_and_wait(Message("Key2", "Calling async"), ["Key4"])
         assert message.key == "Key4"
         assert message.value == "Sleep Finished!"
 
     asyncraft.start(main())
     assert called == 2
+    asyncraft.shutdown()
```

### Comparing `asyncraft-0.0.2/tests/test_pool.py` & `asyncraft-0.0.3/tests/test_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import asyncio
+
+import asyncraft
 from asyncraft.handler import SyncHandler, AsyncHandler
 from asyncraft.message import Message
 from asyncraft.pool import Pool
 
 
 def test_sync_handler():
-    handler = SyncHandler("Sync", keys=["Test"],
+    handler = SyncHandler(keys=["Test"],
                           callback=lambda message: Message("Test1" + message.key, "Value1" + message.value))
     message = Message("Test", "Value")
     call_back_value = None
 
     async def run():
         def callback(message):
             nonlocal call_back_value
@@ -26,15 +28,15 @@
     assert call_back_value == Message("Test1Test", "Value1Value")
 
 
 def test_async_handler():
     async def handler_function(message: Message):
         return Message("Test1" + message.key, "Value1" + message.value)
 
-    handler = AsyncHandler("Async", keys=["Test"],
+    handler = AsyncHandler(keys=["Test"],
                            callback=handler_function)
     message = Message("Test", "Value")
     call_back_value = None
 
     async def run():
         def callback(message):
             nonlocal call_back_value
```

### Comparing `asyncraft-0.0.2/tests/test_queue.py` & `asyncraft-0.0.3/tests/test_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from asyncraft import MessageQueue
 from asyncraft.message import Message
 
 total_count = 2000
 
 
 def test_queue():
-    asyncraft.reset()
-    queue = MessageQueue("queue1", ["Key", "Key1"])
+    asyncraft.init()
+    queue = MessageQueue(["Key", "Key1"])
     asyncraft.register_queue(queue)
 
     async def reader_1():
         """This reader will read from the queue asynchronously."""
         read_messages = set()
         nonlocal queue
         reader_1_count = 0
@@ -58,7 +58,8 @@
     async def run():
         reads1, reads2, _ = await asyncio.gather(reader_1(), asyncio.get_running_loop().run_in_executor(None, reader_2),
                                                  producer())
         assert len(reads1) + len(reads2) == total_count
         assert reads1.intersection(reads2) == set()
 
     asyncraft.start(run())
+    asyncraft.shutdown()
```

### Comparing `asyncraft-0.0.2/LICENSE` & `asyncraft-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncraft-0.0.2/README.md` & `asyncraft-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,60 +24,60 @@
 Synchronous handlers are executed in a separate thread, while asynchronous handlers are executed in an asyncio event loop.
 ```python
 import asyncraft
 from asyncraft.handler import SyncHandler, AsyncHandler
 ...
 # Create a sync handler with decorator.
 # All sync handlers will be executed in a separate thread of a thread pool.
-@asyncraft.asyncraft_handler("handler_0", keys=["key"])
+@asyncraft.asyncraft_handler(keys=["key"])
 def handler_0(message):
     print(message)
     #Handlers can return a message
     return asyncraft.Message(key='key1', value='value1')
 ...
 
 # Create an async handler with decorator
 # All async handlers will be executed in an asyncio event loop.
-@asyncraft.asyncraft_handler("handler_1", keys=["key"])
+@asyncraft.asyncraft_handler(keys=["key"])
 async def handler_1(message):
     print(message)
 ...
 
 # Create a sync handler without decorator
 # First define the callback function
 def handler_2_function(message):
     print(message)
 #Then create the handler
-handler = SyncHandler("handler_2", keys=["key"], callback=handler_2_function)
+handler = SyncHandler(keys=["key"], callback=handler_2_function)
 #Register the handler
 asyncraft.register_handler(handler)
 
 ...
 
 # Create an async handler without decorator
 #First again define the callback function
 async def handler_3_function(message):
     print(message)
 #Then create the handler
-handler = AsyncHandler("handler_3", keys=["key"], callback=handler_3_function)
+handler = AsyncHandler(keys=["key"], callback=handler_3_function)
 #Register the handler
 asyncraft.register_handler(handler)
 ...
 ```
 ### Queues
 Another major part of Asyncraft are queues.
 Queues listen to keys and store messages before they are processed further.
 ```python
 from asyncraft import MessageQueue
 from asyncraft import Message
 import asyncraft
 ...
 #Create a queue which listenes to keys 'Key' and 'Key1'.
 #All messages with at least one of those keys will be stored in the queue.
-queue = MessageQueue("queue_1", ["Key", "Key1"])
+queue = MessageQueue(["Key", "Key1"])
 #Register the queue
 asyncraft.register_queue(queue)
 ...
 #Get the next message from the queue. If the queue is empty, block until a message is available.
 message: Message = queue.get(blocking=True)
 ...
 #Get the next message from the queue in an async context. If the queue is empty, block until a message is available.
@@ -103,23 +103,23 @@
 This example demonstrates how to use Asyncraft to create a simple ping-pong system.
 ```python
 import asyncio
 import time
 import asyncraft
 
 
-@asyncraft.asyncraft_handler("Ping", keys=["Ping"])
+@asyncraft.asyncraft_handler(keys=["Ping"])
 def ping_handler_function(message):
     """This is a sync handler that will respond to the Pong handler. It will be executed in a separate thread."""
     print(f"Received {message.key} with value {message.value}")
     time.sleep(1)
     return asyncraft.Message("Pong", message.value + 1)
 
 
-@asyncraft.asyncraft_handler("Pong", keys=["Pong"])
+@asyncraft.asyncraft_handler(keys=["Pong"])
 async def pong_handler_function(message):
     """This is an async handler that will respond to the Ping handler. It will be executed in the event loop."""
     print(f"Received {message.key} with value {message.value}")
     await asyncio.sleep(1)
     return asyncraft.Message("Ping", message.value + 1)
 
 
@@ -180,13 +180,13 @@
         async_producer(),
         asyncio.to_thread(reader, queue),
         asyncio.to_thread(producer)
     )
 
 
 if __name__ == "__main__":
-    queue = MessageQueue("queue1", ["Key", "Key1"])
+    queue = MessageQueue(["Key", "Key1"])
     asyncraft.register_queue(queue)
     asyncraft.start(main())
 ```
 ### License
 This project is licensed under the terms of the MIT license.
```

### Comparing `asyncraft-0.0.2/pyproject.toml` & `asyncraft-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.pytest.ini_options]
 pythonpath = [
   ".", "src",
 ]
 
 [project]
 name = "asyncraft"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Kilian Müller", email="kilian@mueller.ai"},
 ]
 description = "Simple message/event passing with asyncio and threading support."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `asyncraft-0.0.2/PKG-INFO` & `asyncraft-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: asyncraft
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple message/event passing with asyncio and threading support.
 Project-URL: Homepage, https://github.com/Morxos/asyncraft
 Project-URL: Issues, https://github.com/Morxos/asyncraft/issues
 Author-email: Kilian Müller <kilian@mueller.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,60 +38,60 @@
 Synchronous handlers are executed in a separate thread, while asynchronous handlers are executed in an asyncio event loop.
 ```python
 import asyncraft
 from asyncraft.handler import SyncHandler, AsyncHandler
 ...
 # Create a sync handler with decorator.
 # All sync handlers will be executed in a separate thread of a thread pool.
-@asyncraft.asyncraft_handler("handler_0", keys=["key"])
+@asyncraft.asyncraft_handler(keys=["key"])
 def handler_0(message):
     print(message)
     #Handlers can return a message
     return asyncraft.Message(key='key1', value='value1')
 ...
 
 # Create an async handler with decorator
 # All async handlers will be executed in an asyncio event loop.
-@asyncraft.asyncraft_handler("handler_1", keys=["key"])
+@asyncraft.asyncraft_handler(keys=["key"])
 async def handler_1(message):
     print(message)
 ...
 
 # Create a sync handler without decorator
 # First define the callback function
 def handler_2_function(message):
     print(message)
 #Then create the handler
-handler = SyncHandler("handler_2", keys=["key"], callback=handler_2_function)
+handler = SyncHandler(keys=["key"], callback=handler_2_function)
 #Register the handler
 asyncraft.register_handler(handler)
 
 ...
 
 # Create an async handler without decorator
 #First again define the callback function
 async def handler_3_function(message):
     print(message)
 #Then create the handler
-handler = AsyncHandler("handler_3", keys=["key"], callback=handler_3_function)
+handler = AsyncHandler(keys=["key"], callback=handler_3_function)
 #Register the handler
 asyncraft.register_handler(handler)
 ...
 ```
 ### Queues
 Another major part of Asyncraft are queues.
 Queues listen to keys and store messages before they are processed further.
 ```python
 from asyncraft import MessageQueue
 from asyncraft import Message
 import asyncraft
 ...
 #Create a queue which listenes to keys 'Key' and 'Key1'.
 #All messages with at least one of those keys will be stored in the queue.
-queue = MessageQueue("queue_1", ["Key", "Key1"])
+queue = MessageQueue(["Key", "Key1"])
 #Register the queue
 asyncraft.register_queue(queue)
 ...
 #Get the next message from the queue. If the queue is empty, block until a message is available.
 message: Message = queue.get(blocking=True)
 ...
 #Get the next message from the queue in an async context. If the queue is empty, block until a message is available.
@@ -117,23 +117,23 @@
 This example demonstrates how to use Asyncraft to create a simple ping-pong system.
 ```python
 import asyncio
 import time
 import asyncraft
 
 
-@asyncraft.asyncraft_handler("Ping", keys=["Ping"])
+@asyncraft.asyncraft_handler(keys=["Ping"])
 def ping_handler_function(message):
     """This is a sync handler that will respond to the Pong handler. It will be executed in a separate thread."""
     print(f"Received {message.key} with value {message.value}")
     time.sleep(1)
     return asyncraft.Message("Pong", message.value + 1)
 
 
-@asyncraft.asyncraft_handler("Pong", keys=["Pong"])
+@asyncraft.asyncraft_handler(keys=["Pong"])
 async def pong_handler_function(message):
     """This is an async handler that will respond to the Ping handler. It will be executed in the event loop."""
     print(f"Received {message.key} with value {message.value}")
     await asyncio.sleep(1)
     return asyncraft.Message("Ping", message.value + 1)
 
 
@@ -194,13 +194,13 @@
         async_producer(),
         asyncio.to_thread(reader, queue),
         asyncio.to_thread(producer)
     )
 
 
 if __name__ == "__main__":
-    queue = MessageQueue("queue1", ["Key", "Key1"])
+    queue = MessageQueue(["Key", "Key1"])
     asyncraft.register_queue(queue)
     asyncraft.start(main())
 ```
 ### License
 This project is licensed under the terms of the MIT license.
```

