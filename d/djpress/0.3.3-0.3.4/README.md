# Comparing `tmp/djpress-0.3.3.tar.gz` & `tmp/djpress-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpress-0.3.3.tar", last modified: Tue May 28 08:16:30 2024, max compression
+gzip compressed data, was "djpress-0.3.4.tar", last modified: Mon Jun  3 11:04:13 2024, max compression
```

## Comparing `djpress-0.3.3.tar` & `djpress-0.3.4.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.514467 djpress-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 08:16:23.000000 djpress-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 08:16:23.000000 djpress-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-28 08:16:30.514467 djpress-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-28 08:16:23.000000 djpress-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/feeds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/migrations/0002_rename_content_type_post_post_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/models/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/models/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/models/post.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/static/djpress/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/static/djpress/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/static/djpress/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/static/djpress/css/style.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.506466 djpress-0.3.3/djpress/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/templates/djpress/
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templates/djpress/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/djpress/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templatetags/djpress_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/templatetags/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-28 08:16:23.000000 djpress-0.3.3/djpress/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.514467 djpress-0.3.3/djpress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 08:16:30.000000 djpress-0.3.3/djpress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.510466 djpress-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 08:16:23.000000 djpress-0.3.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-28 08:16:23.000000 djpress-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:16:30.514467 djpress-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 08:16:23.000000 djpress-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:16:30.514467 djpress-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_category_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_djpress_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_post_authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_published_posts_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-28 08:16:23.000000 djpress-0.3.3/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.242993 djpress-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-03 11:04:07.000000 djpress-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-03 11:04:07.000000 djpress-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-06-03 11:04:13.242993 djpress-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-03 11:04:07.000000 djpress-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.238993 djpress-0.3.4/djpress/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/feeds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.238993 djpress-0.3.4/djpress/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/migrations/0002_rename_content_type_post_post_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.238993 djpress-0.3.4/djpress/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/models/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/models/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.234993 djpress-0.3.4/djpress/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.234993 djpress-0.3.4/djpress/static/djpress/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.238993 djpress-0.3.4/djpress/static/djpress/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/static/djpress/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/static/djpress/css/style.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.234993 djpress-0.3.4/djpress/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.238993 djpress-0.3.4/djpress/templates/djpress/
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/templates/djpress/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.238993 djpress-0.3.4/djpress/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/templatetags/djpress_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/templatetags/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-06-03 11:04:07.000000 djpress-0.3.4/djpress/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.242993 djpress-0.3.4/djpress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-06-03 11:04:13.000000 djpress-0.3.4/djpress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-03 11:04:13.000000 djpress-0.3.4/djpress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:04:13.000000 djpress-0.3.4/djpress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-03 11:04:13.000000 djpress-0.3.4/djpress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-03 11:04:13.000000 djpress-0.3.4/djpress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.238993 djpress-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 11:04:07.000000 djpress-0.3.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-03 11:04:07.000000 djpress-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 11:04:13.242993 djpress-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-03 11:04:07.000000 djpress-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:04:13.242993 djpress-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_cache_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_cache_published_posts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_conf_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_models_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15395 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_models_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22556 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_templatetags_djpress_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-06-03 11:04:07.000000 djpress-0.3.4/tests/test_views.py
```

### Comparing `djpress-0.3.3/LICENSE` & `djpress-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/PKG-INFO` & `djpress-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.3.3
+Version: 0.3.4
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,15 @@
 Keywords: django,blog,cms,markdown,wordpress
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `djpress-0.3.3/README.md` & `djpress-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/app_settings.py` & `djpress-0.3.4/djpress/app_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # DJPress settings
 TRUNCATE_TAG = "<!--more-->"
 CACHE_CATEGORIES: bool = True
 CACHE_RECENT_PUBLISHED_POSTS: bool = False
 RECENT_PUBLISHED_POSTS_COUNT: int = 20
 MARKDOWN_EXTENSIONS: list = ["fenced_code", "codehilite", "tables"]
 BLOG_TITLE: str = "My DJ Press Blog"
+BLOG_DESCRIPTION: str = ""
 
 # DJPress URL settings
 CATEGORY_PATH_ENABLED: bool = True
 CATEGORY_PATH: str = "category"
 AUTHOR_PATH_ENABLED: bool = True
 AUTHOR_PATH: str = "author"
 ARCHIVES_PATH_ENABLED: bool = True
```

### Comparing `djpress-0.3.3/djpress/feeds.py` & `djpress-0.3.4/djpress/feeds.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """RSS feed for blog posts."""
 
 from typing import TYPE_CHECKING
 
 from django.contrib.syndication.views import Feed
 from django.urls import reverse
 
+from djpress.conf import settings
 from djpress.models import Post
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from django.db import models
 
 
 class PostFeed(Feed):
     """RSS feed for blog posts."""
 
-    title = "stuartm.nz"
-    link = "/rss"
-    description = "stuartm.nz updates"
+    title = settings.BLOG_TITLE
+    link = f"/{settings.RSS_PATH}/"
+    description = settings.BLOG_DESCRIPTION
 
     def items(self: "PostFeed") -> "models.QuerySet":
         """Return the most recent posts."""
         return Post.post_objects.get_recent_published_posts()
 
     def item_title(self: "PostFeed", item: Post) -> str:
         """Return the title of the post."""
```

### Comparing `djpress-0.3.3/djpress/migrations/0001_initial.py` & `djpress-0.3.4/djpress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/models/category.py` & `djpress-0.3.4/djpress/models/category.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/models/post.py` & `djpress-0.3.4/djpress/models/post.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,32 +63,49 @@
                 self.get_queryset()
                 .filter(
                     status="published",
                 )
                 .prefetch_related("categories", "author")
             )
 
-            future_posts = queryset.filter(date__gt=timezone.now())
-            if future_posts.exists():
-                future_post = future_posts[0]
-                timeout = (future_post.date - timezone.now()).total_seconds()
-            else:
-                timeout = None
+            timeout = self._get_cache_timeout(queryset)
 
             queryset = queryset.filter(date__lte=timezone.now())[
                 : settings.RECENT_PUBLISHED_POSTS_COUNT
             ]
             cache.set(
                 PUBLISHED_POSTS_CACHE_KEY,
                 queryset,
                 timeout=timeout,
             )
 
         return queryset
 
+    def _get_cache_timeout(
+        self: "PostsManager",
+        queryset: models.QuerySet,
+    ) -> int | None:
+        """Return the timeout for the cache.
+
+        If there are any future posts, we calculate the seconds until that post.
+
+        Args:
+            queryset: The queryset of published posts.
+
+        Returns:
+            int | None: The number of seconds until the next future post, or None if
+            there are no future posts.
+        """
+        future_posts = queryset.filter(date__gt=timezone.now())
+        if future_posts.exists():
+            future_post = future_posts[0]
+            return (future_post.date - timezone.now()).total_seconds()
+
+        return None
+
     def get_published_post_by_slug(
         self: "PostsManager",
         slug: str,
     ) -> "Post":
         """Return a single published post.
 
         Must have a date less than or equal to the current date/time based on its slug.
```

### Comparing `djpress-0.3.3/djpress/static/djpress/css/style.css` & `djpress-0.3.4/djpress/static/djpress/css/style.css`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/static/djpress/css/style.min.css` & `djpress-0.3.4/djpress/static/djpress/css/style.min.css`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/templates/djpress/index.html` & `djpress-0.3.4/djpress/templates/djpress/index.html`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/templatetags/djpress_tags.py` & `djpress-0.3.4/djpress/templatetags/djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/templatetags/helpers.py` & `djpress-0.3.4/djpress/templatetags/helpers.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/urls.py` & `djpress-0.3.4/djpress/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         path(
             f"{settings.CATEGORY_PATH}/<slug:slug>/",
             category_posts,
             name="category_posts",
         ),
     ]
 
-if settings.AUTHOR_PATH_ENABLED and settings.AUTHOR_PATH:
+if settings.AUTHOR_PATH_ENABLED:
     urlpatterns += [
         path(
             f"{settings.AUTHOR_PATH}/<str:author>/",
             author_posts,
             name="author_posts",
         ),
     ]
```

### Comparing `djpress-0.3.3/djpress/utils.py` & `djpress-0.3.4/djpress/utils.py`

 * *Files identical despite different names*

### Comparing `djpress-0.3.3/djpress/views.py` & `djpress-0.3.4/djpress/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """djpress views file."""
 
 import logging
 
 from django.contrib.auth.models import User
-from django.http import Http404, HttpRequest, HttpResponse
+from django.http import Http404, HttpRequest, HttpResponse, HttpResponseBadRequest
 from django.shortcuts import render
 from django.utils.timezone import datetime
 
 from djpress.models import Category, Post
 
 logger = logging.getLogger(__name__)
 
@@ -36,19 +36,19 @@
     Args:
         request (HttpRequest): The request object.
         year (str): The year.
         month (str): The month.
         day (str): The day.
     """
     try:
-        test_dates(year, month, day)
+        validate_date(year, month, day)
 
-    except ValueError as exc:
+    except ValueError:
         msg = "Invalid date"
-        raise Http404(msg) from exc
+        return HttpResponseBadRequest(msg)
 
     posts = Post.post_objects._get_published_posts()  # noqa: SLF001
 
     # Django converts strings to integers when they are passed to the filter
     if day:
         logger.debug(f"{year}/{month}/{day}")
         posts = posts.filter(
@@ -68,29 +68,44 @@
     return render(
         request,
         "djpress/index.html",
         {"posts": posts},
     )
 
 
-def test_dates(year: str, month: str | None, day: str | None) -> None:
+def validate_date(year: str, month: str, day: str) -> None:
     """Test the date values.
 
     Convert the date values to integers and test if they are valid dates.
 
+    The regex that gets the date values checks for the following:
+    - year: four digits
+    - month: two digits
+    - day: two digits
+
     Args:
         year (str): The year.
         month (str | None): The month.
         day (str | None): The day.
+
+    Raises:
+        ValueError: If the date is invalid.
+
+    Returns:
+        None
     """
-    try:
-        int_year = int(year)
-        int_month = int(month) if month else None
-        int_day = int(day) if day else None
+    int_year: int = int(year)
+    int_month: int | None = int(month) if month else None
+    int_day: int | None = int(day) if day else None
 
+    if int_month == 0 or int_day == 0:
+        msg = "Invalid date"
+        raise ValueError(msg)
+
+    try:
         if int_month and int_day:
             datetime(int_year, int_month, int_day)
 
         elif int_month:
             datetime(int_year, int_month, 1)
 
         else:
```

### Comparing `djpress-0.3.3/djpress.egg-info/PKG-INFO` & `djpress-0.3.4/djpress.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.3.3
+Version: 0.3.4
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,15 @@
 Keywords: django,blog,cms,markdown,wordpress
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `djpress-0.3.3/djpress.egg-info/SOURCES.txt` & `djpress-0.3.4/djpress.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 djpress/static/djpress/css/style.css
 djpress/static/djpress/css/style.min.css
 djpress/templates/djpress/index.html
 djpress/templatetags/__init__.py
 djpress/templatetags/djpress_tags.py
 djpress/templatetags/helpers.py
 docs/index.md
-tests/test_category_cache.py
-tests/test_djpress_tags.py
+tests/test_cache_category.py
+tests/test_cache_published_posts.py
+tests/test_conf_urls.py
 tests/test_feeds.py
-tests/test_models.py
-tests/test_post_authors.py
-tests/test_published_posts_cache.py
+tests/test_models_category.py
+tests/test_models_post.py
+tests/test_templatetags_djpress_tags.py
+tests/test_utils.py
 tests/test_views.py
```

### Comparing `djpress-0.3.3/pyproject.toml` & `djpress-0.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djpress"
-version = "0.3.3"
+version = "0.3.4"
 authors = [{ name = "Stuart Maxwell", email = "stuart@amanzi.nz" }]
 description = "A blog application for Django sites, inspired by classic WordPress."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["django", "markdown", "pygments"]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Environment :: Web Environment",
   "Framework :: Django",
+  "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
   "Intended Audience :: Developers",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
```

### Comparing `djpress-0.3.3/tests/test_feeds.py` & `djpress-0.3.4/tests/test_feeds.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,63 +3,69 @@
 from django.urls import reverse
 
 from djpress.conf import settings
 from djpress.feeds import PostFeed
 from djpress.models import Post
 
 
+@pytest.fixture
+def user():
+    return User.objects.create_user(username="testuser", password="testpass")
+
+
 @pytest.mark.django_db
-def test_latest_posts_feed(client):
-    user = User.objects.create_user(username="testuser", password="testpass")
+def test_latest_posts_feed(client, user):
     Post.post_objects.create(
         title="Post 1", content="Content of post 1.", author=user, status="published"
     )
     Post.post_objects.create(
         title="Post 2", content="Content of post 2.", author=user, status="published"
     )
 
     url = reverse("djpress:rss_feed")
     response = client.get(url)
 
     assert response.status_code == 200
     assert response["Content-Type"] == "application/rss+xml; charset=utf-8"
 
     feed = response.content.decode("utf-8")
-    assert "<title>stuartm.nz</title>" in feed
-    assert "<link>http://testserver/rss</link>" in feed
-    assert "<description>stuartm.nz updates</description>" in feed
+    assert f"<title>{settings.BLOG_TITLE}</title>" in feed
+    assert f"<link>http://testserver/{settings.RSS_PATH}/</link>" in feed
+    assert f"<description>{settings.BLOG_DESCRIPTION}</description>" in feed
     assert "<item>" in feed
     assert "<title>Post 1</title>" in feed
     assert "<description>&lt;p&gt;Content of post 1.&lt;/p&gt;</description>" in feed
     assert "<title>Post 2</title>" in feed
     assert "<description>&lt;p&gt;Content of post 2.&lt;/p&gt;</description>" in feed
 
 
 @pytest.mark.django_db
-def test_truncated_posts_feed(client):
-    user = User.objects.create_user(username="testuser", password="testpass")
+def test_truncated_posts_feed(client, user):
+    # Confirm the truncate tag is set according to settings_testing.py
+    truncate_tag = "<!--test-more-->"
+    assert settings.TRUNCATE_TAG == truncate_tag
+    post_prefix = "test-posts"
+    assert settings.POST_PREFIX == post_prefix
+
     Post.post_objects.create(
         title="Post 1",
-        content="Content of post 1.<!--more-->Truncated content",
+        content=f"Content of post 1.{truncate_tag}Truncated content",
         author=user,
         status="published",
     )
 
-    # Disable any permalinks
-    settings.POST_PERMALINK = ""
-    settings.POST_PREFIX = ""
-
     url = reverse("djpress:rss_feed")
     response = client.get(url)
 
     assert response.status_code == 200
     assert response["Content-Type"] == "application/rss+xml; charset=utf-8"
 
     feed = response.content.decode("utf-8")
-    assert "<title>stuartm.nz</title>" in feed
-    assert "<link>http://testserver/rss</link>" in feed
-    assert "<description>stuartm.nz updates</description>" in feed
+    assert f"<title>{settings.BLOG_TITLE}</title>" in feed
+    assert f"<link>http://testserver/{settings.RSS_PATH}/</link>" in feed
+    assert f"<description>{settings.BLOG_DESCRIPTION}</description>" in feed
     assert "<item>" in feed
     assert "<title>Post 1</title>" in feed
     assert "Truncated content" not in feed
-    print(feed)
-    assert '&lt;a href="/post-1/"&gt;Read more&lt;/a&gt;&lt;/p&gt;' in feed
+    assert (
+        f'&lt;a href="/{post_prefix}/post-1/"&gt;Read more&lt;/a&gt;&lt;/p&gt;' in feed
+    )
```

### Comparing `djpress-0.3.3/tests/test_views.py` & `djpress-0.3.4/tests/test_views.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from django.contrib.auth.models import User
 from django.urls import reverse
 from django.utils import timezone
 
-from djpress.conf import settings
 from djpress.models import Category, Post
+from djpress.views import validate_date
 
 
 @pytest.fixture
 def user():
     user = User.objects.create_user(
         username="testuser",
         password="testpass",
@@ -40,70 +40,128 @@
     return post
 
 
 @pytest.mark.django_db
 def test_index_view(client):
     url = reverse("djpress:index")
     response = client.get(url)
-    print(response.content)
     assert response.status_code == 200
     assert b"No posts available" in response.content
 
 
 @pytest.mark.django_db
-def test_content_detail_view(client, create_test_post):
-    settings.POST_PREFIX = ""
-    url = reverse("djpress:post_detail", args=[create_test_post.slug])
+def test_post_detail_view(client, create_test_post):
+    url = reverse("djpress:post_detail", args=[create_test_post.permalink])
     response = client.get(url)
     assert response.status_code == 200
     assert "post" in response.context
 
 
 @pytest.mark.django_db
-def test_content_detail_not_exist(client):
+def test_post_detail_not_exist(client):
     url = reverse("djpress:post_detail", args=["foobar-does-not-exist"])
     response = client.get(url)
     assert response.status_code == 404
 
 
 @pytest.mark.django_db
+def test_author_with_no_posts_view(client, user):
+    url = reverse("djpress:author_posts", args=[user.username])
+    response = client.get(url)
+    assert response.status_code == 200
+    assert "author" in response.context
+    assert "posts" in response.context
+    assert b"No posts available" in response.content
+
+
+@pytest.mark.django_db
+def test_author_with_posts_view(client, create_test_post):
+    url = reverse("djpress:author_posts", args=[create_test_post.author.username])
+    response = client.get(url)
+    assert response.status_code == 200
+    assert "author" in response.context
+    assert "posts" in response.context
+    assert not b"No posts available" in response.content
+
+
+@pytest.mark.django_db
+def test_author_with_invalid_author(client):
+    url = reverse("djpress:author_posts", args=["non-existent-author"])
+    response = client.get(url)
+    assert response.status_code == 404
+
+
+@pytest.mark.django_db
 def test_category_with_no_posts_view(client, category):
     url = reverse("djpress:category_posts", args=[category.slug])
     response = client.get(url)
     assert response.status_code == 200
     assert "category" in response.context
     assert "posts" in response.context
     assert b"No posts available" in response.content
 
 
 @pytest.mark.django_db
 def test_category_with_posts_view(client, create_test_post, category):
-    print(create_test_post.title)
     url = reverse("djpress:category_posts", args=[category.slug])
     response = client.get(url)
     assert response.status_code == 200
     assert "category" in response.context
     assert "posts" in response.context
     assert not b"No posts available" in response.content
 
 
 @pytest.mark.django_db
+def test_category_with_invalid_category(client):
+    url = reverse("djpress:category_posts", args=["non-existent-category"])
+    response = client.get(url)
+    assert response.status_code == 404
+
+
+def test_validate_date():
+    # Test 1 - invalid year
+    year = "0000"
+    with pytest.raises(ValueError):
+        validate_date(year, "", "")
+
+    # Test 2 - invalid months
+    month = "00"
+    with pytest.raises(ValueError):
+        validate_date("2024", month, "")
+    month = "13"
+    with pytest.raises(ValueError):
+        validate_date("2024", month, "")
+
+    # Test 3 - invalid days
+    day = "00"
+    with pytest.raises(ValueError):
+        validate_date("2024", "1", day)
+    day = "32"
+    with pytest.raises(ValueError):
+        validate_date("2024", "1", day)
+
+
+@pytest.mark.django_db
 def test_date_archives_year(client, create_test_post):
     url = reverse("djpress:archives_posts", kwargs={"year": "2024"})
-    settings.POST_PREFIX = ""
     response = client.get(url)
     assert response.status_code == 200
     assert "posts" in response.context
     assert create_test_post.title.encode() in response.content
 
 
 @pytest.mark.django_db
+def test_date_archives_year_invalid_year(client):
+    response = client.get("/archives/0000/")
+    assert response.status_code == 400
+
+
+@pytest.mark.django_db
 def test_date_archives_year_no_posts(client, create_test_post):
     url = reverse("djpress:archives_posts", kwargs={"year": "2023"})
-    settings.POST_PREFIX = ""
     response = client.get(url)
     assert response.status_code == 200
     assert "posts" in response.context
     assert not create_test_post.title.encode() in response.content
     assert b"No posts available" in response.content
 
 
@@ -113,14 +171,22 @@
     response = client.get(url)
     assert response.status_code == 200
     assert "posts" in response.context
     assert create_test_post.title.encode() in response.content
 
 
 @pytest.mark.django_db
+def test_date_archives_month_invalid_month(client):
+    response1 = client.get("/archives/2024/00/")
+    assert response1.status_code == 400
+    response2 = client.get("/archives/2024/13/")
+    assert response2.status_code == 400
+
+
+@pytest.mark.django_db
 def test_date_archives_month_no_posts(client, create_test_post):
     url = reverse("djpress:archives_posts", kwargs={"year": "2024", "month": "02"})
     response = client.get(url)
     assert response.status_code == 200
     assert "posts" in response.context
     assert not create_test_post.title.encode() in response.content
     assert b"No posts available" in response.content
@@ -134,14 +200,22 @@
     response = client.get(url)
     assert response.status_code == 200
     assert "posts" in response.context
     assert create_test_post.title.encode() in response.content
 
 
 @pytest.mark.django_db
+def test_date_archives_day_invalid_day(client):
+    response1 = client.get("/archives/2024/01/00/")
+    assert response1.status_code == 400
+    response2 = client.get("/archives/2024/01/32/")
+    assert response2.status_code == 400
+
+
+@pytest.mark.django_db
 def test_date_archives_day_no_posts(client, create_test_post):
     url = reverse(
         "djpress:archives_posts", kwargs={"year": "2024", "month": "01", "day": "02"}
     )
     response = client.get(url)
     assert response.status_code == 200
     assert "posts" in response.context
```

