# Comparing `tmp/dadmin-celery-1.0.tar.gz` & `tmp/dadmin_celery-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dadmin-celery-1.0.tar", last modified: Thu Apr 18 09:07:37 2024, max compression
+gzip compressed data, was "dadmin_celery-1.0.1.tar", last modified: Mon Jun  3 03:52:42 2024, max compression
```

## Comparing `dadmin-celery-1.0.tar` & `dadmin_celery-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 09:07:37.446736 dadmin-celery-1.0/
--rw-rw-rw-   0        0        0     1096 2024-04-18 08:27:09.000000 dadmin-celery-1.0/LICENSE
--rw-rw-rw-   0        0        0       48 2024-04-18 08:27:09.000000 dadmin-celery-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3871 2024-04-18 09:07:37.445737 dadmin-celery-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3354 2024-04-18 08:56:33.000000 dadmin-celery-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 09:07:37.360222 dadmin-celery-1.0/dadmin_celery.egg-info/
--rw-rw-rw-   0        0        0     3871 2024-04-18 09:07:37.000000 dadmin-celery-1.0/dadmin_celery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-04-18 09:07:37.000000 dadmin-celery-1.0/dadmin_celery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 09:07:37.000000 dadmin-celery-1.0/dadmin_celery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2024-04-18 09:07:37.000000 dadmin-celery-1.0/dadmin_celery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-18 09:07:37.000000 dadmin-celery-1.0/dadmin_celery.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 09:07:37.371855 dadmin-celery-1.0/dvadmin_celery/
--rw-rw-rw-   0        0        0        0 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/__init__.py
--rw-rw-rw-   0        0        0       34 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/admin.py
--rw-rw-rw-   0        0        0      200 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:07:37.398481 dadmin-celery-1.0/dvadmin_celery/fixtures/
--rw-rw-rw-   0        0        0        0 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/fixtures/__init__.py
--rw-rw-rw-   0        0        0     1745 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/fixtures/init_menu.json
--rw-rw-rw-   0        0        0      609 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/fixtures/initialize.py
--rw-rw-rw-   0        0        0     2174 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/settings.py
--rw-rw-rw-   0        0        0      360 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/tasks.py
--rw-rw-rw-   0        0        0     1171 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/urls.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:07:37.436257 dadmin-celery-1.0/dvadmin_celery/views/
--rw-rw-rw-   0        0        0        0 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/views/__init__.py
--rw-rw-rw-   0        0        0      721 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/views/crontab_schedule.py
--rw-rw-rw-   0        0        0      639 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/views/interval_schedule.py
--rw-rw-rw-   0        0        0     2719 2024-04-18 08:27:09.000000 dadmin-celery-1.0/dvadmin_celery/views/periodic_task.py
--rw-rw-rw-   0        0        0     5694 2024-04-18 08:32:38.000000 dadmin-celery-1.0/dvadmin_celery/views/task.py
--rw-rw-rw-   0        0        0     1224 2024-04-18 08:29:21.000000 dadmin-celery-1.0/dvadmin_celery/views/task_detail.py
--rw-rw-rw-   0        0        0      110 2024-04-18 08:27:09.000000 dadmin-celery-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 09:07:37.446736 dadmin-celery-1.0/setup.cfg
--rw-rw-rw-   0        0        0      958 2024-04-18 09:07:19.000000 dadmin-celery-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:52:42.647798 dadmin_celery-1.0.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       48 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4000 2024-06-03 03:52:42.646791 dadmin_celery-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3354 2024-04-18 08:56:33.000000 dadmin_celery-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 03:52:42.646791 dadmin_celery-1.0.1/dadmin_celery.egg-info/
+-rw-rw-rw-   0        0        0     4000 2024-06-03 03:52:42.000000 dadmin_celery-1.0.1/dadmin_celery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-06-03 03:52:42.000000 dadmin_celery-1.0.1/dadmin_celery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 03:52:42.000000 dadmin_celery-1.0.1/dadmin_celery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-06-03 03:52:42.000000 dadmin_celery-1.0.1/dadmin_celery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-03 03:52:42.000000 dadmin_celery-1.0.1/dadmin_celery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 03:52:42.557297 dadmin_celery-1.0.1/dvadmin_celery/
+-rw-rw-rw-   0        0        0        0 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/__init__.py
+-rw-rw-rw-   0        0        0       34 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/admin.py
+-rw-rw-rw-   0        0        0      200 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/apps.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:52:42.573923 dadmin_celery-1.0.1/dvadmin_celery/fixtures/
+-rw-rw-rw-   0        0        0        0 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/fixtures/__init__.py
+-rw-rw-rw-   0        0        0     1745 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/fixtures/init_menu.json
+-rw-rw-rw-   0        0        0      609 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/fixtures/initialize.py
+-rw-rw-rw-   0        0        0     2174 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/settings.py
+-rw-rw-rw-   0        0        0      360 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/tasks.py
+-rw-rw-rw-   0        0        0     1171 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/urls.py
+drwxrwxrwx   0        0        0        0 2024-06-03 03:52:42.635766 dadmin_celery-1.0.1/dvadmin_celery/views/
+-rw-rw-rw-   0        0        0        0 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/views/__init__.py
+-rw-rw-rw-   0        0        0      721 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/views/crontab_schedule.py
+-rw-rw-rw-   0        0        0      639 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/views/interval_schedule.py
+-rw-rw-rw-   0        0        0     2719 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/dvadmin_celery/views/periodic_task.py
+-rw-rw-rw-   0        0        0     5694 2024-04-18 08:32:38.000000 dadmin_celery-1.0.1/dvadmin_celery/views/task.py
+-rw-rw-rw-   0        0        0     1327 2024-06-03 03:37:41.000000 dadmin_celery-1.0.1/dvadmin_celery/views/task_detail.py
+-rw-rw-rw-   0        0        0      110 2024-04-18 08:27:09.000000 dadmin_celery-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 03:52:42.647798 dadmin_celery-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      960 2024-06-03 03:47:55.000000 dadmin_celery-1.0.1/setup.py
```

### Comparing `dadmin-celery-1.0/LICENSE` & `dadmin_celery-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/PKG-INFO` & `dadmin_celery-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dadmin-celery
-Version: 1.0
+Version: 1.0.1
 Summary: 适用于 django-vue-admin 的celery异步插件
 Home-page: https://gitee.com/zouxingshun/dvadmin-celery
 Author: zouxs
 Author-email: liqiang@django-vue-admin.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: django-celery-beat>=2.5.0
+Requires-Dist: tenant-schemas-celery>=2.2.0
+Requires-Dist: django-redis>=5.2.0
+Requires-Dist: django-celery-results>=2.5.1
 
 # dvadmin_celery
 
 #### 介绍
 本包仅因为原仓库长期不更新而自行建库,并开源使用
 
 dadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
@@ -139,9 +141,7 @@
 改为
 app = Celery(f"application", include=['dvadmin_celery.tasks'])
 再重启尝试
 ```
 redis下载地址：<br>
 Mac/Linux下载 http://download.redis.io/releases/ <br>
 Windows下载 https://github.com/tporadowski/redis/releases/ <br>
-
-
```

### Comparing `dadmin-celery-1.0/README.md` & `dadmin_celery-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dadmin_celery.egg-info/PKG-INFO` & `dadmin_celery-1.0.1/dadmin_celery.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dadmin-celery
-Version: 1.0
+Version: 1.0.1
 Summary: 适用于 django-vue-admin 的celery异步插件
 Home-page: https://gitee.com/zouxingshun/dvadmin-celery
 Author: zouxs
 Author-email: liqiang@django-vue-admin.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: django-celery-beat>=2.5.0
+Requires-Dist: tenant-schemas-celery>=2.2.0
+Requires-Dist: django-redis>=5.2.0
+Requires-Dist: django-celery-results>=2.5.1
 
 # dvadmin_celery
 
 #### 介绍
 本包仅因为原仓库长期不更新而自行建库,并开源使用
 
 dadmin-celery 插件是集成 django-celery-beat、tenant-schemas-celery、django-redis、django-celery-results 的一个后端插件，
@@ -139,9 +141,7 @@
 改为
 app = Celery(f"application", include=['dvadmin_celery.tasks'])
 再重启尝试
 ```
 redis下载地址：<br>
 Mac/Linux下载 http://download.redis.io/releases/ <br>
 Windows下载 https://github.com/tporadowski/redis/releases/ <br>
-
-
```

### Comparing `dadmin-celery-1.0/dadmin_celery.egg-info/SOURCES.txt` & `dadmin_celery-1.0.1/dadmin_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/fixtures/init_menu.json` & `dadmin_celery-1.0.1/dvadmin_celery/fixtures/init_menu.json`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/fixtures/initialize.py` & `dadmin_celery-1.0.1/dvadmin_celery/fixtures/initialize.py`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/settings.py` & `dadmin_celery-1.0.1/dvadmin_celery/settings.py`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/urls.py` & `dadmin_celery-1.0.1/dvadmin_celery/urls.py`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/views/crontab_schedule.py` & `dadmin_celery-1.0.1/dvadmin_celery/views/crontab_schedule.py`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/views/interval_schedule.py` & `dadmin_celery-1.0.1/dvadmin_celery/views/interval_schedule.py`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/views/periodic_task.py` & `dadmin_celery-1.0.1/dvadmin_celery/views/periodic_task.py`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/views/task.py` & `dadmin_celery-1.0.1/dvadmin_celery/views/task.py`

 * *Files identical despite different names*

### Comparing `dadmin-celery-1.0/dvadmin_celery/views/task_detail.py` & `dadmin_celery-1.0.1/dvadmin_celery/views/task_detail.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     # def get_result(self, obj):
     #     value = json.loads(obj.result)
     #     return value
 
 
 class CeleryTaskDetailFilterSet(django_filters.FilterSet):
     date_created = django_filters.BaseRangeFilter(field_name="date_created")
+    task_name = django_filters.CharFilter(field_name='task_name', lookup_expr='task_name__icontains')
     class Meta:
         model = TaskResult
         fields = ['id', 'status', 'date_done', 'date_created', 'result', 'task_name', 'periodic_task_name']
```

### Comparing `dadmin-celery-1.0/setup.py` & `dadmin_celery-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dadmin-celery",
-    version="1.0",
+    version="1.0.1",
     author="zouxs",
     author_email="liqiang@django-vue-admin.com",
     description="适用于 django-vue-admin 的celery异步插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/zouxingshun/dvadmin-celery",
     packages=setuptools.find_packages(),
```

