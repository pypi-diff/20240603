# Comparing `tmp/menuchoice-0.5.tar.gz` & `tmp/menuchoice-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menuchoice-0.5.tar", last modified: Sat Jun  1 09:34:17 2024, max compression
+gzip compressed data, was "menuchoice-0.6.tar", last modified: Mon Jun  3 04:01:22 2024, max compression
```

## Comparing `menuchoice-0.5.tar` & `menuchoice-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-06-01 09:34:17.952098 menuchoice-0.5/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1055 2024-05-12 03:45:48.000000 menuchoice-0.5/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/menuchoice/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     5408 2024-06-01 09:34:13.000000 menuchoice-0.5/menuchoice/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.5/menuchoice/_validator.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/menuchoice/cursor_control/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     7257 2024-06-01 03:47:37.000000 menuchoice-0.5/menuchoice/cursor_control/_cursorInput.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      882 2024-05-14 10:44:56.000000 menuchoice-0.5/menuchoice/cursor_control/_textHandler.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.5/menuchoice/exceptions.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 09:34:17.952098 menuchoice-0.5/menuchoice.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      311 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-06-01 09:34:17.000000 menuchoice-0.5/menuchoice.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-06-01 09:34:17.952098 menuchoice-0.5/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1078 2024-05-16 03:44:34.000000 menuchoice-0.5/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-03 04:01:22.863404 menuchoice-0.6/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-06-03 04:01:22.863404 menuchoice-0.6/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1055 2024-05-12 03:45:48.000000 menuchoice-0.6/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-03 04:01:22.863404 menuchoice-0.6/menuchoice/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5429 2024-06-03 03:37:16.000000 menuchoice-0.6/menuchoice/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      643 2024-05-10 05:16:56.000000 menuchoice-0.6/menuchoice/_validator.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-03 04:01:22.863404 menuchoice-0.6/menuchoice/cursor_control/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     7462 2024-06-03 02:46:11.000000 menuchoice-0.6/menuchoice/cursor_control/_cursorInput.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      882 2024-05-14 10:44:56.000000 menuchoice-0.6/menuchoice/cursor_control/_textHandler.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      142 2024-05-10 03:13:36.000000 menuchoice-0.6/menuchoice/exceptions.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-03 04:01:22.863404 menuchoice-0.6/menuchoice.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1844 2024-06-03 04:01:22.000000 menuchoice-0.6/menuchoice.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      311 2024-06-03 04:01:22.000000 menuchoice-0.6/menuchoice.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-06-03 04:01:22.000000 menuchoice-0.6/menuchoice.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       11 2024-06-03 04:01:22.000000 menuchoice-0.6/menuchoice.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-06-03 04:01:22.863404 menuchoice-0.6/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1078 2024-05-16 03:44:34.000000 menuchoice-0.6/setup.py
```

### Comparing `menuchoice-0.5/PKG-INFO` & `menuchoice-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.5
+Version: 0.6
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `menuchoice-0.5/README.md` & `menuchoice-0.6/README.md`

 * *Files identical despite different names*

### Comparing `menuchoice-0.5/menuchoice/__init__.py` & `menuchoice-0.6/menuchoice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import curses
 import re
 from .cursor_control import _cursorInput
 from .exceptions import *
 from . import _validator
 
-__version__ = "0.5"
+__version__ = "0.6"
 __author__ = "xyzpw"
 __description__ = "Command line menu selector."
 __license__ = "MIT"
 
 class MenuSelector:
     """Contains items which can be prompted via a menu selector."""
     def __init__(self, items: list | dict, title: str = None, description: str = None):
@@ -76,15 +76,15 @@
         menu = self.createMenuString(num_sep, align)
         if max_items[1] > 1 if max_items[1] != None else True:
             selectedIndexes = curses.wrapper(_cursorInput.cursorArrowMultiselectMenu, menu, max_items[1], allow_all, center)
             usrChoices = [(i, list(self.items)[i]) for i in selectedIndexes] if selectedIndexes != None else []
         else:
             selectedIndexes = curses.wrapper(_cursorInput.cursorArrowMenu, menu, arrow, center)
             usrChoices = [(selectedIndexes, list(self.items)[selectedIndexes])] if selectedIndexes != None else []
-        if not _validator.validateItemSelectionCount(max_items, usrChoices):
+        if not _validator.validateItemSelectionCount(max_items, usrChoices) and bool(usrChoices):
             raise MenuItemError("number of items selected is out of range")
         return usrChoices
     def highlight_select(self, center: bool = False):
         """Highlights the options at the current line index.
 
         :param center: positions the menu selector to the center of the terminal"""
         menuComponents = self.items, self.title, self.description
```

### Comparing `menuchoice-0.5/menuchoice/_validator.py` & `menuchoice-0.6/menuchoice/_validator.py`

 * *Files identical despite different names*

### Comparing `menuchoice-0.5/menuchoice/cursor_control/_cursorInput.py` & `menuchoice-0.6/menuchoice/cursor_control/_cursorInput.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import curses
 import re
 import shutil
 from . import _textHandler
 
+KEYS_QUIT = [ord("q"), ord("Q")]
+
 def getMenuComponents(menuString: str):
     menuLines = menuString.splitlines()
     for l in range(len(menuLines)):
         if re.search(r"^0.\s.*?(?=$|\s)", menuLines[l]) != None:
             meta = menuLines[:l] if l != 0 else None
             menuLines = menuLines[l:]
             break
@@ -44,14 +46,16 @@
             nextLineIndex = currentLineIndex - 1
             currentLineIndex = nextLineIndex if currentLineIndex > 0 else len(menuLines) - 1
         elif keyPressed == curses.KEY_DOWN:
             nextLineIndex = currentLineIndex + 1
             currentLineIndex = nextLineIndex if currentLineIndex < len(menuLines) - 1 else 0
         elif keyPressed in [curses.KEY_ENTER, 10]:
             return currentLineIndex
+        elif keyPressed in KEYS_QUIT:
+            return
 
 def rewriteMultiselectMenu(menuString: str, currentMenuLine: int, selectedItems: list, allowAll: bool = False):
     menuLines = getMenuComponents(menuString)[0]
     for i in range(len(menuLines)):
         selectionStatusCharacter = "\u25cf" if i in selectedItems else "\u25cb"
         if i == len(menuLines) - 1:
             menuLines[i] = "  %s" % menuLines[i] if currentMenuLine != i else "* %s" % menuLines[i]
@@ -118,14 +122,16 @@
                 continue
             if currentLineIndex == len(menuLines) - 1:
                 return selectedItems if bool(selectedItems) else None
             else:
                 if currentLineIndex not in selectedItems and (maxItemCount <= len(selectedItems) if maxItemCount != None else False):
                     continue
                 selectedItems.append(currentLineIndex) if not currentLineIndex in selectedItems else selectedItems.pop(selectedItems.index(currentLineIndex))
+        elif keyPressed in KEYS_QUIT:
+            return
 
 
 def highlightSelectMenu(stdscr, menuComponents: tuple, center: bool = False):
     curses.curs_set(0)
     curses.use_default_colors()
     currentLineIndex = 0
     menuLines: list = menuComponents[0]
@@ -149,7 +155,9 @@
         keyPressed = stdscr.getch()
         if keyPressed == curses.KEY_DOWN:
             currentLineIndex = currentLineIndex + 1 if currentLineIndex != len(menuLines) - 1 else 0
         elif keyPressed == curses.KEY_UP:
             currentLineIndex = currentLineIndex - 1 if currentLineIndex != 0 else len(menuLines) - 1
         elif keyPressed in [curses.KEY_ENTER, 10]:
             return currentLineIndex
+        elif keyPressed in KEYS_QUIT:
+            return
```

### Comparing `menuchoice-0.5/menuchoice/cursor_control/_textHandler.py` & `menuchoice-0.6/menuchoice/cursor_control/_textHandler.py`

 * *Files identical despite different names*

### Comparing `menuchoice-0.5/menuchoice.egg-info/PKG-INFO` & `menuchoice-0.6/menuchoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menuchoice
-Version: 0.5
+Version: 0.6
 Summary: Command line menu selector.
 Home-page: https://github.com/xyzpw/menuchoice/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: menu selector,item selector,ansi
 Classifier: Programming Language :: Python :: 3
```

### Comparing `menuchoice-0.5/setup.py` & `menuchoice-0.6/setup.py`

 * *Files identical despite different names*

