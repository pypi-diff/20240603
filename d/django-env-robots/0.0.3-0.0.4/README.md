# Comparing `tmp/django_env_robots-0.0.3.tar.gz` & `tmp/django_env_robots-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_env_robots-0.0.3.tar", last modified: Mon Jun  3 09:55:59 2024, max compression
+gzip compressed data, was "django_env_robots-0.0.4.tar", last modified: Mon Jun  3 12:53:07 2024, max compression
```

## Comparing `django_env_robots-0.0.3.tar` & `django_env_robots-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 09:55:59.641345 django_env_robots-0.0.3/
--rw-r--r--   0 patsmith   (501) staff       (20)     1064 2024-05-22 15:42:15.000000 django_env_robots-0.0.3/LICENSE
--rw-r--r--   0 patsmith   (501) staff       (20)        0 2024-05-23 11:37:41.000000 django_env_robots-0.0.3/MANIFEST.in
--rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-06-03 09:55:59.640775 django_env_robots-0.0.3/PKG-INFO
--rw-r--r--   0 patsmith   (501) staff       (20)     1521 2024-05-23 14:09:35.000000 django_env_robots-0.0.3/README.md
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 09:55:59.637528 django_env_robots-0.0.3/django_env_robots/
--rw-r--r--   0 patsmith   (501) staff       (20)       21 2024-05-22 15:58:37.000000 django_env_robots-0.0.3/django_env_robots/__init__.py
--rw-r--r--   0 patsmith   (501) staff       (20)      155 2024-05-22 15:56:56.000000 django_env_robots-0.0.3/django_env_robots/apps.py
--rw-r--r--   0 patsmith   (501) staff       (20)       57 2024-05-22 15:23:46.000000 django_env_robots-0.0.3/django_env_robots/models.py
--rw-r--r--   0 patsmith   (501) staff       (20)       60 2024-05-22 15:23:46.000000 django_env_robots-0.0.3/django_env_robots/tests.py
--rw-r--r--   0 patsmith   (501) staff       (20)      115 2024-05-23 13:41:24.000000 django_env_robots-0.0.3/django_env_robots/urls.py
--rw-r--r--   0 patsmith   (501) staff       (20)      811 2024-05-31 16:17:00.000000 django_env_robots-0.0.3/django_env_robots/views.py
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 09:55:59.640164 django_env_robots-0.0.3/django_env_robots.egg-info/
--rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/PKG-INFO
--rw-r--r--   0 patsmith   (501) staff       (20)      412 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/SOURCES.txt
--rw-r--r--   0 patsmith   (501) staff       (20)        1 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/dependency_links.txt
--rw-r--r--   0 patsmith   (501) staff       (20)       12 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/requires.txt
--rw-r--r--   0 patsmith   (501) staff       (20)       18 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/top_level.txt
--rw-r--r--   0 patsmith   (501) staff       (20)      820 2024-05-31 16:20:00.000000 django_env_robots-0.0.3/pyproject.toml
--rw-r--r--   0 patsmith   (501) staff       (20)       38 2024-06-03 09:55:59.641457 django_env_robots-0.0.3/setup.cfg
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 12:53:07.239300 django_env_robots-0.0.4/
+-rw-r--r--   0 patsmith   (501) staff       (20)     1064 2024-05-22 15:42:15.000000 django_env_robots-0.0.4/LICENSE
+-rw-r--r--   0 patsmith   (501) staff       (20)        0 2024-05-23 11:37:41.000000 django_env_robots-0.0.4/MANIFEST.in
+-rw-r--r--   0 patsmith   (501) staff       (20)     3203 2024-06-03 12:53:07.238622 django_env_robots-0.0.4/PKG-INFO
+-rw-r--r--   0 patsmith   (501) staff       (20)     1405 2024-06-03 12:48:32.000000 django_env_robots-0.0.4/README.md
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 12:53:07.234660 django_env_robots-0.0.4/django_env_robots/
+-rw-r--r--   0 patsmith   (501) staff       (20)       21 2024-05-22 15:58:37.000000 django_env_robots-0.0.4/django_env_robots/__init__.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      155 2024-05-22 15:56:56.000000 django_env_robots-0.0.4/django_env_robots/apps.py
+-rw-r--r--   0 patsmith   (501) staff       (20)       57 2024-05-22 15:23:46.000000 django_env_robots-0.0.4/django_env_robots/models.py
+-rw-r--r--   0 patsmith   (501) staff       (20)       60 2024-05-22 15:23:46.000000 django_env_robots-0.0.4/django_env_robots/tests.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      115 2024-05-23 13:41:24.000000 django_env_robots-0.0.4/django_env_robots/urls.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      480 2024-06-03 12:39:31.000000 django_env_robots-0.0.4/django_env_robots/views.py
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 12:53:07.237851 django_env_robots-0.0.4/django_env_robots.egg-info/
+-rw-r--r--   0 patsmith   (501) staff       (20)     3203 2024-06-03 12:53:07.000000 django_env_robots-0.0.4/django_env_robots.egg-info/PKG-INFO
+-rw-r--r--   0 patsmith   (501) staff       (20)      412 2024-06-03 12:53:07.000000 django_env_robots-0.0.4/django_env_robots.egg-info/SOURCES.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)        1 2024-06-03 12:53:07.000000 django_env_robots-0.0.4/django_env_robots.egg-info/dependency_links.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)       12 2024-06-03 12:53:07.000000 django_env_robots-0.0.4/django_env_robots.egg-info/requires.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)       18 2024-06-03 12:53:07.000000 django_env_robots-0.0.4/django_env_robots.egg-info/top_level.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)      820 2024-06-03 12:51:35.000000 django_env_robots-0.0.4/pyproject.toml
+-rw-r--r--   0 patsmith   (501) staff       (20)       38 2024-06-03 12:53:07.239501 django_env_robots-0.0.4/setup.cfg
```

### Comparing `django_env_robots-0.0.3/LICENSE` & `django_env_robots-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_env_robots-0.0.3/PKG-INFO` & `django_env_robots-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-env-robots
-Version: 0.0.3
+Version: 0.0.4
 Summary: Control robots.txt files from environment variables and templates.
 Author-email: Pat Smith <pat.smith@cursive.works>
 License: MIT License
         
         Copyright (c) 2024 Cursive
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,16 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2
 
 # Django Env Robots (.txt)
 
-Serve different robots.txt from your production | stage | etc servers by setting environment variables. Rules are managed via templates.
+Serve different robots.txt from your production | stage | etc servers by setting environment variables.
+Rules are managed via templates.
 By default it excludes robots entirely.
 
 
 ## Installation
 
 Install from [PyPI](https://pypi.org/project/django-env-robots/):
 
@@ -56,20 +57,18 @@
 ```
 
 ## Usage
 
 ### settings.py
 Set the following:
  - `SERVER_ENV` identifies the nature of the server and thus the robots.txt template that will be used.
- - `ROBOT_SITEMAP_URLS` a list of relative urls to your sitemap(s).
 
 E.g:
 ```
 SERVER_ENV = 'production'
-ROBOTS_SITEMAP_URLS = ['/sitemap.xml', '/other_sitemap.xml']
 ```
 
 ### urls.py
 ```
 from django_env_robots import urls as robots_urls
 ...
 urlpatterns = [
@@ -84,16 +83,16 @@
 For example, if `SERVER_ENV` can be `production` or `stage`, then create:
  - `templates/robots/production.txt`
  - `templates/robots/stage.txt`
 
 e.g:
 ```
 User-agent: *
-Disallow: /admin/*
+Disallow: /admin/
 
-{% for sitemap_url in sitemap_urls %}Sitemap: {{ sitemap_url }}
-{% endfor %}
+Sitemap: https://www.example.com/sitemap.xml
+Sitemap: https://www2.example.com/sitemap.xml
 ```
 
 ### Other considertions
 
 A robots.txt being served from a Whitenose public directory will win over this app. That is because of whitenoise's middleware behaviour - quite correct but watch out for that.
```

### Comparing `django_env_robots-0.0.3/README.md` & `django_env_robots-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Django Env Robots (.txt)
 
-Serve different robots.txt from your production | stage | etc servers by setting environment variables. Rules are managed via templates.
+Serve different robots.txt from your production | stage | etc servers by setting environment variables.
+Rules are managed via templates.
 By default it excludes robots entirely.
 
 
 ## Installation
 
 Install from [PyPI](https://pypi.org/project/django-env-robots/):
 
@@ -19,20 +20,18 @@
 ```
 
 ## Usage
 
 ### settings.py
 Set the following:
  - `SERVER_ENV` identifies the nature of the server and thus the robots.txt template that will be used.
- - `ROBOT_SITEMAP_URLS` a list of relative urls to your sitemap(s).
 
 E.g:
 ```
 SERVER_ENV = 'production'
-ROBOTS_SITEMAP_URLS = ['/sitemap.xml', '/other_sitemap.xml']
 ```
 
 ### urls.py
 ```
 from django_env_robots import urls as robots_urls
 ...
 urlpatterns = [
@@ -47,16 +46,16 @@
 For example, if `SERVER_ENV` can be `production` or `stage`, then create:
  - `templates/robots/production.txt`
  - `templates/robots/stage.txt`
 
 e.g:
 ```
 User-agent: *
-Disallow: /admin/*
+Disallow: /admin/
 
-{% for sitemap_url in sitemap_urls %}Sitemap: {{ sitemap_url }}
-{% endfor %}
+Sitemap: https://www.example.com/sitemap.xml
+Sitemap: https://www2.example.com/sitemap.xml
 ```
 
 ### Other considertions
 
 A robots.txt being served from a Whitenose public directory will win over this app. That is because of whitenoise's middleware behaviour - quite correct but watch out for that.
```

### Comparing `django_env_robots-0.0.3/django_env_robots.egg-info/PKG-INFO` & `django_env_robots-0.0.4/django_env_robots.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-env-robots
-Version: 0.0.3
+Version: 0.0.4
 Summary: Control robots.txt files from environment variables and templates.
 Author-email: Pat Smith <pat.smith@cursive.works>
 License: MIT License
         
         Copyright (c) 2024 Cursive
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,15 +33,16 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2
 
 # Django Env Robots (.txt)
 
-Serve different robots.txt from your production | stage | etc servers by setting environment variables. Rules are managed via templates.
+Serve different robots.txt from your production | stage | etc servers by setting environment variables.
+Rules are managed via templates.
 By default it excludes robots entirely.
 
 
 ## Installation
 
 Install from [PyPI](https://pypi.org/project/django-env-robots/):
 
@@ -56,20 +57,18 @@
 ```
 
 ## Usage
 
 ### settings.py
 Set the following:
  - `SERVER_ENV` identifies the nature of the server and thus the robots.txt template that will be used.
- - `ROBOT_SITEMAP_URLS` a list of relative urls to your sitemap(s).
 
 E.g:
 ```
 SERVER_ENV = 'production'
-ROBOTS_SITEMAP_URLS = ['/sitemap.xml', '/other_sitemap.xml']
 ```
 
 ### urls.py
 ```
 from django_env_robots import urls as robots_urls
 ...
 urlpatterns = [
@@ -84,16 +83,16 @@
 For example, if `SERVER_ENV` can be `production` or `stage`, then create:
  - `templates/robots/production.txt`
  - `templates/robots/stage.txt`
 
 e.g:
 ```
 User-agent: *
-Disallow: /admin/*
+Disallow: /admin/
 
-{% for sitemap_url in sitemap_urls %}Sitemap: {{ sitemap_url }}
-{% endfor %}
+Sitemap: https://www.example.com/sitemap.xml
+Sitemap: https://www2.example.com/sitemap.xml
 ```
 
 ### Other considertions
 
 A robots.txt being served from a Whitenose public directory will win over this app. That is because of whitenoise's middleware behaviour - quite correct but watch out for that.
```

### Comparing `django_env_robots-0.0.3/pyproject.toml` & `django_env_robots-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-env-robots"
-version = "0.0.3"
+version = "0.0.4"
 description = "Control robots.txt files from environment variables and templates."
 readme = "README.md"
 authors = [{ name = "Pat Smith", email = "pat.smith@cursive.works" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

