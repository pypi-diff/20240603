# Comparing `tmp/happylife-1.1.1.tar.gz` & `tmp/happylife-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happylife-1.1.1.tar", last modified: Wed May 29 04:17:04 2024, max compression
+gzip compressed data, was "happylife-1.1.2.tar", last modified: Mon Jun  3 10:15:02 2024, max compression
```

## Comparing `happylife-1.1.1.tar` & `happylife-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 04:17:04.731919 happylife-1.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-29 04:17:04.729973 happylife-1.1.1/HappyLife.egg-info/
--rw-rw-rw-   0        0        0     2838 2024-05-29 04:17:04.000000 happylife-1.1.1/HappyLife.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-29 04:17:04.000000 happylife-1.1.1/HappyLife.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 04:17:04.000000 happylife-1.1.1/HappyLife.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-29 04:17:04.000000 happylife-1.1.1/HappyLife.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       66 2024-05-29 04:17:04.000000 happylife-1.1.1/HappyLife.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-29 04:17:04.000000 happylife-1.1.1/HappyLife.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2838 2024-05-29 04:17:04.730946 happylife-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2346 2024-05-29 04:01:04.000000 happylife-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 04:17:04.729973 happylife-1.1.1/auto/
--rw-rw-rw-   0        0        0    30806 2024-05-29 04:16:28.000000 happylife-1.1.1/auto/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-29 04:17:04.731919 happylife-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-28 07:44:37.000000 happylife-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:15:02.874409 happylife-1.1.2/
+drwxrwxrwx   0        0        0        0 2024-06-03 10:15:02.873412 happylife-1.1.2/HappyLife.egg-info/
+-rw-rw-rw-   0        0        0     2818 2024-06-03 10:15:02.000000 happylife-1.1.2/HappyLife.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-06-03 10:15:02.000000 happylife-1.1.2/HappyLife.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:15:02.000000 happylife-1.1.2/HappyLife.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-03 10:15:02.000000 happylife-1.1.2/HappyLife.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       66 2024-06-03 10:15:02.000000 happylife-1.1.2/HappyLife.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-03 10:15:02.000000 happylife-1.1.2/HappyLife.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2818 2024-06-03 10:15:02.873412 happylife-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2024-06-03 10:11:59.000000 happylife-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:15:02.872418 happylife-1.1.2/auto/
+-rw-rw-rw-   0        0        0    31485 2024-06-03 10:05:20.000000 happylife-1.1.2/auto/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:15:02.874409 happylife-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-28 07:44:37.000000 happylife-1.1.2/setup.py
```

### Comparing `happylife-1.1.1/HappyLife.egg-info/PKG-INFO` & `happylife-1.1.2/HappyLife.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: HappyLife
-Version: 1.1.1
+Version: 1.1.2
 Summary: 圖色識別，自動操作滑鼠/鍵盤(可後臺運行)，將一切重複的事，抽象為函數，自動運行。
 Author: 宇宙中的塵埃
 Author-email: yqnacfmh9@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.24.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: pywin32==306
 
 # HappyLife
 
-HappyLife 解決重複無聊的事情，自動操作滑鼠/鍵盤，打遊戲刷副本/日常任務；線上課程定期機器人驗證。  
-不做重複的事，體驗有趣的事，讓人生更輕鬆。
+HappyLife 將重複的事情抽象為函數，自動運行。  
+不做無聊的事，體驗有趣的事，讓人生更輕鬆。
 
 安裝方法：
 ```shell
 pip install HappyLife
 ```
 ## 依賴關係
 
 安裝HappyLife會自動安裝依賴套件
 
 
 ## 使用教學
 
 ### 後臺操作（綁定窗口後，可以後臺運行，但窗口不能最小化，使用者可做別的事情）
 
->       from auto import Bw  # 引入類別
+>       from auto import Bd  # 引入類別
 
 >       # 綁定夜神模擬器方法  
->       bw = Bw("夜神模擬器")
+>       bd = Bd("夜神模擬器")
 
 >       # 綁定雷電模擬器方法(需額外綁定子窗口)  
->       bw = Bw('雷電模擬器');  
->       bw.bind_child_window(0)
+>       bd = Bd('雷電模擬器');  
+>       bd.bind_child_window(0)
 
->       bw.img_click(bw,'0.png')  # 點擊圖片  
->       bw.img_drag(bw,'1.png','2.png')  # 拖拽圖片，滑鼠從圖片1座標拖拽到圖片2座標的位置  
->       bw.lclick(55,64)   # 左鍵單擊  
->       bw.lclick2(55,64)  # 左鍵雙擊  
->       bw.rclick(55,64)   # 右鍵單擊  
+>       bd.img_click(bd,'0.png')  # 點擊圖片  
+>       bd.img_drag(bd,'1.png','2.png')  # 拖拽圖片，滑鼠從圖片1座標拖拽到圖片2座標的位置  
+>       bd.lclick(55,64)   # 左鍵單擊  
+>       bd.lclick2(55,64)  # 左鍵雙擊  
+>       bd.rclick(55,64)   # 右鍵單擊  
 
 
 ### 前臺操作（必須在當前窗口，才能運行，使用者無法做別的事情，通常後臺操作無效時才會使用此方法）
 
 >       from auto import Fd   # 引入類別
 
 >       Fd.img_click('1.png')   # 點擊圖片  
@@ -64,20 +64,20 @@
 
 * 如果使用前臺操作，無法自動操作滑鼠鍵盤，請用系統管理員身份啓動腳本
 
 ## 依序執行任務的方法
 
 >       # 要執行的任務列表
 >       tasks = [
->           (img_click, "81.png"),
->           (img_click, "82.png"),
->           (img_click, "83.png"),
->           (img_click, "84.png")
+>           (bd.img_click, bd,"81.png"),
+>           (bd.img_click, bd,"82.png"),
+>           (bd.img_click, bd,"83.png"),
+>           (bd.img_click, bd,"84.png")
 >       ]
->       # 按照順序執行任務
+>       # 按照順序執行任務，完成全部任務跳出迴圈
 >       execute_tasks_in_sequence(tasks)
```

### Comparing `happylife-1.1.1/PKG-INFO` & `happylife-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: HappyLife
-Version: 1.1.1
+Version: 1.1.2
 Summary: 圖色識別，自動操作滑鼠/鍵盤(可後臺運行)，將一切重複的事，抽象為函數，自動運行。
 Author: 宇宙中的塵埃
 Author-email: yqnacfmh9@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: numpy==1.24.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: pywin32==306
 
 # HappyLife
 
-HappyLife 解決重複無聊的事情，自動操作滑鼠/鍵盤，打遊戲刷副本/日常任務；線上課程定期機器人驗證。  
-不做重複的事，體驗有趣的事，讓人生更輕鬆。
+HappyLife 將重複的事情抽象為函數，自動運行。  
+不做無聊的事，體驗有趣的事，讓人生更輕鬆。
 
 安裝方法：
 ```shell
 pip install HappyLife
 ```
 ## 依賴關係
 
 安裝HappyLife會自動安裝依賴套件
 
 
 ## 使用教學
 
 ### 後臺操作（綁定窗口後，可以後臺運行，但窗口不能最小化，使用者可做別的事情）
 
->       from auto import Bw  # 引入類別
+>       from auto import Bd  # 引入類別
 
 >       # 綁定夜神模擬器方法  
->       bw = Bw("夜神模擬器")
+>       bd = Bd("夜神模擬器")
 
 >       # 綁定雷電模擬器方法(需額外綁定子窗口)  
->       bw = Bw('雷電模擬器');  
->       bw.bind_child_window(0)
+>       bd = Bd('雷電模擬器');  
+>       bd.bind_child_window(0)
 
->       bw.img_click(bw,'0.png')  # 點擊圖片  
->       bw.img_drag(bw,'1.png','2.png')  # 拖拽圖片，滑鼠從圖片1座標拖拽到圖片2座標的位置  
->       bw.lclick(55,64)   # 左鍵單擊  
->       bw.lclick2(55,64)  # 左鍵雙擊  
->       bw.rclick(55,64)   # 右鍵單擊  
+>       bd.img_click(bd,'0.png')  # 點擊圖片  
+>       bd.img_drag(bd,'1.png','2.png')  # 拖拽圖片，滑鼠從圖片1座標拖拽到圖片2座標的位置  
+>       bd.lclick(55,64)   # 左鍵單擊  
+>       bd.lclick2(55,64)  # 左鍵雙擊  
+>       bd.rclick(55,64)   # 右鍵單擊  
 
 
 ### 前臺操作（必須在當前窗口，才能運行，使用者無法做別的事情，通常後臺操作無效時才會使用此方法）
 
 >       from auto import Fd   # 引入類別
 
 >       Fd.img_click('1.png')   # 點擊圖片  
@@ -64,20 +64,20 @@
 
 * 如果使用前臺操作，無法自動操作滑鼠鍵盤，請用系統管理員身份啓動腳本
 
 ## 依序執行任務的方法
 
 >       # 要執行的任務列表
 >       tasks = [
->           (img_click, "81.png"),
->           (img_click, "82.png"),
->           (img_click, "83.png"),
->           (img_click, "84.png")
+>           (bd.img_click, bd,"81.png"),
+>           (bd.img_click, bd,"82.png"),
+>           (bd.img_click, bd,"83.png"),
+>           (bd.img_click, bd,"84.png")
 >       ]
->       # 按照順序執行任務
+>       # 按照順序執行任務，完成全部任務跳出迴圈
 >       execute_tasks_in_sequence(tasks)
```

### Comparing `happylife-1.1.1/README.md` & `happylife-1.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # HappyLife
 
-HappyLife 解決重複無聊的事情，自動操作滑鼠/鍵盤，打遊戲刷副本/日常任務；線上課程定期機器人驗證。  
-不做重複的事，體驗有趣的事，讓人生更輕鬆。
+HappyLife 將重複的事情抽象為函數，自動運行。  
+不做無聊的事，體驗有趣的事，讓人生更輕鬆。
 
 安裝方法：
 ```shell
 pip install HappyLife
 ```
 ## 依賴關係
 
 安裝HappyLife會自動安裝依賴套件
 
 
 ## 使用教學
 
 ### 後臺操作（綁定窗口後，可以後臺運行，但窗口不能最小化，使用者可做別的事情）
 
->       from auto import Bw  # 引入類別
+>       from auto import Bd  # 引入類別
 
 >       # 綁定夜神模擬器方法  
->       bw = Bw("夜神模擬器")
+>       bd = Bd("夜神模擬器")
 
 >       # 綁定雷電模擬器方法(需額外綁定子窗口)  
->       bw = Bw('雷電模擬器');  
->       bw.bind_child_window(0)
+>       bd = Bd('雷電模擬器');  
+>       bd.bind_child_window(0)
 
->       bw.img_click(bw,'0.png')  # 點擊圖片  
->       bw.img_drag(bw,'1.png','2.png')  # 拖拽圖片，滑鼠從圖片1座標拖拽到圖片2座標的位置  
->       bw.lclick(55,64)   # 左鍵單擊  
->       bw.lclick2(55,64)  # 左鍵雙擊  
->       bw.rclick(55,64)   # 右鍵單擊  
+>       bd.img_click(bd,'0.png')  # 點擊圖片  
+>       bd.img_drag(bd,'1.png','2.png')  # 拖拽圖片，滑鼠從圖片1座標拖拽到圖片2座標的位置  
+>       bd.lclick(55,64)   # 左鍵單擊  
+>       bd.lclick2(55,64)  # 左鍵雙擊  
+>       bd.rclick(55,64)   # 右鍵單擊  
 
 
 ### 前臺操作（必須在當前窗口，才能運行，使用者無法做別的事情，通常後臺操作無效時才會使用此方法）
 
 >       from auto import Fd   # 引入類別
 
 >       Fd.img_click('1.png')   # 點擊圖片  
@@ -52,20 +52,20 @@
 
 * 如果使用前臺操作，無法自動操作滑鼠鍵盤，請用系統管理員身份啓動腳本
 
 ## 依序執行任務的方法
 
 >       # 要執行的任務列表
 >       tasks = [
->           (img_click, "81.png"),
->           (img_click, "82.png"),
->           (img_click, "83.png"),
->           (img_click, "84.png")
+>           (bd.img_click, bd,"81.png"),
+>           (bd.img_click, bd,"82.png"),
+>           (bd.img_click, bd,"83.png"),
+>           (bd.img_click, bd,"84.png")
 >       ]
->       # 按照順序執行任務
+>       # 按照順序執行任務，完成全部任務跳出迴圈
 >       execute_tasks_in_sequence(tasks)
```

### Comparing `happylife-1.1.1/auto/__init__.py` & `happylife-1.1.2/auto/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 from PIL import ImageGrab
 from PIL import Image
 from contextlib import contextmanager
 from ctypes import windll
 import collections, ctypes, sys, cv2, numpy, time, win32gui, win32ui, win32con, win32api, win32print
 
 def get_scaling():
     '''獲取螢幕縮放比例'''
     hDC = win32gui.GetDC(0)
     proportion = round(win32print.GetDeviceCaps(hDC, win32con.DESKTOPHORZRES) / win32api.GetSystemMetrics(0), 2)
     return proportion
 
 # 後臺操作
-class Bw:
+class Bd:
  
     # 定義構造方法
     def __init__(self, title = '%', class_name = None, display_zoom = get_scaling()):
         '''
         後臺綁定(窗口名稱,類別名稱,顯示器縮放比例)
-        bw = Bw('夜神模擬器')
+        bw = Bd('夜神模擬器')
         '''
         self.hwnd = win32gui.FindWindow(class_name, title)
         self.display_zoom = display_zoom #display_zoom =>依據顯示器的縮放比調整數值,如縮放與版面配置設定為125%,display_zoom的值則設定為1.25
 
     # 綁定窗口
     def bind_window(self):
         self.hwnd = input('輸入要綁定的窗口句柄\n')
 
     # 綁定子窗口
     def bind_child_window(self, child_list_number):
         '''
         先綁定父窗口,再綁定子窗口,例如:
-        bw = Bw('雷電模擬器');
+        bw = Bd('雷電模擬器');
         bw.bind_child_window(0)
         child_list_number:數字代表選擇的順序,輸入0選擇第一個,輸入1選擇第二個
         '''
         parent_hwnd = self.hwnd
         hwnd_child_list = []
         win32gui.EnumChildWindows(parent_hwnd, lambda hwnd, param: param.append(hwnd), hwnd_child_list)
         self.hwnd = hwnd_child_list[child_list_number]
@@ -253,17 +253,17 @@
         #cv2.imshow('test',target)
         #cv2.waitKey()
         #cv2.destroyAllWindows()
 
     def img_click(self,bind,img,wait=0.3,grayscale=True,confidence=0.9):
         '''
         後臺點擊匹配到的圖片,
-        img_click(圖片,點擊後等待X秒,是否使用灰階,相似度)
-        bw = Bw('夜神模擬器')
-        img_click(bw,'1.png')
+        img_click(圖片,點擊後等待X秒,是否使用灰階,相似度)  
+        bw = Bd('夜神模擬器')  
+        img_click(bw,'1.png')  
         '''
         try:
             print(f"嘗試點擊圖像: {img}")
             search_img = img_center_point2(img, bind, confidence=confidence, grayscale=grayscale)
             if search_img:
                 x,y = search_img
                 self.x = x; self.y = y
@@ -275,15 +275,15 @@
         except ImageNotFoundException as e:
             print(f"未找到圖像: {img}. 錯誤: {e}")
         return False
     
     def img_drag(self, bind, img, img2, delay=0.3, grayscale=True):
         '''
         拖拽圖片,滑鼠從圖片1座標拖拽到圖片2座標
-        bw = Bw('夜神模擬器')
+        bw = Bd('夜神模擬器')
         img_drag(bw,'1.png','2.png')
         '''
         search_img = img_center_point2(img, bind, confidence=0.9, grayscale=grayscale)
         if search_img:
             x,y = img_center_point2(img, bind, confidence=0.9, grayscale=grayscale)
             x2,y2 = img_center_point2(img2, bind, confidence=0.9, grayscale=grayscale)
             self.x = x; self.y = y
@@ -291,15 +291,17 @@
             time.sleep(0.3)
             win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONDOWN, 1, ((int(self.y/self.display_zoom)) << 16 | (int(self.x//self.display_zoom))))
             time.sleep(delay)
             win32api.SendMessage(self.hwnd, win32con.WM_LBUTTONUP, 0, ((int(self.y2/self.display_zoom)) << 16 | (int(self.x2//self.display_zoom))))
 
 
 # 前臺操作        
-class Fd:
+class Fw:
+    hDC = win32gui.GetDC(0)
+    monitor_scaling = round(win32print.GetDeviceCaps(hDC, win32con.DESKTOPHORZRES) / win32api.GetSystemMetrics(0), 2)
 
     def keypress(vk_code,second):
         '''
         keypress(按鍵代碼,按下X秒後鬆開),keypress(68, 1)
         '''
         win32api.keybd_event(vk_code,0,0,0)
         time.sleep(second)
@@ -317,59 +319,59 @@
         '''
         win32api.keybd_event(vk_code,0, win32con.KEYEVENTF_KEYUP,0)
  
     def lclick(x,y):
         '''
         前臺滑鼠左鍵單擊指定座標,lclick(55,110)
         '''
-        win32api.SetCursorPos([x,y])
+        win32api.SetCursorPos([int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling)])
         win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP | win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0) 
         
     def lclick2(x,y):
         '''
         前臺滑鼠左鍵雙擊指定座標,lclick2(55,110)
         '''
-        win32api.SetCursorPos([x,y])
+        win32api.SetCursorPos([int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling)])
         win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP | win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
         win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP | win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
 
     def rclick(x,y):
         '''
         前臺滑鼠右鍵單擊指定座標,rclick(55,110)
         '''
-        win32api.SetCursorPos([x,y])
+        win32api.SetCursorPos([int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling)])
         win32api.mouse_event(win32con.MOUSEEVENTF_RIGHTUP | win32con.MOUSEEVENTF_RIGHTDOWN, 0, 0, 0, 0)
 
     def mouse_down(x,y):
         '''
         前臺滑鼠左鍵按下,mouse_down(55,110)
         '''
-        win32api.SetCursorPos([x,y])
+        win32api.SetCursorPos([int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling)])
         win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
 
     def mouse_up():
         '''
         前臺滑鼠左鍵釋放
         '''
         win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP, 0, 0, 0, 0)
 
     def moveto(x,y):
         '''
         前臺滑鼠移動,moveto(33,56)
         '''
-        win32api.SetCursorPos((x, y))
+        win32api.SetCursorPos(int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling))
 
     def mouse_drag(x,y,x2,y2,delay=0.1):
         '''
         從(x,y) 拖拽到(x2,y2),mouse_drag(132, 556, 0, 0)
         '''
-        win32api.SetCursorPos([x,y])
+        win32api.SetCursorPos([int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling)])
         win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
         time.sleep(delay)
-        win32api.SetCursorPos([x2,y2])
+        win32api.SetCursorPos([int(x2/Fw.monitor_scaling),int(y2/Fw.monitor_scaling)])
         time.sleep(delay)
         win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP, 0, 0, 0, 0)
 
     def scroll_up(WHEEL_DELTA = 120):
         '''
         前臺滑鼠向上滾動(WHEEL_DELTA:滾動幅度),scroll_up(120)
         '''
@@ -435,17 +437,17 @@
         '''
         try:
             print(f"嘗試點擊圖像: {img}")
             search_img = img_center_point(img, confidence=0.9, grayscale=grayscale)
             if search_img:
                 x,y = search_img
                 time.sleep(wait)
-                win32api.SetCursorPos([x,y])
+                win32api.SetCursorPos([int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling)])
                 win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP | win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
-                print(f"點擊位置: ({x}, {y})")
+                print(f"點擊位置: ({int(x/Fw.monitor_scaling)}, {int(y/Fw.monitor_scaling)})")
                 return True
         except ImageNotFoundException as e:
             print(f"未找到圖像: {img}. 錯誤: {e}")
         return False
     
     def img_drag(img, img2, delay=0.3, grayscale=True):
         '''
@@ -453,18 +455,18 @@
         img_drag('1.png','2.png')
         '''
         search_img = img_center_point(img, confidence=0.9, grayscale=grayscale)
         if search_img:
             x,y = img_center_point(img, confidence=0.9, grayscale=grayscale)
             x2,y2 = img_center_point(img2, confidence=0.9, grayscale=grayscale)
             time.sleep(0.3)
-            win32api.SetCursorPos([x,y])
+            win32api.SetCursorPos([int(x/Fw.monitor_scaling),int(y/Fw.monitor_scaling)])
             win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN, 0, 0, 0, 0)
             time.sleep(delay)
-            win32api.SetCursorPos([x2,y2])
+            win32api.SetCursorPos([int(x2/Fw.monitor_scaling),int(y2/Fw.monitor_scaling)])
             time.sleep(delay)
             win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP, 0, 0, 0, 0)
         
 # 圖色識別
 # 函式來自 pyscreeze , https://github.com/asweigart/pyscreeze
 
 unicode = str # 在 Python 3 上,所有 isinstance(spam, (str, unicode)) 調用都將與 Python 2 一樣工作
@@ -689,15 +691,15 @@
         return center(coords)
 
 
 def img_center_point2(image, bind, **kwargs):
     '''
     後臺獲取圖片中心點坐標,
     範例如下:
-    bw = Bw('夜神模擬器')
+    bw = Bd('夜神模擬器')
     auto.img_center_point2('2.png', bw, confidence=0.9, grayscale=True)
     '''
     coords = locateOnScreen2(image, bind, **kwargs)
     if coords is None:
         return None
     else:
         return center(coords)
```

### Comparing `happylife-1.1.1/setup.py` & `happylife-1.1.2/setup.py`

 * *Files identical despite different names*

