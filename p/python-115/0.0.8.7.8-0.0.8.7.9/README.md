# Comparing `tmp/python_115-0.0.8.7.8.tar.gz` & `tmp/python_115-0.0.8.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.7.8.tar", max compression
+gzip compressed data, was "python_115-0.0.8.7.9.tar", max compression
```

## Comparing `python_115-0.0.8.7.8.tar` & `python_115-0.0.8.7.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.8/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.8/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.8/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.8/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     2394 2024-06-01 07:45:37.499962 python_115-0.0.8.7.8/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.8/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.8/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.8/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.8/p115/cmd/init.py
--rwxr-xr-x   0        0        0    10048 2024-06-02 09:13:32.245014 python_115-0.0.8.7.8/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2107 2024-06-01 06:14:01.276468 python_115-0.0.8.7.8/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.8/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.8/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.8/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.8/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.8/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.8/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.8/p115/component/cipher.py
--rwxr-xr-x   0        0        0   265176 2024-06-02 07:24:06.942442 python_115-0.0.8.7.8/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.8/p115/component/exception.py
--rwxr-xr-x   0        0        0    69332 2024-06-02 11:48:03.668857 python_115-0.0.8.7.8/p115/component/fs.py
--rwxr-xr-x   0        0        0    49142 2024-06-02 06:13:46.742966 python_115-0.0.8.7.8/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    15205 2024-06-02 05:55:36.365281 python_115-0.0.8.7.8/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10263 2024-06-02 05:51:11.710739 python_115-0.0.8.7.8/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.8/p115/component/labellist.py
--rwxr-xr-x   0        0        0    10286 2024-06-02 06:30:40.250415 python_115-0.0.8.7.8/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.8/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.8/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.8/p115/py.typed
--rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.8/p115/tool/__init__.py
--rw-r--r--   0        0        0     1687 2024-06-02 11:55:42.248657 python_115-0.0.8.7.8/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-06-02 05:53:33.629676 python_115-0.0.8.7.8/readme.md
--rw-r--r--   0        0        0    36409 1970-01-01 00:00:00.000000 python_115-0.0.8.7.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.9/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.9/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.9/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.9/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     2394 2024-06-01 07:45:37.499962 python_115-0.0.8.7.9/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.9/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.9/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.9/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.9/p115/cmd/init.py
+-rwxr-xr-x   0        0        0    10048 2024-06-02 09:13:32.245014 python_115-0.0.8.7.9/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2107 2024-06-01 06:14:01.276468 python_115-0.0.8.7.9/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.9/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.9/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.9/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.9/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.9/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.9/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.9/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   265176 2024-06-02 07:24:06.942442 python_115-0.0.8.7.9/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.9/p115/component/exception.py
+-rwxr-xr-x   0        0        0    69379 2024-06-03 03:29:07.732641 python_115-0.0.8.7.9/p115/component/fs.py
+-rwxr-xr-x   0        0        0    49142 2024-06-02 06:13:46.742966 python_115-0.0.8.7.9/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    15205 2024-06-02 05:55:36.365281 python_115-0.0.8.7.9/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10263 2024-06-02 05:51:11.710739 python_115-0.0.8.7.9/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.9/p115/component/labellist.py
+-rwxr-xr-x   0        0        0    10286 2024-06-02 06:30:40.250415 python_115-0.0.8.7.9/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.9/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.9/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.9/p115/py.typed
+-rwxr-xr-x   0        0        0     8680 2024-05-30 17:44:22.674012 python_115-0.0.8.7.9/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1687 2024-06-03 03:29:45.342478 python_115-0.0.8.7.9/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-06-02 05:53:33.629676 python_115-0.0.8.7.9/readme.md
+-rw-r--r--   0        0        0    36409 1970-01-01 00:00:00.000000 python_115-0.0.8.7.9/PKG-INFO
```

### Comparing `python_115-0.0.8.7.8/LICENSE` & `python_115-0.0.8.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/cmd/check.py` & `python_115-0.0.8.7.9/p115/cmd/check.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/cmd/iterdir.py` & `python_115-0.0.8.7.9/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/cmd/qrcode.py` & `python_115-0.0.8.7.9/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/__init__.py` & `python_115-0.0.8.7.9/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/cipher.py` & `python_115-0.0.8.7.9/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/client.py` & `python_115-0.0.8.7.9/p115/component/client.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/fs.py` & `python_115-0.0.8.7.9/p115/component/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
     ) -> AttrDict:
         if payload is None:
             payload = self.id
         if isinstance(payload, int):
             id = payload
         else:
             id = int(payload["cid"])
-        resp = check_response(self.client.fs_files(payload))
+        resp = check_response(self.client.fs_files2(payload))
         if int(resp["path"][-1]["cid"]) != id:
             raise NotADirectoryError(errno.ENOTDIR, f"{id!r} is not a directory")
         return resp
 
     @check_response
     def fs_search(self, payload: str | dict, /) -> AttrDict:
         if isinstance(payload, str):
@@ -799,27 +799,28 @@
                     if start is None:
                         start = 0
                     elif start < 0:
                         count = self.dirlen(id)
                         start += count
                         if start < 0:
                             start = 0
-                    if stop is None or stop < 0:
-                        if count < 0:
-                            count = self.dirlen(id)
-                        if stop is None:
-                            stop = count
-                        else:
+                    if stop is not None:
+                        if stop < 0:
+                            if count < 0:
+                                count = self.dirlen(id)
                             stop += count
-                    if start >= stop or stop <= 0 or count >= 0 and start >= count:
+                        if start >= stop or stop <= 0:
+                            return
+                    if count >= 0 and start >= count:
                         return
                     payload["offset"] = start
-                    total = stop - start
-                    if total < page_size:
-                        payload["limit"] = total
+                    if stop is not None:
+                        total = stop - start
+                        if total < page_size:
+                            payload["limit"] = total
                     set_order_payload = {}
                     if "o" in payload:
                         set_order_payload["user_order"] = payload["o"]
                     if "asc" in payload:
                         set_order_payload["user_asc"] = payload["asc"]
                     if set_order_payload:
                         set_order_payload["file_id"] = id
@@ -830,15 +831,15 @@
                 dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
                 if path_to_id is not None:
                     path_to_id[dirname] = id
                 count = resp["count"]
                 for attr in resp["data"]:
                     yield normalize_attr(attr, dirname, fs=self)
                 if total < 0:
-                    total = count
+                    total = count - start
                 if total <= page_size:
                     return
                 for _ in range((total - 1) // page_size + 1):
                     payload["offset"] += page_size
                     resp = get_files(payload)
                     if resp["count"] != count:
                         raise RuntimeError(f"{id} detected count changes during iteration")
```

### Comparing `python_115-0.0.8.7.8/p115/component/fs_base.py` & `python_115-0.0.8.7.9/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/fs_share.py` & `python_115-0.0.8.7.9/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/fs_zip.py` & `python_115-0.0.8.7.9/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/labellist.py` & `python_115-0.0.8.7.9/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/offline.py` & `python_115-0.0.8.7.9/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/recyclebin.py` & `python_115-0.0.8.7.9/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/component/sharing.py` & `python_115-0.0.8.7.9/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/p115/tool/__init__.py` & `python_115-0.0.8.7.9/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/pyproject.toml` & `python_115-0.0.8.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.7.8"
+version = "0.0.8.7.9"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.7.8/readme.md` & `python_115-0.0.8.7.9/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7.8/PKG-INFO` & `python_115-0.0.8.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.7.8
+Version: 0.0.8.7.9
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

