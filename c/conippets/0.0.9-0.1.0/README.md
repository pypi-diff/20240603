# Comparing `tmp/conippets-0.0.9.tar.gz` & `tmp/conippets-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conippets-0.0.9.tar", last modified: Sun Jan 14 14:46:17 2024, max compression
+gzip compressed data, was "conippets-0.1.0.tar", last modified: Mon Jun  3 11:35:30 2024, max compression
```

## Comparing `conippets-0.0.9.tar` & `conippets-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:46:17.343786 conippets-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-14 14:46:10.000000 conippets-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-14 14:46:17.343786 conippets-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-14 14:46:10.000000 conippets-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:46:17.343786 conippets-0.0.9/conippets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 14:46:10.000000 conippets-0.0.9/conippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-14 14:46:10.000000 conippets-0.0.9/conippets/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-14 14:46:10.000000 conippets-0.0.9/conippets/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-14 14:46:10.000000 conippets-0.0.9/conippets/json.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-14 14:46:10.000000 conippets-0.0.9/conippets/lxml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 14:46:17.343786 conippets-0.0.9/conippets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-14 14:46:17.000000 conippets-0.0.9/conippets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-14 14:46:17.000000 conippets-0.0.9/conippets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 14:46:17.000000 conippets-0.0.9/conippets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-14 14:46:17.000000 conippets-0.0.9/conippets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-14 14:46:17.000000 conippets-0.0.9/conippets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 14:46:17.343786 conippets-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-14 14:46:10.000000 conippets-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:35:30.412474 conippets-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 11:35:26.000000 conippets-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-03 11:35:30.412474 conippets-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-06-03 11:35:26.000000 conippets-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:35:30.412474 conippets-0.1.0/conippets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 11:35:26.000000 conippets-0.1.0/conippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-06-03 11:35:26.000000 conippets-0.1.0/conippets/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-03 11:35:26.000000 conippets-0.1.0/conippets/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-03 11:35:26.000000 conippets-0.1.0/conippets/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:35:30.412474 conippets-0.1.0/conippets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-03 11:35:30.000000 conippets-0.1.0/conippets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-03 11:35:30.000000 conippets-0.1.0/conippets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:35:30.000000 conippets-0.1.0/conippets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-03 11:35:30.000000 conippets-0.1.0/conippets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 11:35:30.000000 conippets-0.1.0/conippets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:35:30.412474 conippets-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-03 11:35:26.000000 conippets-0.1.0/setup.py
```

### Comparing `conippets-0.0.9/LICENSE` & `conippets-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conippets-0.0.9/conippets/git.py` & `conippets-0.1.0/conippets/git.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 import httpx
+from lxml.etree import HTML as parse_html
 import conippets.json as json
-import conippets.lxml as lxml
 
 _repo_data_xpath_ = '//react-partial[@partial-name="repos-overview"]/script[@data-target="react-partial.embeddedData"]'
+_code_data_xpath_ = '//react-app[@app-name="react-code-view"]/script[@data-target="react-app.embeddedData"]'
 
 def get_repo_data(user, repo):
     url = f'https://github.com/{user}/{repo}'
-    r = httpx.get(url)
-    html = lxml.parse_html(r.text)
+    r = httpx.get(url, follow_redirects=True)
+    html = parse_html(r.text)
     repo_data = html.xpath(_repo_data_xpath_)[0]
     repo_data = json.loads(repo_data.text)
     return repo_data
 
 def createAt(user, repo):
     repo_data = get_repo_data(user, repo)
     create_time = repo_data['props']['initialPayload']['repo']['createdAt']
     return create_time
 
 def currentOid(user, repo):
     repo_data = get_repo_data(user, repo)
     commit_id = repo_data['props']['initialPayload']['refInfo']['currentOid']
     return commit_id
+
+def get_code_data(url):
+    r = httpx.get(url, follow_redirects=True)
+    html = parse_html(r.text)
+    code_data = html.xpath(_code_data_xpath_)[0]
+    code_data = json.loads(code_data.text)
+    return code_data
+
+def rawLines(url):
+    code_data = get_code_data(url)
+    code = code_data['payload']['blob']['rawLines']
+    return code
+
+def list_dir(url):
+    dir_data = get_code_data(url)
+    items = dir_data['payload']['tree']['items']
+    return items
```

### Comparing `conippets-0.0.9/setup.py` & `conippets-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'conippets',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.9',
+    version = '0.1.0',
     license='MIT',
     description = 'conippets',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/conippets',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
     keywords = [
     ],
-    install_requires=[
-        'lxml', 'httpx',
-    ],
+    extras_require={
+        'git': ['lxml', 'httpx'],
+    },
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
     ],
     python_requires=">=3.8",
 )
```

