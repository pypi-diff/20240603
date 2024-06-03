# Comparing `tmp/funzin_vc_utils-1.0.2-py3-none-any.whl.zip` & `tmp/funzin_vc_utils-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4736 bytes, number of entries: 8
+Zip file size: 4531 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       24 b- defN 23-Jun-22 05:48 fz_logger/__init__.py
--rw-rw-r--  2.0 unx     2479 b- defN 24-May-29 05:33 fz_logger/fz_logger.py
+-rw-rw-r--  2.0 unx     2498 b- defN 24-Jun-03 03:05 fz_logger/fz_logger.py
 -rw-rw-r--  2.0 unx       21 b- defN 24-Jun-03 02:48 fz_mqtt/__init__.py
--rw-rw-r--  2.0 unx     3715 b- defN 24-Jun-03 02:50 fz_mqtt/fz_mqtt.py
--rw-rw-r--  2.0 unx     3042 b- defN 24-Jun-03 03:02 funzin_vc_utils-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Jun-03 03:02 funzin_vc_utils-1.0.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       36 b- defN 24-Jun-03 03:02 funzin_vc_utils-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      634 b- defN 24-Jun-03 03:02 funzin_vc_utils-1.0.2.dist-info/RECORD
-8 files, 10043 bytes uncompressed, 3626 bytes compressed:  63.9%
+-rw-rw-r--  2.0 unx     3718 b- defN 24-Jun-03 03:11 fz_mqtt/fz_mqtt.py
+-rw-rw-r--  2.0 unx     2419 b- defN 24-Jun-03 03:14 funzin_vc_utils-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Jun-03 03:14 funzin_vc_utils-1.0.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       36 b- defN 24-Jun-03 03:14 funzin_vc_utils-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      634 b- defN 24-Jun-03 03:14 funzin_vc_utils-1.0.3.dist-info/RECORD
+8 files, 9442 bytes uncompressed, 3421 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: fz_mqtt/__init__.py
 Comment: 
 
 Filename: fz_mqtt/fz_mqtt.py
 Comment: 
 
-Filename: funzin_vc_utils-1.0.2.dist-info/METADATA
+Filename: funzin_vc_utils-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: funzin_vc_utils-1.0.2.dist-info/WHEEL
+Filename: funzin_vc_utils-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: funzin_vc_utils-1.0.2.dist-info/top_level.txt
+Filename: funzin_vc_utils-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: funzin_vc_utils-1.0.2.dist-info/RECORD
+Filename: funzin_vc_utils-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fz_logger/fz_logger.py

```diff
@@ -1,26 +1,27 @@
 import logging
 import os
 import sys
 from datetime import datetime
 from logging import handlers
+
 import colorlog
 
 
 class Logger:
-    def __init__(self, level: str, save_path: str = None):
-        self.save_path = save_path
+    def __init__(self, config:dict):
+        self.save_path = config["logger"]["save_path"]
         if self.save_path is not None:
             save = True
             os.makedirs(self.save_path, exist_ok=True)
         else:
             save = False
 
         self.settings = {
-            "LEVEL": self.lookup_table(level),
+            "LEVEL": self.lookup_table(config["logger"]["level"]),
             "FILENAME": self.__class__.__module__,
             "MAYBYTES": 15 * 1024 * 1024,
             "BACKUPCOUNT": 100,
             "FORMAT": "%(log_color)s[%(levelname)-8s]%(reset)s [%(name)s]: %(module)s:%(lineno)d:  %(message)s",
             "SAVE": save,
         }
```

## fz_mqtt/fz_mqtt.py

```diff
@@ -102,10 +102,10 @@
                     self.logger.warning("pub data is None")
             else:
                 self.reconnect()
 
         except Exception as e:
             self.logger.error(f"{inspect.currentframe().f_code.co_name} - {e}")
 
-    def sub_data(self):
+    def sub_message(self):
         self.add_listener(self.mqtt_callback)
         self.client.loop_forever()
```

## Comparing `funzin_vc_utils-1.0.2.dist-info/METADATA` & `funzin_vc_utils-1.0.3.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funzin-vc-utils
-Version: 1.0.2
+Version: 1.0.3
 Summary: funzin_vc_utils is a package that provides various utilities for python programming.
 Home-page: 
 Author: dnchoi
 Author-email: luke.dn.choi@funzin.co.kr
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -21,86 +21,77 @@
 To use the logger package, follow these steps:
 
 1. Import the logger module:
     ```python
     from fz_logger.fz_logger import Logger
     ```
 
-2. Create a logger object in class:
+2. Create a Logger object in class:
     ```python
-    from fz_logger.fz_logger import Logger
     class template(Logger):
         def __init__(self):
             super().__init__(level=config["logger"]["level"], save_path=config["logger"]["save_path"])
         ...
     ```
 
     ```python
     self.logger.debug("This is a debug message")
     self.logger.info("This is an info message")
     self.logger.warning("This is a warning message")
     self.logger.error("This is an error message")
     self.logger.critical("This is a critical message")
     ```
 
-3. Create a logger object in not class:
+3. Create a Logger object in not class:
     ```python
-    from fz_logger.fz_logger import Logger
     logger = Logger(level="INFO", save_path="app-logs").logger
     ...
     ```
 
     ```python
     logger.debug("This is a debug message")
     logger.info("This is an info message")
     logger.warning("This is a warning message")
     logger.error("This is an error message")
     logger.critical("This is a critical message")
     ```
-### MQTT
-"""
-This module provides a MQTT client implementation.
 
-Usage:
-    1. Import the `mqtt_client` module.
-    2. Create an instance of the `MQTTClient` class.
-    3. Set the necessary connection parameters using the `set_connection_params` method.
-    4. Connect to the MQTT broker using the `connect` method.
-    5. Subscribe to topics using the `subscribe` method.
-    6. Publish messages using the `publish` method.
-    7. Handle incoming messages using the `on_message` callback.
-    8. Disconnect from the MQTT broker using the `disconnect` method.
+### MQTT
+This module provides a MQTT client implementation. follow these steps:
 
-Example:
+1. Import the mqttc lient module:
+    ```python
+    from fz_mqtt.fz_mqtt import MqttClient
     ```
-    from fz_mqtt import mqtt_client
-
-    # Create an instance of the MQTTClient class
-    client = mqtt_client.MQTTClient()
-
-    # Set the connection parameters
-    client.set_connection_params("mqtt.example.com", 1883, "username", "password")
-
-    # Connect to the MQTT broker
-    client.connect()
 
-    # Subscribe to a topic
-    client.subscribe("my/topic")
-
-    # Publish a message
-    client.publish("my/topic", "Hello, MQTT!")
+2. Create a MqttClient object in class:
+    ```python
+    config = {
+        "mqtt": {
+            "id": "mqtt_id"
+            "pw": "mqtt_pw"
+            "host": "mqtt_host"
+            "port": 1883
+            "qos": 1
+            "pub-topic": "insert your topic"
+            "sub-topic": "insert your topic"
+        }
+    }
+    mqtt_client = MqttTools(config=config)
+    ```
+3. Publish message
+    ```python
+    self.mqtt_client.pub_message(
+        topic=config["mqtt"]["pub-topic"],
+        msg="your message,
+    )
+    ```
 
-    # Define a callback function to handle incoming messages
-    def on_message(topic, message):
-        print(f"Received message on topic '{topic}': {message}")
+4. Subscribe message
+    ```python
+    import threading
+    sub_mqtt = MqttServerClient(config=opt)
 
-    # Set the callback function
-    client.on_message = on_message
+    subscriber_th = threading.Thread(target=sub_mqtt.sub_message, daemon=True)
+    subscriber_th.start()
 
-    # Disconnect from the MQTT broker
-    client.disconnect()
     ```
-
-Note:
-    - This module requires the `paho-mqtt` library to be installed.
-    - Make sure to handle exceptions when using the MQTT client methods.
-"""
```

