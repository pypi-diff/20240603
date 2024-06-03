# Comparing `tmp/imdbtraktsyncer-1.9.0.tar.gz` & `tmp/imdbtraktsyncer-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imdbtraktsyncer-1.9.0.tar", last modified: Thu May 23 12:11:47 2024, max compression
+gzip compressed data, was "imdbtraktsyncer-1.9.1.tar", last modified: Mon Jun  3 02:25:05 2024, max compression
```

## Comparing `imdbtraktsyncer-1.9.0.tar` & `imdbtraktsyncer-1.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 12:11:47.079138 imdbtraktsyncer-1.9.0/
-drwxrwxrwx   0        0        0        0 2024-05-23 12:11:47.054137 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    42098 2024-05-23 11:42:40.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     6398 2023-11-09 08:08:16.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4274 2023-08-08 21:16:45.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     1952 2024-05-23 11:35:10.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/checkVersion.py
--rw-rw-rw-   0        0        0     6946 2023-08-02 06:46:34.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2024-05-19 13:42:35.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    15966 2024-05-23 11:15:28.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10587 2023-10-13 00:03:11.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    13298 2024-05-23 11:30:12.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:11:47.076138 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12838 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 12:11:46.000000 imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 imdbtraktsyncer-1.9.0/LICENSE
--rw-rw-rw-   0        0        0    12838 2024-05-23 12:11:47.077137 imdbtraktsyncer-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0    11988 2024-05-23 12:10:15.000000 imdbtraktsyncer-1.9.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 12:11:47.079138 imdbtraktsyncer-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1390 2024-05-23 11:47:49.000000 imdbtraktsyncer-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:25:05.694299 imdbtraktsyncer-1.9.1/
+drwxrwxrwx   0        0        0        0 2024-06-03 02:25:05.655300 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    42098 2024-06-03 01:08:48.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     6398 2023-11-09 08:08:16.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4274 2023-08-08 21:16:45.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     1952 2024-05-23 11:35:10.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/checkVersion.py
+-rw-rw-rw-   0        0        0     6946 2023-08-02 06:46:34.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2024-05-19 13:42:35.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    17859 2024-06-03 02:22:14.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10587 2024-06-03 01:09:12.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    13275 2024-05-24 14:10:30.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2024-06-03 02:25:05.690308 imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12838 2024-06-03 02:25:05.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-06-03 02:25:05.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 02:25:05.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-06-03 02:25:05.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-06-03 02:25:05.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-03 02:25:05.000000 imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 imdbtraktsyncer-1.9.1/LICENSE
+-rw-rw-rw-   0        0        0    12838 2024-06-03 02:25:05.692308 imdbtraktsyncer-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11988 2024-06-03 02:23:55.000000 imdbtraktsyncer-1.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 02:25:05.694299 imdbtraktsyncer-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1390 2024-06-03 02:23:34.000000 imdbtraktsyncer-1.9.1/setup.py
```

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/IMDBTraktSyncer.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/authTrakt.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/checkChromedriver.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/checkVersion.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/checkVersion.py`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorHandling.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/errorLogger.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/imdbData.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/imdbData.py`

 * *Files 14% similar despite different names*

```diff
@@ -120,31 +120,49 @@
             if not csv_files:
                 raise FileNotFoundError("Watchlist data not found. No CSV files found in the directory")
             
             # Use the first CSV file found 
             watchlist_path = os.path.join(directory, csv_files[0])
             with open(watchlist_path, 'r', encoding='utf-8') as file:
                 reader = csv.reader(file)
-                header = next(reader)  # skip the header row
+                header = next(reader)  # Read the header row
+
+                # Create a mapping from header names to their index
+                header_index = {column_name: index for index, column_name in enumerate(header)}
+                
+                required_columns = ["Title", "Year", "Const", "Created", "Title Type"]
+                missing_columns = [col for col in required_columns if col not in header_index]
+                if missing_columns:
+                    raise ValueError(f"Required columns missing from CSV file: {', '.join(missing_columns)}")
+
                 for row in reader:
-                    title = row[5]
-                    year = row[10]
-                    imdb_id = row[1]
-                    date_added = row[2]
+                    title = row[header_index['Title']]
+                    year = row[header_index['Year']]
+                    imdb_id = row[header_index['Const']]
+                    date_added = row[header_index['Created']]
+                    media_type = row[header_index['Title Type']]
                     # Convert date format
                     date_added = datetime.strptime(date_added, '%Y-%m-%d').strftime('%Y-%m-%dT%H:%M:%S.000Z')
-                    if "tvSeries" in row[7] or "tvMiniSeries" in row[7]:
+                    if "TV Series" in media_type or "TV Mini Series" in media_type:
                         media_type = "show"
-                    elif "tvEpisode" in row[7]:
+                    elif "TV Episode" in media_type:
                         media_type = "episode"
-                    elif "movie" in row[7] or "tvSpecial" in row[7] or "tvMovie" in row[7] or "tvShort" in row[7] or "video" in row[7]:
+                    elif any(media in media_type for media in ["Movie", "TV Special", "TV Movie", "TV Short", "Video"]):
                         media_type = "movie"
                     else:
                         media_type = "unknown"
-                    imdb_watchlist.append({'Title': title, 'Year': year, 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
+                    
+                    imdb_watchlist.append({
+                        'Title': title,
+                        'Year': year,
+                        'IMDB_ID': imdb_id,
+                        'Date_Added': date_added,
+                        'Type': media_type
+                    })
+            
         except FileNotFoundError as e:
             print(f"Error: {error_message}", exc_info=True)
             EL.logger.error(error_message, exc_info=True)
 
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv'):
@@ -197,36 +215,55 @@
             if not csv_files:
                 raise FileNotFoundError("Ratings data not found. No CSV files found in the directory")
                 
             # Use the first CSV file found 
             ratings_path = os.path.join(directory, csv_files[0])
             with open(ratings_path, 'r', encoding='utf-8') as file:
                 reader = csv.reader(file)
-                header = next(reader)  # skip the header row
+                header = next(reader)  # Read the header row
+
+                # Create a mapping from header names to their index
+                header_index = {column: index for index, column in enumerate(header)}
+                
+                required_columns = ["Title", "Year", "Your Rating", "Const", "Date Rated", "Title Type"]
+                missing_columns = [col for col in required_columns if col not in header_index]
+                if missing_columns:
+                    raise ValueError(f"Required columns missing from CSV file: {', '.join(missing_columns)}")
+
                 for row in reader:
-                    title = row[3]
-                    year = row[8]
-                    rating = row[1]
-                    imdb_id = row[0]
-                    date_added = row[2]
-                    # Convert date format
-                    date_added = datetime.strptime(date_added, '%Y-%m-%d').strftime('%Y-%m-%dT%H:%M:%S.000Z')
-                    if "tvSeries" in row[5] or "tvMiniSeries" in row[5]:
-                        media_type = "show"
-                    elif "tvEpisode" in row[5]:
-                        media_type = "episode"
-                    elif "movie" in row[5] or "tvSpecial" in row[5] or "tvMovie" in row[5] or "tvShort" in row[5] or "video" in row[5]:
-                        media_type = "movie"
-                    else:
-                        media_type = "unknown"
-                    imdb_ratings.append({'Title': title, 'Year': year, 'Rating': int(rating), 'IMDB_ID': imdb_id, 'Date_Added': date_added, 'Type': media_type})
+                        title = row[header_index['Title']]
+                        year = row[header_index['Year']]
+                        rating = row[header_index['Your Rating']]
+                        imdb_id = row[header_index['Const']]
+                        date_added = row[header_index['Date Rated']]
+                        media_type = row[header_index['Title Type']]
+                        # Convert date format
+                        date_added = datetime.strptime(date_added, '%Y-%m-%d').strftime('%Y-%m-%dT%H:%M:%S.000Z')
+                        if "TV Series" in media_type or "TV Mini Series" in media_type:
+                            media_type = "show"
+                        elif "TV Episode" in media_type:
+                            media_type = "episode"
+                        elif any(media in media_type for media in ["Movie", "TV Special", "TV Movie", "TV Short", "Video"]):
+                            media_type = "movie"
+                        else:
+                            media_type = "unknown"
+                        # Append to the list
+                        imdb_ratings.append({
+                            'Title': title,
+                            'Year': year,
+                            'Rating': int(rating),
+                            'IMDB_ID': imdb_id,
+                            'Date_Added': date_added,
+                            'Type': media_type
+                        })
+                        
         except FileNotFoundError:
             print(f"Error: {error_message}", exc_info=True)
             EL.logger.error(error_message, exc_info=True)
-            
+        
         # Delete csv files
         for file in os.listdir(directory):
             if file.endswith('.csv'):
                 os.remove(os.path.join(directory, file))
 
     except (NoSuchElementException, TimeoutException):
         # No IMDB Ratings
```

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/traktData.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer/verifyCredentials.py` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer/verifyCredentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
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
         "imdb_username": "empty",
```

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/PKG-INFO` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.9.0
+Version: 1.9.1
 Summary: A python script that syncs user watchlist, ratings and reviews for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imdbtraktsyncer-1.9.0/IMDBTraktSyncer.egg-info/SOURCES.txt` & `imdbtraktsyncer-1.9.1/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/LICENSE` & `imdbtraktsyncer-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/PKG-INFO` & `imdbtraktsyncer-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.9.0
+Version: 1.9.1
 Summary: A python script that syncs user watchlist, ratings and reviews for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imdbtraktsyncer-1.9.0/README.md` & `imdbtraktsyncer-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `imdbtraktsyncer-1.9.0/setup.py` & `imdbtraktsyncer-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.9.0'
+VERSION = '1.9.1'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and reviews for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

