# Comparing `tmp/easymp3-1.2.tar.gz` & `tmp/easymp3-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymp3-1.2.tar", last modified: Sat Jun  1 21:25:16 2024, max compression
+gzip compressed data, was "easymp3-1.2.1.tar", last modified: Sun Jun  2 19:03:37 2024, max compression
```

## Comparing `easymp3-1.2.tar` & `easymp3-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 21:25:16.787364 easymp3-1.2/
--rw-rw-rw-   0        0        0     1090 2024-06-01 20:31:31.000000 easymp3-1.2/LICENSE
--rw-rw-rw-   0        0        0     6961 2024-06-01 21:25:16.786763 easymp3-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6717 2024-06-01 20:31:31.000000 easymp3-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 21:25:16.774109 easymp3-1.2/easymp3/
--rw-rw-rw-   0        0        0       52 2024-06-01 21:24:01.000000 easymp3-1.2/easymp3/__init__.py
--rw-rw-rw-   0        0        0    13994 2024-05-31 04:54:33.000000 easymp3-1.2/easymp3/easymp3.py
--rw-rw-rw-   0        0        0      514 2024-06-01 20:30:47.000000 easymp3-1.2/easymp3/exception.py
--rw-rw-rw-   0        0        0     2603 2024-05-28 00:56:24.000000 easymp3-1.2/easymp3/tag.py
--rw-rw-rw-   0        0        0     9855 2024-05-28 00:56:24.000000 easymp3-1.2/easymp3/util.py
-drwxrwxrwx   0        0        0        0 2024-06-01 21:25:16.785431 easymp3-1.2/easymp3.egg-info/
--rw-rw-rw-   0        0        0     6961 2024-06-01 21:25:16.000000 easymp3-1.2/easymp3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-06-01 21:25:16.000000 easymp3-1.2/easymp3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 21:25:16.000000 easymp3-1.2/easymp3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-06-01 21:25:16.000000 easymp3-1.2/easymp3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 21:25:16.000000 easymp3-1.2/easymp3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 21:25:16.787364 easymp3-1.2/setup.cfg
--rw-rw-rw-   0        0        0      489 2024-06-01 21:24:01.000000 easymp3-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:03:37.039027 easymp3-1.2.1/
+-rw-rw-rw-   0        0        0     1090 2024-06-01 20:31:31.000000 easymp3-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6963 2024-06-02 19:03:37.038211 easymp3-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6717 2024-06-01 20:31:31.000000 easymp3-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 19:03:37.018380 easymp3-1.2.1/easymp3/
+-rw-rw-rw-   0        0        0       52 2024-06-01 21:24:01.000000 easymp3-1.2.1/easymp3/__init__.py
+-rw-rw-rw-   0        0        0    14019 2024-06-02 18:59:51.000000 easymp3-1.2.1/easymp3/easymp3.py
+-rw-rw-rw-   0        0        0      514 2024-06-01 20:30:47.000000 easymp3-1.2.1/easymp3/exception.py
+-rw-rw-rw-   0        0        0     2603 2024-05-28 00:56:24.000000 easymp3-1.2.1/easymp3/tag.py
+-rw-rw-rw-   0        0        0    10811 2024-06-02 19:00:25.000000 easymp3-1.2.1/easymp3/util.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:03:37.023198 easymp3-1.2.1/easymp3.egg-info/
+-rw-rw-rw-   0        0        0     6963 2024-06-02 19:03:36.000000 easymp3-1.2.1/easymp3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-06-02 19:03:36.000000 easymp3-1.2.1/easymp3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:03:36.000000 easymp3-1.2.1/easymp3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 19:03:36.000000 easymp3-1.2.1/easymp3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-02 19:03:36.000000 easymp3-1.2.1/easymp3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 19:03:37.039027 easymp3-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      491 2024-06-02 19:02:17.000000 easymp3-1.2.1/setup.py
```

### Comparing `easymp3-1.2/LICENSE` & `easymp3-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easymp3-1.2/PKG-INFO` & `easymp3-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymp3
-Version: 1.2
+Version: 1.2.1
 Summary: Easily tag and manipulate MP3 files in a programmatic way.
 Author: Chase Minert
 Author-email: cminert58@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EasyMP3
```

### Comparing `easymp3-1.2/README.md` & `easymp3-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `easymp3-1.2/easymp3/easymp3.py` & `easymp3-1.2.1/easymp3/easymp3.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import shutil
 import sys
 
 from mutagen.easyid3 import EasyID3
 from mutagen.id3 import APIC, ID3NoHeaderError, ID3
 from mutagen.mp3 import MP3
 
-import exception
-import tag
-import util
-from util import INVALID_CHAR_TRANS
-from tag import Tag
+from . import exception
+
+from . import tag
+from . import util
+from .util import INVALID_CHAR_TRANS
+from .tag import Tag
 
 COVER_FROM_FILENAME = "cover_from_filename"
 
 
 class EasyMP3:
     def __init__(self, directory: str, search_subfolders=False):
         """
```

### Comparing `easymp3-1.2/easymp3/exception.py` & `easymp3-1.2.1/easymp3/exception.py`

 * *Files identical despite different names*

### Comparing `easymp3-1.2/easymp3/tag.py` & `easymp3-1.2.1/easymp3/tag.py`

 * *Files identical despite different names*

### Comparing `easymp3-1.2/easymp3/util.py` & `easymp3-1.2.1/easymp3/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import mimetypes
 import os
 import re
 import sys
 from typing import Any
 
-from mutagen.id3 import ID3
+from mutagen.easyid3 import EasyID3
+from mutagen.id3 import ID3, APIC
 from mutagen.mp3 import MP3
 
-import tag
-from tag import Tag
+from . import tag
+from . import exception
+from .tag import Tag
 
-import exception
 
 INVALID_CHAR_MAP = {
     ":": "-",
     "\\": "-",
     "/": "-",
     "*": " ",
     "?": " ",
@@ -178,14 +179,40 @@
     # If there's a match, return the group dictionary
     if match:
         result_dict = match.groupdict()
         return {getattr(Tag, key): value for key, value in result_dict.items()}
     else:
         return None
 
+def extract_tags(source_file: str, dest_file: str):
+    # Load the source MP3 file and read its tags
+    source_audio = MP3(source_file, ID3=EasyID3)
+    source_tags = source_audio.tags
+
+    # Load the destination MP3 file and initialize it for ID3 tags if not already present
+    dest_audio = MP3(dest_file, ID3=EasyID3)
+
+    # Clear existing tags in the destination file
+    dest_audio.delete()
+    dest_audio.save()
+
+    # Copy each tag from the source to the destination
+    for tag_key, tag_value in source_tags.items():
+        dest_audio[tag_key] = tag_value
+
+    # Copy the album art if present
+    source_id3 = ID3(source_file)
+    dest_id3 = ID3(dest_file)
+    for _tag in source_id3.values():
+        if isinstance(_tag, APIC):
+            dest_id3.add(_tag)
+
+    # Save the destination file with the new tags
+    dest_audio.save()
+    dest_id3.save(dest_file)
 
 def check_template(template: str) -> None:
     """
     A method to ensure that a template string does not end with .mp3
     :param template: A traditional string template
     :raises InvalidStringTemplateError: If the template ends with .mp3
     """
```

### Comparing `easymp3-1.2/easymp3.egg-info/PKG-INFO` & `easymp3-1.2.1/easymp3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymp3
-Version: 1.2
+Version: 1.2.1
 Summary: Easily tag and manipulate MP3 files in a programmatic way.
 Author: Chase Minert
 Author-email: cminert58@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EasyMP3
```

