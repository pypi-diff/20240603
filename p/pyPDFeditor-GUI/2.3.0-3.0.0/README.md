# Comparing `tmp/pyPDFeditor-GUI-2.3.0.tar.gz` & `tmp/pypdfeditor_gui-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPDFeditor-GUI-2.3.0.tar", last modified: Mon Dec 18 14:32:27 2023, max compression
+gzip compressed data, was "pypdfeditor_gui-3.0.0.tar", last modified: Mon Jun  3 14:52:08 2024, max compression
```

## Comparing `pyPDFeditor-GUI-2.3.0.tar` & `pypdfeditor_gui-3.0.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-12-18 14:32:27.923349 pyPDFeditor-GUI-2.3.0/
--rw-rw-rw-   0        0        0     1091 2021-12-24 11:43:24.000000 pyPDFeditor-GUI-2.3.0/LICENSE
--rw-rw-rw-   0        0        0     5189 2023-12-18 14:32:27.923349 pyPDFeditor-GUI-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2022-09-27 08:35:21.000000 pyPDFeditor-GUI-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-18 14:32:27.922444 pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/
--rw-rw-rw-   0        0        0     5189 2023-12-18 14:32:27.000000 pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2296 2023-12-18 14:32:27.000000 pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-18 14:32:27.000000 pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-12-18 14:32:27.000000 pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-12-18 14:32:27.000000 pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-12-18 14:32:27.000000 pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-18 14:32:27.852873 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/
--rw-rw-rw-   0        0        0     1335 2023-12-18 13:18:07.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/__init__.py
--rw-rw-rw-   0        0        0      965 2023-12-16 12:49:32.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/__main__.py
--rw-rw-rw-   0        0        0    25002 2023-12-18 14:19:29.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/application.py
--rw-rw-rw-   0        0        0    24497 2023-12-18 13:28:42.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/functions.py
-drwxrwxrwx   0        0        0        0 2023-12-18 14:32:27.917434 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/
--rw-rw-rw-   0        0        0      372 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/Add.svg
--rw-rw-rw-   0        0        0      375 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/Add_h.svg
--rw-rw-rw-   0        0        0      375 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/Add_p.svg
--rw-rw-rw-   0        0        0      698 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/Photo.svg
--rw-rw-rw-   0        0        0      198 2022-06-11 07:19:38.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/__init__.py
--rw-rw-rw-   0        0        0      714 2022-06-11 07:24:52.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/arrow_move.svg
--rw-rw-rw-   0        0        0     4680 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/book2.svg
--rw-rw-rw-   0        0        0      422 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/chevron_down.svg
--rw-rw-rw-   0        0        0     1115 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/color.svg
--rw-rw-rw-   0        0        0     1117 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/color_h.svg
--rw-rw-rw-   0        0        0      798 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/color_p.svg
--rw-rw-rw-   0        0        0     1648 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/delete.svg
--rw-rw-rw-   0        0        0     1651 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/delete_h.svg
--rw-rw-rw-   0        0        0     1651 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/delete_p.svg
--rw-rw-rw-   0        0        0      407 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/dismiss.svg
--rw-rw-rw-   0        0        0      410 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/dismiss_h.svg
--rw-rw-rw-   0        0        0      694 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/down.svg
--rw-rw-rw-   0        0        0      697 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/down_h.svg
--rw-rw-rw-   0        0        0      697 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/down_p.svg
--rw-rw-rw-   0        0        0      740 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/edit.svg
--rw-rw-rw-   0        0        0     1068 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder.svg
--rw-rw-rw-   0        0        0     1069 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder_d.svg
--rw-rw-rw-   0        0        0     1068 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder_h.svg
--rw-rw-rw-   0        0        0     1068 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder_p.svg
--rw-rw-rw-   0        0        0      575 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/font.svg
--rw-rw-rw-   0        0        0      578 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/font_h.svg
--rw-rw-rw-   0        0        0      578 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/font_p.svg
--rw-rw-rw-   0        0        0      681 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/home.svg
--rw-rw-rw-   0        0        0     1721 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/lock.svg
--rw-rw-rw-   0        0        0      375 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/maximize.svg
--rw-rw-rw-   0        0        0      666 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/merge.svg
--rw-rw-rw-   0        0        0      445 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/metadata.svg
--rw-rw-rw-   0        0        0      188 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/minimize.svg
--rw-rw-rw-   0        0        0      612 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more.svg
--rw-rw-rw-   0        0        0      621 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more_d.svg
--rw-rw-rw-   0        0        0      621 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more_h.svg
--rw-rw-rw-   0        0        0      621 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more_p.svg
--rw-rw-rw-   0        0        0      442 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/move_page.svg
--rw-rw-rw-   0        0        0     1338 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/pdf icon.svg
--rw-rw-rw-   0        0        0      407 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/rotate_anticlockwise.svg
--rw-rw-rw-   0        0        0      411 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/rotate_clockwise.svg
--rw-rw-rw-   0        0        0      937 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/settings.svg
--rw-rw-rw-   0        0        0      940 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/settings_h.svg
--rw-rw-rw-   0        0        0      940 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/settings_p.svg
--rw-rw-rw-   0        0        0      561 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/square_multiple.svg
--rw-rw-rw-   0        0        0      569 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/sync.svg
--rw-rw-rw-   0        0        0      572 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/sync_h.svg
--rw-rw-rw-   0        0        0      572 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/sync_p.svg
--rw-rw-rw-   0        0        0      785 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/view.svg
--rw-rw-rw-   0        0        0      788 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/view_h.svg
--rw-rw-rw-   0        0        0      788 2022-01-30 23:37:11.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/view_p.svg
--rw-rw-rw-   0        0        0     8548 2023-12-18 13:30:07.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/language.py
--rw-rw-rw-   0        0        0     7967 2023-12-18 13:34:31.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/style_sheets.py
--rw-rw-rw-   0        0        0     3645 2023-12-18 13:31:29.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/window_effect.py
--rw-rw-rw-   0        0        0    47552 2023-12-18 14:24:17.000000 pyPDFeditor-GUI-2.3.0/pypdfeditor_core/windows.py
--rw-rw-rw-   0        0        0       42 2023-12-18 14:32:27.923349 pyPDFeditor-GUI-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2620 2023-11-10 08:43:27.000000 pyPDFeditor-GUI-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:52:08.294428 pypdfeditor_gui-3.0.0/
+-rw-rw-rw-   0        0        0     1091 2021-12-24 11:43:24.000000 pypdfeditor_gui-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5381 2024-06-03 14:52:08.294428 pypdfeditor_gui-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3990 2024-06-03 13:10:19.000000 pypdfeditor_gui-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 14:52:08.291166 pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/
+-rw-rw-rw-   0        0        0     5381 2024-06-03 14:52:08.000000 pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2296 2024-06-03 14:52:08.000000 pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:52:08.000000 pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-06-03 14:52:08.000000 pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-06-03 14:52:08.000000 pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-06-03 14:52:08.000000 pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 14:52:08.157964 pypdfeditor_gui-3.0.0/pypdfeditor_core/
+-rw-rw-rw-   0        0        0      991 2024-06-03 14:39:00.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/__init__.py
+-rw-rw-rw-   0        0        0      965 2023-12-16 12:49:32.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/__main__.py
+-rw-rw-rw-   0        0        0    25169 2024-06-03 14:50:30.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/application.py
+-rw-rw-rw-   0        0        0    24907 2024-06-03 14:37:27.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/functions.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:52:08.289152 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/
+-rw-rw-rw-   0        0        0      372 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/Add.svg
+-rw-rw-rw-   0        0        0      375 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/Add_h.svg
+-rw-rw-rw-   0        0        0      375 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/Add_p.svg
+-rw-rw-rw-   0        0        0      698 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/Photo.svg
+-rw-rw-rw-   0        0        0      198 2022-06-11 07:19:38.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/__init__.py
+-rw-rw-rw-   0        0        0      714 2022-06-11 07:24:52.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/arrow_move.svg
+-rw-rw-rw-   0        0        0     4680 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/book2.svg
+-rw-rw-rw-   0        0        0      422 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/chevron_down.svg
+-rw-rw-rw-   0        0        0     1115 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/color.svg
+-rw-rw-rw-   0        0        0     1117 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/color_h.svg
+-rw-rw-rw-   0        0        0      798 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/color_p.svg
+-rw-rw-rw-   0        0        0     1648 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/delete.svg
+-rw-rw-rw-   0        0        0     1651 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/delete_h.svg
+-rw-rw-rw-   0        0        0     1651 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/delete_p.svg
+-rw-rw-rw-   0        0        0      407 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/dismiss.svg
+-rw-rw-rw-   0        0        0      410 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/dismiss_h.svg
+-rw-rw-rw-   0        0        0      694 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/down.svg
+-rw-rw-rw-   0        0        0      697 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/down_h.svg
+-rw-rw-rw-   0        0        0      697 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/down_p.svg
+-rw-rw-rw-   0        0        0      740 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/edit.svg
+-rw-rw-rw-   0        0        0     1068 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder.svg
+-rw-rw-rw-   0        0        0     1069 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder_d.svg
+-rw-rw-rw-   0        0        0     1068 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder_h.svg
+-rw-rw-rw-   0        0        0     1068 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder_p.svg
+-rw-rw-rw-   0        0        0      575 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/font.svg
+-rw-rw-rw-   0        0        0      578 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/font_h.svg
+-rw-rw-rw-   0        0        0      578 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/font_p.svg
+-rw-rw-rw-   0        0        0      681 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/home.svg
+-rw-rw-rw-   0        0        0     1721 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/lock.svg
+-rw-rw-rw-   0        0        0      375 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/maximize.svg
+-rw-rw-rw-   0        0        0      666 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/merge.svg
+-rw-rw-rw-   0        0        0      445 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/metadata.svg
+-rw-rw-rw-   0        0        0      188 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/minimize.svg
+-rw-rw-rw-   0        0        0      612 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more.svg
+-rw-rw-rw-   0        0        0      621 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more_d.svg
+-rw-rw-rw-   0        0        0      621 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more_h.svg
+-rw-rw-rw-   0        0        0      621 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more_p.svg
+-rw-rw-rw-   0        0        0      442 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/move_page.svg
+-rw-rw-rw-   0        0        0     1338 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/pdf icon.svg
+-rw-rw-rw-   0        0        0      407 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/rotate_anticlockwise.svg
+-rw-rw-rw-   0        0        0      411 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/rotate_clockwise.svg
+-rw-rw-rw-   0        0        0      937 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/settings.svg
+-rw-rw-rw-   0        0        0      940 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/settings_h.svg
+-rw-rw-rw-   0        0        0      940 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/settings_p.svg
+-rw-rw-rw-   0        0        0      561 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/square_multiple.svg
+-rw-rw-rw-   0        0        0      569 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/sync.svg
+-rw-rw-rw-   0        0        0      572 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/sync_h.svg
+-rw-rw-rw-   0        0        0      572 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/sync_p.svg
+-rw-rw-rw-   0        0        0      785 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/view.svg
+-rw-rw-rw-   0        0        0      788 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/view_h.svg
+-rw-rw-rw-   0        0        0      788 2022-01-30 23:37:11.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/view_p.svg
+-rw-rw-rw-   0        0        0     8847 2024-06-03 06:34:20.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/language.py
+-rw-rw-rw-   0        0        0     7959 2024-06-03 13:32:08.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/style_sheets.py
+-rw-rw-rw-   0        0        0     3645 2023-12-18 13:31:29.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/window_effect.py
+-rw-rw-rw-   0        0        0    50540 2024-06-03 12:56:39.000000 pypdfeditor_gui-3.0.0/pypdfeditor_core/windows.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:52:08.294428 pypdfeditor_gui-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2619 2024-06-03 14:36:41.000000 pypdfeditor_gui-3.0.0/setup.py
```

### Comparing `pyPDFeditor-GUI-2.3.0/LICENSE` & `pypdfeditor_gui-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/PKG-INFO` & `pypdfeditor_gui-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPDFeditor-GUI
-Version: 2.3.0
+Version: 3.0.0
 Summary: A desktop application to edit PDF files.
 Home-page: https://github.com/Augus1999/pyPDFeditor-GUI/
 Author: Nianze A. TAO
 Author-email: Augus_1999@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/Augus1999/pyPDFeditor-GUI
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyMuPDF>=1.19.2
-Requires-Dist: PyQt5>=5.15.4
+Requires-Dist: PyMuPDF>=1.24.3
+Requires-Dist: PyQt6>=6.7.0
 
 # pyPDFeditor-GUI
 
 [![PyPI](https://img.shields.io/pypi/v/pyPDFeditor-GUI?color=5f69b4)](https://pypi.org/project/pyPDFeditor-GUI/)
 [![Downloads](https://static.pepy.tech/personalized-badge/pyPDFeditor-GUI?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/pyPDFeditor-GUI)
 ![pylint](https://github.com/Augus1999/pyPDFeditor-GUI/actions/workflows/pylint.yml/badge.svg)
 
@@ -45,14 +45,19 @@
 
 Welcome to use pyPDFeditor-GUI. pyPDFeditor-GUI is a simple cross-platform application, thanks
 to [Python](https://www.python.org/), [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 and [PyMuPDF](https://github.com/pymupdf/PyMuPDF), designed to work on simple PDF handling.
 
 I tried my best to make it close to Fluent UI. Icons used can be found [🔗here](https://fluenticons.co/).
 
+From version 3.0.0, we have moved the GUI library to PyQt6. If you upgraded from a previous version, you can consider removing PyQt5:
+```bash
+$ pip uninstall PyQt5 PyQt5-Qt5 PyQt5-sip
+```
+
 ## Features
 
 * Support 3 languages: English, 日本語 (Japanese), and 中文 (Traditional Chinese)
 * Fluent UI design
 * Cross-platform support
 * Open-source and free to use under MIT licence
 * Frameless Window on
@@ -77,16 +82,16 @@
 ## Requirements 🧩
 
 ```text
 Python>=3.7
 ```
 
 ```text
-PyQt5>=5.15.4
-PyMuPDF>=1.19.2
+PyQt6>=6.7.0
+PyMuPDF>=1.24.0
 ```
 
 ## Install & Run
 
 ### install from source
 
 you will need `setuptools` and `wheel` installed
```

### Comparing `pyPDFeditor-GUI-2.3.0/README.md` & `pypdfeditor_gui-3.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
 Welcome to use pyPDFeditor-GUI. pyPDFeditor-GUI is a simple cross-platform application, thanks
 to [Python](https://www.python.org/), [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 and [PyMuPDF](https://github.com/pymupdf/PyMuPDF), designed to work on simple PDF handling.
 
 I tried my best to make it close to Fluent UI. Icons used can be found [🔗here](https://fluenticons.co/).
 
+From version 3.0.0, we have moved the GUI library to PyQt6. If you upgraded from a previous version, you can consider removing PyQt5:
+```bash
+$ pip uninstall PyQt5 PyQt5-Qt5 PyQt5-sip
+```
+
 ## Features
 
 * Support 3 languages: English, 日本語 (Japanese), and 中文 (Traditional Chinese)
 * Fluent UI design
 * Cross-platform support
 * Open-source and free to use under MIT licence
 * Frameless Window on
@@ -47,16 +52,16 @@
 ## Requirements 🧩
 
 ```text
 Python>=3.7
 ```
 
 ```text
-PyQt5>=5.15.4
-PyMuPDF>=1.19.2
+PyQt6>=6.7.0
+PyMuPDF>=1.24.0
 ```
 
 ## Install & Run
 
 ### install from source
 
 you will need `setuptools` and `wheel` installed
```

### Comparing `pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/PKG-INFO` & `pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPDFeditor-GUI
-Version: 2.3.0
+Version: 3.0.0
 Summary: A desktop application to edit PDF files.
 Home-page: https://github.com/Augus1999/pyPDFeditor-GUI/
 Author: Nianze A. TAO
 Author-email: Augus_1999@outlook.com
 License: MIT
 Project-URL: Source, https://github.com/Augus1999/pyPDFeditor-GUI
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyMuPDF>=1.19.2
-Requires-Dist: PyQt5>=5.15.4
+Requires-Dist: PyMuPDF>=1.24.3
+Requires-Dist: PyQt6>=6.7.0
 
 # pyPDFeditor-GUI
 
 [![PyPI](https://img.shields.io/pypi/v/pyPDFeditor-GUI?color=5f69b4)](https://pypi.org/project/pyPDFeditor-GUI/)
 [![Downloads](https://static.pepy.tech/personalized-badge/pyPDFeditor-GUI?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/pyPDFeditor-GUI)
 ![pylint](https://github.com/Augus1999/pyPDFeditor-GUI/actions/workflows/pylint.yml/badge.svg)
 
@@ -45,14 +45,19 @@
 
 Welcome to use pyPDFeditor-GUI. pyPDFeditor-GUI is a simple cross-platform application, thanks
 to [Python](https://www.python.org/), [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
 and [PyMuPDF](https://github.com/pymupdf/PyMuPDF), designed to work on simple PDF handling.
 
 I tried my best to make it close to Fluent UI. Icons used can be found [🔗here](https://fluenticons.co/).
 
+From version 3.0.0, we have moved the GUI library to PyQt6. If you upgraded from a previous version, you can consider removing PyQt5:
+```bash
+$ pip uninstall PyQt5 PyQt5-Qt5 PyQt5-sip
+```
+
 ## Features
 
 * Support 3 languages: English, 日本語 (Japanese), and 中文 (Traditional Chinese)
 * Fluent UI design
 * Cross-platform support
 * Open-source and free to use under MIT licence
 * Frameless Window on
@@ -77,16 +82,16 @@
 ## Requirements 🧩
 
 ```text
 Python>=3.7
 ```
 
 ```text
-PyQt5>=5.15.4
-PyMuPDF>=1.19.2
+PyQt6>=6.7.0
+PyMuPDF>=1.24.0
 ```
 
 ## Install & Run
 
 ### install from source
 
 you will need `setuptools` and `wheel` installed
```

### Comparing `pyPDFeditor-GUI-2.3.0/pyPDFeditor_GUI.egg-info/SOURCES.txt` & `pypdfeditor_gui-3.0.0/pyPDFeditor_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/__main__.py` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/__main__.py`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/application.py` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import os
 import json
 import shutil
 import getpass
 import subprocess as sp
 from pathlib import Path
 from typing import Dict
-import fitz
-from PyQt5 import QtCore
-from PyQt5.QtGui import QColor, QPixmap
-from PyQt5.QtWidgets import QColorDialog
+import pymupdf as fitz
+from PyQt6 import QtCore
+from PyQt6.QtGui import QColor, QPixmap, QCloseEvent
+from PyQt6.QtWidgets import QColorDialog
 from .language import set_language, lag_s, lag_p
 from .windows import (
     MainR,
     PermMenuR,
     BUTTON_STYLE,
     SettingR,
     FontDialogR,
@@ -116,21 +116,23 @@
                 clean(self.tab3),
                 self.tab3.text.clear(),
                 self.tab3.line1.clear(),
                 self.tab3.line2.clear(),
             )
         )
         self.tab3.button9.clicked.connect(
-            lambda: os.remove(
-                os.path.join(app_home, "font_dir_cache.json"),
-            )
-            if os.path.exists(
-                os.path.join(app_home, "font_dir_cache.json"),
+            lambda: (
+                os.remove(
+                    os.path.join(app_home, "font_dir_cache.json"),
+                )
+                if os.path.exists(
+                    os.path.join(app_home, "font_dir_cache.json"),
+                )
+                else None
             )
-            else None
         )  # delete font dir cache
         self.tab3.line3.returnPressed.connect(self.preview)
         self.tab3.line4.returnPressed.connect(self.preview)
         self.tab3.line5.returnPressed.connect(self.preview)
         self.tab3.check1.stateChanged.connect(self.enable_preview)
         self.tab3.check2.stateChanged.connect(self.enable_perm_set)
         self.tab4.button1.clicked.connect(self.add4)
@@ -151,15 +153,15 @@
         set_language(self)
         self.settings = QtCore.QSettings("QtProject", "pyPDFEditor-GUI")
         if not self.settings.value("geometry") == None:
             self.restoreGeometry(self.settings.value("geometry"))
         if not self.settings.value("windowState") == None:
             self.restoreState(self.settings.value("windowState"))
 
-    def closeEvent(self, event) -> None:
+    def closeEvent(self, event: QCloseEvent) -> None:
         """
         write settings to settings.json
         """
         self.settings.setValue("geometry", self.saveGeometry())
         self.settings.setValue("windowState", self.saveState())
         _settings = {
             "start dir": self.s_dir,
@@ -485,15 +487,15 @@
             initial=QColor(
                 int(255 * self.colour_r),
                 int(255 * self.colour_g),
                 int(255 * self.colour_b),
                 int(255 * float(self.tab3.line4.text()) / 100),
             ),
             options=QColorDialog.ColorDialogOption(
-                QColorDialog.ShowAlphaChannel,
+                QColorDialog.ColorDialogOption.ShowAlphaChannel,
             ),
             parent=self,
             title="Select Colour",
         )
         if _colour.isValid():
             self.colour_r = _colour.getRgbF()[0]
             self.colour_g = _colour.getRgbF()[1]
@@ -509,15 +511,15 @@
         """
         if os.path.exists(os.path.join(app_home, "font_dir_cache.json")):
             name_dict, file_dict = read_from_font_cache(
                 os.path.join(app_home, "font_dir_cache.json"),
             )
         else:
             font_paths = QtCore.QStandardPaths.standardLocations(
-                QtCore.QStandardPaths.FontsLocation,
+                QtCore.QStandardPaths.StandardLocation.FontsLocation,
             )
             name_dict, file_dict = find_font(font_paths)
             store_font_path(name_dict, os.path.join(app_home, "font_dir_cache.json"))
         self.FontDialogCD = FontDialog(
             self.font_dir,
             name_dict,
             file_dict,
@@ -613,15 +615,15 @@
                 BUTTON_STYLE % ("folder.svg", "folder_h.svg", "folder_p.svg"),
             )
             self.button1.clicked.connect(lambda: choose(self.line1, self.s_dir))
             self.button2.clicked.connect(lambda: choose(self.line2, self.o_dir))
             self.line1.setReadOnly(False)
             self.line2.setReadOnly(False)
 
-    def closeEvent(self, event) -> None:
+    def closeEvent(self, event: QCloseEvent) -> None:
         """
         re-write closeEvent
         """
         self.signal.emit(
             self.line1.text(),
             self.line2.text(),
             self.check.isChecked(),
@@ -640,15 +642,15 @@
 
     def set_language(self, language: str) -> None:
         """
         set language
         """
         lag_p(self, language)
 
-    def closeEvent(self, event) -> None:
+    def closeEvent(self, event: QCloseEvent) -> None:
         """
         close event
         """
         perm_int = 0
         if self.check1.isChecked():
             perm_int += fitz.PDF_PERM_PRINT
         if self.check2.isChecked():
@@ -715,15 +717,15 @@
         shape.commit()
         cover = render_pdf_page(page)
         self.label.setPixmap(QPixmap(cover))
         doc.close()
         fitz.TOOLS.store_shrink(100)  # delete MuPDF cache
         del cover, shape, page, r1, doc
 
-    def closeEvent(self, event) -> None:
+    def closeEvent(self, event: QCloseEvent) -> None:
         """
         close event
         """
         self.signal.emit(self.name_dict[self.combobox.currentText()])
         self.close()
         del self
```

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/functions.py` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import os
 import gc
 import sys
 import json
 import time
 from typing import Union, Optional, Tuple, List
 from pathlib import Path
-from fitz import Document, Page, Pixmap, Rect, Point, Font
-from fitz.utils import get_pixmap, set_metadata, Shape
-from fitz import TOOLS, Matrix, Identity
-from PyQt5 import QtGui, QtCore, QtWidgets
-from PyQt5.QtWidgets import (
+from pymupdf import Document, Page, Pixmap, Rect, Point, Font
+from pymupdf.utils import get_pixmap, set_metadata, Shape
+from pymupdf import TOOLS, Matrix, Identity
+from PyQt6 import QtGui, QtCore, QtWidgets
+from PyQt6.QtWidgets import (
     QInputDialog,
     QHBoxLayout,
     QWidget,
     QFileDialog,
     QMessageBox,
     QLineEdit,
 )
@@ -43,21 +43,20 @@
 def copy(doc: Doc) -> Doc:
     """
     copy the doc
 
     :param doc: document to be copied
     :return: copied document
     """
-    _doc = Doc(doc.name)
+    _doc = Doc(filename=doc.name)
     if not _doc.is_pdf:
         pdf_bites = _doc.convert_to_pdf()
         _doc = Doc("pdf", pdf_bites)
     if doc.pass_word is not None:
         _doc.authenticate(doc.pass_word)
-    _doc.name = doc.name
     _doc.rotatedPages = doc.rotatedPages
     if len(_doc.rotatedPages) != 0:
         for page in _doc.rotatedPages:
             _doc[page].set_rotation(_doc.rotatedPages[page])
     return _doc
 
 
@@ -82,15 +81,20 @@
                 return _open_warning(parent)
         pdf_bites = doc.convert_to_pdf()  # convert to pdf
         doc = Doc("pdf", pdf_bites)
         doc.name = file_name
     if doc.needs_pass:
         while doc.is_encrypted:
             value, _ = QInputDialog.getText(
-                parent, " ", "Password:", QLineEdit.Password, "", QtCore.Qt.Dialog
+                parent,
+                " ",
+                "Password:",
+                QLineEdit.EchoMode.Password,
+                "",
+                QtCore.Qt.WindowType.Dialog,
             )
             if not _:
                 doc.close()
                 del doc
                 return None, False
             doc.authenticate(value)
             doc.pass_word = value
@@ -102,17 +106,17 @@
     render PDF page
 
     :param page_data: page data
     :return: a QPixmap
     """
     page_pixmap = get_pixmap(page_data, matrix=Identity, clip=True)
     if page_pixmap.alpha:
-        image_format = QtGui.QImage.Format_RGBA8888
+        image_format = QtGui.QImage.Format.Format_RGBA8888
     else:
-        image_format = QtGui.QImage.Format_RGB888
+        image_format = QtGui.QImage.Format.Format_RGB888
     page_image = QtGui.QImage(
         page_pixmap.samples,
         page_pixmap.w,
         page_pixmap.h,
         page_pixmap.stride,
         image_format,
     )
@@ -210,19 +214,19 @@
         return content
     except FileNotFoundError:
         reply = QMessageBox.warning(
             parent,
             "Error",
             f"Cannot find {os.path.basename(set_file_name)}\n\n"
             f"Create an empty setting file?",
-            QMessageBox.Yes | QMessageBox.No,
+            QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No,
         )
-        if reply == QMessageBox.No:
+        if reply == QMessageBox.StandardButton.No:
             sys.exit(0)
-        if reply == QMessageBox.Yes:
+        if reply == QMessageBox.StandardButton.Yes:
             content = {
                 "start dir": "",
                 "save dir": "",
                 "language": "English",
                 "font dir": "",
                 "dir store": False,
             }
@@ -255,31 +259,31 @@
     :param _scaled: scaled coefficient of label
     :return: shadowed QWidget()
     """
     _cover = render_pdf_page(page)
     label = QtWidgets.QLabel(None)
     layout = QHBoxLayout(None)
     widget = QWidget(None)
-    layout.addWidget(label, alignment=QtCore.Qt.AlignCenter)
+    layout.addWidget(label, alignment=QtCore.Qt.AlignmentFlag.AlignCenter)
     widget.setLayout(layout)
     if _cover.height() / _cover.width() >= 4 / 3:
         scaled_height = int(width // w_col * 4 / 3 * _scaled)
         scaled_width = int(scaled_height * (_cover.width() / _cover.height()))
     else:
         scaled_width = int(width // w_col * _scaled)
         scaled_height = int(scaled_width * (_cover.height() / _cover.width()))
     label.setPixmap(
         QtGui.QPixmap(_cover).scaled(
             scaled_width,
             scaled_height,
-            QtCore.Qt.IgnoreAspectRatio,
-            QtCore.Qt.SmoothTransformation,
+            QtCore.Qt.AspectRatioMode.IgnoreAspectRatio,
+            QtCore.Qt.TransformationMode.SmoothTransformation,
         ),
     )
-    label.setAlignment(QtCore.Qt.AlignCenter)
+    label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
     label.setFixedSize(scaled_width, scaled_height)
     shadow(label, QtGui.QColor(0, 0, 0, 100), 20)
     del _cover, label, layout
     return widget
 
 
 def set_icon(
@@ -292,17 +296,19 @@
     :param doc: doc
     :param _scaled: scaled coefficient of label
     :return: None
     """
     x, y = 0, 0
     for i in widget.book_list:
         label = page_icon(
-            widget.book[i]
-            if isinstance(widget.book_list[0], int)
-            else (i[0] if doc is None else doc[0]),
+            (
+                widget.book[i]
+                if isinstance(widget.book_list[0], int)
+                else (i[0] if doc is None else doc[0])
+            ),
             widget.table.width(),
             widget.w_col,
             _scaled,
         )
         widget.table.setCellWidget(x, y, label)
         del label  # delete label (important)
         # do not change the following codes
@@ -382,14 +388,15 @@
     row_num = col_num = -1  # set to a negative value!
     for i in widget.table.selectionModel().selection().indexes():
         row_num = i.row()
         col_num = i.column()
     index = row_num * widget.w_col + col_num  # get position
     if 0 <= index < len(widget.book_list):
         menu = QtWidgets.QMenu()
+        menu.setStyleSheet("font-size:12pt")
         item1 = menu.addAction(
             QtGui.QIcon(os.path.join(icon_path, "delete.svg")), MENU_L[main.language][0]
         )
         item2, item3, item4, item5, item6, item7, item8 = (None for _ in range(7))
         if select in (0, 2):
             item3 = menu.addAction(
                 QtGui.QIcon(str(icon_path / "view.svg")), MENU_L[main.language][1]
@@ -413,15 +420,15 @@
             item7 = menu.addAction(
                 QtGui.QIcon(str(icon_path / "move_page.svg")), MENU_L[main.language][6]
             )
         if select == 0:
             item8 = menu.addAction(
                 QtGui.QIcon(str(icon_path / "arrow_move.svg")), MENU_L[main.language][7]
             )
-        action = menu.exec_(widget.table.mapToGlobal(pos))
+        action = menu.exec(widget.table.mapToGlobal(pos))
         if action == item1:
             delete(index=index, widget=widget)
         if action == item2 and select == 1:
             save_as(index=index, widget=widget, main=main)
         if action == item3 and select in (0, 2):
             main.view(index, widget)
         if action == item4 and select == 1:
@@ -535,15 +542,15 @@
         # xref is inf[0]
         img = Pixmap(doc, inf[0])
         img.save(img_name)
     QMessageBox.information(
         main,
         "Saved",
         MESSAGE[main.language][1].format(len(img_inf), main.s_dir),
-        QMessageBox.Yes,
+        QMessageBox.StandardButton.Yes,
     )
     TOOLS.store_shrink(100)  # delete MuPDF cache
 
 
 def rotate_page(index: int, degree: int, widget: QWidget) -> None:
     """
     rotate page
@@ -579,15 +586,15 @@
         parent,
         " ",
         f"Move to page: (from 1 to {book_length})",
         value=index + 1,
         min=1,
         max=book_length,
         step=1,
-        flags=QtCore.Qt.Dialog,
+        flags=QtCore.Qt.WindowType.Dialog,
     )
     if not _:
         return None
     page_index = widget.book_list[index]
     widget.book_list[index] = None
     if value <= index:
         widget.book_list.insert(value - 1, page_index)
@@ -604,15 +611,15 @@
     """
     set watermark position in the page
 
     :param main: main widget
     :return: None
     """
     pos_str, _ = QInputDialog.getText(
-        main, " ", "Set watermark position: x,y", flags=QtCore.Qt.Dialog
+        main, " ", "Set watermark position: x,y", flags=QtCore.Qt.WindowType.Dialog
     )
     if _:
         pos = pos_str.strip().split(",")
         try:
             main.tab3.xy = (int(pos[0]), int(pos[1]))
         except ValueError:
             pass
@@ -800,19 +807,23 @@
 
 
 def warning(parent) -> None:
     """
     :param parent: parent
     :return: None
     """
-    QMessageBox.warning(parent, "Oops", MESSAGE[parent.language][2], QMessageBox.Yes)
+    QMessageBox.warning(
+        parent, "Oops", MESSAGE[parent.language][2], QMessageBox.StandardButton.Yes
+    )
 
 
 def _open_warning(parent: QWidget) -> Tuple[None, bool]:
     """
     raise warning pop-up window when encountering an incorrect file
 
     :param parent: parent
     :return: (None, False)
     """
-    QMessageBox.critical(parent, "Oops", MESSAGE[parent.language][0], QMessageBox.Yes)
+    QMessageBox.critical(
+        parent, "Oops", MESSAGE[parent.language][0], QMessageBox.StandardButton.Yes
+    )
     return None, False
```

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/Photo.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/Photo.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/arrow_move.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/arrow_move.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/book2.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/book2.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/color.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/color.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/color_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/color_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/color_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/color_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/delete.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/delete_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/delete_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/delete_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/delete_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/down.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/down.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/down_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/down_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/down_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/down_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/edit.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/edit.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder_d.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder_d.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/folder_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/folder_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/font.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/font.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/font_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/font_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/font_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/font_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/home.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/home.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/lock.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/merge.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/merge.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more_d.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more_d.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/more_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/more_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/pdf icon.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/pdf icon.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/settings.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/settings_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/settings_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/settings_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/settings_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/square_multiple.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/square_multiple.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/sync.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/sync.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/sync_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/sync_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/sync_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/sync_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/view.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/view_h.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/view_h.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/icons/view_p.svg` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/icons/view_p.svg`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/language.py` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/language.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,85 @@
 # -*- coding: utf-8 -*-
 # Author: Nianze A. TAO
 """
 language related functions
 """
-from PyQt5 import QtWidgets
+from PyQt6 import QtWidgets
 
 TAB_L = {
     "English": [
         "     Merge PDF    ",
         "    Organise    ",
         "    Security    ",
         "    Metadata    ",
     ],
-    "中文": ["    合并文檔    ", "    分割頁面    ", "    檔案保護    ", "    元數據    "],
+    "中文": [
+        "    合并文檔    ",
+        "    分割頁面    ",
+        "    檔案保護    ",
+        "    元數據    ",
+    ],
     "日本語": ["ファイル結合", "ページオルガナイズ", "電子透かし", "メタデータ"],
 }
 TIP_L = {
     "English": [
         "Open",
         "Save",
         "Settings",
         "Clean",
         "colours",
         "preview",
         "more",
         "font",
         "update font",
     ],
-    "中文": ["開啓檔案", "保存", "設定", "清除", "顔色", "預覽", "更多", "字體", "更新字體庫"],
-    "日本語": ["開く", "保存する", "設定", "全て閉じる", "色選ぶ", "プレビュー", "詳細設定", "字体", "字体を更新"],
+    "中文": [
+        "開啓檔案",
+        "保存",
+        "設定",
+        "清除",
+        "顔色",
+        "預覽",
+        "更多",
+        "字體",
+        "更新字體庫",
+    ],
+    "日本語": [
+        "開く",
+        "保存する",
+        "設定",
+        "全て閉じる",
+        "色選ぶ",
+        "プレビュー",
+        "詳細設定",
+        "字体",
+        "字体を更新",
+    ],
 }
 LAB_L3 = {
     "English": [
         "PASSWORD",
         "WATERMARK",
         "Font Size:",
         "Open after saving",
         "Opacity:",
         "Rotation:",
         "Preview Mode",
         "Edit Restriction",
     ],
-    "中文": ["密碼", "水印", "字號：", "保存後開啓", "透明度：", "旋轉：", "預覽模式", "限制編輯"],
+    "中文": [
+        "密碼",
+        "水印",
+        "字號：",
+        "保存後開啓",
+        "透明度：",
+        "旋轉：",
+        "預覽模式",
+        "限制編輯",
+    ],
     "日本語": [
         "パスワード",
         "電子透かし",
         "フォントサイズ：",
         "保存してから開く",
         "不透明度：",
         "回転：",
@@ -170,15 +204,19 @@
 }
 MESSAGE = {
     "English": [
         "   Format error:\n cannot open this file",
         "{} image(s) saved to {}",
         "Cannot save! Try a new file name...",
     ],
-    "中文": ["    格式錯誤：\n 無法開啓此檔案", "已保存{}張圖像至{}", "無法保存欸。請嘗試新的文檔名稱。。。"],
+    "中文": [
+        "    格式錯誤：\n 無法開啓此檔案",
+        "已保存{}張圖像至{}",
+        "無法保存欸。請嘗試新的文檔名稱。。。",
+    ],
     "日本語": [
         "    格式エラー：\n このファイルが開けません",
         "{}幅のイメージが{}に保存されました",
         "すみません。保存できませんでした。\n 新たな名前を付けてみて下さい。。。",
     ],
 }
```

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/style_sheets.py` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/style_sheets.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .icons import icon_path
 
 icon_path_ = str(icon_path).replace("\\", "/")
 
 MAIN_COLOUR = "#6272a4"  # main colour of the theme
 COMP_COLOUR = "#b7cbc9"  # complementary colour of MAIN_COLOUR
 COMP_COLOUR_2 = "#ca8fc0"
-LIGHT_COLOUR = "#f8f8f2"  # #f8f8f2
+LIGHT_COLOUR = "#f8f8f2"
 DARK_COLOUR = "#4f5c84"
 TEXT_COLOUR = "#1b124b"
 TAB_STYLE = f"""
         QTabBar::tab{{
         border-left:4px solid {MAIN_COLOUR};
         padding:3ex;
         margin:0px}}
@@ -24,24 +24,24 @@
         QTabBar::tab:hover{{
         border-left:4px solid {COMP_COLOUR_2};
         background-color:{COMP_COLOUR_2}}}
         QToolTip{{
         border:none;
         color:{TEXT_COLOUR};
         background-color:{LIGHT_COLOUR};
-        font-size:9pt;
+        font-size:12pt;
         font-family:Verdana,Microsoft YaHei UI,PingFang SC}}
         QTabWidget{{
         border:none;
         border-radius:5px;
         background-color:{MAIN_COLOUR}}}
         """
 COMBO_BOX_STYLE = f"""
         QComboBox{{
-        font-size:11pt;
+        font-size:14pt;
         font-family:Verdana,Microsoft YaHei UI,PingFang SC;
         border-radius:5px;
         background-color:{MAIN_COLOUR};
         color:{LIGHT_COLOUR}}}
         QComboBox:hover{{
         border:none}}
         QComboBox::drop-down{{
@@ -62,15 +62,15 @@
         width:10px}}
         QScrollBar::handle:vertical{{
         background-color:{MAIN_COLOUR};
         border-radius:3px;
         min-height:45px}}
         """
 TEXTEDIT_STYLE = f"""
-        QTextEdit{{font-size:11pt;
+        QTextEdit{{font-size:14pt;
         border-top-left-radius:5px;
         border-top-right-radius:5px;
         border-bottom-left-radius:0px;
         border-bottom-right-radius:0px;
         background-color:{MAIN_COLOUR};
         color:{LIGHT_COLOUR};
         font-family:Verdana,Microsoft YaHei UI,PingFang SC}}
@@ -95,15 +95,15 @@
         background-color:{MAIN_COLOUR};
         border-radius:4px;
         min-width:45px}}
         """
 LINE_EDIT_STYLE = f"""
         QLineEdit{{
         border:none;
-        font-size:10pt;
+        font-size:12pt;
         border-radius:10px;
         background-color:{MAIN_COLOUR};
         color:{LIGHT_COLOUR};
         font-family:Verdana,Microsoft YaHei UI,PingFang SC}}
         QLineEdit:focus{{
         border:2px solid {COMP_COLOUR}}}
         """
@@ -167,29 +167,29 @@
         border-radius:2px;
         min-height:45px}}
         """
 LABEL_STYLE = f"""
         QLabel{{
         border:none;
         border-radius:10px;
-        font-size:8pt;
+        font-size:12pt;
         font-family:Verdana,Microsoft YaHei UI,PingFang SC;
         color:{TEXT_COLOUR};
         background-color:transparent}}
         """
 BGC_STYLE = f"""
         QWidget{{
         border:none;
         border-radius:0px;
         background-color:%s}}
         QToolTip{{
         border:none;
         color:{TEXT_COLOUR};
         background-color:{LIGHT_COLOUR};
-        font-size:9pt;
+        font-size:12pt;
         font-family:Verdana,Microsoft YaHei UI,PingFang SC}}
         """
 SWITCH_STYLE = f"""
         SwitchBtn:on{{
         background-color:{MAIN_COLOUR};
         color:{LIGHT_COLOUR}}}
         SwitchBtn:off{{
```

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/window_effect.py` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/window_effect.py`

 * *Files identical despite different names*

### Comparing `pyPDFeditor-GUI-2.3.0/pypdfeditor_core/windows.py` & `pypdfeditor_gui-3.0.0/pypdfeditor_core/windows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # -*- coding: utf-8 -*-
 # Author: Nianze A. TAO
 """
 application window forms
 """
 import re
-from typing import Tuple
-from PyQt5.QtGui import (
+from typing import Tuple, Union
+from PyQt6.sip import voidptr
+from PyQt6.QtGui import (
     QIcon,
     QPainter,
     QPainterPath,
     QColor,
     QFont,
     QPixmap,
     QTransform,
     QCursor,
+    QPaintEvent,
+    QMouseEvent,
+    QResizeEvent,
 )
-from PyQt5 import QtCore, QtWidgets
-from PyQt5.QtWidgets import (
+from PyQt6 import QtCore, QtWidgets
+from PyQt6.QtWidgets import (
     QWidget,
     QGridLayout,
     QTabWidget,
     QLabel,
     QTextEdit,
     QScrollArea,
     QComboBox,
     QLineEdit,
     QPushButton,
     QTableWidget,
-    QApplication,
 )
 from .style_sheets import (
     icon_path,
     LIGHT_COLOUR,
     MAIN_COLOUR,
     BGC_STYLE,
     TAB_STYLE,
@@ -71,15 +74,15 @@
         self.space = 6
         self.rectRadius = 5
         self.step = self.width() / 50
         self.startX = 0
         self.endX = 0
         self.timer = QtCore.QTimer(self)
         self.timer.timeout.connect(self.update_value)
-        self.setFont(QFont("calibri", 10))
+        self.setFont(QFont("calibri", 14))
 
     def setStyleSheet(self, style_sheet: str) -> None:
         """
         define set-style-sheet behaviour
         """
         style_sheet = re.sub(r"\s+", "", style_sheet)
         on_style = str(re.findall(r"SwitchBtn:on{.+?}", style_sheet))
@@ -115,15 +118,15 @@
             if self.startX > self.endX:
                 self.startX = self.startX - self.step
             else:
                 self.startX = self.endX
                 self.timer.stop()
         self.update()
 
-    def mousePressEvent(self, event) -> None:
+    def mousePressEvent(self, event: QMouseEvent) -> None:
         """
         mousePressEvent
         """
         self.checked = not self.checked
         self.stateChanged.emit(self.checked)
         self.step = self.width() / 50
         if self.checked:
@@ -147,59 +150,59 @@
 
     def isChecked(self) -> bool:
         """
         is-checked
         """
         return self.checked
 
-    def paintEvent(self, event) -> None:
+    def paintEvent(self, event: QPaintEvent) -> None:
         """
         paintEvent
         """
         painter = QPainter()
         painter.begin(self)
-        painter.setRenderHint(QPainter.Antialiasing)
+        painter.setRenderHint(QPainter.RenderHint.Antialiasing)
         self.draw_bg(painter)
         self.draw_text(painter)
         self.draw_slider(painter)
         painter.end()
 
-    def draw_text(self, painter) -> None:
+    def draw_text(self, painter: QPainter) -> None:
         """
         draw text
         """
         painter.save()
         if self.checked:
             painter.setPen(self.textColorOn)
             painter.drawText(
                 0,
                 0,
                 int(self.width() / 2 + self.space * 2),
                 self.height(),
-                QtCore.Qt.AlignCenter,
+                QtCore.Qt.AlignmentFlag.AlignCenter,
                 self.textOn,
             )
         else:
             painter.setPen(self.textColorOff)
             painter.drawText(
                 int(self.width() / 2),
                 0,
                 int(self.width() / 2 - self.space),
                 self.height(),
-                QtCore.Qt.AlignCenter,
+                QtCore.Qt.AlignmentFlag.AlignCenter,
                 self.textOff,
             )
         painter.restore()
 
-    def draw_bg(self, painter) -> None:
+    def draw_bg(self, painter: QPainter) -> None:
         """
         draw background
         """
         painter.save()
-        painter.setPen(QtCore.Qt.NoPen)
+        painter.setPen(QtCore.Qt.PenStyle.NoPen)
         if self.checked:
             painter.setBrush(self.bgColorOn)
         else:
             painter.setBrush(self.bgColorOff)
         rect = QtCore.QRect(0, 0, self.width(), self.height())
         radius = rect.height() / 2
         circle_width = rect.height()
@@ -218,20 +221,20 @@
             270,
             180,
         )
         path.lineTo(radius, rect.top())
         painter.drawPath(path)
         painter.restore()
 
-    def draw_slider(self, painter) -> None:
+    def draw_slider(self, painter: QPainter) -> None:
         """
         draw slider
         """
         painter.save()
-        painter.setPen(QtCore.Qt.NoPen)
+        painter.setPen(QtCore.Qt.PenStyle.NoPen)
         if self.checked:
             painter.setBrush(self.sliderColorOn)
         else:
             painter.setBrush(self.sliderColorOff)
         rect = QtCore.QRect(0, 0, self.width(), self.height())
         slider_width = rect.height() - self.space * 2
         slider_rect = QtCore.QRect(
@@ -244,20 +247,20 @@
 class TableWidget(QTableWidget):
     """
     a wrapper to QTableWidget
     """
 
     Index = QtCore.pyqtSignal(tuple)
 
-    def mousePressEvent(self, event) -> None:
+    def mousePressEvent(self, event: QMouseEvent) -> None:
         """
         re-write mousePressEvent
         """
         QTableWidget.mousePressEvent(self, event)
-        if event.button() == QtCore.Qt.LeftButton:
+        if event.button() == QtCore.Qt.MouseButton.LeftButton:
             row_num = col_num = int()
             for i in self.selectionModel().selection().indexes():
                 row_num = i.row()
                 col_num = i.column()
             self.Index.emit((row_num, col_num))
 
 
@@ -271,15 +274,15 @@
         super().__init__()
         self.__system__ = system
         self.__version__ = version
         self.resize(1200, 890)  # 1200 890
         self.setMinimumSize(580, 450)
         self.setWindowTitle("PDF Editor")
         self.setWindowIcon(QIcon(str(icon_path / "pdf icon.svg")))
-        self.setTabPosition(QTabWidget.West)
+        self.setTabPosition(QTabWidget.TabPosition.West)
         self.setIconSize(QtCore.QSize(35, 35))
         self.setStyleSheet(TAB_STYLE)
         self.tab0 = QWidget()
         self.tab1 = QWidget()
         self.tab2 = QWidget()
         self.tab3 = QWidget()
         self.tab4 = QWidget()
@@ -295,51 +298,51 @@
         matrix = QTransform()
         matrix.rotate(90)
         self.addTab(
             self.tab0,
             QIcon(
                 QPixmap(
                     str(icon_path / "home.svg"),
-                ).transformed(matrix, QtCore.Qt.SmoothTransformation)
+                ).transformed(matrix, QtCore.Qt.TransformationMode.SmoothTransformation)
             ),
             "",
         )
         self.addTab(
             self.tab1,
             QIcon(
                 QPixmap(
                     str(icon_path / "merge.svg"),
-                ).transformed(matrix, QtCore.Qt.SmoothTransformation)
+                ).transformed(matrix, QtCore.Qt.TransformationMode.SmoothTransformation)
             ),
             "",
         )
         self.addTab(
             self.tab2,
             QIcon(
                 QPixmap(
                     str(icon_path / "edit.svg"),
-                ).transformed(matrix, QtCore.Qt.SmoothTransformation)
+                ).transformed(matrix, QtCore.Qt.TransformationMode.SmoothTransformation)
             ),
             "",
         )
         self.addTab(
             self.tab3,
             QIcon(
                 QPixmap(
                     str(icon_path / "lock.svg"),
-                ).transformed(matrix, QtCore.Qt.SmoothTransformation)
+                ).transformed(matrix, QtCore.Qt.TransformationMode.SmoothTransformation)
             ),
             "",
         )
         self.addTab(
             self.tab4,
             QIcon(
                 QPixmap(
                     str(icon_path / "metadata.svg"),
-                ).transformed(matrix, QtCore.Qt.SmoothTransformation)
+                ).transformed(matrix, QtCore.Qt.TransformationMode.SmoothTransformation)
             ),
             "",
         )
         if self.__system__ == "Windows":
             self.btn_min_0 = QPushButton(self.tab0)
             self.btn_max_0 = QPushButton(self.tab0)
             self.btn_ext_0 = QPushButton(self.tab0)
@@ -437,15 +440,15 @@
             from .window_effect import WindowEffect, MSG
 
             self.windowEffect = WindowEffect()
             self.msg = MSG
             self._title_bar_pos = [
                 QtCore.QPoint(x, y) for x in range(1200) for y in range(52)
             ]
-            self.setWindowFlags(QtCore.Qt.FramelessWindowHint)
+            self.setWindowFlags(QtCore.Qt.WindowType.FramelessWindowHint)
             self.windowEffect.add_shadow_effect(int(self.winId()))
             self.windowEffect.add_window_style(int(self.winId()))
             self.windowHandle().screenChanged.connect(
                 lambda: self.windowEffect.screen_change(int(self.winId())),
             )
         else:
             self.tab1.grid.addWidget(self.tab1.button3, 0, 20)
@@ -461,58 +464,60 @@
     def saveState(self) -> QtCore.QByteArray:
         return QtCore.QByteArray(f"{self.pos().x()},{self.pos().y()}".encode())
 
     def restoreState(self, state: QtCore.QByteArray) -> None:
         x, y = [int(i) for i in str(state)[2:-1].split(",")]
         self.move(x, y)
 
-    def paintEvent(self, event) -> None:
+    def paintEvent(self, event: QPaintEvent) -> None:
         """
         re-write paintEvent
         """
         if self.__system__ != "Windows":
             QTabWidget.paintEvent(self, event)
             return
         super().paintEvent(event)
         painter = QPainter(self)
-        painter.setPen(QtCore.Qt.NoPen)
+        painter.setPen(QtCore.Qt.PenStyle.NoPen)
         painter.setBrush(QColor(MAIN_COLOUR))
         painter.drawRect(QtCore.QRect(0, 0, self.width() - 2, self.height() - 2))
         painter.setBrush(QColor(LIGHT_COLOUR))
         painter.drawRect(QtCore.QRect(0, self.height() - 2, self.width(), 2))
         painter.drawRect(QtCore.QRect(self.width() - 2, 0, 2, self.height()))
 
     # -------well, why do the following ugly codes exist?-------
     # -------they are used to re-enable the window animations under Windows platform-------
-    def mouseMoveEvent(self, event) -> None:
+    def mouseMoveEvent(self, event: QMouseEvent) -> None:
         """
         re-write mouseMoveEvent
         move the frameless window
         """
         if self.__system__ == "Windows":
             if (
                 event.pos() in self._title_bar_pos
-                and event.buttons() == QtCore.Qt.LeftButton
+                and event.buttons() == QtCore.Qt.MouseButton.LeftButton
             ):
                 self.windowEffect.move_window(int(self.winId()))
         return QTabWidget.mouseMoveEvent(self, event)
 
-    def mouseDoubleClickEvent(self, event) -> None:
+    def mouseDoubleClickEvent(self, event: QMouseEvent) -> None:
         """
         re-write mouseDoubleClickEvent
         """
         if self.__system__ == "Windows":
             if (
-                event.button() == QtCore.Qt.LeftButton
+                event.button() == QtCore.Qt.MouseButton.LeftButton
                 and event.pos() in self._title_bar_pos
             ):
                 self.windowChange()
         return QTabWidget.mouseDoubleClickEvent(self, event)
 
-    def nativeEvent(self, event_type, message) -> Tuple[bool, int]:
+    def nativeEvent(
+        self, event_type: QtCore.QByteArray, message: voidptr
+    ) -> Tuple[bool, Union[int, voidptr]]:
         """
         re-write nativeEvent
         """
         if self.__system__ == "Windows":
             msg = self.msg.from_address(message.__int__())
             i = self.currentIndex()
             if msg.message == 132:  # WM_NCHITTEST
@@ -539,34 +544,33 @@
                     return True, 15  # HTBOTTOM
                 elif lx:
                     return True, 10  # HTLEFT
                 elif rx:
                     return True, 11  # HTRIGHT
             if msg.message == 131:  # WM_NCCALCSIZE
                 if self.windowEffect.isMaximised(msg.hWnd):
-                    desktop = QApplication.desktop()
-                    screen_rect = desktop.availableGeometry()
+                    screen_rect = self.screen().availableGeometry()
                     self.windowEffect.monitorNCCALCSIZE(msg, screen_rect)
                     self.btn_max_0.setStyleSheet(BUTTON_STYLE0 % "square_multiple.svg")
                     self.btn_max_1.setStyleSheet(BUTTON_STYLE0 % "square_multiple.svg")
                     self.btn_max_2.setStyleSheet(BUTTON_STYLE0 % "square_multiple.svg")
                     self.btn_max_3.setStyleSheet(BUTTON_STYLE0 % "square_multiple.svg")
                     self.btn_max_4.setStyleSheet(BUTTON_STYLE0 % "square_multiple.svg")
                 else:
                     self.btn_max_0.setStyleSheet(BUTTON_STYLE0 % "maximize.svg")
                     self.btn_max_1.setStyleSheet(BUTTON_STYLE0 % "maximize.svg")
                     self.btn_max_2.setStyleSheet(BUTTON_STYLE0 % "maximize.svg")
                     self.btn_max_3.setStyleSheet(BUTTON_STYLE0 % "maximize.svg")
                     self.btn_max_4.setStyleSheet(BUTTON_STYLE0 % "maximize.svg")
                 return True, 0  # HTNOWHERE
-        return QTabWidget.nativeEvent(self, event_type, message)
+        return False, voidptr(-1)
 
     # -------here ends the ugly code-------
 
-    def resizeEvent(self, event) -> None:
+    def resizeEvent(self, event: QResizeEvent) -> None:
         """
         re-write resizeEvent
         """
         super().resizeEvent(event)
         self.widget3.resize(int(self.width() * 0.9), int(self.height() * 0.9))
         self.widget4.resize(int(self.width() * 0.9), int(self.height() * 0.9))
         if self.__system__ == "Windows":
@@ -585,43 +589,47 @@
 
     def tab0_init(self) -> None:
         """
         initialize tab0
         """
         self.tab0.grid = QGridLayout(self.tab0)
         text = QTextEdit(self.tab0)
-        text.setStyleSheet("border-radius:15px")
-        text.setFocusPolicy(QtCore.Qt.NoFocus)
+        text.setStyleSheet("border-radius:15px;font-size:20pt")
+        text.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
         text.setReadOnly(True)
         text.setHtml(
             """
             <h1 style='color:#02554e;font-family:Verdana'>Welcome 🎃🎉</h1>
-            <p style='color:#333;font-family:Verdana'>Out [1]: Welcome to pyPDFeditor-GUI.</p>
-            <p style='color:#333;font-family:Verdana'>Out [2]: pyPDFeditor-GUI is a cross-platform 
+            <p style='color:#333;font-family:Verdana;font-size:12pt'>Out [1]: Welcome to pyPDFeditor-GUI.</p>
+            <p style='color:#333;font-family:Verdana;font-size:12pt'>Out [2]: pyPDFeditor-GUI is a cross-platform 
             application, thanks to <u>Python</u>, <u>PyQt5</u> and <u>PyMuPDF</u>, 
             designed to work on simple PDF handling.</p>
-            <p style='color:#333;font-family:Verdana'>Out [3]: STAND WITH UKRAINE 🇺🇦</p>
-            <p style='color:#333;font-family:Verdana'>Out [4]: STAND WITH ISRAEL 🇮🇱</p>
-            <p style='color:#333;font-family:Verdana'>Out [5]: ...</p>
+            <p style='color:#333;font-family:Verdana;font-size:12pt'>Out [3]: STAND WITH UKRAINE 🇺🇦</p>
+            <p style='color:#333;font-family:Verdana;font-size:12pt'>Out [4]: STAND WITH ISRAEL 🇮🇱</p>
+            <p style='color:#333;font-family:Verdana;font-size:12pt'>Out [5]: ...</p>
             """
         )
         shadow(text, QColor(0, 0, 0, 90), 10)
         label_w = QLabel(self.tab0)
         label_w.setStyleSheet(LABEL_STYLE)
         label_w.setText(
             "<a href='https://github.com/Augus1999/pyPDFeditor-GUI/' style='color:#a3b5b3'>"
             "<small>https://github.com/Augus1999/pyPDFeditor-GUI</small></a>",
         )
         label_w.setOpenExternalLinks(True)
         self.tab0.label_v = QLabel(self.tab0)
         self.tab0.label_v.setStyleSheet(LABEL_STYLE)
         self.tab0.label_v.setText(f"⌛ version {self.__version__}")
         self.tab0.grid.addWidget(text, 5, 0, 20, 21)
-        self.tab0.grid.addWidget(self.tab0.label_v, 31, 0, 1, 5, QtCore.Qt.AlignBottom)
-        self.tab0.grid.addWidget(label_w, 31, 17, 1, 4, QtCore.Qt.AlignBottom)
+        self.tab0.grid.addWidget(
+            self.tab0.label_v, 31, 0, 1, 5, QtCore.Qt.AlignmentFlag.AlignBottom
+        )
+        self.tab0.grid.addWidget(
+            label_w, 31, 17, 1, 4, QtCore.Qt.AlignmentFlag.AlignBottom
+        )
 
     def tab1_init(self) -> None:
         """
         initialize tab1
         """
         self.tab1.grid = QGridLayout(self.tab1)
         self.tab1.table = QTableWidget(self.tab1)
@@ -644,24 +652,24 @@
         self.tab1.button1.setFixedSize(52, 26)
         self.tab1.button2.setFixedSize(52, 26)
         self.tab1.button3.setFixedSize(52, 26)
         self.tab1.button4.setFixedSize(52, 26)
         self.tab1.table.setShowGrid(False)
         self.tab1.table.verticalHeader().setVisible(False)
         self.tab1.table.horizontalHeader().setVisible(False)
-        self.tab1.table.setFocusPolicy(QtCore.Qt.NoFocus)
+        self.tab1.table.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
         self.tab1.table.setHorizontalScrollBarPolicy(
-            QtCore.Qt.ScrollBarAlwaysOff,
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff,
         )
         self.tab1.table.setEditTriggers(
-            QtWidgets.QAbstractItemView.NoEditTriggers,
+            QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers,
         )
         self.tab1.table.setStyleSheet(TABLE_STYLE1)
         self.tab1.table.setContextMenuPolicy(
-            QtCore.Qt.CustomContextMenu,
+            QtCore.Qt.ContextMenuPolicy.CustomContextMenu,
         )
         self.tab1.grid.addWidget(self.tab1.button1, 0, 0)
         self.tab1.grid.addWidget(self.tab1.button2, 0, 1)
         self.tab1.grid.addWidget(self.tab1.button4, 0, 2)
         self.tab1.grid.addWidget(self.tab1.table, 1, 0, 10, 21)
 
     def tab2_init(self) -> None:
@@ -690,23 +698,23 @@
         self.tab2.button2.setFixedSize(52, 26)
         self.tab2.button3.setFixedSize(52, 26)
         self.tab2.button4.setFixedSize(52, 26)
         self.tab2.table.setShowGrid(False)
         self.tab2.table.verticalHeader().setVisible(False)
         self.tab2.table.horizontalHeader().setVisible(False)
         self.tab2.table.setStyleSheet(TABLE_STYLE1)
-        self.tab2.table.setFocusPolicy(QtCore.Qt.NoFocus)
+        self.tab2.table.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
         self.tab2.table.setHorizontalScrollBarPolicy(
-            QtCore.Qt.ScrollBarAlwaysOff,
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff,
         )
         self.tab2.table.setEditTriggers(
-            QtWidgets.QAbstractItemView.NoEditTriggers,
+            QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers,
         )
         self.tab2.table.setContextMenuPolicy(
-            QtCore.Qt.CustomContextMenu,
+            QtCore.Qt.ContextMenuPolicy.CustomContextMenu,
         )
         self.tab2.grid.addWidget(self.tab2.button1, 0, 0)
         self.tab2.grid.addWidget(self.tab2.button2, 0, 1)
         self.tab2.grid.addWidget(self.tab2.button4, 0, 2)
         self.tab2.grid.addWidget(self.tab2.table, 1, 0, 10, 21)
 
     def tab3_init(self) -> None:
@@ -719,26 +727,28 @@
         layout = QGridLayout(self.widget3)
         scroll_area.setWidget(self.widget3)
         self.tab3.grid = QGridLayout(self.tab3)
         self.tab3.table = QTableWidget(self.tab3)
         self.tab3.table.setShowGrid(False)
         self.tab3.table.verticalHeader().setVisible(False)
         self.tab3.table.horizontalHeader().setVisible(False)
-        self.tab3.table.setFocusPolicy(QtCore.Qt.NoFocus)
+        self.tab3.table.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
         self.tab3.table.setVerticalScrollBarPolicy(
-            QtCore.Qt.ScrollBarAlwaysOff,
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff,
         )
         self.tab3.table.setHorizontalScrollBarPolicy(
-            QtCore.Qt.ScrollBarAlwaysOff,
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff,
         )
         self.tab3.table.setEditTriggers(
-            QtWidgets.QAbstractItemView.NoEditTriggers,
+            QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers,
         )
         self.tab3.table.setStyleSheet(TABLE_STYLE2)
-        self.tab3.table.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
+        self.tab3.table.setContextMenuPolicy(
+            QtCore.Qt.ContextMenuPolicy.CustomContextMenu
+        )
         self.tab3.button1 = QPushButton(self.tab3)
         self.tab3.button2 = QPushButton(self.tab3)
         self.tab3.button3 = QPushButton(self.tab3)
         self.tab3.button4 = QPushButton(self.tab3)
         self.tab3.button5 = QPushButton(self.tab3)
         self.tab3.button6 = QPushButton(self.tab3)
         self.tab3.button7 = QPushButton(self.tab3)
@@ -829,26 +839,26 @@
         self.tab3.label3.setFixedSize(35, 35)
         self.tab3.label6.setFixedSize(35, 35)
         self.tab3.label10.setFixedSize(35, 35)
         self.tab3.label3.setText("pt")
         self.tab3.label6.setText("%")
         self.tab3.label8.setText("* " * 20)
         self.tab3.label10.setText("°")
-        self.tab3.label1.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label2.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label3.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label4.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label5.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label6.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label7.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label8.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label9.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label10.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label11.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab3.label12.setAlignment(QtCore.Qt.AlignCenter)
+        self.tab3.label1.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label2.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label3.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label4.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label5.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label6.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label7.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label8.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label9.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label10.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label11.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab3.label12.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.tab3.check = SwitchBtn(self.tab3)
         self.tab3.check1 = SwitchBtn(self.tab3)
         self.tab3.check2 = SwitchBtn(self.tab3)
         self.tab3.check.setFixedSize(70, 26)
         self.tab3.check1.setFixedSize(70, 26)
         self.tab3.check2.setFixedSize(70, 26)
         self.tab3.check.setChecked(True)
@@ -857,41 +867,95 @@
         self.tab3.check.setStyleSheet(SWITCH_STYLE)
         self.tab3.check1.setStyleSheet(SWITCH_STYLE)
         self.tab3.check2.setStyleSheet(SWITCH_STYLE)
         self.tab3.grid.addWidget(self.tab3.button1, 0, 0)
         self.tab3.grid.addWidget(self.tab3.button2, 0, 1)
         self.tab3.grid.addWidget(self.tab3.button8, 0, 2)
         self.tab3.grid.addWidget(scroll_area, 1, 0, 20, 21)
-        layout.addWidget(self.tab3.table, 0, 0, 14, 10, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.label1, 0, 14, 1, 5, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.line1, 1, 14, 1, 5, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.line2, 2, 14, 1, 5, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.label2, 3, 14, 1, 5, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.text, 4, 14, 2, 5, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.label4, 6, 14, 1, 2, QtCore.Qt.AlignRight)
-        layout.addWidget(self.tab3.label7, 7, 14, 1, 2, QtCore.Qt.AlignRight)
-        layout.addWidget(self.tab3.label9, 8, 14, 1, 2, QtCore.Qt.AlignRight)
-        layout.addWidget(self.tab3.line3, 6, 16, 1, 1, QtCore.Qt.AlignRight)
-        layout.addWidget(self.tab3.line4, 7, 16, 1, 1, QtCore.Qt.AlignRight)
-        layout.addWidget(self.tab3.line5, 8, 16, 1, 1, QtCore.Qt.AlignRight)
-        layout.addWidget(self.tab3.label3, 6, 17, 1, 1, QtCore.Qt.AlignLeft)
-        layout.addWidget(self.tab3.label6, 7, 17, 1, 1, QtCore.Qt.AlignLeft)
-        layout.addWidget(self.tab3.label10, 8, 17, 1, 1, QtCore.Qt.AlignLeft)
-        layout.addWidget(self.tab3.button7, 6, 18, 1, 1, QtCore.Qt.AlignLeft)
-        layout.addWidget(self.tab3.button9, 6, 18, 1, 1, QtCore.Qt.AlignRight)
-        layout.addWidget(self.tab3.button4, 7, 18, 1, 1, QtCore.Qt.AlignLeft)
-        layout.addWidget(self.tab3.button5, 8, 18, 1, 1, QtCore.Qt.AlignLeft)
-        layout.addWidget(self.tab3.label8, 9, 14, 1, 5, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.label12, 10, 14, 1, 2, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.label11, 11, 14, 1, 2, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.label5, 12, 14, 1, 2, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.check2, 10, 16, 1, 2, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.check1, 11, 16, 1, 2, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.check, 12, 16, 1, 2, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab3.button6, 10, 18, 1, 1, QtCore.Qt.AlignLeft)
+        layout.addWidget(
+            self.tab3.table, 0, 0, 14, 10, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.label1, 0, 14, 1, 5, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.line1, 1, 14, 1, 5, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.line2, 2, 14, 1, 5, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.label2, 3, 14, 1, 5, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.text, 4, 14, 2, 5, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.label4, 6, 14, 1, 2, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+        layout.addWidget(
+            self.tab3.label7, 7, 14, 1, 2, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+        layout.addWidget(
+            self.tab3.label9, 8, 14, 1, 2, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+        layout.addWidget(
+            self.tab3.line3, 6, 16, 1, 1, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+        layout.addWidget(
+            self.tab3.line4, 7, 16, 1, 1, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+        layout.addWidget(
+            self.tab3.line5, 8, 16, 1, 1, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+        layout.addWidget(
+            self.tab3.label3, 6, 17, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft
+        )
+        layout.addWidget(
+            self.tab3.label6, 7, 17, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft
+        )
+        layout.addWidget(
+            self.tab3.label10, 8, 17, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft
+        )
+        layout.addWidget(
+            self.tab3.button7, 6, 18, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft
+        )
+        layout.addWidget(
+            self.tab3.button9, 6, 18, 1, 1, QtCore.Qt.AlignmentFlag.AlignRight
+        )
+        layout.addWidget(
+            self.tab3.button4, 7, 18, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft
+        )
+        layout.addWidget(
+            self.tab3.button5, 8, 18, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft
+        )
+        layout.addWidget(
+            self.tab3.label8, 9, 14, 1, 5, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.label12, 10, 14, 1, 2, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.label11, 11, 14, 1, 2, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.label5, 12, 14, 1, 2, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.check2, 10, 16, 1, 2, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.check1, 11, 16, 1, 2, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.check, 12, 16, 1, 2, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab3.button6, 10, 18, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft
+        )
 
     def tab4_init(self) -> None:
         """
         initialize tab4
         """
         scroll_area = QScrollArea()
         scroll_area.setStyleSheet(SCROLL_AREA_STYLE)
@@ -919,41 +983,44 @@
         self.tab4.button2.setFixedSize(52, 26)
         self.tab4.button3.setFixedSize(52, 26)
         self.tab4.button4.setFixedSize(52, 26)
         self.tab4.table = TableWidget(self.tab4)
         self.tab4.table.setShowGrid(False)
         self.tab4.table.verticalHeader().setVisible(False)
         self.tab4.table.horizontalHeader().setVisible(False)
-        self.tab4.table.setFocusPolicy(QtCore.Qt.NoFocus)
+        self.tab4.table.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
         self.tab4.table.setHorizontalScrollBarPolicy(
-            QtCore.Qt.ScrollBarAlwaysOff,
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff,
         )
         self.tab4.table.setEditTriggers(
-            QtWidgets.QAbstractItemView.NoEditTriggers,
+            QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers,
         )
         self.tab4.table.setStyleSheet(TABLE_STYLE2)
         self.tab4.text = QTextEdit(self.tab4)
         self.tab4.text.setStyleSheet(TEXTEDIT_STYLE)
         self.tab4.text.setLineWrapColumnOrWidth(2000)
-        self.tab4.text.setLineWrapMode(QTextEdit.FixedPixelWidth)
+        self.tab4.text.setLineWrapMode(QTextEdit.LineWrapMode.FixedPixelWidth)
         self.tab4.label0 = QLabel(self.tab4)
         self.tab4.label1 = QLabel(self.tab4)
         self.tab4.label2 = QLabel(self.tab4)
         self.tab4.label3 = QLabel(self.tab4)
         self.tab4.label4 = QLabel(self.tab4)
         self.tab4.label5 = QLabel(self.tab4)
         self.tab4.label0.setStyleSheet(LABEL_STYLE)
         self.tab4.label1.setStyleSheet(LABEL_STYLE)
         self.tab4.label2.setStyleSheet(LABEL_STYLE)
         self.tab4.label3.setStyleSheet(LABEL_STYLE)
         self.tab4.label4.setStyleSheet(LABEL_STYLE)
         self.tab4.label5.setStyleSheet(LABEL_STYLE)
         self.tab4.label1.setPixmap(
             QPixmap(str(icon_path / "book2.svg")).scaled(
-                180, 180, QtCore.Qt.IgnoreAspectRatio, QtCore.Qt.SmoothTransformation
+                180,
+                180,
+                QtCore.Qt.AspectRatioMode.IgnoreAspectRatio,
+                QtCore.Qt.TransformationMode.SmoothTransformation,
             ),
         )
         self.tab4.line1 = QLineEdit(self.tab4)
         self.tab4.line2 = QLineEdit(self.tab4)
         self.tab4.line3 = QLineEdit(self.tab4)
         self.tab4.line4 = QLineEdit(self.tab4)
         self.tab4.line1.setStyleSheet(LINE_EDIT_STYLE)
@@ -961,35 +1028,60 @@
         self.tab4.line3.setStyleSheet(LINE_EDIT_STYLE)
         self.tab4.line4.setStyleSheet(LINE_EDIT_STYLE)
         self.tab4.line1.setFixedSize(312, 35)
         self.tab4.line2.setFixedSize(312, 35)
         self.tab4.line3.setFixedSize(312, 35)
         self.tab4.line4.setFixedSize(312, 35)
         self.tab4.text.setFixedSize(312, 450)
-        self.tab4.line1.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab4.line2.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab4.line3.setAlignment(QtCore.Qt.AlignCenter)
-        self.tab4.line4.setAlignment(QtCore.Qt.AlignCenter)
+        self.tab4.line1.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab4.line2.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab4.line3.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.tab4.line4.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.tab4.grid.addWidget(self.tab4.button1, 0, 0)
         self.tab4.grid.addWidget(self.tab4.button2, 0, 1)
         self.tab4.grid.addWidget(self.tab4.button4, 0, 2)
         self.tab4.grid.addWidget(scroll_area, 1, 0, 20, 21)
-        layout.addWidget(self.tab4.text, 4, 0, 8, 7, QtCore.Qt.AlignCenter)
+        layout.addWidget(
+            self.tab4.text, 4, 0, 8, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
         layout.addWidget(self.tab4.table, 0, 7, 20, 7)
-        layout.addWidget(self.tab4.label1, 1, 0, 3, 5, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.label2, 1, 14, 1, 7, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.label3, 3, 14, 1, 7, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.label4, 5, 14, 1, 7, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.label5, 7, 14, 1, 7, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.line1, 2, 14, 1, 7, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.line2, 4, 14, 1, 7, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.line3, 6, 14, 1, 7, QtCore.Qt.AlignCenter)
-        layout.addWidget(self.tab4.line4, 8, 14, 1, 7, QtCore.Qt.AlignCenter)
         layout.addWidget(
-            self.tab4.label0, 19, 0, 1, 3, QtCore.Qt.AlignLeft | QtCore.Qt.AlignBottom
+            self.tab4.label1, 1, 0, 3, 5, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.label2, 1, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.label3, 3, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.label4, 5, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.label5, 7, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.line1, 2, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.line2, 4, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.line3, 6, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.line4, 8, 14, 1, 7, QtCore.Qt.AlignmentFlag.AlignCenter
+        )
+        layout.addWidget(
+            self.tab4.label0,
+            19,
+            0,
+            1,
+            3,
+            QtCore.Qt.AlignmentFlag.AlignLeft | QtCore.Qt.AlignmentFlag.AlignBottom,
         )
 
 
 class SettingR(QWidget):
     """
     setting window
     """
@@ -997,18 +1089,19 @@
     def __init__(self):
         super().__init__()
         grid = QGridLayout(self)
         self.setFixedSize(600, 280)
         self.setWindowTitle("Setting")
         self.setWindowIcon(QIcon(str(icon_path / "settings.svg")))
         self.setWindowFlags(
-            QtCore.Qt.CustomizeWindowHint | QtCore.Qt.WindowCloseButtonHint,
+            QtCore.Qt.WindowType.CustomizeWindowHint
+            | QtCore.Qt.WindowType.WindowCloseButtonHint,
         )
         self.setStyleSheet("background-color:#ffffff")
-        self.setWindowModality(QtCore.Qt.ApplicationModal)
+        self.setWindowModality(QtCore.Qt.WindowModality.ApplicationModal)
         self.label1 = QLabel(self)
         self.label2 = QLabel(self)
         self.label3 = QLabel(self)
         self.check = SwitchBtn(self)
         self.line1 = QLineEdit(self)
         self.line2 = QLineEdit(self)
         self.button1 = QPushButton(self)
@@ -1020,32 +1113,32 @@
         self.label1.setStyleSheet(LABEL_STYLE)
         self.label2.setStyleSheet(LABEL_STYLE)
         self.label3.setStyleSheet(LABEL_STYLE)
         self.check.setStyleSheet(SWITCH_STYLE)
         self.combobox.setStyleSheet(COMBO_BOX_STYLE)
         self.line1.setStyleSheet(LINE_EDIT_STYLE)
         self.line2.setStyleSheet(LINE_EDIT_STYLE)
-        self.label1.setAlignment(QtCore.Qt.AlignVCenter)
-        self.label2.setAlignment(QtCore.Qt.AlignVCenter)
-        self.label3.setAlignment(QtCore.Qt.AlignVCenter)
+        self.label1.setAlignment(QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.label2.setAlignment(QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.label3.setAlignment(QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.check.setFixedSize(80, 30)
         self.line1.setFixedSize(400, 40)
         self.line2.setFixedSize(400, 40)
         self.button1.setFixedSize(28, 28)
         self.button2.setFixedSize(28, 28)
         self.combobox.setFixedSize(170, 40)
-        grid.addWidget(self.label1, 0, 0, 1, 5, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label2, 1, 0, 1, 5, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label3, 2, 0, 1, 7, QtCore.Qt.AlignLeft)
+        grid.addWidget(self.label1, 0, 0, 1, 5, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label2, 1, 0, 1, 5, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label3, 2, 0, 1, 7, QtCore.Qt.AlignmentFlag.AlignLeft)
         grid.addWidget(self.combobox, 3, 0)
         grid.addWidget(self.line1, 0, 5, 1, 10)
         grid.addWidget(self.line2, 1, 5, 1, 10)
-        grid.addWidget(self.button1, 0, 14, 1, 1, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.button2, 1, 14, 1, 1, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.check, 2, 13, 1, 2, QtCore.Qt.AlignHCenter)
+        grid.addWidget(self.button1, 0, 14, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.button2, 1, 14, 1, 1, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.check, 2, 13, 1, 2, QtCore.Qt.AlignmentFlag.AlignHCenter)
         self.setWindowOpacity(0.92)
 
 
 class PermMenuR(QWidget):
     """
     permission setting menu window
     """
@@ -1054,17 +1147,18 @@
         super().__init__()
         grid = QGridLayout(self)
         self.setFixedSize(480, 400)
         self.setWindowTitle(" ")
         self.setWindowIcon(QIcon(str(icon_path / "lock.svg")))
         self.setStyleSheet("background-color:#ffffff")
         self.setWindowFlags(
-            QtCore.Qt.CustomizeWindowHint | QtCore.Qt.WindowCloseButtonHint,
+            QtCore.Qt.WindowType.CustomizeWindowHint
+            | QtCore.Qt.WindowType.WindowCloseButtonHint,
         )
-        self.setWindowModality(QtCore.Qt.ApplicationModal)
+        self.setWindowModality(QtCore.Qt.WindowModality.ApplicationModal)
         self.check1 = SwitchBtn(self)
         self.check2 = SwitchBtn(self)
         self.check3 = SwitchBtn(self)
         self.check4 = SwitchBtn(self)
         self.check5 = SwitchBtn(self)
         self.check6 = SwitchBtn(self)
         self.check7 = SwitchBtn(self)
@@ -1081,22 +1175,22 @@
         self.check2.setFixedSize(80, 30)
         self.check3.setFixedSize(80, 30)
         self.check4.setFixedSize(80, 30)
         self.check5.setFixedSize(80, 30)
         self.check6.setFixedSize(80, 30)
         self.check7.setFixedSize(80, 30)
         self.check8.setFixedSize(80, 30)
-        grid.addWidget(self.label1, 0, 0, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label2, 1, 0, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label3, 2, 0, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label4, 3, 0, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label5, 4, 0, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label6, 5, 0, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label7, 6, 0, QtCore.Qt.AlignLeft)
-        grid.addWidget(self.label8, 7, 0, QtCore.Qt.AlignLeft)
+        grid.addWidget(self.label1, 0, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label2, 1, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label3, 2, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label4, 3, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label5, 4, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label6, 5, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label7, 6, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
+        grid.addWidget(self.label8, 7, 0, QtCore.Qt.AlignmentFlag.AlignLeft)
         grid.addWidget(self.check1, 0, 1)
         grid.addWidget(self.check2, 1, 1)
         grid.addWidget(self.check3, 2, 1)
         grid.addWidget(self.check4, 3, 1)
         grid.addWidget(self.check5, 4, 1)
         grid.addWidget(self.check6, 5, 1)
         grid.addWidget(self.check7, 6, 1)
@@ -1132,18 +1226,19 @@
     def __init__(self):
         super().__init__()
         grid = QGridLayout(self)
         self.setFixedSize(486, 324)
         self.setWindowTitle("Select Font")
         self.setWindowIcon(QIcon(str(icon_path / "font.svg")))
         self.setWindowFlags(
-            QtCore.Qt.CustomizeWindowHint | QtCore.Qt.WindowCloseButtonHint,
+            QtCore.Qt.WindowType.CustomizeWindowHint
+            | QtCore.Qt.WindowType.WindowCloseButtonHint,
         )
-        self.setWindowModality(QtCore.Qt.ApplicationModal)
+        self.setWindowModality(QtCore.Qt.WindowModality.ApplicationModal)
         self.combobox = QComboBox(self)
         self.combobox.setStyleSheet(COMBO_BOX_STYLE)
         self.combobox.setFixedHeight(45)
         self.label = QLabel(self)
-        self.label.setAlignment(QtCore.Qt.AlignTop)
-        grid.addWidget(self.combobox, 0, 0, QtCore.Qt.AlignCenter)
-        grid.addWidget(self.label, 1, 0, QtCore.Qt.AlignCenter)
+        self.label.setAlignment(QtCore.Qt.AlignmentFlag.AlignTop)
+        grid.addWidget(self.combobox, 0, 0, QtCore.Qt.AlignmentFlag.AlignCenter)
+        grid.addWidget(self.label, 1, 0, QtCore.Qt.AlignmentFlag.AlignCenter)
         self.setWindowOpacity(0.92)
```

### Comparing `pyPDFeditor-GUI-2.3.0/setup.py` & `pypdfeditor_gui-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     long_description_content_type="text/markdown",
     author="Nianze A. TAO",
     author_email="Augus_1999@outlook.com",
     packages=["pypdfeditor_core"],
     package_dir={"pypdfeditor_core": "pypdfeditor_core"},
     license="MIT",
     python_requires=">=3.7",
-    install_requires=["PyMuPDF>=1.19.2", "PyQt5>=5.15.4"],
+    install_requires=["PyMuPDF>=1.24.3", "PyQt6>=6.7.0"],
     url="https://github.com/Augus1999/pyPDFeditor-GUI/",
     project_urls={"Source": "https://github.com/Augus1999/pyPDFeditor-GUI"},
     include_package_data=True,
     package_data={"pypdfeditor_core": ["icons/*.svg", "icons/*.py"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
```

