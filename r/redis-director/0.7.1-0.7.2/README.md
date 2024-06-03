# Comparing `tmp/redis_director-0.7.1.tar.gz` & `tmp/redis_director-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_director-0.7.1.tar", max compression
+gzip compressed data, was "redis_director-0.7.2.tar", max compression
```

## Comparing `redis_director-0.7.1.tar` & `redis_director-0.7.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.7.1/README.md
--rw-r--r--   0        0        0      320 2024-05-20 01:51:15.699314 redis_director-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      297 2024-05-20 01:40:49.544799 redis_director-0.7.1/redis_director/__init__.py
--rw-r--r--   0        0        0     1090 2024-05-20 01:51:07.091289 redis_director-0.7.1/redis_director/callback.py
--rw-r--r--   0        0        0      808 2024-05-20 01:34:28.055535 redis_director-0.7.1/redis_director/constants.py
--rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.7.1/redis_director/handler.py
--rw-r--r--   0        0        0     4173 2024-05-20 01:50:13.871109 redis_director-0.7.1/redis_director/publisher.py
--rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.7.1/redis_director/subscriber.py
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-05-16 08:23:46.385495 redis_director-0.7.2/README.md
+-rw-r--r--   0        0        0      320 2024-06-03 06:15:42.920704 redis_director-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      297 2024-05-20 01:40:49.544799 redis_director-0.7.2/redis_director/__init__.py
+-rw-r--r--   0        0        0     1090 2024-05-20 01:51:07.091289 redis_director-0.7.2/redis_director/callback.py
+-rw-r--r--   0        0        0      808 2024-05-20 01:34:28.055535 redis_director-0.7.2/redis_director/constants.py
+-rw-r--r--   0        0        0      457 2024-05-16 07:36:15.466756 redis_director-0.7.2/redis_director/handler.py
+-rw-r--r--   0        0        0     5665 2024-06-03 06:15:31.600767 redis_director-0.7.2/redis_director/publisher.py
+-rw-r--r--   0        0        0     2427 2024-05-16 07:41:50.028080 redis_director-0.7.2/redis_director/subscriber.py
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 redis_director-0.7.2/PKG-INFO
```

### Comparing `redis_director-0.7.1/README.md` & `redis_director-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `redis_director-0.7.1/redis_director/callback.py` & `redis_director-0.7.2/redis_director/callback.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.7.1/redis_director/constants.py` & `redis_director-0.7.2/redis_director/constants.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.7.1/redis_director/publisher.py` & `redis_director-0.7.2/redis_director/publisher.py`

 * *Files 24% similar despite different names*

```diff
@@ -131,28 +131,89 @@
         self.__add_payloads_callback(
             self,
             payloads,
         )
 
         return self
 
-    def publish(
+    def __get_payloads(
         self,
-        batch_size=1,
+        batch_size: int,
     ):
         if self.__pop_payloads_callback == None:
             raise TypeError("`pop_payloads_callback` not provided!")
 
         payloads = self.__pop_payloads_callback(
             self,
             batch_size,
         )
 
         if payloads == None:
-            return self
+            return []
+
+        return payloads
+
+    def publish_max(
+        self,
+        batch_size=1,
+    ):
+        """
+        Publishes to the subscriber with the highest score.
+        """
+        payloads = self.__get_payloads(batch_size)
+
+        for payload in payloads:
+            try:
+                subscriber = max(
+                    self.__subscribers.values(),
+                    key=lambda subscriber: subscriber.score,
+                )
+
+            except:
+                raise Exception("No subscribers found!")
+
+            if subscriber.handler == None:
+                continue
+
+            subscriber.handler(subscriber, payload)
+
+    def publish_min(
+        self,
+        batch_size=1,
+    ):
+        """
+        Publishes to the subscriber with the lowest score.
+        """
+        payloads = self.__get_payloads(batch_size)
+
+        for payload in payloads:
+            try:
+                subscriber = min(
+                    self.__subscribers.values(),
+                    key=lambda subscriber: subscriber.score,
+                )
+
+            except:
+                raise Exception("No subscribers found!")
+
+            if subscriber.handler == None:
+                continue
+
+            subscriber.handler(subscriber, payload)
+
+    def publish(
+        self,
+        batch_size=1,
+    ):
+        """
+        Publishes to a random subscriber.
+
+        High score increases the odds of being chosen.
+        """
+        payloads = self.__get_payloads(batch_size)
 
         for payload in payloads:
             for subscriber in self.random_subscribers:
                 if subscriber.handler != None:
                     subscriber.handler(subscriber, payload)
 
                 break
```

### Comparing `redis_director-0.7.1/redis_director/subscriber.py` & `redis_director-0.7.2/redis_director/subscriber.py`

 * *Files identical despite different names*

### Comparing `redis_director-0.7.1/PKG-INFO` & `redis_director-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-director
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

