# Comparing `tmp/roastery-0.20240531.dev1.tar.gz` & `tmp/roastery-0.20240603.dev0.tar.gz`

## Comparing `roastery-0.20240531.dev1.tar` & `roastery-0.20240603.dev0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.envrc
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.python-version
--rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/CNAME
--rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/flake.lock
--rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/flake.nix
--rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/requirements-dev.lock
--rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/requirements.lock
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/.gitignore
--rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/misc.xml
--rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/modules.xml
--rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/roastery.iml
--rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/vcs.xml
--rw-r--r--   0        0        0     2449 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/workspace.xml
--rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.idea/inspectionProfiles/profiles_settings.xml
--rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/bin/docs.sh
--rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/bin/pypi.sh
--rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/bin/refs.sh
--rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/bin/test-pypi.sh
--rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/bin/upload-docs.sh
--rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/.gitignore
--rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/.python-version
--rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/architecture.rst
--rw-r--r--   0        0        0     1013 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/conf.py
--rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/index.rst
--rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/todo.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/api/cli.rst
--rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/api/config.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/api/edit.rst
--rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/api/formats.rst
--rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/api/importer.rst
--rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/api/index.rst
--rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/api/term.rst
--rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/documentation/getting-started/index.rst
--rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/nix/roastery.nix
--rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/nix/shell.nix
--rw-r--r--   0        0        0      375 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/src/roastery/__init__.py
--rw-r--r--   0        0        0      807 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/src/roastery/cli.py
--rw-r--r--   0        0        0     2256 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/src/roastery/config.py
--rw-r--r--   0        0        0     4143 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/src/roastery/edit.py
--rw-r--r--   0        0        0     2742 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/src/roastery/formats.py
--rw-r--r--   0        0        0     9494 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/src/roastery/importer.py
--rw-r--r--   0        0        0     4220 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/src/roastery/term.py
--rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/.gitignore
--rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/LICENSE
--rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/README.md
--rw-r--r--   0        0        0      700 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/pyproject.toml
--rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240531.dev1/PKG-INFO
+-rw-r--r--   0        0        0       49 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.envrc
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.python-version
+-rw-r--r--   0        0        0       17 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/CNAME
+-rw-r--r--   0        0        0     1499 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/flake.lock
+-rw-r--r--   0        0        0      903 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/flake.nix
+-rw-r--r--   0        0        0     4203 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/requirements-dev.lock
+-rw-r--r--   0        0        0     2910 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/requirements.lock
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/.gitignore
+-rw-r--r--   0        0        0      300 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/misc.xml
+-rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/modules.xml
+-rw-r--r--   0        0        0      712 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/roastery.iml
+-rw-r--r--   0        0        0      167 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2153 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/workspace.xml
+-rw-r--r--   0        0        0      956 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.idea/inspectionProfiles/profiles_settings.xml
+-rwxr-xr-x   0        0        0      142 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/docs.sh
+-rwxr-xr-x   0        0        0       88 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/pypi.sh
+-rwxr-xr-x   0        0        0      105 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/refs.sh
+-rwxr-xr-x   0        0        0      169 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/test-pypi.sh
+-rwxr-xr-x   0        0        0      320 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/bin/upload-docs.sh
+-rw-r--r--   0        0        0       93 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/.gitignore
+-rw-r--r--   0        0        0        7 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/.python-version
+-rw-r--r--   0        0        0     2480 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/architecture.rst
+-rw-r--r--   0        0        0     1013 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/conf.py
+-rw-r--r--   0        0        0      197 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/index.rst
+-rw-r--r--   0        0        0       55 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/todo.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/cli.rst
+-rw-r--r--   0        0        0       61 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/config.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/edit.rst
+-rw-r--r--   0        0        0       60 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/formats.rst
+-rw-r--r--   0        0        0       74 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/importer.rst
+-rw-r--r--   0        0        0      606 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/index.rst
+-rw-r--r--   0        0        0       69 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/api/term.rst
+-rw-r--r--   0        0        0       70 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/documentation/getting-started/index.rst
+-rw-r--r--   0        0        0      520 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/nix/roastery.nix
+-rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/nix/shell.nix
+-rw-r--r--   0        0        0      375 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/__init__.py
+-rw-r--r--   0        0        0      807 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/cli.py
+-rw-r--r--   0        0        0     2256 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/config.py
+-rw-r--r--   0        0        0     4143 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/edit.py
+-rw-r--r--   0        0        0     2742 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/formats.py
+-rw-r--r--   0        0        0     9455 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/importer.py
+-rw-r--r--   0        0        0     4220 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/src/roastery/term.py
+-rw-r--r--   0        0        0      152 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/.gitignore
+-rw-r--r--   0        0        0     1077 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/LICENSE
+-rw-r--r--   0        0        0     1701 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/README.md
+-rw-r--r--   0        0        0      699 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2081 1980-01-01 00:00:00.000000 roastery-0.20240603.dev0/PKG-INFO
```

### Comparing `roastery-0.20240531.dev1/flake.lock` & `roastery-0.20240603.dev0/flake.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/flake.nix` & `roastery-0.20240603.dev0/flake.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/requirements-dev.lock` & `roastery-0.20240603.dev0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/requirements.lock` & `roastery-0.20240603.dev0/requirements.lock`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/.idea/roastery.iml` & `roastery-0.20240603.dev0/.idea/roastery.iml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/.idea/workspace.xml` & `roastery-0.20240603.dev0/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `roastery-0.20240531.dev1/.idea/workspace.xml` & `roastery-0.20240603.dev0/.idea/workspace.xml`

```diff
@@ -1,17 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="a48802e8-3b0a-4c8b-95a9-aefccbff6157" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/roastery/config.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/roastery/config.py" afterDir="false"/>
-    </list>
+    <list default="true" id="a48802e8-3b0a-4c8b-95a9-aefccbff6157" name="Changes" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
```

### Comparing `roastery-0.20240531.dev1/.idea/inspectionProfiles/Project_Default.xml` & `roastery-0.20240603.dev0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/documentation/architecture.rst` & `roastery-0.20240603.dev0/documentation/architecture.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/documentation/conf.py` & `roastery-0.20240603.dev0/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/documentation/api/index.rst` & `roastery-0.20240603.dev0/documentation/api/index.rst`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/nix/roastery.nix` & `roastery-0.20240603.dev0/nix/roastery.nix`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/src/roastery/cli.py` & `roastery-0.20240603.dev0/src/roastery/cli.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/src/roastery/config.py` & `roastery-0.20240603.dev0/src/roastery/config.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/src/roastery/edit.py` & `roastery-0.20240603.dev0/src/roastery/edit.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/src/roastery/formats.py` & `roastery-0.20240603.dev0/src/roastery/formats.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/src/roastery/importer.py` & `roastery-0.20240603.dev0/src/roastery/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,25 +44,25 @@
         'baz'
     """
     original: str | None = None
     cleaned: str | None = None
     edited: str | None = None
 
     @property
-    def value(self) -> str:
+    def value(self) -> str | None:
         """The first not-None value :py:attr:`~edited`, :py:attr:`~cleaned`, and :py:attr:`~original`"""
         vals = (self.edited, self.cleaned, self.original)
-        return next(arg for arg in vals if arg is not None)
+        return next(arg for arg in vals if arg is not None, None)
 
 
 Digest: TypeAlias = str
 """Hash digest of an :class:`Entry`, as a string."""
 
 EntryMeta: TypeAlias = TypeVar("EntryMeta", bound=dict)
-"""Type annotation for the metadata dictionary in Entry. 
+"""Type annotation for the metadata dictionary in Entry.
 
 Import formats can define their own institution specific metadata type if they want
 users to be able to benefit from autocomplete, and things like that."""
 
 
 @dataclasses.dataclass
 class Entry(Generic[EntryMeta]):
@@ -77,20 +77,20 @@
     abstraction well-suited for transactions from bank accounts or credit cards. It
     is less applicable to model transactions involving investments or salary.
     """
 
     digest: Digest
     """
     Computed digest of this entry.
-    
+
     Some banks / data sources do not provide a reliable number / ID for
     a given entry (in e.g. a CSV file). Therefore, implementors of this class
     will have to provide a way to compute a digest.
-   
-    This digest is used when storing the user's manual edits. See also 
+
+    This digest is used when storing the user's manual edits. See also
     :py:mod:`roastery.edit`.
     """
 
     date: datetime.date
     """Booking date of the entry."""
 
     amount: data.Amount
@@ -106,43 +106,43 @@
     """Payee to add to this transaction. For example: ``Rob de Wit``."""
 
     narration: Cleanable
     """Narration to add to this transaction. For example: `Settle the tab at 't Neutje.`"""
 
     meta: EntryMeta = dataclasses.field(default_factory=dict)
     """
-    Dictionary of arbitrary data to attach to the transaction. 
-    
+    Dictionary of arbitrary data to attach to the transaction.
+
     Users can instantiate Entry with a :py:obj:`TypedDict` to get type safety for any extra
     fields they might want to store.
     """
 
     tags: set[str] = dataclasses.field(default_factory=set)
     """
     Set of arbitrary strings to tag this transaction with.
-    
+
     See https://beancount.github.io/docs/beancount_language_syntax.html#tags
     """
 
     links: set[str] = dataclasses.field(default_factory=set)
     """
     Set of arbitrary strings to link this transaction with.
-    
+
     See https://beancount.github.io/docs/beancount_language_syntax.html#tags
     """
 
     flag: str = "*"
     """
     One of the strings ``*`` or ``!``.
-   
-    ``*`` 
-      denotes a 'normal' transaction. 
-      
-    ``!`` 
-      means there is something special / that requires attention about this entry. ``!`` transactions 
+
+    ``*``
+      denotes a 'normal' transaction.
+
+    ``!``
+      means there is something special / that requires attention about this entry. ``!`` transactions
       are highlighted in red in Fava.
     """
 
     @classmethod
     def from_row(
         cls,
         *,
@@ -221,18 +221,18 @@
 
 For example:
 
 .. code-block:: python
 
    def my_clean(entry: Entry) -> None:
        payee = entry.payee.lower()
-      
+
        if payee == "irs":
            entry.account.cleaned = "Expenses:Tax"
-           
+
        elif payee in {"chipotle", "mcdonalds", "five guys"}:
            entry.account.cleaned = "Expenses:FastFood"
 """
 
 
 ExtractFn: TypeAlias = Callable[[dict], Entry]
 """Turns a row of CSV data into an :py:class:`Entry`."""
```

### Comparing `roastery-0.20240531.dev1/src/roastery/term.py` & `roastery-0.20240603.dev0/src/roastery/term.py`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/LICENSE` & `roastery-0.20240603.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/README.md` & `roastery-0.20240603.dev0/README.md`

 * *Files identical despite different names*

### Comparing `roastery-0.20240531.dev1/pyproject.toml` & `roastery-0.20240603.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "roastery"
-version = "0.20240531-dev1"
+version = "0.20240603-dev"
 dependencies = [
     "beancount>=2.0.0",
     "typer>=0.12.0",
     "fava>=1.27.0",
     "prompt-toolkit>=3.0.0",
 ]
 authors = [
```

### Comparing `roastery-0.20240531.dev1/PKG-INFO` & `roastery-0.20240603.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: roastery
-Version: 0.20240531.dev1
+Version: 0.20240603.dev0
 Summary: Framework for Beancount plain text accounting
 Author-email: Laurens Duijvesteijn <git@duijf.io>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: beancount>=2.0.0
 Requires-Dist: fava>=1.27.0
 Requires-Dist: prompt-toolkit>=3.0.0
```

