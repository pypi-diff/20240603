# Comparing `tmp/venv-modulefile-0.1.6.tar.gz` & `tmp/venv-modulefile-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmp4eio51fa/venv-modulefile-0.1.6.tar", last modified: Mon Jun  3 08:45:57 2024, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmprfkug20v/venv-modulefile-0.1.7.tar", last modified: Mon Jun  3 09:02:20 2024, max compression
```

## Comparing `venv-modulefile-0.1.6.tar` & `venv-modulefile-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9786 2024-04-16 09:35:06.000000 venv-modulefile-0.1.6/setup.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/LICENSE.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      193 2024-04-16 09:01:17.000000 venv-modulefile-0.1.6/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/PKG-INFO
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2024-04-16 10:01:25.000000 venv-modulefile-0.1.6/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4919 2024-04-16 11:07:04.000000 venv-modulefile-0.1.6/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10466 2024-06-03 08:45:40.000000 venv-modulefile-0.1.6/src/venvmod/modulefile.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2231175 2024-02-20 12:00:21.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2135014 2023-06-27 18:51:07.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2021637 2022-11-08 06:06:08.000000 venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2024-06-03 08:44:21.000000 venv-modulefile-0.1.6/src/venvmod/VERSION
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      714 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2024-06-03 08:45:57.000000 venv-modulefile-0.1.6/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-12-08 12:27:33.000000 venv-modulefile-0.1.6/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9786 2024-04-16 09:35:06.000000 venv-modulefile-0.1.7/setup.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/LICENSE.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      193 2024-04-16 09:01:17.000000 venv-modulefile-0.1.7/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/PKG-INFO
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2024-04-16 10:01:25.000000 venv-modulefile-0.1.7/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4972 2024-06-03 08:51:41.000000 venv-modulefile-0.1.7/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10467 2024-06-03 08:49:15.000000 venv-modulefile-0.1.7/src/venvmod/modulefile.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venvmod/modulefiles_src/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2231175 2024-02-20 12:00:21.000000 venv-modulefile-0.1.7/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2135014 2023-06-27 18:51:07.000000 venv-modulefile-0.1.7/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)  2021637 2022-11-08 06:06:08.000000 venv-modulefile-0.1.7/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2024-06-03 09:01:08.000000 venv-modulefile-0.1.7/src/venvmod/VERSION
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      714 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2024-06-03 09:02:20.000000 venv-modulefile-0.1.7/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-12-08 12:27:33.000000 venv-modulefile-0.1.7/src/README.md
```

### Comparing `venv-modulefile-0.1.6/setup.py` & `venv-modulefile-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/LICENSE.md` & `venv-modulefile-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/README.md` & `venv-modulefile-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/PKG-INFO` & `venv-modulefile-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/code-coupling/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/code-coupling/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.1.6/src/venvmod/tools.py` & `venv-modulefile-0.1.7/src/venvmod/tools.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venvmod/commands/__init__.py` & `venv-modulefile-0.1.7/src/venvmod/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venvmod/commands/create_module.py` & `venv-modulefile-0.1.7/src/venvmod/commands/create_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,27 +84,28 @@
         If None, arguments are read from :func:`venvmod.commands.get_parser` function,
         else the path to the virtual env, by default None
     applis : List[str], optional
         List of module file to create in addition to those given through cli, by default None
     read_env : bool, optional
         Read environment variables associated to the appli, by default False
     """
-
     if virtual_env is None:
         options = get_parser(description="Initialize Modulefile for an application.",
                              positionals=[("APPLI", [],
                                           "Appli name(s) to add to the environment.", '+')],
                              with_appli=False,
                              options=[
                                  ("read-env", False,
                                   "Read environment variables. 'See cmd-read-env'")
                              ])
         virtual_env = Path(options.virtual_env).absolute()
         virtual_env_name = get_std_name(virtual_env.name)
         read_env = options.read_env
+    else:
+        virtual_env_name = virtual_env.name
 
     fails = []
     for appli in remove_duplicates(options.APPLI + (applis if applis else [])):
         appli_name = get_std_name(appli)
         module_name = f"{virtual_env_name}-{appli_name}"
         if create_modulefile(virtual_env=virtual_env,
                              module_name=module_name,
```

### Comparing `venv-modulefile-0.1.6/src/venvmod/commands/test_imports.py` & `venv-modulefile-0.1.7/src/venvmod/commands/test_imports.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venvmod/commands/append_module.py` & `venv-modulefile-0.1.7/src/venvmod/commands/append_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venvmod/modulefile.py` & `venv-modulefile-0.1.7/src/venvmod/modulefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     virtual_env : Path
         Path to virtual env
     """
     with (virtual_env / "bin" / "activate").open(mode="r", encoding='utf-8') as src_file:
         check_raise(ACTIVATE_HEADER_LINE in src_file.read(), AssertionError,
                     f"{virtual_env} is already a venv-modulefile environment.")
 
+
 class ModuleInstaller:  # pylint: disable=too-few-public-methods
     """Class to install Environment Module.
     """
 
     def __init__(self,
                  version_or_path: str,
                  install_prefix: str or Path,
```

### Comparing `venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz` & `venv-modulefile-0.1.7/src/venvmod/modulefiles_src/modules-5.4.0.tar.gz`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz` & `venv-modulefile-0.1.7/src/venvmod/modulefiles_src/modules-5.3.1.tar.gz`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz` & `venv-modulefile-0.1.7/src/venvmod/modulefiles_src/modules-5.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.1.7/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/venv_modulefile.egg-info/PKG-INFO` & `venv-modulefile-0.1.7/src/venv_modulefile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/code-coupling/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/code-coupling/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.1.6/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.1.7/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.6/src/README.md` & `venv-modulefile-0.1.7/src/README.md`

 * *Files identical despite different names*

