# Comparing `tmp/wheel-axle-runtime-0.0.6.dev20240212035011.tar.gz` & `tmp/wheel_axle_runtime-0.0.6.dev20240603035837.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheel-axle-runtime-0.0.6.dev20240212035011.tar", last modified: Mon Feb 12 03:50:35 2024, max compression
+gzip compressed data, was "wheel_axle_runtime-0.0.6.dev20240603035837.tar", last modified: Mon Jun  3 03:59:08 2024, max compression
```

## Comparing `wheel-axle-runtime-0.0.6.dev20240212035011.tar` & `wheel_axle_runtime-0.0.6.dev20240603035837.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 03:50:35.026728 wheel-axle-runtime-0.0.6.dev20240212035011/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-02-12 03:50:25.000000 wheel-axle-runtime-0.0.6.dev20240212035011/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-02-12 03:50:35.026728 wheel-axle-runtime-0.0.6.dev20240212035011/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 03:50:35.026728 wheel-axle-runtime-0.0.6.dev20240212035011/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     8876 2024-02-12 03:50:25.000000 wheel-axle-runtime-0.0.6.dev20240212035011/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 03:50:35.022728 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 03:50:35.026728 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-02-12 03:50:25.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-02-12 03:50:25.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-12 03:50:06.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_axle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-12 03:50:06.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-02-12 03:50:06.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_symlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-02-12 03:50:06.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-12 03:50:06.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 03:50:35.026728 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-02-12 03:50:34.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-12 03:50:35.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 03:50:34.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 03:50:34.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 03:50:34.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-12 03:50:34.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 03:50:34.000000 wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:59:08.166014 wheel_axle_runtime-0.0.6.dev20240603035837/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-06-03 03:58:54.000000 wheel_axle_runtime-0.0.6.dev20240603035837/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-06-03 03:59:08.166014 wheel_axle_runtime-0.0.6.dev20240603035837/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 03:59:08.166014 wheel_axle_runtime-0.0.6.dev20240603035837/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8876 2024-06-03 03:58:54.000000 wheel_axle_runtime-0.0.6.dev20240603035837/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:59:08.162014 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:59:08.166014 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-06-03 03:58:54.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-06-03 03:58:54.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-06-03 03:58:31.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_axle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-06-03 03:58:31.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-06-03 03:58:31.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_symlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-06-03 03:58:31.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-06-03 03:58:31.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 03:59:08.166014 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-06-03 03:59:08.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-03 03:59:08.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:59:08.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:59:08.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 03:59:08.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 03:59:08.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 03:59:08.000000 wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/zip-safe
```

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/PKG-INFO` & `wheel_axle_runtime-0.0.6.dev20240603035837/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheel-axle-runtime
-Version: 0.0.6.dev20240212035011
+Version: 0.0.6.dev20240603035837
 Summary: Axle Runtime is the runtime part of the Python Wheel enhancement library
 Home-page: https://github.com/karellen/wheel-axle-runtime
 Author: Karellen, Inc.
 Author-email: supervisor@karellen.co
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@karellen.co
 License: Apache License, Version 2.0
```

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/setup.py` & `wheel_axle_runtime-0.0.6.dev20240603035837/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'wheel-axle-runtime',
-        version = '0.0.6.dev20240212035011',
+        version = '0.0.6.dev20240603035837',
         description = 'Axle Runtime is the runtime part of the Python Wheel enhancement library',
         long_description = '# Axle-Runtime - Python Wheel enhancement library\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/Lobby?logo=gitter)](https://app.gitter.im/#/room/#karellen_Lobby:gitter.im)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/wheel-axle-runtime/build.yml?branch=master)](https://github.com/karellen/wheel-axle-runtime/actions/workflows/build.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/wheel-axle-runtime/master?logo=coveralls)](https://coveralls.io/r/karellen/wheel-axle-runtime?branch=master)\n\n[![Wheel Axle Runtime Version](https://img.shields.io/pypi/v/wheel-axle-runtime?logo=pypi)](https://pypi.org/project/wheel-axle-runtime/)\n[![Wheel Axle Runtime Python Versions](https://img.shields.io/pypi/pyversions/wheel-axle-runtime?logo=pypi)](https://pypi.org/project/wheel-axle-runtime/)\n\n[![Wheel Axle Runtime Downloads Per Day](https://img.shields.io/pypi/dd/wheel-axle-runtime?logo=pypi)](https://pypistats.org/packages/wheel-axle-runtime)\n[![Wheel Axle Runtime Downloads Per Week](https://img.shields.io/pypi/dw/wheel-axle-runtime?logo=pypi)](https://pypistats.org/packages/wheel-axle-runtime)\n[![Wheel Axle Runtime Downloads Per Month](https://img.shields.io/pypi/dm/wheel-axle-runtime?logo=pypi)](https://pypistats.org/packages/wheel-axle-runtime)\n\n# This is a companion project to [Wheel Axle/bdist_axle](https://github.com/karellen/wheel-axle)\n\n## Problem\n\n1. Python wheels do not support symlinks.\n2. PIP installation procedure is not locally extensible and does not allow adding post-install hooks.\n\n## Solution\n\n**WARNING: THIS IS EXPERIMENTAL BETA SOFTWARE. THERE ARE NO WARRANTIES OF ANY KIND. USE AT YOUR OWN RISK. ADDITIONAL\nINCLUDED DISCLAIMERS ALSO APPLY.**\n\nWheel Axle Runtime library utilizes a little-known trick used in `site.py`\'s `.pth` files that allows executing\narbitrary code while the site packages are being added. Thus, specially-crafted wheels can silently execute installed\ncode on Python interpreter startup, facilitating the "post-install hook" functionality.\n\n### Python Invariants\n\nThe core functionality relies on the following Python behaviors:\n\n* `site.py` [processes .pth files](https://github.com/python/cpython/blob/8b1b27f1939cc4060531d198fdb09242f247ca7c/Lib/site.py#L171)\n* `site.py` [executes .pth import lines](https://github.com/python/cpython/blob/8b1b27f1939cc4060531d198fdb09242f247ca7c/Lib/site.py#L186)\n* `.pth` file\'s line is executed with a local\n  variable [`fullname` denoting the `.pth` file path](https://github.com/python/cpython/blob/8b1b27f1939cc4060531d198fdb09242f247ca7c/Lib/site.py#L170)\n\nThese invariants have not changed for *18 years*.\n\n### Implementation\n\nOnce the distribution-specific `.pth` is executed by the Python interpreter, the Wheel Axle Runtime behaves as follows:\n\n1. The library checks whether a file `.dist-info/axle.done` exists. If it does it is the indication that the\n   post-install hook has executed successfully and nothing more is to be done, terminating all further processing.\n2. A process-wide *inter-thread* lock is acquired.\n3. An OS-wide *inter-process file* lock is acquired on a file `.dist-info/axle.lck`.\n4. Once the locks are acquired the `.dist-info/axle.done` existence is rechecked (double-checked locking optimization).\n5. Now that in-process and inter-process race conditions are excluded the post-install work can begin.\n6. Registered `installers` are run in sequence. Installers *should be* idempotent. The following installers are\n   currently implemented:\n    1. *Symlinks installer* processes `.dist-info/symlinks.txt`, if any.\n        1. Based on the location of the `.pth` file being executed the current installation `schema` and its paths are\n           determined. Currently, installation into a virtual environment or user location is supported and tested.\n        2. For each symlink the target path is resolved and `realpath` is used to determine the final target path.\n        3. If the symlink path and symlink target path are within one of the permitted schema locations the symlink is\n           created. Otherwise, an exception is raised and the processing is aborted.\n        4. After all symlinks are created, the `.dist-info/RECORD` file is updated to reflect the created symlinks.\n    2. *Axle installer* finalizes the installation. This installer is always executed last.\n        1. The `.dist-info/RECORD` is updated with `.dist-info/axle.done` file record.\n        2. `.dist-info/axle.done` is created.\n        3. `<distribution name and version>.pth` is then removed. If the file cannot be removed it is left in place.\n           This can happen on Windows, since the `.pth` file in question is likely opened for exclusive reading on\n           Windows.\n7. Any failure anywhere in the above process will result in an abort, an error message, and a retry the next time\n   the `.pth` will be activated.\n\n### Security\n\nThere are several security requirements and implications of having post-install hooks implemented this way.\n\n1. The installation requires write permissions to the distribution. This will be a problem if the package is installed\n   as `root` in locations such as `/usr` or `/usr/local`, or is otherwise not write-permitted, unless the post-install\n   hook is also ran with the sufficient privileges. This is generally acceptable as the primary use is considered to be\n   installation into virtual envs and user locations. That said, simply running `python -c pass` or any other python\n   invocation that does activate `site.py` under the required privileges will finalize post-install procedures.\n2. There is *an attempt* to ensure that that axle wheels symlinks and targets don\'t extend beyond the allowed `schema`\n   locations. *Those attempts are **superficial** and **have not been formally verified**.* For example, it may be\n   possible to escape the path validation/confinement by:\n    * hacking symlink creation order\n    * hacking symlink directory targets\n    * exploiting OS-specific `realpath` implementation idiosyncrasies (i.e. `strict` vs not, and what is considered\n      strict)\n\n### TODOs\n\n* Support schema detection for `prefix` installations.\n* Validate and verify Windows support.\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
```

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/LICENSE` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/LICENSE`

 * *Files identical despite different names*

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/__init__.py` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import sys
 import site
 from os.path import exists, join as jp, commonpath
 from threading import RLock
 
 from wheel_axle.runtime.constants import AXLE_DONE_FILE, AXLE_LOCK_FILE
 
-__version__ = "0.0.6.dev20240212035011"
+__version__ = "0.0.6.dev20240603035837"
 
 _DIST_INFO = "dist-info"
 
 inter_thread_lock = RLock()
 
 
 def _run_installers(dist_info_dir):
```

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_axle.py` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_axle.py`

 * *Files identical despite different names*

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_common.py` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_common.py`

 * *Files identical despite different names*

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_symlinks.py` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_symlinks.py`

 * *Files identical despite different names*

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/_wheel.py` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/_wheel.py`

 * *Files identical despite different names*

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle/runtime/constants.py` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle/runtime/constants.py`

 * *Files identical despite different names*

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/PKG-INFO` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheel-axle-runtime
-Version: 0.0.6.dev20240212035011
+Version: 0.0.6.dev20240603035837
 Summary: Axle Runtime is the runtime part of the Python Wheel enhancement library
 Home-page: https://github.com/karellen/wheel-axle-runtime
 Author: Karellen, Inc.
 Author-email: supervisor@karellen.co
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@karellen.co
 License: Apache License, Version 2.0
```

### Comparing `wheel-axle-runtime-0.0.6.dev20240212035011/wheel_axle_runtime.egg-info/SOURCES.txt` & `wheel_axle_runtime-0.0.6.dev20240603035837/wheel_axle_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

