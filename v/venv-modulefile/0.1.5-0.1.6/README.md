# Comparing `tmp/venv-modulefile-0.1.5.tar.gz` & `tmp/venv-modulefile-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmp00a4m8hm/venv-modulefile-0.1.5.tar", last modified: Tue Apr 16 10:40:54 2024, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmp4eio51fa/venv-modulefile-0.1.6.tar", last modified: Mon Jun  3 08:45:57 2024, max compression
```

## Comparing `venv-modulefile-0.1.5.tar` & `venv-modulefile-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9786 2024-04-16 09:35:06.000000 venv-modulefile-0.1.5/setup.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/LICENSE.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      193 2024-04-16 09:01:17.000000 venv-modulefile-0.1.5/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/PKG-INFO
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2024-04-16 10:01:25.000000 venv-modulefile-0.1.5/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5049 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11302 2024-04-16 10:22:44.000000 venv-modulefile-0.1.5/src/venvmod/modulefile.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2231175 2024-02-20 12:00:21.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2135014 2023-06-27 18:51:07.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2021637 2022-11-08 06:06:08.000000 venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2024-04-16 10:28:29.000000 venv-modulefile-0.1.5/src/venvmod/VERSION
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      714 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2024-04-16 10:40:54.000000 venv-modulefile-0.1.5/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-12-08 12:27:33.000000 venv-modulefile-0.1.5/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9786 2024-04-16 09:35:06.000000 venv-modulefile-0.1.6/setup.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/LICENSE.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      193 2024-04-16 09:01:17.000000 venv-modulefile-0.1.6/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/PKG-INFO
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2024-04-16 10:01:25.000000 venv-modulefile-0.1.6/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4919 2024-04-16 11:07:04.000000 venv-modulefile-0.1.6/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10466 2024-06-03 08:45:40.000000 venv-modulefile-0.1.6/src/venvmod/modulefile.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2231175 2024-02-20 12:00:21.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2135014 2023-06-27 18:51:07.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2021637 2022-11-08 06:06:08.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2024-06-03 08:44:21.000000 venv-modulefile-0.1.6/src/venvmod/VERSION
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      714 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/README.md
```

### Comparing `venv-modulefile-0.1.5/setup.py` & `venv-modulefile-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/LICENSE.md` & `venv-modulefile-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/README.md` & `venv-modulefile-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/PKG-INFO` & `venv-modulefile-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/code-coupling/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/code-coupling/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.1.5/src/venvmod/tools.py` & `venv-modulefile-0.1.6/src/venvmod/tools.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venvmod/commands/__init__.py` & `venv-modulefile-0.1.6/src/venvmod/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venvmod/commands/create_module.py` & `venv-modulefile-0.1.6/src/venvmod/commands/create_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Commands to create a modulefile."""
 
 from pathlib import Path
 from typing import List
 
-from packaging import version
-
 from ..tools import get_std_name
 from . import get_parser
 from .append_module import module_load, read_env as read_env_vars
-from ..modulefile import (get_version, ModuleInstaller, upgrade_modulefile, create_modulefile,
+from ..modulefile import (ModuleInstaller, upgrade_modulefile, create_modulefile,
                           upgrade_venv, test_if_already_init)
 
 from ..tools import PACKAGE_NAME, check_raise, remove_duplicates
 
 
 def initialize(virtual_env: Path = None,
                version_or_path: str = "5.2.0",
@@ -49,22 +47,20 @@
         virtual_env = Path(options.virtual_env).absolute()
         if options.modulefile_version:
             version_or_path = options.modulefile_version
         read_env = options.read_env
 
     test_if_already_init(virtual_env=virtual_env)
 
-    if version.parse(get_version()) < version.parse("14.6"):
-
-        install_prefix = virtual_env / "opt" / "modulefiles"
-        if not (install_prefix / "init").exists():
-            ModuleInstaller(install_prefix=install_prefix,
-                            version_or_path=version_or_path,
-                            cache_directory=virtual_env / ".cache").run(
-                                verbose=options.verbose)
+    install_prefix = virtual_env / "opt" / "modulefiles"
+    if not (install_prefix / "init").exists():
+        ModuleInstaller(install_prefix=install_prefix,
+                        version_or_path=version_or_path,
+                        cache_directory=virtual_env / ".cache").run(
+                            verbose=options.verbose)
 
         upgrade_modulefile(virtual_env=virtual_env, module_prefix=install_prefix)
 
     create_modulefile(virtual_env=virtual_env,
                       module_name=get_std_name(virtual_env.name),
                       module_category=PACKAGE_NAME,
                       log_load=options.activate_log)
```

### Comparing `venv-modulefile-0.1.5/src/venvmod/commands/test_imports.py` & `venv-modulefile-0.1.6/src/venvmod/commands/test_imports.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venvmod/commands/append_module.py` & `venv-modulefile-0.1.6/src/venvmod/commands/append_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venvmod/modulefile.py` & `venv-modulefile-0.1.6/src/venvmod/modulefile.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import subprocess
 import tarfile
 
 from packaging import version
 import requests
 
 from venvmod.tools import (get_std_name, get_shell_command, check_raise,
-                           get_shell_name, PACKAGE_NAME, logger)
+                           get_shell_name, PACKAGE_NAME)
 
 
 def get_module_file_directory(virtual_env: Path) -> Path:
     """Gets the modulefiles directory
 
     Parameters
     ----------
@@ -43,38 +43,14 @@
     virtual_env : Path
         Path to virtual env
     """
     with (virtual_env / "bin" / "activate").open(mode="r", encoding='utf-8') as src_file:
         check_raise(ACTIVATE_HEADER_LINE in src_file.read(), AssertionError,
                     f"{virtual_env} is already a venv-modulefile environment.")
 
-
-def get_version() -> str:
-    """Gets modulefile version
-
-    Returns
-    -------
-    str
-        version as 'x.y.z', '0.0.0' if not found
-    """
-    try:
-        result = subprocess.run([get_shell_command(), '-c', "module --version"],
-                                stderr=subprocess.PIPE, stdout=subprocess.PIPE, check=False)
-
-        logger.debug(
-            "get_version: %s\n%s\n%s", result, result.stderr.decode(), result.stdout.decode())
-        if result.returncode == 0:
-            if 'VERSION=' in result.stderr.decode().split()[0]:  # version < 4.0
-                return result.stderr.decode().split()[0].split("=")[1]
-            if 'Modules' == result.stderr.decode().split()[0]:
-                return result.stderr.decode().split()[2]
-    finally:
-        return "0.0.0"  # pylint: disable=lost-exception
-
-
 class ModuleInstaller:  # pylint: disable=too-few-public-methods
     """Class to install Environment Module.
     """
 
     def __init__(self,
                  version_or_path: str,
                  install_prefix: str or Path,
```

### Comparing `venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz` & `venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz` & `venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz` & `venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.1.6/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/venv_modulefile.egg-info/PKG-INFO` & `venv-modulefile-0.1.6/src/venv_modulefile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/code-coupling/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/code-coupling/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.1.5/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.1.6/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.5/src/README.md` & `venv-modulefile-0.1.6/src/README.md`

 * *Files identical despite different names*

