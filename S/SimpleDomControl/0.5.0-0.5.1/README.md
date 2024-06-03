# Comparing `tmp/simpledomcontrol-0.5.0.tar.gz` & `tmp/simpledomcontrol-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpledomcontrol-0.5.0.tar", max compression
+gzip compressed data, was "simpledomcontrol-0.5.1.tar", max compression
```

## Comparing `simpledomcontrol-0.5.0.tar` & `simpledomcontrol-0.5.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0       17 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.0/README.md
--rw-r--r--   0        0        0     1125 2024-05-26 04:43:06.816129 simpledomcontrol-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/__init__.py
--rw-r--r--   0        0        0     1263 2024-02-02 09:59:54.494456 simpledomcontrol-0.5.0/sdc_core/apps.py
--rw-r--r--   0        0        0    19588 2024-05-26 11:28:08.009889 simpledomcontrol-0.5.0/sdc_core/consumers.py
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/_private.py
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/__init__.py
--rw-r--r--   0        0        0    11002 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_controller_manager.py
--rw-r--r--   0        0        0     4590 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_model_manager.py
--rw-r--r--   0        0        0     1177 2024-02-06 09:19:01.417955 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/options.py
--rw-r--r--   0        0        0     1839 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/sdc_core_manager.py
--rw-r--r--   0        0        0     5116 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/settings_manager.py
--rw-r--r--   0        0        0     2077 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/utils.py
--rw-r--r--   0        0        0     3175 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_cc.py
--rw-r--r--   0        0        0     3594 2024-01-17 13:18:27.055931 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_controller_infos.py
--rw-r--r--   0        0        0      507 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_controller_url.py
--rw-r--r--   0        0        0     2665 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_model_infos.py
--rw-r--r--   0        0        0     2650 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_init.py
--rw-r--r--   0        0        0      703 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_is_installed.py
--rw-r--r--   0        0        0     2579 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_new_model.py
--rw-r--r--   0        0        0     1301 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_shell_execute_script.py
--rw-r--r--   0        0        0     3677 2024-01-17 11:51:17.421303 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_links.py
--rw-r--r--   0        0        0     1884 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_url.py
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/__init__.py
--rw-r--r--   0        0        0     1149 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/forms.py
--rw-r--r--   0        0        0      382 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/import_manager.py
--rw-r--r--   0        0        0     2234 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/models.py
--rw-r--r--   0        0        0     4116 2024-03-05 13:01:15.459889 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/response.py
--rw-r--r--   0        0        0     1790 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/search.py
--rw-r--r--   0        0        0     3975 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/sdc_extentions/views.py
--rw-r--r--   0        0        0      106 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/.babelrc
--rw-r--r--   0        0        0     1233 2024-02-05 09:28:14.910183 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/gulpfile.jsx
--rw-r--r--   0        0        0      472 2024-01-19 06:04:45.704481 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/src/index.organizer.js
--rw-r--r--   0        0        0      324 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/src/index.style.scss
--rw-r--r--   0        0        0      196 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/tests/config/post-test-teardown.js
--rw-r--r--   0        0        0     3212 2024-02-02 10:22:46.579597 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/tests/config/pre-test-setup.js
--rw-r--r--   0        0        0      306 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/tests/config/test-setup.js
--rw-r--r--   0        0        0     1278 2024-02-05 08:23:47.706252 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx
--rw-r--r--   0        0        0      320 2024-02-05 08:34:24.715149 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.development.config.jsx
--rw-r--r--   0        0        0      543 2024-02-05 08:34:24.711149 simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx
--rw-r--r--   0        0        0     1191 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt
--rw-r--r--   0        0        0     2414 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/index.html
--rw-r--r--   0        0        0     2253 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/server_call.txt
--rw-r--r--   0        0        0      865 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/asgi.py.txt
--rw-r--r--   0        0        0       80 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/templade_view.html
--rw-r--r--   0        0        0     1293 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_controller.js.txt
--rw-r--r--   0        0        0       15 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_css.scss
--rw-r--r--   0        0        0      535 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_test.js.text
--rw-r--r--   0        0        0      241 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/js_test.js.txt
--rw-r--r--   0        0        0     1633 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/models/detail.html
--rw-r--r--   0        0        0     2303 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/models/list.html
--rw-r--r--   0        0        0     2109 2024-05-26 04:43:06.784130 simpledomcontrol-0.5.0/sdc_core/template_files/package.json
--rw-r--r--   0        0        0      349 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/routing.py.txt
--rw-r--r--   0        0        0      141 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/sdc_urls.py.txt
--rw-r--r--   0        0        0       87 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/sdc_views.py.txt
--rw-r--r--   0        0        0      898 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/settings_extension.py.txt
--rw-r--r--   0        0        0      957 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/templates/base.html
--rw-r--r--   0        0        0      405 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/templates/index.html
--rw-r--r--   0        0        0      281 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_core/template_files/urls.py.txt
--rw-r--r--   0        0        0     2928 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js
--rw-r--r--   0        0        0     1178 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss
--rw-r--r--   0        0        0     2454 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js
--rw-r--r--   0        0        0     1833 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js
--rw-r--r--   0        0        0       23 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.scss
--rw-r--r--   0        0        0     1473 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.js
--rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.scss
--rw-r--r--   0        0        0     1387 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js
--rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.scss
--rw-r--r--   0        0        0     3165 2024-03-26 11:21:21.381111 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js
--rw-r--r--   0        0        0      103 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.scss
--rw-r--r--   0        0        0     3273 2024-03-13 08:30:43.081304 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js
--rw-r--r--   0        0        0      180 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.scss
--rw-r--r--   0        0        0     1457 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js
--rw-r--r--   0        0        0    21405 2024-05-13 11:54:22.067553 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js
--rw-r--r--   0        0        0     1019 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss
--rw-r--r--   0        0        0     4914 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js
--rw-r--r--   0        0        0     2238 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss
--rw-r--r--   0        0        0     2819 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js
--rw-r--r--   0        0        0      722 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js
--rw-r--r--   0        0        0      413 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/sdc_tools.style.scss
--rw-r--r--   0        0        0     6930 2024-03-13 07:55:56.619058 simpledomcontrol-0.5.0/sdc_tools/Assets/tests/sdc_tools.test.js
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/__init__.py
--rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/admin.py
--rw-r--r--   0        0        0       92 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/apps.py
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/models.py
--rw-r--r--   0        0        0      884 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/sdc_urls.py
--rw-r--r--   0        0        0     1618 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/sdc_views.py
--rw-r--r--   0        0        0     1192 2024-04-16 07:32:46.011283 simpledomcontrol-0.5.0/sdc_tools/templates/elements/form.html
--rw-r--r--   0        0        0     1030 2024-04-16 07:43:06.313233 simpledomcontrol-0.5.0/sdc_tools/templates/elements/inline_form.html
--rw-r--r--   0        0        0     1075 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/email/base.html
--rw-r--r--   0        0        0       65 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/dummy_sdc.html
--rw-r--r--   0        0        0      399 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_alert_messenger.html
--rw-r--r--   0        0        0       36 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_detail_view.html
--rw-r--r--   0        0        0      179 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_dummy.html
--rw-r--r--   0        0        0      135 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_error.html
--rw-r--r--   0        0        0       37 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_list_view.html
--rw-r--r--   0        0        0      338 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_model_form.html
--rw-r--r--   0        0        0      207 2024-03-05 12:33:59.397833 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_navigator.html
--rw-r--r--   0        0        0      496 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templates/sdc_tools/sdc/sdc_search_view.html
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/__init__.py
--rw-r--r--   0        0        0      800 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/addclass.py
--rw-r--r--   0        0        0      341 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/indexfilter.py
--rw-r--r--   0        0        0     1092 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/templatetags/sdc_filter.py
--rw-r--r--   0        0        0       60 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/tests.py
--rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_tools/views.py
--rw-r--r--   0        0        0     1453 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js
--rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.scss
--rw-r--r--   0        0        0     1424 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js
--rw-r--r--   0        0        0       18 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.scss
--rw-r--r--   0        0        0     1467 2024-03-05 12:28:28.554496 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.js
--rw-r--r--   0        0        0       24 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.scss
--rw-r--r--   0        0        0      178 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/sdc_user.organizer.js
--rw-r--r--   0        0        0      112 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/sdc_user.style.scss
--rw-r--r--   0        0        0      999 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.0/sdc_user/Assets/tests/sdc_user.test.js
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/__init__.py
--rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/admin.py
--rw-r--r--   0        0        0      147 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/apps.py
--rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/models.py
--rw-r--r--   0        0        0      394 2024-03-05 20:52:54.936870 simpledomcontrol-0.5.0/sdc_user/sdc_urls.py
--rw-r--r--   0        0        0     2331 2024-03-05 11:56:18.694802 simpledomcontrol-0.5.0/sdc_user/sdc_views.py
--rw-r--r--   0        0        0      401 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/templates/sdc_user/sdc/sdc_login.html
--rw-r--r--   0        0        0      327 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/templates/sdc_user/sdc/sdc_logout.html
--rw-r--r--   0        0        0      144 2024-03-05 12:23:24.239188 simpledomcontrol-0.5.0/sdc_user/templates/sdc_user/sdc/sdc_user_nav_btn.html
--rw-r--r--   0        0        0       60 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/tests.py
--rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.0/sdc_user/views.py
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 simpledomcontrol-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.1/README.md
+-rw-r--r--   0        0        0     1125 2024-06-03 10:22:42.621050 simpledomcontrol-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/__init__.py
+-rw-r--r--   0        0        0     1263 2024-02-02 09:59:54.494456 simpledomcontrol-0.5.1/sdc_core/apps.py
+-rw-r--r--   0        0        0    18420 2024-06-03 07:16:27.675073 simpledomcontrol-0.5.1/sdc_core/consumers.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/_private.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/__init__.py
+-rw-r--r--   0        0        0    11002 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/add_controller_manager.py
+-rw-r--r--   0        0        0     4590 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/add_model_manager.py
+-rw-r--r--   0        0        0     1177 2024-02-06 09:19:01.417955 simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/options.py
+-rw-r--r--   0        0        0     1839 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/sdc_core_manager.py
+-rw-r--r--   0        0        0     5116 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/settings_manager.py
+-rw-r--r--   0        0        0     2077 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/utils.py
+-rw-r--r--   0        0        0     3175 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_cc.py
+-rw-r--r--   0        0        0     3594 2024-01-17 13:18:27.055931 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_get_controller_infos.py
+-rw-r--r--   0        0        0      507 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_get_controller_url.py
+-rw-r--r--   0        0        0     2665 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_get_model_infos.py
+-rw-r--r--   0        0        0     2650 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_init.py
+-rw-r--r--   0        0        0      703 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_is_installed.py
+-rw-r--r--   0        0        0     2579 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_new_model.py
+-rw-r--r--   0        0        0     1301 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_shell_execute_script.py
+-rw-r--r--   0        0        0     3677 2024-01-17 11:51:17.421303 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_update_links.py
+-rw-r--r--   0        0        0     1884 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_update_url.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/sdc_extentions/__init__.py
+-rw-r--r--   0        0        0     1149 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/sdc_extentions/forms.py
+-rw-r--r--   0        0        0      382 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/sdc_extentions/import_manager.py
+-rw-r--r--   0        0        0     3570 2024-06-03 10:19:01.141843 simpledomcontrol-0.5.1/sdc_core/sdc_extentions/models.py
+-rw-r--r--   0        0        0     4116 2024-03-05 13:01:15.459889 simpledomcontrol-0.5.1/sdc_core/sdc_extentions/response.py
+-rw-r--r--   0        0        0     1790 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/sdc_extentions/search.py
+-rw-r--r--   0        0        0     3975 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/sdc_extentions/views.py
+-rw-r--r--   0        0        0      106 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/.babelrc
+-rw-r--r--   0        0        0     1233 2024-02-05 09:28:14.910183 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/gulpfile.jsx
+-rw-r--r--   0        0        0      472 2024-01-19 06:04:45.704481 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/src/index.organizer.js
+-rw-r--r--   0        0        0      324 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/src/index.style.scss
+-rw-r--r--   0        0        0      196 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/tests/config/post-test-teardown.js
+-rw-r--r--   0        0        0     3212 2024-02-02 10:22:46.579597 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/tests/config/pre-test-setup.js
+-rw-r--r--   0        0        0      306 2024-01-15 08:35:05.086633 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/tests/config/test-setup.js
+-rw-r--r--   0        0        0     1278 2024-02-05 08:23:47.706252 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx
+-rw-r--r--   0        0        0      320 2024-02-05 08:34:24.715149 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/webpack.config/webpack.development.config.jsx
+-rw-r--r--   0        0        0      543 2024-02-05 08:34:24.711149 simpledomcontrol-0.5.1/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx
+-rw-r--r--   0        0        0     1191 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt
+-rw-r--r--   0        0        0     2414 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/apps/sdc_examples/index.html
+-rw-r--r--   0        0        0     2253 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/apps/sdc_examples/server_call.txt
+-rw-r--r--   0        0        0      865 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/asgi.py.txt
+-rw-r--r--   0        0        0       80 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/controller/templade_view.html
+-rw-r--r--   0        0        0     1293 2024-01-15 08:35:05.106633 simpledomcontrol-0.5.1/sdc_core/template_files/controller/template_controller.js.txt
+-rw-r--r--   0        0        0       15 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/controller/template_css.scss
+-rw-r--r--   0        0        0      535 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/controller/template_test.js.text
+-rw-r--r--   0        0        0      241 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/js_test.js.txt
+-rw-r--r--   0        0        0     1633 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/models/detail.html
+-rw-r--r--   0        0        0     2303 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/models/list.html
+-rw-r--r--   0        0        0     2109 2024-06-03 10:22:42.621050 simpledomcontrol-0.5.1/sdc_core/template_files/package.json
+-rw-r--r--   0        0        0      349 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/routing.py.txt
+-rw-r--r--   0        0        0      141 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/sdc_urls.py.txt
+-rw-r--r--   0        0        0       87 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/sdc_views.py.txt
+-rw-r--r--   0        0        0      898 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/settings_extension.py.txt
+-rw-r--r--   0        0        0      957 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/templates/base.html
+-rw-r--r--   0        0        0      405 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/templates/index.html
+-rw-r--r--   0        0        0      281 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_core/template_files/urls.py.txt
+-rw-r--r--   0        0        0     2928 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js
+-rw-r--r--   0        0        0     1178 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss
+-rw-r--r--   0        0        0     2454 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js
+-rw-r--r--   0        0        0     1833 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js
+-rw-r--r--   0        0        0       23 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.scss
+-rw-r--r--   0        0        0     1473 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.js
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.scss
+-rw-r--r--   0        0        0     1387 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.scss
+-rw-r--r--   0        0        0     3165 2024-03-26 11:21:21.381111 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js
+-rw-r--r--   0        0        0      103 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.scss
+-rw-r--r--   0        0        0     3273 2024-03-13 08:30:43.081304 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js
+-rw-r--r--   0        0        0      180 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.scss
+-rw-r--r--   0        0        0     1457 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js
+-rw-r--r--   0        0        0    21405 2024-05-13 11:54:22.067553 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js
+-rw-r--r--   0        0        0     1019 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss
+-rw-r--r--   0        0        0     4914 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js
+-rw-r--r--   0        0        0     2238 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss
+-rw-r--r--   0        0        0     2819 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js
+-rw-r--r--   0        0        0      722 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js
+-rw-r--r--   0        0        0      413 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/sdc_tools.style.scss
+-rw-r--r--   0        0        0     6930 2024-03-13 07:55:56.619058 simpledomcontrol-0.5.1/sdc_tools/Assets/tests/sdc_tools.test.js
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/__init__.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/admin.py
+-rw-r--r--   0        0        0       92 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/apps.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/models.py
+-rw-r--r--   0        0        0      884 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/sdc_urls.py
+-rw-r--r--   0        0        0     1618 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/sdc_views.py
+-rw-r--r--   0        0        0     1192 2024-04-16 07:32:46.011283 simpledomcontrol-0.5.1/sdc_tools/templates/elements/form.html
+-rw-r--r--   0        0        0     1030 2024-04-16 07:43:06.313233 simpledomcontrol-0.5.1/sdc_tools/templates/elements/inline_form.html
+-rw-r--r--   0        0        0     1075 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/email/base.html
+-rw-r--r--   0        0        0       65 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/dummy_sdc.html
+-rw-r--r--   0        0        0      399 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_alert_messenger.html
+-rw-r--r--   0        0        0       36 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_detail_view.html
+-rw-r--r--   0        0        0      179 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_dummy.html
+-rw-r--r--   0        0        0      135 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_error.html
+-rw-r--r--   0        0        0       37 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_list_view.html
+-rw-r--r--   0        0        0      338 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_model_form.html
+-rw-r--r--   0        0        0      207 2024-03-05 12:33:59.397833 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_navigator.html
+-rw-r--r--   0        0        0      496 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templates/sdc_tools/sdc/sdc_search_view.html
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templatetags/__init__.py
+-rw-r--r--   0        0        0      800 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templatetags/addclass.py
+-rw-r--r--   0        0        0      341 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templatetags/indexfilter.py
+-rw-r--r--   0        0        0     1092 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/templatetags/sdc_filter.py
+-rw-r--r--   0        0        0       60 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/tests.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_tools/views.py
+-rw-r--r--   0        0        0     1453 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js
+-rw-r--r--   0        0        0       17 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.scss
+-rw-r--r--   0        0        0     1424 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js
+-rw-r--r--   0        0        0       18 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.scss
+-rw-r--r--   0        0        0     1467 2024-03-05 12:28:28.554496 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.js
+-rw-r--r--   0        0        0       24 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.scss
+-rw-r--r--   0        0        0      178 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/sdc_user.organizer.js
+-rw-r--r--   0        0        0      112 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/sdc_user.style.scss
+-rw-r--r--   0        0        0      999 2024-03-05 11:56:18.698802 simpledomcontrol-0.5.1/sdc_user/Assets/tests/sdc_user.test.js
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/__init__.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/admin.py
+-rw-r--r--   0        0        0      147 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/apps.py
+-rw-r--r--   0        0        0        0 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/models.py
+-rw-r--r--   0        0        0      394 2024-03-05 20:52:54.936870 simpledomcontrol-0.5.1/sdc_user/sdc_urls.py
+-rw-r--r--   0        0        0     2331 2024-03-05 11:56:18.694802 simpledomcontrol-0.5.1/sdc_user/sdc_views.py
+-rw-r--r--   0        0        0      401 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/templates/sdc_user/sdc/sdc_login.html
+-rw-r--r--   0        0        0      327 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/templates/sdc_user/sdc/sdc_logout.html
+-rw-r--r--   0        0        0      144 2024-03-05 12:23:24.239188 simpledomcontrol-0.5.1/sdc_user/templates/sdc_user/sdc/sdc_user_nav_btn.html
+-rw-r--r--   0        0        0       60 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/tests.py
+-rw-r--r--   0        0        0       63 2024-01-15 08:35:05.110633 simpledomcontrol-0.5.1/sdc_user/views.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 simpledomcontrol-0.5.1/PKG-INFO
```

### Comparing `simpledomcontrol-0.5.0/pyproject.toml` & `simpledomcontrol-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SimpleDomControl"
-version = "0.05.00"
+version = "0.05.01"
 authors = [ "Martin Starman <private@martin-starman.com>", ]
 description = "Simple DOM control -> a django MVC framework"
 readme = "README.md"
 license = 'Apache License 2.0'
 
 packages = [{include = "sdc_core"}, {include = "sdc_user"}, {include = "sdc_tools"}]
 keywords = ["django", "MVC",]
```

### Comparing `simpledomcontrol-0.5.0/sdc_core/apps.py` & `simpledomcontrol-0.5.1/sdc_core/apps.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/consumers.py` & `simpledomcontrol-0.5.1/sdc_core/consumers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 import os
 import types
 import traceback
 from django.conf import settings
 from django.core.exceptions import PermissionDenied
 from django.core.files.uploadhandler import TemporaryFileUploadHandler
-from django.core.serializers.json import Serializer
+
 from django.utils.datastructures import MultiValueDict
 from django.utils.translation import gettext as _f
-from django.apps import apps
-from django.db.models import FileField
 from django.contrib.auth import get_user_model
 from channels.generic.websocket import WebsocketConsumer
 
 from asgiref.sync import async_to_sync
 import importlib
 import json
 
-from sdc_core.sdc_extentions.models import SdcModel
+from sdc_core.sdc_extentions.models import SdcModel, ConsumerSerializer, all_models
 from sdc_core.sdc_extentions.response import sdc_link_factory, sdc_link_obj_factory
 from sdc_core.sdc_extentions.import_manager import import_function
 from sdc_core.sdc_extentions.views import SdcAccessMixin
 
 import logging
 
 logger = logging.getLogger(__name__)
 User = get_user_model()
 
-ALL_MODELS = {
-    model.__name__: model for model in apps.get_models() if hasattr(model, '__is_sdc_model__')
-}
-
 importlist = []
-
+ALL_MODELS = all_models()
 
 class MsgManager:
     _messages = None
     _msg_filepath = os.path.abspath(settings.BASE_DIR / 'templates/sdc_strings.json')
 
     @property
     def messages(self):
@@ -67,34 +61,14 @@
     def _get_empty_msg(self, model):
         return {'save': {'header': f'{model} saved', 'msg': '{0} was successfully saved'},
                 'on_change': {'header': f'{model} was changed', 'msg': '{0} was changed'},
                 'create': {'header': f'{model} created', 'msg': '{0} was successfully created'},
                 'delete': {'header': f'{model} was deleted', 'msg': '{0} was changed'}}
 
 
-class ConsumerSerializer(Serializer):
-
-    def handle_m2m_field(self, obj, field):
-        super().handle_m2m_field(obj, field)
-        self._current[field.name] = {
-           'pk': self._current[field.name],
-           'model': field.related_model.__name__,
-           '__is_sdc_model__': True
-        }
-
-    def _value_from_field(self, obj, field):
-        if hasattr(field, 'foreign_related_fields') and ALL_MODELS.get(
-               field.related_model.__name__) == field.related_model:
-           return {'pk': super()._value_from_field(obj, field), 'model': field.related_model.__name__,
-                   '__is_sdc_model__': True}
-        if issubclass(field.__class__, FileField):
-            return field.value_from_object(obj).url
-        return super()._value_from_field(obj, field)
-
-
 class SDCConsumer(WebsocketConsumer):
 
     def connect(self):
         self.scope["session"]["channel_name"] = self.channel_name
         self.scope["session"].save()
         self.accept()
         self.group_list = []
@@ -216,23 +190,21 @@
         self.scope["session"].save()
         self.accept()
 
     def disconnect(self, close_code):
         pass
 
     def on_update(self, data):
-        if data['args']['data'].pk in self.ids:
-            data['args']['data'] = ConsumerSerializer().serialize([data['args']['data']])
+        if data['pk'] in self.ids:
             self.send(text_data=json.dumps(data))
 
     def on_create(self, data):
-        instance = data['args']['data']
+        instance = data['pk']
         try:
-            self._load_model().get(pk=instance.pk)
-            data['args']['data'] = ConsumerSerializer().serialize([instance])
+            self._load_model().get(pk=instance)
             self.send(text_data=json.dumps(data))
         except:
             pass
 
     def state_error(self, event):
         self.send(text_data=json.dumps({
             'type': event.get('type', 'error'),
```

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_controller_manager.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/add_controller_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/add_model_manager.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/add_model_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/options.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/options.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/sdc_core_manager.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/sdc_core_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/settings_manager.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/settings_manager.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/init_add/utils.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/init_add/utils.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_cc.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_cc.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_controller_infos.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_get_controller_infos.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_get_model_infos.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_get_model_infos.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_init.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_init.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_is_installed.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_is_installed.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_new_model.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_new_model.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_shell_execute_script.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_shell_execute_script.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_links.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_update_links.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/management/commands/sdc_update_url.py` & `simpledomcontrol-0.5.1/sdc_core/management/commands/sdc_update_url.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/sdc_extentions/forms.py` & `simpledomcontrol-0.5.1/sdc_core/sdc_extentions/forms.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/sdc_extentions/response.py` & `simpledomcontrol-0.5.1/sdc_core/sdc_extentions/response.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/sdc_extentions/search.py` & `simpledomcontrol-0.5.1/sdc_core/sdc_extentions/search.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/sdc_extentions/views.py` & `simpledomcontrol-0.5.1/sdc_core/sdc_extentions/views.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/Assets/gulpfile.jsx` & `simpledomcontrol-0.5.1/sdc_core/template_files/Assets/gulpfile.jsx`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/Assets/tests/config/pre-test-setup.js` & `simpledomcontrol-0.5.1/sdc_core/template_files/Assets/tests/config/pre-test-setup.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx` & `simpledomcontrol-0.5.1/sdc_core/template_files/Assets/webpack.config/webpack.default.config.jsx`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx` & `simpledomcontrol-0.5.1/sdc_core/template_files/Assets/webpack.config/webpack.production.config.jsx`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt` & `simpledomcontrol-0.5.1/sdc_core/template_files/apps/sdc_examples/Add_SDCUser.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/index.html` & `simpledomcontrol-0.5.1/sdc_core/template_files/apps/sdc_examples/index.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/apps/sdc_examples/server_call.txt` & `simpledomcontrol-0.5.1/sdc_core/template_files/apps/sdc_examples/server_call.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/asgi.py.txt` & `simpledomcontrol-0.5.1/sdc_core/template_files/asgi.py.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_controller.js.txt` & `simpledomcontrol-0.5.1/sdc_core/template_files/controller/template_controller.js.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/controller/template_test.js.text` & `simpledomcontrol-0.5.1/sdc_core/template_files/controller/template_test.js.text`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/models/detail.html` & `simpledomcontrol-0.5.1/sdc_core/template_files/models/detail.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/models/list.html` & `simpledomcontrol-0.5.1/sdc_core/template_files/models/list.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/package.json` & `simpledomcontrol-0.5.1/sdc_core/template_files/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972222222222222%*

 * *Differences: {"'dependencies'": "{'sdc_client': '^0.05.01'}"}*

```diff
@@ -2,15 +2,15 @@
     "author": "",
     "dependencies": {
         "@popperjs/core": "^2.11.8",
         "bootstrap": "^5.3.2",
         "esm": "^3.2.25",
         "jquery": "^3.7.0",
         "lodash": "^4.17.21",
-        "sdc_client": "^0.05.00"
+        "sdc_client": "^0.05.01"
     },
     "description": "",
     "devDependencies": {
         "@babel/core": "^7.23.7",
         "@babel/preset-react": "^7.23.3",
         "@babel/register": "^7.23.7",
         "babel-jest": "^29.7.0",
```

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/settings_extension.py.txt` & `simpledomcontrol-0.5.1/sdc_core/template_files/settings_extension.py.txt`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_core/template_files/templates/base.html` & `simpledomcontrol-0.5.1/sdc_core/template_files/templates/base.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_alert_messenger/sdc_alert_messenger.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_auto_submit/sdc_auto_submit.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_detail_view/sdc_detail_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_dummy/sdc_dummy.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_error/sdc_error.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_list_view/sdc_list_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_model_form/sdc_model_form.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigation_client/sdc_navigation_client.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_navigator/sdc_navigator.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_search_view/sdc_search_view.scss`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/controller/sdc_update_on_change/sdc_update_on_change.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/src/sdc_tools/sdc_tools.organizer.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/Assets/tests/sdc_tools.test.js` & `simpledomcontrol-0.5.1/sdc_tools/Assets/tests/sdc_tools.test.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/sdc_urls.py` & `simpledomcontrol-0.5.1/sdc_tools/sdc_urls.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/sdc_views.py` & `simpledomcontrol-0.5.1/sdc_tools/sdc_views.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/templates/elements/form.html` & `simpledomcontrol-0.5.1/sdc_tools/templates/elements/form.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/templates/elements/inline_form.html` & `simpledomcontrol-0.5.1/sdc_tools/templates/elements/inline_form.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/templates/email/base.html` & `simpledomcontrol-0.5.1/sdc_tools/templates/email/base.html`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/templatetags/addclass.py` & `simpledomcontrol-0.5.1/sdc_tools/templatetags/addclass.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_tools/templatetags/sdc_filter.py` & `simpledomcontrol-0.5.1/sdc_tools/templatetags/sdc_filter.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js` & `simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_login/sdc_login.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js` & `simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_logout/sdc_logout.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.js` & `simpledomcontrol-0.5.1/sdc_user/Assets/src/sdc_user/controller/sdc_user_nav_btn/sdc_user_nav_btn.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_user/Assets/tests/sdc_user.test.js` & `simpledomcontrol-0.5.1/sdc_user/Assets/tests/sdc_user.test.js`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/sdc_user/sdc_views.py` & `simpledomcontrol-0.5.1/sdc_user/sdc_views.py`

 * *Files identical despite different names*

### Comparing `simpledomcontrol-0.5.0/PKG-INFO` & `simpledomcontrol-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleDomControl
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple DOM control -> a django MVC framework
 Home-page: https://github.com/StarmanMartin/sdc
 License: Apache-2.0
 Keywords: django,MVC
 Author: Martin Starman
 Author-email: private@martin-starman.com
 Requires-Python: >=3.10,<4.0
```

