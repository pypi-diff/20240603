# Comparing `tmp/sysrev-1.3.7.tar.gz` & `tmp/sysrev-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.3.7.tar", last modified: Sun May  5 00:49:21 2024, max compression
+gzip compressed data, was "sysrev-1.3.9.tar", last modified: Mon Jun  3 12:54:53 2024, max compression
```

## Comparing `sysrev-1.3.7.tar` & `sysrev-1.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:49:21.389868 sysrev-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-05 00:49:21.389868 sysrev-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-05 00:49:13.000000 sysrev-1.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 00:49:21.389868 sysrev-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-05 00:49:13.000000 sysrev-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:49:21.389868 sysrev-1.3.7/sysrev/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 00:49:13.000000 sysrev-1.3.7/sysrev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-05-05 00:49:13.000000 sysrev-1.3.7/sysrev/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:49:21.389868 sysrev-1.3.7/sysrev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-05 00:49:21.000000 sysrev-1.3.7/sysrev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-05 00:49:21.000000 sysrev-1.3.7/sysrev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 00:49:21.000000 sysrev-1.3.7/sysrev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 00:49:21.000000 sysrev-1.3.7/sysrev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 00:49:21.000000 sysrev-1.3.7/sysrev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 00:49:21.000000 sysrev-1.3.7/sysrev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 00:49:21.389868 sysrev-1.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-05 00:49:13.000000 sysrev-1.3.7/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-05 00:49:13.000000 sysrev-1.3.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:54:53.115764 sysrev-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-06-03 12:54:53.115764 sysrev-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-06-03 12:54:44.000000 sysrev-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 12:54:53.115764 sysrev-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-06-03 12:54:44.000000 sysrev-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:54:53.115764 sysrev-1.3.9/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 12:54:44.000000 sysrev-1.3.9/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-06-03 12:54:44.000000 sysrev-1.3.9/sysrev/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:54:53.115764 sysrev-1.3.9/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-06-03 12:54:53.000000 sysrev-1.3.9/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-03 12:54:53.000000 sysrev-1.3.9/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:54:53.000000 sysrev-1.3.9/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 12:54:52.000000 sysrev-1.3.9/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-03 12:54:53.000000 sysrev-1.3.9/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 12:54:53.000000 sysrev-1.3.9/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 12:54:53.115764 sysrev-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-06-03 12:54:44.000000 sysrev-1.3.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-06-03 12:54:44.000000 sysrev-1.3.9/tests/test_utils.py
```

### Comparing `sysrev-1.3.7/PKG-INFO` & `sysrev-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.7
+Version: 1.3.9
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.7/setup.py` & `sysrev-1.3.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Assuming your README file is in Markdown
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sysrev',
-    version='1.3.7',
+    version='1.3.9',
     description='get sysrev project data and use the sysrev api',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type here
     url='https://github.com/sysrev/PySysrev',
     author='Thomas Luechtefeld',
     author_email='tom@insilica.co',
     packages=['sysrev'],
```

### Comparing `sysrev-1.3.7/sysrev/client.py` & `sysrev-1.3.9/sysrev/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,22 +28,23 @@
 
         
 class Client():
     
     def __init__(self, api_key, base_url="https://www.sysrev.com"):
         self.api_key = api_key
         self.base_url = base_url
+        self.synchronizer = Synchronizer()
         
     def sync(self, project_id):
-        Synchronizer().sync(self, project_id)
+        self.synchronizer.sync(self, project_id)
     
     def get_project_info(self, project_id):
         endpoint = f"{self.base_url}/api-json/project-info"
         headers = {"Authorization": f"Bearer {self.api_key}"}
-        response = requests.get(endpoint, headers=headers, params={"project-id": project_id})
+        response = self.get(endpoint, headers=headers, params={"project-id": project_id})
         return response.json()
     
     def get_labels(self, project_id):
         raw_labels = self.get_project_info(project_id)['result']['project']['labels']
         labels = [{"label_id": label_id} | raw_labels[label_id] for label_id in raw_labels.keys()]
         return labels
     
@@ -89,15 +90,15 @@
             offset += len(articles)
     
     def get_article_info(self, project_id, article_id):
         endpoint = f"{self.base_url}/api-json/article-info/{article_id}"
         headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
         body = {"project-id": project_id,}
         response = requests.get(endpoint, headers=headers, json=body)
-        return response.json()['result']
+        return response.json().get('result', None)
                    
     def upload_jsonlines(self, file_path, project_id):
         url = f"{self.base_url}/api-json/import-files/{project_id}"
         headers = {"Authorization": f"Bearer {self.api_key}"}
         
         # Prepare the file for upload
         with open(file_path, 'rb') as f:
@@ -195,15 +196,15 @@
             df = df.loc[:, ~df.columns.duplicated()]
             df.to_sql(name, conn, if_exists='replace', index=False) if not df.empty else None
         finally:
             conn.close()
     
     def sync_article_info(self, client:Client, project_id, article_ids):
         article_info = []
-        for article_id in tqdm.tqdm(article_ids, total=len(article_ids)):
+        for article_id in tqdm.tqdm(article_ids, total=len(article_ids), desc="Fetching article info"):
             article_info.append(client.get_article_info(project_id, article_id))
         
         full_texts = pd.DataFrame([{**ft} for a in article_info for ft in a['article'].get('full-texts', []) ])
         full_texts.columns = [col.split('/')[-1] for col in full_texts.columns]
         
         auto_labels = pd.DataFrame([
             {**{'article-id': a['article'].get('article-id'), 'label-id': label_id}, **details} for a in article_info
@@ -224,33 +225,34 @@
     def sync_labels(self, client, project_id):
         labels = client.get_labels(project_id)
         labels_df = pd.DataFrame(labels)
         labels_df['definition'] = labels_df['definition'].apply(json.dumps)
         self.write_df(labels_df,'labels')
         
     # TODO - this could be made more efficient by checking sqlite state and updating the sysrev api
-    def sync(self, client, project_id):
+    def sync(self, client : Client, project_id):
         
         if not pathlib.Path('.sr/sr.sqlite').exists():
             self.create_sqlite_db()
             
         project_info = client.get_project_info(project_id)
         
         n_articles = project_info['result']['project']['stats']['articles']
-        articles = [resp for resp in tqdm.tqdm(client.fetch_all_articles(project_id), total=n_articles)]
+        articles = [resp for resp in tqdm.tqdm(client.fetch_all_articles(project_id), total=n_articles, desc="Fetching articles")]
         
         article_labels = [a['labels'] for a in articles if a['labels'] is not None]
         article_labels = [lbl for lbls in article_labels for lbl in lbls]
         article_label_df = pd.DataFrame(article_labels)
         article_label_df['answer'] = article_label_df['answer'].apply(json.dumps)
+        self.write_df(article_label_df,'article_label')
         
         article_data = [{k: v for k, v in a.items() if k != 'labels'} for a in articles]
         article_data_df = pd.DataFrame(article_data)
         article_data_df['notes'] = article_data_df['notes'].apply(json.dumps)
         article_data_df['resolve'] = article_data_df['resolve'].apply(json.dumps)
+        self.write_df(article_data_df,'article_data')
         
         self.sync_article_info(client, project_id, article_data_df['article-id'])
         self.sync_labels(client, project_id)
 
-        # Writing data to tables
-        self.write_df(article_label_df,'article_label')
-        self.write_df(article_data_df,'article_data')
+        
+
```

### Comparing `sysrev-1.3.7/sysrev.egg-info/PKG-INFO` & `sysrev-1.3.9/sysrev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.7
+Version: 1.3.9
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.7/tests/test_client.py` & `sysrev-1.3.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sysrev-1.3.7/tests/test_utils.py` & `sysrev-1.3.9/tests/test_utils.py`

 * *Files identical despite different names*

