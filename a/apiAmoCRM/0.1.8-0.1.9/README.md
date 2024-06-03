# Comparing `tmp/apiamocrm-0.1.8.tar.gz` & `tmp/apiamocrm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiamocrm-0.1.8.tar", last modified: Mon Jun  3 08:41:36 2024, max compression
+gzip compressed data, was "apiamocrm-0.1.9.tar", last modified: Mon Jun  3 09:28:05 2024, max compression
```

## Comparing `apiamocrm-0.1.8.tar` & `apiamocrm-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 08:41:36.288766 apiamocrm-0.1.8/
--rw-rw-rw-   0        0        0      438 2024-06-03 08:41:36.287765 apiamocrm-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 08:41:36.269612 apiamocrm-0.1.8/amoApi/
--rw-rw-rw-   0        0        0     6486 2024-06-03 04:08:24.000000 apiamocrm-0.1.8/amoApi/API.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.8/amoApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:41:36.272611 apiamocrm-0.1.8/amoApi/amoEntities/
--rw-rw-rw-   0        0        0     3427 2024-06-03 03:55:35.000000 apiamocrm-0.1.8/amoApi/amoEntities/Contact.py
--rw-rw-rw-   0        0        0     3318 2024-06-03 03:51:25.000000 apiamocrm-0.1.8/amoApi/amoEntities/Lead.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.8/amoApi/amoEntities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:41:36.280132 apiamocrm-0.1.8/amoChatApi/
--rw-rw-rw-   0        0        0     5118 2024-06-03 08:41:13.000000 apiamocrm-0.1.8/amoChatApi/API.py
--rw-rw-rw-   0        0        0      138 2024-06-03 04:11:23.000000 apiamocrm-0.1.8/amoChatApi/AbstractMessage.py
--rw-rw-rw-   0        0        0     2011 2024-06-03 08:29:32.000000 apiamocrm-0.1.8/amoChatApi/Payload.py
--rw-rw-rw-   0        0        0      994 2024-06-03 08:30:59.000000 apiamocrm-0.1.8/amoChatApi/PhotoMessage.py
--rw-rw-rw-   0        0        0      392 2024-06-03 04:11:18.000000 apiamocrm-0.1.8/amoChatApi/TextMessage.py
--rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.8/amoChatApi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-03 08:41:36.286765 apiamocrm-0.1.8/apiAmoCRM.egg-info/
--rw-rw-rw-   0        0        0      438 2024-06-03 08:41:36.000000 apiamocrm-0.1.8/apiAmoCRM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-06-03 08:41:36.000000 apiamocrm-0.1.8/apiAmoCRM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 08:41:36.000000 apiamocrm-0.1.8/apiAmoCRM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 08:41:36.000000 apiamocrm-0.1.8/apiAmoCRM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-03 08:41:36.000000 apiamocrm-0.1.8/apiAmoCRM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-03 08:41:36.288766 apiamocrm-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      633 2024-06-03 08:41:28.000000 apiamocrm-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:05.797722 apiamocrm-0.1.9/
+-rw-rw-rw-   0        0        0      438 2024-06-03 09:28:05.796713 apiamocrm-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-30 09:48:06.000000 apiamocrm-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:05.779684 apiamocrm-0.1.9/amoApi/
+-rw-rw-rw-   0        0        0     6486 2024-06-03 04:08:24.000000 apiamocrm-0.1.9/amoApi/API.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:29.000000 apiamocrm-0.1.9/amoApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:05.783684 apiamocrm-0.1.9/amoApi/amoEntities/
+-rw-rw-rw-   0        0        0     3427 2024-06-03 03:55:35.000000 apiamocrm-0.1.9/amoApi/amoEntities/Contact.py
+-rw-rw-rw-   0        0        0     3318 2024-06-03 03:51:25.000000 apiamocrm-0.1.9/amoApi/amoEntities/Lead.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:19:41.000000 apiamocrm-0.1.9/amoApi/amoEntities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:05.789199 apiamocrm-0.1.9/amoChatApi/
+-rw-rw-rw-   0        0        0     6208 2024-06-03 09:27:11.000000 apiamocrm-0.1.9/amoChatApi/API.py
+-rw-rw-rw-   0        0        0      138 2024-06-03 04:11:23.000000 apiamocrm-0.1.9/amoChatApi/AbstractMessage.py
+-rw-rw-rw-   0        0        0     2011 2024-06-03 08:29:32.000000 apiamocrm-0.1.9/amoChatApi/Payload.py
+-rw-rw-rw-   0        0        0      994 2024-06-03 08:30:59.000000 apiamocrm-0.1.9/amoChatApi/PhotoMessage.py
+-rw-rw-rw-   0        0        0      392 2024-06-03 04:11:18.000000 apiamocrm-0.1.9/amoChatApi/TextMessage.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 10:16:39.000000 apiamocrm-0.1.9/amoChatApi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:05.795705 apiamocrm-0.1.9/apiAmoCRM.egg-info/
+-rw-rw-rw-   0        0        0      438 2024-06-03 09:28:05.000000 apiamocrm-0.1.9/apiAmoCRM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-06-03 09:28:05.000000 apiamocrm-0.1.9/apiAmoCRM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:28:05.000000 apiamocrm-0.1.9/apiAmoCRM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 09:28:05.000000 apiamocrm-0.1.9/apiAmoCRM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-03 09:28:05.000000 apiamocrm-0.1.9/apiAmoCRM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 09:28:05.797722 apiamocrm-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      633 2024-06-03 09:27:55.000000 apiamocrm-0.1.9/setup.py
```

### Comparing `apiamocrm-0.1.8/amoApi/API.py` & `apiamocrm-0.1.9/amoApi/API.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.8/amoApi/amoEntities/Contact.py` & `apiamocrm-0.1.9/amoApi/amoEntities/Contact.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.8/amoApi/amoEntities/Lead.py` & `apiamocrm-0.1.9/amoApi/amoEntities/Lead.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.8/amoChatApi/API.py` & `apiamocrm-0.1.9/amoChatApi/API.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,39 @@
         headers = {
             "Date": date,
             "Content-Type": self._content_type,
             'Content-MD5': checksum,
             'X-Signature': signature,
         }
         response = requests.post(send_or_edit_message_url, data=request_body, headers=headers)
+        response.raise_for_status()
+        return response
+
+    def change_message_status(self, msgid:str, delivery_status:int, error_code:int, error:str):
+        path = self._path + self._scope_id
+        url = self._url + path
+        body = {
+            "msgid":msgid,
+            "delivery_status":delivery_status,
+            "error_code":error_code,
+            "error":error
+        }
+        request_body = json.dumps(body)
+        checksum = hashlib.md5(request_body.encode("utf-8")).hexdigest()
+        date = formatdate(timeval=None, localtime=False, usegmt=True)
+        str_to_sign = "\n".join(["POST", checksum, self._content_type, date, path])
+        signature = hmac.new(self._secret.encode("utf-8"), str_to_sign.encode("utf-8"), hashlib.sha1).hexdigest()
+        headers = {
+            "Date": date,
+            "Content-Type": self._content_type,
+            'Content-MD5': checksum,
+            'X-Signature': signature,
+        }
+        response = requests.post(url, data=request_body, headers=headers)
+        response.raise_for_status()
         return response
 
     def create_new_text_message(self):
         return Payload(self)
     def create_new_photo_message(self):
         return Payload(self, "photo")
```

### Comparing `apiamocrm-0.1.8/amoChatApi/Payload.py` & `apiamocrm-0.1.9/amoChatApi/Payload.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.8/amoChatApi/PhotoMessage.py` & `apiamocrm-0.1.9/amoChatApi/PhotoMessage.py`

 * *Files identical despite different names*

### Comparing `apiamocrm-0.1.8/setup.py` & `apiamocrm-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='apiAmoCRM',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author='wlovem',
     author_email='wlovemrock@gmail.com',
     description='Api for amoCRM',
```

