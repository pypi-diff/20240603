# Comparing `tmp/event_outbox-0.1.2.tar.gz` & `tmp/event_outbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_outbox-0.1.2.tar", max compression
+gzip compressed data, was "event_outbox-0.1.3.tar", max compression
```

## Comparing `event_outbox-0.1.2.tar` & `event_outbox-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      236 2024-06-01 15:01:09.206751 event_outbox-0.1.2/README.md
--rw-r--r--   0        0        0      165 2024-06-01 14:30:17.044489 event_outbox-0.1.2/event_outbox/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 14:02:32.595614 event_outbox-0.1.2/event_outbox/py.typed
--rw-r--r--   0        0        0    13354 2024-06-01 14:41:24.026704 event_outbox-0.1.2/event_outbox/transport.py
--rw-r--r--   0        0        0      697 2024-06-01 14:55:44.349638 event_outbox-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 event_outbox-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      281 2024-06-02 08:39:05.199122 event_outbox-0.1.3/README.md
+-rw-r--r--   0        0        0      156 2024-06-02 08:36:10.632838 event_outbox-0.1.3/event_outbox/__init__.py
+-rw-r--r--   0        0        0    13414 2024-06-02 08:36:10.660838 event_outbox-0.1.3/event_outbox/outbox.py
+-rw-r--r--   0        0        0        0 2024-06-02 03:57:20.174057 event_outbox-0.1.3/event_outbox/py.typed
+-rw-r--r--   0        0        0      731 2024-06-02 08:37:26.845835 event_outbox-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 event_outbox-0.1.3/PKG-INFO
```

### Comparing `event_outbox-0.1.2/event_outbox/transport.py` & `event_outbox-0.1.3/event_outbox/outbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     AsyncIOMotorChangeStream,
     AsyncIOMotorClient,
     AsyncIOMotorClientSession,
     AsyncIOMotorDatabase,
 )
 from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
 
-__all__ = ["Event", "EventListener", "EventTransport", "EventHandler"]
+__all__ = ["Event", "EventListener", "EventOutbox", "EventHandler"]
 
 
 class Event(BaseModel):
     topic: str
     content_schema: str
     idempotency_key: str = Field(default_factory=lambda: uuid.uuid4().hex)
     occurred_at: AwareDatetime = Field(default_factory=lambda: datetime.now(tz=UTC))
@@ -45,15 +45,15 @@
         event: Event,
         mongo_session: AsyncIOMotorClientSession,
         /,
     ) -> None:
         pass
 
 
-class EventTransport:
+class EventOutbox:
     def __init__(
         self,
         mongo_client: AsyncIOMotorClient,
         kafka_producer: AIOKafkaProducer,
         kafka_consumer: AIOKafkaConsumer,
         *,
         mongo_db: AsyncIOMotorDatabase | None = None,
@@ -103,21 +103,22 @@
         return asynccontextmanager(event_listener)()
 
     def run_event_handler(
         self, handler: EventHandler
     ) -> AbstractAsyncContextManager[None]:
         async def run_event_handler() -> AsyncIterator[None]:
             async with self._subscribe_to_mongo_change_stream(
-                # TODO: Load state to database
+                # TODO: Load state from database
                 start_after=None,
                 start_at_operation_type=None,
             ) as change_stream:
                 producer_loop = asyncio.create_task(
                     self._produce_messages(
                         change_stream,
+                        # TODO: Configure heartbeat interval
                         heartbeat=timedelta(minutes=5),
                     ),
                 )
                 consumer_loop = asyncio.create_task(
                     self._consume_messages(handler),
                 )
                 try:
@@ -140,15 +141,15 @@
                 try:
                     async with self.mongo_db[self.mongo_collection_outbox].watch(
                         [{"$match": {"operationType": {"$in": ["insert"]}}}],
                         start_after=start_after,
                     ) as change_stream:
                         yield change_stream
                 except pymongo.errors.OperationFailure as ex:
-                    if ex.code in _FailedToResumeChangeStream:
+                    if ex.code in _ResumeChangeStreamErrorCode:
                         logging.getLogger(__name__).warning(
                             "Failed to start change stream of collection %r after %r.",
                             self.mongo_collection_outbox,
                             start_after,
                             exc_info=True,
                         )
                     else:
@@ -163,15 +164,15 @@
                 try:
                     async with self.mongo_db[self.mongo_collection_outbox].watch(
                         [{"$match": {"operationType": {"$in": ["insert"]}}}],
                         start_at_operation_time=Timestamp(start_at_operation_type, 1),
                     ) as change_stream:
                         yield change_stream
                 except pymongo.errors.OperationFailure as ex:
-                    if ex.code in _FailedToResumeChangeStream:
+                    if ex.code in _ResumeChangeStreamErrorCode:
                         logging.getLogger(__name__).critical(
                             "Failed to start change stream of collection %r "
                             "at operation time: %r",
                             self.mongo_collection_outbox,
                             start_at_operation_type.isoformat(),
                             exc_info=True,
                         )
@@ -318,14 +319,14 @@
                             ex,
                         )
                         continue
                     await self.kafka_consumer.commit()
                     break
 
 
-class _FailedToResumeChangeStream(IntEnum):
+class _ResumeChangeStreamErrorCode(IntEnum):
     CHANGE_STREAM_FATAL_ERROR = 280
     CHANGE_STREAM_HISTORY_LOST = 286
 
 
 class _EventAlreadyHandledError(Exception):
     pass
```

### Comparing `event_outbox-0.1.2/pyproject.toml` & `event_outbox-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-outbox"
-version = "0.1.2"
+version = "0.1.3"
 description = "Transactional outbox and idempotent consumer"
 authors = ["Yuriy Kehter <yuriy.kehter@gmail.com>"]
 packages = [{ include = "event_outbox" }]
 repository = "https://github.com/returnnullptr/event-outbox"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -15,15 +15,16 @@
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.7"
 pytest = "^8.2.1"
 mypy = "^1.10.0"
 alt-pytest-asyncio = "^0.7.2"
 coverage = "^7.5.3"
+dynaconf = "^3.2.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.mypy.overrides]]
-module = ["aiokafka.*"]
+module = ["aiokafka.*", "dynaconf.*"]
 ignore_missing_imports = true
```

### Comparing `event_outbox-0.1.2/PKG-INFO` & `event_outbox-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-outbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transactional outbox and idempotent consumer
 Home-page: https://github.com/returnnullptr/event-outbox
 Author: Yuriy Kehter
 Author-email: yuriy.kehter@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -30,7 +30,13 @@
 
 With [poetry](https://python-poetry.org/):
 
 ```bash
 poetry add event-outbox
 ```
 
+## Development
+
+```bash
+bash cleanup.sh
+```
+
```

