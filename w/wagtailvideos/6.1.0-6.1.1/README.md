# Comparing `tmp/wagtailvideos-6.1.0.tar.gz` & `tmp/wagtailvideos-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailvideos-6.1.0.tar", last modified: Fri May 24 06:25:18 2024, max compression
+gzip compressed data, was "wagtailvideos-6.1.1.tar", last modified: Sun Jun  2 23:14:32 2024, max compression
```

## Comparing `wagtailvideos-6.1.0.tar` & `wagtailvideos-6.1.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.258856 wagtailvideos-6.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1481 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6037 2024-05-24 06:25:18.258856 wagtailvideos-6.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5051 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      295 2024-05-24 06:25:18.259856 wagtailvideos-6.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1332 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.240854 wagtailvideos-6.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.241854 wagtailvideos-6.1.0/tests/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.242854 wagtailvideos-6.1.0/tests/app/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    32355 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0002_alter_testpage_video_streamfield.py
--rw-rw-rw-   0 root         (0) root         (0)    27639 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/0004_customvideomodel_height_customvideomodel_width.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2210 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/test_block.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/app/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6455 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    26157 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/test_admin_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/test_custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/test_template_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.245854 wagtailvideos-6.1.0/wagtailvideos/
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/edit_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     2067 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3193 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/jinja2tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.235853 wagtailvideos-6.1.0/wagtailvideos/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.235853 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.247855 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9219 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13787 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.250855 wagtailvideos-6.1.0/wagtailvideos/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1966 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0002_auto_20160321_1610.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0003_auto_20160705_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0004_auto_20160706_1153.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0005_videotranscode_error_message.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0006_auto_20160707_1413.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0007_video_duration.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0008_auto_20160728_1523.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0009_videotranscode_quality.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0010_video_ordering.py
--rw-rw-rw-   0 root         (0) root         (0)    28229 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0011_video_tracks.py
--rw-rw-rw-   0 root         (0) root         (0)    26753 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0012_remove_unique_constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0013_add_choose_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    44986 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/0015_video_height_video_width.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10304 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/models.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2266 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.236853 wagtailvideos-6.1.0/wagtailvideos/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.236853 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.251855 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/css/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/css/edit-video.css
--rw-rw-rw-   0 root         (0) root         (0)      364 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/css/summary-override.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.252855 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/video-chooser.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.236853 wagtailvideos-6.1.0/wagtailvideos/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.237853 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.252855 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
--rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/results.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.252855 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/homepage/
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.253856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/
--rw-rw-rw-   0 root         (0) root         (0)     4414 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/add.html
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.237853 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/permissions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.253856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/permissions/includes/
--rw-rw-rw-   0 root         (0) root         (0)      253 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.255856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/add.html
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     7272 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/edit.html
--rw-rw-rw-   0 root         (0) root         (0)     1393 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/index.html
--rw-rw-rw-   0 root         (0) root         (0)     2019 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/results.html
--rw-rw-rw-   0 root         (0) root         (0)     1903 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.255856 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      442 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.255856 wagtailvideos-6.1.0/wagtailvideos/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/templatetags/wagtailvideos_tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.256856 wagtailvideos-6.1.0/wagtailvideos/transcoders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.256856 wagtailvideos-6.1.0/wagtailvideos/transcoders/base/
--rw-rw-rw-   0 root         (0) root         (0)     1307 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.256856 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     6982 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/ffmpeg.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.257856 wagtailvideos-6.1.0/wagtailvideos/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5285 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/chooser.py
--rw-rw-rw-   0 root         (0) root         (0)     4730 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/multiple.py
--rw-rw-rw-   0 root         (0) root         (0)     7760 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/views/videos.py
--rw-rw-rw-   0 root         (0) root         (0)     4295 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2024-05-24 06:25:09.000000 wagtailvideos-6.1.0/wagtailvideos/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:25:18.258856 wagtailvideos-6.1.0/wagtailvideos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6037 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3734 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-24 06:25:18.000000 wagtailvideos-6.1.0/wagtailvideos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.348492 wagtailvideos-6.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6037 2024-06-02 23:14:32.348492 wagtailvideos-6.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-06-02 23:14:32.349492 wagtailvideos-6.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1332 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.330492 wagtailvideos-6.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.331492 wagtailvideos-6.1.1/tests/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.332491 wagtailvideos-6.1.1/tests/app/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    32355 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/migrations/0002_alter_testpage_video_streamfield.py
+-rw-rw-rw-   0 root         (0) root         (0)    27639 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/migrations/0004_customvideomodel_height_customvideomodel_width.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2210 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/test_block.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/app/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6455 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    26157 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/test_admin_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/test_custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/test_template_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.335492 wagtailvideos-6.1.1/wagtailvideos/
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/edit_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/jinja2tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.325492 wagtailvideos-6.1.1/wagtailvideos/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.325492 wagtailvideos-6.1.1/wagtailvideos/locale/ru_RU/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.337492 wagtailvideos-6.1.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9219 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13787 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.340492 wagtailvideos-6.1.1/wagtailvideos/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0002_auto_20160321_1610.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0003_auto_20160705_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0004_auto_20160706_1153.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0005_videotranscode_error_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0006_auto_20160707_1413.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0007_video_duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0008_auto_20160728_1523.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0009_videotranscode_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0010_video_ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)    28229 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0011_video_tracks.py
+-rw-rw-rw-   0 root         (0) root         (0)    26753 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0012_remove_unique_constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0013_add_choose_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44986 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/0015_video_height_video_width.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10299 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.326492 wagtailvideos-6.1.1/wagtailvideos/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.326492 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.341492 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/css/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/css/edit-video.css
+-rw-rw-rw-   0 root         (0) root         (0)      364 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/css/summary-override.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.342491 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/js/
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/js/video-chooser-telepath.js
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/js/video-chooser.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.326492 wagtailvideos-6.1.1/wagtailvideos/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.327492 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.342491 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/chooser/
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/chooser/results.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.342491 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/homepage/
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.343492 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/multiple/
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/multiple/add.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.327492 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/permissions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.343492 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/permissions/includes/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/permissions/includes/video_permissions_formset.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.345492 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/_file_field.html
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/_file_field_as_li.html
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/add.html
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     7272 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/edit.html
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/results.html
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.345492 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/widgets/video_chooser.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.346492 wagtailvideos-6.1.1/wagtailvideos/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/templatetags/wagtailvideos_tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.346492 wagtailvideos-6.1.1/wagtailvideos/transcoders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/transcoders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.346492 wagtailvideos-6.1.1/wagtailvideos/transcoders/base/
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/transcoders/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.347492 wagtailvideos-6.1.1/wagtailvideos/transcoders/ffmpeg/
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/transcoders/ffmpeg/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/transcoders/ffmpeg/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     6977 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/transcoders/ffmpeg/ffmpeg.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.348492 wagtailvideos-6.1.1/wagtailvideos/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/views/chooser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4730 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/views/multiple.py
+-rw-rw-rw-   0 root         (0) root         (0)     7760 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/views/videos.py
+-rw-rw-rw-   0 root         (0) root         (0)     4295 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/wagtail_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2024-06-02 23:14:23.000000 wagtailvideos-6.1.1/wagtailvideos/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-02 23:14:32.348492 wagtailvideos-6.1.1/wagtailvideos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6037 2024-06-02 23:14:32.000000 wagtailvideos-6.1.1/wagtailvideos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3734 2024-06-02 23:14:32.000000 wagtailvideos-6.1.1/wagtailvideos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 23:14:32.000000 wagtailvideos-6.1.1/wagtailvideos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-02 23:14:32.000000 wagtailvideos-6.1.1/wagtailvideos.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2024-06-02 23:14:32.000000 wagtailvideos-6.1.1/wagtailvideos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-06-02 23:14:32.000000 wagtailvideos-6.1.1/wagtailvideos.egg-info/top_level.txt
```

### Comparing `wagtailvideos-6.1.0/LICENSE` & `wagtailvideos-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/PKG-INFO` & `wagtailvideos-6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 6.1.0
+Version: 6.1.1
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtailvideos-6.1.0/README.rst` & `wagtailvideos-6.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/setup.py` & `wagtailvideos-6.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.rst", "r") as f:
     readme = f.read()
 
 from setuptools import find_packages, setup  # noqa: E4
 
 setup(
     name="wagtailvideos",
-    version="6.1.0",
+    version="6.1.1",
     description="A wagtail module for uploading and displaying videos in various codecs.",
     long_description=readme,
     author="Neon Jungle",
     author_email="developers@neonjungle.studio",
     url="https://github.com/neon-jungle/wagtailvideos",
     install_requires=[
         "wagtail>=5.2",
```

### Comparing `wagtailvideos-6.1.0/tests/app/migrations/0001_initial.py` & `wagtailvideos-6.1.1/tests/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py` & `wagtailvideos-6.1.1/tests/app/migrations/0003_alter_customvideotrack_file_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/app/migrations/0004_customvideomodel_height_customvideomodel_width.py` & `wagtailvideos-6.1.1/tests/app/migrations/0004_customvideomodel_height_customvideomodel_width.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/app/models.py` & `wagtailvideos-6.1.1/tests/app/models.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/app/settings.py` & `wagtailvideos-6.1.1/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/app/test_block.py` & `wagtailvideos-6.1.1/tests/app/test_block.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/app/urls.py` & `wagtailvideos-6.1.1/tests/app/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/storage.py` & `wagtailvideos-6.1.1/tests/storage.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/test_admin_views.py` & `wagtailvideos-6.1.1/tests/test_admin_views.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/test_custom_model.py` & `wagtailvideos-6.1.1/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/tests/test_template_tag.py` & `wagtailvideos-6.1.1/tests/test_template_tag.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/__init__.py` & `wagtailvideos-6.1.1/wagtailvideos/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/apps.py` & `wagtailvideos-6.1.1/wagtailvideos/apps.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/blocks.py` & `wagtailvideos-6.1.1/wagtailvideos/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/enums.py` & `wagtailvideos-6.1.1/wagtailvideos/enums.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/fields.py` & `wagtailvideos-6.1.1/wagtailvideos/fields.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/forms.py` & `wagtailvideos-6.1.1/wagtailvideos/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/jinja2tags.py` & `wagtailvideos-6.1.1/wagtailvideos/jinja2tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo` & `wagtailvideos-6.1.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po` & `wagtailvideos-6.1.1/wagtailvideos/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0001_initial.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0002_auto_20160321_1610.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0002_auto_20160321_1610.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0003_auto_20160705_1646.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0003_auto_20160705_1646.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0004_auto_20160706_1153.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0004_auto_20160706_1153.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0006_auto_20160707_1413.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0006_auto_20160707_1413.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0009_videotranscode_quality.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0009_videotranscode_quality.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0011_video_tracks.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0011_video_tracks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0012_remove_unique_constraint.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0012_remove_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0013_add_choose_permissions.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0013_add_choose_permissions.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0014_alter_videotrack_file_alter_videotrack_kind_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/migrations/0015_video_height_video_width.py` & `wagtailvideos-6.1.1/wagtailvideos/migrations/0015_video_height_video_width.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/models.py` & `wagtailvideos-6.1.1/wagtailvideos/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             attrs = attrs.copy()
         if self.thumbnail:
             attrs['poster'] = self.thumbnail.url
 
         transcodes = self.get_current_transcodes()
         sources = []
         for transcode in transcodes:
-            sources.append("<source src='{0}' type='video/{1}' >".format(transcode.url, transcode.media_format.name))
+            sources.append("<source src='{0}' type='video/{1}' >".format(transcode.url, transcode.media_format))
 
         sources.append("<source src='{0}' type='{1}'>"
                        .format(self.url, self.content_type))
 
         sources.append("<p>Sorry, your browser doesn't support playback for this video</p>")
 
         return mark_safe(
```

### Comparing `wagtailvideos-6.1.0/wagtailvideos/signals.py` & `wagtailvideos-6.1.1/wagtailvideos/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/static/wagtailvideos/js/add-multiple.js` & `wagtailvideos-6.1.1/wagtailvideos/static/wagtailvideos/js/add-multiple.js`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/chooser.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/chooser/chooser.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/chooser/results.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/chooser/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/homepage/videos_summary.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/add.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/multiple/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/multiple/edit_form.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/add.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/add.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/edit.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/edit.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/index.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/index.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/results.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/results.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templates/wagtailvideos/videos/usage.html` & `wagtailvideos-6.1.1/wagtailvideos/templates/wagtailvideos/videos/usage.html`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/templatetags/wagtailvideos_tags.py` & `wagtailvideos-6.1.1/wagtailvideos/templatetags/wagtailvideos_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/transcoders/base/__init__.py` & `wagtailvideos-6.1.1/wagtailvideos/transcoders/base/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/__init__.py` & `wagtailvideos-6.1.1/wagtailvideos/transcoders/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/checks.py` & `wagtailvideos-6.1.1/wagtailvideos/transcoders/ffmpeg/checks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/transcoders/ffmpeg/ffmpeg.py` & `wagtailvideos-6.1.1/wagtailvideos/transcoders/ffmpeg/ffmpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                 "Invalid input_file value {0} for file {1}".format(
                     input_file, video.file
                 )
             )
 
         output_dir = tempfile.mkdtemp()
         transcode_name = "{0}.{1}".format(
-            video.filename(include_ext=False), media_format.name
+            video.filename(include_ext=False), media_format
         )
 
         output_file = os.path.join(output_dir, transcode_name)
         ffmpeg_cmd = self._get_ffmpeg_command(
             input_file, output_file, media_format, self.transcode.quality
         )
         try:
```

### Comparing `wagtailvideos-6.1.0/wagtailvideos/urls.py` & `wagtailvideos-6.1.1/wagtailvideos/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/views/chooser.py` & `wagtailvideos-6.1.1/wagtailvideos/views/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/views/multiple.py` & `wagtailvideos-6.1.1/wagtailvideos/views/multiple.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/views/videos.py` & `wagtailvideos-6.1.1/wagtailvideos/views/videos.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/wagtail_hooks.py` & `wagtailvideos-6.1.1/wagtailvideos/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos/widgets.py` & `wagtailvideos-6.1.1/wagtailvideos/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtailvideos-6.1.0/wagtailvideos.egg-info/PKG-INFO` & `wagtailvideos-6.1.1/wagtailvideos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailvideos
-Version: 6.1.0
+Version: 6.1.1
 Summary: A wagtail module for uploading and displaying videos in various codecs.
 Home-page: https://github.com/neon-jungle/wagtailvideos
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtailvideos-6.1.0/wagtailvideos.egg-info/SOURCES.txt` & `wagtailvideos-6.1.1/wagtailvideos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

