# Comparing `tmp/repopulator-0.2.tar.gz` & `tmp/repopulator-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repopulator-0.2.tar", last modified: Sun Jun  2 01:59:20 2024, max compression
+gzip compressed data, was "repopulator-0.3.tar", last modified: Mon Jun  3 06:46:06 2024, max compression
```

## Comparing `repopulator-0.2.tar` & `repopulator-0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-02 01:59:20.477644 repopulator-0.2/
--rw-r--r--   0 eugene     (501) wheel        (0)      291 2024-06-02 01:56:24.000000 repopulator-0.2/CHANGELOG.md
--rw-r--r--   0 eugene     (501) wheel        (0)     1493 2024-05-24 20:01:21.000000 repopulator-0.2/LICENSE.txt
--rw-r--r--   0 eugene     (501) wheel        (0)       39 2024-05-28 02:10:17.000000 repopulator-0.2/MANIFEST.in
--rw-r--r--   0 eugene     (501) wheel        (0)     5299 2024-06-02 01:59:20.477139 repopulator-0.2/PKG-INFO
--rw-r--r--   0 eugene     (501) wheel        (0)     3989 2024-06-01 18:00:52.000000 repopulator-0.2/README.md
--rw-r--r--   0 eugene     (501) wheel        (0)     1481 2024-06-01 18:11:45.000000 repopulator-0.2/pyproject.toml
--rw-r--r--   0 eugene     (501) wheel        (0)       38 2024-06-02 01:59:20.477741 repopulator-0.2/setup.cfg
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-02 01:59:20.459023 repopulator-0.2/src/
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-02 01:59:20.471010 repopulator-0.2/src/repopulator/
--rw-r--r--   0 eugene     (501) wheel        (0)      779 2024-05-31 17:58:46.000000 repopulator-0.2/src/repopulator/__init__.py
--rw-r--r--   0 eugene     (501) wheel        (0)    13399 2024-06-01 03:40:40.000000 repopulator-0.2/src/repopulator/apt.py
--rw-r--r--   0 eugene     (501) wheel        (0)     6941 2024-05-31 23:29:53.000000 repopulator-0.2/src/repopulator/freebsd.py
--rw-r--r--   0 eugene     (501) wheel        (0)     1490 2024-05-29 15:17:57.000000 repopulator-0.2/src/repopulator/pgp_signer.py
--rw-r--r--   0 eugene     (501) wheel        (0)     2384 2024-05-31 18:59:26.000000 repopulator-0.2/src/repopulator/pki_signer.py
--rw-r--r--   0 eugene     (501) wheel        (0)        0 2024-05-20 06:02:57.000000 repopulator-0.2/src/repopulator/py.typed
--rw-r--r--   0 eugene     (501) wheel        (0)    24781 2024-06-01 03:40:40.000000 repopulator-0.2/src/repopulator/rpm.py
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-02 01:59:20.475798 repopulator-0.2/src/repopulator/rpmfile/
--rw-r--r--   0 eugene     (501) wheel        (0)     7157 2024-05-30 17:16:52.000000 repopulator-0.2/src/repopulator/rpmfile/__init__.py
--rw-r--r--   0 eugene     (501) wheel        (0)       85 2024-05-26 03:17:39.000000 repopulator-0.2/src/repopulator/rpmfile/errors.py
--rw-r--r--   0 eugene     (501) wheel        (0)    12252 2024-05-26 03:30:34.000000 repopulator-0.2/src/repopulator/rpmfile/headers.py
--rw-r--r--   0 eugene     (501) wheel        (0)     2303 2024-05-28 17:12:10.000000 repopulator-0.2/src/repopulator/rpmfile/io_extra.py
--rw-r--r--   0 eugene     (501) wheel        (0)     8689 2024-05-31 23:30:34.000000 repopulator-0.2/src/repopulator/util.py
--rw-r--r--   0 eugene     (501) wheel        (0)      252 2024-06-02 01:56:24.000000 repopulator-0.2/src/repopulator/version.py
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-02 01:59:20.476480 repopulator-0.2/src/repopulator.egg-info/
--rw-r--r--   0 eugene     (501) wheel        (0)     5299 2024-06-02 01:59:20.000000 repopulator-0.2/src/repopulator.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) wheel        (0)      633 2024-06-02 01:59:20.000000 repopulator-0.2/src/repopulator.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) wheel        (0)        1 2024-06-02 01:59:20.000000 repopulator-0.2/src/repopulator.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) wheel        (0)       33 2024-06-02 01:59:20.000000 repopulator-0.2/src/repopulator.egg-info/requires.txt
--rw-r--r--   0 eugene     (501) wheel        (0)       12 2024-06-02 01:59:20.000000 repopulator-0.2/src/repopulator.egg-info/top_level.txt
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-03 06:46:06.800077 repopulator-0.3/
+-rw-r--r--   0 eugene     (501) wheel        (0)      425 2024-06-03 06:45:57.000000 repopulator-0.3/CHANGELOG.md
+-rw-r--r--   0 eugene     (501) wheel        (0)     1493 2024-05-24 20:01:21.000000 repopulator-0.3/LICENSE.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)       39 2024-05-28 02:10:17.000000 repopulator-0.3/MANIFEST.in
+-rw-r--r--   0 eugene     (501) wheel        (0)     6022 2024-06-03 06:46:06.799625 repopulator-0.3/PKG-INFO
+-rw-r--r--   0 eugene     (501) wheel        (0)     4569 2024-06-03 06:36:07.000000 repopulator-0.3/README.md
+-rw-r--r--   0 eugene     (501) wheel        (0)     1649 2024-06-03 06:36:07.000000 repopulator-0.3/pyproject.toml
+-rw-r--r--   0 eugene     (501) wheel        (0)       38 2024-06-03 06:46:06.800178 repopulator-0.3/setup.cfg
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-03 06:46:06.786277 repopulator-0.3/src/
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-03 06:46:06.794017 repopulator-0.3/src/repopulator/
+-rw-r--r--   0 eugene     (501) wheel        (0)      864 2024-06-03 06:36:07.000000 repopulator-0.3/src/repopulator/__init__.py
+-rw-r--r--   0 eugene     (501) wheel        (0)    13399 2024-06-01 03:40:40.000000 repopulator-0.3/src/repopulator/apt.py
+-rw-r--r--   0 eugene     (501) wheel        (0)     6941 2024-06-02 18:14:25.000000 repopulator-0.3/src/repopulator/freebsd.py
+-rw-r--r--   0 eugene     (501) wheel        (0)    11341 2024-06-03 06:36:07.000000 repopulator-0.3/src/repopulator/pacman.py
+-rw-r--r--   0 eugene     (501) wheel        (0)     2044 2024-06-03 06:36:07.000000 repopulator-0.3/src/repopulator/pgp_signer.py
+-rw-r--r--   0 eugene     (501) wheel        (0)     2384 2024-05-31 18:59:26.000000 repopulator-0.3/src/repopulator/pki_signer.py
+-rw-r--r--   0 eugene     (501) wheel        (0)        0 2024-05-20 06:02:57.000000 repopulator-0.3/src/repopulator/py.typed
+-rw-r--r--   0 eugene     (501) wheel        (0)    24781 2024-06-01 03:40:40.000000 repopulator-0.3/src/repopulator/rpm.py
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-03 06:46:06.798654 repopulator-0.3/src/repopulator/rpmfile/
+-rw-r--r--   0 eugene     (501) wheel        (0)     7157 2024-05-30 17:16:52.000000 repopulator-0.3/src/repopulator/rpmfile/__init__.py
+-rw-r--r--   0 eugene     (501) wheel        (0)       85 2024-05-26 03:17:39.000000 repopulator-0.3/src/repopulator/rpmfile/errors.py
+-rw-r--r--   0 eugene     (501) wheel        (0)    12252 2024-05-26 03:30:34.000000 repopulator-0.3/src/repopulator/rpmfile/headers.py
+-rw-r--r--   0 eugene     (501) wheel        (0)     2303 2024-05-28 17:12:10.000000 repopulator-0.3/src/repopulator/rpmfile/io_extra.py
+-rw-r--r--   0 eugene     (501) wheel        (0)     8689 2024-05-31 23:30:34.000000 repopulator-0.3/src/repopulator/util.py
+-rw-r--r--   0 eugene     (501) wheel        (0)      252 2024-06-03 06:45:57.000000 repopulator-0.3/src/repopulator/version.py
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-06-03 06:46:06.799107 repopulator-0.3/src/repopulator.egg-info/
+-rw-r--r--   0 eugene     (501) wheel        (0)     6022 2024-06-03 06:46:06.000000 repopulator-0.3/src/repopulator.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) wheel        (0)      659 2024-06-03 06:46:06.000000 repopulator-0.3/src/repopulator.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)        1 2024-06-03 06:46:06.000000 repopulator-0.3/src/repopulator.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)       57 2024-06-03 06:46:06.000000 repopulator-0.3/src/repopulator.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)       12 2024-06-03 06:46:06.000000 repopulator-0.3/src/repopulator.egg-info/top_level.txt
```

### Comparing `repopulator-0.2/LICENSE.txt` & `repopulator-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/PKG-INFO` & `repopulator-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: repopulator
-Version: 0.2
+Version: 0.3
 Summary: Portably create software repositories for different operating systems
 Author-email: Eugene Gershnik <gershnik@hotmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/gershnik/repopulator
-Keywords: apt,rpm
+Keywords: cross-platform,apt-repository,yum-repositories,freebsd-packages,rpm-repositories,apt-repo,yum-repos,pacman-repo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System
@@ -26,24 +26,26 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: arpy==2.3.0
 Requires-Dist: cryptography==42.0.7
+Requires-Dist: zstandard[cffi]==0.22.0
 
 
 
 # repolulator
 
 [![License](https://img.shields.io/badge/license-BSD-brightgreen.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org)
 [![python](https://img.shields.io/badge/python->=3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![pypi](https://img.shields.io/pypi/v/repopulator)](https://pypi.org/project/repopulator)
 
-A portable Python library to generate binary software repositories (APT, YUM/DNF etc.) 
+A portable Python library to generate binary software repositories (APT, YUM/DNF, Pacman etc.) 
 
 ## Purpose
 
 Ever needed to build an APT package repository on Fedora? Or perhaps a DNF repository on Debian? How about FreeBSD repository on Windows or Mac? This library allows you to do all these things and more. And yes, you can do it even on Windows if you are so inclined for some reason.
 
 All binary package repositories have their own tools that usually range from being "non-portable" to "portable with lots of effort to limited platforms only". On the other hand it is often convenient to build software packages in a Map/Reduce fashion where a single host collects multiple packages built for different platforms to produce binary repositories. Such host will necessarily need to be able to build repositories for "foreign" packages. This library is an attempt to enable such scenario.
 
@@ -52,14 +54,15 @@
 * Python >= 3.8
 * If you plan to build repositories that require GPG signing `gpg` command needs to be available in PATH
 
 ## Supported repository formats
 
 * APT
 * RPM
+* Pacman
 * FreeBSD pkg
 
 ## Installing
 
 ```bash
 pip install repopulator
 ```
@@ -115,14 +118,31 @@
 
 signer = PgpSigner(Path.home() / '.gnupg', 'name_of_key_to_use', 'password_of_that_key')
 
 repo.export(Path('/path/of/new/repo'), signer)
 
 ```
 
+#### Pacman
+
+```python
+from repopulator import PacmanRepo, PgpSigner
+from pathlib import Path
+
+repo = PacmanRepo('myrepo')
+# if .sig file is present next to the .zst file it will be used for signature
+# otherwise new signature will be generated at export time
+repo.addPackage(Path('/path/to/awesome-3.14-1-x86_64.pkg.tar.zst'))
+
+signer = PgpSigner(Path.home() / '.gnupg', 'name_of_key_to_use', 'password_of_that_key')
+
+repo.export(Path('/path/of/new/repo'), signer)
+
+```
+
 #### FreeBSD pkg
 
 ```python
 from repopulator import FreeBSDRepo, PkiSigner
 from pathlib import Path
 
 repo = FreeBSDRepo()
```

### Comparing `repopulator-0.2/README.md` & `repopulator-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 
 # repolulator
 
 [![License](https://img.shields.io/badge/license-BSD-brightgreen.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org)
 [![python](https://img.shields.io/badge/python->=3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![pypi](https://img.shields.io/pypi/v/repopulator)](https://pypi.org/project/repopulator)
 
-A portable Python library to generate binary software repositories (APT, YUM/DNF etc.) 
+A portable Python library to generate binary software repositories (APT, YUM/DNF, Pacman etc.) 
 
 ## Purpose
 
 Ever needed to build an APT package repository on Fedora? Or perhaps a DNF repository on Debian? How about FreeBSD repository on Windows or Mac? This library allows you to do all these things and more. And yes, you can do it even on Windows if you are so inclined for some reason.
 
 All binary package repositories have their own tools that usually range from being "non-portable" to "portable with lots of effort to limited platforms only". On the other hand it is often convenient to build software packages in a Map/Reduce fashion where a single host collects multiple packages built for different platforms to produce binary repositories. Such host will necessarily need to be able to build repositories for "foreign" packages. This library is an attempt to enable such scenario.
 
@@ -19,14 +20,15 @@
 * Python >= 3.8
 * If you plan to build repositories that require GPG signing `gpg` command needs to be available in PATH
 
 ## Supported repository formats
 
 * APT
 * RPM
+* Pacman
 * FreeBSD pkg
 
 ## Installing
 
 ```bash
 pip install repopulator
 ```
@@ -82,14 +84,31 @@
 
 signer = PgpSigner(Path.home() / '.gnupg', 'name_of_key_to_use', 'password_of_that_key')
 
 repo.export(Path('/path/of/new/repo'), signer)
 
 ```
 
+#### Pacman
+
+```python
+from repopulator import PacmanRepo, PgpSigner
+from pathlib import Path
+
+repo = PacmanRepo('myrepo')
+# if .sig file is present next to the .zst file it will be used for signature
+# otherwise new signature will be generated at export time
+repo.addPackage(Path('/path/to/awesome-3.14-1-x86_64.pkg.tar.zst'))
+
+signer = PgpSigner(Path.home() / '.gnupg', 'name_of_key_to_use', 'password_of_that_key')
+
+repo.export(Path('/path/of/new/repo'), signer)
+
+```
+
 #### FreeBSD pkg
 
 ```python
 from repopulator import FreeBSDRepo, PkiSigner
 from pathlib import Path
 
 repo = FreeBSDRepo()
```

### Comparing `repopulator-0.2/pyproject.toml` & `repopulator-0.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -17,17 +17,22 @@
 readme="README.md"
 authors= [
     { name = 'Eugene Gershnik', email='gershnik@hotmail.com'}
 ]
 requires-python = ">=3.8"
 dependencies = [
     "arpy==2.3.0",
-    "cryptography==42.0.7"
+    "cryptography==42.0.7",
+    "zstandard[cffi]==0.22.0"
+]
+keywords = [
+    "cross-platform", "apt-repository", "yum-repositories", 
+    "freebsd-packages", "rpm-repositories", "apt-repo", "yum-repos",
+    "pacman-repo"
 ]
-keywords = ["apt", "rpm"]
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     
     "License :: OSI Approved :: BSD License",
     
     "Operating System :: OS Independent",
```

### Comparing `repopulator-0.2/src/repopulator/__init__.py` & `repopulator-0.3/src/repopulator/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 from .pki_signer import PkiSigner
 
 from .util import VersionKey
 
 from .apt import AptPackage, AptDistribution, AptRepo
 from .rpm import RpmPackage, RpmRepo, RpmVersion
 from .freebsd import FreeBSDPackage, FreeBSDRepo
+from .pacman import PacmanPackage, PacmanRepo
 
 __all__ = [
     'PgpSigner', 
     'PkiSigner', 
     'VersionKey',
     'AptPackage', 
     'AptDistribution', 
     'AptRepo',
     'RpmPackage',
     'RpmRepo',
     'RpmVersion',
     'FreeBSDPackage',
-    'FreeBSDRepo'
+    'FreeBSDRepo',
+    'PacmanPackage',
+    'PacmanRepo'
 ]
```

### Comparing `repopulator-0.2/src/repopulator/apt.py` & `repopulator-0.3/src/repopulator/apt.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator/freebsd.py` & `repopulator-0.3/src/repopulator/freebsd.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator/pki_signer.py` & `repopulator-0.3/src/repopulator/pki_signer.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator/rpm.py` & `repopulator-0.3/src/repopulator/rpm.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator/rpmfile/__init__.py` & `repopulator-0.3/src/repopulator/rpmfile/__init__.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator/rpmfile/headers.py` & `repopulator-0.3/src/repopulator/rpmfile/headers.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator/rpmfile/io_extra.py` & `repopulator-0.3/src/repopulator/rpmfile/io_extra.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator/util.py` & `repopulator-0.3/src/repopulator/util.py`

 * *Files identical despite different names*

### Comparing `repopulator-0.2/src/repopulator.egg-info/PKG-INFO` & `repopulator-0.3/src/repopulator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: repopulator
-Version: 0.2
+Version: 0.3
 Summary: Portably create software repositories for different operating systems
 Author-email: Eugene Gershnik <gershnik@hotmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/gershnik/repopulator
-Keywords: apt,rpm
+Keywords: cross-platform,apt-repository,yum-repositories,freebsd-packages,rpm-repositories,apt-repo,yum-repos,pacman-repo
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: System
@@ -26,24 +26,26 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: arpy==2.3.0
 Requires-Dist: cryptography==42.0.7
+Requires-Dist: zstandard[cffi]==0.22.0
 
 
 
 # repolulator
 
 [![License](https://img.shields.io/badge/license-BSD-brightgreen.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org)
 [![python](https://img.shields.io/badge/python->=3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![pypi](https://img.shields.io/pypi/v/repopulator)](https://pypi.org/project/repopulator)
 
-A portable Python library to generate binary software repositories (APT, YUM/DNF etc.) 
+A portable Python library to generate binary software repositories (APT, YUM/DNF, Pacman etc.) 
 
 ## Purpose
 
 Ever needed to build an APT package repository on Fedora? Or perhaps a DNF repository on Debian? How about FreeBSD repository on Windows or Mac? This library allows you to do all these things and more. And yes, you can do it even on Windows if you are so inclined for some reason.
 
 All binary package repositories have their own tools that usually range from being "non-portable" to "portable with lots of effort to limited platforms only". On the other hand it is often convenient to build software packages in a Map/Reduce fashion where a single host collects multiple packages built for different platforms to produce binary repositories. Such host will necessarily need to be able to build repositories for "foreign" packages. This library is an attempt to enable such scenario.
 
@@ -52,14 +54,15 @@
 * Python >= 3.8
 * If you plan to build repositories that require GPG signing `gpg` command needs to be available in PATH
 
 ## Supported repository formats
 
 * APT
 * RPM
+* Pacman
 * FreeBSD pkg
 
 ## Installing
 
 ```bash
 pip install repopulator
 ```
@@ -115,14 +118,31 @@
 
 signer = PgpSigner(Path.home() / '.gnupg', 'name_of_key_to_use', 'password_of_that_key')
 
 repo.export(Path('/path/of/new/repo'), signer)
 
 ```
 
+#### Pacman
+
+```python
+from repopulator import PacmanRepo, PgpSigner
+from pathlib import Path
+
+repo = PacmanRepo('myrepo')
+# if .sig file is present next to the .zst file it will be used for signature
+# otherwise new signature will be generated at export time
+repo.addPackage(Path('/path/to/awesome-3.14-1-x86_64.pkg.tar.zst'))
+
+signer = PgpSigner(Path.home() / '.gnupg', 'name_of_key_to_use', 'password_of_that_key')
+
+repo.export(Path('/path/of/new/repo'), signer)
+
+```
+
 #### FreeBSD pkg
 
 ```python
 from repopulator import FreeBSDRepo, PkiSigner
 from pathlib import Path
 
 repo = FreeBSDRepo()
```

### Comparing `repopulator-0.2/src/repopulator.egg-info/SOURCES.txt` & `repopulator-0.3/src/repopulator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 src/repopulator/__init__.py
 src/repopulator/apt.py
 src/repopulator/freebsd.py
+src/repopulator/pacman.py
 src/repopulator/pgp_signer.py
 src/repopulator/pki_signer.py
 src/repopulator/py.typed
 src/repopulator/rpm.py
 src/repopulator/util.py
 src/repopulator/version.py
 src/repopulator.egg-info/PKG-INFO
```

