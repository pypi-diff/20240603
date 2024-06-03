# Comparing `tmp/package-tea-three-1.0.0.tar.gz` & `tmp/package-tea-three-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/package-tea-three-1.0.0.tar", last modified: Mon Mar  4 03:22:22 2024, max compression
+gzip compressed data, was "dist/package-tea-three-1.0.1.tar", last modified: Mon Jun  3 02:26:30 2024, max compression
```

## Comparing `package-tea-three-1.0.0.tar` & `package-tea-three-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:22:22.769399 package-tea-three-1.0.0/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1141 2024-03-04 03:22:22.768911 package-tea-three-1.0.0/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      155 2024-03-04 03:18:39.000000 package-tea-three-1.0.0/README.rst
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:22:22.766133 package-tea-three-1.0.0/package-tea-three/
--rw-r--r--   0 xiaofeng   (502) staff       (20)      126 2024-03-04 03:18:39.000000 package-tea-three-1.0.0/package-tea-three/__init__.py
--rw-r--r--   0 xiaofeng   (502) staff       (20)      505 2024-03-04 03:18:39.000000 package-tea-three-1.0.0/package-tea-three/main.py
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 03:22:22.768350 package-tea-three-1.0.0/package_tea_three.egg-info/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1141 2024-03-04 03:22:22.000000 package-tea-three-1.0.0/package_tea_three.egg-info/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      279 2024-03-04 03:22:22.000000 package-tea-three-1.0.0/package_tea_three.egg-info/SOURCES.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)        1 2024-03-04 03:22:22.000000 package-tea-three-1.0.0/package_tea_three.egg-info/dependency_links.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       46 2024-03-04 03:22:22.000000 package-tea-three-1.0.0/package_tea_three.egg-info/requires.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       18 2024-03-04 03:22:22.000000 package-tea-three-1.0.0/package_tea_three.egg-info/top_level.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       38 2024-03-04 03:22:22.769486 package-tea-three-1.0.0/setup.cfg
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1458 2024-03-04 03:21:57.000000 package-tea-three-1.0.0/setup.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1176 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      155 2024-06-03 02:22:53.000000 package-tea-three-1.0.1/README.rst
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/package-tea-three/
+-rw-r--r--   0 xf.shen    (502) staff       (20)      126 2024-06-03 02:22:53.000000 package-tea-three-1.0.1/package-tea-three/__init__.py
+-rw-r--r--   0 xf.shen    (502) staff       (20)      498 2024-06-03 02:24:48.000000 package-tea-three-1.0.1/package-tea-three/main.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/package_tea_three.egg-info/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1176 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/package_tea_three.egg-info/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      279 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/package_tea_three.egg-info/SOURCES.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)        1 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/package_tea_three.egg-info/dependency_links.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       97 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/package_tea_three.egg-info/requires.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       18 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/package_tea_three.egg-info/top_level.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       38 2024-06-03 02:26:30.000000 package-tea-three-1.0.1/setup.cfg
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1500 2024-06-03 02:25:48.000000 package-tea-three-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `package-tea-three-1.0.0/PKG-INFO` & `package-tea-three-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: package-tea-three
-Version: 1.0.0
-Summary: small package just example
+Version: 1.0.1
+Summary: test package
 Home-page: https://github.com/hanyan007/package-tea-three.git
 Author: hanyan_news
 Author-email: hanyan0572@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/hanyan007/package-tea-three.git
+Description: ========
+        发布示例
+        ========
+        - test
+        - 主流的开源技术
+        - 自动化测试
+        - 性能测试
+        - 安全测试
+        - go开发实战
+        - CI/CD
+        - Docker
+        - DevOps
+        
+        
+        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: package-tea-one==1.0.0
-Requires-Dist: package-tea-two==1.0.0
-
-========
-发布示例
-========
-- test
-- 主流的开源技术
-- 自动化测试
-- 性能测试
-- 安全测试
-- go开发实战
-- CI/CD
-- Docker
-- DevOps
-
-
```

### Comparing `package-tea-three-1.0.0/package_tea_three.egg-info/PKG-INFO` & `package-tea-three-1.0.1/package_tea_three.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: package-tea-three
-Version: 1.0.0
-Summary: small package just example
+Version: 1.0.1
+Summary: test package
 Home-page: https://github.com/hanyan007/package-tea-three.git
 Author: hanyan_news
 Author-email: hanyan0572@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/hanyan007/package-tea-three.git
+Description: ========
+        发布示例
+        ========
+        - test
+        - 主流的开源技术
+        - 自动化测试
+        - 性能测试
+        - 安全测试
+        - go开发实战
+        - CI/CD
+        - Docker
+        - DevOps
+        
+        
+        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: package-tea-one==1.0.0
-Requires-Dist: package-tea-two==1.0.0
-
-========
-发布示例
-========
-- test
-- 主流的开源技术
-- 自动化测试
-- 性能测试
-- 安全测试
-- go开发实战
-- CI/CD
-- Docker
-- DevOps
-
-
```

### Comparing `package-tea-three-1.0.0/setup.py` & `package-tea-three-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from setuptools import find_packages
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 
 setup(name='package-tea-three',  # 包名
-      version='1.0.0',  # 版本号
-      description='small package just example',
+      version='1.0.1',  # 版本号
+      description='test package',
       long_description=long_description,
       author='hanyan_news',
       author_email='hanyan0572@gmail.com',
       url='https://github.com/hanyan007/package-tea-three.git',
-      install_requires=["package-tea-one==1.0.0", "package-tea-two==1.0.0"],
+      install_requires=["package-tea-one==1.0.1", "package-tea-two==1.0.0","package-tea-hanyan==1.0.4", "dnspod-domain-log==1.0.2"],
       project_urls={  # Optional
         "Source": 'https://github.com/hanyan007/package-tea-three.git',
       },
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
```

