# Comparing `tmp/pymkv2-2.0.4.tar.gz` & `tmp/pymkv2-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymkv2-2.0.4.tar", max compression
+gzip compressed data, was "pymkv2-2.0.5.tar", max compression
```

## Comparing `pymkv2-2.0.4.tar` & `pymkv2-2.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-05-27 19:54:19.213593 pymkv2-2.0.4/LICENSE.txt
--rw-r--r--   0        0        0     2397 2024-05-27 19:54:19.213593 pymkv2-2.0.4/README.md
--rw-r--r--   0        0        0      479 2024-05-27 19:54:19.213593 pymkv2-2.0.4/pymkv/BCP47.py
--rw-r--r--   0        0        0      480 2024-05-27 19:54:19.213593 pymkv2-2.0.4/pymkv/ISO639_2.py
--rw-r--r--   0        0        0     3692 2024-05-27 19:54:19.213593 pymkv2-2.0.4/pymkv/MKVAttachment.py
--rw-r--r--   0        0        0    41345 2024-05-27 19:54:19.213593 pymkv2-2.0.4/pymkv/MKVFile.py
--rw-r--r--   0        0        0    15711 2024-05-27 19:54:19.213593 pymkv2-2.0.4/pymkv/MKVTrack.py
--rw-r--r--   0        0        0    11593 2024-05-27 19:54:19.213593 pymkv2-2.0.4/pymkv/Timestamp.py
--rw-r--r--   0        0        0     1824 2024-05-27 19:54:19.213593 pymkv2-2.0.4/pymkv/TypeTrack.py
--rw-r--r--   0        0        0     5888 2024-05-27 19:54:19.217593 pymkv2-2.0.4/pymkv/Verifications.py
--rw-r--r--   0        0        0      784 2024-05-27 19:54:19.217593 pymkv2-2.0.4/pymkv/__init__.py
--rw-r--r--   0        0        0      822 2024-05-27 19:54:19.217593 pymkv2-2.0.4/pymkv/utils.py
--rw-r--r--   0        0        0     3241 2024-05-27 19:54:19.217593 pymkv2-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     3515 1970-01-01 00:00:00.000000 pymkv2-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-06-02 22:33:27.638645 pymkv2-2.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1781 2024-06-02 22:33:27.638645 pymkv2-2.0.5/README.md
+-rw-r--r--   0        0        0      479 2024-06-02 22:33:27.638645 pymkv2-2.0.5/pymkv/BCP47.py
+-rw-r--r--   0        0        0      480 2024-06-02 22:33:27.638645 pymkv2-2.0.5/pymkv/ISO639_2.py
+-rw-r--r--   0        0        0     3692 2024-06-02 22:33:27.638645 pymkv2-2.0.5/pymkv/MKVAttachment.py
+-rw-r--r--   0        0        0    41575 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pymkv/MKVFile.py
+-rw-r--r--   0        0        0    15774 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pymkv/MKVTrack.py
+-rw-r--r--   0        0        0    11593 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pymkv/Timestamp.py
+-rw-r--r--   0        0        0     1824 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pymkv/TypeTrack.py
+-rw-r--r--   0        0        0     5922 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pymkv/Verifications.py
+-rw-r--r--   0        0        0      784 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pymkv/__init__.py
+-rw-r--r--   0        0        0      822 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pymkv/utils.py
+-rw-r--r--   0        0        0     3258 2024-06-02 22:33:27.642645 pymkv2-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 pymkv2-2.0.5/PKG-INFO
```

### Comparing `pymkv2-2.0.4/LICENSE.txt` & `pymkv2-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.4/README.md` & `pymkv2-2.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # pymkv2
 [![PyPI Version](https://img.shields.io/pypi/v/pymkv2.svg)](https://pypi.python.org/pypi/pymkv2)
 [![License](https://img.shields.io/github/license/gitbib/pymkv.svg)](https://github.com/gitbib/pymkv/LICENSE.txt)
+[![codecov](https://codecov.io/github/GitBib/pymkv2/branch/master/graph/badge.svg?token=2JDX5HHGUO)](https://codecov.io/github/GitBib/pymkv2)
+[![versions](https://img.shields.io/pypi/pyversions/pymkv2.svg)](https://github.com/GitBib/pymkv2)
 
 pymkv2 is a Python wrapper for mkvmerge and other tools in the MKVToolNix suite. It provides support for muxing,
 splitting, linking, chapters, tags, and attachments through the use of mkvmerge.
 
 ## About pymkv2
 it's a fork of the [project](https://github.com/sheldonkwoodward/pymkv). Pymkv2 is a Python 3 library for manipulating MKV files with mkvmerge. Constructing mkvmerge commands manually can
 quickly become confusing and complex. To remedy this, I decided to write this library to make mkvmerge more
@@ -21,21 +23,7 @@
 
 You can also clone the repo and run the following command in the project root to install the source code as editable:
 
     $ pip install -e .
 
 ## Documentation
 The documentation for pymkv can be found [here](https://gitbib.github.io/pymkv2/) or in the project's docstrings.
-
-### Tests
-Added the first tests for the project. Still a lot to do, but it’s a start. Currently, 49% is covered by tests.
-
-### Cleanup
-~~The existing code base could use some tidying, better commenting, debugging, and a general styling overhaul. Setting up
-[pre-commit](https://pre-commit.com/) and the [Black code formatter](https://github.com/psf/black) will help keep the
-code base more readable and maintainable.~~
-
-### Features
-~~Once these first three steps are complete, pymkv will be ready to start adding new features. The goal is for pymkv to
-implement the functionality of mkvmerge and other MKVToolNix tools as closely as possible. New features and bugs will
-be added to the [GitHub issues page](https://github.com/gitbib/pymkv/issues). As pymkv progresses through
-the previous steps, this roadmap will be expanded to outline new features.~~
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymkv2-2.0.4/pymkv/MKVAttachment.py` & `pymkv2-2.0.5/pymkv/MKVAttachment.py`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.4/pymkv/MKVFile.py` & `pymkv2-2.0.5/pymkv/MKVFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 import bitmath
 
 from pymkv.ISO639_2 import is_iso639_2
 from pymkv.MKVAttachment import MKVAttachment
 from pymkv.MKVTrack import MKVTrack
 from pymkv.Timestamp import Timestamp
 from pymkv.utils import prepare_mkvtoolnix_path
-from pymkv.Verifications import checking_file_path, verify_mkvmerge
+from pymkv.Verifications import checking_file_path, verify_mkvmerge, verify_supported
 
 
 class MKVFile:
     """A class that represents an MKV file.
 
     The :class:`~pymkv.MKVFile` class can either import a pre-existing MKV file or create a new one. After an
     :class:`~pymkv.MKVFile` object has been instantiated, :class:`~pymkv.MKVTrack` objects or other
@@ -100,18 +100,22 @@
         self._global_tags_file = None
         self._link_to_previous_file = None
         self._link_to_next_file = None
         self.tracks: list[MKVTrack] = []
         self.attachments = []
         self._number_file = 0
 
-        if not verify_mkvmerge(mkvmerge_path=mkvmerge_path):
+        if not verify_mkvmerge(mkvmerge_path=self.mkvmerge_path):
             msg = "mkvmerge is not at the specified path, add it there or changed mkvmerge_path property"
             raise FileNotFoundError(msg)
 
+        if not verify_supported(file_path, mkvmerge_path=self.mkvmerge_path):
+            msg = f"The file '{file_path}' is not a valid Matroska file or is not supported."
+            raise ValueError(msg)
+
         if file_path is not None:
             # add file title
             file_path = checking_file_path(file_path)
             try:
                 info_json = json.loads(sp.check_output([*self.mkvmerge_path, "-J", file_path]).decode())  # noqa: S603
             except sp.CalledProcessError as e:
                 error_output = e.output.decode()
```

### Comparing `pymkv2-2.0.4/pymkv/MKVTrack.py` & `pymkv2-2.0.5/pymkv/MKVTrack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-""":class:`~pymkv.MKVTrack` classes are used to represent tracks within an MKV or to be used in an MKV. They can
+"""
+:class:`~pymkv.MKVTrack` classes are used to represent tracks within an MKV or to be used in an MKV. They can
 represent a video, audio, or subtitle track.
 
 Examples
 --------
+
 Below are some basic examples of how the :class:`~pymkv.MKVTrack` objects can be used.
 
 Create a new :class:`~pymkv.MKVTrack` from a track file. This example takes a standalone track file and uses it in an
 :class:`~pymkv.MKVTrack`.
 
 >>> from pymkv import MKVTrack
->>> track1 = MKVTrack('path/to/track.h264')
->>> track1.track_name = 'Some Name'
->>> track1.language = 'eng'
+>>> track1 = MKVTrack("path/to/track.h264")
+>>> track1.track_name = "Some Name"
+>>> track1.language = "eng"
 
 Create a new :class:`~pymkv.MKVTrack` from an MKV file. This example will take a specific track from an MKV and also
 prevent any global tags from being included if the :class:`~pymkv.MKVTrack` is muxed into an :class:`~pymkv.MKVFile`.
 
->>> track2 = MKVTrack('path/to/track.aac')
->>> track2.language = 'eng'
+>>> track2 = MKVTrack("path/to/track.aac")
+>>> track2.language = "eng"
 
 Create a new :class:`~pymkv.MKVTrack` from an MKV file. This example will take a specific track from an MKV and also
 prevent any global tags from being included if the :class:`~pymkv.MKVTrack` is muxed into an :class:`~pymkv.MKVFile`.
 
->>> track3 = MKVTrack('path/to/MKV.mkv', track_id=1)
+>>> track3 = MKVTrack("path/to/MKV.mkv", track_id=1)
 >>> track3.no_global_tags = True
 
 Now all these tracks can be added to an :class:`~pymkv.MKVFile` object and muxed together.
 
 >>> from pymkv import MKVFile
 >>> file = MKVFile()
 >>> file.add_track(track1)
 >>> file.add_track(track2)
 >>> file.add_track(track3)
->>> file.mux('path/to/output.mkv')
+>>> file.mux("path/to/output.mkv")
 """
 
 from __future__ import annotations
 
 import json
 import os
 import subprocess as sp
 from os import devnull
 from pathlib import Path
 
 from pymkv.BCP47 import is_bcp47
 from pymkv.ISO639_2 import is_iso639_2
 from pymkv.TypeTrack import get_track_extension
 from pymkv.utils import prepare_mkvtoolnix_path
-from pymkv.Verifications import verify_supported
+from pymkv.Verifications import checking_file_path, verify_supported
 
 
 class MKVTrack:
     """A class that represents a track for an :class:`~pymkv.MKVFile` object.
     :class:`~pymkv.MKVTrack` objects are video, audio, or subtitles. Tracks can be standalone files or a single track
     within an MKV file, both can be handled by pymkv. An :class:`~pymkv.MKVTrack` object can be added to an
     :class:`~pymkv.MKVFile` and will be included when the MKV is muxed.
@@ -183,17 +185,17 @@
         ValueError
             Raised if `file_path` is not a supported file type.
         """
         return self._file_path
 
     @file_path.setter
     def file_path(self, file_path: str) -> None:
-        file_path = str(Path(file_path).expanduser())
+        file_path = checking_file_path(file_path)
         if not verify_supported(file_path, mkvmerge_path=self.mkvmerge_path):
-            msg = '"{}" is not a supported file'
+            msg = f"The file '{file_path}' is not a valid Matroska file or is not supported."
             raise ValueError(msg)
         self._file_path = file_path
         self.track_id = 0
 
     @property
     def file_id(self) -> int:
         """int: The ID of the file the track belongs to.
```

### Comparing `pymkv2-2.0.4/pymkv/Timestamp.py` & `pymkv2-2.0.5/pymkv/Timestamp.py`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.4/pymkv/TypeTrack.py` & `pymkv2-2.0.5/pymkv/TypeTrack.py`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.4/pymkv/Verifications.py` & `pymkv2-2.0.5/pymkv/Verifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         mkvmerge_command = [*prepare_mkvtoolnix_path(mkvmerge_path), "-V"]
         output = sp.check_output(mkvmerge_command).decode()  # noqa: S603
     except (sp.CalledProcessError, FileNotFoundError):
         return False
     return bool(match("mkvmerge.*", output))
 
 
-def verify_matroska(file_path: str | os.PathLike, mkvmerge_path: str = "mkvmerge") -> bool:
+def verify_matroska(file_path: str | os.PathLike, mkvmerge_path: str | list | os.PathLike | None = "mkvmerge") -> bool:
     """
     Parameters
     ----------
     file_path : str or os.PathLike
         The path to the Matroska file to be verified.
 
     mkvmerge_path : str, optional
@@ -89,15 +89,15 @@
     This method verifies the validity of a Matroska file by checking if it is of type "Matroska"
     using the `mkvmerge` command-line tool.
     """
     if not verify_mkvmerge(mkvmerge_path=mkvmerge_path):
         msg = "mkvmerge is not at the specified path, add it there or change the mkvmerge_path property"
         raise FileNotFoundError(msg)
     try:
-        info_json = json.loads(
+        info_json: dict = json.loads(
             sp.check_output(
                 [*prepare_mkvtoolnix_path(mkvmerge_path), "-J", checking_file_path(file_path)],  # noqa: S603
             ).decode(),
         )
 
     except sp.CalledProcessError as e:
         msg = f'"{file_path}" could not be opened'
```

### Comparing `pymkv2-2.0.4/pymkv/__init__.py` & `pymkv2-2.0.5/pymkv/__init__.py`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.4/pymkv/utils.py` & `pymkv2-2.0.5/pymkv/utils.py`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.4/pyproject.toml` & `pymkv2-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pymkv2"
-version = "2.0.4"
+version = "2.0.5"
 description = "A Python wrapper for mkvmerge. It provides support for muxing, splitting, linking, chapters, tags, and attachments through the use of mkvmerge."
 authors = [
-     "GitBib <job@bnff.website>",
+    "GitBib <job@bnff.website>",
     "Sheldon Woodward <me@sheldonw.com>",
 ]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pymkv" }
 ]
@@ -39,15 +39,15 @@
 pytest-cov = "^5.0.0"
 sphinx-material = {git = "https://github.com/bashtage/sphinx-material.git"}
 
 [tool.poetry.urls]
 homepage = "https://github.com/GitBib/pymkv2"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools", "wheel"]
+requires = ["poetry-core>=1.0.0", "setuptools", "wheel", "setuptools_scm"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
```

### Comparing `pymkv2-2.0.4/PKG-INFO` & `pymkv2-2.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymkv2
-Version: 2.0.4
+Version: 2.0.5
 Summary: A Python wrapper for mkvmerge. It provides support for muxing, splitting, linking, chapters, tags, and attachments through the use of mkvmerge.
 License: MIT
 Keywords: wrapper
 Author: GitBib
 Author-email: job@bnff.website
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -25,14 +25,16 @@
 Requires-Dist: iso-639 (==0.4.5)
 Project-URL: homepage, https://github.com/GitBib/pymkv2
 Description-Content-Type: text/markdown
 
 # pymkv2
 [![PyPI Version](https://img.shields.io/pypi/v/pymkv2.svg)](https://pypi.python.org/pypi/pymkv2)
 [![License](https://img.shields.io/github/license/gitbib/pymkv.svg)](https://github.com/gitbib/pymkv/LICENSE.txt)
+[![codecov](https://codecov.io/github/GitBib/pymkv2/branch/master/graph/badge.svg?token=2JDX5HHGUO)](https://codecov.io/github/GitBib/pymkv2)
+[![versions](https://img.shields.io/pypi/pyversions/pymkv2.svg)](https://github.com/GitBib/pymkv2)
 
 pymkv2 is a Python wrapper for mkvmerge and other tools in the MKVToolNix suite. It provides support for muxing,
 splitting, linking, chapters, tags, and attachments through the use of mkvmerge.
 
 ## About pymkv2
 it's a fork of the [project](https://github.com/sheldonkwoodward/pymkv). Pymkv2 is a Python 3 library for manipulating MKV files with mkvmerge. Constructing mkvmerge commands manually can
 quickly become confusing and complex. To remedy this, I decided to write this library to make mkvmerge more
@@ -50,21 +52,7 @@
 You can also clone the repo and run the following command in the project root to install the source code as editable:
 
     $ pip install -e .
 
 ## Documentation
 The documentation for pymkv can be found [here](https://gitbib.github.io/pymkv2/) or in the project's docstrings.
 
-### Tests
-Added the first tests for the project. Still a lot to do, but it’s a start. Currently, 49% is covered by tests.
-
-### Cleanup
-~~The existing code base could use some tidying, better commenting, debugging, and a general styling overhaul. Setting up
-[pre-commit](https://pre-commit.com/) and the [Black code formatter](https://github.com/psf/black) will help keep the
-code base more readable and maintainable.~~
-
-### Features
-~~Once these first three steps are complete, pymkv will be ready to start adding new features. The goal is for pymkv to
-implement the functionality of mkvmerge and other MKVToolNix tools as closely as possible. New features and bugs will
-be added to the [GitHub issues page](https://github.com/gitbib/pymkv/issues). As pymkv progresses through
-the previous steps, this roadmap will be expanded to outline new features.~~
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

