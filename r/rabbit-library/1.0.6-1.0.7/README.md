# Comparing `tmp/rabbit_library-1.0.6.tar.gz` & `tmp/rabbit_library-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbit_library-1.0.6.tar", max compression
+gzip compressed data, was "rabbit_library-1.0.7.tar", max compression
```

## Comparing `rabbit_library-1.0.6.tar` & `rabbit_library-1.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1130 2024-05-31 17:54:14.782531 rabbit_library-1.0.6/pyproject.toml
--rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-1.0.6/rabbit_library/__init__.py
--rw-r--r--   0        0        0     9700 2024-05-31 17:56:15.289643 rabbit_library-1.0.6/rabbit_library/Rabbit.py
--rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-1.0.6/README.md
--rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rabbit_library-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1130 2024-06-03 14:02:57.301990 rabbit_library-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-1.0.7/rabbit_library/__init__.py
+-rw-r--r--   0        0        0     9715 2024-06-03 13:50:45.690012 rabbit_library-1.0.7/rabbit_library/Rabbit.py
+-rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-1.0.7/README.md
+-rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rabbit_library-1.0.7/PKG-INFO
```

### Comparing `rabbit_library-1.0.6/pyproject.toml` & `rabbit_library-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rabbit-library"
-version = "1.0.6"
+version = "1.0.7"
 description = "Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria"
 license = "MIT"
 authors = ["Eliézer Schwartz <eliezer.mail090@gmail.com>"]
 readme = "README.md"
 packages = [{include = "rabbit_library"}]
 classifiers = [    
     "Environment :: Console",
```

### Comparing `rabbit_library-1.0.6/rabbit_library/Rabbit.py` & `rabbit_library-1.0.7/rabbit_library/Rabbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         return False
 
     def __connect(self) -> None:
         # Create a credentials object with the provided username and password
         credentials = pika.PlainCredentials(self.username, self.password)
         # Create a connection parameters object with the provided host, port, and credentials
         parameters = pika.ConnectionParameters(
-            self.host, self.port, self.virtualhost, credentials)
+            self.host, self.port, self.virtualhost, credentials, heartbeat=600)
         # Create a SelectConnection with the provided parameters and a callback method to handle the established connection
         self.SelectConn = pika.BlockingConnection(parameters)
         # Start the connection's I/O loop in a separate thread
         self.channel = self.SelectConn.channel()
         if not self.channel.is_closed and self.qtd_reconnects > 0:
             self.qtd_reconnects = 0
             self.reconnect_delay_system = self.reconnect_delay_client
```

### Comparing `rabbit_library-1.0.6/README.md` & `rabbit_library-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rabbit_library-1.0.6/PKG-INFO` & `rabbit_library-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbit-library
-Version: 1.0.6
+Version: 1.0.7
 Summary: Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria
 License: MIT
 Author: Eliézer Schwartz
 Author-email: eliezer.mail090@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

