# Comparing `tmp/django_env_robots-0.0.2.tar.gz` & `tmp/django_env_robots-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_env_robots-0.0.2.tar", last modified: Thu May 23 14:10:56 2024, max compression
+gzip compressed data, was "django_env_robots-0.0.3.tar", last modified: Mon Jun  3 09:55:59 2024, max compression
```

## Comparing `django_env_robots-0.0.2.tar` & `django_env_robots-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 14:10:56.354541 django_env_robots-0.0.2/
--rw-r--r--   0 patsmith   (501) staff       (20)     1064 2024-05-22 15:42:15.000000 django_env_robots-0.0.2/LICENSE
--rw-r--r--   0 patsmith   (501) staff       (20)        0 2024-05-23 11:37:41.000000 django_env_robots-0.0.2/MANIFEST.in
--rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-05-23 14:10:56.353827 django_env_robots-0.0.2/PKG-INFO
--rw-r--r--   0 patsmith   (501) staff       (20)     1521 2024-05-23 14:09:35.000000 django_env_robots-0.0.2/README.md
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 14:10:56.349673 django_env_robots-0.0.2/django_env_robots/
--rw-r--r--   0 patsmith   (501) staff       (20)       21 2024-05-22 15:58:37.000000 django_env_robots-0.0.2/django_env_robots/__init__.py
--rw-r--r--   0 patsmith   (501) staff       (20)      155 2024-05-22 15:56:56.000000 django_env_robots-0.0.2/django_env_robots/apps.py
--rw-r--r--   0 patsmith   (501) staff       (20)       57 2024-05-22 15:23:46.000000 django_env_robots-0.0.2/django_env_robots/models.py
--rw-r--r--   0 patsmith   (501) staff       (20)       60 2024-05-22 15:23:46.000000 django_env_robots-0.0.2/django_env_robots/tests.py
--rw-r--r--   0 patsmith   (501) staff       (20)      115 2024-05-23 13:41:24.000000 django_env_robots-0.0.2/django_env_robots/urls.py
--rw-r--r--   0 patsmith   (501) staff       (20)      784 2024-05-23 13:50:02.000000 django_env_robots-0.0.2/django_env_robots/views.py
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 14:10:56.352994 django_env_robots-0.0.2/django_env_robots.egg-info/
--rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/PKG-INFO
--rw-r--r--   0 patsmith   (501) staff       (20)      412 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/SOURCES.txt
--rw-r--r--   0 patsmith   (501) staff       (20)        1 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/dependency_links.txt
--rw-r--r--   0 patsmith   (501) staff       (20)       12 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/requires.txt
--rw-r--r--   0 patsmith   (501) staff       (20)       18 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/top_level.txt
--rw-r--r--   0 patsmith   (501) staff       (20)      820 2024-05-23 13:54:45.000000 django_env_robots-0.0.2/pyproject.toml
--rw-r--r--   0 patsmith   (501) staff       (20)       38 2024-05-23 14:10:56.354680 django_env_robots-0.0.2/setup.cfg
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 09:55:59.641345 django_env_robots-0.0.3/
+-rw-r--r--   0 patsmith   (501) staff       (20)     1064 2024-05-22 15:42:15.000000 django_env_robots-0.0.3/LICENSE
+-rw-r--r--   0 patsmith   (501) staff       (20)        0 2024-05-23 11:37:41.000000 django_env_robots-0.0.3/MANIFEST.in
+-rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-06-03 09:55:59.640775 django_env_robots-0.0.3/PKG-INFO
+-rw-r--r--   0 patsmith   (501) staff       (20)     1521 2024-05-23 14:09:35.000000 django_env_robots-0.0.3/README.md
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 09:55:59.637528 django_env_robots-0.0.3/django_env_robots/
+-rw-r--r--   0 patsmith   (501) staff       (20)       21 2024-05-22 15:58:37.000000 django_env_robots-0.0.3/django_env_robots/__init__.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      155 2024-05-22 15:56:56.000000 django_env_robots-0.0.3/django_env_robots/apps.py
+-rw-r--r--   0 patsmith   (501) staff       (20)       57 2024-05-22 15:23:46.000000 django_env_robots-0.0.3/django_env_robots/models.py
+-rw-r--r--   0 patsmith   (501) staff       (20)       60 2024-05-22 15:23:46.000000 django_env_robots-0.0.3/django_env_robots/tests.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      115 2024-05-23 13:41:24.000000 django_env_robots-0.0.3/django_env_robots/urls.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      811 2024-05-31 16:17:00.000000 django_env_robots-0.0.3/django_env_robots/views.py
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-06-03 09:55:59.640164 django_env_robots-0.0.3/django_env_robots.egg-info/
+-rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/PKG-INFO
+-rw-r--r--   0 patsmith   (501) staff       (20)      412 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/SOURCES.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)        1 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/dependency_links.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)       12 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/requires.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)       18 2024-06-03 09:55:59.000000 django_env_robots-0.0.3/django_env_robots.egg-info/top_level.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)      820 2024-05-31 16:20:00.000000 django_env_robots-0.0.3/pyproject.toml
+-rw-r--r--   0 patsmith   (501) staff       (20)       38 2024-06-03 09:55:59.641457 django_env_robots-0.0.3/setup.cfg
```

### Comparing `django_env_robots-0.0.2/LICENSE` & `django_env_robots-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_env_robots-0.0.2/PKG-INFO` & `django_env_robots-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-env-robots
-Version: 0.0.2
+Version: 0.0.3
 Summary: Control robots.txt files from environment variables and templates.
 Author-email: Pat Smith <pat.smith@cursive.works>
 License: MIT License
         
         Copyright (c) 2024 Cursive
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django_env_robots-0.0.2/README.md` & `django_env_robots-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_env_robots-0.0.2/django_env_robots/views.py` & `django_env_robots-0.0.3/django_env_robots/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
     template_name = f"robots/{settings.SERVER_ENV}.txt"
     try:
         loader.get_template(template_name)
     except TemplateDoesNotExist:
         template_name = "robots/default.txt"
 
-    return render(request, template_name, context=context)
+    return render(request, template_name, context=context, content_type="text/plain")
```

### Comparing `django_env_robots-0.0.2/django_env_robots.egg-info/PKG-INFO` & `django_env_robots-0.0.3/django_env_robots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-env-robots
-Version: 0.0.2
+Version: 0.0.3
 Summary: Control robots.txt files from environment variables and templates.
 Author-email: Pat Smith <pat.smith@cursive.works>
 License: MIT License
         
         Copyright (c) 2024 Cursive
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django_env_robots-0.0.2/pyproject.toml` & `django_env_robots-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-env-robots"
-version = "0.0.2"
+version = "0.0.3"
 description = "Control robots.txt files from environment variables and templates."
 readme = "README.md"
 authors = [{ name = "Pat Smith", email = "pat.smith@cursive.works" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

