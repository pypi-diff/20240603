# Comparing `tmp/EOxServer-1.3.0.tar.gz` & `tmp/EOxServer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EOxServer-1.3.0.tar", last modified: Wed Oct  4 15:17:22 2023, max compression
+gzip compressed data, was "EOxServer-1.3.2.tar", last modified: Mon Jun  3 15:04:06 2024, max compression
```

## Comparing `EOxServer-1.3.0.tar` & `EOxServer-1.3.2.tar`

### file list

```diff
@@ -1,566 +1,566 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.372002 EOxServer-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.324002 EOxServer-1.3.0/EOxServer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-04 15:17:22.000000 EOxServer-1.3.0/EOxServer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21221 2023-10-04 15:17:22.000000 EOxServer-1.3.0/EOxServer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 15:17:22.000000 EOxServer-1.3.0/EOxServer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 15:17:22.000000 EOxServer-1.3.0/EOxServer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-04 15:17:22.000000 EOxServer-1.3.0/EOxServer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-04 15:17:22.000000 EOxServer-1.3.0/EOxServer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-10-04 15:17:05.000000 EOxServer-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-04 15:17:05.000000 EOxServer-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-04 15:17:22.372002 EOxServer-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2023-10-04 15:17:05.000000 EOxServer-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.324002 EOxServer-1.3.0/eoxserver/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/backends/keystone/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/keystone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/keystone/storage_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/backends/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/management/commands/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/management/commands/storageauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/migrations/0002_storage_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/migrations/0003_nameblank.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/migrations/0004_storage_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/storage_auths.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/storages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/testbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/backends/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/conf/default.conf
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/conf/defaultAttributeDictionary
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/conf/default_formats.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/gdal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/gdal_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/mapserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/ogr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/osr.py
--rw-r--r--   0 runner    (1001) docker     (127)    18898 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/vrt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/contrib/vsi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/core/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/commands/create_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/core/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/decoders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/decoders/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/decoders/kvp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/decoders/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/core/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/templates/admin/change_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/templates/eoxserver_index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.328002 EOxServer-1.3.0/eoxserver/core/templates/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/templates/logging/logview.html
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/geotools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/importtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/iteratortools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/multiparttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/perftools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/timetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/util/xmltools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/eoxserver.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/formats.conf
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/outline_template_dataset.html
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/outline_template_footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/outline_template_header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/data/
--rw-r--r--   0 runner    (1001) docker     (127)   879633 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/logs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/logs/DO-NOT-REMOVE
--rw-r--r--   0 runner    (1001) docker     (127)    10753 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/static/DO-NOT-REMOVE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/500.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.html
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.js
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/wcst_perm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/wcst_perm/DO-NOT-REMOVE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/instance_template/project_name/wcst_temp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/wcst_temp/DO-NOT-REMOVE
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/instance_template/project_name/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.320002 EOxServer-1.3.0/eoxserver/media/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/media/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/media/admin/widgets.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/media/images/
--rw-r--r--   0 runner    (1001) docker     (127)   146838 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/media/images/eoxserver_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   171474 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/media/images/eoxserver_logo_transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.332002 EOxServer-1.3.0/eoxserver/processing/gdal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/gdal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31278 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/gdal/reftools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/gdal/vrt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/processing/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/preprocessing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/preprocessing/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/preprocessing/georeference.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/preprocessing/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/processing/preprocessing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/render/browse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/browse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/browse/defaultstyles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11874 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/browse/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16686 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/browse/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/browse/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/browse/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    32836 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/render/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26071 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/coverage/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/render/map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/map/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11973 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/map/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/map/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/render/mapserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/mapserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/mapserver/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    34146 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/mapserver/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/render/mapserver/map_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/resources/coverages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20916 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/crss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/dateline.py
--rw-r--r--   0 runner    (1001) docker     (127)    16764 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.336002 EOxServer-1.3.0/eoxserver/resources/coverages/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.340002 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/browse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/browsetype.py
--rw-r--r--   0 runner    (1001) docker     (127)    12520 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/collectiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/coveragetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/id.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/mapcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/masktype.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/producttype.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/rasterstyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.340002 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.340002 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py
--rw-r--r--   0 runner    (1001) docker     (127)    14250 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.340002 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/gsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.340002 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/utils/gsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.340002 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    35329 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0006_masktype_validity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0007_typemodels.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0008_incidence_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0009_begin_time_end_time_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0011_bandstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0012_out_of_bounds_data_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0013_raster_style.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44946 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/resources/coverages/registration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19948 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/browse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/resources/coverages/registration/registrators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/registrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/registrators/gdal.py
--rw-r--r--   0 runner    (1001) docker     (127)    30492 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/registration/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/synchronization.py
--rw-r--r--   0 runner    (1001) docker     (127)    22900 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7697 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/resources/coverages/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3317 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/scripts/eoxserver-instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13122 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/auth/charonpdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/auth/dummypdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/auth/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/auth/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/cis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/cis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/cis/v11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/cis/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/cis/v11/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ecql.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20852 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/gdal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/gdal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/gdal/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/gdal/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/gml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/gml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/gml/v32/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/gml/v32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/gml/v32/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/management/commands/eoxs_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/management/commands/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/management/commands/wms_options_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/management/commands/wms_options_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/management/commands/wms_options_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/mapserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.344002 EOxServer-1.3.0/eoxserver/services/mapserver/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/connectors/mosaic_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/connectors/multifile_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/connectors/polygonmask_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/connectors/simple_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/connectors/tileindex_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/mapserver/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wcs/base_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wcs/capabilities_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wcs/coverage_description_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14938 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wcs/coverage_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/mapserver/wms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/capabilities_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/feature_info_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/legendgraphic_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/map_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/mapserver/wms/styleapplicators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/styleapplicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/styleapplicators/sld.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/mapserver/wms/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/migrations/0003_service_name_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/native/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/native/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/native/wcs/capabilities_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/native/wcs/coverage_description_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/opensearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/opensearch/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/extensions/cql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11769 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/extensions/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/extensions/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/extensions/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/opensearch/formats/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/formats/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)    22258 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/formats/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/formats/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/formats/kml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/formats/rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.348002 EOxServer-1.3.0/eoxserver/services/opensearch/v11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/v11/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/v11/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/opensearch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/common/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/common/v11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/common/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/common/v11/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/common/v20/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/common/v20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/common/v20/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/common/v20/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/dseo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/dseo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/dseo/v10/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/dseo/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/dseo/v10/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/dseo/v10/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/basehandlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/describecoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/getcoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/describecoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/getcoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/describecoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/describeeocoverageset.py
--rw-r--r--   0 runner    (1001) docker     (127)    29749 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.352002 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/encodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/encodings/geotiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/getcoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16676 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/geteocoverageset.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.356002 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/packages/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/packages/zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13005 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wcs11Transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.356002 EOxServer-1.3.0/eoxserver/services/ows/wms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/basehandlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    30194 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/layermapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.356002 EOxServer-1.3.0/eoxserver/services/ows/wms/v10/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v10/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v10/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v10/getfeatureinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v10/getmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v10/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.356002 EOxServer-1.3.0/eoxserver/services/ows/wms/v11/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v11/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v11/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v11/getfeatureinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v11/getmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v11/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.356002 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getfeatureinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getlegendgraphic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wms/v13/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.356002 EOxServer-1.3.0/eoxserver/services/ows/wps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10181 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/allowed_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/bboxdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21330 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/complexdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/crs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12743 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/literaldata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/response_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/ows/wps/processes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_cloud_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_dem_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_height_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_time_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15191 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/test_allowed_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    17124 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/describeprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/execute_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/process_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_decoder_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_decoder_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v10/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/ows/wps/v20/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v20/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v20/describeprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v20/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/ows/wps/v20/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    20079 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/subset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.324002 EOxServer-1.3.0/eoxserver/services/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/templates/opensearch/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/templates/opensearch/result.html
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/templates/opensearch/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/templates/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/templates/wcs/error_template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/services/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/templatetags/services_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)    25514 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/services/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/testing/xcomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/webclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.360002 EOxServer-1.3.0/eoxserver/webclient/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/migrations/0002_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.364002 EOxServer-1.3.0/eoxserver/webclient/static/
--rw-r--r--   0 runner    (1001) docker     (127)   554482 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/static/5e3c304ea87541cabdab.worker.js
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127) 10119032 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/static/vsclient.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.324002 EOxServer-1.3.0/eoxserver/webclient/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.372002 EOxServer-1.3.0/eoxserver/webclient/templates/webclient/
--rw-r--r--   0 runner    (1001) docker     (127)    14073 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/templates/webclient/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2023-10-04 15:17:06.000000 EOxServer-1.3.0/eoxserver/webclient/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-04 15:17:06.000000 EOxServer-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2023-10-04 15:17:22.372002 EOxServer-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-10-04 15:17:06.000000 EOxServer-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 15:17:22.372002 EOxServer-1.3.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14419 2023-10-04 15:17:06.000000 EOxServer-1.3.0/tools/eoxserver-atpd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19189 2023-10-04 15:17:06.000000 EOxServer-1.3.0/tools/eoxserver-preprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3435 2023-10-04 15:17:06.000000 EOxServer-1.3.0/tools/eoxserver-validate_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.425521 EOxServer-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.349520 EOxServer-1.3.2/EOxServer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-06-03 15:04:06.000000 EOxServer-1.3.2/EOxServer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21221 2024-06-03 15:04:06.000000 EOxServer-1.3.2/EOxServer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:04:06.000000 EOxServer-1.3.2/EOxServer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 15:04:06.000000 EOxServer-1.3.2/EOxServer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-06-03 15:04:06.000000 EOxServer-1.3.2/EOxServer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-03 15:04:06.000000 EOxServer-1.3.2/EOxServer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-03 15:03:42.000000 EOxServer-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-03 15:03:42.000000 EOxServer-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-06-03 15:04:06.425521 EOxServer-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-06-03 15:03:42.000000 EOxServer-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.349520 EOxServer-1.3.2/eoxserver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.349520 EOxServer-1.3.2/eoxserver/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.349520 EOxServer-1.3.2/eoxserver/backends/keystone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/keystone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/keystone/storage_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.349520 EOxServer-1.3.2/eoxserver/backends/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.349520 EOxServer-1.3.2/eoxserver/backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/management/commands/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/management/commands/storageauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.353520 EOxServer-1.3.2/eoxserver/backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/migrations/0002_storage_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/migrations/0003_nameblank.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/migrations/0004_storage_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/storage_auths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/testbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/backends/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.353520 EOxServer-1.3.2/eoxserver/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/conf/default.conf
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/conf/defaultAttributeDictionary
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/conf/default_formats.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.353520 EOxServer-1.3.2/eoxserver/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/gdal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/gdal_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/mapserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/ogr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/osr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/vrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/contrib/vsi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.353520 EOxServer-1.3.2/eoxserver/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.353520 EOxServer-1.3.2/eoxserver/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/commands/create_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/core/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/decoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/decoders/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/decoders/kvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/decoders/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/core/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/templates/admin/change_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/templates/eoxserver_index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/core/templates/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/templates/logging/logview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/geotools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/importtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/iteratortools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/multiparttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/perftools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/timetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/util/xmltools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/instance_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/instance_template/project_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/eoxserver.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/formats.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/outline_template_dataset.html
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/outline_template_footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/outline_template_header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.357520 EOxServer-1.3.2/eoxserver/instance_template/project_name/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   879633 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/instance_template/project_name/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/logs/DO-NOT-REMOVE
+-rw-r--r--   0 runner    (1001) docker     (127)    10753 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/instance_template/project_name/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/static/DO-NOT-REMOVE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/500.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.html
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/instance_template/project_name/wcst_perm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/wcst_perm/DO-NOT-REMOVE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/instance_template/project_name/wcst_temp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/wcst_temp/DO-NOT-REMOVE
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/instance_template/project_name/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.341520 EOxServer-1.3.2/eoxserver/media/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/media/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/media/admin/widgets.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/media/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   146838 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/media/images/eoxserver_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171474 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/media/images/eoxserver_logo_transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.361520 EOxServer-1.3.2/eoxserver/processing/gdal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/gdal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31278 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/gdal/reftools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/gdal/vrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.365520 EOxServer-1.3.2/eoxserver/processing/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/preprocessing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/preprocessing/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/preprocessing/georeference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/preprocessing/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/processing/preprocessing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.365520 EOxServer-1.3.2/eoxserver/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.365520 EOxServer-1.3.2/eoxserver/render/browse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/browse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/browse/defaultstyles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/browse/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/browse/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/browse/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/browse/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32836 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.365520 EOxServer-1.3.2/eoxserver/render/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26071 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/coverage/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.365520 EOxServer-1.3.2/eoxserver/render/map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/map/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/map/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/map/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.365520 EOxServer-1.3.2/eoxserver/render/mapserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/mapserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/mapserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34146 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/mapserver/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/render/mapserver/map_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.365520 EOxServer-1.3.2/eoxserver/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.369520 EOxServer-1.3.2/eoxserver/resources/coverages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/crss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/dateline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.369520 EOxServer-1.3.2/eoxserver/resources/coverages/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.373520 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/browse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/browsetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/collectiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/coveragetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/mapcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/masktype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/producttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/rasterstyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.373520 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.373520 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14250 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.373520 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.373520 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/utils/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.377520 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    35329 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0006_masktype_validity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0007_typemodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0008_incidence_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0009_begin_time_end_time_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0011_bandstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0012_out_of_bounds_data_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0013_raster_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44946 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.377520 EOxServer-1.3.2/eoxserver/resources/coverages/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19948 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/browse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.377520 EOxServer-1.3.2/eoxserver/resources/coverages/registration/registrators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/registrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/registrators/gdal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30724 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/registration/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7697 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/resources/coverages/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.377520 EOxServer-1.3.2/eoxserver/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3317 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/scripts/eoxserver-instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13122 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/auth/charonpdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/auth/dummypdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/auth/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/auth/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/cis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/cis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/cis/v11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/cis/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/cis/v11/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ecql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20852 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/gdal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/gdal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/gdal/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/gdal/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/gml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/gml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/gml/v32/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/gml/v32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/gml/v32/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/management/commands/eoxs_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/management/commands/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/management/commands/wms_options_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/management/commands/wms_options_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/management/commands/wms_options_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.381520 EOxServer-1.3.2/eoxserver/services/mapserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.385520 EOxServer-1.3.2/eoxserver/services/mapserver/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/connectors/mosaic_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/connectors/multifile_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/connectors/polygonmask_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/connectors/simple_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/connectors/tileindex_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.385520 EOxServer-1.3.2/eoxserver/services/mapserver/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wcs/base_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wcs/capabilities_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wcs/coverage_description_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14938 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wcs/coverage_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.385520 EOxServer-1.3.2/eoxserver/services/mapserver/wms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/capabilities_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/feature_info_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.385520 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/legendgraphic_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/map_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.385520 EOxServer-1.3.2/eoxserver/services/mapserver/wms/styleapplicators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/styleapplicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/styleapplicators/sld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/mapserver/wms/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.385520 EOxServer-1.3.2/eoxserver/services/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/migrations/0003_service_name_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.385520 EOxServer-1.3.2/eoxserver/services/native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.389521 EOxServer-1.3.2/eoxserver/services/native/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/native/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/native/wcs/capabilities_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/native/wcs/coverage_description_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.389521 EOxServer-1.3.2/eoxserver/services/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.389521 EOxServer-1.3.2/eoxserver/services/opensearch/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/extensions/cql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/extensions/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/extensions/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/extensions/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.389521 EOxServer-1.3.2/eoxserver/services/opensearch/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/formats/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/formats/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/formats/kml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/formats/rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.389521 EOxServer-1.3.2/eoxserver/services/opensearch/v11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/v11/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/v11/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/opensearch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.389521 EOxServer-1.3.2/eoxserver/services/ows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.393520 EOxServer-1.3.2/eoxserver/services/ows/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/common/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.393520 EOxServer-1.3.2/eoxserver/services/ows/common/v11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/common/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/common/v11/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.393520 EOxServer-1.3.2/eoxserver/services/ows/common/v20/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/common/v20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/common/v20/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/common/v20/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.393520 EOxServer-1.3.2/eoxserver/services/ows/dseo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/dseo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.393520 EOxServer-1.3.2/eoxserver/services/ows/dseo/v10/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/dseo/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/dseo/v10/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/dseo/v10/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.393520 EOxServer-1.3.2/eoxserver/services/ows/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/basehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.393520 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/describecoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/getcoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.397521 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/describecoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/getcoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.397521 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/describecoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/describeeocoverageset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29767 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.397521 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/encodings/geotiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/getcoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16676 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/geteocoverageset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.397521 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/packages/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/packages/zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13005 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wcs11Transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.397521 EOxServer-1.3.2/eoxserver/services/ows/wms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/basehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30194 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/layermapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.401521 EOxServer-1.3.2/eoxserver/services/ows/wms/v10/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v10/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v10/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v10/getfeatureinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v10/getmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v10/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.401521 EOxServer-1.3.2/eoxserver/services/ows/wms/v11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v11/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v11/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v11/getfeatureinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v11/getmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v11/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.401521 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getfeatureinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getlegendgraphic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wms/v13/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.401521 EOxServer-1.3.2/eoxserver/services/ows/wps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.405521 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10181 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/allowed_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/bboxdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/complexdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/literaldata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/response_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.405521 EOxServer-1.3.2/eoxserver/services/ows/wps/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_cloud_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_dem_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_height_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_time_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/test_allowed_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17124 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.405521 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/describeprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/execute_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/process_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_decoder_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_decoder_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v10/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/services/ows/wps/v20/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v20/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v20/describeprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v20/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/ows/wps/v20/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20079 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/subset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.345520 EOxServer-1.3.2/eoxserver/services/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/services/templates/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/templates/opensearch/result.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/templates/opensearch/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/services/templates/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/templates/wcs/error_template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/services/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/templatetags/services_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25514 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/services/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/testing/xcomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/webclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.409521 EOxServer-1.3.2/eoxserver/webclient/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/migrations/0002_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.413521 EOxServer-1.3.2/eoxserver/webclient/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   554482 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/static/5e3c304ea87541cabdab.worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127) 10119032 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/static/vsclient.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.345520 EOxServer-1.3.2/eoxserver/webclient/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.425521 EOxServer-1.3.2/eoxserver/webclient/templates/webclient/
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/templates/webclient/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-06-03 15:03:43.000000 EOxServer-1.3.2/eoxserver/webclient/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-03 15:03:43.000000 EOxServer-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-06-03 15:04:06.425521 EOxServer-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-03 15:03:43.000000 EOxServer-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 15:04:06.425521 EOxServer-1.3.2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14419 2024-06-03 15:03:43.000000 EOxServer-1.3.2/tools/eoxserver-atpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-06-03 15:03:43.000000 EOxServer-1.3.2/tools/eoxserver-preprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3435 2024-06-03 15:03:43.000000 EOxServer-1.3.2/tools/eoxserver-validate_xml.py
```

### Comparing `EOxServer-1.3.0/EOxServer.egg-info/PKG-INFO` & `EOxServer-1.3.2/EOxServer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOxServer
-Version: 1.3.0
+Version: 1.3.2
 Summary: EOxServer is a server for Earth Observation (EO) data
 Home-page: http://eoxserver.org/
 Author: EOX IT Services GmbH
 Author-email: office@eox.at
 Maintainer: EOX IT Services GmbH
 Maintainer-email: packages@eox.at
 License: EOxServer Open License (MIT-style)
```

### Comparing `EOxServer-1.3.0/EOxServer.egg-info/SOURCES.txt` & `EOxServer-1.3.2/EOxServer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/LICENSE` & `EOxServer-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/PKG-INFO` & `EOxServer-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOxServer
-Version: 1.3.0
+Version: 1.3.2
 Summary: EOxServer is a server for Earth Observation (EO) data
 Home-page: http://eoxserver.org/
 Author: EOX IT Services GmbH
 Author-email: office@eox.at
 Maintainer: EOX IT Services GmbH
 Maintainer-email: packages@eox.at
 License: EOxServer Open License (MIT-style)
```

### Comparing `EOxServer-1.3.0/README.md` & `EOxServer-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/__init__.py` & `EOxServer-1.3.2/eoxserver/core/commands/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-# ------------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
 #
 # Project: EOxServer <http://eoxserver.org>
 # Authors: Stephan Krause <stephan.krause@eox.at>
 #          Stephan Meissl <stephan.meissl@eox.at>
 #          Fabian Schindler <fabian.schindler@eox.at>
 #
-# ------------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
 # Copyright (C) 2011 EOX IT Services GmbH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
-# The above copyright notice and this permission notice shall be included in
-# all copies of this Software or works derived from this Software.
+# The above copyright notice and this permission notice shall be included in all
+# copies of this Software or works derived from this Software.
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-# ------------------------------------------------------------------------------
-
-
-__version__ = '1.3.0'
-
-
-def get_version():
-    return __version__
+#-------------------------------------------------------------------------------
```

### Comparing `EOxServer-1.3.0/eoxserver/backends/access.py` & `EOxServer-1.3.2/eoxserver/backends/access.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/admin.py` & `EOxServer-1.3.2/eoxserver/backends/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/cache.py` & `EOxServer-1.3.2/eoxserver/backends/cache.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/component.py` & `EOxServer-1.3.2/eoxserver/backends/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/config.py` & `EOxServer-1.3.2/eoxserver/backends/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/interfaces.py` & `EOxServer-1.3.2/eoxserver/backends/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/keystone/storage_auth.py` & `EOxServer-1.3.2/eoxserver/backends/keystone/storage_auth.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/management/commands/storage.py` & `EOxServer-1.3.2/eoxserver/backends/management/commands/storage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/management/commands/storageauth.py` & `EOxServer-1.3.2/eoxserver/backends/management/commands/storageauth.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/middleware.py` & `EOxServer-1.3.2/eoxserver/backends/middleware.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/migrations/0001_initial.py` & `EOxServer-1.3.2/eoxserver/backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/migrations/0002_storage_auth.py` & `EOxServer-1.3.2/eoxserver/backends/migrations/0002_storage_auth.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/migrations/0003_nameblank.py` & `EOxServer-1.3.2/eoxserver/backends/migrations/0003_nameblank.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/models.py` & `EOxServer-1.3.2/eoxserver/backends/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/storage_auths.py` & `EOxServer-1.3.2/eoxserver/backends/storage_auths.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/storages.py` & `EOxServer-1.3.2/eoxserver/backends/storages.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/testbase.py` & `EOxServer-1.3.2/eoxserver/backends/testbase.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/tests.py` & `EOxServer-1.3.2/eoxserver/backends/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/backends/util.py` & `EOxServer-1.3.2/eoxserver/backends/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/conf/default.conf` & `EOxServer-1.3.2/eoxserver/conf/default.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/conf/default_formats.conf` & `EOxServer-1.3.2/eoxserver/conf/default_formats.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/contrib/__init__.py` & `EOxServer-1.3.2/eoxserver/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/contrib/gdal.py` & `EOxServer-1.3.2/eoxserver/contrib/gdal.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/contrib/gdal_array.py` & `EOxServer-1.3.2/eoxserver/contrib/gdal_array.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/contrib/mapserver.py` & `EOxServer-1.3.2/eoxserver/contrib/mapserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 
 def set_env(map_obj, env, fail_on_override=False, return_old=False):
     old_values = {} if return_old else None
     for key, value in env.items():
         if fail_on_override or return_old:
             old_value = map_obj.getConfigOption(str(key))
             if fail_on_override and old_value is not None \
-                    and old_value != value:
+                    and old_value != value and old_value != 'None':
                 raise Exception(
                     'Would override previous value of %s: %s with %s'
                     % (key, old_value, value)
                 )
             elif old_value != value and return_old:
                 old_values[key] = old_value
```

### Comparing `EOxServer-1.3.0/eoxserver/contrib/ogr.py` & `EOxServer-1.3.2/eoxserver/contrib/ogr.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/contrib/osr.py` & `EOxServer-1.3.2/eoxserver/contrib/osr.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/contrib/vrt.py` & `EOxServer-1.3.2/eoxserver/contrib/vrt.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/contrib/vsi.py` & `EOxServer-1.3.2/eoxserver/contrib/vsi.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/__init__.py` & `EOxServer-1.3.2/eoxserver/core/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/commands/__init__.py` & `EOxServer-1.3.2/eoxserver/core/util/geotools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #-------------------------------------------------------------------------------
 #
 # Project: EOxServer <http://eoxserver.org>
 # Authors: Stephan Krause <stephan.krause@eox.at>
 #          Stephan Meissl <stephan.meissl@eox.at>
-#          Fabian Schindler <fabian.schindler@eox.at>
 #
 #-------------------------------------------------------------------------------
 # Copyright (C) 2011 EOX IT Services GmbH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -21,8 +20,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-#-------------------------------------------------------------------------------
+#-------------------------------------------------------------------------------
```

### Comparing `EOxServer-1.3.0/eoxserver/core/commands/create_instance.py` & `EOxServer-1.3.2/eoxserver/core/commands/create_instance.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/component.py` & `EOxServer-1.3.2/eoxserver/core/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/config.py` & `EOxServer-1.3.2/eoxserver/core/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/decoders/__init__.py` & `EOxServer-1.3.2/eoxserver/core/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/decoders/base.py` & `EOxServer-1.3.2/eoxserver/core/decoders/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/decoders/config.py` & `EOxServer-1.3.2/eoxserver/core/decoders/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/decoders/kvp.py` & `EOxServer-1.3.2/eoxserver/core/decoders/kvp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/decoders/xml.py` & `EOxServer-1.3.2/eoxserver/core/decoders/xml.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/instance.py` & `EOxServer-1.3.2/eoxserver/core/instance.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/management.py` & `EOxServer-1.3.2/eoxserver/core/management.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/models.py` & `EOxServer-1.3.2/eoxserver/core/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/templates/admin/change_confirmation.html` & `EOxServer-1.3.2/eoxserver/core/templates/admin/change_confirmation.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/templates/eoxserver_index.html` & `EOxServer-1.3.2/eoxserver/core/templates/eoxserver_index.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/templates/logging/logview.html` & `EOxServer-1.3.2/eoxserver/core/templates/logging/logview.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/tests.py` & `EOxServer-1.3.2/eoxserver/core/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/functools.py` & `EOxServer-1.3.2/eoxserver/core/util/functools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/geotools.py` & `EOxServer-1.3.2/eoxserver/core/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,7 +21,14 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #-------------------------------------------------------------------------------
+
+from django.shortcuts import render_to_response
+
+
+def index(request):
+    # show overview with links to active components, resources
+    return render_to_response("eoxserver/index.html")
```

### Comparing `EOxServer-1.3.0/eoxserver/core/util/importtools.py` & `EOxServer-1.3.2/eoxserver/core/util/importtools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/iteratortools.py` & `EOxServer-1.3.2/eoxserver/core/util/iteratortools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/multiparttools.py` & `EOxServer-1.3.2/eoxserver/core/util/multiparttools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/perftools.py` & `EOxServer-1.3.2/eoxserver/core/util/perftools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/rect.py` & `EOxServer-1.3.2/eoxserver/core/util/rect.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/timetools.py` & `EOxServer-1.3.2/eoxserver/core/util/timetools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/util/xmltools.py` & `EOxServer-1.3.2/eoxserver/core/util/xmltools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/core/views.py` & `EOxServer-1.3.2/eoxserver/processing/preprocessing/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #-------------------------------------------------------------------------------
 #
 # Project: EOxServer <http://eoxserver.org>
-# Authors: Stephan Krause <stephan.krause@eox.at>
-#          Stephan Meissl <stephan.meissl@eox.at>
+# Authors: Fabian Schindler <fabian.schindler@eox.at>
 #
 #-------------------------------------------------------------------------------
 # Copyright (C) 2011 EOX IT Services GmbH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -22,13 +21,13 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #-------------------------------------------------------------------------------
 
-from django.shortcuts import render_to_response
 
+class PreprocessingException(Exception):
+    pass
 
-def index(request):
-    # show overview with links to active components, resources
-    return render_to_response("eoxserver/index.html")
+class GCPTransformException(PreprocessingException):
+    pass
```

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/manage.py` & `EOxServer-1.3.2/eoxserver/instance_template/manage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/eoxserver.conf` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/eoxserver.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/formats.conf` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/formats.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/conf/outline_template_dataset.html` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/conf/outline_template_dataset.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/settings.py` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/settings.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/templates/admin/base_site.html` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/urls.py` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/instance_template/project_name/wsgi.py` & `EOxServer-1.3.2/eoxserver/instance_template/project_name/wsgi.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/media/images/eoxserver_logo.png` & `EOxServer-1.3.2/eoxserver/media/images/eoxserver_logo.png`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/media/images/eoxserver_logo_transparent.png` & `EOxServer-1.3.2/eoxserver/media/images/eoxserver_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/processing/gdal/reftools.py` & `EOxServer-1.3.2/eoxserver/processing/gdal/reftools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/processing/gdal/vrt.py` & `EOxServer-1.3.2/eoxserver/processing/gdal/vrt.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/processing/preprocessing/__init__.py` & `EOxServer-1.3.2/eoxserver/processing/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/processing/preprocessing/exceptions.py` & `EOxServer-1.3.2/eoxserver/services/auth/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #-------------------------------------------------------------------------------
 #
 # Project: EOxServer <http://eoxserver.org>
 # Authors: Fabian Schindler <fabian.schindler@eox.at>
 #
 #-------------------------------------------------------------------------------
-# Copyright (C) 2011 EOX IT Services GmbH
+# Copyright (C) 2013 EOX IT Services GmbH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,12 +22,12 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #-------------------------------------------------------------------------------
 
 
-class PreprocessingException(Exception):
-    pass
+class AuthorisationException(Exception):
+    """
+    """
 
-class GCPTransformException(PreprocessingException):
-    pass
+    code = "AccessForbidden"
```

### Comparing `EOxServer-1.3.0/eoxserver/processing/preprocessing/format.py` & `EOxServer-1.3.2/eoxserver/processing/preprocessing/format.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/processing/preprocessing/georeference.py` & `EOxServer-1.3.2/eoxserver/processing/preprocessing/georeference.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/processing/preprocessing/optimization.py` & `EOxServer-1.3.2/eoxserver/processing/preprocessing/optimization.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/processing/preprocessing/util.py` & `EOxServer-1.3.2/eoxserver/processing/preprocessing/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/browse/defaultstyles.py` & `EOxServer-1.3.2/eoxserver/render/browse/defaultstyles.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/browse/functions.py` & `EOxServer-1.3.2/eoxserver/render/browse/functions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/browse/generate.py` & `EOxServer-1.3.2/eoxserver/render/browse/generate.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/browse/objects.py` & `EOxServer-1.3.2/eoxserver/render/browse/objects.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/browse/util.py` & `EOxServer-1.3.2/eoxserver/render/browse/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/colors.py` & `EOxServer-1.3.2/eoxserver/render/colors.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/coverage/objects.py` & `EOxServer-1.3.2/eoxserver/render/coverage/objects.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/map/config.py` & `EOxServer-1.3.2/eoxserver/render/map/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/map/objects.py` & `EOxServer-1.3.2/eoxserver/render/map/objects.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/map/renderer.py` & `EOxServer-1.3.2/eoxserver/render/map/renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/mapserver/config.py` & `EOxServer-1.3.2/eoxserver/render/mapserver/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/mapserver/factories.py` & `EOxServer-1.3.2/eoxserver/render/mapserver/factories.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/render/mapserver/map_renderer.py` & `EOxServer-1.3.2/eoxserver/render/mapserver/map_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/admin.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/crss.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/crss.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/dateline.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/dateline.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/formats.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/formats.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/__init__.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/browse.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/browse.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/browsetype.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/browsetype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/collection.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/collection.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/collectiontype.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/collectiontype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/coverage.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/coverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/coveragetype.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/coveragetype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/grid.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/grid.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/id.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/id.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/mapcache.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/mapcache.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/mask.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/mask.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/masktype.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/masktype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/mosaic.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/mosaic.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/product.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/product.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/producttype.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/producttype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/rasterstyle.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/rasterstyle.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/stac.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/stac.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/management/commands/timeseries.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/management/commands/timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,52 +62,52 @@
         register_parser.add_argument(
             "--collection",
             "--collection-identifier",
             "-c",
             dest="collection",
             required=True,
             type=parse_collection,
-            help="Register timeseries for this collection",
+            help="Register timeseries for this collection.",
         )
         register_parser.add_argument(
             "--storage",
-            help="The storage to use",
+            help="The storage to use.",
         )
         register_parser.add_argument(
             "--path",
             required=True,
-            help="Path to timeseries file",
+            help="Path to timeseries file.",
         )
         register_parser.add_argument(
             "--product-type-name",
             required=True,
-            help="The product type name",
+            help="The product type name.",
         )
         register_parser.add_argument(
             "--coverage-type-mapping",
             action="append",
             type=parse_coverage_type_mapping,
             required=True,
             help="Which dimension to map to which coverage type. "
             'Use : as separator, e.g. --coverage-type-mapping "/Band1:b1"',
         )
         register_parser.add_argument(
             "--x-dim-name",
             required=True,
-            help="Name of the X dimension",
+            help="Name of the X dimension.",
         )
         register_parser.add_argument(
             "--y-dim-name",
             required=True,
-            help="Name of the Y dimension",
+            help="Name of the Y dimension.",
         )
         register_parser.add_argument(
             "--time-dim-name",
             required=True,
-            help="Name of the time dimension",
+            help="Name of the time dimension.",
         )
         register_parser.add_argument(
             "--product-template",
             required=True,
             help="Format string for product identifier. "
             "Can use the following template variables: "
             "collection_identifier, file_identifier, index, "
```

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/component.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/config.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/native.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/native.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/interfaces.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/__init__.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/gsc.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/gsc.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/utils/gsc.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/utils/gsc.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0001_initial.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0007_typemodels.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0007_typemodels.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0008_incidence_angle.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0008_incidence_angle.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0011_bandstatistics.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0011_bandstatistics.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/migrations/0013_raster_style.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/migrations/0013_raster_style.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/models.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/base.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/browse.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/browse.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/component.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/exceptions.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/interfaces.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/mask.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/mask.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/product.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/product.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/registrators/gdal.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/registrators/gdal.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/stac.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,17 +351,21 @@
             value = prep(raw_value)
             if isinstance(field_name, str):
                 metadata[field_name] = value
             else:
                 for name in field_name:
                     metadata[name] = value
 
-    # read footprint from metadata if it was not already defined
-    footprint = footprint or metadata.get('footprint')
-
+    if not footprint:
+        # read footprint from metadata if it was not already defined
+        footprint = metadata.get('footprint')
+        if footprint:
+            footprint = GEOSGeometry(footprint)
+    if footprint and not footprint.valid:
+        raise RegistrationError(f'Footprint is not valid {footprint}, reason {footprint.valid_reason}')
     if simplify_footprint_tolerance is not None and footprint:
         footprint = footprint.simplify(
             simplify_footprint_tolerance, preserve_topology=True
         )
 
     # finally create the product and its metadata object
     product = models.Product.objects.create(
```

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/registration/timeseries.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/registration/timeseries.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/synchronization.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/synchronization.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/tests.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/urls.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/util.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/resources/coverages/views.py` & `EOxServer-1.3.2/eoxserver/resources/coverages/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/scripts/eoxserver-instance.py` & `EOxServer-1.3.2/eoxserver/scripts/eoxserver-instance.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/admin.py` & `EOxServer-1.3.2/eoxserver/services/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/auth/base.py` & `EOxServer-1.3.2/eoxserver/services/auth/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/auth/charonpdp.py` & `EOxServer-1.3.2/eoxserver/services/auth/charonpdp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/auth/dummypdp.py` & `EOxServer-1.3.2/eoxserver/services/auth/dummypdp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/auth/exceptions.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_decoder_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #-------------------------------------------------------------------------------
 #
+#  Execute - common decoder subroutines
+#
 # Project: EOxServer <http://eoxserver.org>
 # Authors: Fabian Schindler <fabian.schindler@eox.at>
+#          Martin Paces <martin.paces@eox.at>
 #
 #-------------------------------------------------------------------------------
 # Copyright (C) 2013 EOX IT Services GmbH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -21,13 +24,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #-------------------------------------------------------------------------------
 
-
-class AuthorisationException(Exception):
-    """
-    """
-
-    code = "AccessForbidden"
+def parse_bool(raw_value):
+    """ Parse boolean value. """
+    if raw_value is None:
+        return None
+    elif raw_value == 'true':
+        return True
+    elif raw_value == 'false':
+        return False
+    else:
+        raise ValueError('Not a valid boolean value! %r' % raw_value)
```

### Comparing `EOxServer-1.3.0/eoxserver/services/auth/interfaces.py` & `EOxServer-1.3.2/eoxserver/services/auth/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/auth/middleware.py` & `EOxServer-1.3.2/eoxserver/services/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/cis/v11/encoders.py` & `EOxServer-1.3.2/eoxserver/services/cis/v11/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/config.py` & `EOxServer-1.3.2/eoxserver/services/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ecql.py` & `EOxServer-1.3.2/eoxserver/services/ecql.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/exceptions.py` & `EOxServer-1.3.2/eoxserver/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/filters.py` & `EOxServer-1.3.2/eoxserver/services/filters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py` & `EOxServer-1.3.2/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/gml/v32/encoders.py` & `EOxServer-1.3.2/eoxserver/services/gml/v32/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/management/commands/eoxs_filter.py` & `EOxServer-1.3.2/eoxserver/services/management/commands/eoxs_filter.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/management/commands/visibility.py` & `EOxServer-1.3.2/eoxserver/services/management/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/management/commands/wms_options_list.py` & `EOxServer-1.3.2/eoxserver/services/management/commands/wms_options_list.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/management/commands/wms_options_load.py` & `EOxServer-1.3.2/eoxserver/services/management/commands/wms_options_load.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/management/commands/wms_options_set.py` & `EOxServer-1.3.2/eoxserver/services/management/commands/wms_options_set.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/config.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/connectors/__init__.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/connectors/mosaic_connector.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/connectors/mosaic_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/connectors/multifile_connector.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/connectors/multifile_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/connectors/polygonmask_connector.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/connectors/polygonmask_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/connectors/simple_connector.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/connectors/simple_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/connectors/tileindex_connector.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/connectors/tileindex_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/interfaces.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wcs/base_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wcs/base_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,17 @@
 
         supported_crss = " ".join(all_crss)
         layer.setMetaData("ows_srs", supported_crss)
         layer.setMetaData("wcs_srs", supported_crss)
 
         for band in bands:
             ms.setMetaData(layer, {
-                "band_description": band.description,
-                "band_definition": band.definition,
-                "band_uom": band.unit_of_measure,
+                "band_description": band.description or '',
+                "band_definition": band.definition or '',
+                "band_uom": band.unit_of_measure or '',
             }, namespace=band.identifier)
 
             if band.allowed_values:
                 interval = band.allowed_values[0]
             else:
                 interval = gdal.GDT_NUMERIC_LIMITS[band.data_type]
```

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wcs/capabilities_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wcs/capabilities_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wcs/coverage_description_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wcs/coverage_description_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wcs/coverage_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wcs/coverage_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/capabilities_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/capabilities_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/feature_info_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/feature_info_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/base.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/legendgraphic_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/legendgraphic_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/map_renderer.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/map_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/styleapplicators/sld.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/styleapplicators/sld.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/mapserver/wms/util.py` & `EOxServer-1.3.2/eoxserver/services/mapserver/wms/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/migrations/0001_initial.py` & `EOxServer-1.3.2/eoxserver/services/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py` & `EOxServer-1.3.2/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/migrations/0003_service_name_choices.py` & `EOxServer-1.3.2/eoxserver/services/migrations/0003_service_name_choices.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/models.py` & `EOxServer-1.3.2/eoxserver/services/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/native/wcs/capabilities_renderer.py` & `EOxServer-1.3.2/eoxserver/services/native/wcs/capabilities_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/native/wcs/coverage_description_renderer.py` & `EOxServer-1.3.2/eoxserver/services/native/wcs/coverage_description_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/config.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/extensions/__init__.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/extensions/cql.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/extensions/cql.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/extensions/eo.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/extensions/eo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/extensions/geo.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/extensions/geo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/extensions/time.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/extensions/time.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/formats/__init__.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/formats/atom.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/formats/atom.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/formats/base.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/formats/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/formats/geojson.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/formats/geojson.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/formats/html.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/formats/html.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/formats/kml.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/formats/kml.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/formats/rss.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/formats/rss.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/interfaces.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/urls.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/v11/description.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/v11/description.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/v11/search.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/v11/search.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/opensearch/views.py` & `EOxServer-1.3.2/eoxserver/services/opensearch/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/common/config.py` & `EOxServer-1.3.2/eoxserver/services/ows/common/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/common/v11/encoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/common/v11/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/common/v20/encoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/common/v20/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/common/v20/exceptionhandler.py` & `EOxServer-1.3.2/eoxserver/services/ows/common/v20/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/component.py` & `EOxServer-1.3.2/eoxserver/services/ows/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/config.py` & `EOxServer-1.3.2/eoxserver/services/ows/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/decoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/decoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/dispatch.py` & `EOxServer-1.3.2/eoxserver/services/ows/dispatch.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/dseo/v10/encoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/dseo/v10/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/dseo/v10/handlers.py` & `EOxServer-1.3.2/eoxserver/services/ows/dseo/v10/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/interfaces.py` & `EOxServer-1.3.2/eoxserver/services/ows/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/version.py` & `EOxServer-1.3.2/eoxserver/services/ows/version.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/basehandlers.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/basehandlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/config.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/interfaces.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/parameters.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/renderers.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/renderers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/describecoverage.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/describecoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/exceptionhandler.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/getcoverage.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/getcoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/parameters.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v10/util.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v10/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/describecoverage.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/describecoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/exceptionhandler.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/getcoverage.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/getcoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/parameters.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v11/util.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v11/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/describecoverage.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/describecoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/describeeocoverageset.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/describeeocoverageset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/encoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/encoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,32 +414,32 @@
                 ]
             )
         )
 
     def encode_field(self, field):
         return SWE("field",
             SWE("Quantity",
-                SWE("description", field.description),
+                SWE("description", field.description or ''),
                 self.encode_nil_values(field.nil_values),
-                SWE("uom", code=field.unit_of_measure),
+                SWE("uom", code=field.unit_of_measure or ''),
                 SWE("constraint",
                     SWE("AllowedValues",
                         *[
                             SWE("interval", "%g %g" % value_range)
                             for value_range in field.allowed_values
                         ] + [
                             SWE("significantFigures", str(
                                 field.significant_figures
                             ))
                         ] if field.significant_figures else []
                     )
                 ),
                 # TODO: lookup correct definition according to data type:
                 # http://www.opengis.net/def/dataType/OGC/0/
-                definition=field.definition
+                definition=field.definition or ''
             ),
             name=field.identifier
         )
 
     def encode_range_type(self, range_type):
         return GMLCOV("rangeType",
             SWE("DataRecord",
```

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/encodings/__init__.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/encodings/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/encodings/geotiff.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/encodings/geotiff.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/exceptionhandler.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/getcoverage.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/getcoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/geteocoverageset.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/geteocoverageset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/handlers.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/packages/tar.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/packages/tar.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/packages/zip.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/packages/zip.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/parameters.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs/v20/util.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs/v20/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wcs11Transaction.py` & `EOxServer-1.3.2/eoxserver/services/ows/wcs11Transaction.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/basehandlers.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/basehandlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/exceptions.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/interfaces.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/layermapper.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/layermapper.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/parsing.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/parsing.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/util.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v10/encoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v10/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v10/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v10/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v10/getfeatureinfo.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v10/getfeatureinfo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v10/getmap.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v10/getmap.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v10/handlers.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v10/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v11/encoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v11/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v11/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v11/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v11/getfeatureinfo.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v11/getfeatureinfo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v11/getmap.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v11/getmap.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v11/handlers.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v11/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v13/encoders.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v13/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v13/exceptionhandler.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v13/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getfeatureinfo.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getfeatureinfo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getlegendgraphic.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getlegendgraphic.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v13/getmap.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v13/getmap.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wms/v13/handlers.py` & `EOxServer-1.3.2/eoxserver/services/ows/wms/v13/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/config.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/context.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/context.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/exceptions.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/interfaces.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/__init__.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/allowed_values.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/allowed_values.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/base.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/bboxdata.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/bboxdata.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/codecs.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/codecs.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/complexdata.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/complexdata.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/crs.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/crs.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/data_types.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/data_types.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/formats.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/formats.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/inputs.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/inputs.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/literaldata.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/literaldata.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/response_form.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/response_form.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/parameters/units.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/parameters/units.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_cloud_coverage.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_cloud_coverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_dem_processing.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_dem_processing.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_height_profile.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_height_profile.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_statistics.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 no_data_list = []
                 for no_data in nill_values:
                     no_data_list.append(np.sum(image_array == no_data))
                     data_array = data_array[data_array != no_data]
                 # if the image is empty GetStatistics will throw an error
                 # so we check if the number of the image pixels is greater
                 # than the number of noData pixels
-                nodata_number = sum(no_data_list).item()
+                nodata_number = np.sum(no_data_list).item()
                 if ((image_array.size - nodata_number) > 0):
                     stats = ds.GetRasterBand(band_number).GetStatistics(0, 1)
                     interval = (np.amax(data_array) - np.amin(data_array)) / 25
 
                     bin_array, hist = np.histogram(data_array, bins=np.arange(
                         int(stats[0]), int(stats[1]), interval, int))
```

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/processes/get_time_data.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/processes/get_time_data.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/test_allowed_values.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/test_allowed_values.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/test_data_types.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/test_data_types.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/util.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/describeprocess.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/describeprocess.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/__init__.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/base.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/capabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/capabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/execute_response.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/execute_response.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/parameters.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/encoders/process_description.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/encoders/process_description.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/exceptionhandler.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_decoder_common.py` & `EOxServer-1.3.2/eoxserver/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-#-------------------------------------------------------------------------------
-#
-#  Execute - common decoder subroutines
+# ------------------------------------------------------------------------------
 #
 # Project: EOxServer <http://eoxserver.org>
-# Authors: Fabian Schindler <fabian.schindler@eox.at>
-#          Martin Paces <martin.paces@eox.at>
+# Authors: Stephan Krause <stephan.krause@eox.at>
+#          Stephan Meissl <stephan.meissl@eox.at>
+#          Fabian Schindler <fabian.schindler@eox.at>
 #
-#-------------------------------------------------------------------------------
-# Copyright (C) 2013 EOX IT Services GmbH
+# ------------------------------------------------------------------------------
+# Copyright (C) 2011 EOX IT Services GmbH
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
-# The above copyright notice and this permission notice shall be included in all
-# copies of this Software or works derived from this Software.
+# The above copyright notice and this permission notice shall be included in
+# all copies of this Software or works derived from this Software.
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
-#-------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------
+
+
+__version__ = '1.3.2'
+
 
-def parse_bool(raw_value):
-    """ Parse boolean value. """
-    if raw_value is None:
-        return None
-    elif raw_value == 'true':
-        return True
-    elif raw_value == 'false':
-        return False
-    else:
-        raise ValueError('Not a valid boolean value! %r' % raw_value)
+def get_version():
+    return __version__
```

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_decoder_xml.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_decoder_xml.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/execute_util.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/execute_util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v10/util.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v10/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v20/common.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v20/common.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v20/describeprocess.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v20/describeprocess.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v20/execute.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v20/execute.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/ows/wps/v20/getcapabilities.py` & `EOxServer-1.3.2/eoxserver/services/ows/wps/v20/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/parameters.py` & `EOxServer-1.3.2/eoxserver/services/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/result.py` & `EOxServer-1.3.2/eoxserver/services/result.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/subset.py` & `EOxServer-1.3.2/eoxserver/services/subset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/templates/opensearch/result.html` & `EOxServer-1.3.2/eoxserver/services/templates/opensearch/result.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/templates/opensearch/summary.html` & `EOxServer-1.3.2/eoxserver/services/templates/opensearch/summary.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/templatetags/services_extra.py` & `EOxServer-1.3.2/eoxserver/services/templatetags/services_extra.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/tests.py` & `EOxServer-1.3.2/eoxserver/services/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/urls.py` & `EOxServer-1.3.2/eoxserver/services/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/services/views.py` & `EOxServer-1.3.2/eoxserver/services/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/testing/xcomp.py` & `EOxServer-1.3.2/eoxserver/testing/xcomp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/views.py` & `EOxServer-1.3.2/eoxserver/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/admin.py` & `EOxServer-1.3.2/eoxserver/webclient/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/migrations/0001_initial.py` & `EOxServer-1.3.2/eoxserver/webclient/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/migrations/0002_extra_fields.py` & `EOxServer-1.3.2/eoxserver/webclient/migrations/0002_extra_fields.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/models.py` & `EOxServer-1.3.2/eoxserver/webclient/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/static/5e3c304ea87541cabdab.worker.js` & `EOxServer-1.3.2/eoxserver/webclient/static/5e3c304ea87541cabdab.worker.js`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/static/favicon.ico` & `EOxServer-1.3.2/eoxserver/webclient/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/static/vsclient.js` & `EOxServer-1.3.2/eoxserver/webclient/static/vsclient.js`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/templates/webclient/index.html` & `EOxServer-1.3.2/eoxserver/webclient/templates/webclient/index.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/urls.py` & `EOxServer-1.3.2/eoxserver/webclient/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/eoxserver/webclient/views.py` & `EOxServer-1.3.2/eoxserver/webclient/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/setup.cfg` & `EOxServer-1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/setup.py` & `EOxServer-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/tools/eoxserver-atpd.py` & `EOxServer-1.3.2/tools/eoxserver-atpd.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/tools/eoxserver-preprocess.py` & `EOxServer-1.3.2/tools/eoxserver-preprocess.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.3.0/tools/eoxserver-validate_xml.py` & `EOxServer-1.3.2/tools/eoxserver-validate_xml.py`

 * *Files identical despite different names*

