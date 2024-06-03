# Comparing `tmp/git-picker-0.3.8.tar.gz` & `tmp/git-picker-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-picker-0.3.8.tar", last modified: Fri Feb 23 17:21:11 2024, max compression
+gzip compressed data, was "git-picker-0.3.9.tar", last modified: Sun Feb 25 09:35:48 2024, max compression
```

## Comparing `git-picker-0.3.8.tar` & `git-picker-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:21:11.307769 git-picker-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-23 17:21:04.000000 git-picker-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-23 17:21:11.307769 git-picker-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-23 17:21:04.000000 git-picker-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:21:11.307769 git-picker-0.3.8/git_picker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-23 17:21:11.000000 git-picker-0.3.8/git_picker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-23 17:21:11.000000 git-picker-0.3.8/git_picker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 17:21:11.000000 git-picker-0.3.8/git_picker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-23 17:21:11.000000 git-picker-0.3.8/git_picker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-23 17:21:11.000000 git-picker-0.3.8/git_picker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:21:11.307769 git-picker-0.3.8/gitpicker/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-23 17:21:04.000000 git-picker-0.3.8/gitpicker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-23 17:21:04.000000 git-picker-0.3.8/gitpicker/gitee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-23 17:21:04.000000 git-picker-0.3.8/gitpicker/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-02-23 17:21:04.000000 git-picker-0.3.8/gitpicker/picker.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 17:21:11.307769 git-picker-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-23 17:21:04.000000 git-picker-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:35:48.348164 git-picker-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-25 09:35:41.000000 git-picker-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-25 09:35:48.348164 git-picker-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-25 09:35:41.000000 git-picker-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:35:48.348164 git-picker-0.3.9/git_picker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-25 09:35:48.000000 git-picker-0.3.9/git_picker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-25 09:35:48.000000 git-picker-0.3.9/git_picker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 09:35:48.000000 git-picker-0.3.9/git_picker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-25 09:35:48.000000 git-picker-0.3.9/git_picker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-25 09:35:48.000000 git-picker-0.3.9/git_picker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 09:35:48.348164 git-picker-0.3.9/gitpicker/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 09:35:41.000000 git-picker-0.3.9/gitpicker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-25 09:35:41.000000 git-picker-0.3.9/gitpicker/gitee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-25 09:35:41.000000 git-picker-0.3.9/gitpicker/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-02-25 09:35:41.000000 git-picker-0.3.9/gitpicker/picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 09:35:48.348164 git-picker-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-25 09:35:41.000000 git-picker-0.3.9/setup.py
```

### Comparing `git-picker-0.3.8/LICENSE` & `git-picker-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `git-picker-0.3.8/PKG-INFO` & `git-picker-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-picker
-Version: 0.3.8
+Version: 0.3.9
 Summary: git picker
 Home-page: https://github.com/JiauZhang/git-picker
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: GitHub
 Classifier: Intended Audience :: Developers
```

### Comparing `git-picker-0.3.8/git_picker.egg-info/PKG-INFO` & `git-picker-0.3.9/git_picker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-picker
-Version: 0.3.8
+Version: 0.3.9
 Summary: git picker
 Home-page: https://github.com/JiauZhang/git-picker
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: GitHub
 Classifier: Intended Audience :: Developers
```

### Comparing `git-picker-0.3.8/gitpicker/gitee.py` & `git-picker-0.3.9/gitpicker/gitee.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,11 +21,7 @@
         _dirs = dir_tree.xpath('./div[@data-type="folder"]')
         for i in range(len(_dirs)):
             _dirs[i] = _dirs[i].xpath('./div[@data-type="folder"]')[0].attrib['data-path']
         _files = dir_tree.xpath('./div[@data-type="file"]')
         for i in range(len(_files)):
             _files[i] = _files[i].xpath('./div[@data-type="file"]')[0].attrib['data-path']
         return _dirs, _files
-
-    def parse_items(self, items):
-        _dirs, _files = items
-        return _dirs, _files
```

### Comparing `git-picker-0.3.8/gitpicker/github.py` & `git-picker-0.3.9/gitpicker/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return lines
 
     def get_dir_items(self, dir):
         url = f'{self.base_url}/{dir}'
         r = self.client.get(url, follow_redirects=True)
         js = r.json()
         items = js['payload']['tree']['items']
-        return items
+        return self.parse_items(items)
 
     def parse_items(self, items):
         _dirs, _files = [], []
         for item in items:
             ctype = item['contentType']
             path = item['path']
             if ctype == 'directory':
```

### Comparing `git-picker-0.3.8/gitpicker/picker.py` & `git-picker-0.3.9/gitpicker/picker.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,18 +116,14 @@
         if lines is None or retry == self.retry:
             self.failed = True
             raise RuntimeError(f'retry[{retry}/{self.retry}] downloading {self.repo}/{file} failed!')
 
         filename = f'{self.repo}/{file}'
         self.save_file(filename, lines)
 
-    @abstractmethod
-    def parse_items(self, items):
-        ...
-
     def download_dir(self, dir):
         print(f'downloading {self.repo}/{dir}')
         os.makedirs(f'{self.repo}/{dir}', exist_ok=True)
         retry, items = 0, None
         while not self.failed and retry < self.retry:
             try:
                 items = self.get_dir_items(dir)
@@ -138,15 +134,15 @@
                 traceback.print_exc()
                 time.sleep(1)
 
         if items is None or retry == self.retry:
             self.failed = True
             raise RuntimeError(f'retry[{retry}/{self.retry}] downloading {self.repo}/{dir} failed!')
 
-        _dirs, _files = self.parse_items(items)
+        _dirs, _files = items
 
         self.lock.acquire()
         for file in _files:
             self.tasks.put(file)
         self.lock.release()
         for dir in _dirs:
             self.download_dir(dir)
```

### Comparing `git-picker-0.3.8/setup.py` & `git-picker-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'git-picker',
     packages = find_packages(exclude=['examples']),
-    version = '0.3.8',
+    version = '0.3.9',
     license='MIT',
     description = 'git picker',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/git-picker',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

