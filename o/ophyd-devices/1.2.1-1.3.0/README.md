# Comparing `tmp/ophyd_devices-1.2.1.tar.gz` & `tmp/ophyd_devices-1.3.0.tar.gz`

## Comparing `ophyd_devices-1.2.1.tar` & `ophyd_devices-1.3.0.tar`

### file list

```diff
@@ -1,403 +1,402 @@
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/README.md
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/.git_hooks/pre-commit
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.gitignore
--rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.gitlab-ci.yml
--rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.pylintrc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.readthedocs.yaml
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/CHANGELOG.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/LICENSE
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/README.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_config_template.yaml
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.git_hooks/post-commit
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.git_hooks/pre-commit
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.gitlab/issue_templates/bug_report_template.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.gitlab/issue_templates/documentation_update_template.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.gitlab/issue_templates/feature_request_template.md
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/.gitlab/merge_request_templates/default.md
--rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/demo.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/pyproject.toml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
--rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/main.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/prettytable.py
--rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/progressbar.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/signals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/conftest.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
--rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_device_progress.py
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_live_table.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
--rw-r--r--   0        0        0    25202 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/README.md
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/pyproject.toml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/__init__.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bec_service.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bec_yaml_loader.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/client.py
--rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/connector.py
--rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    31017 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/device.py
--rw-r--r--   0        0        0    23466 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    38756 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/logger.py
--rw-r--r--   0        0        0    24060 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/plugin_helper.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/queue_items.py
--rw-r--r--   0        0        0    41753 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/request_items.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_data.py
--rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_report.py
--rw-r--r--   0        0        0    16698 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/serialization.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22495 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/import_utils.py
--rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/proxy.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/rpc_utils.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/scan_utils.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/threading_utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_bec_logger.py
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_callback_handler.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_config_helper.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_core_utils.py
--rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_device_manager.py
--rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_file_utils.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_import_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_pdf_writer.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_plugin_helper.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_redis_connector.py
--rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_data.py
--rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_items.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_object.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/tests/test_yaml_loader.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/init_config.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/pyproject.toml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    19037 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22204 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    16121 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    35246 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18915 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35721 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    51830 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25417 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    53947 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
--rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/bin/install_bec_dev.sh
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/ci/Dockerfile.run_pytest
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/ci/Dockerfile.run_server
--rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/ci/build_python_services.sh
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/ci/docker-compose.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/ci/functionalAccounts.json
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/ci/semantic_release.toml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/ci/test_config.yaml
--rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/architecture/BEC.drawio
--rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/architecture/BEC_config_db.drawio
--rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/architecture/BEC_config_db.svg
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/architecture/bec_architecture.png
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/Makefile
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/conf.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/make.bat
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/requirements.txt
--rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/_static/bec.png
--rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/_static/custom.css
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/_static/switcher.json
--rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/_static/gif/bec_plotter.gif
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/api_reference/api_reference.md
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/api_reference/modules.rst
--rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/BEC_context_user_centric.png
--rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/bec_architecture.png
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/bec_device_structure.drawio
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/bec_device_structure.png
--rw-r--r--   0        0        0   185658 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/bec_widgets_glance.png
--rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/gauss_scatter_plot.png
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/index_api.svg
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/index_contribute.svg
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/index_getting_started.svg
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/index_user_guide.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/portrait_48dp.svg
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/precision_manufacturing_48dp.svg
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/rocket_launch_48dp.svg
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/simulation_context_diagram.drawio
--rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/simulation_context_diagram.png
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/tab-complete-devices.png
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/timeline_48dp.svg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/toc_48dp.svg
--rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/vscode_debug_button.png
--rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/vscode_with_annotations.drawio
--rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/vscode_with_annotations.png
--rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/assets/wm-devices.png
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/developer.md
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/glossary.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/data_acess/data_access.md
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/data_acess/event_data.md
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/devices/bec_sim.md
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/devices/device_configuration.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/devices/devices.md
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/devices/external_sources.md
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/devices/ophyd.md
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/architecture.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/bec_config.md
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/bec_plugins.md
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/contributing.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/getting_started.md
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/install_developer_env.md
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/logs.md
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/tests.md
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/vscode.md
--rw-r--r--   0        0        0    16567 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/scans/scans.md
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/user_interfaces/bec_cli.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/user_interfaces/bec_gui.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/developer/user_interfaces/user_interfaces.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/introduction/introduction.md
--rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/user/command_line_interface.md
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/user/data_access_and_plotting.md
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/user/devices.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/user/graphical_user_interface.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/user/installation.md
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/docs/source/user/user.md
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/pytest_bec_e2e/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/ophyd_patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/configs/__init__.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/configs/ophyd_devices_simulation.yaml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/configs/ophyd_simulation.yaml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/configs/sls_devices.yaml
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/SpmBase.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/XbpmBase.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/__init__.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/device_list.md
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/epics_motor_ex.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/mono_dccm.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/slits.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/sls_detector.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/sls_devices.py
--rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/devices/specMotors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/interfaces/base_classes/__init__.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
--rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/interfaces/base_classes/psi_detector_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/interfaces/protocols/__init__.py
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/interfaces/protocols/bec_protocols.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/__init__.py
--rw-r--r--   0        0        0    27852 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/sim.py
--rw-r--r--   0        0        0    27990 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/sim_data.py
--rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/sim_frameworks.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/sim_signals.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/sim_test_devices.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/sim_utils.py
--rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/sim_xtreme.py
--rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
--rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/__init__.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/bec_device_base.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/bec_scaninfo_mixin.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/bec_utils.py
--rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/controller.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/dynamic_pseudo.py
--rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/socket.py
--rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/ophyd_devices/utils/static_device_test.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/tests/test_base_classes.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/tests/test_controller.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/tests/test_dynamic_pseudo.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/tests/test_ophyd_status_obj.py
--rw-r--r--   0        0        0    12549 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/tests/test_simulation.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/tests/test_socket.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/tests/test_static_device_test.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/LICENSE
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ophyd_devices-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/README.md
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.gitignore
+-rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.gitlab-ci.yml
+-rw-r--r--   0        0        0    18519 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.pylintrc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.readthedocs.yaml
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/CHANGELOG.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/LICENSE
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/README.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_config_template.yaml
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.git_hooks/post-commit
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.git_hooks/pre-commit
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.gitlab/issue_templates/bug_report_template.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.gitlab/issue_templates/documentation_update_template.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.gitlab/issue_templates/feature_request_template.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/.gitlab/merge_request_templates/default.md
+-rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/demo.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8631 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py
+-rw-r--r--   0        0        0    10038 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    12166 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/conftest.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0    25294 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/README.md
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/pyproject.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bec_yaml_loader.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9619 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/client.py
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/connector.py
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    31017 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/device.py
+-rw-r--r--   0        0        0    23466 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    38756 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/logger.py
+-rw-r--r--   0        0        0    24060 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    41753 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    11042 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    16934 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22495 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/import_utils.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/proxy.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/rpc_utils.py
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/scan_utils.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/threading_utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26550 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25863 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_file_utils.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_import_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    22325 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/tests/test_yaml_loader.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/init_config.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/setup_device_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/post-commit
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/git_hooks/pre-commit
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/README.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/pyproject.toml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9729 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    19037 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22629 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22204 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    16121 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    35246 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    21324 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35937 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    54743 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10735 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25417 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    27545 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_server_scan_manager.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    53947 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    95331 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py
+-rwxr-xr-x   0        0        0     3629 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/bin/install_bec_dev.sh
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/ci/Dockerfile.run_pytest
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/ci/Dockerfile.run_server
+-rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/ci/build_python_services.sh
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/ci/docker-compose.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/ci/functionalAccounts.json
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/ci/semantic_release.toml
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/ci/test_config.yaml
+-rw-r--r--   0        0        0   307212 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/architecture/BEC.drawio
+-rw-r--r--   0        0        0   124683 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/architecture/BEC_config_db.drawio
+-rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/architecture/BEC_config_db.svg
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/architecture/bec_architecture.png
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/Makefile
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/conf.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/make.bat
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/requirements.txt
+-rw-r--r--   0        0        0    41260 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/_static/bec.png
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/_static/custom.css
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/_static/switcher.json
+-rw-r--r--   0        0        0  4672990 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/_static/gif/bec_plotter.gif
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/api_reference/api_reference.md
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/api_reference/modules.rst
+-rw-r--r--   0        0        0   310535 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/BEC_context_user_centric.png
+-rw-r--r--   0        0        0   278334 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/bec_architecture.png
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/bec_device_structure.drawio
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/bec_device_structure.png
+-rw-r--r--   0        0        0   185658 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/bec_widgets_glance.png
+-rw-r--r--   0        0        0    17460 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/gauss_scatter_plot.png
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/index_api.svg
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/index_contribute.svg
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/index_getting_started.svg
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/index_user_guide.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/portrait_48dp.svg
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/precision_manufacturing_48dp.svg
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/rocket_launch_48dp.svg
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/simulation_context_diagram.drawio
+-rw-r--r--   0        0        0    69323 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/simulation_context_diagram.png
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/tab-complete-devices.png
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/timeline_48dp.svg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/toc_48dp.svg
+-rw-r--r--   0        0        0    37244 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/vscode_debug_button.png
+-rw-r--r--   0        0        0   374770 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/vscode_with_annotations.drawio
+-rw-r--r--   0        0        0   711275 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/vscode_with_annotations.png
+-rw-r--r--   0        0        0    96330 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/assets/wm-devices.png
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/developer.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/glossary.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/data_acess/data_access.md
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/data_acess/event_data.md
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/devices/bec_sim.md
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/devices/device_configuration.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/devices/devices.md
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/devices/external_sources.md
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/devices/ophyd.md
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/architecture.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/bec_config.md
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/bec_plugins.md
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/contributing.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/getting_started.md
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/install_developer_env.md
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/logs.md
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/tests.md
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/vscode.md
+-rw-r--r--   0        0        0    17125 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/scans/scans.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/user_interfaces/bec_cli.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/user_interfaces/bec_gui.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/developer/user_interfaces/user_interfaces.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/introduction/introduction.md
+-rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/user/command_line_interface.md
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/user/data_access_and_plotting.md
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/user/devices.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/user/graphical_user_interface.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/user/installation.md
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/docs/source/user/user.md
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/pytest_bec_e2e/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/pytest_bec_e2e/pytest_bec_e2e/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/ophyd_patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/configs/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/configs/ophyd_devices_simulation.yaml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/configs/ophyd_simulation.yaml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/configs/sls_devices.yaml
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/devices/SpmBase.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/devices/XbpmBase.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/devices/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/devices/device_list.md
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/devices/epics_motor_ex.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/devices/sls_detector.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/devices/sls_devices.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/interfaces/base_classes/__init__.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py
+-rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py
+-rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/interfaces/protocols/bec_protocols.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/__init__.py
+-rw-r--r--   0        0        0    27852 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim.py
+-rw-r--r--   0        0        0    27990 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim_data.py
+-rw-r--r--   0        0        0    12071 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim_frameworks.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim_monitor_async.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim_signals.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim_test_devices.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim_utils.py
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/sim_xtreme.py
+-rw-r--r--   0        0        0   671622 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0   669534 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   670586 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt
+-rw-r--r--   0        0        0   668300 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/__init__.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/bec_device_base.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/bec_scaninfo_mixin.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/bec_utils.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/controller.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/dynamic_pseudo.py
+-rw-r--r--   0        0        0     7309 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/socket.py
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/ophyd_devices/utils/static_device_test.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/tests/test_base_classes.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/tests/test_controller.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/tests/test_dynamic_pseudo.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/tests/test_ophyd_status_obj.py
+-rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/tests/test_simulation.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/tests/test_socket.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/tests/test_static_device_test.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ophyd_devices-1.3.0/PKG-INFO
```

### Comparing `ophyd_devices-1.2.1/.gitlab-ci.yml` & `ophyd_devices-1.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/CHANGELOG.md` & `ophyd_devices-1.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # CHANGELOG
 
 
 
+## v1.3.0 (2024-06-03)
+
+### Documentation
+
+* docs: Update device list ([`f9b126c`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/f9b126c60ce710fba221ffb208d66541b8264c0b))
+
+* docs: Update device list ([`be25cba`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/be25cbae92540b074bb4533331656d20a049a809))
+
+### Feature
+
+* feat: add async monitor, add on_complete to psi_det_base and rm duplicated mocks, closes #67 ([`1aece61`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/1aece61a3b09267f87f0771b163a5d07b4549eff))
+
+### Refactor
+
+* refactor: add .wait() to set methods ([`7334925`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/73349257ee0228a9563051d4f8e0bf5f7e6b551f))
+
+* refactor: removed deprecated devices ([`8ef6d10`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/8ef6d10eb759e6ce874ddf05a38c586e9475eed3))
+
+### Test
+
+* test: add tests for new device ([`c554422`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/c5544226be3f12d238a0793a0f41da07af36e460))
+
+
 ## v1.2.1 (2024-05-29)
 
 ### Documentation
 
 * docs: Update device list ([`5a591ce`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/5a591ce024b7815a432460fe9e8d97e648dcdb5e))
 
 * docs: Update device list ([`ae0c766`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/ae0c766975cdfc69ffe9d48eca92ad8d51a0497c))
@@ -116,18 +139,14 @@
 
 * ci: fixed typo ([`81f1fee`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/81f1feea853882e8d557063612cc0acc601bbe2a))
 
 * ci: fixed rules for downstream pipelines ([`f5e69f9`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/f5e69f9b9528871d9a011b2257b87c1faf89e6b0))
 
 * ci: limit stages to run in child pipelines ([`815921a`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/815921a6c9cd97e5df94a584c5d4c2c22a4d408a))
 
-* ci: removed awi-utils for now ([`27d4b6a`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/27d4b6ae83ec3d0f4d7a85c3cd4f6f70ecd528eb))
-
-* ci: added parent-child pipelines ([`e27d2db`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/e27d2db4ac21830c95f2db2ccba58c650c25cad5))
-
 ### Documentation
 
 * docs: improved doc strings for controllerr ([`339f050`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/339f050a8662de86ed2528ad4ffed18482dd546b))
 
 ### Fix
 
 * fix: fixed controller error classes ([`c3fa7ad`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/c3fa7ad30d1b9a151bce599b34b4a3f82e4e6ce8))
@@ -137,21 +156,7 @@
 * refactor: added common controller methods ([`00b3ae8`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/00b3ae82580df6bbe8a01a52d37c43199cf761bd))
 
 ### Unknown
 
 * Update file .gitlab-ci.yml ([`2f8772b`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/2f8772b618836fc4029691ad03f7dafee17f1ca5))
 
 * Update file .gitlab-ci.yml ([`bd01f60`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/bd01f6050a6c4957e4943577dff1ff53a5179f8b))
-
-
-## v0.33.5 (2024-05-02)
-
-### Fix
-
-* fix: fixed device data signature ([`e8290db`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/e8290dbf4466f1415fb9c963ae203a4e6da7cc42))
-
-
-## v0.33.4 (2024-04-29)
-
-### Ci
-
-* ci: removed redundant build step ([`a919632`](https://gitlab.psi.ch/bec/ophyd_devices/-/commit/a9196328e7d7efe4b6718b22d72c6df9bf59411c))
```

### Comparing `ophyd_devices-1.2.1/README.md` & `ophyd_devices-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.3.0/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.3.0/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.3.0/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/.gitignore` & `ophyd_devices-1.3.0/bec/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/.gitlab-ci.yml` & `ophyd_devices-1.3.0/bec/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/.pylintrc` & `ophyd_devices-1.3.0/bec/.pylintrc`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/.readthedocs.yaml` & `ophyd_devices-1.3.0/bec/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/CHANGELOG.md` & `ophyd_devices-1.3.0/bec/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,62 @@
 # CHANGELOG
 
 
 
+## v2.13.1 (2024-06-03)
+
+### Fix
+
+* fix: fixed support for mv during scan defs; closes #308 ([`835bf50`](https://gitlab.psi.ch/bec/bec/-/commit/835bf5004ad1c9aaec1792ed20f3ffc613584d31))
+
+
+## v2.13.0 (2024-06-03)
+
+### Documentation
+
+* docs: improved scan stub docs and glossary ([`e04cf65`](https://gitlab.psi.ch/bec/bec/-/commit/e04cf65f9cbcff4ea8fe3676813e4dce663757a4))
+
+### Feature
+
+* feat(scan_server): added set_with_response and request_is_completed stubs ([`8ac80c1`](https://gitlab.psi.ch/bec/bec/-/commit/8ac80c11ce0e83bb782254b06e2552e8a15c1002))
+
+* feat(scan_server): convert arg inputs to supported scan arg types ([`30b4528`](https://gitlab.psi.ch/bec/bec/-/commit/30b4528de5e448a0c3477d49dff727703de3ed17))
+
+### Fix
+
+* fix(scan_server): worker respects use_scan_progress_report ([`3ad46ef`](https://gitlab.psi.ch/bec/bec/-/commit/3ad46efb148ab9c32e34a6500f1f1af0dbd7144c))
+
+* fix(ipython_client): readback callback must listen to instruction RID ([`c4551d3`](https://gitlab.psi.ch/bec/bec/-/commit/c4551d3b953bc97557e285f350e81b000f7c2cbe))
+
+* fix: minor cleanup ([`8d4a066`](https://gitlab.psi.ch/bec/bec/-/commit/8d4a066832dc45d67b77d13b484d7cd2e565c2f9))
+
+* fix(scan_server): fixed default args ([`0f42a49`](https://gitlab.psi.ch/bec/bec/-/commit/0f42a4926de28252f01d9f9fab53244cc099ca21))
+
+* fix(scan_server): simplify scan args ([`005ff56`](https://gitlab.psi.ch/bec/bec/-/commit/005ff5685609b403b35131cdff0380d8e5b2b742))
+
+* fix(bec_lib): convert devices to strings for scan requests ([`3b176f7`](https://gitlab.psi.ch/bec/bec/-/commit/3b176f7b97087fe87fcfaacd4d575c27be4cbcaf))
+
+### Refactor
+
+* refactor(scan_server): cleanup of scan args ([`3acc13a`](https://gitlab.psi.ch/bec/bec/-/commit/3acc13a8c4fa45765c1b29f446c01df21b056135))
+
+### Test
+
+* test(scan_server): added test for convert_arg_input ([`a302844`](https://gitlab.psi.ch/bec/bec/-/commit/a302844d70659e2d1b074a76c2649a2c15bf0754))
+
+* test: added tests for stubs and contlineflyscan ([`8fed5f6`](https://gitlab.psi.ch/bec/bec/-/commit/8fed5f64a09ea28bb911aaf57a96ba4b50498a56))
+
+
+## v2.12.6 (2024-05-31)
+
+### Fix
+
+* fix: end the color sequence ([`22be4c4`](https://gitlab.psi.ch/bec/bec/-/commit/22be4c4c6b54133277411e837e9c102aa39685d3))
+
+
 ## v2.12.5 (2024-05-28)
 
 ### Fix
 
 * fix: remove deprecated arg speed from deviceconfig ([`67f0bea`](https://gitlab.psi.ch/bec/bec/-/commit/67f0beac75bbeecf69768662e373b96a0839f122))
 
 
@@ -91,69 +142,7 @@
 
 ### Feature
 
 * feat(scan_bundler): added scan progress ([`27befe9`](https://gitlab.psi.ch/bec/bec/-/commit/27befe966607a3ae319dbee3af9e59ef0d044bc8))
 
 
 ## v2.11.1 (2024-05-16)
-
-### Ci
-
-* ci: cleanup ARGs in dockerfiles ([`b670d1a`](https://gitlab.psi.ch/bec/bec/-/commit/b670d1aa6b6e2af0cb09e7dbc77ea5d1bc66593b))
-
-* ci: run AdditionalTests jobs on pipeline start
-
-This is a followup to !573 ([`c9ece7e`](https://gitlab.psi.ch/bec/bec/-/commit/c9ece7ef2f1f9b052ed9b92bcb29463cf8371c64))
-
-### Documentation
-
-* docs(bec_lib): improved scripts documentation ([`79f487e`](https://gitlab.psi.ch/bec/bec/-/commit/79f487ea8b9dc135102204872390631e59a60e54))
-
-### Fix
-
-* fix(bec_lib): fixed loading scripts from plugins
-
-User scripts from plugins were still relying on the old plugin structure ([`3264434`](https://gitlab.psi.ch/bec/bec/-/commit/3264434d40647d260400045f7bbd4c2ee9bb2c4e))
-
-
-## v2.11.0 (2024-05-15)
-
-### Feature
-
-* feat: add utility function to determine instance of an object by class name ([`0ccd13c`](https://gitlab.psi.ch/bec/bec/-/commit/0ccd13cd738dc12d4a587b4c5e0d6b447d7cfc50))
-
-* feat: add utilities to lazy import a module ([`a37ae57`](https://gitlab.psi.ch/bec/bec/-/commit/a37ae577f68c154dc3da544816b7c7f0cb532c50))
-
-* feat: add &#39;Proxy&#39; to bec_lib utils ([`11a3f6d`](https://gitlab.psi.ch/bec/bec/-/commit/11a3f6daa46b3e6a82b66bd781b7590d01478b54))
-
-### Style
-
-* style: create directory to contain utils ([`549994d`](https://gitlab.psi.ch/bec/bec/-/commit/549994d0fdffcd4f5ed0948e1cd4cd4a0d0092af))
-
-
-## v2.10.4 (2024-05-14)
-
-### Build
-
-* build: fixed fakeredis version for now ([`51dfe69`](https://gitlab.psi.ch/bec/bec/-/commit/51dfe69298170eba7220fcb506d99515c46ea32a))
-
-### Ci
-
-* ci: update dependencies and add ci job to check for package versions ([`2aafb24`](https://gitlab.psi.ch/bec/bec/-/commit/2aafb249e8f0b8afa8ede0dc4ba0a811ecb2a70f))
-
-### Fix
-
-* fix: disabled script linter for now ([`5c5c18e`](https://gitlab.psi.ch/bec/bec/-/commit/5c5c18ef0eab33ebaa33d1a0daa846ea7f2f59a8))
-
-
-## v2.10.3 (2024-05-08)
-
-### Fix
-
-* fix: upgraded to ophyd_devices v1 ([`3077dbe`](https://gitlab.psi.ch/bec/bec/-/commit/3077dbe22ae50e6aae317c72022df6ea88b14cce))
-
-
-## v2.10.2 (2024-05-08)
-
-### Fix
-
-* fix(RedisConnector): add &#39;from_start&#39; support in &#39;register&#39; for streams ([`f059bf9`](https://gitlab.psi.ch/bec/bec/-/commit/f059bf9318038404ebbcc82b5abf5cd148486021))
```

### Comparing `ophyd_devices-1.2.1/bec/LICENSE` & `ophyd_devices-1.3.0/bec/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/README.md` & `ophyd_devices-1.3.0/bec/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/.gitlab/issue_templates/documentation_update_template.md` & `ophyd_devices-1.3.0/bec/.gitlab/issue_templates/documentation_update_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/.gitlab/issue_templates/feature_request_template.md` & `ophyd_devices-1.3.0/bec/.gitlab/issue_templates/feature_request_template.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/.gitlab/merge_request_templates/default.md` & `ophyd_devices-1.3.0/bec/.gitlab/merge_request_templates/default.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/demo.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/pyproject.toml` & `ophyd_devices-1.3.0/bec/bec_ipython_client/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_ipython_client"
-version = "2.12.5"
+version = "2.13.1"
 description = "BEC IPython client"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/bec_magics.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/bec_startup.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/main.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/prettytable.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/progressbar.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/signals.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/device_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,18 @@
                 "Scan is enqueued and is waiting for execution. Current position in queue:"
                 f" {queue.queue_position + 1}. Queue status: {status}.",
                 end="\r",
                 flush=True,
             )
         available_blocks = self._available_req_blocks(queue, request)
         req_block = available_blocks[self._request_block_index[req_id]]
-        if req_block["content"]["scan_type"] == "open_scan_def":
+        if req_block["content"]["scan_type"] in [
+            "open_scan_def",
+            "mv",
+        ]:  # TODO: make this more general for all scan types that don't have report instructions
             return True
 
         report_instructions = req_block["report_instructions"]
         if not report_instructions:
             return False
         self._process_report_instructions(report_instructions)
```

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/move_device.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,15 +128,20 @@
                 self._print_client_msgs_asap()
 
                 msgs = data_source.get_request_done_msgs()
                 request_ids = [
                     msg.metadata["RID"] if (msg and msg.metadata.get("RID")) else None
                     for msg in msgs
                 ]
-                if set(request_ids) != set([self.request.metadata["RID"]]):
+
+                if self.report_instruction:
+                    compare_rids = set([self.report_instruction["readback"]["RID"]])
+                else:
+                    compare_rids = set([self.request.metadata["RID"]])
+                if set(request_ids) != set(compare_rids):
                     progress.sleep()
                     continue
 
                 req_done = True
                 for dev, msg in zip(self.devices, msgs):
                     if not msg:
                         continue
```

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml` & `ophyd_devices-1.3.0/bec/bec_ipython_client/bec_ipython_client/plugins/flomni/flomni_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_beamline_mixins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_bec_client.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_bec_client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_device_progress.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_device_progress.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_live_table.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_live_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/client_tests/test_move_callback.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/client_tests/test_move_callback.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/end-2-end/test_scans_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,24 +474,26 @@
     scans = bec.scans
     dev = bec.device_manager.devices
     scan_number = bec.queue.next_scan_number
     with scans.scan_def:
         scans.line_scan(dev.samx, -5, 5, steps=10, exp_time=0.1, relative=False)
         scans.umv(dev.samy, 5, relative=False)
         scans.line_scan(dev.samx, -5, 5, steps=10, exp_time=0.1, relative=False)
+        scans.mv(dev.samx, 0, relative=False)
 
     assert scan_number == bec.queue.next_scan_number - 1
 
     scan_number = bec.queue.next_scan_number
 
     @scans.scan_def
     def scan_def_with_decorator():
         scans.line_scan(dev.samx, -5, 5, steps=10, exp_time=0.1, relative=False)
         scans.umv(dev.samy, 5, relative=False)
         scans.line_scan(dev.samx, -5, 5, steps=10, exp_time=0.1, relative=False)
+        scans.mv(dev.samx, 0, relative=False)
 
     scan_def_with_decorator()
     assert scan_number == bec.queue.next_scan_number - 1
 
 
 @pytest.mark.timeout(100)
 def test_group_def(bec_ipython_client_fixture):
```

### Comparing `ophyd_devices-1.2.1/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py` & `ophyd_devices-1.3.0/bec/bec_ipython_client/tests/end-2-end/test_scans_lib_e2e.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/README.md` & `ophyd_devices-1.3.0/bec/bec_lib/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/pyproject.toml` & `ophyd_devices-1.3.0/bec/bec_lib/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_lib"
-version = "2.12.5"
+version = "2.13.1"
 description = "BEC library"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/alarm_handler.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/async_data.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bec_service.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bec_yaml_loader.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bec_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bl_checks.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/bl_conditions.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/callback_handler.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/channel_monitor.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/client.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/config_helper.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/connector.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/dap_plugin_objects.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/dap_plugins.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/device.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/devicemanager.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/endpoints.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/file_utils.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/lmfit_serializer.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/logbook_connector.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/logger.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/messages.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/numpy_encoder.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/observer.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/pdf_writer.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/plugin_helper.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/queue_items.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/redis_connector.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/request_items.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_data.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_items.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_manager.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scan_report.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scans.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scans.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
 from toolz import partition
 from typeguard import typechecked
 
 from bec_lib import messages
+from bec_lib.bec_errors import ScanAbortion
 from bec_lib.device import DeviceBase
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.scan_report import ScanReport
 from bec_lib.signature_serializer import dict_to_signature
 from bec_lib.utils import scan_to_csv
 
@@ -263,15 +264,15 @@
             args:
             bundle_size: number of parameters per bundle
 
         Returns:
 
         """
         if not bundle_size:
-            return args
+            return tuple(cmd.name if hasattr(cmd, "name") else cmd for cmd in args)
         params = {}
         for cmds in partition(bundle_size, args):
             cmds_serialized = [cmd.name if hasattr(cmd, "name") else cmd for cmd in cmds]
             params[cmds_serialized[0]] = cmds_serialized[1:]
         return params
 
     @property
@@ -320,14 +321,16 @@
     """ScanDef is a ContextDecorator for defining a new scan"""
 
     def __init__(self, parent: Scans = None) -> None:
         super().__init__()
         self.parent = parent
 
     def __enter__(self):
+        if self.parent._scan_def_id is not None:
+            raise ScanAbortion("Nested scan definitions currently not supported.")
         scan_def_id = str(uuid.uuid4())
         self.parent._scan_def_id = scan_def_id
         self.parent.open_scan_def()
         return self
 
     def __exit__(self, *exc):
         if exc[0] is None:
```

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/scibec_validator.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/serialization.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/service_config.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/signature_serializer.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/user_scripts_mixin.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/configs/demo_config.yaml` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/configs/openapi_schema.json` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/fixtures.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/test_config.yaml` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/tests/utils.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/import_utils.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/proxy.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/rpc_utils.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/bec_lib/utils/scan_utils.py` & `ophyd_devices-1.3.0/bec/bec_lib/bec_lib/utils/scan_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_async_data.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_beamline_checks.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_bec_logger.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_bec_messages.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_bec_service.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_bec_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_bl_conditions.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_callback_handler.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_channel_monitor.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_channel_monitor.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_config_helper.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_core_utils.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_dap_plugins.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_dap_plugins.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_device_manager.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_devices.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_file_utils.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_lmfit_serializer.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_observer.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_plugin_helper.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_plugin_helper.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_redis_connector.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_redis_connector_fakeredis.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_redis_connector_fakeredis.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_context.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_data.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_items.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_items.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_manager.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_object.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_object.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_scan_report.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_serializer.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_signature_serializer.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_user_scripts_mixin.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/tests/test_yaml_loader.py` & `ophyd_devices-1.3.0/bec/bec_lib/tests/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/create_plugin_structure.py` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/create_plugin_structure.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/init_config.py` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/README_template_tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/gitignore` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/post_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/pre_startup.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py` & `ophyd_devices-1.3.0/bec/bec_lib/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/pyproject.toml` & `ophyd_devices-1.3.0/bec/bec_server/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.12.5"
+version = "2.13.1"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/service_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/service_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         """
         Start the BEC server using the available interface.
         """
         if self.interface == "tmux":
             print("Starting BEC server using tmux...")
             tmux_start(self.bec_path, self.config_path, self.SERVICES)
             print(
-                f"{bcolors.OKCYAN}{bcolors.BOLD}Use `tmux attach -t bec` to attach to the BEC server. Once connected, use `ctrl+b d` to detach again."
+                f"{bcolors.OKCYAN}{bcolors.BOLD}Use `tmux attach -t bec` to attach to the BEC server. Once connected, use `ctrl+b d` to detach again.{bcolors.ENDC}"
             )
         elif self.interface == "iterm2":
             pass
         else:
             # no tmux
             return subprocess_start(self.bec_path, self.config_path, self.SERVICES)
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/dap_server.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/dap_service.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/dap_service_manager.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/lmfit1d_service.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/data_processing/cli/launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/device_server.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/rpc_mixin.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/cli/launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/devices/config_update_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/devices/device_serializer.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/devices/devicemanager.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/device_server/tests/utils.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/default_writer.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/file_writer.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/file_writer_manager.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/merged_dicts.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer/cli/launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/bec_emitter.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/emitter.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/scan_bundler.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_bundler/cli/launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/device_validation.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/path_optimization.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_assembler.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_guard.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_manager.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+"""
+Scan Manager loads the available scans and publishes them to redis.
+"""
+
 import inspect
 
 from bec_lib import plugin_helper
+from bec_lib.device import DeviceBase
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 from bec_lib.messages import AvailableResourceMessage
 from bec_lib.signature_serializer import signature_to_dict
 
 from . import scans as ScanServerScans
 
 logger = bec_logger.logger
 
 
 class ScanManager:
+    """
+    Scan Manager loads the available scans and publishes them to redis.
+    """
 
     def __init__(self, *, parent):
         """
         Scan Manager loads and manages the available scans.
         """
         self.parent = parent
         self.available_scans = {}
@@ -70,20 +78,43 @@
             for report_cls in report_classes:
                 if issubclass(scan_cls, report_cls):
                     base_cls = report_cls.__name__
             self.scan_dict[scan_cls.__name__] = scan_cls
             self.available_scans[scan_cls.scan_name] = {
                 "class": scan_cls.__name__,
                 "base_class": base_cls,
-                "arg_input": scan_cls.arg_input,
+                "arg_input": self.convert_arg_input(scan_cls.arg_input),
                 "required_kwargs": scan_cls.required_kwargs,
                 "arg_bundle_size": scan_cls.arg_bundle_size,
                 "doc": scan_cls.__doc__ or scan_cls.__init__.__doc__,
                 "signature": signature_to_dict(scan_cls.__init__),
             }
 
+    def convert_arg_input(self, arg_input) -> dict:
+        """
+        Convert the arg_input to supported data types
+
+        Args:
+            arg_input: dict
+
+        Returns:
+            dict: converted arg_input
+        """
+        for key, value in arg_input.items():
+            if isinstance(value, ScanServerScans.ScanArgType):
+                continue
+            if issubclass(value, DeviceBase):
+                # once we have generalized the device types, this should be removed
+                arg_input[key] = "device"
+            elif issubclass(value, bool):
+                # should be unified with the ScanArgType.BOOL
+                arg_input[key] = "boolean"
+            else:
+                arg_input[key] = value.__name__
+        return arg_input
+
     def publish_available_scans(self):
         """send all available scans to the broker"""
         self.parent.connector.set(
             MessageEndpoints.available_scans(),
             AvailableResourceMessage(resource=self.available_scans),
         )
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_queue.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_server.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_stubs.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_stubs.py`

 * *Files 14% similar despite different names*

```diff
@@ -118,26 +118,64 @@
         return_val = msg.content.get("return_val")
         if not isinstance(return_val, dict):
             return return_val
         if return_val.get("type") == "status" and return_val.get("RID"):
             return Status(self.connector, return_val.get("RID"))
         return return_val
 
+    def set_with_response(
+        self, *, device: str, value: float, request_id: str = None, metadata=None
+    ) -> Generator[None, None, None]:
+        """Set a device to a specific value and return the request ID. Use :func:`request_is_completed` to later check if the request is completed.
+
+        Args:
+            device (str): Device name.
+            value (float): Target value.
+
+        Returns:
+            Generator[None, None, None]: Generator that yields a device message.
+
+        see also: :func:`request_is_completed`
+
+        """
+        request_id = str(uuid.uuid4()) if request_id is None else request_id
+        metadata = metadata if metadata is not None else {}
+        metadata.update({"response": True, "RID": request_id})
+        yield from self.set(device=device, value=value, wait_group="set", metadata=metadata)
+        return request_id
+
+    def request_is_completed(self, RID: str) -> bool:
+        """Check if a request that was initiated with :func:`set_with_response` is completed.
+
+        Args:
+            RID (str): Request ID.
+
+        Returns:
+            bool: True if the request is completed, False otherwise.
+
+        """
+        msg = self.connector.lrange(MessageEndpoints.device_req_status_container(RID), 0, -1)
+        if not msg:
+            return False
+        return True
+
     def set_and_wait(
         self, *, device: list[str], positions: list | np.ndarray
     ) -> Generator[None, None, None]:
         """Set devices to a specific position and wait completion.
 
         Args:
             device (list[str]): List of device names.
             positions (list | np.ndarray): Target position.
 
         Returns:
             Generator[None, None, None]: Generator that yields a device message.
 
+        see also: :func:`set`, :func:`wait`, :func:`set_with_response`
+
         """
         if not isinstance(positions, list) and not isinstance(positions, np.ndarray):
             positions = [positions]
         if len(positions) == 0:
             return
         for ind, val in enumerate(device):
             yield from self.set(device=val, value=positions[ind], wait_group="scan_motor")
@@ -275,33 +313,39 @@
 
     def close_scan(self) -> Generator[None, None, None]:
         """
         Close the scan.
 
         Returns:
             Generator[None, None, None]: Generator that yields a device message.
+
+        see also: :func:`open_scan`
         """
 
         yield self._device_msg(device=None, action="close_scan", parameter={})
 
     def stage(self) -> Generator[None, None, None]:
         """
         Stage all devices
 
         Returns:
             Generator[None, None, None]: Generator that yields a device message.
+
+        see also: :func:`unstage`
         """
         yield self._device_msg(device=None, action="stage", parameter={})
 
     def unstage(self) -> Generator[None, None, None]:
         """
         Unstage all devices
 
         Returns:
             Generator[None, None, None]: Generator that yields a device message.
+
+        see also: :func:`stage`
         """
         yield self._device_msg(device=None, action="unstage", parameter={})
 
     def pre_scan(self) -> Generator[None, None, None]:
         """
         Trigger pre-scan actions on all devices. Typically, pre-scan actions are called directly before the scan core starts and
         are used to perform time-critical actions.
@@ -412,41 +456,54 @@
             device=device,
             action="publish_data_as_read",
             parameter={"data": data},
             metadata=metadata,
         )
 
     def trigger(self, *, group: str, point_id: int) -> Generator[None, None, None]:
-        """Trigger a device group
+        """Trigger a device group. Note that the trigger event is not blocking and does not wait for the completion of the trigger event.
+        To wait for the completion of the trigger event, use the :func:`wait` command, specifying the wait_type as "trigger".
 
         Args:
             group (str): Device group that should receive the trigger.
             point_id (int): point_id that should be attached to this trigger event.
 
         Returns:
             Generator[None, None, None]: Generator that yields a device message.
+
+        see also: :func:`wait`
         """
         yield self._device_msg(
             device=None,
             action="trigger",
             parameter={"group": group},
             metadata={"point_id": point_id},
         )
 
     def set(self, *, device: str, value: float, wait_group: str, metadata=None):
-        """Set the device to a specific value.
+        """Set the device to a specific value. This is similar to the direct set command
+        in the command-line interface. The wait_group can be used to wait for the completion of this event.
+        For a set operation, this simply means that the device has acknowledged the set command and does not
+        necessarily mean that the device has reached the target value.
 
         Args:
             device (str): Device name
             value (float): Target value.
             wait_group (str): wait group for this event.
 
         Returns:
             Generator[None, None, None]: Generator that yields a device message.
 
+        .. warning::
+
+            Do not use this command to kickoff a long running operation. Use :func:`kickoff` instead or, if the
+            device does not support the kickoff command, use :func:`set_with_response` instead.
+
+        see also: :func:`wait`, :func:`set_and_wait`, :func:`set_with_response`
+
         """
         yield self._device_msg(
             device=device,
             action="set",
             parameter={"value": value, "wait_group": wait_group},
             metadata=metadata,
         )
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_worker.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,27 +62,31 @@
                     for dev in instr.content["parameter"].get("scan_motors")
                 ]
                 self.readout_priority = instr.content["parameter"].get("readout_priority", {})
             self.scan_type = instr.content["parameter"].get("scan_type")
 
         if not instr.metadata.get("scan_def_id"):
             self.max_point_id = 0
-        num_points = self.max_point_id + instr.content["parameter"]["num_points"]
+        instr_num_points = instr.content["parameter"].get("num_points", 0)
+        if instr_num_points is None:
+            instr_num_points = 0
+        num_points = self.max_point_id + instr_num_points
         if self.max_point_id:
             num_points += 1
 
         active_rb = self.current_instruction_queue_item.active_request_block
 
         self._initialize_scan_info(active_rb, instr, num_points)
 
         # only append the scan_progress if the scan is not using device_progress
-        if not self.scan_report_instructions or not self.scan_report_instructions[-1].get(
-            "device_progress"
-        ):
-            self.scan_report_instructions.append({"scan_progress": num_points})
+        if active_rb.scan.use_scan_progress_report:
+            if not self.scan_report_instructions or not self.scan_report_instructions[-1].get(
+                "device_progress"
+            ):
+                self.scan_report_instructions.append({"scan_progress": num_points})
         self.current_instruction_queue_item.parent.queue_manager.send_queue_status()
 
         self._send_scan_status("open")
 
     def close_scan(self, instr: messages.DeviceInstructionMessage, max_point_id: int) -> None:
         """
         Close a scan and emit a scan status message.
@@ -761,15 +765,15 @@
                     self._instruction_step(instr)
             except Exception as exc_return_to_start:
                 # if the return_to_start fails, raise the original exception
                 content = traceback.format_exc()
                 logger.error(content)
                 self.connector.raise_alarm(
                     severity=Alarms.MAJOR,
-                    source="ScanWorker",
+                    source={"ScanWorker": "_process_instructions"},
                     msg=content,
                     alarm_type=exc_return_to_start.__class__.__name__,
                     metadata={},
                 )
                 raise ScanAbortion from exc
             raise ScanAbortion from exc
         except Exception as exc:
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scans.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scans.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import ast
 import enum
 import threading
 import time
+import uuid
 from abc import ABC, abstractmethod
 from typing import Any, Literal
 
 import numpy as np
 
+from bec_lib.device import DeviceBase
 from bec_lib.devicemanager import DeviceManagerBase
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.logger import bec_logger
 
 from .errors import LimitError, ScanAbortion
 from .path_optimization import PathOptimizerMixin
 from .scan_stubs import ScanStubs
@@ -176,18 +178,19 @@
 
 class RequestBase(ABC):
     """
     Base class for all scan requests.
     """
 
     scan_name = ""
-    arg_input = {"device": ScanArgType.DEVICE}
-    arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
+    arg_input = {}
+    arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
     required_kwargs = []
     return_to_start_after_abort = False
+    use_scan_progress_report = False
 
     def __init__(
         self,
         *args,
         device_manager: DeviceManagerBase = None,
         monitored: list = None,
         parameter: dict = None,
@@ -325,18 +328,17 @@
             - max: maximum number of bundles
         required_kwargs (list): list of required kwargs
         return_to_start_after_abort (bool): if True, the scan will return to the start position after an abort
     """
 
     scan_name = ""
     scan_type = "step"
-    arg_input = {"device": ScanArgType.DEVICE}
-    arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": None}
     required_kwargs = ["required"]
     return_to_start_after_abort = True
+    use_scan_progress_report = True
 
     # perform pre-move action before the pre_scan trigger is sent
     pre_move = True
 
     def __init__(
         self,
         *args,
@@ -372,15 +374,15 @@
         self.burst_at_each_point = burst_at_each_point
         self.frames_per_trigger = frames_per_trigger
         self.optim_trajectory = optim_trajectory
         self.burst_index = 0
 
         self.start_pos = np.repeat(0, len(self.scan_motors)).tolist()
         self.positions = []
-        self.num_pos = None
+        self.num_pos = 0
 
         if self.scan_name == "":
             raise ValueError("scan_name cannot be empty")
 
         if acquisition_config is None or "default" not in acquisition_config:
             self.acquisition_config = {
                 "default": {"exp_time": self.exp_time, "readout_time": self.readout_time}
@@ -401,15 +403,14 @@
     def read_scan_motors(self):
         """read the scan motors"""
         yield from self.stubs.read_and_wait(device=self.scan_motors, wait_group="scan_motor")
 
     @abstractmethod
     def _calculate_positions(self) -> None:
         """Calculate the positions"""
-        pass
 
     def _optimize_trajectory(self):
         if not self.optim_trajectory:
             return
         if self.optim_trajectory == "corridor":
             self.positions = self.optimize_corridor(self.positions)
             return
@@ -622,42 +623,41 @@
 
 class ScanStub(RequestBase):
     pass
 
 
 class OpenScanDef(ScanStub):
     scan_name = "open_scan_def"
-    arg_input = {}
-    arg_bundle_size = {"bundle": len(arg_input), "min": 0, "max": 0}
 
     def run(self):
         yield from self.stubs.open_scan_def()
 
 
 class CloseScanDef(ScanStub):
     scan_name = "close_scan_def"
-    arg_input = {}
-    arg_bundle_size = {"bundle": len(arg_input), "min": 0, "max": 0}
 
     def run(self):
         yield from self.stubs.close_scan_def()
 
 
 class CloseScanGroup(ScanStub):
     scan_name = "close_scan_group"
-    arg_input = {}
-    arg_bundle_size = {"bundle": len(arg_input), "min": 0, "max": 0}
 
     def run(self):
         yield from self.stubs.close_scan_group()
 
 
 class DeviceRPC(ScanStub):
     scan_name = "device_rpc"
-    arg_input = [ScanArgType.DEVICE, ScanArgType.STR, ScanArgType.LIST, ScanArgType.DICT]
+    arg_input = {
+        "device": ScanArgType.DEVICE,
+        "func": ScanArgType.STR,
+        "args": ScanArgType.LIST,
+        "kwargs": ScanArgType.DICT,
+    }
     arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
 
     def _get_scan_motors(self):
         pass
 
     def run(self):
         # different to calling self.device_rpc, this procedure will not wait for a reply and therefore not check any errors.
@@ -816,24 +816,23 @@
         else:
             self.positions = np.vstack(tuple(self.axis)).T
 
 
 class FermatSpiralScan(ScanBase):
     scan_name = "fermat_scan"
     required_kwargs = ["step", "relative"]
-    arg_input = {
-        "device": ScanArgType.DEVICE,
-        "start": ScanArgType.FLOAT,
-        "stop": ScanArgType.FLOAT,
-    }
-    arg_bundle_size = {"bundle": len(arg_input), "min": 2, "max": 2}
 
     def __init__(
         self,
-        *args,
+        motor1: DeviceBase,
+        start_motor1: float,
+        stop_motor1: float,
+        motor2: DeviceBase,
+        start_motor2: float,
+        stop_motor2: float,
         step: float = 0.1,
         exp_time: float = 0,
         settling_time: float = 0,
         relative: bool = False,
         burst_at_each_point: int = 1,
         spiral_type: float = 0,
         optim_trajectory: Literal["corridor", None] = None,
@@ -857,89 +856,97 @@
 
         Examples:
             >>> scans.fermat_scan(dev.motor1, -5, 5, dev.motor2, -5, 5, step=0.5, exp_time=0.1, relative=True, optim_trajectory="corridor")
 
         """
         super().__init__(**kwargs)
         self.axis = []
+        self.motor1 = motor1
+        self.motor2 = motor2
+        self.start_motor1 = start_motor1
+        self.stop_motor1 = stop_motor1
+        self.start_motor2 = start_motor2
+        self.stop_motor2 = stop_motor2
         self.step = step
         self.exp_time = exp_time
         self.settling_time = settling_time
         self.relative = relative
         self.burst_at_each_point = burst_at_each_point
         self.spiral_type = spiral_type
         self.optim_trajectory = optim_trajectory
 
     def _calculate_positions(self):
-        params = list(self.caller_args.values())
         self.positions = get_fermat_spiral_pos(
-            params[0][0],
-            params[0][1],
-            params[1][0],
-            params[1][1],
+            self.start_motor1,
+            self.stop_motor1,
+            self.start_motor2,
+            self.stop_motor2,
             step=self.step,
             spiral_type=self.spiral_type,
             center=False,
         )
 
 
 class RoundScan(ScanBase):
     scan_name = "round_scan"
     required_kwargs = ["relative"]
-    arg_input = {
-        "motor_1": ScanArgType.DEVICE,
-        "motor_2": ScanArgType.DEVICE,
-        "inner_ring": ScanArgType.FLOAT,
-        "outer_ring": ScanArgType.FLOAT,
-        "number_of_rings": ScanArgType.INT,
-        "number_of_positions_in_first_ring": ScanArgType.INT,
-    }
-    arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
 
     def __init__(
         self,
-        motor_1,
-        motor2,
+        motor_1: DeviceBase,
+        motor2: DeviceBase,
         inner_ring: float,
         outer_ring: float,
         number_of_rings: int,
         pos_in_first_ring: int,
-        *args,
         relative: bool = False,
         burst_at_each_point: int = 1,
         **kwargs,
     ):
         """
         A scan following a round shell-like pattern.
 
         Args:
-            *args: motor1, motor2, inner ring, outer ring, number of rings, number of positions in the first ring
+            motor_1 (DeviceBase): first motor
+            motor2 (DeviceBase): second motor
+            inner_ring (float): inner radius
+            outer_ring (float): outer radius
+            number_of_rings (int): number of rings
+            pos_in_first_ring (int): number of positions in the first ring
             relative (bool): if True, the motors will be moved relative to their current position. Default is False.
             burst_at_each_point (int): number of exposures at each point. Default is 1.
 
         Returns:
             ScanReport
 
         Examples:
             >>> scans.round_scan(dev.motor1, dev.motor2, 0, 25, 5, 3, exp_time=0.1, relative=True)
 
         """
         super().__init__(**kwargs)
         self.relative = relative
         self.burst_at_each_point = burst_at_each_point
         self.axis = []
+        self.motor_1 = motor_1
+        self.motor_2 = motor2
+        self.inner_ring = inner_ring
+        self.outer_ring = outer_ring
+        self.number_of_rings = number_of_rings
+        self.pos_in_first_ring = pos_in_first_ring
 
     def _get_scan_motors(self):
         caller_args = list(self.caller_args.items())[0]
         self.scan_motors = [caller_args[0], caller_args[1][0]]
 
     def _calculate_positions(self):
-        params = list(self.caller_args.values())[0]
         self.positions = get_round_scan_positions(
-            r_in=params[1], r_out=params[2], nr=params[3], nth=params[4]
+            r_in=self.inner_ring,
+            r_out=self.outer_ring,
+            nr=self.number_of_rings,
+            nth=self.pos_in_first_ring,
         )
 
 
 class ContLineScan(ScanBase):
     scan_name = "cont_line_scan"
     required_kwargs = ["steps", "relative"]
     arg_input = {
@@ -957,15 +964,16 @@
         steps: int = 10,
         relative: bool = False,
         offset: float = 100,
         burst_at_each_point: int = 1,
         **kwargs,
     ):
         """
-        A line scan for one or more motors.
+        A continuous line scan. Use this scan if you want to move a motor continuously from start to stop position whilst
+        acquiring data at predefined positions. The scan will abort if the motor moves too fast and a point is skipped.
 
         Args:
             *args (Device, float, float): pairs of device / start position / end position
             exp_time (float): exposure time in seconds. Default is 0.
             steps (int): number of steps. Default is 10.
             relative (bool): if True, the motors will be moved relative to their current position. Default is False.
             burst_at_each_point (int): number of exposures at each point. Default is 1.
@@ -988,15 +996,15 @@
 
     def _calculate_positions(self) -> None:
         for _, val in self.caller_args.items():
             ax_pos = np.linspace(val[0], val[1], self.steps)
             self.axis.append(ax_pos)
         self.positions = np.array(list(zip(*self.axis)))
 
-    def _at_each_point(self):
+    def _at_each_point(self, _pos=None):
         yield from self.stubs.trigger(group="trigger", point_id=self.point_id)
         yield from self.stubs.read(group="primary", wait_group="primary", point_id=self.point_id)
         self.point_id += 1
 
     def scan_core(self):
         yield from self._move_scan_motors_and_wait(self.positions[0] - self.offset)
         # send the slow motor on its way
@@ -1016,50 +1024,142 @@
                 logger.debug(f"reading point {self.point_id}")
                 yield from self._at_each_point()
                 continue
             if cont_motor_positions > self.positions[self.point_id][0]:
                 raise ScanAbortion(f"Skipped point {self.point_id + 1}")
 
 
+class ContLineFlyScan(AsyncFlyScanBase):
+    scan_name = "cont_line_fly_scan"
+    required_kwargs = []
+    use_scan_progress_report = False
+
+    def __init__(
+        self,
+        motor: DeviceBase,
+        start: float,
+        stop: float,
+        exp_time: float = 0,
+        relative: bool = False,
+        **kwargs,
+    ):
+        """
+        A continuous line fly scan. Use this scan if you want to move a motor continuously from start to stop position whilst
+        acquiring data as fast as possible (respecting the exposure time). The scan will stop automatically when the motor
+        reaches the end position.
+
+        Args:
+            motor (DeviceBase): motor to move continuously from start to stop position
+            start (float): start position
+            stop (float): stop position
+            exp_time (float): exposure time in seconds. Default is 0.
+            relative (bool): if True, the motor will be moved relative to its current position. Default is False.
+
+        Returns:
+            ScanReport
+
+        Examples:
+            >>> scans.cont_line_fly_scan(dev.sam_rot, 0, 180, exp_time=0.1)
+
+        """
+        super().__init__(**kwargs)
+        self.motor = motor
+        self.start = start
+        self.stop = stop
+        self.exp_time = exp_time
+        self.relative = relative
+        self.device_move_request_id = str(uuid.uuid4())
+
+    def prepare_positions(self):
+        self.positions = np.array([[self.start], [self.stop]])
+        self.num_pos = None
+        yield from self._set_position_offset()
+
+    def scan_report_instructions(self):
+        yield from self.stubs.scan_report_instruction(
+            {
+                "readback": {
+                    "RID": self.device_move_request_id,
+                    "devices": [self.motor],
+                    "start": [self.start],
+                    "end": [self.stop],
+                }
+            }
+        )
+
+    def scan_core(self):
+        # move the motor to the start position
+        yield from self.stubs.set_and_wait(device=[self.motor], positions=self.positions[0])
+
+        # start the flyer
+        flyer_request = yield from self.stubs.set_with_response(
+            device=self.motor, value=self.positions[1][0], request_id=self.device_move_request_id
+        )
+
+        while True:
+            yield from self.stubs.trigger(group="trigger", point_id=self.point_id)
+            yield from self.stubs.read_and_wait(
+                group="primary", wait_group="readout_primary", point_id=self.point_id
+            )
+            yield from self.stubs.wait(
+                wait_type="trigger", group="trigger", wait_time=self.exp_time
+            )
+            if self.stubs.request_is_completed(flyer_request):
+                break
+            self.point_id += 1
+
+    def finalize(self):
+        yield from super().finalize()
+        self.num_pos = self.point_id + 1
+
+
 class RoundScanFlySim(SyncFlyScanBase):
     scan_name = "round_scan_fly"
     scan_type = "fly"
     pre_move = False
     required_kwargs = ["relative"]
-    arg_input = {
-        "flyer": ScanArgType.DEVICE,
-        "inner_ring": ScanArgType.FLOAT,
-        "outer_ring": ScanArgType.FLOAT,
-        "number_of_rings": ScanArgType.INT,
-        "number_of_positions_in_first_ring": ScanArgType.INT,
-    }
-    arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
 
-    def __init__(self, *args, **kwargs):
+    def __init__(
+        self,
+        flyer: DeviceBase,
+        inner_ring: float,
+        outer_ring: float,
+        number_of_rings: int,
+        number_pos: int,
+        **kwargs,
+    ):
         """
         A fly scan following a round shell-like pattern.
 
         Args:
-            *args: motor1, motor2, inner ring, outer ring, number of rings, number of positions in the first ring
-            relative: Start from an absolute or relative position
-            burst: number of acquisition per point
+            flyer (DeviceBase): flyer device
+            inner_ring (float): inner radius
+            outer_ring (float): outer radius
+            number_of_rings (int): number of rings
+            number_pos (int): number of positions in the first ring
+            relative (bool): if True, the motors will be moved relative to their current position. Default is False.
+            burst_at_each_point (int): number of exposures at each point. Default is 1.
 
         Returns:
             ScanReport
 
         Examples:
             >>> scans.round_scan_fly(dev.flyer_sim, 0, 50, 5, 3, exp_time=0.1, relative=True)
 
         """
         super().__init__(**kwargs)
         self.axis = []
+        self.flyer = flyer
+        self.inner_ring = inner_ring
+        self.outer_ring = outer_ring
+        self.number_of_rings = number_of_rings
+        self.number_pos = number_pos
 
     def _get_scan_motors(self):
         self.scan_motors = []
-        self.flyer = list(self.caller_args.keys())[0]
 
     @property
     def monitor_sync(self):
         return self.flyer
 
     def prepare_positions(self):
         self._calculate_positions()
@@ -1067,17 +1167,19 @@
         self._check_limits()
         yield None
 
     def finalize(self):
         yield
 
     def _calculate_positions(self):
-        params = list(self.caller_args.values())[0]
         self.positions = get_round_scan_positions(
-            r_in=params[0], r_out=params[1], nr=params[2], nth=params[3]
+            r_in=self.inner_ring,
+            r_out=self.outer_ring,
+            nr=self.number_of_rings,
+            nth=self.number_pos,
         )
 
     def scan_core(self):
         yield from self.stubs.kickoff(
             device=self.flyer,
             parameter={
                 "num_pos": self.num_pos,
@@ -1100,37 +1202,36 @@
             time.sleep(1)
             logger.debug("reading monitors")
 
 
 class RoundROIScan(ScanBase):
     scan_name = "round_roi_scan"
     required_kwargs = ["dr", "nth", "relative"]
-    arg_input = {
-        "motor_1": ScanArgType.DEVICE,
-        "motor_2": ScanArgType.DEVICE,
-        "width_1": ScanArgType.FLOAT,
-        "width_2": ScanArgType.FLOAT,
-    }
-    arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
 
     def __init__(
         self,
-        *args,
+        motor_1: DeviceBase,
+        width_1: float,
+        motor_2: DeviceBase,
+        width_2: float,
         dr: float = 1,
         nth: int = 5,
         exp_time: float = 0,
         relative: bool = False,
         burst_at_each_point: int = 1,
         **kwargs,
     ):
         """
         A scan following a round-roi-like pattern.
 
         Args:
-            *args: motor1, width for motor1, motor2, width for motor2,
+            motor_1 (DeviceBase): first motor
+            width_1 (float): width of region of interest for motor_1
+            motor_2 (DeviceBase): second motor
+            width_2 (float): width of region of interest for motor_2
             dr (float): shell width. Default is 1.
             nth (int): number of points in the first shell. Default is 5.
             exp_time (float): exposure time in seconds. Default is 0.
             relative (bool): Start from an absolute or relative position. Default is False.
             burst_at_each_point (int): number of acquisition per point. Default is 1.
 
         Returns:
@@ -1138,24 +1239,27 @@
 
         Examples:
             >>> scans.round_roi_scan(dev.motor1, 20, dev.motor2, 20, dr=2, nth=3, exp_time=0.1, relative=True)
 
         """
         super().__init__(**kwargs)
         self.axis = []
+        self.motor_1 = motor_1
+        self.motor_2 = motor_2
+        self.width_1 = width_1
+        self.width_2 = width_2
         self.dr = dr
         self.nth = nth
         self.exp_time = exp_time
         self.relative = relative
         self.burst_at_each_point = burst_at_each_point
 
     def _calculate_positions(self) -> None:
-        params = list(self.caller_args.values())
         self.positions = get_round_roi_scan_positions(
-            lx=params[0][0], ly=params[1][0], dr=self.dr, nth=self.nth
+            lx=self.width_1, ly=self.width_2, dr=self.dr, nth=self.nth
         )
 
 
 class ListScan(ScanBase):
     scan_name = "list_scan"
     required_kwargs = ["relative"]
     arg_input = {"device": ScanArgType.DEVICE, "positions": ScanArgType.LIST}
@@ -1186,16 +1290,14 @@
     def _calculate_positions(self):
         self.positions = np.vstack(tuple(self.caller_args.values())).T.tolist()
 
 
 class TimeScan(ScanBase):
     scan_name = "time_scan"
     required_kwargs = ["points", "interval"]
-    arg_input = {}
-    arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
 
     def __init__(
         self,
         points: int,
         interval: float,
         exp_time: float = 0,
         burst_at_each_point: int = 1,
@@ -1252,23 +1354,19 @@
         for ind in range(self.num_pos):
             yield from self._at_each_point(ind)
 
 
 class MonitorScan(ScanBase):
     scan_name = "monitor_scan"
     required_kwargs = ["relative"]
-    arg_input = {
-        "device": ScanArgType.DEVICE,
-        "start": ScanArgType.FLOAT,
-        "stop": ScanArgType.FLOAT,
-    }
-    arg_bundle_size = {"bundle": len(arg_input), "min": 1, "max": 1}
     scan_type = "fly"
 
-    def __init__(self, device, start: float, stop: float, *args, relative: bool = False, **kwargs):
+    def __init__(
+        self, device: DeviceBase, start: float, stop: float, relative: bool = False, **kwargs
+    ):
         """
         Readout all primary devices at each update of the monitored device.
 
         Args:
             device (Device): monitored device
             start (float): start position of the monitored device
             stop (float): stop position of the monitored device
@@ -1292,15 +1390,15 @@
         self.flyer = self.device
 
     @property
     def monitor_sync(self):
         return self.flyer
 
     def _calculate_positions(self) -> None:
-        self.positions = np.vstack(tuple(self.caller_args.values())).T.tolist()
+        self.positions = np.array([[self.start], [self.stop]])
 
     def prepare_positions(self):
         self._calculate_positions()
         self.num_pos = 0
         yield from self._set_position_offset()
         self._check_limits()
 
@@ -1343,16 +1441,14 @@
             self.point_id += 1
             self.num_pos += 1
 
 
 class Acquire(ScanBase):
     scan_name = "acquire"
     required_kwargs = []
-    arg_input = {}
-    arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
 
     def __init__(self, *args, exp_time: float = 0, burst_at_each_point: int = 1, **kwargs):
         """
         A simple acquisition at the current position.
 
         Args:
             burst: number of acquisition per point
@@ -1546,16 +1642,14 @@
         yield from self.open_scan()
         yield from self._at_each_point()
         yield from self.close_scan()
 
 
 class CloseInteractiveScan(ScanComponent):
     scan_name = "close_interactive_scan"
-    arg_input = {}
-    arg_bundle_size = {"bundle": len(arg_input), "min": None, "max": None}
 
     def __init__(self, *args, **kwargs):
         """
         An interactive scan for one or more motors.
 
         Args:
             *args: devices
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/cli/launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scan_server/tests/utils.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scan_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/repeated_timer.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scihub.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/cli/launch.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scibec/config_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/bec_server/scihub/scilog/scilog.py` & `ophyd_devices-1.3.0/bec/bec_server/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_bec_server_utils/test_main.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/conftest.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_config_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_serializer.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_server.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_file_writer/test_file_writer.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_file_writer/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/conftest.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_emitter.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_path_optimization.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_guard.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_stubs.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,7 +118,25 @@
     if raised_error:
         with pytest.raises(DeviceMessageError):
             with mock.patch.object(stubs.connector, "get", return_value=msg):
                 assert stubs.get_device_progress(device="samx", RID="rid") == ret_value
         return
     with mock.patch.object(stubs.connector, "get", return_value=msg):
         assert stubs.get_device_progress(device="samx", RID="rid") == ret_value
+
+
+def test_set_with_response(stubs):
+    out = stubs.set_with_response(device="samx", value=5, request_id="rid")
+    assert list(out) == [
+        messages.DeviceInstructionMessage(
+            metadata={"response": True, "RID": "rid"},
+            device="samx",
+            action="set",
+            parameter={"value": 5, "wait_group": "set"},
+        )
+    ]
+
+
+def test_request_is_completed(stubs):
+    with mock.patch.object(stubs.connector, "lrange", side_effect=[[], ["msg"]]):
+        assert stubs.request_is_completed("rid") is False
+        assert stubs.request_is_completed("rid") is True
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scan_worker.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scan_server/test_scans.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scan_server/test_scans.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from bec_server.device_server.tests.utils import DMMock
 from bec_server.scan_server.errors import ScanAbortion
 from bec_server.scan_server.scan_plugins.otf_scan import OTFScan
 from bec_server.scan_server.scans import (
     Acquire,
     AddInteractiveScanPoint,
     CloseInteractiveScan,
+    ContLineFlyScan,
     ContLineScan,
     DeviceRPC,
     FermatSpiralScan,
     LineScan,
     ListScan,
     MonitorScan,
     Move,
@@ -1045,16 +1046,18 @@
     device_manager.add_device("samx")
     macros = inspect.getsource(pre_scan_macro).encode()
     scan_msg = messages.ScanQueueMessage(
         scan_type="fermat_scan",
         parameter={"args": {"samx": (-5, 5), "samy": (-5, 5)}, "kwargs": {"step": 3}},
         queue="primary",
     )
+    args = unpack_scan_args(scan_msg.content.get("parameter", {}).get("args", []))
+    kwargs = scan_msg.content.get("parameter", {}).get("kwargs", {})
     request = FermatSpiralScan(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        *args, device_manager=device_manager, parameter=scan_msg.content["parameter"], **kwargs
     )
     with mock.patch.object(
         request.device_manager.connector,
         "lrange",
         new_callable=mock.PropertyMock,
         return_value=[messages.VariableMessage(value=macros)],
     ) as macros_mock:
@@ -1082,14 +1085,15 @@
     positions = get_round_roi_scan_positions(*in_args)
     assert np.isclose(positions, reference_positions).all()
 
 
 def test_round_roi_scan():
     device_manager = DMMock()
     device_manager.add_device("samx")
+    device_manager.add_device("samy")
     scan_msg = messages.ScanQueueMessage(
         scan_type="round_roi_scan",
         parameter={
             "args": {"samx": (10,), "samy": (10,)},
             "kwargs": {"dr": 2, "nth": 4, "exp_time": 2, "relative": True},
         },
         queue="primary",
@@ -1180,30 +1184,36 @@
     device_manager.add_device("samx")
     macros = [inspect.getsource(pre_scan_macro).encode()]
     scan_msg = messages.ScanQueueMessage(
         scan_type="fermat_scan",
         parameter={"args": {"samx": (-5, 5), "samy": (-5, 5)}, "kwargs": {"step": 3}},
         queue="primary",
     )
+    args = unpack_scan_args(scan_msg.content.get("parameter", {}).get("args", []))
+    kwargs = scan_msg.content.get("parameter", {}).get("kwargs", {})
     request = FermatSpiralScan(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        *args, device_manager=device_manager, parameter=scan_msg.content["parameter"], **kwargs
     )
     assert request._get_func_name_from_macro(macros[0].decode().strip()) == "pre_scan_macro"
 
 
 def test_scan_report_devices():
     device_manager = DMMock()
     device_manager.add_device("samx")
+    device_manager.add_device("samy")
     scan_msg = messages.ScanQueueMessage(
         scan_type="fermat_scan",
         parameter={"args": {"samx": (-5, 5), "samy": (-5, 5)}, "kwargs": {"step": 3}},
         queue="primary",
     )
+    args = unpack_scan_args(scan_msg.content.get("parameter", {}).get("args", []))
+    kwargs = scan_msg.content.get("parameter", {}).get("kwargs", {})
+
     request = FermatSpiralScan(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        *args, device_manager=device_manager, parameter=scan_msg.content["parameter"], **kwargs
     )
     assert set(request.scan_report_devices) == set(["samx", "samy"])
 
     request.scan_report_devices = ["samx", "samy", "samz"]
     assert request.scan_report_devices == ["samx", "samy", "samz"]
 
 
@@ -1313,47 +1323,57 @@
         )
     assert exc_info.value.args[0] == "scan_name cannot be empty"
 
 
 def test_scan_base_set_position_offset():
     device_manager = DMMock()
     device_manager.add_device("samx")
+    device_manager.add_device("samy")
 
     scan_msg = messages.ScanQueueMessage(
         scan_type="fermat_scan",
-        parameter={"args": {"samx": (-5, 5), "samy": (-5, 5)}, "kwargs": {"step": 3}},
+        parameter={
+            "args": {"samx": (-5, 5), "samy": (-5, 5)},
+            "kwargs": {"step": 3, "relative": False},
+        },
         queue="primary",
     )
+
+    args = unpack_scan_args(scan_msg.content.get("parameter", {}).get("args", []))
+    kwargs = scan_msg.content.get("parameter", {}).get("kwargs", {})
     request = FermatSpiralScan(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        *args, device_manager=device_manager, parameter=scan_msg.content["parameter"], **kwargs
     )
 
     assert request.positions == []
     request._set_position_offset()
     assert request.positions == []
 
-    request.relative == True
+    assert request.relative is False
     request._set_position_offset()
 
-    start_pos_ref = [0, 0]
-    request.positions += start_pos_ref
-    assert request.positions == [0, 0]
-    assert request.start_pos == start_pos_ref
+    assert request.start_pos == [0, 0]
 
 
 def test_round_scan_fly_sim_get_scan_motors():
     device_manager = DMMock()
     device_manager.add_device("flyer_sim")
     scan_msg = messages.ScanQueueMessage(
         scan_type="round_scan_fly",
         parameter={"args": {"flyer_sim": (0, 50, 5, 3)}, "kwargs": {"realtive": True}},
         queue="primary",
     )
     request = RoundScanFlySim(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        flyer="flyer_sim",
+        inner_ring=0,
+        outer_ring=50,
+        number_of_rings=5,
+        number_pos=3,
+        device_manager=device_manager,
+        parameter=scan_msg.content["parameter"],
     )
 
     request._get_scan_motors()
     assert request.scan_motors == []
     assert request.flyer == list(scan_msg.content["parameter"]["args"].keys())[0]
 
 
@@ -1362,15 +1382,21 @@
     device_manager.add_device("flyer_sim")
     scan_msg = messages.ScanQueueMessage(
         scan_type="round_scan_fly",
         parameter={"args": {"flyer_sim": (0, 50, 5, 3)}, "kwargs": {"realtive": True}},
         queue="primary",
     )
     request = RoundScanFlySim(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        flyer="flyer_sim",
+        inner_ring=0,
+        outer_ring=50,
+        number_of_rings=5,
+        number_pos=3,
+        device_manager=device_manager,
+        parameter=scan_msg.content["parameter"],
     )
     request._calculate_positions = mock.MagicMock()
     request._check_limits = mock.MagicMock()
     pos = [1, 2, 3, 4]
     request.positions = pos
 
     next(request.prepare_positions())
@@ -1388,15 +1414,21 @@
     device_manager.add_device("flyer_sim")
     scan_msg = messages.ScanQueueMessage(
         scan_type="round_scan_fly",
         parameter={"args": {"flyer_sim": in_args}, "kwargs": {"realtive": True}},
         queue="primary",
     )
     request = RoundScanFlySim(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        flyer="flyer_sim",
+        inner_ring=in_args[0],
+        outer_ring=in_args[1],
+        number_of_rings=in_args[2],
+        number_pos=in_args[3],
+        device_manager=device_manager,
+        parameter=scan_msg.content["parameter"],
     )
 
     request._calculate_positions()
     assert np.isclose(request.positions, reference_positions).all()
 
 
 @pytest.mark.parametrize(
@@ -1407,24 +1439,30 @@
     device_manager.add_device("flyer_sim")
     scan_msg = messages.ScanQueueMessage(
         scan_type="round_scan_fly",
         parameter={"args": {"flyer_sim": in_args}, "kwargs": {"realtive": True}},
         queue="primary",
     )
     request = RoundScanFlySim(
-        device_manager=device_manager, parameter=scan_msg.content["parameter"]
+        flyer="flyer_sim",
+        inner_ring=in_args[0],
+        outer_ring=in_args[1],
+        number_of_rings=in_args[2],
+        number_pos=in_args[3],
+        device_manager=device_manager,
+        parameter=scan_msg.content["parameter"],
     )
     request.positions = np.array(reference_positions)
 
     ret = next(request.scan_core())
     assert ret == messages.DeviceInstructionMessage(
         device="flyer_sim",
         action="kickoff",
         parameter={
-            "configure": {"num_pos": None, "positions": reference_positions, "exp_time": 0},
+            "configure": {"num_pos": 0, "positions": reference_positions, "exp_time": 0},
             "wait_group": "kickoff",
         },
         metadata={"readout_priority": "monitored", "DIID": 0},
     )
 
 
 @pytest.mark.parametrize(
@@ -2045,15 +2083,15 @@
                 "scan_motors": ["samx"],
                 "readout_priority": {
                     "monitored": ["samx"],
                     "baseline": [],
                     "on_request": [],
                     "async": [],
                 },
-                "num_points": None,
+                "num_points": 0,
                 "positions": [],
                 "scan_name": "open_interactive_scan",
                 "scan_type": "step",
             },
             metadata={"readout_priority": "monitored", "DIID": 3},
         ),
         messages.DeviceInstructionMessage(
@@ -2095,15 +2133,15 @@
                 "scan_motors": ["samx"],
                 "readout_priority": {
                     "monitored": ["samx"],
                     "baseline": [],
                     "on_request": [],
                     "async": [],
                 },
-                "num_points": None,
+                "num_points": 0,
                 "positions": [],
                 "scan_name": "interactive_scan_trigger",
                 "scan_type": "step",
             },
             metadata={"readout_priority": "monitored", "DIID": 0},
         ),
         messages.DeviceInstructionMessage(
@@ -2226,7 +2264,171 @@
         **scan_msg.content["parameter"]["kwargs"],
     )
 
     with mock.patch.object(request, "_check_limits") as check_limits:
         with mock.patch.object(request, "_set_position_offset") as position_offset:
             ref = list(request.run())
             assert len(ref) == 88
+
+
+def test_ContLineFlyScan():
+    device_manager = DMMock()
+    device_manager.add_device("samx")
+    request = ContLineFlyScan(
+        motor="samx", start=0, stop=5, relative=False, device_manager=device_manager
+    )
+    with mock.patch.object(request.stubs, "request_is_completed") as req_completed:
+        req_completed.side_effect = [False, True]
+        ref_list = list(request.run())
+        assert len(req_completed.mock_calls) == 2
+    ref_list[1].parameter["readback"]["RID"] = "ddaad496-6178-4f6a-8c2e-0c9d416e5d9c"
+    for item in ref_list:
+        if hasattr(item, "metadata") and "RID" in item.metadata:
+            item.metadata["RID"] = "ddaad496-6178-4f6a-8c2e-0c9d416e5d9c"
+
+    assert ref_list == [
+        None,
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 0},
+            device=None,
+            action="scan_report_instruction",
+            parameter={
+                "readback": {
+                    "RID": "ddaad496-6178-4f6a-8c2e-0c9d416e5d9c",
+                    "devices": ["samx"],
+                    "start": [0],
+                    "end": [5],
+                }
+            },
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 1},
+            device=None,
+            action="open_scan",
+            parameter={
+                "scan_motors": [],
+                "readout_priority": {
+                    "monitored": [],
+                    "baseline": [],
+                    "on_request": [],
+                    "async": [],
+                },
+                "num_points": None,
+                "positions": [[0], [5]],
+                "scan_name": "cont_line_fly_scan",
+                "scan_type": "fly",
+            },
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 2},
+            device=None,
+            action="stage",
+            parameter={},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "baseline", "DIID": 3},
+            device=None,
+            action="baseline_reading",
+            parameter={},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 4},
+            device=None,
+            action="pre_scan",
+            parameter={},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 5},
+            device="samx",
+            action="set",
+            parameter={"value": 0, "wait_group": "scan_motor"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 6},
+            device=["samx"],
+            action="wait",
+            parameter={"type": "move", "wait_group": "scan_motor"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={
+                "readout_priority": "monitored",
+                "DIID": 7,
+                "response": True,
+                "RID": "ddaad496-6178-4f6a-8c2e-0c9d416e5d9c",
+            },
+            device="samx",
+            action="set",
+            parameter={"value": 5, "wait_group": "set"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 8, "point_id": 0},
+            device=None,
+            action="trigger",
+            parameter={"group": "trigger"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 9, "point_id": 0},
+            device=None,
+            action="read",
+            parameter={"group": "primary", "wait_group": "readout_primary"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 10},
+            device=None,
+            action="wait",
+            parameter={"type": "read", "group": "primary", "wait_group": "readout_primary"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 11},
+            device=None,
+            action="wait",
+            parameter={"type": "trigger", "time": 0, "group": "trigger"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 12, "point_id": 1},
+            device=None,
+            action="trigger",
+            parameter={"group": "trigger"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 13, "point_id": 1},
+            device=None,
+            action="read",
+            parameter={"group": "primary", "wait_group": "readout_primary"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 14},
+            device=None,
+            action="wait",
+            parameter={"type": "read", "group": "primary", "wait_group": "readout_primary"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 15},
+            device=None,
+            action="wait",
+            parameter={"type": "trigger", "time": 0, "group": "trigger"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 16},
+            device=None,
+            action="wait",
+            parameter={"type": "read", "group": "primary", "wait_group": "readout_primary"},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 17},
+            device=None,
+            action="complete",
+            parameter={},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 18},
+            device=None,
+            action="unstage",
+            parameter={},
+        ),
+        messages.DeviceInstructionMessage(
+            metadata={"readout_priority": "monitored", "DIID": 19},
+            device=None,
+            action="close_scan",
+            parameter={},
+        ),
+    ]
```

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/conftest.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/conftest.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_repeated_timer.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scibec_connector.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scibec_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bec_server/tests/tests_scihub/test_scilog_connector.py` & `ophyd_devices-1.3.0/bec/bec_server/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/bin/install_bec_dev.sh` & `ophyd_devices-1.3.0/bec/bin/install_bec_dev.sh`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/ci/Dockerfile.run_pytest` & `ophyd_devices-1.3.0/bec/ci/Dockerfile.run_pytest`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/ci/Dockerfile.run_server` & `ophyd_devices-1.3.0/bec/ci/Dockerfile.run_server`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/ci/docker-compose.yaml` & `ophyd_devices-1.3.0/bec/ci/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/ci/semantic_release.toml` & `ophyd_devices-1.3.0/bec/ci/semantic_release.toml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/architecture/BEC.drawio` & `ophyd_devices-1.3.0/bec/docs/architecture/BEC.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/architecture/BEC_config_db.drawio` & `ophyd_devices-1.3.0/bec/docs/architecture/BEC_config_db.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/architecture/BEC_config_db.svg` & `ophyd_devices-1.3.0/bec/docs/architecture/BEC_config_db.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/architecture/bec_architecture.png` & `ophyd_devices-1.3.0/bec/docs/architecture/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/Makefile` & `ophyd_devices-1.3.0/bec/docs/source/Makefile`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/conf.py` & `ophyd_devices-1.3.0/bec/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/index.md` & `ophyd_devices-1.3.0/bec/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/make.bat` & `ophyd_devices-1.3.0/bec/docs/source/make.bat`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/_static/bec.png` & `ophyd_devices-1.3.0/bec/docs/source/_static/bec.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/_static/custom.css` & `ophyd_devices-1.3.0/bec/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/_static/gif/bec_plotter.gif` & `ophyd_devices-1.3.0/bec/docs/source/_static/gif/bec_plotter.gif`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/_templates/custom-class-template.rst` & `ophyd_devices-1.3.0/bec/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/_templates/custom-module-template.rst` & `ophyd_devices-1.3.0/bec/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/BEC_context_user_centric.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/BEC_context_user_centric.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/bec_architecture.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/bec_architecture.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/bec_device_structure.drawio` & `ophyd_devices-1.3.0/bec/docs/source/assets/bec_device_structure.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/bec_device_structure.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/bec_device_structure.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/bec_widgets_glance.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/bec_widgets_glance.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/gauss_scatter_plot.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/gauss_scatter_plot.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/index_api.svg` & `ophyd_devices-1.3.0/bec/docs/source/assets/index_api.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/index_contribute.svg` & `ophyd_devices-1.3.0/bec/docs/source/assets/index_contribute.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/index_getting_started.svg` & `ophyd_devices-1.3.0/bec/docs/source/assets/index_getting_started.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/index_user_guide.svg` & `ophyd_devices-1.3.0/bec/docs/source/assets/index_user_guide.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/precision_manufacturing_48dp.svg` & `ophyd_devices-1.3.0/bec/docs/source/assets/precision_manufacturing_48dp.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/rocket_launch_48dp.svg` & `ophyd_devices-1.3.0/bec/docs/source/assets/rocket_launch_48dp.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/simulation_context_diagram.drawio` & `ophyd_devices-1.3.0/bec/docs/source/assets/simulation_context_diagram.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/simulation_context_diagram.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/simulation_context_diagram.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/tab-complete-devices.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/tab-complete-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/timeline_48dp.svg` & `ophyd_devices-1.3.0/bec/docs/source/assets/timeline_48dp.svg`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/vscode_debug_button.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/vscode_debug_button.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/vscode_with_annotations.drawio` & `ophyd_devices-1.3.0/bec/docs/source/assets/vscode_with_annotations.drawio`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/vscode_with_annotations.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/vscode_with_annotations.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/assets/wm-devices.png` & `ophyd_devices-1.3.0/bec/docs/source/assets/wm-devices.png`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/developer.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/developer.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/glossary.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/glossary.md`

 * *Files 21% similar despite different names*

```diff
@@ -11,10 +11,16 @@
     The ``dataset_number`` is an integer that is assigned to a dataset by the scan server. It is used to group scans into larger, logical units. The ``dataset_number`` is typically reset to 1 for each new experiment.
 request_id
     The ``request_id`` is an identifier for a request to the scan server. As of now, it is a uuid4 string that is generated by the bec_lib during the preparation of a new request. A scan can comprise instructions from multiple requests.
 queue_id
     The ``queue_id`` is an identifier for an element in a queue. Each queue element can contain multiple scans and thus enforce the sequential execution of those scans. The ``queue_id`` is a uuid4 string that is generated by the bec_lib during the preparation of a new queue element.
 DIID
     The ``DIID`` is the device instruction ID. It is a continuously increasing integer that is assigned to each device instruction in a scan. The ``DIID`` is used to uniquely identify each device instruction and its response in the scan. 
-
-
-```
+point_id
+    The ``point_id`` is an integer that is assigned to each point in a scan. It is used to uniquely identify each point in a scan and is used to group the data that is generated by a scan. The ``point_id`` is typically set directly during the scan definition and used by the {term}`Scan Bundler` to logically bundle the data that is generated by a scan. In synchronous fly scans, the ``point_id may`` also be set directly by the device. 
+Device Server
+    The Device Server provides a core service of BEC and handles the communication to the devices. It is the only process that actually holds the connection to the devices. Other services, like the {term}`Scan Server`, communicate with the Device Server to interact with the devices.
+Scan Server
+    The Scan Server provides a core service of BEC and handles the execution of scans. It is responsible for receiving and validating scan requests, assembling the scan instructions, queueing the scan and finally executing the scan using a Scan Worker. If necessary, the Scan Server emits DeviceInstructionMessages to the {term}`Device Server` to interact with the devices. 
+Scan Bundler
+    The Scan Bundler is a core service of BEC that is responsible for bundling the data that is generated by a scan. It subscribes to Redis channels and listens for data that is generated by the devices. The Scan Bundler then bundles the data into logical units, called scan segments, and emits them as ScanMessage back to Redis. 
+```
```

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/devices/bec_sim.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/devices/bec_sim.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/devices/device_configuration.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/devices/device_configuration.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/devices/devices.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/devices/devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/devices/external_sources.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/devices/external_sources.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/devices/ophyd.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/devices/ophyd.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/architecture.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/architecture.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/bec_plugins.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/bec_plugins.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/contributing.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/contributing.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/install_developer_env.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/install_developer_env.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/logs.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/logs.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/tests.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/tests.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/getting_started/vscode.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/getting_started/vscode.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/scans/scans.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/scans/scans.md`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,16 @@
 - [`baseline_reading`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.baseline_reading) Trigger the baseline readings. 
 - [`wait`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.wait) Wait for an event to finish. Could be a trigger, a readout or a movement. 
 - [`read`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.read) Read from a device.
 - [`trigger`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.trigger) Trigger a device.
 - [`set`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.set) Set a device to a value.
 - [`rpc`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.rpc) Send an RPC command to a device.
 - [`send_rpc_and_wait`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.send_rpc_and_wait) Send an RPC command to a device and wait for it to finish.
-
+- [`set_with_response`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.set_with_response) Set a device to a specific value and return the request ID. Use this method as an alternative to `kickoff` if the device does not support `kickoff`. 
+- [`request_is_completed`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.request_is_completed) Check if a request that was initiated with `set_with_response` is completed.
 *Scan operations*
 - [`open_scan`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.open_scan) Open a scan.
 - [`close_scan`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.close_scan) Close a scan. 
 - [`publish_data_as_read`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.publish_data_as_read) Publish data as read.
 - [`open_scan_def`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.open_scan_def) Open a scan definition. 
 - [`close_scan_def`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.close_scan_def) Close a scan definition. 
 - [`scan_report_instruction`](/api_reference/_autosummary/bec_server.scan_server.scan_stubs.ScanStubs.rst#bec_server.scan_server.scan_stubs.ScanStubs.scan_report_instruction) Update the scan report instruction.
```

### Comparing `ophyd_devices-1.2.1/bec/docs/source/developer/user_interfaces/bec_gui.md` & `ophyd_devices-1.3.0/bec/docs/source/developer/user_interfaces/bec_gui.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/introduction/introduction.md` & `ophyd_devices-1.3.0/bec/docs/source/introduction/introduction.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/user/command_line_interface.md` & `ophyd_devices-1.3.0/bec/docs/source/user/command_line_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/user/data_access_and_plotting.md` & `ophyd_devices-1.3.0/bec/docs/source/user/data_access_and_plotting.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/user/devices.md` & `ophyd_devices-1.3.0/bec/docs/source/user/devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/user/graphical_user_interface.md` & `ophyd_devices-1.3.0/bec/docs/source/user/graphical_user_interface.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/user/installation.md` & `ophyd_devices-1.3.0/bec/docs/source/user/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/docs/source/user/user.md` & `ophyd_devices-1.3.0/bec/docs/source/user/user.md`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/bec/pytest_bec_e2e/pyproject.toml` & `ophyd_devices-1.3.0/bec/pytest_bec_e2e/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytest-bec-e2e"
-version = "2.12.5"
+version = "2.13.1"
 description = "BEC pytest plugin for end-to-end tests"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.2.1/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py` & `ophyd_devices-1.3.0/bec/pytest_bec_e2e/pytest_bec_e2e/plugin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/__init__.py` & `ophyd_devices-1.3.0/ophyd_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/ophyd_patch.py` & `ophyd_devices-1.3.0/ophyd_devices/ophyd_patch.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/configs/ophyd_devices_simulation.yaml` & `ophyd_devices-1.3.0/ophyd_devices/configs/ophyd_devices_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/configs/ophyd_simulation.yaml` & `ophyd_devices-1.3.0/ophyd_devices/configs/ophyd_simulation.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/devices/SpmBase.py` & `ophyd_devices-1.3.0/ophyd_devices/devices/SpmBase.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/devices/XbpmBase.py` & `ophyd_devices-1.3.0/ophyd_devices/devices/XbpmBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,11 @@
 import numpy as np
 from ophyd import Component, Device, EpicsSignal, EpicsSignalRO
 
 
-class XbpmCsaxsOp(Device):
-    """Python wrapper for custom XBPMs in the cSAXS optics hutch
-
-    This is  completely custom XBPM with templates directly in the
-    VME repo. Thus it needs a custom ophyd template as well...
-
-    WARN: The x and y are not updated by the IOC
-    """
-
-    sum = Component(EpicsSignalRO, "SUM", auto_monitor=True)
-    x = Component(EpicsSignalRO, "POSH", auto_monitor=True)
-    y = Component(EpicsSignalRO, "POSV", auto_monitor=True)
-    s1 = Component(EpicsSignalRO, "CHAN1", auto_monitor=True)
-    s2 = Component(EpicsSignalRO, "CHAN2", auto_monitor=True)
-    s3 = Component(EpicsSignalRO, "CHAN3", auto_monitor=True)
-    s4 = Component(EpicsSignalRO, "CHAN4", auto_monitor=True)
-
-
 class XbpmBase(Device):
     """Python wrapper for X-ray Beam Position Monitors
 
     XBPM's consist of a metal-coated diamond window that ejects
     photoelectrons from the incoming X-ray beam. These electons
     are collected and their current is measured. Effectively
     they act as four quadrant photodiodes and are used as BPMs
```

### Comparing `ophyd_devices-1.2.1/ophyd_devices/devices/epics_motor_ex.py` & `ophyd_devices-1.3.0/ophyd_devices/devices/epics_motor_ex.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/devices/sls_detector.py` & `ophyd_devices-1.3.0/ophyd_devices/devices/sls_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/devices/sls_devices.py` & `ophyd_devices-1.3.0/ophyd_devices/devices/sls_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py` & `ophyd_devices-1.3.0/ophyd_devices/interfaces/base_classes/ophyd_rotation_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py` & `ophyd_devices-1.3.0/ophyd_devices/interfaces/base_classes/psi_delay_generator_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/interfaces/base_classes/psi_detector_base.py` & `ophyd_devices-1.3.0/ophyd_devices/interfaces/base_classes/psi_detector_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 We use composition with a custom prepare class to implement BL specific logic for the detector.
 The beamlines need to inherit from the CustomDetectorMixing for their mixin classes."""
 
 import os
 import time
 
 from bec_lib import messages
-from bec_lib.device import DeviceStatus
 from bec_lib.endpoints import MessageEndpoints
 from bec_lib.file_utils import FileWriter
-from ophyd import Device
+from ophyd import Device, DeviceStatus
 from ophyd.device import Staged
 
 from ophyd_devices.utils import bec_utils
 from ophyd_devices.utils.bec_scaninfo_mixin import BecScaninfoMixin
 
 
 class DetectorInitError(Exception):
@@ -84,14 +83,21 @@
     def on_pre_scan(self) -> None:
         """
         Specify actions to be executed right before a scan starts.
 
         Only use if needed, and it is recommended to keep this function as short/fast as possible.
         """
 
+    def on_complete(self) -> None:
+        """
+        Specify actions to be executed when the scan is complete.
+
+        This can for instance be to check with the detector and backend if all data is written succsessfully.
+        """
+
     # TODO add configurable file_path instead of hardcoding self.parent.filepath
     def publish_file_location(
         self, done: bool = False, successful: bool = None, metadata: dict = {}
     ) -> None:
         """
         Publish the filepath to REDIS.
 
@@ -270,14 +276,27 @@
         self.custom_prepare.on_pre_scan()
 
     def trigger(self) -> DeviceStatus:
         """Trigger the detector, called from BEC."""
         self.custom_prepare.on_trigger()
         return super().trigger()
 
+    def complete(self) -> None:
+        """Complete the acquisition, called from BEC.
+
+        This function is called after the scan is complete, just before unstage.
+        We can check here with the data backend and detector if the acquisition successfully finished.
+
+        Actions are implemented in custom_prepare.on_complete since they are beamline specific.
+        """
+        status = DeviceStatus(self)
+        self.custom_prepare.on_complete()
+        status.set_finished()
+        return status
+
     def unstage(self) -> list[object]:
         """
         Unstage device after a scan.
 
         We first check if the scanID has changed, thus, the scan was unexpectedly interrupted but the device was not stopped.
         If that is the case, the stopped flag is set to True, which will immediately unstage the device.
```

### Comparing `ophyd_devices-1.2.1/ophyd_devices/interfaces/protocols/bec_protocols.py` & `ophyd_devices-1.3.0/ophyd_devices/interfaces/protocols/bec_protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/sim.py` & `ophyd_devices-1.3.0/ophyd_devices/sim/sim.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/sim_data.py` & `ophyd_devices-1.3.0/ophyd_devices/sim/sim_data.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/sim_frameworks.py` & `ophyd_devices-1.3.0/ophyd_devices/sim/sim_frameworks.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/sim_signals.py` & `ophyd_devices-1.3.0/ophyd_devices/sim/sim_signals.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/sim_test_devices.py` & `ophyd_devices-1.3.0/ophyd_devices/sim/sim_test_devices.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/sim_utils.py` & `ophyd_devices-1.3.0/ophyd_devices/sim/sim_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/sim_xtreme.py` & `ophyd_devices-1.3.0/ophyd_devices/sim/sim_xtreme.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1634_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1637_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt` & `ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1640_Mn_thick_30K_grazing_minus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt` & `ophyd_devices-1.3.0/ophyd_devices/sim/xmcd_loop/20230512_1643_Mn_thick_30K_grazing_plus_0000.txt`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/tests/utils.py` & `ophyd_devices-1.3.0/ophyd_devices/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/utils/bec_device_base.py` & `ophyd_devices-1.3.0/ophyd_devices/utils/bec_device_base.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/utils/bec_scaninfo_mixin.py` & `ophyd_devices-1.3.0/ophyd_devices/utils/bec_scaninfo_mixin.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/utils/controller.py` & `ophyd_devices-1.3.0/ophyd_devices/utils/controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/utils/dynamic_pseudo.py` & `ophyd_devices-1.3.0/ophyd_devices/utils/dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/utils/socket.py` & `ophyd_devices-1.3.0/ophyd_devices/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/ophyd_devices/utils/static_device_test.py` & `ophyd_devices-1.3.0/ophyd_devices/utils/static_device_test.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/tests/test_base_classes.py` & `ophyd_devices-1.3.0/tests/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/tests/test_controller.py` & `ophyd_devices-1.3.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/tests/test_dynamic_pseudo.py` & `ophyd_devices-1.3.0/tests/test_dynamic_pseudo.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/tests/test_ophyd_status_obj.py` & `ophyd_devices-1.3.0/tests/test_ophyd_status_obj.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/tests/test_socket.py` & `ophyd_devices-1.3.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/.gitignore` & `ophyd_devices-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/LICENSE` & `ophyd_devices-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_devices-1.2.1/pyproject.toml` & `ophyd_devices-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ophyd_devices"
-version = "1.2.1"
+version = "1.3.0"
 description = "Custom device implementations based on the ophyd hardware abstraction layer"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `ophyd_devices-1.2.1/PKG-INFO` & `ophyd_devices-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ophyd_devices
-Version: 1.2.1
+Version: 1.3.0
 Summary: Custom device implementations based on the ophyd hardware abstraction layer
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/ophyd_devices/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/ophyd_devices
 Project-URL: documentation, https://bec.readthedocs.org
 Project-URL: changelog, https://gitlab.psi.ch/bec/ophyd_devices/blob/main/CHANGELOG.md
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

