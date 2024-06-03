# Comparing `tmp/roastery-0.20240603.dev1.tar.gz` & `tmp/roastery-0.20240603.dev2.tar.gz`

## Comparing `roastery-0.20240603.dev1.tar` & `roastery-0.20240603.dev2.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.envrc
--rw-r--r--   0        0        0      367 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.python-version
--rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/CNAME
--rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/flake.lock
--rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/flake.nix
--rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/requirements-dev.lock
--rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/requirements.lock
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/.gitignore
--rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/misc.xml
--rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/modules.xml
--rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/roastery.iml
--rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/vcs.xml
--rw-r--r--   0        0        0     2525 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/workspace.xml
--rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/docs.sh
--rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/pypi.sh
--rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/refs.sh
--rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/test-pypi.sh
--rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/upload-docs.sh
--rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/.gitignore
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/.python-version
--rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/architecture.rst
--rw-r--r--   0        0        0     1021 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/conf.py
--rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/index.rst
--rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/todo.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/cli.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/config.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/edit.rst
--rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/formats.rst
--rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/importer.rst
--rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/index.rst
--rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/term.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/getting-started/index.rst
--rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/nix/roastery.nix
--rw-r--r--   0        0        0      108 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/nix/shell.nix
--rw-r--r--   0        0        0      374 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/__init__.py
--rw-r--r--   0        0        0      828 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/cli.py
--rw-r--r--   0        0        0     2257 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/config.py
--rw-r--r--   0        0        0     4211 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/edit.py
--rw-r--r--   0        0        0     2880 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/formats.py
--rw-r--r--   0        0        0     9575 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/importer.py
--rw-r--r--   0        0        0     4362 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/term.py
--rw-r--r--   0        0        0      355 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/tests/test_cleanable.py
--rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.gitignore
--rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/LICENSE
--rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/README.md
--rw-r--r--   0        0        0      721 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/pyproject.toml
--rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/PKG-INFO
+-rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.envrc
+-rw-r--r--   0        0        0      367 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.python-version
+-rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/CNAME
+-rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/flake.lock
+-rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/flake.nix
+-rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/requirements-dev.lock
+-rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/requirements.lock
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/.gitignore
+-rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/misc.xml
+-rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/modules.xml
+-rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/roastery.iml
+-rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/vcs.xml
+-rw-r--r--   0        0        0     2994 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/workspace.xml
+-rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/docs.sh
+-rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/pypi.sh
+-rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/refs.sh
+-rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/test-pypi.sh
+-rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/upload-docs.sh
+-rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/.gitignore
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/.python-version
+-rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/architecture.rst
+-rw-r--r--   0        0        0     1021 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/conf.py
+-rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/index.rst
+-rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/todo.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/cli.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/config.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/edit.rst
+-rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/formats.rst
+-rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/importer.rst
+-rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/index.rst
+-rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/term.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/getting-started/index.rst
+-rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/nix/roastery.nix
+-rw-r--r--   0        0        0      108 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/nix/shell.nix
+-rw-r--r--   0        0        0      374 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/__init__.py
+-rw-r--r--   0        0        0     1395 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/cli.py
+-rw-r--r--   0        0        0     2675 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/config.py
+-rw-r--r--   0        0        0     4211 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/edit.py
+-rw-r--r--   0        0        0     2880 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/formats.py
+-rw-r--r--   0        0        0     9738 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/importer.py
+-rw-r--r--   0        0        0     4362 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/term.py
+-rw-r--r--   0        0        0      214 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/conftest.py
+-rw-r--r--   0        0        0      355 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/test_cleanable.py
+-rw-r--r--   0        0        0     1336 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/test_cli.py
+-rw-r--r--   0        0        0     1540 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/test_import_csv.py
+-rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.gitignore
+-rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/LICENSE
+-rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/README.md
+-rw-r--r--   0        0        0      721 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/PKG-INFO
```

### Comparing `roastery-0.20240603.dev1/flake.lock` & `roastery-0.20240603.dev2/flake.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/flake.nix` & `roastery-0.20240603.dev2/flake.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/requirements-dev.lock` & `roastery-0.20240603.dev2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/requirements.lock` & `roastery-0.20240603.dev2/requirements.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/.idea/roastery.iml` & `roastery-0.20240603.dev2/.idea/roastery.iml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/.idea/workspace.xml` & `roastery-0.20240603.dev2/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `roastery-0.20240603.dev1/.idea/workspace.xml` & `roastery-0.20240603.dev2/.idea/workspace.xml`

```diff
@@ -1,22 +1,31 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="a48802e8-3b0a-4c8b-95a9-aefccbff6157" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/.pre-commit-config.yaml" beforeDir="false" afterPath="$PROJECT_DIR$/.pre-commit-config.yaml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/test_cleanable.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_cleanable.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/roastery/config.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/roastery/config.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/roastery/importer.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/roastery/importer.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test_import_csv.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_import_csv.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
+  <component name="FileTemplateManagerImpl">
+    <option name="RECENT_TEMPLATES">
+      <list>
+        <option value="Python Script"/>
+      </list>
+    </option>
+  </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="ProjectColorInfo">{
   &quot;associatedIndex&quot;: 6
 }</component>
   <component name="ProjectId" id="2hCkutbpdpIYGPifZHQJ5wXrclA"/>
```

### Comparing `roastery-0.20240603.dev1/.idea/inspectionProfiles/Project_Default.xml` & `roastery-0.20240603.dev2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/documentation/architecture.rst` & `roastery-0.20240603.dev2/documentation/architecture.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/documentation/conf.py` & `roastery-0.20240603.dev2/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/documentation/api/index.rst` & `roastery-0.20240603.dev2/documentation/api/index.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/nix/roastery.nix` & `roastery-0.20240603.dev2/nix/roastery.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/src/roastery/cli.py` & `roastery-0.20240603.dev2/src/roastery/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import json
 import os
+import sys
 
 import typer
 from rich.traceback import install as install_traceback_handler
 
 from roastery.config import Config
 from roastery.edit import main as edit_main
 
@@ -25,8 +27,24 @@
     def fava_cmd() -> None:
         """Start fava, the beancount web UI."""
         typer.launch(
             "http://localhost:5000/",
         )
         os.execvp("fava", ["fava", config.journal_path])
 
+    @cli.command(name="flag")
+    def flag_cmd(digest: str) -> None:
+        """Flag an entry for later review, based on digest."""
+        if len(digest) != 32:
+            print("Digest should be a 32 character md5 hash")
+            sys.exit(1)
+
+        try:
+            flags = set(json.loads(config.flags_path.read_text()))
+        except Exception:
+            flags = set()
+
+        flags.add(digest)
+        config.flags_path.parent.mkdir(exist_ok=True)
+        config.flags_path.write_text(json.dumps(sorted(flags), indent=4) + "\n")
+
     return cli
```

### Comparing `roastery-0.20240603.dev1/src/roastery/config.py` & `roastery-0.20240603.dev2/src/roastery/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ---
 
 .. autoclass:: Config
    :members:
 """
 
 import dataclasses
+import datetime
 import os
 import sys
 from pathlib import Path
 
 
 @dataclasses.dataclass
 class Config:
@@ -37,27 +38,36 @@
     journal_path: Path
     """Location of the main journal."""
 
     manual_edits_path: Path
     """Filepath to store end user manual edits."""
 
     skip_path: Path
-    """File containing digests of transactions to skip while editing . See :py:mod:`roastery.edit`."""
+    """File containing digests of transactions to skip while editing. See :py:mod:`roastery.edit`."""
+
+    flags_path: Path
+    """File containing digests of transactions that have been flagged for later review."""
 
     default_account_name_suffix: str = "Unknown"
     """Income/Expenses account name suffix to use when no better one is available in
     :py:obj:`roastery.importer.Entry.as_transaction`
 
     ``"Expenses:Unknown"``
       When :py:obj:`roastery.importer.Entry.is_expense` returns ``True``.
 
     ``"Income:Unknown"``
       When :py:obj:`roastery.importer.Entry.is_income` returns ``True``.
      """
 
+    do_not_import_before: datetime.date = None
+    """Date before which to skip importing transactions.
+
+    This is useful if you want to keep a your entire history of financial statements and
+    gradually import / classify them."""
+
     @classmethod
     def from_env(cls, project_root: Path = None) -> "Config":
         """
         Create a :py:class:`Config` based on the `Environment variables`_ that are set.
 
         This is a convenience method. If you want different defaults you can instantiate
         this class yourself.
@@ -72,8 +82,9 @@
             sys.exit(1)
 
         return cls(
             statements_dir=root / "statements",
             journal_path=root / "journal/main.beancount",
             manual_edits_path=root / ".roastery/manual-edits.json",
             skip_path=root / ".roastery/skip.json",
+            flags_path=root / ".roastery/flags.json",
         )
```

### Comparing `roastery-0.20240603.dev1/src/roastery/edit.py` & `roastery-0.20240603.dev2/src/roastery/edit.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/src/roastery/formats.py` & `roastery-0.20240603.dev2/src/roastery/formats.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/src/roastery/importer.py` & `roastery-0.20240603.dev2/src/roastery/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,10 +290,16 @@
 
     with csv_file.open() as f_csv, beancount_file.open(
         mode="w", encoding="utf-8"
     ) as f_journal:
         reader = csv.DictReader(f_csv, **_csv_args)
         for row in reader:
             entry = extract(row)
+
+            if (config.do_not_import_before is not None) and (
+                entry.date <= config.do_not_import_before
+            ):
+                continue
+
             entry.apply_manual_edits(manual_edits)
             _clean(entry)
             printer.print_entry(entry.as_transaction(), file=f_journal)
```

### Comparing `roastery-0.20240603.dev1/src/roastery/term.py` & `roastery-0.20240603.dev2/src/roastery/term.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/LICENSE` & `roastery-0.20240603.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/README.md` & `roastery-0.20240603.dev2/README.md`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev1/pyproject.toml` & `roastery-0.20240603.dev2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "roastery"
-version = "0.20240603-dev1"
+version = "0.20240603-dev2"
 dependencies = [
     "beancount>=2.0.0",
     "typer>=0.12.0",
     "fava>=1.27.0",
     "prompt-toolkit>=3.0.0",
 ]
 authors = [
```

### Comparing `roastery-0.20240603.dev1/PKG-INFO` & `roastery-0.20240603.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: roastery
-Version: 0.20240603.dev1
+Version: 0.20240603.dev2
 Summary: Framework for Beancount plain text accounting
 Author-email: Laurens Duijvesteijn <git@duijf.io>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: beancount>=2.0.0
 Requires-Dist: fava>=1.27.0
 Requires-Dist: prompt-toolkit>=3.0.0
```

