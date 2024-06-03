# Comparing `tmp/aparatlib-0.1.3.tar.gz` & `tmp/aparatlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aparatlib-0.1.3.tar", last modified: Mon Jun  3 09:44:58 2024, max compression
+gzip compressed data, was "aparatlib-0.2.0.tar", last modified: Mon Jun  3 14:06:51 2024, max compression
```

## Comparing `aparatlib-0.1.3.tar` & `aparatlib-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 09:44:58.330101 aparatlib-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-06-03 09:44:58.329119 aparatlib-0.1.3/AparatLib.egg-info/
--rw-rw-rw-   0        0        0     1023 2024-06-03 09:44:58.000000 aparatlib-0.1.3/AparatLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-06-03 09:44:58.000000 aparatlib-0.1.3/AparatLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 09:44:58.000000 aparatlib-0.1.3/AparatLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 09:44:58.000000 aparatlib-0.1.3/AparatLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-03 09:44:58.000000 aparatlib-0.1.3/AparatLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-06-02 06:49:28.000000 aparatlib-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1023 2024-06-03 09:44:58.329119 aparatlib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      503 2024-06-03 09:42:32.000000 aparatlib-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 09:44:58.326214 aparatlib-0.1.3/aparat/
--rw-rw-rw-   0        0        0       52 2024-06-02 06:45:10.000000 aparatlib-0.1.3/aparat/__init__.py
--rw-rw-rw-   0        0        0    17528 2024-06-03 09:22:03.000000 aparatlib-0.1.3/aparat/aparat.py
--rw-rw-rw-   0        0        0       42 2024-06-03 09:44:58.330101 aparatlib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      790 2024-06-03 09:44:46.000000 aparatlib-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-03 09:44:58.328154 aparatlib-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-06-02 06:44:06.000000 aparatlib-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0      977 2024-06-02 09:38:58.000000 aparatlib-0.1.3/tests/test_aparat.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:06:51.335625 aparatlib-0.2.0/
+drwxrwxrwx   0        0        0        0 2024-06-03 14:06:51.334648 aparatlib-0.2.0/AparatLib.egg-info/
+-rw-rw-rw-   0        0        0     1023 2024-06-03 14:06:51.000000 aparatlib-0.2.0/AparatLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-06-03 14:06:51.000000 aparatlib-0.2.0/AparatLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:06:51.000000 aparatlib-0.2.0/AparatLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 14:06:51.000000 aparatlib-0.2.0/AparatLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 14:06:51.000000 aparatlib-0.2.0/AparatLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-06-02 06:49:28.000000 aparatlib-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1023 2024-06-03 14:06:51.335625 aparatlib-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2024-06-03 09:42:32.000000 aparatlib-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 14:06:51.333673 aparatlib-0.2.0/aparat/
+-rw-rw-rw-   0        0        0       52 2024-06-02 06:45:10.000000 aparatlib-0.2.0/aparat/__init__.py
+-rw-rw-rw-   0        0        0    18490 2024-06-03 14:04:09.000000 aparatlib-0.2.0/aparat/aparat.py
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:06:51.336601 aparatlib-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      790 2024-06-03 14:06:25.000000 aparatlib-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:06:51.334648 aparatlib-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-02 06:44:06.000000 aparatlib-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-06-02 09:38:58.000000 aparatlib-0.2.0/tests/test_aparat.py
```

### Comparing `aparatlib-0.1.3/AparatLib.egg-info/PKG-INFO` & `aparatlib-0.2.0/AparatLib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AparatLib
-Version: 0.1.3
+Version: 0.2.0
 Summary: A library for interacting with the Aparat API
 Home-page: https://github.com/AbolDev/AparatLib
 Author: Abol
 Author-email: abaqry8686@gmail.com
 Keywords: Aparat API video streaming python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aparatlib-0.1.3/LICENSE` & `aparatlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aparatlib-0.1.3/PKG-INFO` & `aparatlib-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AparatLib
-Version: 0.1.3
+Version: 0.2.0
 Summary: A library for interacting with the Aparat API
 Home-page: https://github.com/AbolDev/AparatLib
 Author: Abol
 Author-email: abaqry8686@gmail.com
 Keywords: Aparat API video streaming python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aparatlib-0.1.3/aparat/aparat.py` & `aparatlib-0.2.0/aparat/aparat.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,39 +34,39 @@
         self.message = message
         super().__init__(self.message)
 
 class Video(object):
     """ Aparat Video Model
         
     Attributes:
-        id (str): The ID of the video.
+        id (int): The ID of the video.
         title (str): The title of the video.
         description (str): The description of the video.
         uid (str): The UID of the video.
         visit_cnt (int): The visit count of the video.
-        visit_cnt_non_formatted (str): The non-formatted visit count of the video.
-        like_cnt_non_formatted (str): The non-formatted like count of the video.
+        visit_cnt_non_formatted (int): The non-formatted visit count of the video.
+        like_cnt_non_formatted (int): The non-formatted like count of the video.
         big_poster (str): The URL of the big poster of the video.
         medium_poster (str): The URL of the medium poster of the video.
         small_poster (str): The URL of the small poster of the video.
         duration (str): The duration of the video.
         meta_duration (str): The meta duration of the video.
         date_exact (str): The exact date of the video.
         sdate (str): The sdate of the video.
-        sdate_timediff (str): The time difference of the video.
+        sdate_timediff (int): The time difference of the video.
         sdate_real (str): The real sdate of the video.
         deleted (str): The deleted status of the video.
         mdate (str): The mdate of the video.
-        file_link_all (str): The all file link of the video.
+        file_link_all (List[Dict[str, Union[str, List[str]]]]): List of dictionaries containing file links and their details.
         file_link (str): The file link of the video.
         hls_link (str): The HLS link of the video.
-        can_download (str): The download status of the video.
+        can_download (bool): The download status of the video.
         tags (str): The tags of the video.
         tags_str (str): The string representation of tags of the video.
-        tags_fa (str): The Persian tags of the video.
+        tags_fa (List[str]): The Persian tags of the video.
         frame_src (str): The frame source of the video.
         category (str): The category of the video.
         360d (str): The 360d status of the video.
         comment_enable (str): The comment enable status of the video.
         official (str): The official status of the video.
         extra_data (str): The extra data of the video.
         content_type (str): The content type of the video.
@@ -90,15 +90,15 @@
                        'meta_duration', 'date_exact', 'sdate', 'sdate_timediff', 'sdate_real', 'deleted', 'mdate',
                        'file_link_all', 'file_link', 'hls_link', 'can_download', 'tags', 'tags_str', 'tags_fa',
                        'frame_src', 'category', '360d', 'comment_enable', 'official', 'extra_data', 'content_type',
                        'file_hash', 'isCompany', 'isAbroad', 'kids_friendly', 'owner_username', 'max_width',
                        'max_height']:
                 setattr(self, key, value)
     
-    def commentSend(self, comment):
+    def send_comment(self, comment):
         """Send a comment for this video.
 
         Args:
             comment (str): The comment to be sent.
         """
         if not self.is_logged_in:
             raise LoginRequiredError()
@@ -109,25 +109,133 @@
         if self.data['data']['attributes']['comment_enable'] != 'yes':
             raise ValueError("Comments are disabled for this video.")
 
         data = {'commentbody': comment}
         response = self.session.post(self.data['data']['attributes']['commentSendLink'], data=data)
         
         return response.json()
+    
+    def like(self, timeout: int = 10) -> bool:
+        """
+        Like a video.
+
+        :param timeout: The timeout for the HTTP request (default is 10 seconds).
+        :return: True if the video is successfully liked, False otherwise.
+        """
+
+        for item in self.data['included']:
+            if 'type' in item and item['type'] == 'Like':
+                if item['attributes']['status'] == 'unlike':
+                    follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
+                    if follow_response.status_code == 200:
+                        return True
+        return False
+
+    def unlike(self, timeout: int = 10) -> bool:
+        """
+        Unlike a video.
+
+        :param timeout: The timeout for the HTTP request (default is 10 seconds).
+        :return: True if the video is successfully liked, False otherwise.
+        """
+
+        for item in self.data['included']:
+            if 'type' in item and item['type'] == 'Like':
+                if item['attributes']['status'] == 'like':
+                    follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
+                    if follow_response.status_code == 200:
+                        return True
+        return False
+
+class User(object):
+    """ Aparat User Model
+        
+    Attributes:
+        id (str): The unique identifier of the user.
+        hash_user_id (str): The hashed identifier of the user.
+        afcn (str): The user's name in a format suitable for related publications.
+        username (str): The username of the user.
+        name (str): The name of the user.
+        pic_s (str): The URL of the small profile picture of the user.
+        pic_m (str): The URL of the medium profile picture of the user.
+        pic_b (str): The URL of the large profile picture of the user.
+        follower_cnt (int): The number of followers of the user.
+        follow_cnt (int): The number of users that the user follows.
+        official (str): The official status of the user.
+        url (str): The URL of the user's profile.
+        video_cnt (int): The number of videos uploaded by the user.
+        cover_src (str): The URL of the user's cover image.
+        video_visit (int): The number of visits to the user's videos.
+        priority (str): The priority of the user.
+        brand_priority (str): The brand priority of the user.
+        description (str): The description of the user.
+        start_date (str): The start date of the user's activity.
+        start_date_jalali (str): The start date of the user's activity in the Jalali calendar.
+        show_kids_friendly (str): The display of a suitable label for children.
+        banned (str): The banned status of the user.
+        has_event (str): The event status of the user.
+    """
+
+    def __init__(self, data: Dict[str, Union[str, int]], is_logged_in, session):
+        self.data = data
+        self.is_logged_in = is_logged_in
+        self.session = session
+        data_ = data['data']['attributes']
+        for key, value in data_.items():
+            if key in ['id', 'hash_user_id', 'afcn', 'username', 'name', 'pic_s', 'pic_m', 'pic_b', 'follower_cnt',
+                       'follow_cnt', 'official', 'url', 'video_cnt', 'cover_src', 'video_visit', 'priority', 'brand_priority',
+                       'description', 'start_date', 'start_date_jalali','show_kids_friendly', 'banned', 'has_event']:
+                setattr(self, key, value)
+    
+    def follow(self, timeout: int = 10) -> bool:
+        """
+        Follow a user.
+
+        :param timeout: The timeout for the HTTP request (default is 10 seconds).
+        :return: True if the user is successfully followed, False otherwise.
+        """
+        if not self.is_logged_in:
+            raise LoginRequiredError()
+
+        for item in self.data['included']:
+            if item['type'] == 'Follow':
+                if item['attributes']['status'] == 'unfollow':
+                    follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
+                    if follow_response.status_code == 200:
+                        return True
+        return False
+
+    def unfollow(self, timeout: int = 10) -> bool:
+        """
+        Unfollow a user.
+
+        :param timeout: The timeout for the HTTP request (default is 10 seconds).
+        :return: True if the user is successfully followed, False otherwise.
+        """
+        if not self.is_logged_in:
+            raise LoginRequiredError()
+
+        for item in self.data['included']:
+            if item['type'] == 'Follow':
+                if item['attributes']['status'] == 'follow':
+                    follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
+                    if follow_response.status_code == 200:
+                        return True
+        return False
 
 class Aparat:
     """Aparat API Client
     
     Attributes:
         proxy (str): The proxy URL, if used.
         session (requests.Session): The requests session object.
         is_logged_in (bool): Flag indicating if the client is logged in.
     """
 
-    def __init__(self, proxy=None):
+    def __init__(self, timeout: int = 10, proxy: str = None):
         """Initialize Aparat API client.
         
         Args:
             proxy (str, optional): The proxy URL. Defaults to None.
         """
         self.session = requests.Session()
         self.is_logged_in = False
@@ -217,26 +325,26 @@
 
         response = self.session.get(f'{base_url}/api/fa/v1/user/user/information', timeout=timeout)
         if response.status_code == 200:
             data = response.json()
             return data['data']
         return None
 
-    def username_information(self, user_id: str, timeout: int = 10) -> Union[Dict, None]:
+    def get_user(self, user_id: str, timeout: int = 10) -> User:
         """
         Get information about a user by their username.
 
         :param user_id: The username of the user.
         :param timeout: The timeout for the HTTP request (default is 10 seconds).
         :return: A dictionary containing user information if successful, otherwise None.
         """
         response = self.session.get(f'{base_url}/api/fa/v1/user/user/information/username/{user_id}', timeout=timeout)
         if response.status_code == 200:
             data = response.json()
-            return data['data']
+            return User(data, self.is_logged_in, self.session)
         return None
 
     def notifications(self, timeout: int = 10) -> Union[Dict, None]:
         """
         Get notifications for the current user.
 
         :param timeout: The timeout for the HTTP request (default is 10 seconds).
@@ -257,110 +365,14 @@
         """
         response = self.session.get(f'{base_url}/api/fa/v1/user/dashboard/comments/list_type/all', timeout=timeout)
         if response.status_code == 200:
             data = response.json()
             return data
         return None
 
-    def follow(self, user_id: str, timeout: int = 10) -> bool:
-        """
-        Follow a user.
-
-        :param user_id: The ID of the user to follow.
-        :param timeout: The timeout for the HTTP request (default is 10 seconds).
-        :return: True if the user is successfully followed, False otherwise.
-        """
-        if not self.is_logged_in:
-            raise LoginRequiredError()
-
-        response = self.session.get(f'{base_url}/api/fa/v1/user/user/information/username/{user_id}', timeout=timeout)
-
-        if response.status_code == 200:
-            data = response.json()
-            for item in data['included']:
-                if item['type'] == 'Follow':
-                    if item['attributes']['status'] == 'unfollow':
-                        follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
-                        if follow_response.status_code == 200:
-                            return True
-            return False
-        else:
-            raise UsernameNotFoundError()
-
-    def unfollow(self, user_id: str, timeout: int = 10) -> bool:
-        """
-        Unfollow a user.
-
-        :param user_id: The ID of the user to unfollow.
-        :param timeout: The timeout for the HTTP request (default is 10 seconds).
-        :return: True if the user is successfully unfollowed, False otherwise.
-        """
-        if not self.is_logged_in:
-            raise LoginRequiredError()
-
-        response = self.session.get(f'{base_url}/api/fa/v1/user/user/information/username/{user_id}', timeout=timeout)
-
-        if response.status_code == 200:
-            data = response.json()
-            for item in data['included']:
-                if item['type'] == 'Follow':
-                    if item['attributes']['status'] == 'follow':
-                        follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
-                        if follow_response.status_code == 200:
-                            return True
-            return False
-        else:
-            raise UsernameNotFoundError()
-
-    def like(self, vid: str, timeout: int = 10) -> bool:
-        """
-        Like a video.
-
-        :param vid: The ID of the video to like.
-        :param timeout: The timeout for the HTTP request (default is 10 seconds).
-        :return: True if the video is successfully liked, False otherwise.
-        """
-
-        response = self.session.get(f'{base_url}/api/fa/v1/video/video/show/videohash/{vid}?pr=1&mf=1', timeout=timeout)
-        data = response.json()
-
-        if 'meta' in data and 'status' not in data['meta']:
-            for item in data['included']:
-                if 'type' in item and item['type'] == 'Like':
-                    if item['attributes']['status'] == 'unlike':
-                        follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
-                        if follow_response.status_code == 200:
-                            return True
-            return False
-        else:
-            raise VideoNotFoundError()
-
-    def unlike(self, vid: str, timeout: int = 10) -> bool:
-        """
-        Unlike a video.
-
-        :param vid: The ID of the video to unlike.
-        :param timeout: The timeout for the HTTP request (default is 10 seconds).
-        :return: True if the video is successfully unliked, False otherwise.
-        """
-
-        response = self.session.get(f'{base_url}/api/fa/v1/video/video/show/videohash/{vid}?pr=1&mf=1', timeout=timeout)
-        data = response.json()
-
-        if 'meta' in data and 'status' not in data['meta']:
-            for item in data['included']:
-                if item['type'] == 'Like':
-                    if item['attributes']['status'] == 'like':
-                        follow_response = self.session.get(item['attributes']['link'], timeout=timeout)
-                        if follow_response.status_code == 200:
-                            return True
-            return False
-        else:
-            raise VideoNotFoundError()
-
     def get_video(self, vid: str, timeout: int = 10) -> Video:
         """Get video details from Aparat.
         
         Args:
             vid (str): The video ID.
             timeout (int, optional): The request timeout. Defaults to 10.
```

### Comparing `aparatlib-0.1.3/setup.py` & `aparatlib-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='AparatLib',
-    version='0.1.3',
+    version='0.2.0',
     packages=find_packages(),
     author='Abol',
     author_email='abaqry8686@gmail.com',
     description='A library for interacting with the Aparat API',
     long_description=open('C:\\Users\\Bagheri\\Desktop\\projects\\python\\Github projects\\aparat\\README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/AbolDev/AparatLib',
```

### Comparing `aparatlib-0.1.3/tests/test_aparat.py` & `aparatlib-0.2.0/tests/test_aparat.py`

 * *Files identical despite different names*

