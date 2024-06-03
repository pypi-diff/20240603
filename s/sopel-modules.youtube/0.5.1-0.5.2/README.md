# Comparing `tmp/sopel_modules.youtube-0.5.1.tar.gz` & `tmp/sopel_modules_youtube-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_modules.youtube-0.5.1.tar", last modified: Tue Nov  8 22:30:03 2022, max compression
+gzip compressed data, was "sopel_modules_youtube-0.5.2.tar", last modified: Mon Jun  3 05:17:32 2024, max compression
```

## Comparing `sopel_modules.youtube-0.5.1.tar` & `sopel_modules_youtube-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-08 22:30:03.660520 sopel_modules.youtube-0.5.1/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2021-11-22 18:23:03.000000 sopel_modules.youtube-0.5.1/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2021-11-22 18:23:03.000000 sopel_modules.youtube-0.5.1/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)     2688 2022-11-08 22:26:29.000000 sopel_modules.youtube-0.5.1/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     6341 2022-11-08 22:30:03.660020 sopel_modules.youtube-0.5.1/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)     2156 2022-01-11 20:49:05.000000 sopel_modules.youtube-0.5.1/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2021-11-22 18:23:03.000000 sopel_modules.youtube-0.5.1/dev-requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)      210 2022-11-08 22:24:15.000000 sopel_modules.youtube-0.5.1/requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       38 2022-11-08 22:30:03.661014 sopel_modules.youtube-0.5.1/setup.cfg
--rwxr-xr-x   0 dgw       (1000) dgw       (1000)     1428 2022-11-08 22:25:39.000000 sopel_modules.youtube-0.5.1/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-08 22:30:03.634022 sopel_modules.youtube-0.5.1/sopel_modules/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       57 2021-11-22 18:23:03.000000 sopel_modules.youtube-0.5.1/sopel_modules/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-08 22:30:03.656520 sopel_modules.youtube-0.5.1/sopel_modules/youtube/
--rw-r--r--   0 dgw       (1000) dgw       (1000)      385 2022-11-08 22:24:15.000000 sopel_modules.youtube-0.5.1/sopel_modules/youtube/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)    16003 2022-11-08 22:26:05.000000 sopel_modules.youtube-0.5.1/sopel_modules/youtube/youtube.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-08 22:30:03.654020 sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     6341 2022-11-08 22:30:03.000000 sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      492 2022-11-08 22:30:03.000000 sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2022-11-08 22:30:03.000000 sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       14 2022-11-08 22:30:03.000000 sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/namespace_packages.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)      152 2022-11-08 22:30:03.000000 sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2022-11-08 22:30:03.000000 sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/top_level.txt
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2022-11-08 22:30:03.658514 sopel_modules.youtube-0.5.1/tests/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2021-11-22 18:23:03.000000 sopel_modules.youtube-0.5.1/tests/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2021-11-22 18:23:03.000000 sopel_modules.youtube-0.5.1/tests/test_youtube.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-06-03 05:17:32.059860 sopel_modules_youtube-0.5.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1022 2024-06-03 04:53:04.000000 sopel_modules_youtube-0.5.2/COPYING
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      161 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2834 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/NEWS
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5744 2024-06-03 05:17:32.055860 sopel_modules_youtube-0.5.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2400 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/README.md
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/dev-requirements.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      210 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/requirements.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-06-03 05:17:32.059860 sopel_modules_youtube-0.5.2/setup.cfg
+-rwxr-xr-x   0 gitpod   (33333) gitpod   (33333)     1428 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-06-03 05:17:32.051860 sopel_modules_youtube-0.5.2/sopel_modules/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       57 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/sopel_modules/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-06-03 05:17:32.055860 sopel_modules_youtube-0.5.2/sopel_modules/youtube/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      385 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/sopel_modules/youtube/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    16003 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/sopel_modules/youtube/youtube.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-06-03 05:17:32.055860 sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5744 2024-06-03 05:17:31.000000 sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      492 2024-06-03 05:17:31.000000 sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-06-03 05:17:31.000000 sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       14 2024-06-03 05:17:31.000000 sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/namespace_packages.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      152 2024-06-03 05:17:31.000000 sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       20 2024-06-03 05:17:31.000000 sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-06-03 05:17:32.055860 sopel_modules_youtube-0.5.2/tests/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       15 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/tests/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      296 2024-06-03 05:17:19.000000 sopel_modules_youtube-0.5.2/tests/test_youtube.py
```

### Comparing `sopel_modules.youtube-0.5.1/COPYING` & `sopel_modules_youtube-0.5.2/COPYING`

 * *Files identical despite different names*

### Comparing `sopel_modules.youtube-0.5.1/NEWS` & `sopel_modules_youtube-0.5.2/NEWS`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Changes between 0.5.1 and 0.5.2
+===============================
+* Document `sopel_modules.youtube` end-of-life and transition to `sopel-youtube`
+
 Changes between 0.5.0 and 0.5.1
 ===============================
 * Fix hiding load-time import errors (#52)
 
 
 Changes between 0.4.3 and 0.5.0
 ===============================
```

### Comparing `sopel_modules.youtube-0.5.1/PKG-INFO` & `sopel_modules_youtube-0.5.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,159 +1,173 @@
 Metadata-Version: 2.1
 Name: sopel_modules.youtube
-Version: 0.5.1
+Version: 0.5.2
 Summary: YouTube plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-youtube
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
-Description: # sopel-youtube
-        
-        YouTube info plugin for Sopel
-        
-        ## Installing
-        
-        If possible, use `pip` to install this plugin. Below are example commands; you
-        might need to add `sudo` and/or call a different `pip` (e.g. `pip3`) depending
-        on your system and environment. Do not use `setup.py install`; Sopel won't be
-        able to load the plugin correctly.
-        
-        ### Published release
-        
-            pip install sopel_modules.youtube
-        
-        ### From source
-        
-            # Clone the repo, then run this in /path/to/sopel-youtube
-            pip install .
-        
-        ## Getting your API key
-        Go to the [Google Developers Console](https://console.developers.google.com/)
-        and create an application. When it's created, go to the APIs section, select
-        the YouTube Data API and enable it. Then go to the Credentials section,
-        select "Add credentials", pick "API key", and then "Server key". You can enter
-        a name for it and limit the IPs it can be used from, but you don't have to.
-        Copy the value it gives you into the prompt in the config wizard, or the
-        `api_key` value of the config in the `[youtube]` section.
-        
-        ## Config settings
-        `sopel-youtube` supports Sopel's interactive configuration wizard:
-        
-            sopel-plugins configure youtube
-        
-        The `api_key` option is self-explanatory (see above).
-        
-        If video "watch" links contain a playlist ID, the plugin will show the
-        playlist info as well as the video info by default. To disable this, set
-        `playlist_watch` to `False`.
-        
-        For videos, by default, only the video length, uploader (channel name), view
-        count, and upload date are shown. The included items, and the order in which
-        they appear, depend on the `info_items` setting, which is a list of keywords.
-        Unrecognized keywords are simply ignored. Supported `info_items` are:
-        
-        * `comments` (comment count)
-        * `date` (upload time/date)
-        * `length` (duration)
-        * `likes` (count)
-        * `uploader` (channel name)
-        * `views` (view count)
-        
-        ### Legacy `info_items`
-        Prior to YouTube's removal of public dislike counts, there were two vote-related
-        `info_items`: `votes` and `votes_color`. These keywords are deprecated as of
-        `sopel-youtube` 0.4.3. They will function as aliases to the new `likes` keyword
-        until they are removed entirely in v0.5 or thereabouts.
-        
-        
-        Changes between 0.5.0 and 0.5.1
-        ===============================
-        * Fix hiding load-time import errors (#52)
-        
-        
-        Changes between 0.4.3 and 0.5.0
-        ===============================
-        * Prep for Sopel 8:
-          * Require Sopel 7.1+; Sopel 7.0 is no longer supported
-          * Use `BooleanAttribute` setting type (#41)
-          * Switch from `sopel.module` to `sopel.plugin` (#42)
-        * Format time according to the channel's preference, w/fallback to bot setting (#50)
-        * Permit newer `google-api-python-client` library versions (#51)
-        
-        
-        Changes between 0.4.2 and 0.4.3
-        ===============================
-        * Remove handling of dislikes, which YouTube removed from its API (#45)
-        * Make live-stream handling more robust, again (#48)
-        * Replace `votes` and `votes_color` keywords in `info_items` with `votes` (#49)
-          * The old keywords will function as aliases until at least plugin version 0.5.0
-        
-        
-        Changes between 0.4.1 and 0.4.2
-        ===============================
-        * Improve error handling (#44)
-        
-        
-        Changes between 0.4.0 and 0.4.1
-        ===============================
-        * Handle "shorts" links (#36)
-        * Be more careful about auto-playlists (#38)
-        
-        
-        Changes between 0.3.2 and 0.4.0
-        ===============================
-        * Enhance live stream support (#28)
-        * Add playlist handling (#29, #33)
-        * Protect against bidirectional text (#31)
-        
-        
-        Changes between 0.3.1 and 0.3.2
-        ===============================
-        * Clean up some problematic imports (#25)
-        * Request only the necessary data fields from YouTube API (#27)
-        
-        
-        Changes between 0.3.0 and 0.3.1
-        ===============================
-        * Override handling of rare API errors reported to output the key (#23)
-        
-        
-        Changes between 0.2.1 and 0.3.0
-        ===============================
-        * Allow configuring what video details to include (#18)
-        * Remove outdated, ugly colors on "[YouTube]" output tag (#21)
-        * Minor cleanup (regex patterns, package metadata)
-        
-        
-        Changes between 0.2.0 and 0.2.1
-        ===============================
-        * Handle API sending wrongly formatted timestamps (#20)
-        
-        
-        Changes between 0.1.3 and 0.2.0
-        ===============================
-        * Update for Sopel 7 (#15)
-        
-        
-        Changes between 0.1.2 and 0.1.3
-        ===============================
-        * Add retry mechanic to API fetching (#11)
-        * Fix exception traceback sometimes thrown on reconnect (#14)
-        * Update ancient, deprecated usage of Sopel's memory API (#16)
-        
-        
-        Changes between 0.1.1 and 0.1.2
-        ===============================
-        * Fix error when video comments are disabled
-        * Improve duration parser
-        * Restrict google-api-python-client to compatible version range
-        * Fix version-number import issue during installation
-        
-        
-        Changes between 0.1.0 and 0.1.1
-        ===============================
-        * Output is colorized
-        * Fix configuration wizard
-        * pip installation works regardless of pip version
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: COPYING
+Requires-Dist: sopel<8,>=7.1
+Requires-Dist: google-api-python-client<1.8,>=1.5.5; python_version < "3.6"
+Requires-Dist: google-api-python-client<3,>=1.5.5; python_version >= "3.6"
+Requires-Dist: setuptools
+
+# sopel-youtube
+
+Legacy YouTube info plugin for Sopel
+
+## IMPORTANT
+
+**This version of the plugin is no longer maintained. When you are ready to
+upgrade to Sopel 8.0+, please uninstall `sopel-modules.youtube` and install
+[`sopel-youtube`](https://pypi.org/project/sopel-youtube/) instead.**
+
+## Installing
+
+If possible, use `pip` to install this plugin. Below are example commands; you
+might need to add `sudo` and/or call a different `pip` (e.g. `pip3`) depending
+on your system and environment. Do not use `setup.py install`; Sopel won't be
+able to load the plugin correctly.
+
+### Published release
+
+    pip install sopel_modules.youtube
+
+### From source
+
+    # Clone the repo, then run this in /path/to/sopel-youtube
+    pip install .
+
+## Getting your API key
+Go to the [Google Developers Console](https://console.developers.google.com/)
+and create an application. When it's created, go to the APIs section, select
+the YouTube Data API and enable it. Then go to the Credentials section,
+select "Add credentials", pick "API key", and then "Server key". You can enter
+a name for it and limit the IPs it can be used from, but you don't have to.
+Copy the value it gives you into the prompt in the config wizard, or the
+`api_key` value of the config in the `[youtube]` section.
+
+## Config settings
+`sopel-youtube` supports Sopel's interactive configuration wizard:
+
+    sopel-plugins configure youtube
+
+The `api_key` option is self-explanatory (see above).
+
+If video "watch" links contain a playlist ID, the plugin will show the
+playlist info as well as the video info by default. To disable this, set
+`playlist_watch` to `False`.
+
+For videos, by default, only the video length, uploader (channel name), view
+count, and upload date are shown. The included items, and the order in which
+they appear, depend on the `info_items` setting, which is a list of keywords.
+Unrecognized keywords are simply ignored. Supported `info_items` are:
+
+* `comments` (comment count)
+* `date` (upload time/date)
+* `length` (duration)
+* `likes` (count)
+* `uploader` (channel name)
+* `views` (view count)
+
+### Legacy `info_items`
+Prior to YouTube's removal of public dislike counts, there were two vote-related
+`info_items`: `votes` and `votes_color`. These keywords are deprecated as of
+`sopel-youtube` 0.4.3. They will function as aliases to the new `likes` keyword
+until they are removed entirely in v0.5 or thereabouts.
+
+
+Changes between 0.5.1 and 0.5.2
+===============================
+* Document `sopel_modules.youtube` end-of-life and transition to `sopel-youtube`
+
+Changes between 0.5.0 and 0.5.1
+===============================
+* Fix hiding load-time import errors (#52)
+
+
+Changes between 0.4.3 and 0.5.0
+===============================
+* Prep for Sopel 8:
+  * Require Sopel 7.1+; Sopel 7.0 is no longer supported
+  * Use `BooleanAttribute` setting type (#41)
+  * Switch from `sopel.module` to `sopel.plugin` (#42)
+* Format time according to the channel's preference, w/fallback to bot setting (#50)
+* Permit newer `google-api-python-client` library versions (#51)
+
+
+Changes between 0.4.2 and 0.4.3
+===============================
+* Remove handling of dislikes, which YouTube removed from its API (#45)
+* Make live-stream handling more robust, again (#48)
+* Replace `votes` and `votes_color` keywords in `info_items` with `votes` (#49)
+  * The old keywords will function as aliases until at least plugin version 0.5.0
+
+
+Changes between 0.4.1 and 0.4.2
+===============================
+* Improve error handling (#44)
+
+
+Changes between 0.4.0 and 0.4.1
+===============================
+* Handle "shorts" links (#36)
+* Be more careful about auto-playlists (#38)
+
+
+Changes between 0.3.2 and 0.4.0
+===============================
+* Enhance live stream support (#28)
+* Add playlist handling (#29, #33)
+* Protect against bidirectional text (#31)
+
+
+Changes between 0.3.1 and 0.3.2
+===============================
+* Clean up some problematic imports (#25)
+* Request only the necessary data fields from YouTube API (#27)
+
+
+Changes between 0.3.0 and 0.3.1
+===============================
+* Override handling of rare API errors reported to output the key (#23)
+
+
+Changes between 0.2.1 and 0.3.0
+===============================
+* Allow configuring what video details to include (#18)
+* Remove outdated, ugly colors on "[YouTube]" output tag (#21)
+* Minor cleanup (regex patterns, package metadata)
+
+
+Changes between 0.2.0 and 0.2.1
+===============================
+* Handle API sending wrongly formatted timestamps (#20)
+
+
+Changes between 0.1.3 and 0.2.0
+===============================
+* Update for Sopel 7 (#15)
+
+
+Changes between 0.1.2 and 0.1.3
+===============================
+* Add retry mechanic to API fetching (#11)
+* Fix exception traceback sometimes thrown on reconnect (#14)
+* Update ancient, deprecated usage of Sopel's memory API (#16)
+
+
+Changes between 0.1.1 and 0.1.2
+===============================
+* Fix error when video comments are disabled
+* Improve duration parser
+* Restrict google-api-python-client to compatible version range
+* Fix version-number import issue during installation
+
+
+Changes between 0.1.0 and 0.1.1
+===============================
+* Output is colorized
+* Fix configuration wizard
+* pip installation works regardless of pip version
```

### Comparing `sopel_modules.youtube-0.5.1/README.md` & `sopel_modules_youtube-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # sopel-youtube
 
-YouTube info plugin for Sopel
+Legacy YouTube info plugin for Sopel
+
+## IMPORTANT
+
+**This version of the plugin is no longer maintained. When you are ready to
+upgrade to Sopel 8.0+, please uninstall `sopel-modules.youtube` and install
+[`sopel-youtube`](https://pypi.org/project/sopel-youtube/) instead.**
 
 ## Installing
 
 If possible, use `pip` to install this plugin. Below are example commands; you
 might need to add `sudo` and/or call a different `pip` (e.g. `pip3`) depending
 on your system and environment. Do not use `setup.py install`; Sopel won't be
 able to load the plugin correctly.
```

### Comparing `sopel_modules.youtube-0.5.1/setup.py` & `sopel_modules_youtube-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 with open('dev-requirements.txt') as dev_requirements_file:
     dev_requirements = [req for req in dev_requirements_file.readlines()]
 
 
 setup(
     name='sopel_modules.youtube',
-    version='0.5.1',
+    version='0.5.2',
     description='YouTube plugin for Sopel',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='dgw',
     author_email='dgw@technobabbl.es',
     url='https://github.com/sopel-irc/sopel-youtube',
     packages=find_packages('.'),
```

### Comparing `sopel_modules.youtube-0.5.1/sopel_modules/youtube/youtube.py` & `sopel_modules_youtube-0.5.2/sopel_modules/youtube/youtube.py`

 * *Files identical despite different names*

### Comparing `sopel_modules.youtube-0.5.1/sopel_modules.youtube.egg-info/PKG-INFO` & `sopel_modules_youtube-0.5.2/sopel_modules.youtube.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,159 +1,173 @@
 Metadata-Version: 2.1
-Name: sopel-modules.youtube
-Version: 0.5.1
+Name: sopel_modules.youtube
+Version: 0.5.2
 Summary: YouTube plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-youtube
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
-Description: # sopel-youtube
-        
-        YouTube info plugin for Sopel
-        
-        ## Installing
-        
-        If possible, use `pip` to install this plugin. Below are example commands; you
-        might need to add `sudo` and/or call a different `pip` (e.g. `pip3`) depending
-        on your system and environment. Do not use `setup.py install`; Sopel won't be
-        able to load the plugin correctly.
-        
-        ### Published release
-        
-            pip install sopel_modules.youtube
-        
-        ### From source
-        
-            # Clone the repo, then run this in /path/to/sopel-youtube
-            pip install .
-        
-        ## Getting your API key
-        Go to the [Google Developers Console](https://console.developers.google.com/)
-        and create an application. When it's created, go to the APIs section, select
-        the YouTube Data API and enable it. Then go to the Credentials section,
-        select "Add credentials", pick "API key", and then "Server key". You can enter
-        a name for it and limit the IPs it can be used from, but you don't have to.
-        Copy the value it gives you into the prompt in the config wizard, or the
-        `api_key` value of the config in the `[youtube]` section.
-        
-        ## Config settings
-        `sopel-youtube` supports Sopel's interactive configuration wizard:
-        
-            sopel-plugins configure youtube
-        
-        The `api_key` option is self-explanatory (see above).
-        
-        If video "watch" links contain a playlist ID, the plugin will show the
-        playlist info as well as the video info by default. To disable this, set
-        `playlist_watch` to `False`.
-        
-        For videos, by default, only the video length, uploader (channel name), view
-        count, and upload date are shown. The included items, and the order in which
-        they appear, depend on the `info_items` setting, which is a list of keywords.
-        Unrecognized keywords are simply ignored. Supported `info_items` are:
-        
-        * `comments` (comment count)
-        * `date` (upload time/date)
-        * `length` (duration)
-        * `likes` (count)
-        * `uploader` (channel name)
-        * `views` (view count)
-        
-        ### Legacy `info_items`
-        Prior to YouTube's removal of public dislike counts, there were two vote-related
-        `info_items`: `votes` and `votes_color`. These keywords are deprecated as of
-        `sopel-youtube` 0.4.3. They will function as aliases to the new `likes` keyword
-        until they are removed entirely in v0.5 or thereabouts.
-        
-        
-        Changes between 0.5.0 and 0.5.1
-        ===============================
-        * Fix hiding load-time import errors (#52)
-        
-        
-        Changes between 0.4.3 and 0.5.0
-        ===============================
-        * Prep for Sopel 8:
-          * Require Sopel 7.1+; Sopel 7.0 is no longer supported
-          * Use `BooleanAttribute` setting type (#41)
-          * Switch from `sopel.module` to `sopel.plugin` (#42)
-        * Format time according to the channel's preference, w/fallback to bot setting (#50)
-        * Permit newer `google-api-python-client` library versions (#51)
-        
-        
-        Changes between 0.4.2 and 0.4.3
-        ===============================
-        * Remove handling of dislikes, which YouTube removed from its API (#45)
-        * Make live-stream handling more robust, again (#48)
-        * Replace `votes` and `votes_color` keywords in `info_items` with `votes` (#49)
-          * The old keywords will function as aliases until at least plugin version 0.5.0
-        
-        
-        Changes between 0.4.1 and 0.4.2
-        ===============================
-        * Improve error handling (#44)
-        
-        
-        Changes between 0.4.0 and 0.4.1
-        ===============================
-        * Handle "shorts" links (#36)
-        * Be more careful about auto-playlists (#38)
-        
-        
-        Changes between 0.3.2 and 0.4.0
-        ===============================
-        * Enhance live stream support (#28)
-        * Add playlist handling (#29, #33)
-        * Protect against bidirectional text (#31)
-        
-        
-        Changes between 0.3.1 and 0.3.2
-        ===============================
-        * Clean up some problematic imports (#25)
-        * Request only the necessary data fields from YouTube API (#27)
-        
-        
-        Changes between 0.3.0 and 0.3.1
-        ===============================
-        * Override handling of rare API errors reported to output the key (#23)
-        
-        
-        Changes between 0.2.1 and 0.3.0
-        ===============================
-        * Allow configuring what video details to include (#18)
-        * Remove outdated, ugly colors on "[YouTube]" output tag (#21)
-        * Minor cleanup (regex patterns, package metadata)
-        
-        
-        Changes between 0.2.0 and 0.2.1
-        ===============================
-        * Handle API sending wrongly formatted timestamps (#20)
-        
-        
-        Changes between 0.1.3 and 0.2.0
-        ===============================
-        * Update for Sopel 7 (#15)
-        
-        
-        Changes between 0.1.2 and 0.1.3
-        ===============================
-        * Add retry mechanic to API fetching (#11)
-        * Fix exception traceback sometimes thrown on reconnect (#14)
-        * Update ancient, deprecated usage of Sopel's memory API (#16)
-        
-        
-        Changes between 0.1.1 and 0.1.2
-        ===============================
-        * Fix error when video comments are disabled
-        * Improve duration parser
-        * Restrict google-api-python-client to compatible version range
-        * Fix version-number import issue during installation
-        
-        
-        Changes between 0.1.0 and 0.1.1
-        ===============================
-        * Output is colorized
-        * Fix configuration wizard
-        * pip installation works regardless of pip version
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: COPYING
+Requires-Dist: sopel<8,>=7.1
+Requires-Dist: google-api-python-client<1.8,>=1.5.5; python_version < "3.6"
+Requires-Dist: google-api-python-client<3,>=1.5.5; python_version >= "3.6"
+Requires-Dist: setuptools
+
+# sopel-youtube
+
+Legacy YouTube info plugin for Sopel
+
+## IMPORTANT
+
+**This version of the plugin is no longer maintained. When you are ready to
+upgrade to Sopel 8.0+, please uninstall `sopel-modules.youtube` and install
+[`sopel-youtube`](https://pypi.org/project/sopel-youtube/) instead.**
+
+## Installing
+
+If possible, use `pip` to install this plugin. Below are example commands; you
+might need to add `sudo` and/or call a different `pip` (e.g. `pip3`) depending
+on your system and environment. Do not use `setup.py install`; Sopel won't be
+able to load the plugin correctly.
+
+### Published release
+
+    pip install sopel_modules.youtube
+
+### From source
+
+    # Clone the repo, then run this in /path/to/sopel-youtube
+    pip install .
+
+## Getting your API key
+Go to the [Google Developers Console](https://console.developers.google.com/)
+and create an application. When it's created, go to the APIs section, select
+the YouTube Data API and enable it. Then go to the Credentials section,
+select "Add credentials", pick "API key", and then "Server key". You can enter
+a name for it and limit the IPs it can be used from, but you don't have to.
+Copy the value it gives you into the prompt in the config wizard, or the
+`api_key` value of the config in the `[youtube]` section.
+
+## Config settings
+`sopel-youtube` supports Sopel's interactive configuration wizard:
+
+    sopel-plugins configure youtube
+
+The `api_key` option is self-explanatory (see above).
+
+If video "watch" links contain a playlist ID, the plugin will show the
+playlist info as well as the video info by default. To disable this, set
+`playlist_watch` to `False`.
+
+For videos, by default, only the video length, uploader (channel name), view
+count, and upload date are shown. The included items, and the order in which
+they appear, depend on the `info_items` setting, which is a list of keywords.
+Unrecognized keywords are simply ignored. Supported `info_items` are:
+
+* `comments` (comment count)
+* `date` (upload time/date)
+* `length` (duration)
+* `likes` (count)
+* `uploader` (channel name)
+* `views` (view count)
+
+### Legacy `info_items`
+Prior to YouTube's removal of public dislike counts, there were two vote-related
+`info_items`: `votes` and `votes_color`. These keywords are deprecated as of
+`sopel-youtube` 0.4.3. They will function as aliases to the new `likes` keyword
+until they are removed entirely in v0.5 or thereabouts.
+
+
+Changes between 0.5.1 and 0.5.2
+===============================
+* Document `sopel_modules.youtube` end-of-life and transition to `sopel-youtube`
+
+Changes between 0.5.0 and 0.5.1
+===============================
+* Fix hiding load-time import errors (#52)
+
+
+Changes between 0.4.3 and 0.5.0
+===============================
+* Prep for Sopel 8:
+  * Require Sopel 7.1+; Sopel 7.0 is no longer supported
+  * Use `BooleanAttribute` setting type (#41)
+  * Switch from `sopel.module` to `sopel.plugin` (#42)
+* Format time according to the channel's preference, w/fallback to bot setting (#50)
+* Permit newer `google-api-python-client` library versions (#51)
+
+
+Changes between 0.4.2 and 0.4.3
+===============================
+* Remove handling of dislikes, which YouTube removed from its API (#45)
+* Make live-stream handling more robust, again (#48)
+* Replace `votes` and `votes_color` keywords in `info_items` with `votes` (#49)
+  * The old keywords will function as aliases until at least plugin version 0.5.0
+
+
+Changes between 0.4.1 and 0.4.2
+===============================
+* Improve error handling (#44)
+
+
+Changes between 0.4.0 and 0.4.1
+===============================
+* Handle "shorts" links (#36)
+* Be more careful about auto-playlists (#38)
+
+
+Changes between 0.3.2 and 0.4.0
+===============================
+* Enhance live stream support (#28)
+* Add playlist handling (#29, #33)
+* Protect against bidirectional text (#31)
+
+
+Changes between 0.3.1 and 0.3.2
+===============================
+* Clean up some problematic imports (#25)
+* Request only the necessary data fields from YouTube API (#27)
+
+
+Changes between 0.3.0 and 0.3.1
+===============================
+* Override handling of rare API errors reported to output the key (#23)
+
+
+Changes between 0.2.1 and 0.3.0
+===============================
+* Allow configuring what video details to include (#18)
+* Remove outdated, ugly colors on "[YouTube]" output tag (#21)
+* Minor cleanup (regex patterns, package metadata)
+
+
+Changes between 0.2.0 and 0.2.1
+===============================
+* Handle API sending wrongly formatted timestamps (#20)
+
+
+Changes between 0.1.3 and 0.2.0
+===============================
+* Update for Sopel 7 (#15)
+
+
+Changes between 0.1.2 and 0.1.3
+===============================
+* Add retry mechanic to API fetching (#11)
+* Fix exception traceback sometimes thrown on reconnect (#14)
+* Update ancient, deprecated usage of Sopel's memory API (#16)
+
+
+Changes between 0.1.1 and 0.1.2
+===============================
+* Fix error when video comments are disabled
+* Improve duration parser
+* Restrict google-api-python-client to compatible version range
+* Fix version-number import issue during installation
+
+
+Changes between 0.1.0 and 0.1.1
+===============================
+* Output is colorized
+* Fix configuration wizard
+* pip installation works regardless of pip version
```

