# Comparing `tmp/event_outbox-0.1.3.tar.gz` & `tmp/event_outbox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_outbox-0.1.3.tar", max compression
+gzip compressed data, was "event_outbox-0.1.5.tar", max compression
```

## Comparing `event_outbox-0.1.3.tar` & `event_outbox-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      281 2024-06-02 08:39:05.199122 event_outbox-0.1.3/README.md
--rw-r--r--   0        0        0      156 2024-06-02 08:36:10.632838 event_outbox-0.1.3/event_outbox/__init__.py
--rw-r--r--   0        0        0    13414 2024-06-02 08:36:10.660838 event_outbox-0.1.3/event_outbox/outbox.py
--rw-r--r--   0        0        0        0 2024-06-02 03:57:20.174057 event_outbox-0.1.3/event_outbox/py.typed
--rw-r--r--   0        0        0      731 2024-06-02 08:37:26.845835 event_outbox-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 event_outbox-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      281 2024-06-02 08:39:05.199122 event_outbox-0.1.5/README.md
+-rw-r--r--   0        0        0      156 2024-06-02 08:36:10.632838 event_outbox-0.1.5/event_outbox/__init__.py
+-rw-r--r--   0        0        0    13684 2024-06-03 06:39:42.695634 event_outbox-0.1.5/event_outbox/outbox.py
+-rw-r--r--   0        0        0        0 2024-06-02 03:57:20.174057 event_outbox-0.1.5/event_outbox/py.typed
+-rw-r--r--   0        0        0      731 2024-06-03 06:39:43.571646 event_outbox-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 event_outbox-0.1.5/PKG-INFO
```

### Comparing `event_outbox-0.1.3/event_outbox/outbox.py` & `event_outbox-0.1.5/event_outbox/outbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import asyncio
 import logging
 import uuid
 from asyncio import CancelledError
 from collections import deque
-from contextlib import AbstractAsyncContextManager, asynccontextmanager, suppress
+from contextlib import (
+    AbstractAsyncContextManager,
+    asynccontextmanager,
+    nullcontext,
+    suppress,
+)
 from datetime import UTC, datetime, timedelta
 from enum import IntEnum
 from typing import Any, AsyncIterator, Deque, Mapping, Protocol
 
 import pymongo.errors
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from bson import Timestamp
@@ -73,15 +78,15 @@
 
     def event_listener(
         self, mongo_session: AsyncIOMotorClientSession
     ) -> AbstractAsyncContextManager[EventListener]:
         async def event_listener() -> AsyncIterator[EventListener]:
             events: Deque[Event] = deque()
             listener = EventListener(events)
-            async with mongo_session.start_transaction():
+            async with _ensure_in_transaction(mongo_session):
                 yield listener
                 documents = []
                 while events:
                     event = events.popleft()
                     document = {
                         "_id": event.model_dump(
                             mode="json",
@@ -319,14 +324,22 @@
                             ex,
                         )
                         continue
                     await self.kafka_consumer.commit()
                     break
 
 
+def _ensure_in_transaction(
+    mongo_session: AsyncIOMotorClientSession,
+) -> AbstractAsyncContextManager[Any]:
+    if bool(mongo_session.in_transaction):
+        return nullcontext()
+    return mongo_session.start_transaction()
+
+
 class _ResumeChangeStreamErrorCode(IntEnum):
     CHANGE_STREAM_FATAL_ERROR = 280
     CHANGE_STREAM_HISTORY_LOST = 286
 
 
 class _EventAlreadyHandledError(Exception):
     pass
```

### Comparing `event_outbox-0.1.3/pyproject.toml` & `event_outbox-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-outbox"
-version = "0.1.3"
+version = "0.1.5"
 description = "Transactional outbox and idempotent consumer"
 authors = ["Yuriy Kehter <yuriy.kehter@gmail.com>"]
 packages = [{ include = "event_outbox" }]
 repository = "https://github.com/returnnullptr/event-outbox"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `event_outbox-0.1.3/PKG-INFO` & `event_outbox-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-outbox
-Version: 0.1.3
+Version: 0.1.5
 Summary: Transactional outbox and idempotent consumer
 Home-page: https://github.com/returnnullptr/event-outbox
 Author: Yuriy Kehter
 Author-email: yuriy.kehter@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

