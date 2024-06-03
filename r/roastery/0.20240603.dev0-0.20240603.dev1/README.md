# Comparing `tmp/roastery-0.20240603.dev0.tar.gz` & `tmp/roastery-0.20240603.dev1.tar.gz`

## Comparing `roastery-0.20240603.dev0.tar` & `roastery-0.20240603.dev1.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.envrc
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.python-version
--rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/CNAME
--rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/flake.lock
--rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/flake.nix
--rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/requirements-dev.lock
--rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/requirements.lock
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/.gitignore
--rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/misc.xml
--rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/modules.xml
--rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/roastery.iml
--rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/vcs.xml
--rw-r--r--   0        0        0     2153 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/workspace.xml
--rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/docs.sh
--rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/pypi.sh
--rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/refs.sh
--rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/test-pypi.sh
--rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/upload-docs.sh
--rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/.gitignore
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/.python-version
--rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/architecture.rst
--rw-r--r--   0        0        0     1013 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/conf.py
--rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/index.rst
--rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/todo.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/cli.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/config.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/edit.rst
--rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/formats.rst
--rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/importer.rst
--rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/index.rst
--rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/term.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/getting-started/index.rst
--rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/nix/roastery.nix
--rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/nix/shell.nix
--rw-r--r--   0        0        0      375 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/__init__.py
--rw-r--r--   0        0        0      807 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/cli.py
--rw-r--r--   0        0        0     2256 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/config.py
--rw-r--r--   0        0        0     4143 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/edit.py
--rw-r--r--   0        0        0     2742 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/formats.py
--rw-r--r--   0        0        0     9455 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/importer.py
--rw-r--r--   0        0        0     4220 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/term.py
--rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.gitignore
--rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/LICENSE
--rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/README.md
--rw-r--r--   0        0        0      699 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/pyproject.toml
--rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/PKG-INFO
+-rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.envrc
+-rw-r--r--   0        0        0      367 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.python-version
+-rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/CNAME
+-rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/flake.lock
+-rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/flake.nix
+-rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/requirements-dev.lock
+-rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/requirements.lock
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/.gitignore
+-rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/misc.xml
+-rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/modules.xml
+-rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/roastery.iml
+-rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/vcs.xml
+-rw-r--r--   0        0        0     2525 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/workspace.xml
+-rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/docs.sh
+-rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/pypi.sh
+-rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/refs.sh
+-rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/test-pypi.sh
+-rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/bin/upload-docs.sh
+-rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/.gitignore
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/.python-version
+-rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/architecture.rst
+-rw-r--r--   0        0        0     1021 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/conf.py
+-rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/index.rst
+-rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/todo.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/cli.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/config.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/edit.rst
+-rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/formats.rst
+-rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/importer.rst
+-rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/index.rst
+-rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/api/term.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/documentation/getting-started/index.rst
+-rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/nix/roastery.nix
+-rw-r--r--   0        0        0      108 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/nix/shell.nix
+-rw-r--r--   0        0        0      374 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/__init__.py
+-rw-r--r--   0        0        0      828 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/cli.py
+-rw-r--r--   0        0        0     2257 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/config.py
+-rw-r--r--   0        0        0     4211 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/edit.py
+-rw-r--r--   0        0        0     2880 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/formats.py
+-rw-r--r--   0        0        0     9575 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/importer.py
+-rw-r--r--   0        0        0     4362 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/src/roastery/term.py
+-rw-r--r--   0        0        0      355 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/tests/test_cleanable.py
+-rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/.gitignore
+-rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/LICENSE
+-rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/README.md
+-rw-r--r--   0        0        0      721 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240603.dev1/PKG-INFO
```

### Comparing `roastery-0.20240603.dev0/flake.lock` & `roastery-0.20240603.dev1/flake.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/flake.nix` & `roastery-0.20240603.dev1/flake.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/requirements-dev.lock` & `roastery-0.20240603.dev1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/requirements.lock` & `roastery-0.20240603.dev1/requirements.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/.idea/roastery.iml` & `roastery-0.20240603.dev1/.idea/roastery.iml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/.idea/workspace.xml` & `roastery-0.20240603.dev1/.idea/workspace.xml`

 * *Files 17% similar despite different names*

#### Comparing `roastery-0.20240603.dev0/.idea/workspace.xml` & `roastery-0.20240603.dev1/.idea/workspace.xml`

```diff
@@ -1,37 +1,40 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="a48802e8-3b0a-4c8b-95a9-aefccbff6157" name="Changes" comment=""/>
+    <list default="true" id="a48802e8-3b0a-4c8b-95a9-aefccbff6157" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/.pre-commit-config.yaml" beforeDir="false" afterPath="$PROJECT_DIR$/.pre-commit-config.yaml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/tests/test_cleanable.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_cleanable.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
-  <component name="ProjectColorInfo"><![CDATA[{
-  "associatedIndex": 6
-}]]></component>
+  <component name="ProjectColorInfo">{
+  &quot;associatedIndex&quot;: 6
+}</component>
   <component name="ProjectId" id="2hCkutbpdpIYGPifZHQJ5wXrclA"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "/Users/duijf/fin/roastery",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/Users/duijf/fin/roastery&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
-}]]></component>
+}</component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
         <option value="bundled-python-sdk-babbdf50b680-746f403e7f0c-com.jetbrains.pycharm.community.sharedIndexes.bundled-PC-241.15989.155"/>
       </set>
     </attachedChunks>
   </component>
```

### Comparing `roastery-0.20240603.dev0/.idea/inspectionProfiles/Project_Default.xml` & `roastery-0.20240603.dev1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/documentation/architecture.rst` & `roastery-0.20240603.dev1/documentation/architecture.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/documentation/conf.py` & `roastery-0.20240603.dev1/documentation/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,37 +12,35 @@
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
 ]
 html_theme = "furo"
 html_title = "<code>roastery</code>"
 
 autodoc_default_options = {
-  "undoc-members": True,
-  "member-order": "bysource",
+    "undoc-members": True,
+    "member-order": "bysource",
 }
 autodoc_typehints = "both"
 
 autodoc_type_aliases = {
     "CleanFn": "roastery.importer.CleanFn",
     "ExtractFn": "roastery.importer.ExtractFn",
 }
 
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3', None),
-    'fava': ("https://beancount.github.io/fava/", None),
+    "python": ("https://docs.python.org/3", None),
+    "fava": ("https://beancount.github.io/fava/", None),
 }
 
 nitpicky = True
 nitpick_ignore = [
-  ("py:class", r"any"),
-  ("py:class", r"roastery.importer.CleanFn"),
-  ("py:class", r"roastery.importer.ExtractFn"),
+    ("py:class", r"any"),
+    ("py:class", r"roastery.importer.CleanFn"),
+    ("py:class", r"roastery.importer.ExtractFn"),
 ]
 nitpick_ignore_regex = [
-  ("py:class", r"beancount.*"),
+    ("py:class", r"beancount.*"),
 ]
 
-exclude_patterns = [
-  r"getting-started/finance.*"
-]
+exclude_patterns = [r"getting-started/finance.*"]
 
 todo_include_todos = True
```

### Comparing `roastery-0.20240603.dev0/documentation/api/index.rst` & `roastery-0.20240603.dev1/documentation/api/index.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/nix/roastery.nix` & `roastery-0.20240603.dev1/nix/roastery.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/src/roastery/cli.py` & `roastery-0.20240603.dev1/src/roastery/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,11 +20,13 @@
     def edit_cmd() -> None:
         """Edit transactions that haven't been classified yet."""
         edit_main(config)
 
     @cli.command(name="fava")
     def fava_cmd() -> None:
         """Start fava, the beancount web UI."""
-        typer.launch("http://localhost:5000/", )
+        typer.launch(
+            "http://localhost:5000/",
+        )
         os.execvp("fava", ["fava", config.journal_path])
 
     return cli
```

### Comparing `roastery-0.20240603.dev0/src/roastery/config.py` & `roastery-0.20240603.dev1/src/roastery/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 API
 ---
 
 .. autoclass:: Config
    :members:
 """
+
 import dataclasses
 import os
 import sys
 from pathlib import Path
 
 
 @dataclasses.dataclass
@@ -50,15 +51,15 @@
       When :py:obj:`roastery.importer.Entry.is_expense` returns ``True``.
 
     ``"Income:Unknown"``
       When :py:obj:`roastery.importer.Entry.is_income` returns ``True``.
      """
 
     @classmethod
-    def from_env(cls, project_root: Path = None) -> 'Config':
+    def from_env(cls, project_root: Path = None) -> "Config":
         """
         Create a :py:class:`Config` based on the `Environment variables`_ that are set.
 
         This is a convenience method. If you want different defaults you can instantiate
         this class yourself.
         """
         try:
```

### Comparing `roastery-0.20240603.dev0/src/roastery/edit.py` & `roastery-0.20240603.dev1/src/roastery/edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Find all unclassified / unprocessed transactions and prompt the user to classify
 and edit them.
 
 This is one of the nice tools that Roastery has on offer and is what allows you to
 easily and quickly edit large amounts of transaction data. Any edits made by the
 end user are saved in a JSON file that can be version controlled with git.
 """
+
 import datetime
 import json
 import typing
 from collections import defaultdict
 
 from beancount import loader
 from beancount.core import data
@@ -41,14 +42,15 @@
     narration: str
     tags: list[str]
     links: list[str]
 
 
 class Unprocessed(typing.Protocol):
     """Utility type representing an unprocessed entry."""
+
     date: datetime.date
     position: Position
     payee: str
     narration: str
     digest: str
     type: str
 
@@ -93,34 +95,38 @@
 
     :param config: The configuration to use to find files on disk.
     """
     entries, errors, options = loader.load_file(config.journal_path)
 
     accounts = {entry.account for entry in entries if isinstance(entry, data.Open)}
     accounts = [
-        account for account in accounts
-        if "Assets:Bank" not in account
-            and "Equity:Opening-Balances" not in account
+        account
+        for account in accounts
+        if "Assets:Bank" not in account and "Equity:Opening-Balances" not in account
     ]
 
     to_save = defaultdict(dict)
     to_skip = set(json.loads(config.skip_path.read_text()))
 
     try:
         for item in get_unprocessed(entries, options):
             if item.digest in to_skip:
                 continue
 
             display(item)
-            account_or_skip = term.select_fuzzy_search("Select account", options=accounts + ["Skip"])
+            account_or_skip = term.select_fuzzy_search(
+                "Select account", options=accounts + ["Skip"]
+            )
 
             if account_or_skip == "Skip":
                 to_skip.add(item.digest)
             else:
-                payee_pretty = item.payee.title() if item.payee.isupper() else item.payee
+                payee_pretty = (
+                    item.payee.title() if item.payee.isupper() else item.payee
+                )
                 item_edits = {
                     "account": account_or_skip,
                     "payee": term.ask("Payee", default=payee_pretty),
                     "narration": term.ask("Narration", default=item.narration),
                 }
                 to_save[item.digest] = item_edits
     except KeyboardInterrupt:
```

### Comparing `roastery-0.20240603.dev0/src/roastery/formats.py` & `roastery-0.20240603.dev1/src/roastery/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 
 from beancount.core.data import Amount
 from beancount.core.number import D
 
 from roastery.importer import Entry
 
 
-DemoCsvRow = TypedDict("DemoCsvRow", {
-    "date": str,
-    "payee": str,
-    "description": str,
-    "amount": str,
-    "type": str,
-    "balance_after": str,
-})
+DemoCsvRow = TypedDict(
+    "DemoCsvRow",
+    {
+        "date": str,
+        "payee": str,
+        "description": str,
+        "amount": str,
+        "type": str,
+        "balance_after": str,
+    },
+)
 
 
 def extract_demo(row: DemoCsvRow) -> Entry:
     # TODO: Extract `Assets:Bank` and `EUR`
     return Entry.from_row(
         digest=hashlib.md5(str(row).encode("utf-8")).hexdigest(),
         asset_account="Assets:Bank",
@@ -29,37 +32,40 @@
         original_payee=row["payee"],
         original_narration=row["description"],
         meta={"balance_after": row["balance_after"], "type": row["type"]},
     )
 
 
 # CSV columns of the
-AsnCsvRow = TypedDict("AsnCsvRow", {
-    "Boekingsdatum": str,
-    "Opdrachtgeversrekening": str,
-    "Tegenrekeningnummer": str,
-    "Naam tegenrekening": str,
-    # Begin: unused
-    "Adres": str,
-    "Postcode": str,
-    "Plaats": str,
-    # End: unused
-    "Valutasoort rekening": str,
-    "Saldo rekening voor mutatie": str,
-    "Valutasoort mutatie": str,
-    "Transactiebedrag": str,
-    "Journaaldatum": str,
-    "Valutadatum": str,
-    "Interne transactiecode": str,
-    "Globale transactiecode": str,
-    "Volgnummer transactie": str,
-    "Betalingskenmerk": str,
-    "Omschrijving": str,
-    "Afschriftnummer": str,
-})
+AsnCsvRow = TypedDict(
+    "AsnCsvRow",
+    {
+        "Boekingsdatum": str,
+        "Opdrachtgeversrekening": str,
+        "Tegenrekeningnummer": str,
+        "Naam tegenrekening": str,
+        # Begin: unused
+        "Adres": str,
+        "Postcode": str,
+        "Plaats": str,
+        # End: unused
+        "Valutasoort rekening": str,
+        "Saldo rekening voor mutatie": str,
+        "Valutasoort mutatie": str,
+        "Transactiebedrag": str,
+        "Journaaldatum": str,
+        "Valutadatum": str,
+        "Interne transactiecode": str,
+        "Globale transactiecode": str,
+        "Volgnummer transactie": str,
+        "Betalingskenmerk": str,
+        "Omschrijving": str,
+        "Afschriftnummer": str,
+    },
+)
 
 
 class AsnMeta(TypedDict):
     digest: str
     type: str
     tegenrekening: NotRequired[str]
     volgnummer: NotRequired[str]
```

### Comparing `roastery-0.20240603.dev0/src/roastery/importer.py` & `roastery-0.20240603.dev1/src/roastery/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,23 +39,24 @@
 
         >>> Cleanable(original="foo", cleaned="bar").value
         'bar'
 
         >>> Cleanable(original="foo", cleaned="bar", edited="baz").value
         'baz'
     """
+
     original: str | None = None
     cleaned: str | None = None
     edited: str | None = None
 
     @property
     def value(self) -> str | None:
         """The first not-None value :py:attr:`~edited`, :py:attr:`~cleaned`, and :py:attr:`~original`"""
         vals = (self.edited, self.cleaned, self.original)
-        return next(arg for arg in vals if arg is not None, None)
+        return next((arg for arg in vals if arg is not None), None)
 
 
 Digest: TypeAlias = str
 """Hash digest of an :class:`Entry`, as a string."""
 
 EntryMeta: TypeAlias = TypeVar("EntryMeta", bound=dict)
 """Type annotation for the metadata dictionary in Entry.
@@ -148,16 +149,16 @@
         *,
         digest: str,
         date: datetime.date,
         amount: data.Amount,
         asset_account: str,
         meta: EntryMeta | None = None,
         original_payee: str | None = None,
-        original_narration: str | None = None
-    ) -> 'Entry':
+        original_narration: str | None = None,
+    ) -> "Entry":
         """Convenience constructor that can be called by integrators of a new source data type."""
         return cls(
             digest=digest,
             date=date,
             amount=amount,
             meta=meta or {},
             asset_account=asset_account,
@@ -174,22 +175,29 @@
     @property
     def is_expense(self) -> bool:
         """Does this entry represent an expense?"""
         return not self.is_income
 
     def as_transaction(self) -> data.Transaction:
         """Turn this entry into a beancount ``Transaction``."""
+
         def _p(account, amount=None):
-            return data.Posting(account=account, units=amount, cost=None, price=None, flag=None, meta={})
+            return data.Posting(
+                account=account, units=amount, cost=None, price=None, flag=None, meta={}
+            )
 
-        self.account.original = "Income:Unknown" if self.is_income else "Expenses:Unknown"
+        self.account.original = (
+            "Income:Unknown" if self.is_income else "Expenses:Unknown"
+        )
 
         postings = [
             _p(self.asset_account, self.amount),
-            _p(self.account.value),  # beancount will infer the inverse amount automatically.
+            _p(
+                self.account.value
+            ),  # beancount will infer the inverse amount automatically.
         ]
 
         return data.Transaction(
             date=self.date,
             postings=postings,
             payee=self.payee.value,
             narration=self.narration.value,
@@ -241,15 +249,15 @@
 def import_csv(
     *,
     csv_file: Path,
     config: Config,
     extract: ExtractFn,
     beancount_file: Path = None,
     clean: CleanFn = None,
-    csv_args: dict[str, any] = None
+    csv_args: dict[str, any] = None,
 ) -> None:
     """
     Import a CSV file and write a beancount file.
 
     For each row of the CSV file:
 
     - Create an :class:`Entry` using the ``extract`` function.
@@ -265,23 +273,27 @@
     :param config: Configuration to use.
     :param csv_args: Arguments to forward to :py:class:`csv.DictReader`. This is used to
       parse weird CSV dialects. For example: ``dict(delimiter=";", quotechar="|")``.
     :param extract: How to extract an :class:`Entry` from a row of CSV data. See :py:class:`~ExtractFn`.
     :param clean: User-implemented cleaning function. See :py:class:`~CleanFn`.
     :param beancount_file: Path of the beancount file to write to.
     """
-    beancount_file = csv_file.with_suffix(".beancount") if beancount_file is None else beancount_file
+    beancount_file = (
+        csv_file.with_suffix(".beancount") if beancount_file is None else beancount_file
+    )
     try:
         manual_edits = json.loads(config.manual_edits_path.read_text())
     except FileNotFoundError:
         manual_edits = {}
 
     _csv_args = {} if csv_args is None else csv_args
     _clean = (lambda x: None) if clean is None else clean
 
-    with csv_file.open() as f_csv, beancount_file.open(mode="w", encoding="utf-8") as f_journal:
+    with csv_file.open() as f_csv, beancount_file.open(
+        mode="w", encoding="utf-8"
+    ) as f_journal:
         reader = csv.DictReader(f_csv, **_csv_args)
         for row in reader:
             entry = extract(row)
             entry.apply_manual_edits(manual_edits)
             _clean(entry)
             printer.print_entry(entry.as_transaction(), file=f_journal)
```

### Comparing `roastery-0.20240603.dev0/src/roastery/term.py` & `roastery-0.20240603.dev1/src/roastery/term.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 User input
 ----------
 
 .. autofunction:: roastery.term.ask
 .. autofunction:: roastery.term.select_fuzzy_search
 """
+
 import subprocess
 
 from prompt_toolkit import prompt
 from prompt_toolkit.enums import EditingMode
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.output.color_depth import ColorDepth
 from rich import print as rprint
@@ -96,20 +97,31 @@
 
     Users will be able to enter their answer in a readline-style environment with
     vi-style keybindings.
 
     :param question: Question to prompt the user with.
     :param default: Default to pre-populate the readline env
     """
-    display = FormattedText([("bold blue", f"| {question} > ",)])
+    display = FormattedText(
+        [
+            (
+                "bold blue",
+                f"| {question} > ",
+            )
+        ]
+    )
     # The color depth is so that `blue` refers to the color scheme in
     # use by the terminal. This means we respect the theme that was set
     # by the user.
-    res = prompt(display, editing_mode=EditingMode.VI, default=default,
-                 color_depth=ColorDepth.ANSI_COLORS_ONLY)
+    res = prompt(
+        display,
+        editing_mode=EditingMode.VI,
+        default=default,
+        color_depth=ColorDepth.ANSI_COLORS_ONLY,
+    )
     print()
     return res
 
 
 def select_fuzzy_search(
     prompt: str,
     *,
@@ -123,19 +135,24 @@
     :param options: List of options that the user can choose from.
 
     :raises KeyboardInterrupt: If the user did not confirm the selection.
     """
     fzf_input = "\n".join(options)
     fzf_cmd = ["fzf", "--height", "~30%", f"--prompt=| {prompt} > "]
 
-    fzf_proc = subprocess.run(fzf_cmd, input=fzf_input, text=True, stdout=subprocess.PIPE)
+    fzf_proc = subprocess.run(
+        fzf_cmd, input=fzf_input, text=True, stdout=subprocess.PIPE
+    )
     fzf_choice = fzf_proc.stdout.strip()
 
     if fzf_choice == "":
         error("User aborted selection")
         raise KeyboardInterrupt
 
     # Log the users choice in the same style as the FZF prompt.
-    log(f"[bold blue]{prompt} >[/bold blue] [bold]{fzf_choice}[/bold]", style="bold blue")
+    log(
+        f"[bold blue]{prompt} >[/bold blue] [bold]{fzf_choice}[/bold]",
+        style="bold blue",
+    )
 
     assert fzf_choice in options
     return fzf_choice
```

### Comparing `roastery-0.20240603.dev0/LICENSE` & `roastery-0.20240603.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/README.md` & `roastery-0.20240603.dev1/README.md`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev0/pyproject.toml` & `roastery-0.20240603.dev1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "roastery"
-version = "0.20240603-dev"
+version = "0.20240603-dev1"
 dependencies = [
     "beancount>=2.0.0",
     "typer>=0.12.0",
     "fava>=1.27.0",
     "prompt-toolkit>=3.0.0",
 ]
 authors = [
@@ -21,14 +21,15 @@
 [tool.rye]
 managed = true
 dev-dependencies = [
     "sphinx>=7.3.7",
     "sphinx-autobuild>=2024.4.16",
     "furo>=2024.5.6",
     "myst-parser>=3.0.1",
+    "pytest>=8.2.1",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/roastery"]
```

### Comparing `roastery-0.20240603.dev0/PKG-INFO` & `roastery-0.20240603.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: roastery
-Version: 0.20240603.dev0
+Version: 0.20240603.dev1
 Summary: Framework for Beancount plain text accounting
 Author-email: Laurens Duijvesteijn <git@duijf.io>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: beancount>=2.0.0
 Requires-Dist: fava>=1.27.0
 Requires-Dist: prompt-toolkit>=3.0.0
```

