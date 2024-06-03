# Comparing `tmp/pyxo-0.4.tar.gz` & `tmp/pyxo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxo-0.4.tar", last modified: Sun Feb 19 20:35:05 2023, max compression
+gzip compressed data, was "pyxo-1.0.2.tar", max compression
```

## Comparing `pyxo-0.4.tar` & `pyxo-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 20:35:05.436138 pyxo-0.4/
--rw-rw-rw-   0        0        0     1093 2023-02-19 14:58:25.000000 pyxo-0.4/LICENSE
--rw-rw-rw-   0        0        0      386 2023-02-19 20:35:05.436138 pyxo-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-02-19 18:44:45.000000 pyxo-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 20:35:05.370602 pyxo-0.4/pyxo/
--rw-rw-rw-   0        0        0      109 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 20:35:05.411154 pyxo-0.4/pyxo/controler/
--rw-rw-rw-   0        0        0       38 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/controler/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/controler/engin.py
-drwxrwxrwx   0        0        0        0 2023-02-19 20:35:05.411154 pyxo-0.4/pyxo/models/
--rw-rw-rw-   0        0        0       69 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/models/__init__.py
--rw-rw-rw-   0        0        0     3088 2023-02-19 19:43:44.000000 pyxo-0.4/pyxo/models/board.py
--rw-rw-rw-   0        0        0     1066 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/models/player.py
-drwxrwxrwx   0        0        0        0 2023-02-19 20:35:05.423164 pyxo-0.4/pyxo/utils/
--rw-rw-rw-   0        0        0       38 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/utils/__init__.py
--rw-rw-rw-   0        0        0     1497 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/utils/functions.py
-drwxrwxrwx   0        0        0        0 2023-02-19 20:35:05.435184 pyxo-0.4/pyxo/views/
--rw-rw-rw-   0        0        0      306 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/views/__init__.py
--rw-rw-rw-   0        0        0      608 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/views/addplayer.py
--rw-rw-rw-   0        0        0      156 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/views/playagain.py
--rw-rw-rw-   0        0        0      705 2023-02-19 20:30:25.000000 pyxo-0.4/pyxo/views/playing.py
--rw-rw-rw-   0        0        0      402 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/views/showiner.py
--rw-rw-rw-   0        0        0     1550 2023-02-19 14:58:25.000000 pyxo-0.4/pyxo/views/start.py
-drwxrwxrwx   0        0        0        0 2023-02-19 20:35:05.411154 pyxo-0.4/pyxo.egg-info/
--rw-rw-rw-   0        0        0      386 2023-02-19 20:35:05.000000 pyxo-0.4/pyxo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-02-19 20:35:05.000000 pyxo-0.4/pyxo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 20:35:05.000000 pyxo-0.4/pyxo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-02-19 20:35:05.000000 pyxo-0.4/pyxo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 20:35:05.436138 pyxo-0.4/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-02-19 20:33:37.000000 pyxo-0.4/setup.py
+-rw-r--r--   0        0        0     1074 2024-06-03 11:59:01.709243 pyxo-1.0.2/LICENSE
+-rw-r--r--   0        0        0      361 2024-06-03 11:59:01.709243 pyxo-1.0.2/README.md
+-rw-r--r--   0        0        0      620 2024-06-03 11:59:32.521455 pyxo-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      127 2024-06-03 11:59:32.521455 pyxo-1.0.2/pyxo/__init__.py
+-rw-r--r--   0        0        0       36 2024-06-03 11:59:01.709243 pyxo-1.0.2/pyxo/controler/__init__.py
+-rw-r--r--   0        0        0     3163 2024-06-03 11:59:01.709243 pyxo-1.0.2/pyxo/controler/engin.py
+-rw-r--r--   0        0        0       66 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/models/__init__.py
+-rw-r--r--   0        0        0     2995 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/models/board.py
+-rw-r--r--   0        0        0     1024 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/models/player.py
+-rw-r--r--   0        0        0       36 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/utils/__init__.py
+-rw-r--r--   0        0        0     1448 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/utils/functions.py
+-rw-r--r--   0        0        0      291 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/views/__init__.py
+-rw-r--r--   0        0        0      588 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/views/addplayer.py
+-rw-r--r--   0        0        0      147 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/views/playagain.py
+-rw-r--r--   0        0        0      682 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/views/playing.py
+-rw-r--r--   0        0        0      387 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/views/showiner.py
+-rw-r--r--   0        0        0     1504 2024-06-03 11:59:01.713243 pyxo-1.0.2/pyxo/views/start.py
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 pyxo-1.0.2/PKG-INFO
```

### Comparing `pyxo-0.4/LICENSE` & `pyxo-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2022 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2022 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyxo-0.4/pyxo/models/board.py` & `pyxo-1.0.2/pyxo/models/board.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from pyxo.utils import  equals
-
-
-class Board:
-
-    """the Board is the model responseble of saving 
-    the information about the board of the X O game
-    and every player move.
-    Every board has three rows every row contain three
-    case with True for X and False for O.
-    """
-
-    def __init__(self) -> None:
-       
-        """to create an object Board use this following code:
-        ```python
-        >>> xo_board = Board()
-        >>> # to see the rows you need this code
-        >>> xo_board.row_1 # or xo_board.row_2
-        ```
-        """
-
-        self.row_1 :list[bool] = 3*[None]
-        self.row_2 :list[bool] = 3*[None]
-        self.row_3 :list[bool] = 3*[None]
-
-
-    def reset(self) -> None:
-        
-        """After the end of the game of XO
-        we need to reset the board to do that we use this
-        folowing code :
-        ```python
-        >>> xo_board = Board()
-        >>> xo_board.reset()
-        ```
-        """
-
-        self.row_1 :list[bool] = 3*[None]
-        self.row_2 :list[bool] = 3*[None]
-        self.row_3 :list[bool] = 3*[None]
-
-    
-    def check_move(self,move :int) -> bool:
-        new_move = move % 3
-        if move in [1,2,3]: return True if self.row_1[new_move-1] is None else False
-        if move in [4,5,6]: return True if self.row_2[new_move-1] is None else False
-        if move in [7,8,9]: return True if self.row_3[new_move-1] is None else False
-        return False
-
-    def make_move(self,move:int,choise:bool) -> None:
-        new_move = move % 3
-        if move in [1,2,3]: self.row_1[new_move-1] = choise
-        if move in [4,5,6]: self.row_2[new_move-1] = choise
-        if move in [7,8,9]:self.row_3[new_move-1] = choise
-
-    def game_ended(self) -> bool:
-        return self.count_full() == 8 or self.winer_exist()
-
-
-    def winer_exist(self) -> bool:
-        return self.check_row() or self.check_colum() or self.check_corner()
-
-    def check_row(self) -> bool:
-        if equals(self.row_1[0],self.row_1[1],self.row_1[2]) :return True
-        if equals(self.row_2[0],self.row_2[1],self.row_2[2]) :return True
-        if equals(self.row_3[0],self.row_3[1],self.row_3[2]) :return True
-        return False
-
-
-    def check_colum(self) -> bool:
-        
-        if equals(self.row_1[0],self.row_2[0],self.row_3[0]) :return True
-        if equals(self.row_1[1],self.row_2[1],self.row_3[1]) :return True
-        if equals(self.row_1[2],self.row_2[2],self.row_3[2]) :return True
-        return False
-
-    def check_corner(self) -> bool:
-        
-        if equals(self.row_1[0],self.row_2[1],self.row_3[2]) :return True
-        if equals(self.row_3[0],self.row_2[1],self.row_1[2]) :return True
-        return False
-
-    def count_full(self) -> int:
-        count :int = 0
-        for i in range(3):
-            if self.row_1[i] is not None:
-                count += 1
-            if self.row_2[i] is not None:
-                count += 1
-            if self.row_3[i] is not None:
-                count += 1
-        return count
+from pyxo.utils import  equals
+
+
+class Board:
+
+    """the Board is the model responseble of saving 
+    the information about the board of the X O game
+    and every player move.
+    Every board has three rows every row contain three
+    case with True for X and False for O.
+    """
+
+    def __init__(self) -> None:
+       
+        """to create an object Board use this following code:
+        ```python
+        >>> xo_board = Board()
+        >>> # to see the rows you need this code
+        >>> xo_board.row_1 # or xo_board.row_2
+        ```
+        """
+
+        self.row_1 :list[bool] = 3*[None]
+        self.row_2 :list[bool] = 3*[None]
+        self.row_3 :list[bool] = 3*[None]
+
+
+    def reset(self) -> None:
+        
+        """After the end of the game of XO
+        we need to reset the board to do that we use this
+        folowing code :
+        ```python
+        >>> xo_board = Board()
+        >>> xo_board.reset()
+        ```
+        """
+
+        self.row_1 :list[bool] = 3*[None]
+        self.row_2 :list[bool] = 3*[None]
+        self.row_3 :list[bool] = 3*[None]
+
+    
+    def check_move(self,move :int) -> bool:
+        new_move = move % 3
+        if move in [1,2,3]: return True if self.row_1[new_move-1] is None else False
+        if move in [4,5,6]: return True if self.row_2[new_move-1] is None else False
+        if move in [7,8,9]: return True if self.row_3[new_move-1] is None else False
+        return False
+
+    def make_move(self,move:int,choise:bool) -> None:
+        new_move = move % 3
+        if move in [1,2,3]: self.row_1[new_move-1] = choise
+        if move in [4,5,6]: self.row_2[new_move-1] = choise
+        if move in [7,8,9]:self.row_3[new_move-1] = choise
+
+    def game_ended(self) -> bool:
+        return self.count_full() == 8 or self.winer_exist()
+
+
+    def winer_exist(self) -> bool:
+        return self.check_row() or self.check_colum() or self.check_corner()
+
+    def check_row(self) -> bool:
+        if equals(self.row_1[0],self.row_1[1],self.row_1[2]) :return True
+        if equals(self.row_2[0],self.row_2[1],self.row_2[2]) :return True
+        if equals(self.row_3[0],self.row_3[1],self.row_3[2]) :return True
+        return False
+
+
+    def check_colum(self) -> bool:
+        
+        if equals(self.row_1[0],self.row_2[0],self.row_3[0]) :return True
+        if equals(self.row_1[1],self.row_2[1],self.row_3[1]) :return True
+        if equals(self.row_1[2],self.row_2[2],self.row_3[2]) :return True
+        return False
+
+    def check_corner(self) -> bool:
+        
+        if equals(self.row_1[0],self.row_2[1],self.row_3[2]) :return True
+        if equals(self.row_3[0],self.row_2[1],self.row_1[2]) :return True
+        return False
+
+    def count_full(self) -> int:
+        count :int = 0
+        for i in range(3):
+            if self.row_1[i] is not None:
+                count += 1
+            if self.row_2[i] is not None:
+                count += 1
+            if self.row_3[i] is not None:
+                count += 1
+        return count
```

### Comparing `pyxo-0.4/pyxo/utils/functions.py` & `pyxo-1.0.2/pyxo/utils/functions.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import os
-
-def clear() -> None:
-
-    """this function is respenseble of clearing 
-    the terminal on linux or the console on 
-    windows .
-    """
-
-    try:
-        os.system("clear")
-    except Exception as ex:
-        os.system("cls")
-
-
-def bool_str(boolean:bool) -> str:
-    if boolean is None: return " "
-    if boolean : return "X"
-    if not boolean : return "O"
-
-
-
-def show_board(board:"Board",players:list["Player"]) -> None:
-    
-    row_1 :list[str] = [ bool_str(cas) for cas in board.row_1] 
-    row_2 :list[str] = [ bool_str(cas) for cas in board.row_2] 
-    row_3 :list[str] = [ bool_str(cas) for cas in board.row_3] 
-    
-    print(f"""    
-
-
-            _|___|___|___|_       |       _|___|___|___|_         
-             | {row_1[0]} | {row_1[1]} | {row_1[2]} |        |       _| 1 | 2 | 3 |_  {players[0].name} :  {players[0].points}
-            _|___|___|___|_       |       _|___|___|___|_   
-             | {row_2[0]} | {row_2[1]} | {row_2[2]} |        |       _| 4 | 5 | 6 |_  {players[1].name} :  {players[1].points}
-            _|___|___|___|_       |       _|___|___|___|_         
-             | {row_3[0]} | {row_3[1]} | {row_3[2]} |        |       _| 7 | 8 | 9 |_
-            _|___|___|___|_       |       _|___|___|___|_         
-
-
-        ____________________________________________________________
-        
-        """)
-
-
-def equals(a:bool,b:bool,c:bool) -> bool:
-    return (a == b and b == c and a is not None)
-
-
+import os
+
+def clear() -> None:
+
+    """this function is respenseble of clearing 
+    the terminal on linux or the console on 
+    windows .
+    """
+
+    try:
+        os.system("clear")
+    except Exception as ex:
+        os.system("cls")
+
+
+def bool_str(boolean:bool) -> str:
+    if boolean is None: return " "
+    if boolean : return "X"
+    if not boolean : return "O"
+
+
+
+def show_board(board:"Board",players:list["Player"]) -> None:
+    
+    row_1 :list[str] = [ bool_str(cas) for cas in board.row_1] 
+    row_2 :list[str] = [ bool_str(cas) for cas in board.row_2] 
+    row_3 :list[str] = [ bool_str(cas) for cas in board.row_3] 
+    
+    print(f"""    
+
+
+            _|___|___|___|_       |       _|___|___|___|_         
+             | {row_1[0]} | {row_1[1]} | {row_1[2]} |        |       _| 1 | 2 | 3 |_  {players[0].name} :  {players[0].points}
+            _|___|___|___|_       |       _|___|___|___|_   
+             | {row_2[0]} | {row_2[1]} | {row_2[2]} |        |       _| 4 | 5 | 6 |_  {players[1].name} :  {players[1].points}
+            _|___|___|___|_       |       _|___|___|___|_         
+             | {row_3[0]} | {row_3[1]} | {row_3[2]} |        |       _| 7 | 8 | 9 |_
+            _|___|___|___|_       |       _|___|___|___|_         
+
+
+        ____________________________________________________________
+        
+        """)
+
+
+def equals(a:bool,b:bool,c:bool) -> bool:
+    return (a == b and b == c and a is not None)
+
+
```

### Comparing `pyxo-0.4/pyxo/views/addplayer.py` & `pyxo-1.0.2/pyxo/views/addplayer.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pyxo.views import View
-from pyxo.utils import clear
-
-class AddPlayer(View):
-    
-
-    def __init__(self,controler:"Engin") -> None:
-        
-        self.controler :"Engin" = controler
-
-    
-    def print(self) -> None:
-
-        clear()
-        name_first_player :str = str(input("     the name of the player - 1 - :\t"))
-        choise :str = input("      chose {X} or {O}  :\t ")
-        self.controler.add_player(name_first_player,choise)
-        name_second_player :str = str(input("     the name of the player - 2 - :\t"))
-        self.controler.add_player(name_second_player)
-
+from pyxo.views import View
+from pyxo.utils import clear
+
+class AddPlayer(View):
+    
+
+    def __init__(self,controler:"Engin") -> None:
+        
+        self.controler :"Engin" = controler
+
+    
+    def print(self) -> None:
+
+        clear()
+        name_first_player :str = str(input("     the name of the player - 1 - :\t"))
+        choise :str = input("      chose {X} or {O}  :\t ")
+        self.controler.add_player(name_first_player,choise)
+        name_second_player :str = str(input("     the name of the player - 2 - :\t"))
+        self.controler.add_player(name_second_player)
+
```

### Comparing `pyxo-0.4/pyxo/views/playing.py` & `pyxo-1.0.2/pyxo/views/playing.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from pyxo.views import View
-from pyxo.utils import clear,show_board
-
-
-class Playing(View):
-
-    def __init__(self,controler:"Engin") -> None:
-        self.controler :"Engin" = controler
-
-    def print(self,number:int) -> int:
-        clear()
-        show_board(self.controler.board,self.controler.players)
-
-        try:
-            return int(input(f"  what is your next move  {self.controler.players[number].name}  :(1...9) \t"))
-        except Exception as ex:
-            return 100
-
-    def print_error(self) -> int:
-        try :
-            return int(input(" this nomber is not vailable chose an ather one:(1...9) \t"))
-        except Exception as ex:
-            return 100
+from pyxo.views import View
+from pyxo.utils import clear,show_board
+
+
+class Playing(View):
+
+    def __init__(self,controler:"Engin") -> None:
+        self.controler :"Engin" = controler
+
+    def print(self,number:int) -> int:
+        clear()
+        show_board(self.controler.board,self.controler.players)
+
+        try:
+            return int(input(f"  what is your next move  {self.controler.players[number].name}  :(1...9) \t"))
+        except Exception as ex:
+            return 100
+
+    def print_error(self) -> int:
+        try :
+            return int(input(" this nomber is not vailable chose an ather one:(1...9) \t"))
+        except Exception as ex:
+            return 100
```

