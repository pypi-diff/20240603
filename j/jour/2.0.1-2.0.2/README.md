# Comparing `tmp/jour-2.0.1.tar.gz` & `tmp/jour-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jour-2.0.1.tar", max compression
+gzip compressed data, was "jour-2.0.2.tar", max compression
```

## Comparing `jour-2.0.1.tar` & `jour-2.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35082 2024-03-16 23:44:16.798479 jour-2.0.1/LICENSE
--rw-r--r--   0        0        0     2953 2024-03-16 23:44:16.798879 jour-2.0.1/README.md
--rw-r--r--   0        0        0        0 2024-03-16 23:44:16.799017 jour-2.0.1/jour/__init__.py
--rw-r--r--   0        0        0     4483 2024-03-16 23:44:16.799319 jour-2.0.1/jour/__main__.py
--rw-r--r--   0        0        0    12744 2024-03-17 11:15:34.100683 jour-2.0.1/jour/jour.py
--rw-r--r--   0        0        0     2905 2024-03-17 11:15:34.100980 jour-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3963 1970-01-01 00:00:00.000000 jour-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35082 2024-03-16 23:44:16.798479 jour-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3366 2024-06-03 13:50:15.740255 jour-2.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-16 23:44:16.799017 jour-2.0.2/jour/__init__.py
+-rw-r--r--   0        0        0     4503 2024-06-03 13:50:15.740592 jour-2.0.2/jour/__main__.py
+-rw-r--r--   0        0        0    12746 2024-06-03 13:50:15.740900 jour-2.0.2/jour/jour.py
+-rw-r--r--   0        0        0     2905 2024-06-03 13:52:40.394353 jour-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 jour-2.0.2/PKG-INFO
```

### Comparing `jour-2.0.1/LICENSE` & `jour-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jour-2.0.1/README.md` & `jour-2.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 # Jour
 
 This repository contains the Jour tool, an utility for a high-level machine maintenance journal. The final purpose of this tool is to write and handle a journal in which the user or some automated process can write and tag the performed actions related with the machine configuration, maintenance, and other relevant information. This way, the user can keep track of the changes and the performed actions, and also can obtain a high-level overview of the machine status over time.
 
 Some examples of the usage of this tool could be:
 
-1. Write a journal to keep track of an operating system update you just ran:
+1. Write a journal entry to register an OS update. Just run the following command in the terminal:
 
 ```sh
-jw -w 'OS update to 24.5.2'
+jour --write 'OS update to 24.5.2'
 ```
 
 Output:
 
 ```
 0014. 2024-03-16 17:04:50,123 - test_username - OS update to 24.5.2.
 ```
 
-2. Write a journal entry about a backup of the machine. Use a tag.
+2. Write a journal entry about a backup of the machine. Use a Jour tag.
 
 ```sh
-jw -w 'General system backup' && w -t BUP
+jour --write 'General system backup' && jour --tag 'BUP'
 ```
 
 Output:
 
 ```
 0015. 2024-03-16 17:06:08,630 - test_username - General system backup. #BUP1
 ```
 
-You could then use this same tag `BUP1` to also tag a commit in a Git repository with your machine config. This way your journal and your machine config are paired.
+3. Register other backup some time later. Use the same tag. Take into account that the tag index is automatically incremented, like the entry index.
+
+```sh
+jour --write 'General system backup' && jour --tag 'BUP'
+```
+
+Output:
+
+```
+0016. 2024-03-16 17:09:14,123 - test_username - General system backup. #BUP2
+```
+
+You could then use these same tags `BUP1`, `BUP2`, etc. to also tag a commit in a Git repository with your machine config or dotfiles. This way your Jour journal and your machine config are paired.
 
 ### The journal file
 
-Basically, each new journal entry is a new line in the journal file, with an index and a date. The index is useful to cross-reference the journal entries. The entries are appended to the journal file sequentially. The journal file location is defined in the environment variable `$JOURNAL` (or, by default in `~/.journal.md`). If the tool cannot reach the file, the incoming entries are stored in an emergency journal file, which location is `$JOURNAL_EMERGENCY`, if defined, or `~/.journal_emergency.md`, otherwise. This is useful if, for example, the journal file is located in a remote file system or cloud provider and the connection is lost. The user can then manually arrange the journal entries merging the emergency journal.
+Basically, each new journal entry is a new line in the journal file, with an index and a date. The index is useful to cross-reference the journal entries. The entries are appended to the journal file sequentially. The journal file location is defined in the environment variable `$JOURNAL` (or, by default in `~/journal.md`). If the tool cannot reach the file, the incoming entries are stored in an emergency journal file, which location is `$JOURNAL_EMERGENCY`, if defined, or `~/journal_emergency.md`, otherwise. This is useful if, for example, the journal file is located in a remote file system or cloud provider and the connection is lost. The user can then manually arrange the journal entries merging the emergency journal.
 
-In addition to the entries, the tool also handle tags, like `#backup1`, to an easier navigation of the journal file. This is specially useful to link the journal entries with tags in a configuration Git repository, for example, because a journal tag can be also set in the repo.
+In addition to the entries, like explained before, the tool also handle tags, like `#BUP1`, to an easier navigation of the journal file. This is specially useful to link the journal entries with tags in a configuration Git repository, for example, because a journal tag can be also set in the repo.
 
 Journal format is Markdown, so the user can also export all the history to a more readable format, like a PDF, using a Markdown to PDF converter.
 
 After some time, the user can obtain with Jour a high-level traceability of the machine changes and fixes, helping even to debug some issues or roll back to a previous state.
 
 ## Installation
```

### Comparing `jour-2.0.1/jour/__main__.py` & `jour-2.0.2/jour/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Main
 ====
 
-This module is the main entry point for the `jw` command line utility. It uses the
+This module is the main entry point for the `jour` command line utility. It uses the
 `argparse` module to parse the command line arguments and the `Jour` class
 to access the functionality.
 """
 
 import argparse
 import logging
 
@@ -23,15 +23,15 @@
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
 
 def parse_args():
     # Define the parser
     parser = argparse.ArgumentParser(
-        prog="jw",
+        prog="jour",
         description="An utility for a high-level machine maintenance journal. Uses the file defined in `JOURNAL` environment variable as the journal file location",
         epilog="© Borja González Seoane",
     )
 
     group = parser.add_mutually_exclusive_group(required=False)
     group.add_argument(
         "--print",
@@ -127,37 +127,37 @@
 
     # Check that a tag is provided when the `--tag` or `--return_tag` options are used
     if (args.tag or args.return_tag) and args.MESSAGE_OR_TAG is None:
         logger.error("No tag to add.")
         return
 
     # Create a `Jour` object
-    jw = Jour(create_journal=args.create_journal)
+    jour = Jour(create_journal=args.create_journal)
 
     # Enter context an run the command
-    with jw:
+    with jour:
         if args.write:
-            jw.write_line(
+            jour.write_line(
                 args.MESSAGE_OR_TAG,
                 as_command=args.as_command,
                 signature=args.signature,
                 printing=True,
             )
         elif args.append:
-            jw.append_to_last_line(
+            jour.append_to_last_line(
                 args.MESSAGE_OR_TAG, as_command=args.as_command, printing=True
             )
         elif args.tag:
-            jw.tag_last_line(args.MESSAGE_OR_TAG, printing=True)
+            jour.tag_last_line(args.MESSAGE_OR_TAG, printing=True)
 
         elif args.return_tag:
-            jw.get_next_tag(args.MESSAGE_OR_TAG, printing=True)
+            jour.get_next_tag(args.MESSAGE_OR_TAG, printing=True)
 
         elif args.remove:
-            jw.remove_last_line()
+            jour.remove_last_line()
 
         else:  # Default
-            jw.print_journal()
+            jour.print_journal()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jour-2.0.1/jour/jour.py` & `jour-2.0.2/jour/jour.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         Enter the context manager to get a lock over the journal file.
         """
         logger.debug(
             f"Using journal file: `{self._active_journal_file}`..."
         )  # Debug level
 
         self._journal_lock = ILock(
-            f"jw_lock_{self._active_journal_file.name}", reentrant=True, timeout=10
+            f"jour_lock_{self._active_journal_file.name}", reentrant=True, timeout=10
         )
         with self._journal_lock:
             # Load the journal file to memory
             with open(self._active_journal_file, "r") as f:
                 self._journal = f.readlines()
 
         return self
```

### Comparing `jour-2.0.1/pyproject.toml` & `jour-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     "machine-maintenance",
     "markdown",
 ]
 license = "LICENSE"
 name = "jour"
 readme = "README.md"
 repository = "https://github.com/bglezseoane/jour"
-version = "2.0.1"
+version = "2.0.2"
 
 [tool.poetry.dependencies]
 ilock = "^1.0.3"
 mdformat = "^0.7.17"
 python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `jour-2.0.1/PKG-INFO` & `jour-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jour
-Version: 2.0.1
+Version: 2.0.2
 Summary: An utility for a high-level machine maintenance journal
 Home-page: https://github.com/bglezseoane/jour
 License: LICENSE
 Keywords: configuration,journal,journaling,machine-administration,machine-maintenance,markdown
 Author: Borja González Seoane
 Author-email: borja@glezseoane.es
 Requires-Python: >=3.11,<4.0
@@ -25,45 +25,57 @@
 
 # Jour
 
 This repository contains the Jour tool, an utility for a high-level machine maintenance journal. The final purpose of this tool is to write and handle a journal in which the user or some automated process can write and tag the performed actions related with the machine configuration, maintenance, and other relevant information. This way, the user can keep track of the changes and the performed actions, and also can obtain a high-level overview of the machine status over time.
 
 Some examples of the usage of this tool could be:
 
-1. Write a journal to keep track of an operating system update you just ran:
+1. Write a journal entry to register an OS update. Just run the following command in the terminal:
 
 ```sh
-jw -w 'OS update to 24.5.2'
+jour --write 'OS update to 24.5.2'
 ```
 
 Output:
 
 ```
 0014. 2024-03-16 17:04:50,123 - test_username - OS update to 24.5.2.
 ```
 
-2. Write a journal entry about a backup of the machine. Use a tag.
+2. Write a journal entry about a backup of the machine. Use a Jour tag.
 
 ```sh
-jw -w 'General system backup' && w -t BUP
+jour --write 'General system backup' && jour --tag 'BUP'
 ```
 
 Output:
 
 ```
 0015. 2024-03-16 17:06:08,630 - test_username - General system backup. #BUP1
 ```
 
-You could then use this same tag `BUP1` to also tag a commit in a Git repository with your machine config. This way your journal and your machine config are paired.
+3. Register other backup some time later. Use the same tag. Take into account that the tag index is automatically incremented, like the entry index.
+
+```sh
+jour --write 'General system backup' && jour --tag 'BUP'
+```
+
+Output:
+
+```
+0016. 2024-03-16 17:09:14,123 - test_username - General system backup. #BUP2
+```
+
+You could then use these same tags `BUP1`, `BUP2`, etc. to also tag a commit in a Git repository with your machine config or dotfiles. This way your Jour journal and your machine config are paired.
 
 ### The journal file
 
-Basically, each new journal entry is a new line in the journal file, with an index and a date. The index is useful to cross-reference the journal entries. The entries are appended to the journal file sequentially. The journal file location is defined in the environment variable `$JOURNAL` (or, by default in `~/.journal.md`). If the tool cannot reach the file, the incoming entries are stored in an emergency journal file, which location is `$JOURNAL_EMERGENCY`, if defined, or `~/.journal_emergency.md`, otherwise. This is useful if, for example, the journal file is located in a remote file system or cloud provider and the connection is lost. The user can then manually arrange the journal entries merging the emergency journal.
+Basically, each new journal entry is a new line in the journal file, with an index and a date. The index is useful to cross-reference the journal entries. The entries are appended to the journal file sequentially. The journal file location is defined in the environment variable `$JOURNAL` (or, by default in `~/journal.md`). If the tool cannot reach the file, the incoming entries are stored in an emergency journal file, which location is `$JOURNAL_EMERGENCY`, if defined, or `~/journal_emergency.md`, otherwise. This is useful if, for example, the journal file is located in a remote file system or cloud provider and the connection is lost. The user can then manually arrange the journal entries merging the emergency journal.
 
-In addition to the entries, the tool also handle tags, like `#backup1`, to an easier navigation of the journal file. This is specially useful to link the journal entries with tags in a configuration Git repository, for example, because a journal tag can be also set in the repo.
+In addition to the entries, like explained before, the tool also handle tags, like `#BUP1`, to an easier navigation of the journal file. This is specially useful to link the journal entries with tags in a configuration Git repository, for example, because a journal tag can be also set in the repo.
 
 Journal format is Markdown, so the user can also export all the history to a more readable format, like a PDF, using a Markdown to PDF converter.
 
 After some time, the user can obtain with Jour a high-level traceability of the machine changes and fixes, helping even to debug some issues or roll back to a previous state.
 
 ## Installation
```

