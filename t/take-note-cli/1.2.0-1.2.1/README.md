# Comparing `tmp/take_note_cli-1.2.0.tar.gz` & `tmp/take_note_cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "take_note_cli-1.2.0.tar", max compression
+gzip compressed data, was "take_note_cli-1.2.1.tar", max compression
```

## Comparing `take_note_cli-1.2.0.tar` & `take_note_cli-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-12-11 14:50:23.598793 take_note_cli-1.2.0/LICENSE
--rw-r--r--   0        0        0     4036 2023-12-11 14:50:23.598793 take_note_cli-1.2.0/README.md
--rw-r--r--   0        0        0     1103 2024-01-20 17:13:47.340583 take_note_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-20 16:53:29.139902 take_note_cli-1.2.0/src/take_note_cli/__init__.py
--rw-r--r--   0        0        0      131 2024-01-20 16:41:03.050207 take_note_cli-1.2.0/src/take_note_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-12-11 14:50:23.599793 take_note_cli-1.2.0/src/take_note_cli/core/__init__.py
--rw-r--r--   0        0        0     2888 2024-01-20 16:43:08.331184 take_note_cli-1.2.0/src/take_note_cli/core/notes.py
--rw-r--r--   0        0        0        0 2023-12-11 14:50:23.599793 take_note_cli-1.2.0/src/take_note_cli/utils/__init__.py
--rw-r--r--   0        0        0     2563 2024-01-20 16:42:47.227683 take_note_cli-1.2.0/src/take_note_cli/utils/args.py
--rw-r--r--   0        0        0      682 2024-01-20 15:41:52.983047 take_note_cli-1.2.0/src/take_note_cli/utils/dates.py
--rw-r--r--   0        0        0      421 2024-01-20 08:01:53.550491 take_note_cli-1.2.0/src/take_note_cli/utils/paths.py
--rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 take_note_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-12-11 14:50:23.598793 take_note_cli-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3758 2024-06-03 13:53:23.602260 take_note_cli-1.2.1/README.md
+-rw-r--r--   0        0        0     1103 2024-06-03 13:43:55.878356 take_note_cli-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-20 16:53:29.139902 take_note_cli-1.2.1/src/take_note_cli/__init__.py
+-rw-r--r--   0        0        0      131 2024-01-20 16:41:03.050207 take_note_cli-1.2.1/src/take_note_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-12-11 14:50:23.599793 take_note_cli-1.2.1/src/take_note_cli/core/__init__.py
+-rw-r--r--   0        0        0     2888 2024-01-20 16:43:08.331184 take_note_cli-1.2.1/src/take_note_cli/core/notes.py
+-rw-r--r--   0        0        0        0 2023-12-11 14:50:23.599793 take_note_cli-1.2.1/src/take_note_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2563 2024-01-20 16:42:47.227683 take_note_cli-1.2.1/src/take_note_cli/utils/args.py
+-rw-r--r--   0        0        0      682 2024-01-20 15:41:52.983047 take_note_cli-1.2.1/src/take_note_cli/utils/dates.py
+-rw-r--r--   0        0        0      421 2024-01-20 08:01:53.550491 take_note_cli-1.2.1/src/take_note_cli/utils/paths.py
+-rw-r--r--   0        0        0     4753 1970-01-01 00:00:00.000000 take_note_cli-1.2.1/PKG-INFO
```

### Comparing `take_note_cli-1.2.0/LICENSE` & `take_note_cli-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `take_note_cli-1.2.0/pyproject.toml` & `take_note_cli-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "take-note-cli"
-version = "1.2.0"
+version = "1.2.1"
 description = "Create and open notes in your favourite editor."
 license = "MIT"
 authors = [
   "wsinned <wsinned@tutanota.com>",
 ]
 readme = "README.md"
 homepage = "https://github.com/wsinned/take-note"
```

### Comparing `take_note_cli-1.2.0/src/take_note_cli/core/notes.py` & `take_note_cli-1.2.1/src/take_note_cli/core/notes.py`

 * *Files identical despite different names*

### Comparing `take_note_cli-1.2.0/src/take_note_cli/utils/args.py` & `take_note_cli-1.2.1/src/take_note_cli/utils/args.py`

 * *Files identical despite different names*

### Comparing `take_note_cli-1.2.0/src/take_note_cli/utils/dates.py` & `take_note_cli-1.2.1/src/take_note_cli/utils/dates.py`

 * *Files identical despite different names*

### Comparing `take_note_cli-1.2.0/PKG-INFO` & `take_note_cli-1.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: take-note-cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: Create and open notes in your favourite editor.
 Home-page: https://github.com/wsinned/take-note
 License: MIT
 Keywords: note,tool,utility,cli
 Author: wsinned
 Author-email: wsinned@tutanota.com
 Requires-Python: >=3.8,<4.0
@@ -31,14 +31,15 @@
 ## Features
 
 - Written in Python with no runtime dependencies.
   - Works on Python 3.8 - 3.11.
 - Open notes files for specified week using the `code` command line for VS Code.
   - --thisWeek, --lastWeek and --nextWeek are supported.
 - Organises notes in a date based folder structure from your root notes folder, e.g. 2023/08
+  - The default folder is $HOME/Notes
   - set the root notes folder using --notesFolder
 - Choose which editor to use with --editor
 - Specify a VS Code workspace to open along with the note file with --workspace
   - This will override the --editor setting to `code`
 - Specify a template file relative to the root notes folder to use when a new file is created using --template. This also performs a simple replacement of the text HEADER_DATE with the date formatted as "%A %d %B %Y" to use in the document title.
 - Support for batch creation of files in advance. This is useful if you use a device where you can edit files, but can't easily create them. Use --batch 5 along with any of the --*Week options to create that week and the following 4 weeks too.
 
@@ -74,20 +75,19 @@
 A note will be created in the under the MyNotes/YYYY/mm folder named with the date of the Monday of this week, e.g. 2023-08-07-Weekly-log.md
 
 ### Aliases
 
 Setting up aliases in you preferred shell is a great way to make accessing your notes quick and easy.
 
 ```bash
-notes_folder="$HOME/SomePath/MyNotes"
-args="--notesFolder $notes_folder --workspace notes.code-workspace --template Home-weekly-log-template.md"
+NOTES_FOLDER="$HOME/SomePath/MyNotes"
 
-alias thisWeek="take-note --thisWeek $args"
-alias nextWeek="take-note --nextWeek $args"
-alias lastWeek="take-note --lastWeek $args"
+alias thisWeek="take-note --thisWeek --notesFolder $NOTES_FOLDER --workspace notes.code-workspace"
+alias nextWeek="take-note --nextWeek --notesFolder $NOTES_FOLDER --workspace notes.code-workspace --batch 5"
+alias lastWeek="take-note --lastWeek --editor hx"
 ```
 
 All you have to do now is type one of the following to open the desired note file.
 
 ```bash
 > thisWeek
 > lastWeek
@@ -112,73 +112,58 @@
 
 ## Development
 
 ### Nix & NixOS
 
 The supplied shell.nix definition provides support for entering a nix-shell directly in the repository with all dependencies.
 
-```zsh
+```bash
 nix-shell --run zsh # ensure using zsh over default bash session
-
-# only needed once, or to recreate the virtual environment
-python -m venv venv 
-
-source venv/bin/activate
-
-# install with tests as editable src
-venv/bin/pip install -e '.[test]'
-
-# run the tests
-pytest
-
-# close the virtual environment and exit the shell when done
-deactivate
-exit
 ```
 
+Then follow the instructions for other OS.
+
 ### Other Linux or macOS
 
-```zsh
+```bash
 # only needed once, or to recreate the virtual environment
-python -m venv venv 
-
-source venv/bin/activate
-
-venv/bin/pip install -r requirements.txt -r requirements.dev.txt
+# install dependencies
+poetry install
 
-# install with tests as editable src
-venv/bin/pip install -e '.[test]'
+# enter an activated shell and run tests
+poetry shell
+pytest
+ruff . --config pyproject.toml
 
-# run the tests
-venv/bin/pytest
+# run the tests without activating a shell
+poetry run pytest
 
-# close the virtual environment when done
-deactivate
+# exit the shell
+exit
 ```
 
 ## Linting
 
 The project uses [ruff](https://github.com/charliermarsh/ruff) for linting and optionally for formatting.
 
 ```bash
-venv/bin/ruff . --config pyproject.toml
+poetry run ruff . --config pyproject.toml
 ```
 
 ## Build & Publish
 
 From an installed and tested venv, do the following:
 
-```bash
-# check the version:
-cat src/takenote/__version__.py
+Bump the version inpyproject.tom
 
+```bash
 # build the package
-venv/bin/pyproject-build
+poetry build
 
 # publish the package
-venv/bin/twine upload dist/*
+poetry publish
 ```
 
 Credentials for twine should be either:
     - stored in .pypirc in the [pypi] section
     - entered at the prompt, username = **token** and password = your_api_key
```

