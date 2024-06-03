# Comparing `tmp/scripy_utils-0.0.1.tar.gz` & `tmp/scripy_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scripy_utils-0.0.1.tar", last modified: Sun Aug 13 10:43:21 2023, max compression
+gzip compressed data, was "scripy_utils-0.0.2.tar", last modified: Mon Jun  3 10:13:53 2024, max compression
```

## Comparing `scripy_utils-0.0.1.tar` & `scripy_utils-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-13 10:43:21.503899 scripy_utils-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-08-09 03:49:22.000000 scripy_utils-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       62 2023-08-13 10:42:49.000000 scripy_utils-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2119 2023-08-13 10:43:21.503899 scripy_utils-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-08-11 01:47:08.000000 scripy_utils-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-13 10:43:21.498900 scripy_utils-0.0.1/scripy_utils/
--rw-rw-rw-   0        0        0      173 2023-08-13 10:39:48.000000 scripy_utils-0.0.1/scripy_utils/__init__.py
--rw-rw-rw-   0        0        0     2621 2023-08-11 05:17:04.000000 scripy_utils-0.0.1/scripy_utils/html_font_parse.py
-drwxrwxrwx   0        0        0        0 2023-08-13 10:43:21.502901 scripy_utils-0.0.1/scripy_utils/media/
--rw-rw-rw-   0        0        0    49516 2021-07-14 03:18:52.000000 scripy_utils-0.0.1/scripy_utils/media/fake_useragent.json
--rw-rw-rw-   0        0        0     1549 2021-06-26 06:27:46.000000 scripy_utils-0.0.1/scripy_utils/mylog.py
--rw-rw-rw-   0        0        0     6150 2023-08-11 05:17:03.000000 scripy_utils-0.0.1/scripy_utils/request_parse.py
--rw-rw-rw-   0        0        0     9800 2021-07-14 03:21:02.000000 scripy_utils-0.0.1/scripy_utils/select_headers.py
--rw-rw-rw-   0        0        0     3066 2023-08-11 05:17:04.000000 scripy_utils-0.0.1/scripy_utils/url_parse.py
-drwxrwxrwx   0        0        0        0 2023-08-13 10:43:21.502901 scripy_utils-0.0.1/scripy_utils.egg-info/
--rw-rw-rw-   0        0        0     2119 2023-08-13 10:43:21.000000 scripy_utils-0.0.1/scripy_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-08-13 10:43:21.000000 scripy_utils-0.0.1/scripy_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-13 10:43:21.000000 scripy_utils-0.0.1/scripy_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-08-13 10:43:21.000000 scripy_utils-0.0.1/scripy_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-13 10:43:21.000000 scripy_utils-0.0.1/scripy_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-13 10:43:21.504900 scripy_utils-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3082 2023-08-13 10:36:39.000000 scripy_utils-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:13:53.720162 scripy_utils-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-08-09 03:49:22.000000 scripy_utils-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       62 2023-08-13 10:42:49.000000 scripy_utils-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2119 2024-06-03 10:13:53.719164 scripy_utils-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2023-08-11 01:47:08.000000 scripy_utils-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:13:53.645249 scripy_utils-0.0.2/scripy_utils/
+-rw-rw-rw-   0        0        0      173 2023-08-13 10:39:48.000000 scripy_utils-0.0.2/scripy_utils/__init__.py
+-rw-rw-rw-   0        0        0     2621 2023-08-11 05:17:04.000000 scripy_utils-0.0.2/scripy_utils/html_font_parse.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:13:53.718164 scripy_utils-0.0.2/scripy_utils/media/
+-rwxrwxrwx   0        0        0  6405632 2018-04-20 09:01:38.000000 scripy_utils-0.0.2/scripy_utils/media/chromedriver.exe
+-rw-rw-rw-   0        0        0    49516 2021-07-14 03:18:52.000000 scripy_utils-0.0.2/scripy_utils/media/fake_useragent.json
+-rw-rw-rw-   0        0        0    22503 2024-06-03 10:12:07.000000 scripy_utils-0.0.2/scripy_utils/request_parse.py
+-rw-rw-rw-   0        0        0     1254 2024-05-23 14:17:54.000000 scripy_utils-0.0.2/scripy_utils/request_util.py
+-rw-rw-rw-   0        0        0    19033 2024-06-03 10:01:27.000000 scripy_utils-0.0.2/scripy_utils/selenium_util.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:13:53.647776 scripy_utils-0.0.2/scripy_utils.egg-info/
+-rw-rw-rw-   0        0        0     2119 2024-06-03 10:13:52.000000 scripy_utils-0.0.2/scripy_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-06-03 10:13:52.000000 scripy_utils-0.0.2/scripy_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:13:52.000000 scripy_utils-0.0.2/scripy_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-06-03 10:13:52.000000 scripy_utils-0.0.2/scripy_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 10:13:52.000000 scripy_utils-0.0.2/scripy_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:13:53.720162 scripy_utils-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2920 2023-12-12 02:17:20.000000 scripy_utils-0.0.2/setup.py
```

### Comparing `scripy_utils-0.0.1/LICENSE` & `scripy_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scripy_utils-0.0.1/PKG-INFO` & `scripy_utils-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scripy_utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Short description
 Home-page: https://gitee.com/SkyOceanchen/scripy_utils.git
 Author: SkyOceanChen
 Author-email: skyoceanchen@foxmail.com
 Maintainer: SkyOceanChen
 Maintainer-email: skyoceanchen@foxmail.com
 License: MIT
```

### Comparing `scripy_utils-0.0.1/README.md` & `scripy_utils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scripy_utils-0.0.1/scripy_utils/html_font_parse.py` & `scripy_utils-0.0.2/scripy_utils/html_font_parse.py`

 * *Files identical despite different names*

### Comparing `scripy_utils-0.0.1/scripy_utils/media/fake_useragent.json` & `scripy_utils-0.0.2/scripy_utils/media/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `scripy_utils-0.0.1/scripy_utils.egg-info/PKG-INFO` & `scripy_utils-0.0.2/scripy_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scripy-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Short description
 Home-page: https://gitee.com/SkyOceanchen/scripy_utils.git
 Author: SkyOceanChen
 Author-email: skyoceanchen@foxmail.com
 Maintainer: SkyOceanChen
 Maintainer-email: skyoceanchen@foxmail.com
 License: MIT
```

### Comparing `scripy_utils-0.0.1/setup.py` & `scripy_utils-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '0.0.1'  # Any format you want
+version = '0.0.2'  # Any format you want
 DESCRIPTION = 'Easily cut the basic type by scripy_utils'
 AUTHOR = "SkyOceanChen"  # 留下大名
 AUTHOR_EMAIL = "skyoceanchen@foxmail.com"  # 留下邮箱
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
@@ -26,23 +26,16 @@
     url='https://gitee.com/SkyOceanchen/scripy_utils.git',  # 项目开源地址
     keywords=['basic_type', 'python', ],
     # 许可协议
     license='MIT',
     # PLATFORMS=["all", ],  # 支的乎台，如所有乎台超支，可以葵 aLLall'
     # 要安装的依赖包 ['py-L>=0.12.0', 'ter==3.1.0'],  # 指定了当前软件包所依赖的其他python类库。这些指定的python类库将会在本package被安装的时候一并被安装
     install_requires=[
-        "pdfkit==1.0.0",
-        "pyyaml",
-        "basic_type_operations",
-        "pandas",
-        "openpyxl",
-        "patool",
-        "filetype",
-        "Pillow==9.5.0",
-        "qrcode",
+        "chardet",
+        "fontTools",
         # "django==4.2.3",
         # All external pip packages you are importing
     ],
     classifiers=[  # 关于包的其他元数据(metadata)
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',  # 与操作系统无关
```

