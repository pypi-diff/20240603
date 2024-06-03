# Comparing `tmp/unzipwalk-1.2.1.tar.gz` & `tmp/unzipwalk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unzipwalk-1.2.1.tar", last modified: Fri May 31 19:27:18 2024, max compression
+gzip compressed data, was "unzipwalk-1.3.0.tar", last modified: Mon Jun  3 11:02:21 2024, max compression
```

## Comparing `unzipwalk-1.2.1.tar` & `unzipwalk-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 19:27:18.122310 unzipwalk-1.2.1/
--rw-r--r--   0 haukex    (1000) haukex    (1000)     7652 2024-05-22 15:08:44.000000 unzipwalk-1.2.1/LICENSE.txt
--rw-r--r--   0 haukex    (1000) haukex    (1000)    12362 2024-05-31 19:27:18.122310 unzipwalk-1.2.1/PKG-INFO
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    11149 2024-05-31 19:19:59.000000 unzipwalk-1.2.1/README.md
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    10178 2024-05-31 19:15:24.000000 unzipwalk-1.2.1/pyproject.toml
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       19 2024-05-22 09:16:06.000000 unzipwalk-1.2.1/requirements.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       38 2024-05-31 19:27:18.122310 unzipwalk-1.2.1/setup.cfg
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 19:27:18.110304 unzipwalk-1.2.1/tests/
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    12874 2024-05-31 18:12:28.000000 unzipwalk-1.2.1/tests/test_unzipwalk.py
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 19:27:18.110304 unzipwalk-1.2.1/unzipwalk/
--rw-rw-r--   0 haukex    (1000) haukex    (1000)    19074 2024-05-31 19:18:23.000000 unzipwalk-1.2.1/unzipwalk/__init__.py
-drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-05-31 19:27:18.122310 unzipwalk-1.2.1/unzipwalk.egg-info/
--rw-r--r--   0 haukex    (1000) haukex    (1000)    12362 2024-05-31 19:27:18.000000 unzipwalk-1.2.1/unzipwalk.egg-info/PKG-INFO
--rw-rw-r--   0 haukex    (1000) haukex    (1000)      299 2024-05-31 19:27:18.000000 unzipwalk-1.2.1/unzipwalk.egg-info/SOURCES.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)        1 2024-05-31 19:27:18.000000 unzipwalk-1.2.1/unzipwalk.egg-info/dependency_links.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       45 2024-05-31 19:27:18.000000 unzipwalk-1.2.1/unzipwalk.egg-info/entry_points.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       18 2024-05-31 19:27:18.000000 unzipwalk-1.2.1/unzipwalk.egg-info/requires.txt
--rw-rw-r--   0 haukex    (1000) haukex    (1000)       10 2024-05-31 19:27:18.000000 unzipwalk-1.2.1/unzipwalk.egg-info/top_level.txt
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-06-03 11:02:21.961428 unzipwalk-1.3.0/
+-rw-r--r--   0 haukex    (1000) haukex    (1000)     7652 2024-05-22 15:08:44.000000 unzipwalk-1.3.0/LICENSE.txt
+-rw-r--r--   0 haukex    (1000) haukex    (1000)    14839 2024-06-03 11:02:21.961428 unzipwalk-1.3.0/PKG-INFO
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    13626 2024-06-03 10:56:11.000000 unzipwalk-1.3.0/README.md
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    10178 2024-06-03 10:27:38.000000 unzipwalk-1.3.0/pyproject.toml
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       19 2024-05-22 09:16:06.000000 unzipwalk-1.3.0/requirements.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       38 2024-06-03 11:02:21.961428 unzipwalk-1.3.0/setup.cfg
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-06-03 11:02:21.905400 unzipwalk-1.3.0/tests/
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    16520 2024-06-03 10:17:08.000000 unzipwalk-1.3.0/tests/test_unzipwalk.py
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-06-03 11:02:21.917406 unzipwalk-1.3.0/unzipwalk/
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)    23101 2024-06-03 10:48:01.000000 unzipwalk-1.3.0/unzipwalk/__init__.py
+drwxrwxr-x   0 haukex    (1000) haukex    (1000)        0 2024-06-03 11:02:21.961428 unzipwalk-1.3.0/unzipwalk.egg-info/
+-rw-r--r--   0 haukex    (1000) haukex    (1000)    14839 2024-06-03 11:02:21.000000 unzipwalk-1.3.0/unzipwalk.egg-info/PKG-INFO
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)      299 2024-06-03 11:02:21.000000 unzipwalk-1.3.0/unzipwalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)        1 2024-06-03 11:02:21.000000 unzipwalk-1.3.0/unzipwalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       45 2024-06-03 11:02:21.000000 unzipwalk-1.3.0/unzipwalk.egg-info/entry_points.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       18 2024-06-03 11:02:21.000000 unzipwalk-1.3.0/unzipwalk.egg-info/requires.txt
+-rw-rw-r--   0 haukex    (1000) haukex    (1000)       10 2024-06-03 11:02:21.000000 unzipwalk-1.3.0/unzipwalk.egg-info/top_level.txt
```

### Comparing `unzipwalk-1.2.1/LICENSE.txt` & `unzipwalk-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unzipwalk-1.2.1/PKG-INFO` & `unzipwalk-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: unzipwalk
-Version: 1.2.1
-Summary: Recursively walk into directories and archives
-Author-email: Hauke D <haukex@zero-g.net>
-Project-URL: Repository, https://github.com/haukex/unzipwalk
-Project-URL: Bug Tracker, https://github.com/haukex/unzipwalk/issues
-Project-URL: Changelog, https://github.com/haukex/unzipwalk/blob/main/CHANGELOG.md
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Archiving
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: igbpyutils==0.5.0
-
 <a id="module-unzipwalk"></a>
 
 # Recursively Walk Into Directories and Archives
 
 This module primarily provides the function [`unzipwalk()`](#function-unzipwalk), which recursively walks
 into directories and compressed files and returns all files, directories, etc. found,
 together with binary file handles (file objects) for reading the files.
@@ -92,14 +65,16 @@
 This generator recursively walks into directories and compressed files and yields named tuples of type [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 * **Parameters:**
   * **paths** – A filename or iterable of filenames.
   * **matcher** – When you provide this optional argument, it must be a callable that accepts a sequence of paths
     as its only argument, and returns a boolean value whether this filename should be further processed or not.
 
+<a id="unzipwalk.UnzipWalkResult"></a>
+
 ### *class* unzipwalk.UnzipWalkResult(names: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...], typ: [FileType](#unzipwalk.FileType), hnd: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 Return type for [`unzipwalk()`](#function-unzipwalk).
 
 #### names *: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...]*
 
 A tuple of the filename(s) as [`pathlib`](https://docs.python.org/3/library/pathlib.html#module-pathlib) objects. The first element is always the physical file in the file system.
@@ -110,24 +85,67 @@
 
 A [`FileType`](#unzipwalk.FileType) value representing the type of the current file.
 
 #### hnd *: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None)*
 
 When [`typ`](#unzipwalk.UnzipWalkResult.typ) is [`FileType.FILE`](#unzipwalk.FileType), this is a [`ReadOnlyBinary`](#unzipwalk.ReadOnlyBinary) file handle (file object)
 for reading the file contents in binary mode. Otherwise, this is [`None`](https://docs.python.org/3/library/constants.html#None).
+If this object was produced by [`from_checksum_line()`](#unzipwalk.UnzipWalkResult.from_checksum_line), this handle will read the checksum of the data, *not the data itself!*
 
 #### validate()
 
 Validate whether the object’s fields are set properly and throw errors if not.
 
 Intended for internal use, mainly when type checkers are not being used.
 [`unzipwalk()`](#function-unzipwalk) validates all the results it returns.
 
 * **Returns:**
   The object itself, for method chaining.
+* **Raises:**
+  [**ValueError**](https://docs.python.org/3/library/exceptions.html#ValueError)**,** [**TypeError**](https://docs.python.org/3/library/exceptions.html#TypeError) – If the object is invalid.
+
+<a id="unzipwalk.UnzipWalkResult.checksum_line"></a>
+
+#### checksum_line(hash_algo: [str](https://docs.python.org/3/library/stdtypes.html#str))
+
+Encodes this object into a line of text suitable for use as a checksum line.
+
+Intended mostly for internal use by the `--checksum` CLI option.
+
+**Warning:** Requires that the file handle be open (for files), and will read from it!
+
+See also [`from_checksum_line()`](#unzipwalk.UnzipWalkResult.from_checksum_line) for the inverse operation.
+
+* **Parameters:**
+  **hash_algo** – The hashing algorithm to use, as recognized by [`hashlib.new()`](https://docs.python.org/3/library/hashlib.html#hashlib.new).
+* **Returns:**
+  The checksum line, without trailing newline.
+
+<a id="unzipwalk.UnzipWalkResult.from_checksum_line"></a>
+
+#### *classmethod* from_checksum_line(line: [str](https://docs.python.org/3/library/stdtypes.html#str), \*, windows: [bool](https://docs.python.org/3/library/functions.html#bool) = False)
+
+Decodes a checksum line as produced by [`checksum_line()`](#unzipwalk.UnzipWalkResult.checksum_line).
+
+**Warning:** The `hnd` of the returned object will *not* be a handle to
+the data from the file, instead it will be a handle to read the checksum of the file!
+(You could use [`recursive_open()`](#unzipwalk.recursive_open) to open the files themselves.)
+
+Intended as a utility function for use when reading files produced by the `--checksum` CLI option.
+
+* **Parameters:**
+  * **line** – The line to parse.
+  * **windows** – Set this to [`True`](https://docs.python.org/3/library/constants.html#True) if the pathname in the line is in Windows format,
+    otherwise it is assumed the filename is in POSIX format.
+* **Returns:**
+  The [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult) object, or [`None`](https://docs.python.org/3/library/constants.html#None) for empty or comment lines.
+* **Raises:**
+  [**ValueError**](https://docs.python.org/3/library/exceptions.html#ValueError) – If the line could not be parsed.
+
+<a id="unzipwalk.ReadOnlyBinary"></a>
 
 ### *class* unzipwalk.ReadOnlyBinary(\*args, \*\*kwargs)
 
 Interface for the file handle (file object) used in [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 The interface is the intersection of [`typing.BinaryIO`](https://docs.python.org/3/library/typing.html#typing.BinaryIO), [`gzip.GzipFile`](https://docs.python.org/3/library/gzip.html#gzip.GzipFile), and [`zipfile.ZipExtFile`](https://docs.python.org/3/library/zipfile.html#module-zipfile).
 Because [`gzip.GzipFile`](https://docs.python.org/3/library/gzip.html#gzip.GzipFile) doesn’t implement `.tell()`, that method isn’t available here.
@@ -147,14 +165,16 @@
 
 #### readline(limit: [int](https://docs.python.org/3/library/functions.html#int) = -1)
 
 #### seekable()
 
 #### seek(offset: [int](https://docs.python.org/3/library/functions.html#int), whence: [int](https://docs.python.org/3/library/functions.html#int) = 0)
 
+<a id="unzipwalk.FileType"></a>
+
 ### *class* unzipwalk.FileType(value)
 
 Used in [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult) to indicate the type of the file.
 
 #### FILE *= 0*
 
 A regular file.
```

### Comparing `unzipwalk-1.2.1/README.md` & `unzipwalk-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: unzipwalk
+Version: 1.3.0
+Summary: Recursively walk into directories and archives
+Author-email: Hauke D <haukex@zero-g.net>
+Project-URL: Repository, https://github.com/haukex/unzipwalk
+Project-URL: Bug Tracker, https://github.com/haukex/unzipwalk/issues
+Project-URL: Changelog, https://github.com/haukex/unzipwalk/blob/main/CHANGELOG.md
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: Archiving
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: igbpyutils==0.5.0
+
 <a id="module-unzipwalk"></a>
 
 # Recursively Walk Into Directories and Archives
 
 This module primarily provides the function [`unzipwalk()`](#function-unzipwalk), which recursively walks
 into directories and compressed files and returns all files, directories, etc. found,
 together with binary file handles (file objects) for reading the files.
@@ -65,14 +92,16 @@
 This generator recursively walks into directories and compressed files and yields named tuples of type [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 * **Parameters:**
   * **paths** – A filename or iterable of filenames.
   * **matcher** – When you provide this optional argument, it must be a callable that accepts a sequence of paths
     as its only argument, and returns a boolean value whether this filename should be further processed or not.
 
+<a id="unzipwalk.UnzipWalkResult"></a>
+
 ### *class* unzipwalk.UnzipWalkResult(names: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...], typ: [FileType](#unzipwalk.FileType), hnd: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 Return type for [`unzipwalk()`](#function-unzipwalk).
 
 #### names *: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...]*
 
 A tuple of the filename(s) as [`pathlib`](https://docs.python.org/3/library/pathlib.html#module-pathlib) objects. The first element is always the physical file in the file system.
@@ -83,24 +112,67 @@
 
 A [`FileType`](#unzipwalk.FileType) value representing the type of the current file.
 
 #### hnd *: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None)*
 
 When [`typ`](#unzipwalk.UnzipWalkResult.typ) is [`FileType.FILE`](#unzipwalk.FileType), this is a [`ReadOnlyBinary`](#unzipwalk.ReadOnlyBinary) file handle (file object)
 for reading the file contents in binary mode. Otherwise, this is [`None`](https://docs.python.org/3/library/constants.html#None).
+If this object was produced by [`from_checksum_line()`](#unzipwalk.UnzipWalkResult.from_checksum_line), this handle will read the checksum of the data, *not the data itself!*
 
 #### validate()
 
 Validate whether the object’s fields are set properly and throw errors if not.
 
 Intended for internal use, mainly when type checkers are not being used.
 [`unzipwalk()`](#function-unzipwalk) validates all the results it returns.
 
 * **Returns:**
   The object itself, for method chaining.
+* **Raises:**
+  [**ValueError**](https://docs.python.org/3/library/exceptions.html#ValueError)**,** [**TypeError**](https://docs.python.org/3/library/exceptions.html#TypeError) – If the object is invalid.
+
+<a id="unzipwalk.UnzipWalkResult.checksum_line"></a>
+
+#### checksum_line(hash_algo: [str](https://docs.python.org/3/library/stdtypes.html#str))
+
+Encodes this object into a line of text suitable for use as a checksum line.
+
+Intended mostly for internal use by the `--checksum` CLI option.
+
+**Warning:** Requires that the file handle be open (for files), and will read from it!
+
+See also [`from_checksum_line()`](#unzipwalk.UnzipWalkResult.from_checksum_line) for the inverse operation.
+
+* **Parameters:**
+  **hash_algo** – The hashing algorithm to use, as recognized by [`hashlib.new()`](https://docs.python.org/3/library/hashlib.html#hashlib.new).
+* **Returns:**
+  The checksum line, without trailing newline.
+
+<a id="unzipwalk.UnzipWalkResult.from_checksum_line"></a>
+
+#### *classmethod* from_checksum_line(line: [str](https://docs.python.org/3/library/stdtypes.html#str), \*, windows: [bool](https://docs.python.org/3/library/functions.html#bool) = False)
+
+Decodes a checksum line as produced by [`checksum_line()`](#unzipwalk.UnzipWalkResult.checksum_line).
+
+**Warning:** The `hnd` of the returned object will *not* be a handle to
+the data from the file, instead it will be a handle to read the checksum of the file!
+(You could use [`recursive_open()`](#unzipwalk.recursive_open) to open the files themselves.)
+
+Intended as a utility function for use when reading files produced by the `--checksum` CLI option.
+
+* **Parameters:**
+  * **line** – The line to parse.
+  * **windows** – Set this to [`True`](https://docs.python.org/3/library/constants.html#True) if the pathname in the line is in Windows format,
+    otherwise it is assumed the filename is in POSIX format.
+* **Returns:**
+  The [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult) object, or [`None`](https://docs.python.org/3/library/constants.html#None) for empty or comment lines.
+* **Raises:**
+  [**ValueError**](https://docs.python.org/3/library/exceptions.html#ValueError) – If the line could not be parsed.
+
+<a id="unzipwalk.ReadOnlyBinary"></a>
 
 ### *class* unzipwalk.ReadOnlyBinary(\*args, \*\*kwargs)
 
 Interface for the file handle (file object) used in [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 The interface is the intersection of [`typing.BinaryIO`](https://docs.python.org/3/library/typing.html#typing.BinaryIO), [`gzip.GzipFile`](https://docs.python.org/3/library/gzip.html#gzip.GzipFile), and [`zipfile.ZipExtFile`](https://docs.python.org/3/library/zipfile.html#module-zipfile).
 Because [`gzip.GzipFile`](https://docs.python.org/3/library/gzip.html#gzip.GzipFile) doesn’t implement `.tell()`, that method isn’t available here.
@@ -120,14 +192,16 @@
 
 #### readline(limit: [int](https://docs.python.org/3/library/functions.html#int) = -1)
 
 #### seekable()
 
 #### seek(offset: [int](https://docs.python.org/3/library/functions.html#int), whence: [int](https://docs.python.org/3/library/functions.html#int) = 0)
 
+<a id="unzipwalk.FileType"></a>
+
 ### *class* unzipwalk.FileType(value)
 
 Used in [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult) to indicate the type of the file.
 
 #### FILE *= 0*
 
 A regular file.
```

### Comparing `unzipwalk-1.2.1/pyproject.toml` & `unzipwalk-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unzipwalk"
 description = "Recursively walk into directories and archives"
-version = "1.2.1"
+version = "1.3.0"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.md"
 requires-python = ">=3.9"
 dynamic = ["dependencies"]
 # https://pypi.org/classifiers/
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `unzipwalk-1.2.1/unzipwalk/__init__.py` & `unzipwalk-1.3.0/unzipwalk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -93,27 +93,29 @@
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 details.
 
 You should have received a copy of the GNU Lesser General Public License
 along with this program. If not, see https://www.gnu.org/licenses/
 """
+import re
 import io
+import ast
 import stat
 import hashlib
 import argparse
 from enum import Enum
 from gzip import GzipFile
 from tarfile import TarFile
 from zipfile import ZipFile
 from itertools import chain
 from fnmatch import fnmatch
 from contextlib import contextmanager
-from pathlib import PurePosixPath, PurePath, Path
 from collections.abc import Generator, Sequence, Callable
+from pathlib import PurePosixPath, PurePath, Path, PureWindowsPath
 from typing import Optional, cast, Protocol, Literal, BinaryIO, NamedTuple, runtime_checkable, Union
 from igbpyutils.file import AnyPaths, to_Paths, Filename
 import igbpyutils.error
 
 class FileType(Enum):
     """Used in :class:`UnzipWalkResult` to indicate the type of the file."""
     #: A regular file.
@@ -143,44 +145,130 @@
     def closed(self) -> bool: ...
     def readable(self) -> Literal[True]: ...
     def read(self, n: int = -1) -> bytes: ...
     def readline(self, limit: int = -1) -> bytes: ...
     def seekable(self) -> bool: ...
     def seek(self, offset: int, whence: int = io.SEEK_SET) -> int: ...
 
+def decode_tuple(code :str) -> tuple[str, ...]:
+    """Helper function to parse a string as produced by :func:`repr` from a :class:`tuple` of one or more :class:`str`.
+
+    :param code: The code to parse.
+    :return: The :class:`tuple` that was parsed.
+    :raises ValueError: If the code could not be parsed.
+    """
+    try:
+        tree = ast.parse(code)
+    except SyntaxError as ex:
+        raise ValueError() from ex
+    if not len(tree.body)==1 or not isinstance(tree.body[0], ast.Expr) or not isinstance(tree.body[0].value, ast.Tuple) \
+            or not isinstance(tree.body[0].value.ctx, ast.Load) or len(tree.body[0].value.elts)<1:
+        raise ValueError(f"failed to decode tuple {code!r}")
+    elements = []
+    for e in tree.body[0].value.elts:
+        if not isinstance(e, ast.Constant) or not isinstance(e.value, str):
+            raise ValueError(f"failed to decode tuple {code!r}")
+        elements.append(e.value)
+    return tuple(elements)
+
+CHECKSUM_LINE_RE = re.compile(r'^([0-9a-f]+) \*(.+)$')
+CHECKSUM_COMMENT_RE = re.compile(r'^# ([A-Z]+) (.+)$')
+
 class UnzipWalkResult(NamedTuple):
     """Return type for :func:`unzipwalk`."""
     #: A tuple of the filename(s) as :mod:`pathlib` objects. The first element is always the physical file in the file system.
     #: If the tuple has more than one element, then the yielded file is contained in a compressed file, possibly nested in
     #: other compressed file(s), and the last element of the tuple will contain the file's actual name.
     names :tuple[PurePath, ...]
     #: A :class:`FileType` value representing the type of the current file.
     typ :FileType
     #: When :attr:`typ` is :class:`FileType.FILE<FileType>`, this is a :class:`ReadOnlyBinary` file handle (file object)
     #: for reading the file contents in binary mode. Otherwise, this is :obj:`None`.
+    #: If this object was produced by :meth:`from_checksum_line`, this handle will read the checksum of the data, *not the data itself!*
     hnd :Optional[ReadOnlyBinary] = None
+
     def validate(self):
         """Validate whether the object's fields are set properly and throw errors if not.
 
         Intended for internal use, mainly when type checkers are not being used.
         :func:`unzipwalk` validates all the results it returns.
 
-        :return: The object itself, for method chaining."""
+        :return: The object itself, for method chaining.
+        :raises ValueError, TypeError: If the object is invalid.
+        """
         if not self.names:
             raise ValueError('names is empty')
         if not all( isinstance(n, PurePath) for n in self.names ):  # pyright: ignore [reportUnnecessaryIsInstance]
             raise TypeError(f"invalid names {self.names!r}")
         if not isinstance(self.typ, FileType):  # pyright: ignore [reportUnnecessaryIsInstance]
             raise TypeError(f"invalid type {self.typ!r}")
         if self.typ==FileType.FILE and not isinstance(self.hnd, ReadOnlyBinary):
             raise TypeError(f"invalid handle {self.hnd!r}")
         if self.typ!=FileType.FILE and self.hnd is not None:
             raise TypeError(f"invalid handle, should be None but is {self.hnd!r}")
         return self
 
+    def checksum_line(self, hash_algo :str) -> str:
+        """Encodes this object into a line of text suitable for use as a checksum line.
+
+        Intended mostly for internal use by the ``--checksum`` CLI option.
+
+        **Warning:** Requires that the file handle be open (for files), and will read from it!
+
+        See also :meth:`from_checksum_line` for the inverse operation.
+
+        :param hash_algo: The hashing algorithm to use, as recognized by :func:`hashlib.new`.
+        :return: The checksum line, without trailing newline.
+        """
+        names = tuple( str(n) for n in self.names )
+        if len(names)==1 and names[0] and names[0].strip()==names[0] and not names[0].startswith('(') \
+                and '\n' not in names[0] and '\r' not in names[0]:  # pylint: disable=too-many-boolean-expressions
+            name = names[0]
+        else:
+            name = repr(names)
+            assert name.startswith('(')
+        assert '\n' not in name and '\r' not in name
+        if self.typ == FileType.FILE:
+            assert self.hnd is not None
+            h = hashlib.new(hash_algo)
+            h.update(self.hnd.read())
+            return f"{h.hexdigest().lower()} *{name}"
+        return f"# {self.typ.name} {name}"
+
+    @classmethod
+    def from_checksum_line(cls, line :str, *, windows :bool=False) -> Optional['UnzipWalkResult']:
+        """Decodes a checksum line as produced by :meth:`checksum_line`.
+
+        **Warning:** The ``hnd`` of the returned object will *not* be a handle to
+        the data from the file, instead it will be a handle to read the checksum of the file!
+        (You could use :func:`recursive_open` to open the files themselves.)
+
+        Intended as a utility function for use when reading files produced by the ``--checksum`` CLI option.
+
+        :param line: The line to parse.
+        :param windows: Set this to :obj:`True` if the pathname in the line is in Windows format,
+            otherwise it is assumed the filename is in POSIX format.
+        :return: The :class:`UnzipWalkResult` object, or :obj:`None` for empty or comment lines.
+        :raises ValueError: If the line could not be parsed.
+        """
+        if not line.strip():
+            return None
+        path_cls = PureWindowsPath if windows else PurePosixPath
+        def mk_names(name :str)-> tuple[PurePath, ...]:
+            names = decode_tuple(name) if name.startswith('(') else (name,)
+            return tuple(path_cls(p) for p in names)
+        if line.lstrip().startswith('#'):  # comment, be lenient to allow user comments
+            if m := CHECKSUM_COMMENT_RE.match(line):
+                if m.group(1) in FileType.__members__:
+                    return cls( names=mk_names(m.group(2)), typ=FileType[m.group(1)] )
+            return None
+        if m := CHECKSUM_LINE_RE.match(line):
+            return cls( names=mk_names(m.group(2)), typ=FileType.FILE, hnd=cast(ReadOnlyBinary, io.BytesIO(bytes.fromhex(m.group(1)))) )
+        raise ValueError(f"failed to decode checksum line {line!r}")
+
 @contextmanager
 def _inner_recur_open(fh :BinaryIO, fns :tuple[PurePath, ...]) -> Generator[BinaryIO, None, None]:
     try:
         bl = fns[0].name.lower()
         assert fns
         if len(fns)==1:
             yield fh
@@ -338,24 +426,18 @@
 def main(argv=None):
     igbpyutils.error.init_handlers()
     parser = _arg_parser()
     args = parser.parse_args(argv)
     def matcher(paths :Sequence[PurePath]) -> bool:
         return not any( fnmatch(paths[-1].name, pat) for pat in args.exclude )
     for result in unzipwalk( args.paths if args.paths else Path(), matcher=matcher ):
-        names = tuple( str(n) for n in result.names )
         if args.checksum:
-            name = names[0] if len(names)==1 and not names[0].startswith('(') and '\n' not in names[0] and '\r' not in names[0] else repr(names)
-            if result.typ==FileType.FILE:
-                assert result.hnd is not None
-                h = hashlib.new(args.checksum)
-                h.update(result.hnd.read())
-                print(f"{h.hexdigest()} *{name}")
-            elif args.all_files:
-                print(f"# {result.typ.name} {name}")
+            if result.typ == FileType.FILE or args.all_files:
+                print(result.checksum_line(args.checksum))
         else:
+            names = tuple( str(n) for n in result.names )
             if result.typ==FileType.FILE and args.dump:
                 assert result.hnd is not None
                 print(f"{result.typ.name} {names!r} {result.hnd.read()!r}")
             elif result.typ==FileType.FILE or args.all_files:
                 print(f"{result.typ.name} {names!r}")
     parser.exit(0)
```

### Comparing `unzipwalk-1.2.1/unzipwalk.egg-info/PKG-INFO` & `unzipwalk-1.3.0/unzipwalk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unzipwalk
-Version: 1.2.1
+Version: 1.3.0
 Summary: Recursively walk into directories and archives
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Repository, https://github.com/haukex/unzipwalk
 Project-URL: Bug Tracker, https://github.com/haukex/unzipwalk/issues
 Project-URL: Changelog, https://github.com/haukex/unzipwalk/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -92,14 +92,16 @@
 This generator recursively walks into directories and compressed files and yields named tuples of type [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 * **Parameters:**
   * **paths** – A filename or iterable of filenames.
   * **matcher** – When you provide this optional argument, it must be a callable that accepts a sequence of paths
     as its only argument, and returns a boolean value whether this filename should be further processed or not.
 
+<a id="unzipwalk.UnzipWalkResult"></a>
+
 ### *class* unzipwalk.UnzipWalkResult(names: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...], typ: [FileType](#unzipwalk.FileType), hnd: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None) = None)
 
 Return type for [`unzipwalk()`](#function-unzipwalk).
 
 #### names *: [tuple](https://docs.python.org/3/library/stdtypes.html#tuple)[[PurePath](https://docs.python.org/3/library/pathlib.html#pathlib.PurePath), ...]*
 
 A tuple of the filename(s) as [`pathlib`](https://docs.python.org/3/library/pathlib.html#module-pathlib) objects. The first element is always the physical file in the file system.
@@ -110,24 +112,67 @@
 
 A [`FileType`](#unzipwalk.FileType) value representing the type of the current file.
 
 #### hnd *: [ReadOnlyBinary](#unzipwalk.ReadOnlyBinary) | [None](https://docs.python.org/3/library/constants.html#None)*
 
 When [`typ`](#unzipwalk.UnzipWalkResult.typ) is [`FileType.FILE`](#unzipwalk.FileType), this is a [`ReadOnlyBinary`](#unzipwalk.ReadOnlyBinary) file handle (file object)
 for reading the file contents in binary mode. Otherwise, this is [`None`](https://docs.python.org/3/library/constants.html#None).
+If this object was produced by [`from_checksum_line()`](#unzipwalk.UnzipWalkResult.from_checksum_line), this handle will read the checksum of the data, *not the data itself!*
 
 #### validate()
 
 Validate whether the object’s fields are set properly and throw errors if not.
 
 Intended for internal use, mainly when type checkers are not being used.
 [`unzipwalk()`](#function-unzipwalk) validates all the results it returns.
 
 * **Returns:**
   The object itself, for method chaining.
+* **Raises:**
+  [**ValueError**](https://docs.python.org/3/library/exceptions.html#ValueError)**,** [**TypeError**](https://docs.python.org/3/library/exceptions.html#TypeError) – If the object is invalid.
+
+<a id="unzipwalk.UnzipWalkResult.checksum_line"></a>
+
+#### checksum_line(hash_algo: [str](https://docs.python.org/3/library/stdtypes.html#str))
+
+Encodes this object into a line of text suitable for use as a checksum line.
+
+Intended mostly for internal use by the `--checksum` CLI option.
+
+**Warning:** Requires that the file handle be open (for files), and will read from it!
+
+See also [`from_checksum_line()`](#unzipwalk.UnzipWalkResult.from_checksum_line) for the inverse operation.
+
+* **Parameters:**
+  **hash_algo** – The hashing algorithm to use, as recognized by [`hashlib.new()`](https://docs.python.org/3/library/hashlib.html#hashlib.new).
+* **Returns:**
+  The checksum line, without trailing newline.
+
+<a id="unzipwalk.UnzipWalkResult.from_checksum_line"></a>
+
+#### *classmethod* from_checksum_line(line: [str](https://docs.python.org/3/library/stdtypes.html#str), \*, windows: [bool](https://docs.python.org/3/library/functions.html#bool) = False)
+
+Decodes a checksum line as produced by [`checksum_line()`](#unzipwalk.UnzipWalkResult.checksum_line).
+
+**Warning:** The `hnd` of the returned object will *not* be a handle to
+the data from the file, instead it will be a handle to read the checksum of the file!
+(You could use [`recursive_open()`](#unzipwalk.recursive_open) to open the files themselves.)
+
+Intended as a utility function for use when reading files produced by the `--checksum` CLI option.
+
+* **Parameters:**
+  * **line** – The line to parse.
+  * **windows** – Set this to [`True`](https://docs.python.org/3/library/constants.html#True) if the pathname in the line is in Windows format,
+    otherwise it is assumed the filename is in POSIX format.
+* **Returns:**
+  The [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult) object, or [`None`](https://docs.python.org/3/library/constants.html#None) for empty or comment lines.
+* **Raises:**
+  [**ValueError**](https://docs.python.org/3/library/exceptions.html#ValueError) – If the line could not be parsed.
+
+<a id="unzipwalk.ReadOnlyBinary"></a>
 
 ### *class* unzipwalk.ReadOnlyBinary(\*args, \*\*kwargs)
 
 Interface for the file handle (file object) used in [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult).
 
 The interface is the intersection of [`typing.BinaryIO`](https://docs.python.org/3/library/typing.html#typing.BinaryIO), [`gzip.GzipFile`](https://docs.python.org/3/library/gzip.html#gzip.GzipFile), and [`zipfile.ZipExtFile`](https://docs.python.org/3/library/zipfile.html#module-zipfile).
 Because [`gzip.GzipFile`](https://docs.python.org/3/library/gzip.html#gzip.GzipFile) doesn’t implement `.tell()`, that method isn’t available here.
@@ -147,14 +192,16 @@
 
 #### readline(limit: [int](https://docs.python.org/3/library/functions.html#int) = -1)
 
 #### seekable()
 
 #### seek(offset: [int](https://docs.python.org/3/library/functions.html#int), whence: [int](https://docs.python.org/3/library/functions.html#int) = 0)
 
+<a id="unzipwalk.FileType"></a>
+
 ### *class* unzipwalk.FileType(value)
 
 Used in [`UnzipWalkResult`](#unzipwalk.UnzipWalkResult) to indicate the type of the file.
 
 #### FILE *= 0*
 
 A regular file.
```

