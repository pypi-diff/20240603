# Comparing `tmp/pyproject-requirements-20240203.tar.gz` & `tmp/pyproject_requirements-20240601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-requirements-20240203.tar", last modified: Wed Feb 28 05:07:09 2024, max compression
+gzip compressed data, was "pyproject_requirements-20240601.tar", last modified: Mon Jun  3 13:23:34 2024, max compression
```

## Comparing `pyproject-requirements-20240203.tar` & `pyproject_requirements-20240601.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-28 05:07:09.172017 pyproject-requirements-20240203/
--rw-r--r--   0 nate      (1000) nate      (1000)     2938 2024-02-28 05:07:09.171017 pyproject-requirements-20240203/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)     2627 2024-02-28 05:07:05.000000 pyproject-requirements-20240203/README.md
--rw-rw-r--   0 nate      (1000) nate      (1000)      804 2024-02-28 05:07:05.000000 pyproject-requirements-20240203/pyproject.toml
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-28 05:07:09.169017 pyproject-requirements-20240203/python/
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-28 05:07:09.170017 pyproject-requirements-20240203/python/pip_requirements/
--rw-rw-r--   0 nate      (1000) nate      (1000)     6398 2024-02-28 05:07:05.000000 pyproject-requirements-20240203/python/pip_requirements/__main__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)       19 2024-02-28 05:07:05.000000 pyproject-requirements-20240203/python/pip_requirements/version.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-28 05:07:09.171017 pyproject-requirements-20240203/python/pyproject_requirements.egg-info/
--rw-r--r--   0 nate      (1000) nate      (1000)     2938 2024-02-28 05:07:08.000000 pyproject-requirements-20240203/python/pyproject_requirements.egg-info/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      415 2024-02-28 05:07:09.000000 pyproject-requirements-20240203/python/pyproject_requirements.egg-info/SOURCES.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-02-28 05:07:08.000000 pyproject-requirements-20240203/python/pyproject_requirements.egg-info/dependency_links.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       63 2024-02-28 05:07:08.000000 pyproject-requirements-20240203/python/pyproject_requirements.egg-info/entry_points.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        9 2024-02-28 05:07:08.000000 pyproject-requirements-20240203/python/pyproject_requirements.egg-info/requires.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       17 2024-02-28 05:07:08.000000 pyproject-requirements-20240203/python/pyproject_requirements.egg-info/top_level.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       38 2024-02-28 05:07:09.172017 pyproject-requirements-20240203/setup.cfg
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-03 13:23:34.437270 pyproject_requirements-20240601/
+-rw-r--r--   0 nate      (1000) nate      (1000)     2973 2024-06-03 13:23:34.437270 pyproject_requirements-20240601/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2662 2024-06-03 13:23:31.000000 pyproject_requirements-20240601/README.md
+-rw-r--r--   0 nate      (1000) nate      (1000)      809 2024-06-03 13:23:31.000000 pyproject_requirements-20240601/pyproject.toml
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-03 13:23:34.436270 pyproject_requirements-20240601/python/
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-03 13:23:34.436270 pyproject_requirements-20240601/python/pip_requirements/
+-rw-r--r--   0 nate      (1000) nate      (1000)     6524 2024-06-03 13:23:31.000000 pyproject_requirements-20240601/python/pip_requirements/__main__.py
+-rw-r--r--   0 nate      (1000) nate      (1000)       19 2024-06-03 13:23:31.000000 pyproject_requirements-20240601/python/pip_requirements/version.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-06-03 13:23:34.437270 pyproject_requirements-20240601/python/pyproject_requirements.egg-info/
+-rw-r--r--   0 nate      (1000) nate      (1000)     2973 2024-06-03 13:23:34.000000 pyproject_requirements-20240601/python/pyproject_requirements.egg-info/PKG-INFO
+-rw-r--r--   0 nate      (1000) nate      (1000)      415 2024-06-03 13:23:34.000000 pyproject_requirements-20240601/python/pyproject_requirements.egg-info/SOURCES.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)        1 2024-06-03 13:23:34.000000 pyproject_requirements-20240601/python/pyproject_requirements.egg-info/dependency_links.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       68 2024-06-03 13:23:34.000000 pyproject_requirements-20240601/python/pyproject_requirements.egg-info/entry_points.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)        9 2024-06-03 13:23:34.000000 pyproject_requirements-20240601/python/pyproject_requirements.egg-info/requires.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       17 2024-06-03 13:23:34.000000 pyproject_requirements-20240601/python/pyproject_requirements.egg-info/top_level.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       38 2024-06-03 13:23:34.437270 pyproject_requirements-20240601/setup.cfg
```

### Comparing `pyproject-requirements-20240203/PKG-INFO` & `pyproject_requirements-20240601/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: pyproject-requirements
-Version: 20240203
+Version: 20240601
 Summary: Install dependencies from a pyproject using pip.
 Author: MetaCompany, Nate Skulic
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pip
 Requires-Dist: toml
 
-# pip-requirements
+# pip-requirements (aka pyproject-requirements)
 
 Install requirements/dependencies specified in a pyproject.toml using pip.
 
 ## Features
 
 - Installs required, optional and/or all dependencies.
 - Detects and works with pip in installed in virtual environments.
 - Generates a requirements.txt file from a pyproject.toml (for tool compatibility).
 
 ## Quick Start
 
 1. Install pip-requirements:
 
    ```shell
-   pip install pip-requirements
+   pip install pyproject-requirements
    ```
 
 2. Install all dependencies of your pyproject.toml 
 
    ```shell
    # use `--optional name` to limit to optional named dependency section
    # use `--required` to install required dependencies
```

### Comparing `pyproject-requirements-20240203/README.md` & `pyproject_requirements-20240601/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# pip-requirements
+# pip-requirements (aka pyproject-requirements)
 
 Install requirements/dependencies specified in a pyproject.toml using pip.
 
 ## Features
 
 - Installs required, optional and/or all dependencies.
 - Detects and works with pip in installed in virtual environments.
 - Generates a requirements.txt file from a pyproject.toml (for tool compatibility).
 
 ## Quick Start
 
 1. Install pip-requirements:
 
    ```shell
-   pip install pip-requirements
+   pip install pyproject-requirements
    ```
 
 2. Install all dependencies of your pyproject.toml 
 
    ```shell
    # use `--optional name` to limit to optional named dependency section
    # use `--required` to install required dependencies
```

### Comparing `pyproject-requirements-20240203/pyproject.toml` & `pyproject_requirements-20240601/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 [tool.setuptools.packages.find]
 where = ["python"]
 #include = ["*", "themes"]
 namespaces = true
 
 
 [project.scripts]
-pip-requirements = "pip_requirements.__main__"
+pip-requirements = "pip_requirements.__main__:main"
```

### Comparing `pyproject-requirements-20240203/python/pip_requirements/__main__.py` & `pyproject_requirements-20240601/python/pip_requirements/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,23 +61,30 @@
         "--optional",
         nargs="*",
         default=[],
         help="Optional dependency to install. May be specified multiple times.",
     )
     parser.add_argument(
         "--pip",
+        default=found_pip,
         required=False if found_pip else True,
         help=f"Pip tool to use. Autodetected. Default: {found_pip}",
     )
     parser.add_argument(
         "--dry",
         help="Dry run",
         default=False,
         action="store_true",
     )
+    parser.add_argument(
+        "--target",
+        default=None,
+        help="Install requirements to target path specified. Ignores already installed dependencies.",
+    )
+
 
     parser = subparsers.add_parser(
         "txt",
         description="Generate a requirements.txt files for compatibility.",
     )
     parser.add_argument("pyproject_toml", help="pyproject.toml")
     parser.add_argument(
@@ -114,32 +121,47 @@
     result = subprocess.run(arg)
     if result.returncode != 0:
         print("Error installing packages with pip:")
         print(result.stderr)
         sys.exit(-1)
 
 
-def main():
+def get_packages_to_install(pyproject_toml: Path, all=False, required=True, optional=False):
+    install_list = []
+    with pyproject_toml.open("r") as f:
+        d = toml.load(f)
 
-    values = cast(list, sys.argv)
-    try:
-        dash_index = values.index("--")
-        extra_args = values[dash_index + 1:]
-        args = values[1:dash_index]
-    except ValueError:
-        args = values[1:]
-        extra_args = []
+        project = d.get("project", None)
 
-    parser = get_argument_parser()
-    args = parser.parse_args(args)
+        if project is None:
+            return install_list
 
-    if args.command == "install":
-        main_install(args, extra_args)
-    elif args.command == "txt":
-        main_generate_txt(args, extra_args)
+        if all or required:
+            install_list += project.get("dependencies", [])
+
+        if all:
+            for category, deps in project.get("optional-dependencies", {}).items():
+                install_list += deps
+        else:
+            for optional_name in optional:
+                optional = project.get("optional-dependencies").get(optional_name, None)
+                if optional is None:
+                    print(f"No optional dependency section: {optional_name}")
+                    sys.exit(-1)
+
+                install_list += optional
+    return install_list
+
+
+def open_toml_file(pyproject_toml):
+    tomlfile = Path(pyproject_toml).expanduser().resolve()
+    if not tomlfile.exists():
+        print(f"pyproject.toml does not exist at {pyproject_toml}")
+        sys.exit(-1)
+    return tomlfile
 
 
 def main_generate_txt(args, extra_args):
 
     if args.output_file:
         output = Path(args.output_file).expanduser()
         if not output.parent.exists():
@@ -152,32 +174,21 @@
 
     tomlfile = open_toml_file(args.pyproject_toml)
 
     if not tomlfile.exists():
         print(f"pyproject.toml does not exist at {args.pyproject_toml}")
         sys.exit(-1)
 
-    install_list = []
-    with tomlfile.open("r") as f:
-        d = toml.load(f)
-
-        if args.all or args.required:
-            install_list += d.get("project").get("dependencies", [])
-
-        if args.all:
-            for category, deps in d.get("project").get("optional-dependencies", {}).items():
-                install_list += deps
-        else:
-            for optional_name in args.optional:
-                optional = d.get("project").get("optional-dependencies").get(optional_name, None)
-                if optional is None:
-                    print(f"No optional dependency section: {optional_name}")
-                    sys.exit(-1)
+    install_list = get_packages_to_install(
+        tomlfile,
+        all=args.all,
+        required=args.required,
+        optional=args.optional,
+    )
 
-                install_list += optional
     if not install_list:
         sys.exit(0)
 
     for line in install_list:
         print(line, file=output)
 
 
@@ -191,43 +202,48 @@
         sys.exit(-1)
 
     if os.access(pip_tool, os.X_OK) is False:
         print(f"Error: pip is not executable at {pip_tool}")
         sys.exit(-1)
 
     print("Reading pyproject file: ", tomlfile)
-    install_list = []
-    with tomlfile.open("r") as f:
-        d = toml.load(f)
-
-        if args.all or args.required:
-            install_list += d.get("project").get("dependencies", [])
-
-        if args.all:
-            for category, deps in d.get("project").get("optional-dependencies", {}).items():
-                install_list += deps
-        else:
-            for optional_name in args.optional:
-                optional = d.get("project").get("optional-dependencies").get(optional_name, None)
-                if optional is None:
-                    print(f"No optional dependency section: {optional_name}")
-                    sys.exit(-1)
+    install_list = get_packages_to_install(
+        tomlfile,
+        all=args.all,
+        required=args.required,
+        optional=args.optional,
+    )
 
-                install_list += optional
     if not install_list:
         print("Nothing found to install.")
         sys.exit(-1)
     print("Installing required packages: ", install_list)
+
+    if args.target:
+        extra_args += ["--target", Path(args.target).expanduser().resolve(strict=False).as_posix()]
+
     if not args.dry:
         pip_install(install_list, pip_tool, extra_args)
 
 
-def open_toml_file(pyproject_toml):
-    tomlfile = Path(pyproject_toml).expanduser().resolve()
-    if not tomlfile.exists():
-        print(f"pyproject.toml does not exist at {pyproject_toml}")
-        sys.exit(-1)
-    return tomlfile
+def main():
+
+    values = cast(list, sys.argv)
+    try:
+        dash_index = values.index("--")
+        extra_args = values[dash_index + 1:]
+        args = values[1:dash_index]
+    except ValueError:
+        args = values[1:]
+        extra_args = []
+
+    parser = get_argument_parser()
+    args = parser.parse_args(args)
+
+    if args.command == "install":
+        main_install(args, extra_args)
+    elif args.command == "txt":
+        main_generate_txt(args, extra_args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyproject-requirements-20240203/python/pyproject_requirements.egg-info/PKG-INFO` & `pyproject_requirements-20240601/python/pyproject_requirements.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: pyproject-requirements
-Version: 20240203
+Version: 20240601
 Summary: Install dependencies from a pyproject using pip.
 Author: MetaCompany, Nate Skulic
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pip
 Requires-Dist: toml
 
-# pip-requirements
+# pip-requirements (aka pyproject-requirements)
 
 Install requirements/dependencies specified in a pyproject.toml using pip.
 
 ## Features
 
 - Installs required, optional and/or all dependencies.
 - Detects and works with pip in installed in virtual environments.
 - Generates a requirements.txt file from a pyproject.toml (for tool compatibility).
 
 ## Quick Start
 
 1. Install pip-requirements:
 
    ```shell
-   pip install pip-requirements
+   pip install pyproject-requirements
    ```
 
 2. Install all dependencies of your pyproject.toml 
 
    ```shell
    # use `--optional name` to limit to optional named dependency section
    # use `--required` to install required dependencies
```

