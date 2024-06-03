# Comparing `tmp/otsuwinAPI-2022.11.23.1.tar.gz` & `tmp/otsuwinAPI-2022.11.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otsuwinAPI-2022.11.23.1.tar", last modified: Tue Nov 22 15:22:46 2022, max compression
+gzip compressed data, was "otsuwinAPI-2022.11.30.tar", last modified: Tue Nov 29 15:14:25 2022, max compression
```

## Comparing `otsuwinAPI-2022.11.23.1.tar` & `otsuwinAPI-2022.11.30.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-11-22 15:22:46.564400 otsuwinAPI-2022.11.23.1/
--rw-rw-rw-   0        0        0      245 2022-11-22 15:22:46.563400 otsuwinAPI-2022.11.23.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-11-22 15:22:46.545336 otsuwinAPI-2022.11.23.1/otsuwinAPI/
--rw-rw-rw-   0        0        0      151 2022-11-22 15:21:36.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-22 15:22:46.562399 otsuwinAPI-2022.11.23.1/otsuwinAPI/constants/
--rw-rw-rw-   0        0        0       94 2022-11-21 02:49:14.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI/constants/__init__.py
--rw-rw-rw-   0        0        0      244 2022-11-21 02:44:24.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI/constants/hWndInsertAfter.py
--rw-rw-rw-   0        0        0      948 2022-11-21 02:51:35.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI/constants/uFlags.py
--rw-rw-rw-   0        0        0      568 2022-11-22 15:21:32.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI/kernel32.py
--rw-rw-rw-   0        0        0    11764 2022-11-22 15:21:30.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI/user32.py
-drwxrwxrwx   0        0        0        0 2022-11-22 15:22:46.556910 otsuwinAPI-2022.11.23.1/otsuwinAPI.egg-info/
--rw-rw-rw-   0        0        0      245 2022-11-22 15:22:46.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2022-11-22 15:22:46.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-22 15:22:46.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-11-22 15:22:46.000000 otsuwinAPI-2022.11.23.1/otsuwinAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-22 15:22:46.564400 otsuwinAPI-2022.11.23.1/setup.cfg
--rw-rw-rw-   0        0        0      403 2022-11-22 15:21:40.000000 otsuwinAPI-2022.11.23.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-29 15:14:25.191215 otsuwinAPI-2022.11.30/
+-rw-rw-rw-   0        0        0      243 2022-11-29 15:14:25.191215 otsuwinAPI-2022.11.30/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-11-29 15:14:25.170052 otsuwinAPI-2022.11.30/otsuwinAPI/
+-rw-rw-rw-   0        0        0      151 2022-11-22 15:21:36.000000 otsuwinAPI-2022.11.30/otsuwinAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-29 15:14:25.190221 otsuwinAPI-2022.11.30/otsuwinAPI/constants/
+-rw-rw-rw-   0        0        0      121 2022-11-29 14:35:37.000000 otsuwinAPI-2022.11.30/otsuwinAPI/constants/__init__.py
+-rw-rw-rw-   0        0        0      244 2022-11-21 02:44:24.000000 otsuwinAPI-2022.11.30/otsuwinAPI/constants/hWndInsertAfter.py
+-rw-rw-rw-   0        0        0      578 2022-11-29 14:55:21.000000 otsuwinAPI-2022.11.30/otsuwinAPI/constants/nCmdShow.py
+-rw-rw-rw-   0        0        0      948 2022-11-21 02:51:35.000000 otsuwinAPI-2022.11.30/otsuwinAPI/constants/uFlags.py
+-rw-rw-rw-   0        0        0      568 2022-11-22 15:21:32.000000 otsuwinAPI-2022.11.30/otsuwinAPI/kernel32.py
+-rw-rw-rw-   0        0        0    12277 2022-11-29 15:09:22.000000 otsuwinAPI-2022.11.30/otsuwinAPI/user32.py
+drwxrwxrwx   0        0        0        0 2022-11-29 15:14:25.184211 otsuwinAPI-2022.11.30/otsuwinAPI.egg-info/
+-rw-rw-rw-   0        0        0      243 2022-11-29 15:14:25.000000 otsuwinAPI-2022.11.30/otsuwinAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2022-11-29 15:14:25.000000 otsuwinAPI-2022.11.30/otsuwinAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-29 15:14:25.000000 otsuwinAPI-2022.11.30/otsuwinAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2022-11-29 15:14:25.000000 otsuwinAPI-2022.11.30/otsuwinAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-29 15:14:25.192720 otsuwinAPI-2022.11.30/setup.cfg
+-rw-rw-rw-   0        0        0      401 2022-11-29 15:09:06.000000 otsuwinAPI-2022.11.30/setup.py
```

### Comparing `otsuwinAPI-2022.11.23.1/otsuwinAPI/constants/uFlags.py` & `otsuwinAPI-2022.11.30/otsuwinAPI/constants/uFlags.py`

 * *Files identical despite different names*

### Comparing `otsuwinAPI-2022.11.23.1/otsuwinAPI/kernel32.py` & `otsuwinAPI-2022.11.30/otsuwinAPI/kernel32.py`

 * *Files identical despite different names*

### Comparing `otsuwinAPI-2022.11.23.1/otsuwinAPI/user32.py` & `otsuwinAPI-2022.11.30/otsuwinAPI/user32.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     - IsWindowEnabled
     - MoveWindow
     - SendMessageW
     - SetActiveWindow
     - SetFocus
     - SetForegroundWindow
     - SetWindowPos
+    - ShowWindow
     """
 
     @staticmethod
     def AttachThreadInput(idAttach: int, idAttachTo: int, fAttach: bool) -> bool:
         """スレッドの入力処理メカニズムを別のスレッドの入力処理メカニズムにアタッチまたはデタッチします。
 
         Args:
@@ -292,7 +293,20 @@
             cy (Optional[int], optional): ウィンドウの新しい高さ(ピクセル)。 Defaults to None.
             uFlags (Optional[int], optional): ウィンドウサイズ設定とフラグ。`constants.uFlags`内の定数を`|`演算子で組み合わせて使用。 Defaults to None.
 
         Returns:
             bool: 成否。
         """
         return bool(ctypes.windll.user32.SetWindowPos(hWnd, hWndInsertAfter, X, Y, cx, cy, uFlags))
+
+    @staticmethod
+    def ShowWindow(hWnd: int, nCmdShow: int) -> bool:
+        """指定したウィンドウの表示状態に設定します。
+
+        Args:
+            hWnd (int): ウィンドウハンドル。
+            nCmdShow (int): ウィンドウの表示方法。constants.nCmdShow内の定数を使用。
+
+        Returns:
+            bool: 以前のウィンドウの表示状態。
+        """
+        return bool(ctypes.windll.user32.ShowWindow(hWnd, nCmdShow))
```

