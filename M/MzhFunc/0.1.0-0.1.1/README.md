# Comparing `tmp/mzhfunc-0.1.0.tar.gz` & `tmp/mzhfunc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzhfunc-0.1.0.tar", last modified: Sun Jun  2 17:08:22 2024, max compression
+gzip compressed data, was "mzhfunc-0.1.1.tar", last modified: Mon Jun  3 00:55:20 2024, max compression
```

## Comparing `mzhfunc-0.1.0.tar` & `mzhfunc-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 17:08:22.026915 mzhfunc-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-06-02 17:08:22.025942 mzhfunc-0.1.0/MzhFunc.egg-info/
--rw-rw-rw-   0        0        0      383 2024-06-02 17:08:21.000000 mzhfunc-0.1.0/MzhFunc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-06-02 17:08:21.000000 mzhfunc-0.1.0/MzhFunc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 17:08:21.000000 mzhfunc-0.1.0/MzhFunc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-06-02 17:08:21.000000 mzhfunc-0.1.0/MzhFunc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      383 2024-06-02 17:08:22.025942 mzhfunc-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 mzhfunc-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 17:08:22.023995 mzhfunc-0.1.0/db/
--rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 mzhfunc-0.1.0/db/MzhFunc.py
--rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 mzhfunc-0.1.0/db/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-02 17:08:22.026915 mzhfunc-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2085 2024-06-02 17:08:17.000000 mzhfunc-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:55:20.639139 mzhfunc-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-06-03 00:55:20.638166 mzhfunc-0.1.1/MzhFunc.egg-info/
+-rw-rw-rw-   0        0        0      397 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-06-03 00:55:20.000000 mzhfunc-0.1.1/MzhFunc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      397 2024-06-03 00:55:20.639139 mzhfunc-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-06-01 16:57:53.000000 mzhfunc-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 00:55:20.637193 mzhfunc-0.1.1/db/
+-rw-rw-rw-   0        0        0    12418 2024-06-02 15:37:07.000000 mzhfunc-0.1.1/db/MzhFunc.py
+-rw-rw-rw-   0        0        0      211 2024-06-02 15:37:07.000000 mzhfunc-0.1.1/db/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 00:55:20.639139 mzhfunc-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2028 2024-06-03 00:50:55.000000 mzhfunc-0.1.1/setup.py
```

### Comparing `mzhfunc-0.1.0/db/MzhFunc.py` & `mzhfunc-0.1.1/db/MzhFunc.py`

 * *Files identical despite different names*

### Comparing `mzhfunc-0.1.0/setup.py` & `mzhfunc-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,15 @@
     name=package_name,
     version=get_version(),
     author="Author's name",  # 作者名称
     author_email="191891173@qq.com",  # 作者邮箱
     description="Python helper tools",  # 库描述
     long_description='python for mytools',
     long_description_content_type="text/markdown",
-    url=f"https://github.com/",  # 库的官方地址
-    # url=f"https://pypi.org/project/{package_name}/",  # 库的官方地址
+    url=f"https://pypi.org/project/{package_name}/",  # 库的官方地址
     packages=setuptools.find_packages(),
     # data_files=["requirements.txt"],  # yourtools库依赖的其他库
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

