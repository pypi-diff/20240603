# Comparing `tmp/eink_calendar-0.2.0.tar.gz` & `tmp/eink_calendar-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eink_calendar-0.2.0.tar", max compression
+gzip compressed data, was "eink_calendar-0.2.1.tar", max compression
```

## Comparing `eink_calendar-0.2.0.tar` & `eink_calendar-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5513 2023-11-24 16:03:02.608589 eink_calendar-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     1193 2024-05-28 00:04:30.022934 eink_calendar-0.2.0/README.md
--rw-r--r--   0        0        0       66 2024-04-29 02:46:00.712186 eink_calendar-0.2.0/eink_calendar/__init__.py
--rw-r--r--   0        0        0     2398 2024-05-27 23:50:55.086114 eink_calendar-0.2.0/eink_calendar/__main__.py
--rw-r--r--   0        0        0      198 2024-04-29 02:52:44.826512 eink_calendar-0.2.0/eink_calendar/api/__init__.py
--rw-r--r--   0        0        0     2968 2024-05-28 00:04:30.002933 eink_calendar-0.2.0/eink_calendar/api/client.py
--rw-r--r--   0        0        0      957 2024-04-29 02:46:47.255992 eink_calendar-0.2.0/eink_calendar/api/event.py
--rw-r--r--   0        0        0     1439 2024-04-29 02:46:47.255992 eink_calendar-0.2.0/eink_calendar/api/event_stream.py
--rw-r--r--   0        0        0     1169 2024-05-28 00:03:28.001350 eink_calendar-0.2.0/eink_calendar/display.py
--rw-r--r--   0        0        0   212004 2023-11-24 16:03:02.612589 eink_calendar-0.2.0/eink_calendar/lora.ttf
--rw-r--r--   0        0        0       77 2024-05-22 18:22:32.647084 eink_calendar-0.2.0/eink_calendar/ui/__init__.py
--rw-r--r--   0        0        0     1585 2024-05-22 18:27:10.364189 eink_calendar-0.2.0/eink_calendar/ui/event.py
--rw-r--r--   0        0        0      837 2024-05-22 18:26:45.330959 eink_calendar-0.2.0/eink_calendar/ui/text.py
--rw-r--r--   0        0        0     1428 2024-05-28 00:05:05.815848 eink_calendar-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2247 1970-01-01 00:00:00.000000 eink_calendar-0.2.0/setup.py
--rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 eink_calendar-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5513 2023-11-24 16:03:02.608589 eink_calendar-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     1193 2024-05-28 00:04:30.022934 eink_calendar-0.2.1/README.md
+-rw-r--r--   0        0        0       66 2024-04-29 02:46:00.712186 eink_calendar-0.2.1/eink_calendar/__init__.py
+-rw-r--r--   0        0        0     2398 2024-05-28 06:15:17.922768 eink_calendar-0.2.1/eink_calendar/__main__.py
+-rw-r--r--   0        0        0      198 2024-04-29 02:52:44.826512 eink_calendar-0.2.1/eink_calendar/api/__init__.py
+-rw-r--r--   0        0        0     2968 2024-05-28 00:04:30.002933 eink_calendar-0.2.1/eink_calendar/api/client.py
+-rw-r--r--   0        0        0      957 2024-04-29 02:46:47.255992 eink_calendar-0.2.1/eink_calendar/api/event.py
+-rw-r--r--   0        0        0     1452 2024-06-03 14:58:13.562492 eink_calendar-0.2.1/eink_calendar/api/event_stream.py
+-rw-r--r--   0        0        0     1182 2024-06-03 14:58:13.554491 eink_calendar-0.2.1/eink_calendar/display.py
+-rw-r--r--   0        0        0   212004 2023-11-24 16:03:02.612589 eink_calendar-0.2.1/eink_calendar/lora.ttf
+-rw-r--r--   0        0        0       77 2024-05-22 18:22:32.647084 eink_calendar-0.2.1/eink_calendar/ui/__init__.py
+-rw-r--r--   0        0        0     1585 2024-05-22 18:27:10.364189 eink_calendar-0.2.1/eink_calendar/ui/event.py
+-rw-r--r--   0        0        0      837 2024-05-22 18:26:45.330959 eink_calendar-0.2.1/eink_calendar/ui/text.py
+-rw-r--r--   0        0        0     1428 2024-06-03 14:58:36.103257 eink_calendar-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2247 1970-01-01 00:00:00.000000 eink_calendar-0.2.1/setup.py
+-rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 eink_calendar-0.2.1/PKG-INFO
```

### Comparing `eink_calendar-0.2.0/LICENSE.md` & `eink_calendar-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/README.md` & `eink_calendar-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/eink_calendar/__main__.py` & `eink_calendar-0.2.1/eink_calendar/__main__.py`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/eink_calendar/api/client.py` & `eink_calendar-0.2.1/eink_calendar/api/client.py`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/eink_calendar/api/event.py` & `eink_calendar-0.2.1/eink_calendar/api/event.py`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/eink_calendar/api/event_stream.py` & `eink_calendar-0.2.1/eink_calendar/api/event_stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class EventStream:
     def __init__(self, client: Client, poll_delay: float = 60):
         self._client = client
         self._poll_delay = poll_delay
         self._output = Queue[list[Event]]()
         self._running = True
-        self._thread = Thread(target=self._run)
+        self._thread = Thread(target=self._run, daemon=True)
         self._thread.start()
 
     def get(self) -> Optional[list[Event]]:
         try:
             return self._output.get_nowait()
         except Empty:
             return None
```

### Comparing `eink_calendar-0.2.0/eink_calendar/display.py` & `eink_calendar-0.2.1/eink_calendar/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class EInkDisplay(Display):
     def __init__(self) -> None:
         self._inky = Inky7Colour()
         self._image_queue = Queue[Image.Image]()
         self._running = True
-        self._thread = Thread(target=self._run)
+        self._thread = Thread(target=self._run, daemon=True)
         self._thread.start()
 
     def set_image(self, image: Image.Image) -> None:
         self._image_queue.put(image)
 
     def close(self) -> None:
         self._running = False
```

### Comparing `eink_calendar-0.2.0/eink_calendar/lora.ttf` & `eink_calendar-0.2.1/eink_calendar/lora.ttf`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/eink_calendar/ui/event.py` & `eink_calendar-0.2.1/eink_calendar/ui/event.py`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/eink_calendar/ui/text.py` & `eink_calendar-0.2.1/eink_calendar/ui/text.py`

 * *Files identical despite different names*

### Comparing `eink_calendar-0.2.0/pyproject.toml` & `eink_calendar-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eink-calendar"
-version = "0.2.0"
+version = "0.2.1"
 description = "Shows Google Calendar events on an Inky Impression display"
 authors = ["Tyler Compton <xaviosx@gmail.com>"]
 readme = "README.md"
 packages = [ { include = "eink_calendar" } ]
 
 [tool.poetry.scripts]
 eink-calendar = "eink_calendar.__main__:main"
```

### Comparing `eink_calendar-0.2.0/setup.py` & `eink_calendar-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pyxdg>=0.28,<0.29']
 
 entry_points = \
 {'console_scripts': ['eink-calendar = eink_calendar.__main__:main']}
 
 setup_kwargs = {
     'name': 'eink-calendar',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Shows Google Calendar events on an Inky Impression display',
     'long_description': "# eInk Calendar\n\nDisplays Google Calendar events on an Inky Impression display connected to a\nRaspberry Pi.\n\n![Example showing how the UI looks](https://i.imgur.com/cKqnSmU.png)\n\n## Installation\n\nThis project is available on PyPI and can be installed with `pipx`.\n\n```bash\npipx install eink-calendar\n```\n\nThen, you will need to create a desktop OAuth2 client ID using the Google Cloud\nconsole. For details on how to do this, see\n[Google's Documentation][oauth2_client_docs].\n\nOnce you have created the client ID, download the client secret JSON file to\n`~/.local/share/eink-calendar/credentials.json`.\n\nThen, start the application:\n\n```bash\neink-calendar\n```\n\nA browser window will automatically open prompting you to give eInk Calendar\nread access to your calendars. Once this process completes, the application\nwill start. You only need to complete this process once.\n\n## Development\n\nIf you want to develop without the eInk display connected, start the\napplication with the following flag:\n\n```bash\neink-calendar --no-display\n```\n\nThe generated images will be opened using your image viewer instead.\n\n[oauth2_client_docs]: https://developers.google.com/identity/protocols/oauth2/native-app\n",
     'author': 'Tyler Compton',
     'author_email': 'xaviosx@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eink_calendar-0.2.0/PKG-INFO` & `eink_calendar-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eink-calendar
-Version: 0.2.0
+Version: 0.2.1
 Summary: Shows Google Calendar events on an Inky Impression display
 Author: Tyler Compton
 Author-email: xaviosx@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

