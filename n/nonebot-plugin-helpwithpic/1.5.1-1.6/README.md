# Comparing `tmp/nonebot_plugin_helpwithpic-1.5.1.tar.gz` & `tmp/nonebot_plugin_helpwithpic-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_helpwithpic-1.5.1.tar", last modified: Wed Apr 24 09:46:24 2024, max compression
+gzip compressed data, was "nonebot_plugin_helpwithpic-1.6.tar", last modified: Mon Jun  3 09:00:27 2024, max compression
```

## Comparing `nonebot_plugin_helpwithpic-1.5.1.tar` & `nonebot_plugin_helpwithpic-1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:46:24.367210 nonebot_plugin_helpwithpic-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44334 2024-04-24 09:46:24.363210 nonebot_plugin_helpwithpic-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:46:24.363210 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw_contect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/hwp_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:46:24.363210 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44334 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:46:24.367210 nonebot_plugin_helpwithpic-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:27.887140 nonebot_plugin_helpwithpic-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44412 2024-06-03 09:00:27.887140 nonebot_plugin_helpwithpic-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:27.883140 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/basedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/draw_contect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/hwp_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 09:00:27.887140 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44412 2024-06-03 09:00:27.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-06-03 09:00:27.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 09:00:27.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-03 09:00:27.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 09:00:27.000000 nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-06-03 09:00:24.000000 nonebot_plugin_helpwithpic-1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 09:00:27.887140 nonebot_plugin_helpwithpic-1.6/setup.cfg
```

### Comparing `nonebot_plugin_helpwithpic-1.5.1/LICENSE` & `nonebot_plugin_helpwithpic-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5.1/PKG-INFO` & `nonebot_plugin_helpwithpic-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helpwithpic
-Version: 1.5.1
+Version: 1.6
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -787,13 +787,15 @@
 | HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如["file:///./data/draw/default_bg1.png"]此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
 | HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 | cubplugin_datadir | 否 | ""  | 插件数据文件夹 |
+| hwp_addseparator | 否 | "\n"  | helpadd的命令分割符,默认为回车 |
+
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

### Comparing `nonebot_plugin_helpwithpic-1.5.1/README.md` & `nonebot_plugin_helpwithpic-1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,13 +91,15 @@
 | HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如["file:///./data/draw/default_bg1.png"]此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
 | HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 | cubplugin_datadir | 否 | ""  | 插件数据文件夹 |
+| hwp_addseparator | 否 | "\n"  | helpadd的命令分割符,默认为回车 |
+
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

#### html2text {}

```diff
@@ -22,11 +22,12 @@
 -:|:----:|:----:|:----:| | HWP_font | å¦ | None | ä½¿ç¨çå­ä½æä»¶ | |
 HWP_custom_bg | å¦ | [] | å¾çèæ¯,éè¦ä»¥file:///å¼å¤´,æ¯å¦["file://
 /./data/draw/default_bg1.png"]æ­¤å¤ä½¿ç¨ç¸å¯¹è·¯å¾,é»è®¤ä½¿ç¨bingå£çº¸ |
 | version | å¦ | "Unknow" | å¯ä»¥å¡«ä½ çbotçæ¬ | | HWP_commandstart |
 å¦ | "#" | èªå®ä¹å½ä»¤å¤´ | | HWP_nickname | å¦ | "æ¬botçå¸®å©ææ¡£"
 | æ é¢ | | HWP_text | å¦ | "ä½ æ³è¦ç,æä»¬é½æ²¡æ
 (ä¸æ¯\nè¿æ¯æè¿°" | æè¿° | | HWP_version | å¦ | "HelpWithPic-Betaxxx" |
-æä»¶çæ¬ | | cubplugin_datadir | å¦ | "" | æä»¶æ°æ®æä»¶å¤¹ | ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:
-----:|:----:|:----:|:----:| | #help | user | å¦ | ç¾¤è/ç§è |
+æä»¶çæ¬ | | cubplugin_datadir | å¦ | "" | æä»¶æ°æ®æä»¶å¤¹ | |
+hwp_addseparator | å¦ | "\n" | helpaddçå½ä»¤åå²ç¬¦,é»è®¤ä¸ºåè½¦ | ##
+ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:---
+--:|:----:|:----:|:----:|:----:| | #help | user | å¦ | ç¾¤è/ç§è |
 è¯·æ ¹æ®HWP_commandstartä½¿ç¨ |
```

### Comparing `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/__init__.py` & `nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw.py` & `nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/draw.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     bg_help = Image.new("RGBA", (865,260), WHITE_BG_COLOR)
     bg_draw = ImageDraw.Draw(bg_help)
     aaa = await make_command_card(
         f"{cs}help / {cs}帮助","获取本帮助页",300
         )
     bbb = await make_command_card(
-        f"{cs}helpadd \\n[命令]\\n[描述]\\n[触发权限]","为本帮助页添加一条命令",700,perm="admin"
+        f"{cs}helpadd [命令]</>[描述]</>[触发权限]","为本帮助页添加一条命令,</>默认为换行",750,perm="admin"
         )
     ccc = await make_command_card(
         f"{cs}helpdel [命令]","删除一条命令",400,perm="admin"
         )
     unkown = await make_command_card("unkown","",250 ,"unkown","center")
     user = await make_command_card("user","",250 ,"user","center")
     admin = await make_command_card("admin","",250 ,"admin","center")
@@ -124,19 +124,15 @@
         bg.paste(aaa , (sidel, sidew) , aaa)
         sidel +=600
         if sidel > 1800:
             sidel = 33
             sidew +=140
     return bg
 
-permcolor={
-    "user":["#48dbfbc0","#0abde3"],
-    "admin":["#ff9ff3c0","#f368e0"],
-    "root":["#ff6b6bc0","#ee5253"]
-}
+from .basedata import permcolor
 
 async def make_command_card(
     text:str , 
     text2:str="",
     long:int=600,
     perm:str="user",
     chalign:str = "center"
```

### Comparing `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw_contect.py` & `nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/draw_contect.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/jsondata.py` & `nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/jsondata.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,19 +25,22 @@
 def delHWP(
     command :str,
 ):
     temp = rdata(jsonname)
     a = temp["cmdlist"].pop(command,"NotFound")
     wdata(jsonname,temp)
     return a
-    
-def format_data():
+
+permlist = ['unkown','user','admin','root']
+def format_data(perm:str="user"):
     temp = rdata(jsonname)
+    p = permlist.index(perm)+1
     cmdlist = temp.get("cmdlist",{})
     data = []
     for key , values in cmdlist.items():
-        data.append(
+        if values["perm"] in permlist[:p]:
+            data.append(
             [ key , values["text"] , values["perm"] ]
         )
     return data
 
 #本插件由 cubstaryow 编写
```

### Comparing `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/plugins_data.py` & `nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO` & `nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helpwithpic
-Version: 1.5.1
+Version: 1.6
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -787,13 +787,15 @@
 | HWP_custom_bg | 否 | [] | 图片背景,需要以file:///开头,比如["file:///./data/draw/default_bg1.png"]此处使用相对路径,默认使用bing壁纸 |
 | version | 否 | "Unknow" | 可以填你的bot版本 |
 | HWP_commandstart | 否 | "#" | 自定义命令头 |
 | HWP_nickname | 否 | "本bot的帮助文档" | 标题 |
 | HWP_text | 否 | "你想要的,我们都没有(不是\n这是描述" | 描述 |
 | HWP_version | 否 | "HelpWithPic-Betaxxx"  | 插件版本 |
 | cubplugin_datadir | 否 | ""  | 插件数据文件夹 |
+| hwp_addseparator | 否 | "\n"  | helpadd的命令分割符,默认为回车 |
+
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | #help | user | 否 | 群聊/私聊 | 请根据HWP_commandstart使用 |
```

### Comparing `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt` & `nonebot_plugin_helpwithpic-1.6/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 nonebot_plugin_helpwithpic/__init__.py
+nonebot_plugin_helpwithpic/basedata.py
 nonebot_plugin_helpwithpic/config.py
 nonebot_plugin_helpwithpic/draw.py
 nonebot_plugin_helpwithpic/draw_contect.py
 nonebot_plugin_helpwithpic/hwp_main.py
 nonebot_plugin_helpwithpic/jsondata.py
 nonebot_plugin_helpwithpic/plugins_data.py
 nonebot_plugin_helpwithpic.egg-info/PKG-INFO
```

### Comparing `nonebot_plugin_helpwithpic-1.5.1/pyproject.toml` & `nonebot_plugin_helpwithpic-1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-helpwithpic"
-version = "1.5.1"
+version = "1.6"
 description = "nonebot插件-动态帮助图片制作"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

