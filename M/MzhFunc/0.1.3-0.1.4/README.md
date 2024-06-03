# Comparing `tmp/MzhFunc-0.1.3-py3-none-any.whl.zip` & `tmp/MzhFunc-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 5405 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    12418 b- defN 24-Jun-02 15:37 db/MzhFunc.py
+Zip file size: 5697 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       74 b- defN 24-Jun-02 16:21 MzhFunc-0.1.4.data/data/requirements.txt
+-rw-rw-rw-  2.0 fat    12424 b- defN 24-Jun-03 02:01 db/MzhFunc.py
 -rw-rw-rw-  2.0 fat      211 b- defN 24-Jun-02 15:37 db/__init__.py
--rw-rw-rw-  2.0 fat      397 b- defN 24-Jun-03 01:52 MzhFunc-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-03 01:52 MzhFunc-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        3 b- defN 24-Jun-03 01:52 MzhFunc-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      437 b- defN 24-Jun-03 01:52 MzhFunc-0.1.3.dist-info/RECORD
-6 files, 13558 bytes uncompressed, 4617 bytes compressed:  65.9%
+-rw-rw-rw-  2.0 fat      397 b- defN 24-Jun-03 02:01 MzhFunc-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-03 02:01 MzhFunc-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        3 b- defN 24-Jun-03 02:01 MzhFunc-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      532 b- defN 24-Jun-03 02:01 MzhFunc-0.1.4.dist-info/RECORD
+7 files, 13733 bytes uncompressed, 4753 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
+Filename: MzhFunc-0.1.4.data/data/requirements.txt
+Comment: 
+
 Filename: db/MzhFunc.py
 Comment: 
 
 Filename: db/__init__.py
 Comment: 
 
-Filename: MzhFunc-0.1.3.dist-info/METADATA
+Filename: MzhFunc-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: MzhFunc-0.1.3.dist-info/WHEEL
+Filename: MzhFunc-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: MzhFunc-0.1.3.dist-info/top_level.txt
+Filename: MzhFunc-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: MzhFunc-0.1.3.dist-info/RECORD
+Filename: MzhFunc-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## db/MzhFunc.py

```diff
@@ -12,15 +12,15 @@
 import requests
 import pandas as pd
 import xlrd
 import openpyxl
 import os
 
 """
-cd MzhFunc & del /q dist && del /q MzhFunc.egg-info && python setup.py sdist && twine upload dist/*
+cd MzhFunc & del /q dist && del /q MzhFunc.egg-info && python setup.py bdist_wheel && twine upload dist/*
 """
 
 
 def qywx_sendtxt(text, key, all=None):
     """
     向指定企业微信群发送文本信息
     :param text: 发送的文本内容
```

