# Comparing `tmp/knuckles-0.2.0.tar.gz` & `tmp/knuckles-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knuckles-0.2.0.tar", last modified: Sun Jun  2 21:51:41 2024, max compression
+gzip compressed data, was "knuckles-1.0.0.tar", last modified: Sun Jun  2 21:55:06 2024, max compression
```

## Comparing `knuckles-0.2.0.tar` & `knuckles-1.0.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.670433 knuckles-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 21:51:29.000000 knuckles-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-02 21:51:41.666433 knuckles-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-02 21:51:29.000000 knuckles-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-02 21:51:29.000000 knuckles-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 21:51:41.670433 knuckles-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.658433 knuckles-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.662433 knuckles-0.2.0/src/knuckles/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_browsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_internet_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_jukebox.py
--rw-r--r--   0 runner    (1001) docker     (127)    25877 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_media_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_media_library_scanning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_media_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_podcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_sharing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_subsonic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/_user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.666433 knuckles-0.2.0/src/knuckles/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_album.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_artist_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_contributor.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_cover_art.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_genre.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_internet_radio_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_jukebox.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_lyrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_music_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_music_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_now_playing_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_play_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_podcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_replay_gain.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_scan_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_share.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_song.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_starred_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/models/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:29.000000 knuckles-0.2.0/src/knuckles/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:51:41.666433 knuckles-0.2.0/src/knuckles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 21:51:41.000000 knuckles-0.2.0/src/knuckles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:55:06.486251 knuckles-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-02 21:54:53.000000 knuckles-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-02 21:55:06.486251 knuckles-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-02 21:54:53.000000 knuckles-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-02 21:54:53.000000 knuckles-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 21:55:06.486251 knuckles-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:55:06.474251 knuckles-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:55:06.478251 knuckles-1.0.0/src/knuckles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_browsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_internet_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_jukebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25877 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_media_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_media_library_scanning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_media_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_podcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_subsonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/_user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:55:06.486251 knuckles-1.0.0/src/knuckles/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_artist_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_contributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_cover_art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_genre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_internet_radio_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_jukebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_lyrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_music_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_music_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_now_playing_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_play_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_podcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_replay_gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_scan_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_song.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_starred_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/models/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:54:53.000000 knuckles-1.0.0/src/knuckles/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:55:06.486251 knuckles-1.0.0/src/knuckles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-02 21:55:06.000000 knuckles-1.0.0/src/knuckles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-02 21:55:06.000000 knuckles-1.0.0/src/knuckles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 21:55:06.000000 knuckles-1.0.0/src/knuckles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-02 21:55:06.000000 knuckles-1.0.0/src/knuckles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 21:55:06.000000 knuckles-1.0.0/src/knuckles.egg-info/top_level.txt
```

### Comparing `knuckles-0.2.0/LICENSE.txt` & `knuckles-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/PKG-INFO` & `knuckles-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knuckles
-Version: 0.2.0
+Version: 1.0.0
 Summary: A Subsonic/OpenSubsonic API wrapper for Python.
 Author-email: "Jorge \"Kutu\" Dobón Blanco" <code@dobon.dev>
 Keywords: api-wrapper,api,wrapper,library,subsonic,opensubsonic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `knuckles-0.2.0/README.md` & `knuckles-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/pyproject.toml` & `knuckles-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 requires-python = ">=3.11.0"
 
 dependencies = [
     "requests>=2.32.3",
     "python-dateutil>=2.8.2"
 ]
 
-version = "0.2.0"
+version = "1.0.0"
 readme = "README.md"
 
 authors = [
   {name = 'Jorge "Kutu" Dobón Blanco', email="code@dobon.dev"}
 ]
 
 keywords = [
```

### Comparing `knuckles-0.2.0/src/knuckles/__init__.py` & `knuckles-1.0.0/src/knuckles/__init__.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_api.py` & `knuckles-1.0.0/src/knuckles/_api.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_bookmarks.py` & `knuckles-1.0.0/src/knuckles/_bookmarks.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_browsing.py` & `knuckles-1.0.0/src/knuckles/_browsing.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_chat.py` & `knuckles-1.0.0/src/knuckles/_chat.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_internet_radio.py` & `knuckles-1.0.0/src/knuckles/_internet_radio.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_jukebox.py` & `knuckles-1.0.0/src/knuckles/_jukebox.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_lists.py` & `knuckles-1.0.0/src/knuckles/_lists.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_media_annotation.py` & `knuckles-1.0.0/src/knuckles/_media_annotation.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_media_library_scanning.py` & `knuckles-1.0.0/src/knuckles/_media_library_scanning.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_media_retrieval.py` & `knuckles-1.0.0/src/knuckles/_media_retrieval.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_playlists.py` & `knuckles-1.0.0/src/knuckles/_playlists.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_podcast.py` & `knuckles-1.0.0/src/knuckles/_podcast.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_searching.py` & `knuckles-1.0.0/src/knuckles/_searching.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_sharing.py` & `knuckles-1.0.0/src/knuckles/_sharing.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_subsonic.py` & `knuckles-1.0.0/src/knuckles/_subsonic.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_system.py` & `knuckles-1.0.0/src/knuckles/_system.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/_user_management.py` & `knuckles-1.0.0/src/knuckles/_user_management.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/exceptions.py` & `knuckles-1.0.0/src/knuckles/exceptions.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_album.py` & `knuckles-1.0.0/src/knuckles/models/_album.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_artist.py` & `knuckles-1.0.0/src/knuckles/models/_artist.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_artist_index.py` & `knuckles-1.0.0/src/knuckles/models/_artist_index.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_bookmark.py` & `knuckles-1.0.0/src/knuckles/models/_bookmark.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_chat_message.py` & `knuckles-1.0.0/src/knuckles/models/_chat_message.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_contributor.py` & `knuckles-1.0.0/src/knuckles/models/_contributor.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_genre.py` & `knuckles-1.0.0/src/knuckles/models/_genre.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_internet_radio_station.py` & `knuckles-1.0.0/src/knuckles/models/_internet_radio_station.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_jukebox.py` & `knuckles-1.0.0/src/knuckles/models/_jukebox.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_lyrics.py` & `knuckles-1.0.0/src/knuckles/models/_lyrics.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_music_directory.py` & `knuckles-1.0.0/src/knuckles/models/_music_directory.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_music_folder.py` & `knuckles-1.0.0/src/knuckles/models/_music_folder.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_now_playing_entry.py` & `knuckles-1.0.0/src/knuckles/models/_now_playing_entry.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_play_queue.py` & `knuckles-1.0.0/src/knuckles/models/_play_queue.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_playlist.py` & `knuckles-1.0.0/src/knuckles/models/_playlist.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_podcast.py` & `knuckles-1.0.0/src/knuckles/models/_podcast.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_replay_gain.py` & `knuckles-1.0.0/src/knuckles/models/_replay_gain.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_scan_status.py` & `knuckles-1.0.0/src/knuckles/models/_scan_status.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_search_result.py` & `knuckles-1.0.0/src/knuckles/models/_search_result.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_share.py` & `knuckles-1.0.0/src/knuckles/models/_share.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_song.py` & `knuckles-1.0.0/src/knuckles/models/_song.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_starred_content.py` & `knuckles-1.0.0/src/knuckles/models/_starred_content.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_system.py` & `knuckles-1.0.0/src/knuckles/models/_system.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_user.py` & `knuckles-1.0.0/src/knuckles/models/_user.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles/models/_video.py` & `knuckles-1.0.0/src/knuckles/models/_video.py`

 * *Files identical despite different names*

### Comparing `knuckles-0.2.0/src/knuckles.egg-info/PKG-INFO` & `knuckles-1.0.0/src/knuckles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knuckles
-Version: 0.2.0
+Version: 1.0.0
 Summary: A Subsonic/OpenSubsonic API wrapper for Python.
 Author-email: "Jorge \"Kutu\" Dobón Blanco" <code@dobon.dev>
 Keywords: api-wrapper,api,wrapper,library,subsonic,opensubsonic
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `knuckles-0.2.0/src/knuckles.egg-info/SOURCES.txt` & `knuckles-1.0.0/src/knuckles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

