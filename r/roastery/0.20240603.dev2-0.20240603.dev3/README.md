# Comparing `tmp/roastery-0.20240603.dev2.tar.gz` & `tmp/roastery-0.20240603.dev3.tar.gz`

## Comparing `roastery-0.20240603.dev2.tar` & `roastery-0.20240603.dev3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.envrc
--rw-r--r--   0        0        0      367 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.python-version
--rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/CNAME
--rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/flake.lock
--rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/flake.nix
--rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/requirements-dev.lock
--rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/requirements.lock
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/.gitignore
--rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/misc.xml
--rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/modules.xml
--rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/roastery.iml
--rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/vcs.xml
--rw-r--r--   0        0        0     2994 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/workspace.xml
--rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/docs.sh
--rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/pypi.sh
--rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/refs.sh
--rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/test-pypi.sh
--rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/bin/upload-docs.sh
--rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/.gitignore
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/.python-version
--rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/architecture.rst
--rw-r--r--   0        0        0     1021 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/conf.py
--rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/index.rst
--rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/todo.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/cli.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/config.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/edit.rst
--rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/formats.rst
--rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/importer.rst
--rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/index.rst
--rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/api/term.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/documentation/getting-started/index.rst
--rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/nix/roastery.nix
--rw-r--r--   0        0        0      108 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/nix/shell.nix
--rw-r--r--   0        0        0      374 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/__init__.py
--rw-r--r--   0        0        0     1395 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/cli.py
--rw-r--r--   0        0        0     2675 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/config.py
--rw-r--r--   0        0        0     4211 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/edit.py
--rw-r--r--   0        0        0     2880 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/formats.py
--rw-r--r--   0        0        0     9738 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/importer.py
--rw-r--r--   0        0        0     4362 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/src/roastery/term.py
--rw-r--r--   0        0        0      214 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/conftest.py
--rw-r--r--   0        0        0      355 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/test_cleanable.py
--rw-r--r--   0        0        0     1336 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/test_cli.py
--rw-r--r--   0        0        0     1540 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/tests/test_import_csv.py
--rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/.gitignore
--rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/LICENSE
--rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/README.md
--rw-r--r--   0        0        0      721 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/pyproject.toml
--rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240603.dev2/PKG-INFO
+-rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.envrc
+-rw-r--r--   0        0        0      367 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.python-version
+-rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/CNAME
+-rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/flake.lock
+-rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/flake.nix
+-rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/requirements-dev.lock
+-rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/requirements.lock
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/.gitignore
+-rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/misc.xml
+-rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/modules.xml
+-rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/roastery.iml
+-rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/vcs.xml
+-rw-r--r--   0        0        0     2708 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/workspace.xml
+-rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/bin/docs.sh
+-rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/bin/pypi.sh
+-rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/bin/refs.sh
+-rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/bin/test-pypi.sh
+-rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/bin/upload-docs.sh
+-rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/.gitignore
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/.python-version
+-rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/architecture.rst
+-rw-r--r--   0        0        0     1021 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/conf.py
+-rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/index.rst
+-rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/todo.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/api/cli.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/api/config.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/api/edit.rst
+-rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/api/formats.rst
+-rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/api/importer.rst
+-rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/api/index.rst
+-rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/api/term.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/documentation/getting-started/index.rst
+-rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/nix/roastery.nix
+-rw-r--r--   0        0        0      108 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/nix/shell.nix
+-rw-r--r--   0        0        0      374 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/src/roastery/__init__.py
+-rw-r--r--   0        0        0     1395 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/src/roastery/cli.py
+-rw-r--r--   0        0        0     2675 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/src/roastery/config.py
+-rw-r--r--   0        0        0     4211 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/src/roastery/edit.py
+-rw-r--r--   0        0        0     2880 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/src/roastery/formats.py
+-rw-r--r--   0        0        0    10133 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/src/roastery/importer.py
+-rw-r--r--   0        0        0     4362 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/src/roastery/term.py
+-rw-r--r--   0        0        0      214 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/tests/conftest.py
+-rw-r--r--   0        0        0      355 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/tests/test_cleanable.py
+-rw-r--r--   0        0        0     1336 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/tests/test_cli.py
+-rw-r--r--   0        0        0     2331 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/tests/test_import_csv.py
+-rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/.gitignore
+-rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/LICENSE
+-rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/README.md
+-rw-r--r--   0        0        0      721 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240603.dev3/PKG-INFO
```

### Comparing `roastery-0.20240603.dev2/flake.lock` & `roastery-0.20240603.dev3/flake.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/flake.nix` & `roastery-0.20240603.dev3/flake.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/requirements-dev.lock` & `roastery-0.20240603.dev3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/requirements.lock` & `roastery-0.20240603.dev3/requirements.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/.idea/roastery.iml` & `roastery-0.20240603.dev3/.idea/roastery.iml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/.idea/workspace.xml` & `roastery-0.20240603.dev3/.idea/workspace.xml`

 * *Files 15% similar despite different names*

#### Comparing `roastery-0.20240603.dev2/.idea/workspace.xml` & `roastery-0.20240603.dev3/.idea/workspace.xml`

```diff
@@ -1,16 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="a48802e8-3b0a-4c8b-95a9-aefccbff6157" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/roastery/config.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/roastery/config.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/roastery/importer.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/roastery/importer.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/tests/test_import_csv.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_import_csv.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
```

### Comparing `roastery-0.20240603.dev2/.idea/inspectionProfiles/Project_Default.xml` & `roastery-0.20240603.dev3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/documentation/architecture.rst` & `roastery-0.20240603.dev3/documentation/architecture.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/documentation/conf.py` & `roastery-0.20240603.dev3/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/documentation/api/index.rst` & `roastery-0.20240603.dev3/documentation/api/index.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/nix/roastery.nix` & `roastery-0.20240603.dev3/nix/roastery.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/src/roastery/cli.py` & `roastery-0.20240603.dev3/src/roastery/cli.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/src/roastery/config.py` & `roastery-0.20240603.dev3/src/roastery/config.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/src/roastery/edit.py` & `roastery-0.20240603.dev3/src/roastery/edit.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/src/roastery/formats.py` & `roastery-0.20240603.dev3/src/roastery/formats.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/src/roastery/importer.py` & `roastery-0.20240603.dev3/src/roastery/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,20 +192,23 @@
         postings = [
             _p(self.asset_account, self.amount),
             _p(
                 self.account.value
             ),  # beancount will infer the inverse amount automatically.
         ]
 
+        meta = {k: str(v) for k, v in self.meta.items()}
+        meta |= {"digest": self.digest}
+
         return data.Transaction(
             date=self.date,
             postings=postings,
             payee=self.payee.value,
             narration=self.narration.value,
-            meta={k: str(v) for k, v in self.meta.items()},
+            meta=meta,
             tags=self.tags,
             links=self.links,
             flag=self.flag,
         )
 
     def apply_manual_edits(self, edits: dict[Digest, ManualEdits]) -> None:
         """Apply manual edits to this entry.
@@ -265,14 +268,17 @@
     - Clean the entry using the ``clean`` function, if provided.
     - Write the entry to disk as a Beancount transaction.
 
     The resulting Beancount file is created in the same directory as the CSV file, but with
     the extension changed to ``.beancount``. So: ``statements/foo.csv`` -> ``statements/foo.beancount``
     You can specify a different path with the ``beancount_file`` parameter.
 
+    The transaction is flagged with ``"!"`` if the digest of the entry occurs in the JSON file
+    at :obj:`roastery.config.Config.flags_path`.
+
     :param csv_file: Path of the CSV file to import.
     :param config: Configuration to use.
     :param csv_args: Arguments to forward to :py:class:`csv.DictReader`. This is used to
       parse weird CSV dialects. For example: ``dict(delimiter=";", quotechar="|")``.
     :param extract: How to extract an :class:`Entry` from a row of CSV data. See :py:class:`~ExtractFn`.
     :param clean: User-implemented cleaning function. See :py:class:`~CleanFn`.
     :param beancount_file: Path of the beancount file to write to.
@@ -281,24 +287,32 @@
         csv_file.with_suffix(".beancount") if beancount_file is None else beancount_file
     )
     try:
         manual_edits = json.loads(config.manual_edits_path.read_text())
     except FileNotFoundError:
         manual_edits = {}
 
+    try:
+        flags = json.loads(config.flags_path.read_text())
+    except FileNotFoundError:
+        flags = {}
+
     _csv_args = {} if csv_args is None else csv_args
     _clean = (lambda x: None) if clean is None else clean
 
     with csv_file.open() as f_csv, beancount_file.open(
         mode="w", encoding="utf-8"
     ) as f_journal:
         reader = csv.DictReader(f_csv, **_csv_args)
         for row in reader:
             entry = extract(row)
 
+            if entry.digest in flags:
+                entry.flag = "!"
+
             if (config.do_not_import_before is not None) and (
                 entry.date <= config.do_not_import_before
             ):
                 continue
 
             entry.apply_manual_edits(manual_edits)
             _clean(entry)
```

### Comparing `roastery-0.20240603.dev2/src/roastery/term.py` & `roastery-0.20240603.dev3/src/roastery/term.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/tests/test_cli.py` & `roastery-0.20240603.dev3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/tests/test_import_csv.py` & `roastery-0.20240603.dev3/tests/test_import_csv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 from pathlib import Path
 from typing import Iterator
 
 import pytest
 from beancount import loader
+from beancount.query.query import run_query
 
 from roastery import import_csv, Config, formats
 
 
 def test_import_demo_csv(config: Config, demo_csv: Path) -> None:
     beancount_file = demo_csv.with_suffix(".beancount")
     import_csv(
@@ -31,14 +32,37 @@
         csv_args=dict(delimiter=";"),
     )
     assert beancount_file.exists()
     entries, errors, options = loader.load_file(beancount_file)
     assert len(entries) == 2
 
 
+def test_import_flags(config: Config, demo_csv: Path) -> None:
+    config.flags_path.parent.mkdir(exist_ok=True)
+    md5 = "08f11d07d99ede2c9cb385b77ba5d203"
+    config.flags_path.write_text(f'["{md5}"]')
+    beancount_file = demo_csv.with_suffix(".beancount")
+    import_csv(
+        config=config,
+        csv_file=demo_csv,
+        extract=formats.extract_demo,
+        csv_args=dict(delimiter=";"),
+    )
+    print(beancount_file.read_text())
+    entries, errors, options = loader.load_file(beancount_file)
+    assert len(entries) == 3
+
+    query = """
+    select distinct(any_meta("digest")) where flag = "!"
+    """
+    res_type, res_rows = run_query(entries, options, query)
+    assert len(res_rows) == 1
+    assert res_rows[0][0] == md5
+
+
 @pytest.fixture
 def demo_csv(config: Config) -> Iterator[Path]:
     config.statements_dir.mkdir(exist_ok=True)
     csv_file = config.statements_dir / "test.csv"
 
     csv_file.write_text("""\
 "date";"payee";"description";"amount";"type";"balance_after"
```

### Comparing `roastery-0.20240603.dev2/LICENSE` & `roastery-0.20240603.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/README.md` & `roastery-0.20240603.dev3/README.md`

 * *Files identical despite different names*

### Comparing `roastery-0.20240603.dev2/pyproject.toml` & `roastery-0.20240603.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "roastery"
-version = "0.20240603-dev2"
+version = "0.20240603-dev3"
 dependencies = [
     "beancount>=2.0.0",
     "typer>=0.12.0",
     "fava>=1.27.0",
     "prompt-toolkit>=3.0.0",
 ]
 authors = [
```

### Comparing `roastery-0.20240603.dev2/PKG-INFO` & `roastery-0.20240603.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: roastery
-Version: 0.20240603.dev2
+Version: 0.20240603.dev3
 Summary: Framework for Beancount plain text accounting
 Author-email: Laurens Duijvesteijn <git@duijf.io>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: beancount>=2.0.0
 Requires-Dist: fava>=1.27.0
 Requires-Dist: prompt-toolkit>=3.0.0
```

