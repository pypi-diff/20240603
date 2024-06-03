# Comparing `tmp/tmdbtraktsyncer-1.7.0.tar.gz` & `tmp/tmdbtraktsyncer-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmdbtraktsyncer-1.7.0.tar", last modified: Thu May 23 12:13:53 2024, max compression
+gzip compressed data, was "tmdbtraktsyncer-1.7.1.tar", last modified: Mon Jun  3 03:16:45 2024, max compression
```

## Comparing `tmdbtraktsyncer-1.7.0.tar` & `tmdbtraktsyncer-1.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 12:13:53.680636 tmdbtraktsyncer-1.7.0/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 tmdbtraktsyncer-1.7.0/LICENSE
--rw-rw-rw-   0        0        0    11457 2024-05-23 12:13:53.677636 tmdbtraktsyncer-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    10683 2024-05-23 12:12:53.000000 tmdbtraktsyncer-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 12:13:53.645636 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    18294 2024-05-23 11:44:31.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-07-31 05:41:54.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     6379 2023-11-09 08:07:17.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     1952 2024-05-23 11:39:00.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/checkVersion.py
--rw-rw-rw-   0        0        0    10185 2023-11-09 06:21:42.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1642 2023-11-28 22:57:57.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0     4058 2023-11-08 13:56:56.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     7135 2023-10-13 00:03:27.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     9367 2024-05-23 11:39:52.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:13:53.676635 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    11457 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 12:13:53.680636 tmdbtraktsyncer-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1341 2024-05-23 12:13:18.000000 tmdbtraktsyncer-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:16:45.874931 tmdbtraktsyncer-1.7.1/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 tmdbtraktsyncer-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0    11457 2024-06-03 03:16:45.872942 tmdbtraktsyncer-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10683 2024-05-23 12:12:53.000000 tmdbtraktsyncer-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 03:16:45.832933 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    18294 2024-05-23 11:44:31.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 05:41:54.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-11-09 08:07:17.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     1936 2024-06-03 03:13:03.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/checkVersion.py
+-rw-rw-rw-   0        0        0    10185 2023-11-09 06:21:42.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1642 2023-11-28 22:57:57.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0     4058 2023-11-08 13:56:56.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7135 2023-10-13 00:03:27.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     9344 2024-05-24 14:09:55.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:16:45.869931 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11457 2024-06-03 03:16:45.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2024-06-03 03:16:45.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 03:16:45.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-06-03 03:16:45.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 03:16:45.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-03 03:16:45.000000 tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 03:16:45.874931 tmdbtraktsyncer-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2024-06-03 03:16:17.000000 tmdbtraktsyncer-1.7.1/setup.py
```

### Comparing `tmdbtraktsyncer-1.7.0/LICENSE` & `tmdbtraktsyncer-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/PKG-INFO` & `tmdbtraktsyncer-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tmdbtraktsyncer-1.7.0/README.md` & `tmdbtraktsyncer-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/TMDBTraktSyncer.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/authTrakt.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/checkVersion.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/checkVersion.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def compare_versions(installed, latest):
     def parse_version(v):
         return tuple(map(int, v.split('.')))
     
     return parse_version(installed) < parse_version(latest)
 
-def main():
+def checkVersion():
     installed_version = get_installed_version()
     if not installed_version:
         print("TMDBTraktSyncer is not installed.")
         return
 
     latest_version = get_latest_version()
     if not latest_version:
@@ -45,9 +45,8 @@
     if compare_versions(installed_version, latest_version):
         print(f"A new version of TMDBTraktSyncer is available: {latest_version} (installed: {installed_version}).")
         print("To update use: python -m pip install TMDBTraktSyncer --upgrade")
         print("Documentation: https://github.com/RileyXX/TMDB-Trakt-Syncer")
     # else:
         # print(f"TMDBTraktSyncer is up to date (installed: {installed_version})")
 
-if __name__ == "__main__":
-    main()
+checkVersion()
```

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorHandling.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorLogger.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/tmdbData.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/traktData.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/verifyCredentials.py` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer/verifyCredentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     import authTrakt
     import errorLogger as EL
 
 def prompt_get_credentials():
     # Define the file path
     here = os.path.abspath(os.path.dirname(__file__))
     file_path = os.path.join(here, 'credentials.txt')
-    print(f"Your credentials and error log files are saved at:\n{here}")
+    print(f"Your settings are saved at:\n{here}")
 
     default_values = {
         "trakt_client_id": "empty",
         "trakt_client_secret": "empty",
         "trakt_access_token": "empty",
         "trakt_refresh_token": "empty",
         "tmdb_access_token": "empty",
```

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/PKG-INFO` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.7.0
+Version: 1.7.1
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/SOURCES.txt` & `tmdbtraktsyncer-1.7.1/TMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmdbtraktsyncer-1.7.0/setup.py` & `tmdbtraktsyncer-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.7.0'
+VERSION = '1.7.1'
 DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

