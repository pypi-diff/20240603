# Comparing `tmp/almax_common-1.0.5.dev20240601232428.tar.gz` & `tmp/almax_common-1.0.5.dev20240602164342.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.5.dev20240601232428.tar", last modified: Sat Jun  1 23:24:30 2024, max compression
+gzip compressed data, was "almax_common-1.0.5.dev20240602164342.tar", last modified: Sun Jun  2 16:43:45 2024, max compression
```

## Comparing `almax_common-1.0.5.dev20240601232428.tar` & `almax_common-1.0.5.dev20240602164342.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.981844 almax_common-1.0.5.dev20240601232428/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.977844 almax_common-1.0.5.dev20240601232428/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.977844 almax_common-1.0.5.dev20240601232428/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.977844 almax_common-1.0.5.dev20240601232428/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.977844 almax_common-1.0.5.dev20240601232428/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.977844 almax_common-1.0.5.dev20240601232428/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxUtils/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 23:24:30.981844 almax_common-1.0.5.dev20240601232428/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.981844 almax_common-1.0.5.dev20240601232428/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-01 23:24:30.000000 almax_common-1.0.5.dev20240601232428/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-06-01 23:24:30.000000 almax_common-1.0.5.dev20240601232428/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 23:24:30.000000 almax_common-1.0.5.dev20240601232428/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 23:24:30.000000 almax_common-1.0.5.dev20240601232428/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 23:24:30.000000 almax_common-1.0.5.dev20240601232428/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 23:24:30.981844 almax_common-1.0.5.dev20240601232428/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 23:24:30.981844 almax_common-1.0.5.dev20240601232428/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/tests/test_AlmaxUtilsGeneric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/tests/test_AlmaxUtilsPdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-01 23:24:19.000000 almax_common-1.0.5.dev20240601232428/tests/test_AlmaxUtilsTime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.232867 almax_common-1.0.5.dev20240602164342/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.228867 almax_common-1.0.5.dev20240602164342/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.228867 almax_common-1.0.5.dev20240602164342/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.228867 almax_common-1.0.5.dev20240602164342/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.228867 almax_common-1.0.5.dev20240602164342/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.228867 almax_common-1.0.5.dev20240602164342/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxUtils/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-02 16:43:45.232867 almax_common-1.0.5.dev20240602164342/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.232867 almax_common-1.0.5.dev20240602164342/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-02 16:43:45.000000 almax_common-1.0.5.dev20240602164342/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-06-02 16:43:45.000000 almax_common-1.0.5.dev20240602164342/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:43:45.000000 almax_common-1.0.5.dev20240602164342/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-02 16:43:45.000000 almax_common-1.0.5.dev20240602164342/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 16:43:45.000000 almax_common-1.0.5.dev20240602164342/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:43:45.232867 almax_common-1.0.5.dev20240602164342/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:43:45.232867 almax_common-1.0.5.dev20240602164342/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/tests/test_AlmaxUtilsGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/tests/test_AlmaxUtilsPdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-06-02 16:43:34.000000 almax_common-1.0.5.dev20240602164342/tests/test_AlmaxUtilsTime.py
```

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxClasses/__init__.py` & `almax_common-1.0.5.dev20240602164342/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.5.dev20240602164342/AlmaxGraphics/FrameManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,93 +1,16 @@
 import tkinter as TK;
 from tkinter import ttk;
 from tkinter import messagebox;
+from tkcalendar import DateEntry;
 import sys;
 
 WindowElementsDefaultPaddingWidth = 10;
 WindowElementsDefaultPaddingHeight = 10;
 
-def WindowCreateLabel(
-    Window: TK.Tk,
-    Text: str
-) -> TK.Label:
-    WindowLabel = TK.Label(
-        Window,
-        text=Text,
-        padx=WindowElementsDefaultPaddingWidth,
-        pady=WindowElementsDefaultPaddingHeight,
-        anchor=TK.W
-    );
-    return WindowLabel;
-
-def WindowCreateButton(
-    Window: TK.Tk,
-    Text: str,
-    CommandIndex: int,
-    AssignCommand
-) -> TK.Button:
-    WindowButton = TK.Button(
-        Window,
-        text = Text,
-        command = lambda: AssignCommand(WindowButton, CommandIndex),
-        width=WindowElementsDefaultPaddingWidth,
-        padx=WindowElementsDefaultPaddingWidth
-    );
-    return WindowButton;
-
-def WindowCreateRadioButton(
-    Window: TK.Tk,
-    Options: list,
-    WindowRadioButtonSelected: TK.IntVar
-):
-    radioButtons = [];
-    for (optionLabel, optionValue) in Options:
-        radioButtons.append(TK.Radiobutton(
-            Window,
-            text = optionLabel,
-            value = optionValue,
-            variable=WindowRadioButtonSelected,
-            width=WindowElementsDefaultPaddingWidth
-        ));
-    return radioButtons;
-
-def WindowCreateProgressbar(
-   Window: TK.Tk
-):
-    progressbar = ttk.Progressbar(
-        Window,
-        mode="determinate",
-        orient="horizontal",
-        maximum=100,
-        length=286
-    );
-    return progressbar;
-     
-class ProgressbarProgression:
-    def __init__(
-        self,
-        progressbarRow: ttk.Progressbar,
-        progressbarPercRow: TK.Label,
-        progressRatio: int = 50
-    ):
-        self.__Progression = 0;
-        self.__ProgressbarRow = progressbarRow;
-        self.__ProgressbarPercRow = progressbarPercRow;
-        self.__ProgressRatio = progressRatio;
-   
-    def Update(self):
-        self.__Progression += self.__ProgressRatio;
-        self.__ProgressbarRow["value"] = self.__Progression;
-        self.__ProgressbarRow.update();
-        self.__ProgressbarPercRow["text"] = str(round(self.__Progression, 2)) + "%";
-        self.__ProgressbarPercRow.update();
-
-    def ChangeProgressionRatio(self, progressionRatio: int):
-        self.__ProgressRatio = progressionRatio;
-
 class Window:
     def __init__(
         self,
         programName: str
     ):
         self.__Istance = TK.Tk();
         self.__Istance.resizable(False, False);
@@ -131,14 +54,24 @@
             WindowProgressionProgressbarRow,
             self.AddLabelToFrame("0%", "Progressbar", TK.LEFT)
         );
 
         WindowProgressionProgressbarRow.pack(in_=self.__Frames[frameName], side=TK.LEFT);
         return Progression;
 
+    def AddCalendarToFrame(self, frameName, position, defaultYear = 2024, defaultMoth = 1, defaultDay = 1):
+        date_entry = DateEntry(
+            self.__Istance, 
+            year=defaultYear, 
+            month=defaultMoth, 
+            day=defaultDay
+        );
+        date_entry.pack(in_=self.__Frames[frameName], side=position);
+        return date_entry;
+
     def DisableAllButtons(self):
         for button in self.__ButtonsToDisable:
             button["state"] = "disabled";
         for rbutton in self.__RadioButtons:
             rbutton["state"] = "disabled";
 
     def Resize(self):
@@ -169,8 +102,86 @@
 
     def Quit(self, message: str = ''):
         if message != '':
             messagebox.showerror(self.__Istance.title(), message);
         print(f"{self.__Istance.title()} è stato Terminato!");
         self.__IsRunning = False;
         self.__Istance.quit();
-        sys.exit();
+        sys.exit();
+   
+class ProgressbarProgression:
+    def __init__(
+        self,
+        progressbarRow: ttk.Progressbar,
+        progressbarPercRow: TK.Label,
+        progressRatio: int = 50
+    ):
+        self.__Progression = 0;
+        self.__ProgressbarRow = progressbarRow;
+        self.__ProgressbarPercRow = progressbarPercRow;
+        self.__ProgressRatio = progressRatio;
+   
+    def Update(self):
+        self.__Progression += self.__ProgressRatio;
+        self.__ProgressbarRow["value"] = self.__Progression;
+        self.__ProgressbarRow.update();
+        self.__ProgressbarPercRow["text"] = str(round(self.__Progression, 2)) + "%";
+        self.__ProgressbarPercRow.update();
+
+    def ChangeProgressionRatio(self, progressionRatio: int):
+        self.__ProgressRatio = progressionRatio;
+
+def WindowCreateLabel(
+    Window: TK.Tk,
+    Text: str
+) -> TK.Label:
+    WindowLabel = TK.Label(
+        Window,
+        text=Text,
+        padx=WindowElementsDefaultPaddingWidth,
+        pady=WindowElementsDefaultPaddingHeight,
+        anchor=TK.W
+    );
+    return WindowLabel;
+
+def WindowCreateButton(
+    Window: TK.Tk,
+    Text: str,
+    CommandIndex: int,
+    AssignCommand
+) -> TK.Button:
+    WindowButton = TK.Button(
+        Window,
+        text = Text,
+        command = lambda: AssignCommand(WindowButton, CommandIndex),
+        width=WindowElementsDefaultPaddingWidth,
+        padx=WindowElementsDefaultPaddingWidth
+    );
+    return WindowButton;
+
+def WindowCreateRadioButton(
+    Window: TK.Tk,
+    Options: list,
+    WindowRadioButtonSelected: TK.IntVar
+):
+    radioButtons = [];
+    for (optionLabel, optionValue) in Options:
+        radioButtons.append(TK.Radiobutton(
+            Window,
+            text = optionLabel,
+            value = optionValue,
+            variable=WindowRadioButtonSelected,
+            width=WindowElementsDefaultPaddingWidth
+        ));
+    return radioButtons;
+
+def WindowCreateProgressbar(
+   Window: TK.Tk
+):
+    progressbar = ttk.Progressbar(
+        Window,
+        mode="determinate",
+        orient="horizontal",
+        maximum=100,
+        length=286
+    );
+    return progressbar;
```

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxLogs/LoggerService.py` & `almax_common-1.0.5.dev20240602164342/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.5.dev20240602164342/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.5.dev20240602164342/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxUtils/FileSystem.py` & `almax_common-1.0.5.dev20240602164342/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxUtils/Generic.py` & `almax_common-1.0.5.dev20240602164342/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxUtils/PdfManager.py` & `almax_common-1.0.5.dev20240602164342/AlmaxUtils/PdfManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/AlmaxUtils/Time.py` & `almax_common-1.0.5.dev20240602164342/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/PKG-INFO` & `almax_common-1.0.5.dev20240602164342/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601232428
+Version: 1.0.5.dev20240602164342
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601232428/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.5.dev20240602164342/almax_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.5.dev20240601232428
+Version: 1.0.5.dev20240602164342
 Summary: Library with my most used Classes and Methods
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: chardet==5.2.0
 Requires-Dist: codicefiscale==0.9
 Requires-Dist: colorama==0.4.6
```

### Comparing `almax_common-1.0.5.dev20240601232428/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.5.dev20240602164342/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/setup.py` & `almax_common-1.0.5.dev20240602164342/setup.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/tests/test_AlmaxUtilsGeneric.py` & `almax_common-1.0.5.dev20240602164342/tests/test_AlmaxUtilsGeneric.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/tests/test_AlmaxUtilsPdfManager.py` & `almax_common-1.0.5.dev20240602164342/tests/test_AlmaxUtilsPdfManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.5.dev20240601232428/tests/test_AlmaxUtilsTime.py` & `almax_common-1.0.5.dev20240602164342/tests/test_AlmaxUtilsTime.py`

 * *Files identical despite different names*

