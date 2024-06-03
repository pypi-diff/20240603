# Comparing `tmp/simpledomcontrol-0.4.8.tar.gz` & `tmp/simpledomcontrol-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpledomcontrol-0.4.8.tar", max compression
+gzip compressed data, was "simpledomcontrol-0.5.0.tar", max compression
```

## Comparing `simpledomcontrol-0.4.8.tar` & `simpledomcontrol-0.5.0.tar`

### file list

```diff
@@ -1,167 +1,130 @@
--rwxr-xr-x   0        0        0       18 2023-09-13 12:39:11.659921 simpledomcontrol-0.4.8/README.md
--rwxr-xr-x   0        0        0     1082 2023-12-15 08:45:39.702665 simpledomcontrol-0.4.8/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.166975 simpledomcontrol-0.4.8/sdc_core/__init__.py
--rwxr-xr-x   0        0        0       98 2023-09-21 08:45:54.656855 simpledomcontrol-0.4.8/sdc_core/apps.py
--rw-r--r--   0        0        0    18645 2023-12-13 14:34:04.092799 simpledomcontrol-0.4.8/sdc_core/consumers.py
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/__init__.py
--rw-r--r--   0        0        0      164 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      176 2023-04-04 08:09:48.092720 simpledomcontrol-0.4.8/sdc_core/management/__pycache__/__init__.cpython-39.pyc
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/commands/__init__.py
--rw-r--r--   0        0        0      173 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      185 2023-04-04 08:09:48.092720 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      185 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/_private.cpython-39.pyc
--rw-r--r--   0        0        0     3111 2023-11-16 20:41:41.244279 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_cc.cpython-310.pyc
--rw-r--r--   0        0        0     3235 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_cc.cpython-39.pyc
--rw-r--r--   0        0        0     3278 2023-11-15 14:57:12.955993 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_controller_infos.cpython-310.pyc
--rw-r--r--   0        0        0      967 2023-11-15 07:20:44.934088 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_controller_url.cpython-310.pyc
--rw-r--r--   0        0        0     2669 2023-11-07 13:16:56.062974 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_get_model_infos.cpython-310.pyc
--rw-r--r--   0        0        0     2302 2023-11-24 09:37:56.060620 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_init.cpython-310.pyc
--rw-r--r--   0        0        0     2368 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_init.cpython-39.pyc
--rw-r--r--   0        0        0     2777 2023-11-16 20:24:39.232107 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-310.pyc
--rw-r--r--   0        0        0     2785 2023-04-04 10:33:03.270414 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_new_model.cpython-39.pyc
--rw-r--r--   0        0        0     3134 2023-11-24 08:07:05.791278 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_links.cpython-310.pyc
--rw-r--r--   0        0        0     2033 2023-09-21 08:46:16.872860 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-310.pyc
--rw-r--r--   0        0        0     2048 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_url.cpython-39.pyc
--rw-r--r--   0        0        0     5905 2023-03-31 13:46:19.184969 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-310.pyc
--rw-r--r--   0        0        0     5940 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/__pycache__/sdc_update_version.cpython-39.pyc
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/commands/_private.py
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.170975 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__init__.py
--rw-r--r--   0        0        0      182 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      194 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8592 2023-11-24 08:07:06.275254 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-310.pyc
--rw-r--r--   0        0        0     8033 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_controller_manager.cpython-39.pyc
--rw-r--r--   0        0        0     4225 2023-09-21 08:46:16.120859 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-310.pyc
--rw-r--r--   0        0        0     4205 2023-04-04 10:50:54.427002 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/add_model_manager.cpython-39.pyc
--rw-r--r--   0        0        0     1515 2023-09-14 07:32:05.321797 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/options.cpython-310.pyc
--rw-r--r--   0        0        0     1545 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/options.cpython-39.pyc
--rw-r--r--   0        0        0     1793 2023-09-21 08:46:13.508859 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2023-04-04 08:09:48.096721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/sdc_core_manager.cpython-39.pyc
--rw-r--r--   0        0        0     4789 2023-11-16 20:45:13.741182 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-310.pyc
--rw-r--r--   0        0        0     4479 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/settings_manager.cpython-39.pyc
--rw-r--r--   0        0        0     2641 2023-09-14 07:32:05.325796 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     2665 2023-04-04 08:09:48.100721 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/__pycache__/utils.cpython-39.pyc
--rwxr-xr-x   0        0        0    11256 2023-11-24 06:39:15.995849 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_controller_manager.py
--rw-r--r--   0        0        0     4591 2023-09-21 08:45:54.636855 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_model_manager.py
--rwxr-xr-x   0        0        0     1217 2023-09-14 07:16:20.174975 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/options.py
--rwxr-xr-x   0        0        0     1889 2023-09-21 08:45:54.644855 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/sdc_core_manager.py
--rwxr-xr-x   0        0        0     4472 2023-11-16 20:45:12.821178 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/settings_manager.py
--rwxr-xr-x   0        0        0     2157 2023-09-14 07:16:20.174975 simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/utils.py
--rwxr-xr-x   0        0        0     3251 2023-11-16 20:25:56.852389 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_cc.py
--rw-r--r--   0        0        0     3694 2023-11-15 14:56:59.559480 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_controller_infos.py
--rw-r--r--   0        0        0      507 2023-11-15 07:20:42.554086 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_controller_url.py
--rw-r--r--   0        0        0     2665 2023-11-07 13:16:45.855370 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_model_infos.py
--rwxr-xr-x   0        0        0     2711 2023-11-24 09:32:19.797721 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_init.py
--rw-r--r--   0        0        0      703 2023-10-12 09:29:35.938805 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_is_installed.py
--rwxr-xr-x   0        0        0     2642 2023-11-16 20:24:23.716052 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_new_model.py
--rwxr-xr-x   0        0        0     3608 2023-11-24 06:25:48.207532 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_links.py
--rwxr-xr-x   0        0        0     1933 2023-09-21 08:45:54.588855 simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_url.py
--rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__init__.py
--rw-r--r--   0        0        0      165 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1322 2023-09-21 08:46:16.496859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/forms.cpython-310.pyc
--rw-r--r--   0        0        0      605 2023-11-15 08:32:34.682753 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/import_manager.cpython-310.pyc
--rw-r--r--   0        0        0     2508 2023-10-11 13:59:42.076794 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     2201 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/response.cpython-310.pyc
--rw-r--r--   0        0        0     1280 2023-09-21 08:46:16.496859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/search.cpython-310.pyc
--rw-r--r--   0        0        0     2597 2023-09-21 08:46:13.852859 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/__pycache__/views.cpython-310.pyc
--rwxr-xr-x   0        0        0     1174 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/forms.py
--rwxr-xr-x   0        0        0      399 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/import_manager.py
--rw-r--r--   0        0        0     2234 2023-10-11 13:59:37.053640 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/models.py
--rwxr-xr-x   0        0        0     2458 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/response.py
--rwxr-xr-x   0        0        0     1838 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/search.py
--rwxr-xr-x   0        0        0     2380 2023-09-21 08:45:54.668855 simpledomcontrol-0.4.8/sdc_core/sdc_extentions/views.py
--rw-r--r--   0        0        0      107 2023-12-12 08:17:05.980843 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/.babelrc
--rw-r--r--   0        0        0     4673 2023-12-15 08:40:53.567934 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/gulpfile.jsx
--rwxr-xr-x   0        0        0      399 2023-12-12 12:31:17.861882 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/src/index.organizer.js
--rw-r--r--   0        0        0      324 2023-11-24 09:54:39.300747 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/src/index.style.scss
--rw-r--r--   0        0        0      429 2023-11-24 09:34:33.772197 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/tests/pre-test-setup.js
--rw-r--r--   0        0        0      212 2023-12-12 12:31:17.893882 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/tests/test-setup.js
--rw-r--r--   0        0        0     1139 2023-09-22 07:43:59.149945 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx
--rw-r--r--   0        0        0      432 2023-09-22 07:54:08.342934 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.development.config.jsx
--rw-r--r--   0        0        0      677 2023-09-22 07:54:40.070948 simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx
--rwxr-xr-x   0        0        0     1228 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt
--rwxr-xr-x   0        0        0     2464 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/index.html
--rwxr-xr-x   0        0        0     2328 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/server_call.txt
--rwxr-xr-x   0        0        0      895 2023-11-17 10:42:24.806725 simpledomcontrol-0.4.8/sdc_core/template_files/asgi.py.txt
--rwxr-xr-x   0        0        0       82 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/controller/templade_view.html
--rwxr-xr-x   0        0        0     1337 2023-12-12 12:31:17.885882 simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_controller.js.txt
--rwxr-xr-x   0        0        0       18 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_css.scss
--rw-r--r--   0        0        0      535 2023-11-24 10:09:44.297249 simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_test.js.text
--rw-r--r--   0        0        0      278 2023-12-12 12:31:17.897882 simpledomcontrol-0.4.8/sdc_core/template_files/js_test.js.txt
--rw-r--r--   0        0        0     1633 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/models/detail.html
--rw-r--r--   0        0        0     2303 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/models/list.html
--rwxr-xr-x   0        0        0     1635 2023-12-15 08:45:07.802861 simpledomcontrol-0.4.8/sdc_core/template_files/package.json
--rwxr-xr-x   0        0        0      357 2023-09-21 08:45:54.596855 simpledomcontrol-0.4.8/sdc_core/template_files/routing.py.txt
--rwxr-xr-x   0        0        0      149 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/sdc_urls.py.txt
--rwxr-xr-x   0        0        0       90 2023-09-21 08:45:54.608855 simpledomcontrol-0.4.8/sdc_core/template_files/sdc_views.py.txt
--rwxr-xr-x   0        0        0      936 2023-11-24 11:35:47.297156 simpledomcontrol-0.4.8/sdc_core/template_files/settings_extension.py.txt
--rwxr-xr-x   0        0        0      989 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/templates/base.html
--rwxr-xr-x   0        0        0      427 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/templates/index.html
--rwxr-xr-x   0        0        0      289 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_core/template_files/urls.py.txt
--rw-r--r--   0        0        0     2847 2023-12-12 12:31:17.821882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js
--rw-r--r--   0        0        0     1178 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss
--rw-r--r--   0        0        0     2454 2023-12-12 12:31:17.869882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js
--rw-r--r--   0        0        0     1833 2023-12-12 12:31:17.901882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js
--rw-r--r--   0        0        0       23 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.scss
--rw-r--r--   0        0        0     1318 2023-12-12 12:31:17.793882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js
--rw-r--r--   0        0        0       17 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.scss
--rw-r--r--   0        0        0     3046 2023-12-13 13:46:40.556259 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js
--rw-r--r--   0        0        0      103 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.scss
--rw-r--r--   0        0        0     3267 2023-12-12 12:31:17.909881 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js
--rw-r--r--   0        0        0      180 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.scss
--rw-r--r--   0        0        0     1457 2023-12-12 12:31:17.829882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js
--rw-r--r--   0        0        0    20079 2023-12-13 15:05:52.501451 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js
--rw-r--r--   0        0        0     1019 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss
--rw-r--r--   0        0        0     4914 2023-12-12 12:31:17.837882 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js
--rw-r--r--   0        0        0     2238 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss
--rw-r--r--   0        0        0     2819 2023-12-12 12:31:17.961881 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js
--rw-r--r--   0        0        0      668 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js
--rw-r--r--   0        0        0      364 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/sdc_tools.style.scss
--rw-r--r--   0        0        0      462 2023-12-12 12:31:17.945881 simpledomcontrol-0.4.8/sdc_tools/Assets/tests/sdc_tools.test.js
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_tools/__init__.py
--rwxr-xr-x   0        0        0       66 2023-09-14 07:16:20.198976 simpledomcontrol-0.4.8/sdc_tools/admin.py
--rwxr-xr-x   0        0        0       97 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/apps.py
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/migrations/__init__.py
--rw-r--r--   0        0        0      233 2023-09-14 07:34:03.056641 simpledomcontrol-0.4.8/sdc_tools/migrations/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0       60 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/models.py
--rwxr-xr-x   0        0        0      804 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/sdc_urls.py
--rwxr-xr-x   0        0        0     1485 2023-09-21 08:45:54.640855 simpledomcontrol-0.4.8/sdc_tools/sdc_views.py
--rwxr-xr-x   0        0        0     2110 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/elements/form.html
--rwxr-xr-x   0        0        0     1866 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/elements/inline_form.html
--rwxr-xr-x   0        0        0     1132 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/email/base.html
--rw-r--r--   0        0        0      399 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_alert_messenger.html
--rw-r--r--   0        0        0       36 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_detail_view.html
--rw-r--r--   0        0        0      136 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_error.html
--rw-r--r--   0        0        0       37 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_list_view.html
--rw-r--r--   0        0        0      338 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_model_form.html
--rwxr-xr-x   0        0        0      141 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_navigator.html
--rw-r--r--   0        0        0      496 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templates/sdc_tools/sdc/sdc_search_view.html
--rwxr-xr-x   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/__init__.py
--rw-r--r--   0        0        0      164 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1061 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/addclass.cpython-310.pyc
--rw-r--r--   0        0        0      667 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/indexfilter.cpython-310.pyc
--rw-r--r--   0        0        0     1481 2023-09-14 07:32:05.881810 simpledomcontrol-0.4.8/sdc_tools/templatetags/__pycache__/sdc_filter.cpython-310.pyc
--rwxr-xr-x   0        0        0      825 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/addclass.py
--rwxr-xr-x   0        0        0      357 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/indexfilter.py
--rwxr-xr-x   0        0        0     1135 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/templatetags/sdc_filter.py
--rwxr-xr-x   0        0        0       63 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/tests.py
--rwxr-xr-x   0        0        0       66 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_tools/views.py
--rw-r--r--   0        0        0     1453 2023-12-12 12:31:17.865882 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js
--rw-r--r--   0        0        0       17 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.scss
--rw-r--r--   0        0        0     1424 2023-12-12 12:31:17.797882 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js
--rw-r--r--   0        0        0       18 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.scss
--rw-r--r--   0        0        0      110 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/sdc_user.organizer.js
--rw-r--r--   0        0        0       49 2023-09-21 07:23:01.967412 simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/sdc_user.style.scss
--rw-r--r--   0        0        0      456 2023-12-12 12:31:17.813882 simpledomcontrol-0.4.8/sdc_user/Assets/tests/sdc_user.test.js
--rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/__init__.py
--rw-r--r--   0        0        0       63 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/admin.py
--rw-r--r--   0        0        0      147 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/apps.py
--rw-r--r--   0        0        0        0 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/migrations/__init__.py
--rw-r--r--   0        0        0      232 2023-09-14 07:34:03.060642 simpledomcontrol-0.4.8/sdc_user/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0       57 2023-09-14 07:16:20.202976 simpledomcontrol-0.4.8/sdc_user/models.py
--rw-r--r--   0        0        0      304 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/sdc_urls.py
--rw-r--r--   0        0        0     2140 2023-09-21 08:45:54.648855 simpledomcontrol-0.4.8/sdc_user/sdc_views.py
--rw-r--r--   0        0        0      401 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/templates/sdc_user/sdc/sdc_login.html
--rw-r--r--   0        0        0      327 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/templates/sdc_user/sdc/sdc_logout.html
--rw-r--r--   0        0        0       60 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/tests.py
--rw-r--r--   0        0        0       63 2023-09-14 07:16:20.206976 simpledomcontrol-0.4.8/sdc_user/views.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 simpledomcontrol-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.0/README.md
+-rw-r--r--   0        0        0     1125 2024-05-26 04:43:06.816129 simpledomcontrol-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/__init__.py
+-rw-r--r--   0        0        0     1263 2024-02-02 09:59:54.494456 simpledomcontrol-0.5.0/sdc_core/apps.py
+-rw-r--r--   0        0        0    19588 2024-05-26 11:28:08.009889 simpledomcontrol-0.5.0/sdc_core/consumers.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/_private.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/__init__.py
+-rw-r--r--   0        0        0    11002 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_controller_manager.py
+-rw-r--r--   0        0        0     4590 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_model_manager.py
+-rw-r--r--   0        0        0     1177 2024-02-06 09:19:01.417955 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/options.py
+-rw-r--r--   0        0        0     1839 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/sdc_core_manager.py
+-rw-r--r--   0        0        0     5116 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/settings_manager.py
+-rw-r--r--   0        0        0     2077 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/utils.py
+-rw-r--r--   0        0        0     3175 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_cc.py
+-rw-r--r--   0        0        0     3594 2024-01-17 13:18:27.055931 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_controller_infos.py
+-rw-r--r--   0        0        0      507 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_controller_url.py
+-rw-r--r--   0        0        0     2665 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_model_infos.py
+-rw-r--r--   0        0        0     2650 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_init.py
+-rw-r--r--   0        0        0      703 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_is_installed.py
+-rw-r--r--   0        0        0     2579 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_new_model.py
+-rw-r--r--   0        0        0     1301 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_shell_execute_script.py
+-rw-r--r--   0        0        0     3677 2024-01-17 11:51:17.421303 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_links.py
+-rw-r--r--   0        0        0     1884 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_url.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/__init__.py
+-rw-r--r--   0        0        0     1149 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/forms.py
+-rw-r--r--   0        0        0      382 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/import_manager.py
+-rw-r--r--   0        0        0     2234 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/models.py
+-rw-r--r--   0        0        0     4116 2024-03-05 13:01:15.459889 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/response.py
+-rw-r--r--   0        0        0     1790 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/search.py
+-rw-r--r--   0        0        0     3975 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/views.py
+-rw-r--r--   0        0        0      106 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/.babelrc
+-rw-r--r--   0        0        0     1233 2024-02-05 09:28:14.910183 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/gulpfile.jsx
+-rw-r--r--   0        0        0      472 2024-01-19 06:04:45.704481 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/src/index.organizer.js
+-rw-r--r--   0        0        0      324 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/src/index.style.scss
+-rw-r--r--   0        0        0      196 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/tests/config/post-test-teardown.js
+-rw-r--r--   0        0        0     3212 2024-02-02 10:22:46.579597 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/tests/config/pre-test-setup.js
+-rw-r--r--   0        0        0      306 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/tests/config/test-setup.js
+-rw-r--r--   0        0        0     1278 2024-02-05 08:23:47.706252 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx
+-rw-r--r--   0        0        0      320 2024-02-05 08:34:24.715149 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.development.config.jsx
+-rw-r--r--   0        0        0      543 2024-02-05 08:34:24.711149 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx
+-rw-r--r--   0        0        0     1191 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt
+-rw-r--r--   0        0        0     2414 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/index.html
+-rw-r--r--   0        0        0     2253 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/server_call.txt
+-rw-r--r--   0        0        0      865 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/asgi.py.txt
+-rw-r--r--   0        0        0       80 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/templade_view.html
+-rw-r--r--   0        0        0     1293 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_controller.js.txt
+-rw-r--r--   0        0        0       15 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_css.scss
+-rw-r--r--   0        0        0      535 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_test.js.text
+-rw-r--r--   0        0        0      241 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/js_test.js.txt
+-rw-r--r--   0        0        0     1633 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/models/detail.html
+-rw-r--r--   0        0        0     2303 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/models/list.html
+-rw-r--r--   0        0        0     2109 2024-05-26 04:43:06.784130 simpledomcontrol-0.5.0/sdc_core/template_files/package.json
+-rw-r--r--   0        0        0      349 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/routing.py.txt
+-rw-r--r--   0        0        0      141 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/sdc_urls.py.txt
+-rw-r--r--   0        0        0       87 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/sdc_views.py.txt
+-rw-r--r--   0        0        0      898 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/settings_extension.py.txt
+-rw-r--r--   0        0        0      957 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/templates/base.html
+-rw-r--r--   0        0        0      405 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/templates/index.html
+-rw-r--r--   0        0        0      281 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/urls.py.txt
+-rw-r--r--   0        0        0     2928 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js
+-rw-r--r--   0        0        0     1178 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss
+-rw-r--r--   0        0        0     2454 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js
+-rw-r--r--   0        0        0     1833 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js
+-rw-r--r--   0        0        0       23 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.scss
+-rw-r--r--   0        0        0     1473 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.js
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.scss
+-rw-r--r--   0        0        0     1387 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.scss
+-rw-r--r--   0        0        0     3165 2024-03-26 11:21:21.381111 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js
+-rw-r--r--   0        0        0      103 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.scss
+-rw-r--r--   0        0        0     3273 2024-03-13 08:30:43.081304 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js
+-rw-r--r--   0        0        0      180 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.scss
+-rw-r--r--   0        0        0     1457 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js
+-rw-r--r--   0        0        0    21405 2024-05-13 11:54:22.067553 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js
+-rw-r--r--   0        0        0     1019 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss
+-rw-r--r--   0        0        0     4914 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js
+-rw-r--r--   0        0        0     2238 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss
+-rw-r--r--   0        0        0     2819 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js
+-rw-r--r--   0        0        0      722 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js
+-rw-r--r--   0        0        0      413 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/sdc_tools.style.scss
+-rw-r--r--   0        0        0     6930 2024-03-13 07:55:56.619058 simpledomcontrol-0.5.0/sdc_tools/Assets/tests/sdc_tools.test.js
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/__init__.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/admin.py
+-rw-r--r--   0        0        0       92 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/apps.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/models.py
+-rw-r--r--   0        0        0      884 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/sdc_urls.py
+-rw-r--r--   0        0        0     1618 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/sdc_views.py
+-rw-r--r--   0        0        0     1192 2024-04-16 07:32:46.011283 simpledomcontrol-0.5.0/sdc_tools/templates/elements/form.html
+-rw-r--r--   0        0        0     1030 2024-04-16 07:43:06.313233 simpledomcontrol-0.5.0/sdc_tools/templates/elements/inline_form.html
+-rw-r--r--   0        0        0     1075 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/email/base.html
+-rw-r--r--   0        0        0       65 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/dummy_sdc.html
+-rw-r--r--   0        0        0      399 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_alert_messenger.html
+-rw-r--r--   0        0        0       36 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_detail_view.html
+-rw-r--r--   0        0        0      179 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_dummy.html
+-rw-r--r--   0        0        0      135 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_error.html
+-rw-r--r--   0        0        0       37 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_list_view.html
+-rw-r--r--   0        0        0      338 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_model_form.html
+-rw-r--r--   0        0        0      207 2024-03-05 12:33:59.397833 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_navigator.html
+-rw-r--r--   0        0        0      496 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_search_view.html
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/__init__.py
+-rw-r--r--   0        0        0      800 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/addclass.py
+-rw-r--r--   0        0        0      341 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/indexfilter.py
+-rw-r--r--   0        0        0     1092 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/sdc_filter.py
+-rw-r--r--   0        0        0       60 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/tests.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/views.py
+-rw-r--r--   0        0        0     1453 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.scss
+-rw-r--r--   0        0        0     1424 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js
+-rw-r--r--   0        0        0       18 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.scss
+-rw-r--r--   0        0        0     1467 2024-03-05 12:28:28.554496 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.js
+-rw-r--r--   0        0        0       24 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.scss
+-rw-r--r--   0        0        0      178 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/sdc_user.organizer.js
+-rw-r--r--   0        0        0      112 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/sdc_user.style.scss
+-rw-r--r--   0        0        0      999 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/tests/sdc_user.test.js
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/__init__.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/admin.py
+-rw-r--r--   0        0        0      147 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/apps.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/models.py
+-rw-r--r--   0        0        0      394 2024-03-05 20:52:54.936870 simpledomcontrol-0.5.0/sdc_user/sdc_urls.py
+-rw-r--r--   0        0        0     2331 2024-03-05 11:56:18.694802 simpledomcontrol-0.5.0/sdc_user/sdc_views.py
+-rw-r--r--   0        0        0      401 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/templates/sdc_user/sdc/sdc_login.html
+-rw-r--r--   0        0        0      327 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/templates/sdc_user/sdc/sdc_logout.html
+-rw-r--r--   0        0        0      144 2024-03-05 12:23:24.239188 simpledomcontrol-0.5.0/sdc_user/templates/sdc_user/sdc/sdc_user_nav_btn.html
+-rw-r--r--   0        0        0       60 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/tests.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/views.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 simpledomcontrol-0.5.0/PKG-INFO
```

### Comparing `simpledomcontrol-0.4.8/pyproject.toml` & `simpledomcontrol-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SimpleDomControl"
-version = "0.4.8"
+version = "0.05.00"
 authors = [ "Martin Starman <private@martin-starman.com>", ]
 description = "Simple DOM control -> a django MVC framework"
 readme = "README.md"
 license = 'Apache License 2.0'
 
 packages = [{include = "sdc_core"}, {include = "sdc_user"}, {include = "sdc_tools"}]
 keywords = ["django", "MVC",]
@@ -14,29 +14,31 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Environment :: Web Environment",
     "Operating System :: OS Independent",
     ]
 homepage = "https://github.com/StarmanMartin/sdc"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-daphne = "^4.0.0"
-channels = "^4.0.0"
-channels-redis = "^4.1.0"
-django = "^4.2.7"
+python = "^3.10"
+daphne = "^4.1.2"
+channels = "^4.1.0"
+channels-redis = "^4.2.0"
+django = "^5.0.6"
 psycopg2-binary = "^2.9.9"
-attrs = "^23.1.0"
+attrs = "^23.2.0"
+regex = "^2024.5.15"
 
 [tool.pytest.ini_options]
 pythonpath = [
     "."
 ]
 testpaths = [
     "pytests",
 ]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
+pillow = "^10.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/consumers.py` & `simpledomcontrol-0.5.0/sdc_core/consumers.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,34 +5,41 @@
 from django.core.exceptions import PermissionDenied
 from django.core.files.uploadhandler import TemporaryFileUploadHandler
 from django.core.serializers.json import Serializer
 from django.utils.datastructures import MultiValueDict
 from django.utils.translation import gettext as _f
 from django.apps import apps
 from django.db.models import FileField
+from django.contrib.auth import get_user_model
 from channels.generic.websocket import WebsocketConsumer
 
 from asgiref.sync import async_to_sync
 import importlib
 import json
 
 from sdc_core.sdc_extentions.models import SdcModel
 from sdc_core.sdc_extentions.response import sdc_link_factory, sdc_link_obj_factory
 from sdc_core.sdc_extentions.import_manager import import_function
+from sdc_core.sdc_extentions.views import SdcAccessMixin
+
+import logging
+
+logger = logging.getLogger(__name__)
+User = get_user_model()
 
 ALL_MODELS = {
     model.__name__: model for model in apps.get_models() if hasattr(model, '__is_sdc_model__')
 }
 
 importlist = []
 
 
 class MsgManager:
     _messages = None
-    _msg_filepath = os.path.abspath(settings.BASE_DIR /  'templates/sdc_strings.json')
+    _msg_filepath = os.path.abspath(settings.BASE_DIR / 'templates/sdc_strings.json')
 
     @property
     def messages(self):
         if self._messages is None:
             self._messages = {}
             if os.path.exists(self._msg_filepath):
                 with open(self._msg_filepath, 'r') as f:
@@ -64,26 +71,25 @@
                 'delete': {'header': f'{model} was deleted', 'msg': '{0} was changed'}}
 
 
 class ConsumerSerializer(Serializer):
 
     def handle_m2m_field(self, obj, field):
         super().handle_m2m_field(obj, field)
-        #self._current[field.name] = {
-        #    'pk': self._current[field.name],
-        #    'model': field.related_model.__name__,
-        #    '__is_sdc_model__': True
-        #}
+        self._current[field.name] = {
+           'pk': self._current[field.name],
+           'model': field.related_model.__name__,
+           '__is_sdc_model__': True
+        }
 
     def _value_from_field(self, obj, field):
-
-        #if hasattr(field, 'foreign_related_fields') and ALL_MODELS.get(
-        #        field.related_model.__name__) == field.related_model:
-        #    return {'pk': super()._value_from_field(obj, field), 'model': field.related_model.__name__,
-        #            '__is_sdc_model__': True}
+        if hasattr(field, 'foreign_related_fields') and ALL_MODELS.get(
+               field.related_model.__name__) == field.related_model:
+           return {'pk': super()._value_from_field(obj, field), 'model': field.related_model.__name__,
+                   '__is_sdc_model__': True}
         if issubclass(field.__class__, FileField):
             return field.value_from_object(obj).url
         return super()._value_from_field(obj, field)
 
 
 class SDCConsumer(WebsocketConsumer):
 
@@ -138,59 +144,54 @@
         # We capitalize the first letter of each component except the first one
         # with the 'title' method and join them together.
         return ''.join(x.title() for x in components)
 
     def receive(self, text_data=None, bytes_data=None):
         json_data = {}
         try:
+            session = self.scope['session'].load()
             json_data = json.loads(text_data)
             if json_data['event'] == 'sdc_call':
                 controller_name = self.to_camel_case(json_data['controller'])
                 controller = import_function("%s.sdc_views.%s" % (json_data['app'], controller_name))
+                c_instance = controller()
+                if isinstance(c_instance, SdcAccessMixin):
+                    if not c_instance.check_requirements(self.scope['user']):
+                        raise PermissionDenied()
                 method = getattr(controller(), json_data['function'])
+
+                logger.info(f"SDC call Socket received: {json_data['app']}.{controller_name}.{json_data['function']}")
+
                 return_vals = method(channel=self, **json_data.get('args', {}))
                 return_vals_generator = []
                 if isinstance(return_vals, types.GeneratorType):
                     return_vals_generator = return_vals
                     return_vals = next(return_vals, None)
 
                 self.send(text_data=json.dumps({
                     'id': json_data['id'],
                     'type': 'sdc_recall',
                     'data': return_vals,
                     'is_error': False
                 }))
                 for x in return_vals_generator: pass
-            elif json_data['event'] == 'sdc_add_group':
-                if json_data['group'] not in self.group_list:
-                    self.group_list.append(json_data['group'])
-                    async_to_sync(self.channel_layer.group_add)(
-                        json_data['group'],
-                        self.channel_name
-                    )
-            elif json_data['event'] == 'sdc_remove_group':
-                if json_data['group'] in self.group_list:
-                    self.group_list.remove(json_data['group'])
-                    async_to_sync(self.channel_layer.group_discard)(
-                        json_data['group'],
-                        self.channel_name
-                    )
+            else:
+                raise ValueError("event must be sdc_call")
 
         except PermissionDenied:
             self.state_error({
                 'msg': _f('403 Not allowed!'),
                 'header': _f('Upps!!')
             }, json_data.get('id'))
 
         except Exception as e:
-            if settings.DEBUG:
-                extracted_list = traceback.extract_tb(e.__traceback__)
-                traceback.print_tb(e.__traceback__)
-                e_text = e.__str__() + '\n'.join([item for item in traceback.StackSummary.from_list(extracted_list).format()])
-            else:
+            extracted_list = traceback.extract_tb(e.__traceback__)
+            e_text = [e.__str__()] + [item for item in traceback.StackSummary.from_list(extracted_list).format()]
+            logger.error('\n'.join(e_text))
+            if not settings.DEBUG:
                 e_text = _f('Something went wrong')
             self.state_error({
                 'msg': e_text,
                 'header': _f('Upps!!')
             }, json_data.get('id'))
 
 
@@ -233,74 +234,86 @@
             pass
 
     def state_error(self, event):
         self.send(text_data=json.dumps({
             'type': event.get('type', 'error'),
             'is_error': True,
             'msg': event.get('msg', ''),
+            'event_id': event.get('event_id'),
             'header': event.get('header', ''),
         }))
 
     def receive(self, text_data=None, bytes_data=None):
         msg_type = 'error'
+        json_data = {}
         try:
             json_data = json.loads(text_data)
             self.scope['request'] = json_data
             msg_type = json_data.get('event_type', msg_type)
             self.scope['event_type'] = msg_type
             event_type = "%s_%s" % (json_data['event'], json_data['event_type'])
-            self.queryset = json_data['args']['model_query']
+            logger.debug("Socket received: " + event_type)
+            self.queryset = json_data['args'].get('model_query', {})
             if not self.model.is_authorised(self.scope['user'], msg_type, self.queryset):
                 raise PermissionDenied
             if event_type == 'model_connect':
                 self._init_connection(json_data)
-            if event_type == 'model_edit_form':
+            elif event_type == 'model_edit_form':
                 self._load_edit_form(json_data)
-            if event_type == 'model_create_form':
+            elif event_type == 'model_named_form':
+                self._load_named_form(json_data)
+            elif event_type == 'model_create_form':
                 self._load_create_form(json_data)
-            if event_type == 'model_list_view':
+            elif event_type == 'model_list_view':
                 self._load_list_view(json_data)
-            if event_type == 'model_detail_view':
+            elif event_type == 'model_detail_view':
                 self._load_detail_view(json_data)
-            if event_type == 'model_save':
+            elif event_type == 'model_save':
                 self._save_element(json_data)
-            if event_type == 'model_create':
+            elif event_type == 'model_create':
                 self._create_element(json_data)
-            if event_type == 'model_upload':
+            elif event_type == 'model_upload':
                 self._upload_file(json_data)
-            if event_type == 'model_delete':
+            elif event_type == 'model_delete':
                 self._delete_element(json_data)
             elif event_type == 'model_load':
                 model_data = ConsumerSerializer().serialize(self._load_model())
                 self.send(text_data=json.dumps({
                     'type': json_data['event_type'],
                     'event_id': json_data['event_id'],
                     'args': {
                         'data': model_data,
                         'media_url': settings.MEDIA_URL or '/'
                     },
                     'is_error': False
                 }))
+            else:
+                raise ValueError(
+                    f"{json_data['event']} must be 'model' and {json_data['event_type']} must be in [load, delete, upload, create, save, detail_view, 'connect', 'edit_form', 'create_form', 'list_view']")
         except PermissionDenied as e:
+            logger.error("403 Not allowed!")
             self.state_error({
                 'type': msg_type,
                 'msg': _f('403 Not allowed!'),
+                'event_id': json_data.get('event_id'),
                 'header': _f('Upps!!')
             })
 
         except Exception as e:
+            extracted_list = traceback.extract_tb(e.__traceback__)
+            e_text = [e.__str__()] + [item for item in traceback.StackSummary.from_list(extracted_list).format()]
             if settings.DEBUG:
-                extracted_list = traceback.extract_tb(e.__traceback__)
                 traceback.print_tb(e.__traceback__)
-                e_text = e.__str__() + '\n'.join([item for item in traceback.StackSummary.from_list(extracted_list).format()])
             else:
+                logger.error(e_text)
                 e_text = _f('Something went wrong')
             self.state_error({
                 'type': msg_type,
                 'msg': e_text,
+                'event_id': json_data.get('event_id'),
                 'header': _f('Upps!!')
             })
 
     def _add_to_class(self):
         async_to_sync(self.channel_layer.group_add)(
             self.model_name,
             self.channel_name
@@ -333,14 +346,23 @@
         return self._load_form(json_data, self.model.create_form, instance)
 
     def _load_edit_form(self, json_data):
         instance = self._load_model().get(pk=json_data['args']['pk'])
         instance.scope = self.scope
         return self._load_form(json_data, self.model.edit_form, instance)
 
+    def _load_named_form(self, json_data):
+        instance = self._load_model().get(pk=json_data['args']['pk'])
+        instance.scope = self.scope
+        form_name = json_data['args']['form_name']
+        if not hasattr(self.model, 'forms'):
+            raise NotImplemented()
+
+        return self._load_form(json_data, self.model.forms.get(form_name), instance)
+
     def _load_form(self, json_data, form_attr, instance=None):
         if callable(form_attr):
             form_attr = form_attr({})
         if form_attr is None:
             raise NotImplemented()
         elif isinstance(form_attr, str):
             edit_form_path = form_attr.split('.')
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_controller_manager.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_controller_manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-import os
-import re
-import subprocess
-import sys
-
-from django.urls import get_resolver
-
-from sdc_core.management.commands.init_add import options
-from sdc_core.management.commands.init_add.utils import convert_to_snake_case, copy_and_prepare, \
-    convert_to_camel_case, \
-    convert_to_title_camel_case, convert_to_tag_name, prepare_as_string
-
-
-class AddControllerManager:
-    def __init__(self, app_name: str, controller_name: str):
-        self.app_name = app_name
-        self.controller_name_sc = convert_to_snake_case(controller_name)
-        self.controller_name_cc = convert_to_camel_case(controller_name)
-        self.controller_name_tcc = convert_to_title_camel_case(controller_name)
-        self.controller_name = controller_name
-        self._template_url = None
-
-        self.reps = {**options.REPLACEMENTS, **{'§CONTROLLERNAMETITLE§': self.controller_name_tcc,
-                                                '§CONTROLLERNAMECC§': self.controller_name_cc,
-                                                '§CONTROLLERNAMESC§': self.controller_name_sc,
-                                                '§APPNAME§': self.app_name
-                                                }}
-
-    @staticmethod
-    def check_controller_name(c_name_sc):
-        url_name = "scd_view_" + c_name_sc
-
-        for i in get_resolver().reverse_dict.keys():
-            if str(i).endswith(url_name):
-                return True
-
-        return False
-
-    @staticmethod
-    def get_url(c_name_sc):
-        url_name = "scd_view_" + c_name_sc
-
-        for i in get_resolver().reverse_dict.keys():
-            if str(i).endswith(url_name):
-                url_to_sdc = "/" + get_resolver().reverse_dict[i][0][0][0]
-                return url_to_sdc
-        return ''
-
-    def check_if_url_is_unique(self):
-        return not self.check_controller_name(self.controller_name_sc)
-
-    def get_template_url(self):
-        if self._template_url is not None:
-            return self._template_url
-        cmd = '%s manage.py sdc_get_controller_url %s' % (sys.executable, self.controller_name_sc)
-        p = subprocess.Popen(cmd, stdout=subprocess.PIPE, shell=True, cwd=options.PROJECT_ROOT)
-        out = str(p.communicate()[0], encoding="utf-8")
-        out = re.sub(r'\\r?\\n.*$', r'', out)
-        out = re.sub(r'\r?\n.*$', r'', out)
-        self._template_url = re.sub(r'^b\'([^\']*)\'$', r'\g<1>', out)
-        return self._template_url
-
-    def get_template_url_sync(self):
-        if self._template_url is not None:
-            return self._template_url
-        out = self.get_url(self.controller_name_sc)
-        self._template_url = re.sub(r'^b\'([^\']*)\'$', r'\g<1>', out)
-        return self._template_url
-
-    def get_url_params(self):
-        url = self.get_template_url()
-        return re.findall('%\(([^)]+)\)\w', url)
-
-    def get_params_as_string(self):
-        params_list = self.get_url_params()
-        if len(params_list) > 0:
-            return ', ' + ', '.join(params_list)
-        return ''
-
-    def add_url_to_url_pattern(self, main_urls_path):
-        urls_path = os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_urls.py")
-
-        if not os.path.exists(urls_path):
-            copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "sdc_urls.py.txt"),
-                             os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_urls.py"),
-                             self.reps)
-
-            copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "sdc_views.py.txt"),
-                             os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_views.py"),
-                             self.reps)
-
-            copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "js_test.js.txt"),
-                             os.path.join(options.PROJECT_ROOT, self.app_name, 'Assets/tests',
-                                          f"{self.app_name}.test.js"),
-                             self.reps)
-
-            self._add_new_sdc_to_main_urls(main_urls_path)
-
-        self._add_sdc_views_to_main_urls(os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_urls.py"))
-
-    def _add_new_sdc_to_main_urls(self, main_urls_path):
-        return self._add_to_urls(main_urls_path, "sdc_view/%s/" % self.app_name,
-                                 "include('%s.sdc_urls')" % self.app_name)
-
-    def _add_sdc_views_to_main_urls(self, main_urls_path):
-        return self._add_to_urls(main_urls_path, self.controller_name_sc,
-                                 "sdc_views.%s.as_view(), name='scd_view_%s'" % (
-                                     self.controller_name_tcc, self.controller_name_sc))
-
-    def add_view_class_to_sdc_views(self):
-        fin = open(os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_views.py"), "at", encoding='utf-8')
-        fin.write(
-            "\n\nclass %s(SDCView):\n%stemplate_name='%s/sdc/%s.html'\n" % (
-                self.controller_name_tcc, options.SEP, self.app_name, self.controller_name_sc))
-        fin.close()
-        fin = open(os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_views.py"), "at", encoding='utf-8')
-
-        fin.write(
-            "\n%sdef get_content(self, request%s, *args, **kwargs):\n%sreturn render(request, self.template_name)" % (
-                options.SEP, self.get_params_as_string(), options.SEP * 2))
-        fin.close()
-
-    def prepare_files(self):
-        main_static = os.path.join(
-            options.PROJECT_ROOT, self.app_name, "Assets/src", self.app_name, 'controller', self.controller_name_sc)
-        main_templates = os.path.join(options.PROJECT_ROOT, self.app_name, "templates", self.app_name)
-        self.reps['§TEMPLATEURL§'] = self.get_template_url()
-        self.reps['§TAGNAME§'] = self.prepare_tag_name()
-        self.reps['§TAG§'] = convert_to_tag_name(self.controller_name_cc)
-
-        copy_and_prepare(
-            os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "template_controller.js.txt"),
-            os.path.join(main_static, self.controller_name_sc + ".js"),
-            self.reps)
-
-        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "template_css.scss"),
-                         os.path.join(main_static,
-                                      self.controller_name_sc + ".scss"),
-                         self.reps)
-
-        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "templade_view.html"),
-                         os.path.join(main_templates, "sdc",
-                                      self.controller_name_sc + ".html"),
-                         self.reps)
-
-    def add_to_organizer(self, add_css=True):
-        org_js_file_path = os.path.join(options.PROJECT_ROOT, self.app_name, "Assets/src", self.app_name,
-                                        "%s.organizer.js" % self.app_name)
-        org_style_file_path = os.path.join(options.PROJECT_ROOT, self.app_name, "Assets/src", self.app_name,
-                                           "%s.style.scss" % self.app_name)
-
-        if not os.path.exists(org_js_file_path):
-            org_file_path_root = os.path.join(options.PROJECT_ROOT, "Assets/src",
-                                         "index.organizer.js")
-            line = 'import {} from "./%s/%s.organizer.js";\n' % (self.app_name, self.app_name)
-
-            self._add_js_to_src(org_file_path_root, line)
-
-        if add_css:
-            if not os.path.exists(org_style_file_path):
-                org_file_path_root = os.path.join(options.PROJECT_ROOT, "Assets/src",
-                                             "index.style.scss")
-                line = '@import "./%s/%s.style.scss";\n' % (self.app_name, self.app_name)
-
-                self._add_scss_to_src(org_file_path_root, line)
-
-            line = '@import "./controller/%s/%s.scss";\n' % (self.controller_name_sc, self.controller_name_sc)
-            self._add_scss_to_src(org_style_file_path, line)
-
-        line = 'import {} from "./controller/%s/%s.js";\n' % (self.controller_name_sc, self.controller_name_sc)
-        self._add_js_to_src(org_js_file_path, line)
-
-    def add_js_test(self):
-        text = prepare_as_string(
-            os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "template_test.js.text"), self.reps)
-        fp = os.path.join(options.PROJECT_ROOT, self.app_name, 'Assets/tests', f"{self.app_name}.test.js")
-        fout = open(fp, "a", encoding='utf-8')
-        fout.write(text)
-        fout.close()
-
-    @staticmethod
-    def _add_js_to_src(org_file_path, new_line):
-        text = new_line
-        if not os.path.exists(org_file_path):
-            fin = open(org_file_path, 'x', encoding='utf-8')
-        else:
-            fin = open(org_file_path, 'r', encoding='utf-8')
-
-            for line in fin:
-                text += line
-
-        fin.close()
-
-        fout = open(org_file_path, "w+", encoding='utf-8')
-        fout.write(text)
-        fout.close()
-
-    @staticmethod
-    def _add_scss_to_src(org_file_path, new_line):
-
-        if not os.path.exists(org_file_path):
-            fin = open(org_file_path, 'x', encoding='utf-8')
-            text = new_line
-        else:
-            fin = open(org_file_path, 'r', encoding='utf-8')
-            text = ''
-            added = False
-            for line in fin:
-                if not line.startswith('@import') and not added:
-                    text += "%s" % new_line
-                    added = True
-                text += line
-            if not added:
-                text += "%s" % new_line
-
-        fin.close()
-
-        fout = open(org_file_path, "w+", encoding='utf-8')
-        fout.write(text)
-        fout.close()
-
-    @staticmethod
-    def _add_to_urls(main_urls_path, url_path, handler):
-        fin = open(main_urls_path, "r+", encoding='utf-8')
-        text = ""
-        is_done = False
-
-        for line in fin:
-            if not is_done and "# scd view below" in line:
-                line += "%spath('%s', %s),\n" % (options.SEP, url_path.lower(), handler)
-                is_done = True
-            text += line
-
-        fin.close()
-        if not is_done:
-            print(options.CMD_COLORS.as_warning("Do not forgett to add:"))
-            print(options.CMD_COLORS.as_important(
-                "%spath('%s', %s),\n # scd view below\n]" % (options.SEP, url_path.lower(), handler)))
-            print(options.CMD_COLORS.as_warning("to: %s " % main_urls_path))
-
-        fout = open(main_urls_path, "w+", encoding='utf-8')
-        fout.write(text)
-        fout.close()
-
-    def prepare_tag_name(self):
-        tag_name = convert_to_tag_name(self.controller_name_cc)
-        param_list = []
-        for x in self.get_url_params():
-            param_list.append(convert_to_tag_name(x) + '=""')
-        param_data_str = ""
-        if len(param_list) > 0:
-            param_data_str = " data-"
-        param_data_str += param_data_str.join(param_list)
-        return "<%s%s></%s>" % (tag_name, param_data_str, tag_name)
+import os
+import re
+import subprocess
+import sys
+
+from django.urls import get_resolver
+
+from sdc_core.management.commands.init_add import options
+from sdc_core.management.commands.init_add.utils import convert_to_snake_case, copy_and_prepare, \
+    convert_to_camel_case, \
+    convert_to_title_camel_case, convert_to_tag_name, prepare_as_string
+
+
+class AddControllerManager:
+    def __init__(self, app_name: str, controller_name: str):
+        self.app_name = app_name
+        self.controller_name_sc = convert_to_snake_case(controller_name)
+        self.controller_name_cc = convert_to_camel_case(controller_name)
+        self.controller_name_tcc = convert_to_title_camel_case(controller_name)
+        self.controller_name = controller_name
+        self._template_url = None
+
+        self.reps = {**options.REPLACEMENTS, **{'§CONTROLLERNAMETITLE§': self.controller_name_tcc,
+                                                '§CONTROLLERNAMECC§': self.controller_name_cc,
+                                                '§CONTROLLERNAMESC§': self.controller_name_sc,
+                                                '§APPNAME§': self.app_name
+                                                }}
+
+    @staticmethod
+    def check_controller_name(c_name_sc):
+        url_name = "scd_view_" + c_name_sc
+
+        for i in get_resolver().reverse_dict.keys():
+            if str(i).endswith(url_name):
+                return True
+
+        return False
+
+    @staticmethod
+    def get_url(c_name_sc):
+        url_name = "scd_view_" + c_name_sc
+
+        for i in get_resolver().reverse_dict.keys():
+            if str(i).endswith(url_name):
+                url_to_sdc = "/" + get_resolver().reverse_dict[i][0][0][0]
+                return url_to_sdc
+        return ''
+
+    def check_if_url_is_unique(self):
+        return not self.check_controller_name(self.controller_name_sc)
+
+    def get_template_url(self):
+        if self._template_url is not None:
+            return self._template_url
+        cmd = '%s manage.py sdc_get_controller_url %s' % (sys.executable, self.controller_name_sc)
+        p = subprocess.Popen(cmd, stdout=subprocess.PIPE, shell=True, cwd=options.PROJECT_ROOT)
+        out = str(p.communicate()[0], encoding="utf-8")
+        out = re.sub(r'\\r?\\n.*$', r'', out)
+        out = re.sub(r'\r?\n.*$', r'', out)
+        self._template_url = re.sub(r'^b\'([^\']*)\'$', r'\g<1>', out)
+        return self._template_url
+
+    def get_template_url_sync(self):
+        if self._template_url is not None:
+            return self._template_url
+        out = self.get_url(self.controller_name_sc)
+        self._template_url = re.sub(r'^b\'([^\']*)\'$', r'\g<1>', out)
+        return self._template_url
+
+    def get_url_params(self):
+        url = self.get_template_url()
+        return re.findall('%\(([^)]+)\)\w', url)
+
+    def get_params_as_string(self):
+        params_list = self.get_url_params()
+        if len(params_list) > 0:
+            return ', ' + ', '.join(params_list)
+        return ''
+
+    def add_url_to_url_pattern(self, main_urls_path):
+        urls_path = os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_urls.py")
+
+        if not os.path.exists(urls_path):
+            copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "sdc_urls.py.txt"),
+                             os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_urls.py"),
+                             self.reps)
+
+            copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "sdc_views.py.txt"),
+                             os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_views.py"),
+                             self.reps)
+
+            copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "js_test.js.txt"),
+                             os.path.join(options.PROJECT_ROOT, self.app_name, 'Assets/tests',
+                                          f"{self.app_name}.test.js"),
+                             self.reps)
+
+            self._add_new_sdc_to_main_urls(main_urls_path)
+
+        self._add_sdc_views_to_main_urls(os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_urls.py"))
+
+    def _add_new_sdc_to_main_urls(self, main_urls_path):
+        return self._add_to_urls(main_urls_path, "sdc_view/%s/" % self.app_name,
+                                 "include('%s.sdc_urls')" % self.app_name)
+
+    def _add_sdc_views_to_main_urls(self, main_urls_path):
+        return self._add_to_urls(main_urls_path, self.controller_name_sc,
+                                 "sdc_views.%s.as_view(), name='scd_view_%s'" % (
+                                     self.controller_name_tcc, self.controller_name_sc))
+
+    def add_view_class_to_sdc_views(self):
+        fin = open(os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_views.py"), "at", encoding='utf-8')
+        fin.write(
+            "\n\nclass %s(SDCView):\n%stemplate_name='%s/sdc/%s.html'\n" % (
+                self.controller_name_tcc, options.SEP, self.app_name, self.controller_name_sc))
+        fin.close()
+        fin = open(os.path.join(options.PROJECT_ROOT, self.app_name, "sdc_views.py"), "at", encoding='utf-8')
+
+        fin.write(
+            "\n%sdef get_content(self, request%s, *args, **kwargs):\n%sreturn render(request, self.template_name)" % (
+                options.SEP, self.get_params_as_string(), options.SEP * 2))
+        fin.close()
+
+    def prepare_files(self):
+        main_static = os.path.join(
+            options.PROJECT_ROOT, self.app_name, "Assets/src", self.app_name, 'controller', self.controller_name_sc)
+        main_templates = os.path.join(options.PROJECT_ROOT, self.app_name, "templates", self.app_name)
+        self.reps['§TEMPLATEURL§'] = self.get_template_url()
+        self.reps['§TAGNAME§'] = self.prepare_tag_name()
+        self.reps['§TAG§'] = convert_to_tag_name(self.controller_name_cc)
+
+        copy_and_prepare(
+            os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "template_controller.js.txt"),
+            os.path.join(main_static, self.controller_name_sc + ".js"),
+            self.reps)
+
+        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "template_css.scss"),
+                         os.path.join(main_static,
+                                      self.controller_name_sc + ".scss"),
+                         self.reps)
+
+        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "templade_view.html"),
+                         os.path.join(main_templates, "sdc",
+                                      self.controller_name_sc + ".html"),
+                         self.reps)
+
+    def add_to_organizer(self, add_css=True):
+        org_js_file_path = os.path.join(options.PROJECT_ROOT, self.app_name, "Assets/src", self.app_name,
+                                        "%s.organizer.js" % self.app_name)
+        org_style_file_path = os.path.join(options.PROJECT_ROOT, self.app_name, "Assets/src", self.app_name,
+                                           "%s.style.scss" % self.app_name)
+
+        if not os.path.exists(org_js_file_path):
+            org_file_path_root = os.path.join(options.PROJECT_ROOT, "Assets/src",
+                                         "index.organizer.js")
+            line = 'import {} from "./%s/%s.organizer.js";\n' % (self.app_name, self.app_name)
+
+            self._add_js_to_src(org_file_path_root, line)
+
+        if add_css:
+            if not os.path.exists(org_style_file_path):
+                org_file_path_root = os.path.join(options.PROJECT_ROOT, "Assets/src",
+                                             "index.style.scss")
+                line = '@import "./%s/%s.style.scss";\n' % (self.app_name, self.app_name)
+
+                self._add_scss_to_src(org_file_path_root, line)
+
+            line = '@import "./controller/%s/%s.scss";\n' % (self.controller_name_sc, self.controller_name_sc)
+            self._add_scss_to_src(org_style_file_path, line)
+
+        line = 'import {} from "./controller/%s/%s.js";\n' % (self.controller_name_sc, self.controller_name_sc)
+        self._add_js_to_src(org_js_file_path, line)
+
+    def add_js_test(self):
+        text = prepare_as_string(
+            os.path.join(options.SCRIPT_ROOT, "template_files", "controller", "template_test.js.text"), self.reps)
+        fp = os.path.join(options.PROJECT_ROOT, self.app_name, 'Assets/tests', f"{self.app_name}.test.js")
+        fout = open(fp, "a", encoding='utf-8')
+        fout.write(text)
+        fout.close()
+
+    @staticmethod
+    def _add_js_to_src(org_file_path, new_line):
+        text = new_line
+        if not os.path.exists(org_file_path):
+            fin = open(org_file_path, 'x', encoding='utf-8')
+        else:
+            fin = open(org_file_path, 'r', encoding='utf-8')
+
+            for line in fin:
+                text += line
+
+        fin.close()
+
+        fout = open(org_file_path, "w+", encoding='utf-8')
+        fout.write(text)
+        fout.close()
+
+    @staticmethod
+    def _add_scss_to_src(org_file_path, new_line):
+
+        if not os.path.exists(org_file_path):
+            fin = open(org_file_path, 'x', encoding='utf-8')
+            text = new_line
+        else:
+            fin = open(org_file_path, 'r', encoding='utf-8')
+            text = ''
+            added = False
+            for line in fin:
+                if not line.startswith('@import') and not added:
+                    text += "%s" % new_line
+                    added = True
+                text += line
+            if not added:
+                text += "%s" % new_line
+
+        fin.close()
+
+        fout = open(org_file_path, "w+", encoding='utf-8')
+        fout.write(text)
+        fout.close()
+
+    @staticmethod
+    def _add_to_urls(main_urls_path, url_path, handler):
+        fin = open(main_urls_path, "r+", encoding='utf-8')
+        text = ""
+        is_done = False
+
+        for line in fin:
+            if not is_done and "# scd view below" in line:
+                line += "%spath('%s', %s),\n" % (options.SEP, url_path.lower(), handler)
+                is_done = True
+            text += line
+
+        fin.close()
+        if not is_done:
+            print(options.CMD_COLORS.as_warning("Do not forgett to add:"))
+            print(options.CMD_COLORS.as_important(
+                "%spath('%s', %s),\n # scd view below\n]" % (options.SEP, url_path.lower(), handler)))
+            print(options.CMD_COLORS.as_warning("to: %s " % main_urls_path))
+
+        fout = open(main_urls_path, "w+", encoding='utf-8')
+        fout.write(text)
+        fout.close()
+
+    def prepare_tag_name(self):
+        tag_name = convert_to_tag_name(self.controller_name_cc)
+        param_list = []
+        for x in self.get_url_params():
+            param_list.append(convert_to_tag_name(x) + '=""')
+        param_data_str = ""
+        if len(param_list) > 0:
+            param_data_str = " data-"
+        param_data_str += param_data_str.join(param_list)
+        return "<%s%s></%s>" % (tag_name, param_data_str, tag_name)
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/add_model_manager.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,27 +48,27 @@
 
         self._check_if_sdcmodel_imported(model_path)
         f = open(model_path, 'a')
 
         search_form_def = "\n".join([
             'class {2}SearchForm(AbstractSearchForm):',
             '{0}CHOICES = (("id", "Id"),)',
-            '{0}PLACEHOLDER = "Id"',
+            '{0}PLACEHOLDER = ""',
             '{0}DEFAULT_CHOICES = CHOICES[0][0]',
             '{0}SEARCH_FIELDS = ("id",)',
         ]).format(options.SEP, self.app_name, self.model_name)
 
         class_def = "\n".join([
             'class {2}(models.Model, SdcModel):',
             '{0}edit_form = "{1}.forms.{2}Form"',
             '{0}create_form = "{1}.forms.{2}Form"',
             '{0}html_list_template = "{1}/models/{2}/{2}_list.html"',
             '{0}html_detail_template = "{1}/models/{2}/{2}_details.html"',
             '',
-            '{0}@classmethod\n{0}def render(cls, template_name, context=None, request=None, using=None):\n{0}{0}if template_name == cls.html_list_template:\n{0}{0}{0}sf = {2}SearchForm(data=context.get("filter", {{}}))\n{0}{0}{0}context = context | handle_search_form(context["instances"], sf,  range=2)\n{0}{0}return render_to_string(template_name=template_name, context=context, request=request, using=using)',
+            '{0}@classmethod\n{0}def render(cls, template_name, context=None, request=None, using=None):\n{0}{0}if template_name == cls.html_list_template:\n{0}{0}{0}sf = {2}SearchForm(data=context.get("filter", {{}}))\n{0}{0}{0}context = context | handle_search_form(context["instances"], sf,  range=10)\n{0}{0}return render_to_string(template_name=template_name, context=context, request=request, using=using)',
             '',
             '{0}@classmethod\n{0}def is_authorised(cls, user, action, obj):\n{0}{0}return True',
             '',
             '{0}@classmethod\n{0}def get_queryset(cls, user, action, obj):\n{0}{0}return cls.objects.all()',
         ]).format(options.SEP, self.app_name, self.model_name)
 
         f.write('\n{0}\n\n{1}\n'.format(search_form_def, class_def))
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/options.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/options.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import os
-
-MAIN_APP_NAME = "Undefined"
-SEP = '    '
-PROJECT = 'Undefined'
-PROJECT_ROOT = os.getcwd()
-SCRIPT_ROOT = os.path.abspath(os.path.join(os.path.dirname(os.path.realpath(__file__)), '../../../'))
-REPLACEMENTS = {"<!--§MAIN_APP§-->": MAIN_APP_NAME,"§MAIN_APP§": MAIN_APP_NAME,
-                "<!--§PROJECT§-->": PROJECT,"§PROJECT§": PROJECT}
-
-def setPROJECT(project):
-    global PROJECT, MAIN_APP_NAME
-    MAIN_APP_NAME = project
-    PROJECT = project
-    REPLACEMENTS['<!--§PROJECT§-->'] = project
-    REPLACEMENTS['§PROJECT§'] = project
-    REPLACEMENTS['<!--§MAIN_APP§-->'] = project
-    REPLACEMENTS['§MAIN_APP§'] = project
-
-class CMD_COLORS:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
-    @classmethod
-    def as_error(cls, text):
-        return "%s%s%s" % (cls.FAIL,text,cls.ENDC)
-
-    @classmethod
-    def as_warning(cls, text):
-        return "%s%s%s" % (cls.WARNING,text,cls.ENDC) \
-
-    @classmethod
-    def as_important(cls, text):
-        return "%s%s%s%s" % (cls.BOLD, cls.HEADER,text,cls.ENDC)
+import os
+
+MAIN_APP_NAME = "Undefined"
+SEP = '    '
+PROJECT = 'Undefined'
+PROJECT_ROOT = os.getcwd()
+SCRIPT_ROOT = os.path.abspath(os.path.join(os.path.dirname(os.path.realpath(__file__)), '../../../'))
+REPLACEMENTS = {"<!--§MAIN_APP§-->": MAIN_APP_NAME,"§MAIN_APP§": MAIN_APP_NAME,
+                "<!--§PROJECT§-->": PROJECT,"§PROJECT§": PROJECT}
+
+def setPROJECT(project):
+    global PROJECT, MAIN_APP_NAME
+    MAIN_APP_NAME = project
+    PROJECT = project
+    REPLACEMENTS['<!--§PROJECT§-->'] = project
+    REPLACEMENTS['§PROJECT§'] = project
+    REPLACEMENTS['<!--§MAIN_APP§-->'] = project
+    REPLACEMENTS['§MAIN_APP§'] = project
+
+class CMD_COLORS:
+    HEADER = '\033[95m'
+    OKBLUE = '\033[94m'
+    OKGREEN = '\033[92m'
+    WARNING = '\033[93m'
+    FAIL = '\033[91m'
+    ENDC = '\033[0m'
+    BOLD = '\033[1m'
+    UNDERLINE = '\033[4m'
+
+    @classmethod
+    def as_error(cls, text):
+        return "%s%s%s" % (cls.FAIL,text,cls.ENDC)
+
+    @classmethod
+    def as_warning(cls, text):
+        return "%s%s%s" % (cls.WARNING,text,cls.ENDC) \
+
+    @classmethod
+    def as_important(cls, text):
+        return "%s%s%s%s" % (cls.BOLD, cls.HEADER,text,cls.ENDC)
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/init_add/settings_manager.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/settings_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,127 @@
-import importlib
-import re
-import os
-
-from django.core.management import CommandError
-
-from sdc_core.management.commands.init_add import options
-from django.conf import settings
-
-def get_app_path(app_name):
-    try:
-        app_module = importlib.import_module(app_name)
-        return os.path.dirname(app_module.__file__)
-    except:
-        raise CommandError(f"{app_name} is not an installed app")
-
-
-class SettingsManager:
-
-    def __init__(self, manage_py_file: str):
-        self.manage_py_file_path = os.path.join(options.PROJECT_ROOT, manage_py_file)
-        self.settings_file_path = None
-        self.setting_vals = None
-
-    def get_settings_file_path(self):
-        if self.settings_file_path is not None:
-            return self.settings_file_path
-
-        settings_file_path = os.environ.get('DJANGO_SETTINGS_MODULE').replace(".", "/") + ".py"
-        self.settings_file_path = os.path.join(options.PROJECT_ROOT, settings_file_path)
-        return self.settings_file_path
-
-    def find_and_set_whitespace_sep(self):
-        manage_py_file = open(self.manage_py_file_path, "r", encoding='utf-8')
-        regexp = re.compile(r'DJANGO_SETTINGS_MODULE')
-
-        for line in manage_py_file.readlines():
-            if regexp.search(line):
-                options.SEP = re.search(r'[^o]+', line).group(0)
-
-    def get_setting_vals(self):
-        return settings
-
-    def check_settings(self):
-        if not self.get_setting_vals().TEMPLATES[0]['APP_DIRS']:
-            print(options.CMD_COLORS.as_error("SDC only works if TEMPLATES -> APP_DIRS is ture"))
-            exit(1)
-        temp_dir = self.get_setting_vals().BASE_DIR / 'templates'
-        if not temp_dir in self.get_setting_vals().TEMPLATES[0]['DIRS']:
-            print(options.CMD_COLORS.as_error("SDC only works if '%s' is in  TEMPLATES -> DIRS" % temp_dir))
-            exit(1)
-
-    def update_settings(self, settings_extension):
-
-        apps = self.get_setting_vals().INSTALLED_APPS
-        apps = [a for a in apps if a != 'sdc_core']
-        apps.insert(0, 'daphne')
-        apps.append('channels')
-        apps.append('sdc_tools')
-        apps.append('sdc_user')
-        apps.append('sdc_core')
-        sep = str(options.SEP)
-
-        new_val = f"VERSION=0.0\n\nINSTALLED_APPS = [\n{sep}'%s'\n]" % (("',\n%s'" % sep).join(apps))
-        pre_add = '\n'.join(["if not DEBUG:",
-                             sep + "hosts = [urlparse(x)  for x in os.environ.get('ALLOWED_HOST').split(',')]",
-                             sep + "ALLOWED_HOSTS = [host.hostname for host in hosts]",
-                             sep + "CSRF_TRUSTED_ORIGINS = [urlunparse(x) for x in hosts]",
-                             "else:",
-                             sep + "ALLOWED_HOSTS = ['*']"])
-
-        new_val = f"{pre_add}\n\n{new_val}"
-        new_val += "\n\nINTERNAL_IPS = (\n%s'127.0.0.1',\n)\n" % (options.SEP)
-
-        fin = open(self.get_settings_file_path(), "rt", encoding='utf-8')
-
-        data = fin.read()
-        fin.close()
-        data = re.sub(r'(from[^\n]*)', '\g<1>\nimport os\nfrom urllib.parse import urlparse, urlunparse', data)
-        data = re.sub(r'(ALLOWED_HOSTS[^\n]*)', '# \g<1>', data)
-        data = re.sub(r'INSTALLED_APPS\s*=\s*\[[^\]]+\]', new_val, data)
-
-        data += settings_extension
-
-        fout = open(self.get_settings_file_path(), "wt", encoding='utf-8')
-        fout.write(data)
-        fout.close()
-
-    def get_apps(self):
-        self.find_and_set_project_name()
-        app_list = [options.MAIN_APP_NAME]
-        for app_name in self.get_setting_vals().INSTALLED_APPS:
-            if os.path.exists(os.path.join(options.PROJECT_ROOT, app_name)) and app_name not in app_list:
-                app_list.append(app_name)
-
-        return app_list
-
-    def get_sdc_apps(self):
-        self.find_and_set_project_name()
-        app_list = []
-        for app_name in self.get_setting_vals().INSTALLED_APPS:
-            if os.path.exists(os.path.join(get_app_path(app_name), 'sdc_views.py')):
-                app_list.append(app_name)
-
-        return app_list
-
-
-
-
-
-    def get_main_url_path(self):
-        return os.path.join(options.PROJECT_ROOT, self.get_setting_vals().ROOT_URLCONF.replace(".", "/") + ".py")
-
-    def find_and_set_project_name(self):
-        options.setPROJECT(self.get_setting_vals().ROOT_URLCONF.split(".")[0])
-        print(options.PROJECT)
+import importlib
+import re
+import os
+
+import regex
+from django.core.management import CommandError
+
+from sdc_core.management.commands.init_add import options
+from django.conf import settings
+
+def get_app_path(app_name):
+    try:
+        app_module = importlib.import_module(app_name)
+        return os.path.dirname(app_module.__file__)
+    except:
+        raise CommandError(f"{app_name} is not an installed app")
+
+
+class SettingsManager:
+
+    def __init__(self, manage_py_file: str):
+        self.manage_py_file_path = os.path.join(options.PROJECT_ROOT, manage_py_file)
+        self.settings_file_path = None
+        self.setting_vals = None
+
+    def get_settings_file_path(self):
+        if self.settings_file_path is not None:
+            return self.settings_file_path
+
+        settings_file_path = os.environ.get('DJANGO_SETTINGS_MODULE').replace(".", "/") + ".py"
+        self.settings_file_path = os.path.join(options.PROJECT_ROOT, settings_file_path)
+        return self.settings_file_path
+
+    def find_and_set_whitespace_sep(self):
+        manage_py_file = open(self.manage_py_file_path, "r", encoding='utf-8')
+        regexp = re.compile(r'DJANGO_SETTINGS_MODULE')
+
+        for line in manage_py_file.readlines():
+            if regexp.search(line):
+                options.SEP = re.search(r'[^o]+', line).group(0)
+
+    def get_setting_vals(self):
+        return settings
+
+    def check_settings(self):
+        if not self.get_setting_vals().TEMPLATES[0]['APP_DIRS']:
+            print(options.CMD_COLORS.as_error("SDC only works if TEMPLATES -> APP_DIRS is ture"))
+            exit(1)
+        temp_dir = self.get_setting_vals().BASE_DIR / 'templates'
+        if not temp_dir in self.get_setting_vals().TEMPLATES[0]['DIRS']:
+            print(options.CMD_COLORS.as_error("SDC only works if '%s' is in  TEMPLATES -> DIRS" % temp_dir))
+            exit(1)
+
+    def update_settings(self, settings_extension):
+
+        apps = self.get_setting_vals().INSTALLED_APPS
+        apps = [a for a in apps if a != 'sdc_core']
+        apps.insert(0, 'daphne')
+        apps.append('channels')
+        apps.append('sdc_tools')
+        apps.append('sdc_user')
+        apps.append('sdc_core')
+        sep = str(options.SEP)
+
+        new_val = f"VERSION=0.0\n\nINSTALLED_APPS = [\n{sep}'%s'\n]" % (("',\n%s'" % sep).join(apps))
+        pre_add = '\n'.join(["if not DEBUG:",
+                             sep + "hosts = [urlparse(x)  for x in os.environ.get('ALLOWED_HOST').split(',')]",
+                             sep + "ALLOWED_HOSTS = [host.hostname for host in hosts]",
+                             sep + "CSRF_TRUSTED_ORIGINS = [urlunparse(x) for x in hosts]",
+                             "else:",
+                             sep + "ALLOWED_HOSTS = ['*']"])
+
+        new_val = f"{pre_add}\n\n{new_val}"
+        new_val += "\n\nINTERNAL_IPS = (\n%s'127.0.0.1',\n)\n" % (options.SEP)
+
+        fin = open(self.get_settings_file_path(), "rt", encoding='utf-8')
+
+        data = fin.read()
+        fin.close()
+        data = re.sub(r'(from[^\n]*)', '\g<1>\nimport os\nfrom urllib.parse import urlparse, urlunparse', data)
+        data = re.sub(r'(ALLOWED_HOSTS[^\n]*)', '# \g<1>', data)
+        data = re.sub(r'INSTALLED_APPS\s*=\s*\[[^\]]+\]', new_val, data)
+
+        new_val = f"DATABASES_AVAILABLE = {{\n{sep}'jest': {{'ENGINE': 'django.db.backends.sqlite3', 'NAME': BASE_DIR / 'test_db.sqlite3', }},"
+        data = re.sub(r'DATABASES\s*=\s*\{', new_val, data)
+        db_pattern = self.balanced_pattern_factory('DATABASES_AVAILABLE = ')
+        db_settings = db_pattern.search(data).group()
+        data = db_pattern.sub(db_settings + f"\n\ndatabase = os.environ.get('DJANGO_DATABASE', 'default')\n\nDATABASES = {{'default': DATABASES_AVAILABLE[database]}}", data)
+
+        data += settings_extension
+
+        fout = open(self.get_settings_file_path(), "wt", encoding='utf-8')
+        fout.write(data)
+        fout.close()
+
+    def get_apps(self):
+        self.find_and_set_project_name()
+        app_list = [options.MAIN_APP_NAME]
+        for app_name in self.get_setting_vals().INSTALLED_APPS:
+            if os.path.exists(os.path.join(options.PROJECT_ROOT, app_name)) and app_name not in app_list:
+                app_list.append(app_name)
+
+        return app_list
+
+    def get_sdc_apps(self):
+        self.find_and_set_project_name()
+        app_list = []
+        for app_name in self.get_setting_vals().INSTALLED_APPS:
+            if os.path.exists(os.path.join(get_app_path(app_name), 'sdc_views.py')):
+                app_list.append(app_name)
+
+        return app_list
+
+
+
+
+
+    def get_main_url_path(self):
+        return os.path.join(options.PROJECT_ROOT, self.get_setting_vals().ROOT_URLCONF.replace(".", "/") + ".py")
+
+    def find_and_set_project_name(self):
+        options.setPROJECT(self.get_setting_vals().ROOT_URLCONF.split(".")[0])
+        print(options.PROJECT)
+
+    @classmethod
+    def balanced_pattern_factory(cls, prefix: str,  icon_start: str = r"\{", icon_end: str = r"\}") -> regex.regex:
+        return regex.compile(fr'{prefix}({icon_start}(?:[^{icon_start}{icon_end}]+|(?1))*{icon_end})')
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_cc.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_cc.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import sys
-import re
-
-from django.core.management.base import BaseCommand, CommandError
-
-from sdc_core.management.commands.init_add import settings_manager
-from sdc_core.management.commands.init_add.add_controller_manager import AddControllerManager
-from sdc_core.management.commands.sdc_update_links import make_link
-
-
-class Command(BaseCommand):
-    help = 'This function creates a new sdc controller and adds the django url parts'
-
-    def __init__(self, *args, **kwargs):
-        super(Command, self).__init__(*args, **kwargs)
-        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
-        self.sdc_settings = settings_manager.SettingsManager(manage_py_file_path)
-
-    def add_arguments(self, parser):
-        all_apps = self.sdc_settings.get_apps()
-        parser.add_argument('-c', '--controller_name', type=str, help='The name of the new controller as snake_case')
-        parser.add_argument('-a', '--app_name', type=str, help='The name of the django app: [%s]' % ', '.join(all_apps))
-
-
-    def check_snake_name(self, name):
-        x = re.search("[A-Z]", name)
-        if x:
-            raise CommandError('Lower case letters only.', 8)
-        x = re.search("[^0-9a-z_]", name)
-        if x:
-            raise CommandError("No special characters. Only lowercase letters, numbers and '_'", 9)
-        x = re.search("^[a-z]", name)
-        if not x:
-            raise CommandError("Only lowercase letters at first symbol", 10)
-
-        return True
-
-    def handle(self, *args, **ops):
-
-        self.sdc_settings.check_settings()
-
-        self.sdc_settings.find_and_set_project_name()
-        all_apps = self.sdc_settings.get_apps()
-
-        text = "Enter number to select an django App:"
-        for idx in range(1, len(all_apps)):
-            text += "\n%d -> %s" % (idx, all_apps[idx])
-        app_name = ops.get('app_name')
-        if app_name is None or not app_name in all_apps:
-            try:
-                idx = int(input(text + "\nEnter number: [%d]" % (len(all_apps) - 1)) or (len(all_apps) - 1))
-            except Exception as ex:
-                print(ex)
-                raise  CommandError("Input has to be a number between 1 and %d" % (len(all_apps) - 1), 4)
-
-            app_name = all_apps[idx]
-        controller_name = ops.get('controller_name')
-        if controller_name is None:
-            text = "Enter the name of the new controller (use snake_case):"
-            controller_name = str(input(text))
-
-        if not self.check_snake_name(controller_name):
-            exit(1)
-
-        add_sdc_core = AddControllerManager(app_name, controller_name)
-        if len(controller_name) == 0:
-            raise CommandError("Controller name must not be empty!", 5)
-        elif not add_sdc_core.check_if_url_is_unique():
-            raise CommandError("%s already exists. Controller name has to be unique!" % controller_name, 6)
-
-
-        add_sdc_core.add_url_to_url_pattern(self.sdc_settings.get_main_url_path())
-        add_sdc_core.add_view_class_to_sdc_views()
-        add_sdc_core.prepare_files()
-        add_sdc_core.add_to_organizer()
-        add_sdc_core.add_js_test()
+import sys
+import re
+
+from django.core.management.base import BaseCommand, CommandError
+
+from sdc_core.management.commands.init_add import settings_manager
+from sdc_core.management.commands.init_add.add_controller_manager import AddControllerManager
+from sdc_core.management.commands.sdc_update_links import make_link
+
+
+class Command(BaseCommand):
+    help = 'This function creates a new sdc controller and adds the django url parts'
+
+    def __init__(self, *args, **kwargs):
+        super(Command, self).__init__(*args, **kwargs)
+        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
+        self.sdc_settings = settings_manager.SettingsManager(manage_py_file_path)
+
+    def add_arguments(self, parser):
+        all_apps = self.sdc_settings.get_apps()
+        parser.add_argument('-c', '--controller_name', type=str, help='The name of the new controller as snake_case')
+        parser.add_argument('-a', '--app_name', type=str, help='The name of the django app: [%s]' % ', '.join(all_apps))
+
+
+    def check_snake_name(self, name):
+        x = re.search("[A-Z]", name)
+        if x:
+            raise CommandError('Lower case letters only.', 8)
+        x = re.search("[^0-9a-z_]", name)
+        if x:
+            raise CommandError("No special characters. Only lowercase letters, numbers and '_'", 9)
+        x = re.search("^[a-z]", name)
+        if not x:
+            raise CommandError("Only lowercase letters at first symbol", 10)
+
+        return True
+
+    def handle(self, *args, **ops):
+
+        self.sdc_settings.check_settings()
+
+        self.sdc_settings.find_and_set_project_name()
+        all_apps = self.sdc_settings.get_apps()
+
+        text = "Enter number to select an django App:"
+        for idx in range(1, len(all_apps)):
+            text += "\n%d -> %s" % (idx, all_apps[idx])
+        app_name = ops.get('app_name')
+        if app_name is None or not app_name in all_apps:
+            try:
+                idx = int(input(text + "\nEnter number: [%d]" % (len(all_apps) - 1)) or (len(all_apps) - 1))
+            except Exception as ex:
+                print(ex)
+                raise  CommandError("Input has to be a number between 1 and %d" % (len(all_apps) - 1), 4)
+
+            app_name = all_apps[idx]
+        controller_name = ops.get('controller_name')
+        if controller_name is None:
+            text = "Enter the name of the new controller (use snake_case):"
+            controller_name = str(input(text))
+
+        if not self.check_snake_name(controller_name):
+            exit(1)
+
+        add_sdc_core = AddControllerManager(app_name, controller_name)
+        if len(controller_name) == 0:
+            raise CommandError("Controller name must not be empty!", 5)
+        elif not add_sdc_core.check_if_url_is_unique():
+            raise CommandError("%s already exists. Controller name has to be unique!" % controller_name, 6)
+
+
+        add_sdc_core.add_url_to_url_pattern(self.sdc_settings.get_main_url_path())
+        add_sdc_core.add_view_class_to_sdc_views()
+        add_sdc_core.prepare_files()
+        add_sdc_core.add_to_organizer()
+        add_sdc_core.add_js_test()
         make_link(app_name, controller_name)
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_controller_infos.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_controller_infos.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                 # Check if the line contains the class definition
                 if f"class {class_name}(" in line:
                     return i
 
         return line_number
 
     def _parse_controller_to_info_json(self, app_name, controller_name):
-        controller_asset_dir = os.path.join(self.src_path, app_name, 'controller', controller_name)
         app = importlib.import_module(app_name)
         app_path = os.path.dirname(app.__file__)
         app_view_path = os.path.join(app_path, 'sdc_views.py')
         app_asset_path = os.path.join(app_path, 'Assets/src', app_name, 'controller')
         app_template_path = os.path.join(app_path, 'templates', app_name, 'sdc')
 
         view_class_name = convert_to_camel_case(controller_name)
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_get_model_infos.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_model_infos.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_init.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_init.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import os
-import sys
-
-from django.core.management.base import BaseCommand, CommandError
-
-from sdc_core.management.commands.init_add import options, settings_manager
-from sdc_core.management.commands.init_add.sdc_core_manager import add_sdc_to_main_urls, copy_apps
-from sdc_core.management.commands.init_add.utils import makedirs_if_not_exist, copy, copy_and_prepare, \
-    prepare_as_string
-from sdc_core.management.commands.sdc_update_links import make_app_links
-
-
-class Command(BaseCommand):
-    help = 'This function inits SDC in your django Project'
-
-    def add_arguments(self, parser):
-        pass
-
-    def handle(self, *args, **ops):
-        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
-
-        sdc_settings = settings_manager.SettingsManager(manage_py_file_path)
-        sdc_settings.check_settings()
-
-        sdc_settings.find_and_set_project_name()
-        sdc_settings.find_and_set_whitespace_sep()
-
-        project_app_root = os.path.join(options.PROJECT_ROOT, options.PROJECT)
-        main_static = os.path.join(options.PROJECT_ROOT, "Assets")
-        main_templates = os.path.join(options.PROJECT_ROOT, "templates")
-
-        if 'sdc_tools' in sdc_settings.get_setting_vals().INSTALLED_APPS:
-            raise CommandError("SimpleDomControl has initialized already!", 2)
-
-
-        sdc_settings.update_settings(prepare_as_string(os.path.join(options.SCRIPT_ROOT, "template_files", "settings_extension.py.txt"), options.REPLACEMENTS))
-
-        makedirs_if_not_exist(main_templates)
-        copy_apps()
-        copy(os.path.join(options.SCRIPT_ROOT, "template_files", "Assets"), main_static, options.REPLACEMENTS)
-        copy(os.path.join(options.SCRIPT_ROOT, "template_files", "templates"), main_templates, options.REPLACEMENTS)
-
-        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "routing.py.txt"),
-                         os.path.join(project_app_root, "routing.py"),
-                         options.REPLACEMENTS)
-
-        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "package.json"),
-                         os.path.join(options.PROJECT_ROOT, "package.json"),
-                         options.REPLACEMENTS)
-
-        asgi_file = os.path.join(project_app_root, "asgi.py")
-        if os.path.exists(asgi_file):
-            os.remove(asgi_file)
-
-        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "asgi.py.txt"),
-                         asgi_file,
-                         options.REPLACEMENTS)
-
-        add_sdc_to_main_urls(sdc_settings.get_main_url_path())
-        make_app_links('sdc_tools')
-        make_app_links('sdc_user')
+import os
+import sys
+
+from django.core.management.base import BaseCommand, CommandError
+
+from sdc_core.management.commands.init_add import options, settings_manager
+from sdc_core.management.commands.init_add.sdc_core_manager import add_sdc_to_main_urls, copy_apps
+from sdc_core.management.commands.init_add.utils import makedirs_if_not_exist, copy, copy_and_prepare, \
+    prepare_as_string
+from sdc_core.management.commands.sdc_update_links import make_app_links
+
+
+class Command(BaseCommand):
+    help = 'This function inits SDC in your django Project'
+
+    def add_arguments(self, parser):
+        pass
+
+    def handle(self, *args, **ops):
+        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
+
+        sdc_settings = settings_manager.SettingsManager(manage_py_file_path)
+        sdc_settings.check_settings()
+
+        sdc_settings.find_and_set_project_name()
+        sdc_settings.find_and_set_whitespace_sep()
+
+        project_app_root = os.path.join(options.PROJECT_ROOT, options.PROJECT)
+        main_static = os.path.join(options.PROJECT_ROOT, "Assets")
+        main_templates = os.path.join(options.PROJECT_ROOT, "templates")
+
+        if 'sdc_tools' in sdc_settings.get_setting_vals().INSTALLED_APPS:
+            raise CommandError("SimpleDomControl has initialized already!", 2)
+
+
+        sdc_settings.update_settings(prepare_as_string(os.path.join(options.SCRIPT_ROOT, "template_files", "settings_extension.py.txt"), options.REPLACEMENTS))
+
+        makedirs_if_not_exist(main_templates)
+        copy_apps()
+        copy(os.path.join(options.SCRIPT_ROOT, "template_files", "Assets"), main_static, options.REPLACEMENTS)
+        copy(os.path.join(options.SCRIPT_ROOT, "template_files", "templates"), main_templates, options.REPLACEMENTS)
+
+        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "routing.py.txt"),
+                         os.path.join(project_app_root, "routing.py"),
+                         options.REPLACEMENTS)
+
+        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "package.json"),
+                         os.path.join(options.PROJECT_ROOT, "package.json"),
+                         options.REPLACEMENTS)
+
+        asgi_file = os.path.join(project_app_root, "asgi.py")
+        if os.path.exists(asgi_file):
+            os.remove(asgi_file)
+
+        copy_and_prepare(os.path.join(options.SCRIPT_ROOT, "template_files", "asgi.py.txt"),
+                         asgi_file,
+                         options.REPLACEMENTS)
+
+        add_sdc_to_main_urls(sdc_settings.get_main_url_path())
+        make_app_links('sdc_tools')
+        make_app_links('sdc_user')
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_is_installed.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_is_installed.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_new_model.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_new_model.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import sys
-
-from django.core.management.base import BaseCommand
-from django.apps import apps
-from sdc_core.management.commands.init_add.add_model_manager import AddModelManager
-
-from sdc_core.management.commands.init_add import options, settings_manager
-from sdc_core.management.commands.sdc_update_links import make_model_link
-
-
-class Command(BaseCommand):
-    help = 'This function add a new SDC/Django model in your django project'
-
-    def __init__(self, *args, **kwargs):
-        super(Command, self).__init__(*args, **kwargs)
-        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
-        self.sdc_settings = settings_manager.SettingsManager(manage_py_file_path)
-
-    def add_arguments(self, parser):
-        all_apps = self.sdc_settings.get_apps()
-        parser.add_argument('-m', '--model_name', type=str, help='The name of the new django model class')
-        parser.add_argument('-a', '--app_name', type=str, help='The name of the django app: [%s]' % ', '.join(all_apps))
-
-    def handle(self, *args, **ops):
-
-        self.sdc_settings.check_settings()
-
-        self.sdc_settings.find_and_set_project_name()
-        self.sdc_settings.find_and_set_whitespace_sep()
-        all_apps = self.sdc_settings.get_apps()
-
-
-        app_name = ops.get('app_name')
-        if app_name is None or not app_name in all_apps:
-            text = "Enter number to select an django App:"
-            for idx in range(1, len(all_apps)):
-                text += "\n%d -> %s" % (idx, all_apps[idx])
-            idx = 1
-            try:
-                idx = int(input(text + "\nEnter number: [%d]" % (len(all_apps) - 1)) or (len(all_apps) - 1))
-            except Exception as ex:
-                print(ex)
-                print(options.CMD_COLORS.as_error("Input has to be a number between 1 and %d" % (len(all_apps) - 1)))
-                exit(1)
-
-            app_name = all_apps[idx]
-        model_name = ops.get('model_name')
-        if model_name is None:
-            text = "Enter the name of the new Model class name (use camel-case):"
-            model_name = str(input(text))
-
-        if model_name in [model.__name__ for model in apps.get_app_config(app_name).get_models()]:
-            exit(1)
-        if len(model_name) == 0:
-            print(options.CMD_COLORS.as_error("Controller name must not be empty!"))
-            exit(1)
-
-        add_sdc_core = AddModelManager(app_name, model_name)
-
-
-        add_sdc_core.add_model()
-        add_sdc_core.add_model_form()
-        add_sdc_core.add_model_template()
+import sys
+
+from django.core.management.base import BaseCommand
+from django.apps import apps
+from sdc_core.management.commands.init_add.add_model_manager import AddModelManager
+
+from sdc_core.management.commands.init_add import options, settings_manager
+from sdc_core.management.commands.sdc_update_links import make_model_link
+
+
+class Command(BaseCommand):
+    help = 'This function add a new SDC/Django model in your django project'
+
+    def __init__(self, *args, **kwargs):
+        super(Command, self).__init__(*args, **kwargs)
+        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
+        self.sdc_settings = settings_manager.SettingsManager(manage_py_file_path)
+
+    def add_arguments(self, parser):
+        all_apps = self.sdc_settings.get_apps()
+        parser.add_argument('-m', '--model_name', type=str, help='The name of the new django model class')
+        parser.add_argument('-a', '--app_name', type=str, help='The name of the django app: [%s]' % ', '.join(all_apps))
+
+    def handle(self, *args, **ops):
+
+        self.sdc_settings.check_settings()
+
+        self.sdc_settings.find_and_set_project_name()
+        self.sdc_settings.find_and_set_whitespace_sep()
+        all_apps = self.sdc_settings.get_apps()
+
+
+        app_name = ops.get('app_name')
+        if app_name is None or not app_name in all_apps:
+            text = "Enter number to select an django App:"
+            for idx in range(1, len(all_apps)):
+                text += "\n%d -> %s" % (idx, all_apps[idx])
+            idx = 1
+            try:
+                idx = int(input(text + "\nEnter number: [%d]" % (len(all_apps) - 1)) or (len(all_apps) - 1))
+            except Exception as ex:
+                print(ex)
+                print(options.CMD_COLORS.as_error("Input has to be a number between 1 and %d" % (len(all_apps) - 1)))
+                exit(1)
+
+            app_name = all_apps[idx]
+        model_name = ops.get('model_name')
+        if model_name is None:
+            text = "Enter the name of the new Model class name (use camel-case):"
+            model_name = str(input(text))
+
+        if model_name in [model.__name__ for model in apps.get_app_config(app_name).get_models()]:
+            exit(1)
+        if len(model_name) == 0:
+            print(options.CMD_COLORS.as_error("Controller name must not be empty!"))
+            exit(1)
+
+        add_sdc_core = AddModelManager(app_name, model_name)
+
+
+        add_sdc_core.add_model()
+        add_sdc_core.add_model_form()
+        add_sdc_core.add_model_template()
         make_model_link(app_name, model_name)
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_links.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_links.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,85 @@
-import os
-import sys
-
-from django.core.management.base import BaseCommand
-
-from sdc_core.management.commands.init_add import options, settings_manager
-from django.apps import apps
-
-from sdc_core.management.commands.init_add.settings_manager import get_app_path
-
-
-def relative_symlink(src, dst):
-    try:
-        os.unlink(dst)
-    except:
-        pass
-    dir = os.path.dirname(dst)
-    Src = os.path.relpath(src, dir)
-    Dst = os.path.join(dir, os.path.basename(src))
-    os.makedirs(dir, exist_ok=True)
-    return os.symlink(Src, Dst)
-
-def make_app_links(app_name):
-    app_root = get_app_path(app_name)
-    sdc_controller_link_dir = os.path.join(options.PROJECT_ROOT, "Assets/src", app_name)
-    sdc_controller_dir = os.path.join(app_root, "Assets/src", app_name)
-    if os.path.exists(sdc_controller_link_dir):
-        os.remove(sdc_controller_link_dir)
-    relative_symlink(sdc_controller_dir, sdc_controller_link_dir)
-
-    sdc_test_link = os.path.join(options.PROJECT_ROOT, "Assets/tests", f"{app_name}.test.js")
-    sdc_test_file = os.path.join(app_root, "Assets/tests", f"{app_name}.test.js")
-
-    relative_symlink(sdc_test_file, sdc_test_link)
-
-
-def make_link(app_name, controller_name):
-    make_app_links(app_name)
-    app_root = get_app_path(app_name)
-
-    sdc_controller_dir = os.path.join(app_root, "Assets/src", app_name, 'controller')
-    if os.path.exists(sdc_controller_dir):
-        sdc_c_dir = os.path.join(sdc_controller_dir, controller_name)
-        sdc_c_js = os.path.join(sdc_c_dir, "%s.js" % controller_name)
-        if os.path.isdir(sdc_c_dir) and os.path.isfile(sdc_c_js):
-            sdc_c_html = os.path.join(app_root, "templates", app_name, 'sdc',
-                                      "%s.html" % controller_name)
-            if os.path.isfile(sdc_c_html):
-                sdc_link_path = os.path.join(sdc_c_dir, "%s.html" % controller_name)
-                if os.path.exists(sdc_link_path):
-                    os.remove(sdc_link_path)
-                relative_symlink(sdc_c_html, sdc_link_path)
-
-
-def make_model_link(app_name, model_name):
-    sdc_dst_dir = os.path.join(get_app_path(app_name), "Assets/src", app_name, "models", model_name)
-    sdc_src_dir = os.path.join(options.PROJECT_ROOT, app_name, "templates", app_name, 'models', model_name)
-    if not os.path.exists(sdc_dst_dir):
-        os.makedirs(sdc_dst_dir)
-    if os.path.exists(sdc_src_dir):
-        for file in os.listdir(sdc_src_dir):
-            sdc_src_file = os.path.join(sdc_src_dir, file)
-            sdc_dst_file = os.path.join(sdc_dst_dir, file)
-            if os.path.isdir(sdc_dst_dir) and os.path.isfile(sdc_src_file):
-                relative_symlink(sdc_src_file, sdc_dst_file)
-
-
-class Command(BaseCommand):
-    help = 'This function links all templates into the controller directory'
-
-    def add_arguments(self, parser):
-        pass
-
-    def handle(self, *args, **ops):
-        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
-        settings = settings_manager.SettingsManager(manage_py_file_path)
-        all_apps = settings.get_sdc_apps()
-        for app_name in all_apps:
-            sdc_controller_list_dir = os.path.join(get_app_path(app_name), "Assets/src", app_name, "controller")
-            if os.path.exists(sdc_controller_list_dir):
-                for file in os.listdir(sdc_controller_list_dir):
-                    make_link(app_name, file)
-            for model in apps.get_app_config(app_name).get_models():
-                make_model_link(app_name, model.__name__)
+import os
+import sys
+
+from django.core.management.base import BaseCommand
+
+from sdc_core.management.commands.init_add import options, settings_manager
+from django.apps import apps
+
+from sdc_core.management.commands.init_add.settings_manager import get_app_path
+
+
+def relative_symlink(src, dst):
+    try:
+        os.unlink(dst)
+    except:
+        pass
+    dir = os.path.dirname(dst)
+    Src = os.path.relpath(src, dir)
+    Dst = os.path.join(dir, os.path.basename(src))
+    os.makedirs(dir, exist_ok=True)
+    return os.symlink(Src, Dst)
+
+def make_app_links(app_name):
+    app_root = get_app_path(app_name)
+    sdc_controller_link_dir = os.path.join(options.PROJECT_ROOT, "Assets/src", app_name)
+    sdc_controller_dir = os.path.join(app_root, "Assets/src", app_name)
+    if os.path.exists(sdc_controller_link_dir):
+        os.remove(sdc_controller_link_dir)
+    relative_symlink(sdc_controller_dir, sdc_controller_link_dir)
+
+    sdc_test_link_dir = os.path.join(options.PROJECT_ROOT, "Assets/tests")#, f"{app_name}.test.js")
+    sdc_test_file_dir = os.path.join(app_root, "Assets/tests")#, f"{app_name}.test.js")
+    for file in  os.listdir(sdc_test_file_dir):
+        if file.endswith('.test.js'):
+            relative_symlink(os.path.join(sdc_test_file_dir, file), os.path.join(sdc_test_link_dir, file))
+
+
+def make_link(app_name, controller_name):
+    make_app_links(app_name)
+    app_root = get_app_path(app_name)
+
+    sdc_controller_dir = os.path.join(app_root, "Assets/src", app_name, 'controller')
+    if os.path.exists(sdc_controller_dir):
+        sdc_c_dir = os.path.join(sdc_controller_dir, controller_name)
+        sdc_c_js = os.path.join(sdc_c_dir, "%s.js" % controller_name)
+        if os.path.isdir(sdc_c_dir) and os.path.isfile(sdc_c_js):
+            sdc_c_html = os.path.join(app_root, "templates", app_name, 'sdc',
+                                      "%s.html" % controller_name)
+            if os.path.isfile(sdc_c_html):
+                sdc_link_path = os.path.join(sdc_c_dir, "%s.html" % controller_name)
+                if os.path.exists(sdc_link_path):
+                    os.remove(sdc_link_path)
+                relative_symlink(sdc_c_html, sdc_link_path)
+
+
+def make_model_link(app_name, model_name):
+    sdc_dst_dir = os.path.join(get_app_path(app_name), "Assets/src", app_name, "models", model_name)
+    sdc_src_dir = os.path.join(options.PROJECT_ROOT, app_name, "templates", app_name, 'models', model_name)
+    if not os.path.exists(sdc_dst_dir):
+        os.makedirs(sdc_dst_dir)
+    if os.path.exists(sdc_src_dir):
+        for file in os.listdir(sdc_src_dir):
+            sdc_src_file = os.path.join(sdc_src_dir, file)
+            sdc_dst_file = os.path.join(sdc_dst_dir, file)
+            if os.path.isdir(sdc_dst_dir) and os.path.isfile(sdc_src_file):
+                relative_symlink(sdc_src_file, sdc_dst_file)
+
+
+class Command(BaseCommand):
+    help = 'This function links all templates into the controller directory'
+
+    def add_arguments(self, parser):
+        pass
+
+    def handle(self, *args, **ops):
+        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
+        settings = settings_manager.SettingsManager(manage_py_file_path)
+        all_apps = settings.get_sdc_apps()
+        for app_name in all_apps:
+            sdc_controller_list_dir = os.path.join(get_app_path(app_name), "Assets/src", app_name, "controller")
+            if os.path.exists(sdc_controller_list_dir):
+                for file in os.listdir(sdc_controller_list_dir):
+                    make_link(app_name, file)
+            for model in apps.get_app_config(app_name).get_models():
+                make_model_link(app_name, model.__name__)
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/management/commands/sdc_update_url.py` & `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_url.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import os
-import re
-import sys
-
-from django.core.management.base import BaseCommand
-
-from sdc_core.management.commands.init_add import options, settings_manager
-from sdc_core.management.commands.init_add.add_controller_manager import AddControllerManager
-
-
-def change_content_url(file_path, app_name, controller_name):
-    fin = open(file_path, 'rt')
-    data = ""
-    app_controller = AddControllerManager(app_name, controller_name)
-    new_url_line = '"%s"; //%s' % (app_controller.get_template_url_sync(), app_controller.prepare_tag_name())
-    regexp = re.compile(r'(\s*this.)contentUrl *= *.*')
-    is_done = False
-    for line in fin:
-        match = regexp.match(line)
-        if not is_done and match:
-            line = regexp.sub(r'\1contentUrl = %s' % new_url_line, line)
-            is_done = True
-        data += line
-
-    fin.close()
-    fout = open(file_path, 'wt')
-    fout.write(data)
-    fout.close()
-
-
-class Command(BaseCommand):
-    help = 'This function updates all content urls of the SDC controller'
-
-    def add_arguments(self, parser):
-        pass
-
-    def handle(self, *args, **ops):
-        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
-        settings = settings_manager.SettingsManager(manage_py_file_path)
-        all_apps = settings.get_apps()
-        for app_name in all_apps[1:]:
-            sdc_js_dir = os.path.join(options.PROJECT_ROOT, "Assets/src", app_name, "controller")
-            if os.path.exists(sdc_js_dir):
-                for file in os.listdir(sdc_js_dir):
-                    sdc_c_dir = os.path.join(sdc_js_dir, file)
-                    sdc_c_js = os.path.join(str(sdc_c_dir), "%s.js" % file)
-                    if os.path.isdir(sdc_c_dir) and os.path.isfile(sdc_c_js):
-                        controller_name_sc = file
-                        change_content_url(sdc_c_js, app_name, controller_name_sc)
+import os
+import re
+import sys
+
+from django.core.management.base import BaseCommand
+
+from sdc_core.management.commands.init_add import options, settings_manager
+from sdc_core.management.commands.init_add.add_controller_manager import AddControllerManager
+
+
+def change_content_url(file_path, app_name, controller_name):
+    fin = open(file_path, 'rt')
+    data = ""
+    app_controller = AddControllerManager(app_name, controller_name)
+    new_url_line = '"%s"; //%s' % (app_controller.get_template_url_sync(), app_controller.prepare_tag_name())
+    regexp = re.compile(r'(\s*this.)contentUrl *= *.*')
+    is_done = False
+    for line in fin:
+        match = regexp.match(line)
+        if not is_done and match:
+            line = regexp.sub(r'\1contentUrl = %s' % new_url_line, line)
+            is_done = True
+        data += line
+
+    fin.close()
+    fout = open(file_path, 'wt')
+    fout.write(data)
+    fout.close()
+
+
+class Command(BaseCommand):
+    help = 'This function updates all content urls of the SDC controller'
+
+    def add_arguments(self, parser):
+        pass
+
+    def handle(self, *args, **ops):
+        manage_py_file_path = sys.argv[0] if len(sys.argv) > 0 else 'manage.py'
+        settings = settings_manager.SettingsManager(manage_py_file_path)
+        all_apps = settings.get_apps()
+        for app_name in all_apps[1:]:
+            sdc_js_dir = os.path.join(options.PROJECT_ROOT, "Assets/src", app_name, "controller")
+            if os.path.exists(sdc_js_dir):
+                for file in os.listdir(sdc_js_dir):
+                    sdc_c_dir = os.path.join(sdc_js_dir, file)
+                    sdc_c_js = os.path.join(str(sdc_c_dir), "%s.js" % file)
+                    if os.path.isdir(sdc_c_dir) and os.path.isfile(sdc_c_js):
+                        controller_name_sc = file
+                        change_content_url(sdc_c_js, app_name, controller_name_sc)
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/forms.py` & `simpledomcontrol-0.5.0/sdc_core/sdc_extentions/forms.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from django import forms
-from django.utils.translation import gettext_lazy as _
-
-class AbstractSearchForm(forms.Form):
-    CHOICES = ()
-    SEARCH_FIELDS = ()
-    DEFAULT_CHOICES = ""
-    NO_RESULTS_ON_EMPTY_SEARCH = False
-    PLACEHOLDER = _('Search')
-    search = forms.CharField(label=_('Search'), required=False, max_length=100, initial='')
-    order_by = forms.ChoiceField(widget=forms.Select, required=False, choices=CHOICES)
-    range_start = forms.IntegerField(widget=forms.HiddenInput(), required=False, initial=0)
-    _method = forms.CharField(widget=forms.HiddenInput(), required=True, initial='search')
-
-
-    def __init__(self, data=None, *args, **kwargs):
-        auto_id= self.__class__.__name__ + "_%s"
-        if len(data) == 0:
-            data = None
-        super(AbstractSearchForm, self).__init__(data, auto_id=auto_id, *args, **kwargs)
-        self.fields['search'].widget.attrs['placeholder'] = self.PLACEHOLDER
-        if len(self.CHOICES) == 0:
-            del self.fields["order_by"]
-        else:
-            self.fields['order_by'].choices = self.CHOICES
+from django import forms
+from django.utils.translation import gettext_lazy as _
+
+class AbstractSearchForm(forms.Form):
+    CHOICES = ()
+    SEARCH_FIELDS = ()
+    DEFAULT_CHOICES = ""
+    NO_RESULTS_ON_EMPTY_SEARCH = False
+    PLACEHOLDER = _('Search')
+    search = forms.CharField(label=_('Search'), required=False, max_length=100, initial='')
+    order_by = forms.ChoiceField(widget=forms.Select, required=False, choices=CHOICES)
+    range_start = forms.IntegerField(widget=forms.HiddenInput(), required=False, initial=0)
+    _method = forms.CharField(widget=forms.HiddenInput(), required=True, initial='search')
+
+
+    def __init__(self, data=None, *args, **kwargs):
+        auto_id= self.__class__.__name__ + "_%s"
+        if len(data) == 0:
+            data = None
+        super(AbstractSearchForm, self).__init__(data, auto_id=auto_id, *args, **kwargs)
+        self.fields['search'].widget.attrs['placeholder'] = self.PLACEHOLDER
+        if len(self.CHOICES) == 0:
+            del self.fields["order_by"]
+        else:
+            self.fields['order_by'].choices = self.CHOICES
             self.fields['order_by'].initial = self.DEFAULT_CHOICES
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/models.py` & `simpledomcontrol-0.5.0/sdc_core/sdc_extentions/models.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_core/sdc_extentions/search.py` & `simpledomcontrol-0.5.0/sdc_core/sdc_extentions/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from django.db.models import Q
-
-def generate_q_key_value_request(key, val):
-    map_val = {key + '__icontains': val}
-    return Q(**map_val)
-
-
-def handle_search_form(query_set, search_form, filter_dict=None, range=0):
-    if not search_form.is_valid():
-        data = {}
-    else:
-        data = search_form.cleaned_data
-
-    key_word = data.get('search', None)
-    does_order = len(search_form.CHOICES) > 0
-    order_by = None
-    if(does_order):
-        order_by = data.get('order_by', search_form.DEFAULT_CHOICES)
-
-    if filter_dict is not None:
-        query_set = query_set.filter(**filter_dict)
-    else:
-        pass#query_set = query_set.all()
-    query_set_count = 0
-    if key_word is not None and key_word != '':
-        q_list = None
-        for key in search_form.SEARCH_FIELDS:
-            if q_list is None:
-                q_list = generate_q_key_value_request(key, key_word)
-            else:
-                q_list = q_list | generate_q_key_value_request(key, key_word)
-        query_set = query_set.filter(q_list)
-        query_set_count = query_set.count()
-    elif(search_form.NO_RESULTS_ON_EMPTY_SEARCH):
-        query_set = []
-    else:
-        query_set_count = query_set.count()
-
-
-    if(does_order):
-        query_set = query_set.order_by(order_by)
-
-    context = {
-        'total_count': query_set_count,
-        'search_form': search_form
-    }
-
-    if range > 0:
-        from_idx = data.get('range_start', 0)
-        if from_idx >= query_set_count:
-            from_idx = max(query_set_count - 2, 0)
-
-        to_idx = min(from_idx + range, query_set_count)
-        query_set = query_set[from_idx:to_idx]
-        context['range'] = [from_idx + 1, to_idx]
-        context['range_size'] = range
-
-    context['instances'] = query_set
-    return context
+from django.db.models import Q
+
+def generate_q_key_value_request(key, val):
+    map_val = {key + '__icontains': val}
+    return Q(**map_val)
+
+
+def handle_search_form(query_set, search_form, filter_dict=None, range=0):
+    if not search_form.is_valid():
+        data = {}
+    else:
+        data = search_form.cleaned_data
+
+    key_word = data.get('search', None)
+    does_order = len(search_form.CHOICES) > 0
+    order_by = None
+    if(does_order):
+        order_by = data.get('order_by', search_form.DEFAULT_CHOICES)
+
+    if filter_dict is not None:
+        query_set = query_set.filter(**filter_dict)
+    else:
+        pass#query_set = query_set.all()
+    query_set_count = 0
+    if key_word is not None and key_word != '':
+        q_list = None
+        for key in search_form.SEARCH_FIELDS:
+            if q_list is None:
+                q_list = generate_q_key_value_request(key, key_word)
+            else:
+                q_list = q_list | generate_q_key_value_request(key, key_word)
+        query_set = query_set.filter(q_list).distinct()
+        query_set_count = query_set.count()
+    elif(search_form.NO_RESULTS_ON_EMPTY_SEARCH):
+        query_set = []
+    else:
+        query_set_count = query_set.count()
+
+
+    if(does_order):
+        query_set = query_set.order_by(order_by)
+
+    context = {
+        'total_count': query_set_count,
+        'search_form': search_form
+    }
+
+    if range > 0:
+        from_idx = data.get('range_start', 0)
+        if from_idx >= query_set_count:
+            from_idx = max(query_set_count - 2, 0)
+
+        to_idx = min(from_idx + range, query_set_count)
+        query_set = query_set[from_idx:to_idx]
+        context['range'] = [from_idx + 1, to_idx]
+        context['range_size'] = range
+
+    context['instances'] = query_set
+    return context
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx` & `simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,19 @@
     output: {
         path: outputDir,
         filename: '[name].js'
     },
     module: {
         rules: [
             {
+                test: /\.js$/,
+                exclude: /node_modules/,
+                use: ['babel-loader']
+            },
+            {
                 test: /\.s[ac]ss$/i,
                 use: [{
                     loader: 'style-loader', // inject CSS to page
                 }, {
                     loader: 'css-loader', // translates CSS into CommonJS modules
                 }, {
                     loader: 'postcss-loader', // Run post css actions
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx` & `simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-const path = require('path');
 const TerserPlugin = require("terser-webpack-plugin");
 let default_conf = require('./webpack.default.config.jsx');
 const _ = require("lodash");
 
 
 const prod_conf = {
     mode: 'production',
-    entry: {
-        'index.organizer': path.resolve(__dirname, '../_build/index.organizer.js'),
-    },
 
     optimization: {
         minimize: true,
         minimizer: [
             new TerserPlugin({
                 test: /\.js(\?.*)?$/i,
                 terserOptions: {
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt` & `simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-1) Uncomend sdc_user in "project_app"/settings.py INSTALLED_APPS: (replace project_app by the app name of your project)
-...
-INSTALLED_APPS = [
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'sdc_core',
-    'sdc_tools',
-    'sdc_user' # <--
-]
-
-2) Uncomend AUTH_USER_MODEL in "project_app"/settings.py INSTALLED_APPS: (replace project_app by the app name of your project)
-...
-AUTH_USER_MODEL = 'sdc_user.CustomUser'
-...
-
-3) Uncomend the import in sdc_core/consumer.py :
-...
-from sdc_user import sdc_views as sdc_user # <--
-...
-
-4) Uncomend the import in "project_app"/url.py: (replace project_app by the app name of your project)
-...
-urlpatterns = [
-    path('sdc_view/sdc_tools/', include('sdc_tools.sdc_urls')),
-    path('sdc_view/sdc_user/', include('sdc_user.sdc_urls')), # <--
-    # scd view below
-...
-
-5)  Uncomend the import in sdc_core/static/index.organizerl.js:
-...
-import {} from "./sdc_tools/js/sdc_tools.organizer.js"
-import {} from "./sdc_user/js/test_app_two.organizer.js" // <--
-import {app} from './simpleDomControl/sdc_main.js';
+1) Uncomend sdc_user in "project_app"/settings.py INSTALLED_APPS: (replace project_app by the app name of your project)
+...
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    'sdc_core',
+    'sdc_tools',
+    'sdc_user' # <--
+]
+
+2) Uncomend AUTH_USER_MODEL in "project_app"/settings.py INSTALLED_APPS: (replace project_app by the app name of your project)
+...
+AUTH_USER_MODEL = 'sdc_user.CustomUser'
+...
+
+3) Uncomend the import in sdc_core/consumer.py :
+...
+from sdc_user import sdc_views as sdc_user # <--
+...
+
+4) Uncomend the import in "project_app"/url.py: (replace project_app by the app name of your project)
+...
+urlpatterns = [
+    path('sdc_view/sdc_tools/', include('sdc_tools.sdc_urls')),
+    path('sdc_view/sdc_user/', include('sdc_user.sdc_urls')), # <--
+    # scd view below
+...
+
+5)  Uncomend the import in sdc_core/static/index.organizerl.js:
+...
+import {} from "./sdc_tools/js/sdc_tools.organizer.js"
+import {} from "./sdc_user/js/test_app_two.organizer.js" // <--
+import {app} from './simpleDomControl/sdc_main.js';
 ...
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/apps/sdc_examples/index.html` & `simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/index.html`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-{% extends "base.html" %}
-
-{% load addclass %}
-{% load static %}
-{% load i18n %}
-
-{% block title %}Title{% endblock %}
-
-{% block scripts %}
-    <script type="module" src="{% static 'index.organizer.js' %}?{% random_tag 5 %}"></script>
-{% endblock %}
-
-{% block content %}
-    <g-alert-msg></g-alert-msg>
-    <global-dom-events></global-dom-events>
-
-    <!-- nav view controller ind sdc_tools -->
-    <!-- data-default-controller sets the default view -->
-    <nav-view data-default-controller="second-view">
-        <!-- .header-loading element will have an addition class .active while loading -->
-        <div class="header-loading">
-            <h1>{% trans 'loading...' %}</h1>
-        </div>
-        <nav class="navbar navbar-expand-lg navbar-light bg-light">
-            <a class="navbar-brand navigation-links"
-               href="{% url 'sdc_index' %}~first-view">{% trans 'First' %}</a>
-            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
-                <span class="navbar-toggler-icon"></span>
-            </button>
-            <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
-                <div class="navbar-nav nav-menu-set menu-1 active">
-                    <!-- .navigation-links is automatically handled by the nav-view controller-->
-                    <a class="nav-item nav-link navigation-links"
-                       href="{% url 'sdc_index' %}~second-view~&pk=-1">{% trans 'Second' %}</a>
-                    <a class="nav-item nav-link navigation-links"
-                       href="{% url 'sdc_index' %}~third-view">{% trans 'Third' %}</a>
-                </div>
-                <!-- Alternative menu. It changes Navbar for each controller which have this.menu_id = 2; -->
-                <!-- this.menu_id = 0; keeps current menu bar -->
-                <div class="navbar-nav nav-menu-set menu-2">
-                    <a class="nav-item nav-link navigation-links"
-                       href="{% url 'sdc_index' %}~third-view~fifth-view">{% trans 'Fifth' %}</a>
-                    <a class="nav-item nav-link navigation-links"
-                       href="{% url 'sdc_index' %}~third-view~fourth-view">{% trans 'Fourth' %}</a>
-                </div>
-            </div>
-        </nav>
-    </nav-view>
-{% endblock %}
-
+{% extends "base.html" %}
+
+{% load addclass %}
+{% load static %}
+{% load i18n %}
+
+{% block title %}Title{% endblock %}
+
+{% block scripts %}
+    <script type="module" src="{% static 'index.organizer.js' %}?{% random_tag 5 %}"></script>
+{% endblock %}
+
+{% block content %}
+    <g-alert-msg></g-alert-msg>
+    <global-dom-events></global-dom-events>
+
+    <!-- nav view controller ind sdc_tools -->
+    <!-- data-default-controller sets the default view -->
+    <nav-view data-default-controller="second-view">
+        <!-- .header-loading element will have an addition class .active while loading -->
+        <div class="header-loading">
+            <h1>{% trans 'loading...' %}</h1>
+        </div>
+        <nav class="navbar navbar-expand-lg navbar-light bg-light">
+            <a class="navbar-brand navigation-links"
+               href="{% url 'sdc_index' %}~first-view">{% trans 'First' %}</a>
+            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
+                <span class="navbar-toggler-icon"></span>
+            </button>
+            <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
+                <div class="navbar-nav nav-menu-set menu-1 active">
+                    <!-- .navigation-links is automatically handled by the nav-view controller-->
+                    <a class="nav-item nav-link navigation-links"
+                       href="{% url 'sdc_index' %}~second-view~&pk=-1">{% trans 'Second' %}</a>
+                    <a class="nav-item nav-link navigation-links"
+                       href="{% url 'sdc_index' %}~third-view">{% trans 'Third' %}</a>
+                </div>
+                <!-- Alternative menu. It changes Navbar for each controller which have this.menu_id = 2; -->
+                <!-- this.menu_id = 0; keeps current menu bar -->
+                <div class="navbar-nav nav-menu-set menu-2">
+                    <a class="nav-item nav-link navigation-links"
+                       href="{% url 'sdc_index' %}~third-view~fifth-view">{% trans 'Fifth' %}</a>
+                    <a class="nav-item nav-link navigation-links"
+                       href="{% url 'sdc_index' %}~third-view~fourth-view">{% trans 'Fourth' %}</a>
+                </div>
+            </div>
+        </nav>
+    </nav-view>
+{% endblock %}
+
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/asgi.py.txt` & `simpledomcontrol-0.5.0/sdc_core/template_files/asgi.py.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""
-ASGI config for §PROJECT§ project.
-
-It exposes the ASGI callable as a module-level variable named ``application``.
-
-To run it using daphne set DEBUG to false and then execute the following commmand:
-env ALLOWED_HOST=http://localhost:8000 daphne §PROJECT§.asgi:application
-
-For more information on this file, see
-https://docs.djangoproject.com/en/3.1/howto/deployment/asgi/
-"""
-
-import os
-os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'ElnAdapter.settings')
-
-import django
-django.setup()
-
-from channels.auth import AuthMiddlewareStack
-from channels.routing import ProtocolTypeRouter, URLRouter
-from . import routing
-from django.core.asgi import get_asgi_application
-
-application = ProtocolTypeRouter({
-    "http": get_asgi_application(),
-    "websocket": AuthMiddlewareStack(
-        URLRouter(
-            routing.websocket_urlpatterns
-        )
-    ),
+"""
+ASGI config for §PROJECT§ project.
+
+It exposes the ASGI callable as a module-level variable named ``application``.
+
+To run it using daphne set DEBUG to false and then execute the following commmand:
+env ALLOWED_HOST=http://localhost:8000 daphne §PROJECT§.asgi:application
+
+For more information on this file, see
+https://docs.djangoproject.com/en/3.1/howto/deployment/asgi/
+"""
+
+import os
+os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'ElnAdapter.settings')
+
+import django
+django.setup()
+
+from channels.auth import AuthMiddlewareStack
+from channels.routing import ProtocolTypeRouter, URLRouter
+from . import routing
+from django.core.asgi import get_asgi_application
+
+application = ProtocolTypeRouter({
+    "http": get_asgi_application(),
+    "websocket": AuthMiddlewareStack(
+        URLRouter(
+            routing.websocket_urlpatterns
+        )
+    ),
 })
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_controller.js.txt` & `simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,89 @@
 00000000: 696d 706f 7274 207b 4162 7374 7261 6374  import {Abstract
-00000010: 5344 432c 2061 7070 7d20 6672 6f6d 2027  SDC, app} from '
-00000020: 7364 635f 636c 6965 6e74 273b 0d0a 0d0a  sdc_client';....
-00000030: 0d0a 636c 6173 7320 c2a7 434f 4e54 524f  ..class ..CONTRO
-00000040: 4c4c 4552 4e41 4d45 5449 544c 45c2 a743  LLERNAMETITLE..C
-00000050: 6f6e 7472 6f6c 6c65 7220 6578 7465 6e64  ontroller extend
-00000060: 7320 4162 7374 7261 6374 5344 4320 7b0d  s AbstractSDC {.
-00000070: 0a0d 0a20 2020 2063 6f6e 7374 7275 6374  ...    construct
-00000080: 6f72 2829 207b 0d0a 2020 2020 2020 2020  or() {..        
-00000090: 7375 7065 7228 293b 0d0a 2020 2020 2020  super();..      
-000000a0: 2020 7468 6973 2e63 6f6e 7465 6e74 5572    this.contentUr
-000000b0: 6c20 3d20 22c2 a754 454d 504c 4154 4555  l = "..TEMPLATEU
-000000c0: 524c c2a7 223b 202f 2fc2 a754 4147 4e41  RL.."; //..TAGNA
-000000d0: 4d45 c2a7 0d0a 0d0a 2020 2020 2020 2020  ME......        
-000000e0: 2f2a 2a0d 0a20 2020 2020 2020 2020 2a20  /**..         * 
-000000f0: 4576 656e 7473 2069 7320 616e 2061 7272  Events is an arr
-00000100: 6179 206f 6620 646f 6d20 6576 656e 7473  ay of dom events
-00000110: 2e0d 0a20 2020 2020 2020 2020 2a20 5468  ...         * Th
-00000120: 6520 7061 7474 6572 6e20 6973 207b 2765  e pattern is {'e
-00000130: 7665 6e74 273a 207b 2764 6f6d 5f73 656c  vent': {'dom_sel
-00000140: 6563 746f 7227 3a20 6861 6e64 6c65 727d  ector': handler}
-00000150: 7d0d 0a20 2020 2020 2020 2020 2a20 556e  }..         * Un
-00000160: 636f 6d6d 656e 6420 7468 6520 666f 6c6c  commend the foll
-00000170: 6f77 696e 6720 6c69 6e65 2074 6f20 6164  owing line to ad
-00000180: 6420 6576 656e 7473 3b0d 0a20 2020 2020  d events;..     
-00000190: 2020 2020 2a2f 0d0a 2020 2020 2020 2020      */..        
-000001a0: 2f2f 2074 6869 732e 6576 656e 7473 2e75  // this.events.u
-000001b0: 6e73 6869 6674 287b 2763 6c69 636b 273a  nshift({'click':
-000001c0: 207b 272e 6865 6164 6572 2d73 616d 706c   {'.header-sampl
-000001d0: 6527 3a20 2865 762c 2024 656c 656d 293d  e': (ev, $elem)=
-000001e0: 3e20 2465 6c65 6d2e 6373 7328 2762 6f72  > $elem.css('bor
-000001f0: 6465 7227 2c20 2732 7078 2073 6f6c 6964  der', '2px solid
-00000200: 2062 6c61 636b 2729 7d7d 7d29 3b0d 0a20   black')}}});.. 
-00000210: 2020 207d 0d0a 0d0a 2020 2020 2f2f 2d2d     }....    //--
-00000220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2f  ---------------/
-00000250: 2f0d 0a20 2020 202f 2f20 4c69 6665 6379  /..    // Lifecy
-00000260: 636c 6520 6861 6e64 6c65 7220 2020 2020  cle handler     
-00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000280: 2020 2020 2020 2020 2020 2f2f 0d0a 2020            //..  
-00000290: 2020 2f2f 202d 206f 6e49 6e69 7420 2874    // - onInit (t
-000002a0: 6167 2070 6172 616d 6574 6572 2920 2020  ag parameter)   
-000002b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002c0: 2020 2020 202f 2f0d 0a20 2020 202f 2f20       //..    // 
-000002d0: 2d20 6f6e 4c6f 6164 2028 444f 4d20 6e6f  - onLoad (DOM no
-000002e0: 7420 7365 7429 2020 2020 2020 2020 2020  t set)          
-000002f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000300: 2f2f 0d0a 2020 2020 2f2f 202d 2077 696c  //..    // - wil
-00000310: 6c53 686f 7720 2028 444f 4d20 7365 7429  lShow  (DOM set)
-00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000330: 2020 2020 2020 2020 2020 202f 2f0d 0a20             //.. 
-00000340: 2020 202f 2f20 2d20 6f6e 5265 6672 6573     // - onRefres
-00000350: 6820 2028 7265 6361 6c6c 6564 206f 6e20  h  (recalled on 
-00000360: 7265 6c6f 6164 2920 2020 2020 2020 2020  reload)         
-00000370: 2020 2020 202f 2f0d 0a20 2020 202f 2f2d       //..    //-
-00000380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000010: 5344 432c 2061 7070 2c20 7472 6967 6765  SDC, app, trigge
+00000020: 722c 2073 6f63 6b65 7452 6563 6f6e 6e65  r, socketReconne
+00000030: 6374 7d20 6672 6f6d 2027 7364 635f 636c  ct} from 'sdc_cl
+00000040: 6965 6e74 273b 0a0a 636c 6173 7320 5364  ient';..class Sd
+00000050: 634c 6f67 6f75 7443 6f6e 7472 6f6c 6c65  cLogoutControlle
+00000060: 7220 6578 7465 6e64 7320 4162 7374 7261  r extends Abstra
+00000070: 6374 5344 4320 7b0a 0a20 2020 2063 6f6e  ctSDC {..    con
+00000080: 7374 7275 6374 6f72 2829 207b 0a20 2020  structor() {.   
+00000090: 2020 2020 2073 7570 6572 2829 3b0a 2020       super();.  
+000000a0: 2020 2020 2020 7468 6973 2e63 6f6e 7465        this.conte
+000000b0: 6e74 5572 6c20 3d20 222f 7364 635f 7669  ntUrl = "/sdc_vi
+000000c0: 6577 2f73 6463 5f75 7365 722f 7364 635f  ew/sdc_user/sdc_
+000000d0: 6c6f 676f 7574 223b 202f 2f3c 7364 632d  logout"; //<sdc-
+000000e0: 6c6f 676f 7574 3e3c 2f73 6463 2d6c 6f67  logout></sdc-log
+000000f0: 6f75 743e 0a0a 2020 2020 2020 2020 2f2a  out>..        /*
+00000100: 2a0a 2020 2020 2020 2020 202a 2045 7665  *.         * Eve
+00000110: 6e74 7320 6973 2061 6e20 6172 7261 7920  nts is an array 
+00000120: 6f66 2064 6f6d 2065 7665 6e74 732e 0a20  of dom events.. 
+00000130: 2020 2020 2020 2020 2a20 5468 6520 7061          * The pa
+00000140: 7474 6572 6e20 6973 207b 2765 7665 6e74  ttern is {'event
+00000150: 273a 207b 2764 6f6d 5f73 656c 6563 746f  ': {'dom_selecto
+00000160: 7227 3a20 6861 6e64 6c65 727d 7d0a 2020  r': handler}}.  
+00000170: 2020 2020 2020 202a 2055 6e63 6f6d 6d65         * Uncomme
+00000180: 6e64 2074 6865 2066 6f6c 6c6f 7769 6e67  nd the following
+00000190: 206c 696e 6520 746f 2061 6464 2065 7665   line to add eve
+000001a0: 6e74 733b 0a20 2020 2020 2020 2020 2a2f  nts;.         */
+000001b0: 0a20 2020 2020 2020 202f 2f20 7468 6973  .        // this
+000001c0: 2e65 7665 6e74 732e 756e 7368 6966 7428  .events.unshift(
+000001d0: 7b27 636c 6963 6b27 3a20 7b27 2e68 6561  {'click': {'.hea
+000001e0: 6465 722d 7361 6d70 6c65 273a 2028 6576  der-sample': (ev
+000001f0: 2c20 2465 6c65 6d29 3d3e 2024 656c 656d  , $elem)=> $elem
+00000200: 2e63 7373 2827 626f 7264 6572 272c 2027  .css('border', '
+00000210: 3270 7820 736f 6c69 6420 626c 6163 6b27  2px solid black'
+00000220: 297d 7d7d 293b 0a20 2020 207d 0a0a 2020  )}}});.    }..  
+00000230: 2020 2f2f 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    //------------
+00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000260: 2d2d 2d2d 2d2f 2f0a 2020 2020 2f2f 204c  -----//.    // L
+00000270: 6966 6563 7963 6c65 2068 616e 646c 6572  ifecycle handler
+00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000290: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+000002a0: 2f0a 2020 2020 2f2f 202d 206f 6e49 6e69  /.    // - onIni
+000002b0: 7420 2874 6167 2070 6172 616d 6574 6572  t (tag parameter
+000002c0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+000002d0: 2020 2020 2020 2020 202f 2f0a 2020 2020           //.    
+000002e0: 2f2f 202d 206f 6e4c 6f61 6420 2844 4f4d  // - onLoad (DOM
+000002f0: 206e 6f74 2073 6574 2920 2020 2020 2020   not set)       
+00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000310: 2020 202f 2f0a 2020 2020 2f2f 202d 2077     //.    // - w
+00000320: 696c 6c53 686f 7720 2028 444f 4d20 7365  illShow  (DOM se
+00000330: 7429 2020 2020 2020 2020 2020 2020 2020  t)              
+00000340: 2020 2020 2020 2020 2020 2020 202f 2f0a               //.
+00000350: 2020 2020 2f2f 202d 206f 6e52 6566 7265      // - onRefre
+00000360: 7368 2020 2872 6563 616c 6c65 6420 6f6e  sh  (recalled on
+00000370: 2072 656c 6f61 6429 2020 2020 2020 2020   reload)        
+00000380: 2020 2020 2020 2f2f 0a20 2020 202f 2f2d        //.    //-
 00000390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000003a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003b0: 2f2f 0d0a 2020 2020 2f2f 202d 206f 6e52  //..    // - onR
-000003c0: 656d 6f76 6520 2020 2020 2020 2020 2020  emove           
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 2020 2020 2020 2020 202f 2f0d 0a20             //.. 
-000003f0: 2020 202f 2f2d 2d2d 2d2d 2d2d 2d2d 2d2d     //-----------
-00000400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003c0: 2f2f 0a20 2020 202f 2f20 2d20 6f6e 5265  //.    // - onRe
+000003d0: 6d6f 7665 2020 2020 2020 2020 2020 2020  move            
+000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003f0: 2020 2020 2020 2020 2020 2f2f 0a20 2020            //.   
+00000400: 202f 2f2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   //-------------
 00000410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000420: 2d2d 2d2d 2d2d 2f2f 0d0a 0d0a 2020 2020  ------//....    
-00000430: 6f6e 496e 6974 2829 207b 0d0a 2020 2020  onInit() {..    
-00000440: 7d0d 0a0d 0a20 2020 206f 6e4c 6f61 6428  }....    onLoad(
-00000450: 2468 746d 6c29 207b 0d0a 2020 2020 2020  $html) {..      
-00000460: 2020 7265 7475 726e 2073 7570 6572 2e6f    return super.o
-00000470: 6e4c 6f61 6428 2468 746d 6c29 3b0d 0a20  nLoad($html);.. 
-00000480: 2020 207d 0d0a 0d0a 2020 2020 7769 6c6c     }....    will
-00000490: 5368 6f77 2829 207b 0d0a 2020 2020 2020  Show() {..      
-000004a0: 2020 7265 7475 726e 2073 7570 6572 2e77    return super.w
-000004b0: 696c 6c53 686f 7728 293b 0d0a 2020 2020  illShow();..    
-000004c0: 7d0d 0a0d 0a20 2020 206f 6e52 6566 7265  }....    onRefre
-000004d0: 7368 2829 207b 0d0a 2020 2020 2020 2020  sh() {..        
+00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000430: 2d2d 2d2d 2f2f 0a0a 2020 2020 6f6e 496e  ----//..    onIn
+00000440: 6974 2829 207b 0a20 2020 207d 0a0a 2020  it() {.    }..  
+00000450: 2020 6f6e 4c6f 6164 2824 6874 6d6c 2920    onLoad($html) 
+00000460: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
+00000470: 2073 7570 6572 2e6f 6e4c 6f61 6428 2468   super.onLoad($h
+00000480: 746d 6c29 3b0a 2020 2020 7d0a 0a20 2020  tml);.    }..   
+00000490: 2077 696c 6c53 686f 7728 2920 7b0a 2020   willShow() {.  
+000004a0: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
+000004b0: 6572 2e77 696c 6c53 686f 7728 293b 0a20  er.willShow();. 
+000004c0: 2020 207d 0a0a 2020 2020 6f6e 5265 6672     }..    onRefr
+000004d0: 6573 6828 2920 7b0a 2020 2020 2020 2020  esh() {.        
 000004e0: 7265 7475 726e 2073 7570 6572 2e6f 6e52  return super.onR
-000004f0: 6566 7265 7368 2829 3b0d 0a20 2020 207d  efresh();..    }
-00000500: 0d0a 0d0a 7d0d 0a0d 0a61 7070 2e72 6567  ....}....app.reg
-00000510: 6973 7465 7228 c2a7 434f 4e54 524f 4c4c  ister(..CONTROLL
-00000520: 4552 4e41 4d45 5449 544c 45c2 a743 6f6e  ERNAMETITLE..Con
-00000530: 7472 6f6c 6c65 7229 3b                   troller);
+000004f0: 6566 7265 7368 2829 3b0a 2020 2020 7d0a  efresh();.    }.
+00000500: 0a20 2020 206f 6e53 7562 6d69 7428 2920  .    onSubmit() 
+00000510: 7b0a 2020 2020 2020 2020 736f 636b 6574  {.        socket
+00000520: 5265 636f 6e6e 6563 7428 293b 0a20 2020  Reconnect();.   
+00000530: 2020 2020 2074 7269 6767 6572 2827 6c6f       trigger('lo
+00000540: 676f 7574 2729 3b0a 2020 2020 7d0a 0a7d  gout');.    }..}
+00000550: 0a0a 6170 702e 7265 6769 7374 6572 2853  ..app.register(S
+00000560: 6463 4c6f 676f 7574 436f 6e74 726f 6c6c  dcLogoutControll
+00000570: 6572 292e 6164 644d 6978 696e 2827 7364  er).addMixin('sd
+00000580: 632d 6175 746f 2d73 7562 6d69 7427 293b  c-auto-submit');
```

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/controller/template_test.js.text` & `simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_test.js.text`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/models/detail.html` & `simpledomcontrol-0.5.0/sdc_core/template_files/models/detail.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/models/list.html` & `simpledomcontrol-0.5.0/sdc_core/template_files/models/list.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_core/template_files/package.json` & `simpledomcontrol-0.5.0/sdc_core/template_files/package.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.815162037037037%*

 * *Differences: {"'dependencies'": "{'jquery': '^3.7.0', 'sdc_client': '^0.05.00', '@popperjs/core': '^2.11.8', "*

 * *                   "'esm': '^3.2.25'}",*

 * * "'devDependencies'": "{'@babel/core': '^7.23.7', '@babel/register': '^7.23.7', 'css-loader': "*

 * *                      "'^6.9.0', 'sass': '^1.69.7', 'sass-loader': '^13.3.3', 'style-loader': "*

 * *                      "'^3.3.4', 'terser-webpack-plugin': '^5.3.10', 'dotenv': '^16.3.1', "*

 * *                      "'glob-parent': '^6.0.2', 'glob-watcher': '^6.0.0', 'js-cookie': '^3 […]*

```diff
@@ -1,59 +1,78 @@
 {
     "author": "",
     "dependencies": {
+        "@popperjs/core": "^2.11.8",
         "bootstrap": "^5.3.2",
-        "jquery": "^3.7.1",
+        "esm": "^3.2.25",
+        "jquery": "^3.7.0",
         "lodash": "^4.17.21",
-        "sdc_client": "^0.3.8"
+        "sdc_client": "^0.05.00"
     },
     "description": "",
     "devDependencies": {
-        "@babel/core": "^7.23.3",
+        "@babel/core": "^7.23.7",
         "@babel/preset-react": "^7.23.3",
-        "@babel/register": "^7.22.15",
+        "@babel/register": "^7.23.7",
         "babel-jest": "^29.7.0",
         "babel-loader": "^9.1.3",
-        "chokidar": "^3.5.3",
-        "css-loader": "^6.8.1",
+        "css-loader": "^6.9.0",
+        "dotenv": "^16.3.1",
+        "glob-parent": "^6.0.2",
+        "glob-watcher": "^6.0.0",
         "gulp": "^4.0.2",
         "gulp-clean": "^0.4.0",
         "gulp-exec": "^5.0.0",
         "gulp-rename": "^2.0.0",
         "gulp-sass": "^5.1.0",
         "gulp-uglify": "^3.0.2",
         "jest": "^29.7.0",
         "jest-environment-jsdom": "^29.7.0",
-        "sass": "^1.69.5",
-        "sass-loader": "^13.3.2",
-        "style-loader": "^3.3.3",
-        "terser-webpack-plugin": "^5.3.9",
-        "through2": "^4.0.2",
+        "js-cookie": "^3.0.5",
+        "micromatch": "^4.0.5",
+        "sass": "^1.69.7",
+        "sass-loader": "^13.3.3",
+        "style-loader": "^3.3.4",
+        "terser-webpack-plugin": "^5.3.10",
         "webpack": "^5.89.0",
         "webpack-stream": "^7.0.0"
     },
+    "imports": {
+        "#root/*.js": "./Assets/*.js"
+    },
     "jest": {
-        "setupFiles": [
-            "<rootDir>/Assets/tests/pre-test-setup.js"
-        ],
+        "globalSetup": "<rootDir>/Assets/tests/config/pre-test-setup.js",
+        "globalTeardown": "<rootDir>/Assets/tests/config/post-test-teardown.js",
         "setupFilesAfterEnv": [
-            "<rootDir>/Assets/tests/test-setup.js"
+            "<rootDir>/Assets/tests/config/test-setup.js"
         ],
         "testEnvironment": "jest-environment-jsdom",
         "testEnvironmentOptions": {
-            "url": "http://127.0.0.1:8000"
+            "url": "http://127.0.0.1:8765"
         },
         "testMatch": [
-            "**/Assets/tests/*.test.js?(x)"
-        ]
+            "<rootDir>/*/Assets/tests/*.test.js?(x)"
+        ],
+        "transform": {
+            "\\.[jt]sx?$": [
+                "babel-jest",
+                {
+                    "configFile": "./Assets/.babelrc"
+                }
+            ]
+        }
     },
     "keywords": [],
     "license": "",
     "module": "esnext",
     "name": "<!--\u00a7PROJECT\u00a7-->",
+    "overrides": {
+        "glob-parent": "$glob-parent",
+        "glob-watcher": "$glob-watcher"
+    },
     "private": true,
     "scripts": {
         "build": "gulp --gulpfile=Assets/gulpfile.jsx --mode=production",
         "develop": "gulp --gulpfile=Assets/gulpfile.jsx develop --mode=development",
         "sdc_test": "NODE_OPTIONS=--experimental-vm-modules jest"
     },
     "type": "module",
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -28,14 +28,16 @@
     //-------------------------------------------------//
     // - onRemove                                      //
     //-------------------------------------------------//
 
     onInit() {}
 
     onLoad($html) {
+        on('pushMsg', this);
+        on('pushErrorMsg', this);
         return super.onLoad($html);
     }
 
     willShow() {
         return super.willShow();
     }
 
@@ -52,21 +54,23 @@
     }
 
     _pushMsg(header, msgList, isError) {
         if (typeof msgList === 'string') {
             msgList = [msgList];
         }
 
-        for (let msg of msgList) {
-            this._pushMsgArray(header, msgList, isError);
-        }
+        this._pushMsgArray(header, msgList, isError);
     }
 
     _pushMsgArray(header, msg, isError) {
         let $dummyRow = this.find('.dummy_row');
+        if ($dummyRow.length === 0) {
+            return
+        }
+
         let $cloneRow = $dummyRow.clone();
         $cloneRow.removeClass('dummy_row');
         if (isError) {
             $cloneRow.addClass('error_box');
         }
 
         $cloneRow.find('.msg_header').text(header);
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 import {
     AbstractSDC,
     app
 } from 'sdc_client';
 
 
-export class SdcErrorController extends AbstractSDC {
+class SdcDummyController extends AbstractSDC {
 
     constructor() {
         super();
-        this.contentUrl = "/sdc_view/sdc_tools/sdc_error/%(code)s"; //<sdc-error data-code=""></sdc-error>
+        this.contentUrl = "/sdc_view/sdc_tools/sdc_dummy"; //<sdc-dummy></sdc-dummy>
 
         /**
          * Events is an array of dom events.
          * The pattern is {'event': {'dom_selector': handler}}
          * Uncommend the following line to add events;
          */
         // this.events.unshift({'click': {'.header-sample': (ev, $elem)=> $elem.css('border', '2px solid black')}}});
@@ -24,24 +24,33 @@
     // - onLoad (DOM not set)                          //
     // - willShow  (DOM set)                           //
     // - onRefresh  (recalled on reload)              //
     //-------------------------------------------------//
     // - onRemove                                      //
     //-------------------------------------------------//
 
-    onInit() {}
+    onInit(text) {
+        this._text = text;
+    }
 
     onLoad($html) {
+        $html.find('.origen_content').append(this.$container.html());
         return super.onLoad($html);
     }
 
     willShow() {
         return super.willShow();
     }
 
     onRefresh() {
         return super.onRefresh();
     }
 
+    page_text() {
+        return < p className = "col" > {
+            this._text || ''
+        } < /p>;
+    }
+
 }
 
-app.register(SdcErrorController);
+app.register(SdcDummyController);
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -52,15 +52,19 @@
             this.model.load().then(() => {
                 this.on_update(this.model.values_list);
             });
         }
     }
 
     onLoad($html) {
-        $html.filter('.list-container').append(this.model.listView(this.search_values));
+        let lc = $html.filter('.list-container');
+        if (lc.length === 0) {
+            lc = $html.find('.list-container');
+        }
+        lc.append(this.model.listView(this.search_values));
         this.model.on_update = this.model.on_create = () => {
             if (this.on_update) {
                 this.model.load().then(() => {
                     this.on_update(this.model.values_list);
                 });
             }
             this._updateView();
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -81,15 +81,15 @@
 
     onRefresh() {
         return super.onRefresh();
     }
 
     submitModelForm($form, e) {
         let self = this;
-        return super._submitModelForm($form, e).then(function(res) {
+        return super.defaultSubmitModelForm($form, e).then(function(res) {
             if (res && res.type === 'create') {
                 $form[0].reset();
             }
 
             self.on_update && self.on_update(res);
         }).catch((res) => {
             self.on_error && self.on_error(res);
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -2,43 +2,24 @@
     AbstractSDC,
     app,
     on,
     trigger,
     checkIfParamNumberBoolOrString
 } from 'sdc_client';
 
-import {
-    isMatch
-} from 'lodash';
-
 const SDC_SUB_DETAIL_CONTROLLER = 'sdc_sub_detail_container';
 const SDC_DETAIL_CONTROLLER = 'sdc_detail_view';
 
 
 export class SdcNavigatorController extends AbstractSDC {
 
     constructor() {
         super();
         this.contentUrl = "/sdc_view/sdc_tools/sdc_navigator"; //<sdc-navigator></sdc-navigator>
-
-        this._history_path = [];
-        this._history_path = [];
-        this._breadcrumb = [];
-        this._history_idx = 0;
-        this._origin_target = [];
-        this._$detail_view_container = [];
-        this._default_controller = null;
-        this._previous_args = [];
-
-        this._is_processing = false;
-        this._process_queue = [];
-
-        this._non_controller_path_prefix = '/';
-        this._menu_id = 0;
-
+        this._setup();
         /**
          * Events is an array of dom events.
          * The pattern is {'event': {'dom_selector': handler}}
          * Uncommend the following line to add events;
          */
         this.events.unshift({
             'click': {
@@ -47,14 +28,34 @@
                     // noinspection JSPotentiallyInvalidUsageOfClassThis
                     this.onNavLink(btn, ev);
                 }
             }
         });
     }
 
+    _setup() {
+
+        this._isLoggedIn = false;
+        this._history_path = [];
+        this._breadcrumb = [];
+        this._history_idx = 0;
+        this._origin_target = [];
+        this._$detail_view_container = [];
+        this._default_controller = null;
+        this._previous_args = [];
+
+        this._is_processing = false;
+        this._process_queue = [];
+        this._current_process = null;
+        this._redirectAfterCurrentProcess = null;
+
+        this._non_controller_path_prefix = '/';
+        this._menu_id = 0;
+    }
+
     //-------------------------------------------------//
     // Lifecycle handler                               //
     // - onInit (tag parameter)                        //
     // - onLoad (DOM not set)                          //
     // - willShow  (DOM set)                           //
     // - onRefresh  (recalled on reload)              //
     //-------------------------------------------------//
@@ -64,23 +65,24 @@
     onInit(defaultController) {
         this._default_controller = defaultController;
     }
 
     onLoad($html) {
         on('onNavLink', this);
         on('onNavigateToController', this);
+        on('_RedirectOnView', this);
         on('goTo', this);
-        on('onNavigateToController', this);
         on('changeMenu', this);
         on('navigateToPage', this);
         on('navLoaded', this);
         on('login', this);
         on('logout', this);
 
         $html.find('.main-nav-import-container').append(this.$container.html());
+        this._isLoggedIn = $html.data('user');
         return super.onLoad($html);
     }
 
     willShow() {
         let self = this;
         $(window).resize(function() {
             trigger('_onResize', self);
@@ -107,23 +109,33 @@
 
     /** Event Handler **/
     onNavLink($btn, ev) {
         if (ev) {
             ev.preventDefault();
         }
 
-        let c_list = $($btn).attr('href').split('~').map((x) => x.split('/')).flat().filter((x, i) => i < 1 || x.length > 0);
-        if (c_list.length === 1 && !c_list[0].startsWith('.')) c_list.unshift('');
-
-        const link = c_list.join('~').split('~~').join('~');
 
-        this.onNavigateToController(link);
+        this.goTo($($btn).attr('href'));
     }
 
     goTo(controller_path_as_array, args = null) {
+        if (Array.isArray(controller_path_as_array)) {
+            controller_path_as_array = controller_path_as_array.join('~');
+        }
+
+        let c_list = controller_path_as_array.split('~').map((x) => x.split('/')).flat().filter((x, i) => i < 1 || x.length > 0);
+        if (!c_list[0].startsWith('.') && c_list[0] !== '*' && c_list[0] !== '') {
+            for (let i = 0; i < this._history_path.length; ++i) {
+                c_list.unshift('*');
+            }
+            c_list.unshift('');
+        }
+
+        controller_path_as_array = c_list.join('~').split('~~').join('~');
+
         return this.onNavigateToController(controller_path_as_array, args);
     }
 
     onNavigateToController(controller_path_as_array, args = null) {
         if (Array.isArray(controller_path_as_array)) {
             controller_path_as_array = controller_path_as_array.join('~')
         }
@@ -135,24 +147,21 @@
                 for (const [key, value] of Object.entries(args)) {
                     args_list.push(`${key}=${value}`);
                 }
                 args = args_list.join('&')
             }
             controller_path_as_array += '~&' + args
         }
-        let data = this._handleUrl(controller_path_as_array);
-        history.pushState(data, "", data.url);
+
+        this._pushState(controller_path_as_array);
     }
 
     navigateToPage(target, args, _state) {
-        if (this._is_processing) {
-            this._process_queue[0] = [target, args];
-            return;
-        }
-        this.state && this._updateButton(this.state.buttonSelector);
+        this._current_process = [target, args];
+        _state && this._updateButton(_state.buttonSelector);
         this._is_processing = true;
         this._origin_target = target;
 
         let viewObj = this._getSubViewObj(args);
         this._previous_args = args;
 
         if (viewObj.container.container.data('modal')) {
@@ -184,16 +193,15 @@
             let controller = app.getController(viewObj.container.active_container.find('> ._sdc_controller_'));
             this._manageDefault(viewObj.container.active_container);
             if (typeof controller.onBack === 'function') {
                 controller.onBack();
             }
             this._is_processing = false;
             this._updateBreadcrumb();
-            let next = this._process_queue.shift();
-            if (next) this.navigateToPage(next[0], next[1]);
+            this._checkProcessQueue();
             this.refresh();
             return;
         }
 
         viewObj.container.empty_container.addClass('loading');
         viewObj.container.active_sub_container.addClass('loading');
         viewObj.container.active_container.addClass('loading');
@@ -208,14 +216,15 @@
                 (group) => '-' + group.toLowerCase()
             )
 
             if (controller_key.length === 1 || (controller_key.length > 1 && parseInt(controller_key[0]) === viewObj.idx + 1)) {
                 $newElement.data(data_key, value);
             }
         }
+
         viewObj.container.empty_container.safeEmpty().append($newElement);
 
         this.refresh();
         this.find('.header-loading').addClass('active');
         if (!$newElement.hasClass("_sdc_controller_")) {
             viewObj.container.empty_container.empty().append(`<sdc-error_sdc-sdc-navigation-client data-code="${404}"></sdc-error_sdc-sdc-navigation-client>`);
             this.refresh();
@@ -232,30 +241,43 @@
         last_view_array.empty_container.addClass('active').removeClass('empty loading');
         last_view_array.deeper_sub_container.safeEmpty().removeClass('empty loading');
         this._breadcrumb.splice(idx);
         this._is_processing = false;
         $('.tooltip.fade.show').remove();
         this._breadcrumb[idx] = controller.controller_name();
         if (this._origin_target.length !== this._history_path.length) {
-            let data = this._handleUrl(window.location.pathname);
-            if (data.path.length > 1) {
-                history.pushState(data, "", data.url);
-            }
+            if (this._current_process) this.navigateToPage(this._current_process[0], this._current_process[1]);
         } else {
             this._updateBreadcrumb();
             if (!this._manageDefault(last_view_array.empty_container)) {
-                let next = this._process_queue.shift()
-                if (next) this.navigateToPage(next[0], next[1])
+                this._checkProcessQueue();
             }
             setTimeout(() => {
                 this.$container.find('.header-loading').removeClass('active');
             }, 100);
         }
     }
 
+    _checkProcessQueue() {
+        let next = this._process_queue.shift();
+        this._current_process = null;
+        if (next) {
+            this._pushState(next[0], next[1]);
+        } else if (this._redirectAfterCurrentProcess) {
+            const temp = this._redirectAfterCurrentProcess;
+            this._redirectAfterCurrentProcess = null;
+            this.goTo(temp);
+        }
+
+    }
+
+    _RedirectOnView($btn) {
+        this._redirectAfterCurrentProcess = $($btn).attr('href');
+    }
+
     _updateBreadcrumb() {
         this._breadcrumb.splice(this._history_path.length);
         const $breadcrumps = this.find('.breadcrumb');
         const self = this;
         $breadcrumps.each(function() {
             const $breadcrumb = $(this);
             $breadcrumb.safeEmpty();
@@ -337,15 +359,15 @@
         while (idx < Math.min(target.length, this._history_path.length) &&
             target[idx] === this._history_path[idx]) {
             idx++;
         }
 
         if (idx >= target.length && target[idx - 1] === this._history_path[idx - 1]) {
             idx = target.length - 1;
-            isBack = target.length < this._history_path.length && isMatch(this._previous_args, args);
+            isBack = target.length < this._history_path.length && _.isMatch(this._previous_args, args);
             this._history_path = [...target];
         } else if (idx >= target.length) {
             idx = target.length - 1;
             this._history_path = [...target];
         } else {
             this._history_path = [...target].slice(0, idx + 1);
         }
@@ -392,14 +414,22 @@
 
 
         if ($button) {
             this.find('.navigation-links').removeClass('active');
             $button.addClass('active');
         }
 
+        if (this._isLoggedIn) {
+            this.find('.navigation-links.only-logged-in').show();
+            this.find('.navigation-links.only-logged-out').hide();
+        } else {
+            this.find('.navigation-links.only-logged-in').hide();
+            this.find('.navigation-links.only-logged-out').show();
+        }
+
         return $button;
     }
 
     _handleUrl(location_path_str) {
         let args_idx = location_path_str.match(/[&?]/);
         let args, path_array;
         if (args_idx) {
@@ -498,29 +528,45 @@
         return route_args;
     }
 
     _manageDefault(container) {
         const $sub_container = container.find(`.${SDC_DETAIL_CONTROLLER}`);
         const df = $sub_container.data('default-controller');
         if (df) {
-            let data = this._handleUrl(`.~${df}`);
-            history.pushState(data, "", data.url);
+            this._pushState(`.~${df}`, false);
             return true;
         }
 
         return false;
     }
 
+    _pushState(url, commit = true) {
+        if (this._is_processing) {
+            this._process_queue.push([url, commit]);
+            return;
+        }
+
+        let state = this._handleUrl(url);
+        if (commit) {
+            history.pushState(state, "", state.url);
+        } else {
+            this.navigateToPage(state.path, state.args, state);
+        }
+    }
+
     login() {
-        app.cleanCache();
-        this.onNavigateToController(window.location.pathname);
+        window.addEventListener("beforeunload", function(e) {
+            // Do something
+            e.preventDefault();
+        }, false);
+        location.reload();
     }
 
-    logout(pk) {
-        this.login(pk);
+    logout() {
+        this.login();
     }
 
 }
 
 app.register(SdcNavigatorController);
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+import {} from "./controller/sdc_dummy/sdc_dummy.js";
 import {} from "./controller/sdc_auto_submit/sdc_auto_submit.js";
 import {} from "./controller/sdc_error/sdc_error.js";
 import {} from "./controller/sdc_navigation_client/sdc_navigation_client.js";
 import {} from "./controller/sdc_alert_messenger/sdc_alert_messenger.js";
 import {} from "./controller/sdc_update_on_change/sdc_update_on_change.js";
 import {} from "./controller/sdc_search_view/sdc_search_view.js";
 import {} from "./controller/sdc_detail_view/sdc_detail_view.js";
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/sdc_urls.py` & `simpledomcontrol-0.5.0/sdc_tools/sdc_urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from . import sdc_views
 
 # Do not add an app_name to this file
 
 urlpatterns = [
     # scd view below
+    path('sdc_dummy', sdc_views.SdcDummy.as_view(), name='scd_view_sdc_dummy'),
     path('sdc_error/<int:code>', sdc_views.SdcError.as_view(), name='scd_view_sdc_error'),
     path('sdc_alert_messenger', sdc_views.SdcAlertMessenger.as_view(), name='scd_view_sdc_alert_messenger'),
     path('sdc_search_view', sdc_views.SdcSearchView.as_view(), name='scd_view_sdc_search_view'),
     path('sdc_detail_view', sdc_views.SdcDetailView.as_view(), name='scd_view_sdc_detail_view'),
     path('sdc_model_form', sdc_views.SdcModelForm.as_view(), name='scd_view_sdc_model_form'),
     path('sdc_list_view', sdc_views.SdcListView.as_view(), name='scd_view_sdc_list_view'),
     path('sdc_navigator', sdc_views.SdcNavigator.as_view(), name='scd_view_sdc_navigator'),
```

### Comparing `simpledomcontrol-0.4.8/sdc_tools/sdc_views.py` & `simpledomcontrol-0.5.0/sdc_tools/sdc_views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-from django.shortcuts import render
-from sdc_core.sdc_extentions.views import SDCView
-
-
-
-
-class SdcNavigator(SDCView):
-    template_name = 'sdc_tools/sdc/sdc_navigator.html'
-
-    def get_content(self, request, *args, **kwargs):
-        return render(request, self.template_name)
-
-
-class SdcListView(SDCView):
-    template_name='sdc_tools/sdc/sdc_list_view.html'
-
-    def get_content(self, request, *args, **kwargs):
-        return render(request, self.template_name)
-
-class SdcModelForm(SDCView):
-    template_name='sdc_tools/sdc/sdc_model_form.html'
-
-    def get_content(self, request, *args, **kwargs):
-        return render(request, self.template_name)
-
-class SdcDetailView(SDCView):
-    template_name='sdc_tools/sdc/sdc_detail_view.html'
-
-    def get_content(self, request, *args, **kwargs):
-        return render(request, self.template_name)
-
-class SdcSearchView(SDCView):
-    template_name='sdc_tools/sdc/sdc_search_view.html'
-
-    def get_content(self, request, *args, **kwargs):
-        return render(request, self.template_name)
-
-class SdcAlertMessenger(SDCView):
-    template_name='sdc_tools/sdc/sdc_alert_messenger.html'
-
-    def get_content(self, request, *args, **kwargs):
-        return render(request, self.template_name)
-
-class SdcError(SDCView):
-    template_name='sdc_tools/sdc/sdc_error.html'
-
-    def get_content(self, request, code, *args, **kwargs):
-        return render(request, self.template_name, {'code': code})
+from django.shortcuts import render
+from sdc_core.sdc_extentions.views import SDCView
+
+
+
+
+class SdcNavigator(SDCView):
+    template_name = 'sdc_tools/sdc/sdc_navigator.html'
+
+    def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
+
+
+class SdcListView(SDCView):
+    template_name='sdc_tools/sdc/sdc_list_view.html'
+
+    def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
+
+class SdcModelForm(SDCView):
+    template_name='sdc_tools/sdc/sdc_model_form.html'
+
+    def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
+
+class SdcDetailView(SDCView):
+    template_name='sdc_tools/sdc/sdc_detail_view.html'
+
+    def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
+
+class SdcSearchView(SDCView):
+    template_name='sdc_tools/sdc/sdc_search_view.html'
+
+    def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
+
+class SdcAlertMessenger(SDCView):
+    template_name='sdc_tools/sdc/sdc_alert_messenger.html'
+
+    def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
+
+class SdcError(SDCView):
+    template_name='sdc_tools/sdc/sdc_error.html'
+
+    def get_content(self, request, code, *args, **kwargs):
+        return render(request, self.template_name, {'code': code})
+
+class SdcDummy(SDCView):
+    template_name='sdc_tools/sdc/sdc_dummy.html'
+
+    def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
```

### Comparing `simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js` & `simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.4.8/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js` & `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,18 @@
 import {
     AbstractSDC,
-    app,
-    trigger,
-    socketReconnect
+    app
 } from 'sdc_client';
 
-class SdcLogoutController extends AbstractSDC {
+
+export class SdcErrorController extends AbstractSDC {
 
     constructor() {
         super();
-        this.contentUrl = "/sdc_view/sdc_user/sdc_logout"; //<sdc-logout></sdc-logout>
+        this.contentUrl = "/sdc_view/sdc_tools/sdc_error/%(code)s"; //<sdc-error data-code=""></sdc-error>
 
         /**
          * Events is an array of dom events.
          * The pattern is {'event': {'dom_selector': handler}}
          * Uncommend the following line to add events;
          */
         // this.events.unshift({'click': {'.header-sample': (ev, $elem)=> $elem.css('border', '2px solid black')}}});
@@ -28,26 +27,22 @@
     //-------------------------------------------------//
     // - onRemove                                      //
     //-------------------------------------------------//
 
     onInit() {}
 
     onLoad($html) {
+        $html.find('.error_content').append(this.$container.html());
         return super.onLoad($html);
     }
 
     willShow() {
         return super.willShow();
     }
 
     onRefresh() {
         return super.onRefresh();
     }
 
-    onSubmit() {
-        socketReconnect();
-        trigger('logout');
-    }
-
 }
 
-app.register(SdcLogoutController).addMixin('sdc-auto-submit');
+app.register(SdcErrorController);
```

### Comparing `simpledomcontrol-0.4.8/sdc_user/sdc_views.py` & `simpledomcontrol-0.5.0/sdc_user/sdc_views.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,8 +45,14 @@
     template_name='sdc_user/sdc/sdc_logout.html'
 
     def post_api(self, request):
         logout(request)
         return send_redirect(url=f'/~{settings.LOGIN_CONTROLLER}')
 
     def get_content(self, request, *args, **kwargs):
+        return render(request, self.template_name)
+
+class SdcUserNavBtn(SDCView):
+    template_name='sdc_user/sdc/sdc_user_nav_btn.html'
+
+    def get_content(self, request, *args, **kwargs):
         return render(request, self.template_name)
```

### Comparing `simpledomcontrol-0.4.8/PKG-INFO` & `simpledomcontrol-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
-Name: simpledomcontrol
-Version: 0.4.8
+Name: SimpleDomControl
+Version: 0.5.0
 Summary: Simple DOM control -> a django MVC framework
 Home-page: https://github.com/StarmanMartin/sdc
 License: Apache-2.0
 Keywords: django,MVC
 Author: Martin Starman
 Author-email: private@martin-starman.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: channels (>=4.0.0,<5.0.0)
-Requires-Dist: channels-redis (>=4.1.0,<5.0.0)
-Requires-Dist: daphne (>=4.0.0,<5.0.0)
-Requires-Dist: django (>=4.2.7,<5.0.0)
+Requires-Dist: attrs (>=23.2.0,<24.0.0)
+Requires-Dist: channels (>=4.1.0,<5.0.0)
+Requires-Dist: channels-redis (>=4.2.0,<5.0.0)
+Requires-Dist: daphne (>=4.1.2,<5.0.0)
+Requires-Dist: django (>=5.0.6,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
+Requires-Dist: regex (>=2024.5.15,<2025.0.0)
 Description-Content-Type: text/markdown
 
 simpleDomControl
```

