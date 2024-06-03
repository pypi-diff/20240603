# Comparing `tmp/pytest_splunk_addon-5.3.0b2.tar.gz` & `tmp/pytest_splunk_addon-5.3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon-5.3.0b2.tar", max compression
+gzip compressed data, was "pytest_splunk_addon-5.3.0b3.tar", max compression
```

## Comparing `pytest_splunk_addon-5.3.0b2.tar` & `pytest_splunk_addon-5.3.0b3.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0    11341 2024-05-27 08:10:07.067065 pytest_splunk_addon-5.3.0b2/LICENSE
--rw-r--r--   0        0        0     2160 2024-05-27 08:11:05.815477 pytest_splunk_addon-5.3.0b2/pyproject.toml
--rw-r--r--   0        0        0     1886 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/.ignore_splunk_internal_errors
--rw-r--r--   0        0        0      751 2024-05-27 08:11:05.811477 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/__init__.py
--rw-r--r--   0        0        0     5364 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/docker_class.py
--rw-r--r--   0        0        0     8543 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/plugin.py
--rw-r--r--   0        0        0    34181 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/splunk.py
--rw-r--r--   0        0        0      579 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
--rw-r--r--   0        0        0    46781 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
--rw-r--r--   0        0        0     1220 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/__init__.py
--rw-r--r--   0        0        0     2791 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_basic.py
--rw-r--r--   0        0        0     3312 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
--rw-r--r--   0        0        0     2082 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
--rw-r--r--   0        0        0     3136 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/fields.py
--rw-r--r--   0        0        0    13284 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
--rw-r--r--   0        0        0     2760 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
--rw-r--r--   0        0        0     2447 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
--rw-r--r--   0        0        0     5391 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
--rw-r--r--   0        0        0     6168 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/app_test_generator.py
--rw-r--r--   0        0        0      754 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
--rw-r--r--   0        0        0     1130 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
--rw-r--r--   0        0        0     9586 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
--rw-r--r--   0        0        0     2351 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
--rw-r--r--   0        0        0     2801 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
--rw-r--r--   0        0        0     2442 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
--rw-r--r--   0        0        0     3553 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
--rw-r--r--   0        0        0     3699 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
--rw-r--r--   0        0        0      970 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
--rw-r--r--   0        0        0     2024 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
--rw-r--r--   0        0        0     2386 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
--rw-r--r--   0        0        0     3937 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
--rw-r--r--   0        0        0     3267 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
--rw-r--r--   0        0        0     4226 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
--rw-r--r--   0        0        0     9218 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
--rw-r--r--   0        0        0     2965 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
--rw-r--r--   0        0        0    11204 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
--rw-r--r--   0        0        0    20768 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
--rw-r--r--   0        0        0     2390 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Alerts.json
--rw-r--r--   0        0        0     5281 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Authentication.json
--rw-r--r--   0        0        0     9626 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Certificates.json
--rw-r--r--   0        0        0     8173 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Change.json
--rw-r--r--   0        0        0     2814 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/DLP.json
--rw-r--r--   0        0        0     8598 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Email.json
--rw-r--r--   0        0        0    18855 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
--rw-r--r--   0        0        0     9890 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
--rw-r--r--   0        0        0     4255 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Malware.json
--rw-r--r--   0        0        0     8683 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
--rw-r--r--   0        0        0     5599 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
--rw-r--r--   0        0        0    18953 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
--rw-r--r--   0        0        0     3862 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Updates.json
--rw-r--r--   0        0        0     5184 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
--rw-r--r--   0        0        0     7178 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Web.json
--rw-r--r--   0        0        0      889 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
--rw-r--r--   0        0        0      862 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
--rw-r--r--   0        0        0     7339 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
--rw-r--r--   0        0        0     5002 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
--rw-r--r--   0        0        0     4418 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
--rw-r--r--   0        0        0     4995 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
--rw-r--r--   0        0        0     3615 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
--rw-r--r--   0        0        0     3015 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
--rw-r--r--   0        0        0      812 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
--rw-r--r--   0        0        0     5420 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
--rw-r--r--   0        0        0    11040 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
--rw-r--r--   0        0        0    10360 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
--rw-r--r--   0        0        0    21984 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
--rw-r--r--   0        0        0      766 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/__init__.py
--rw-r--r--   0        0        0      711 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
--rw-r--r--   0        0        0    11987 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
--rw-r--r--   0        0        0    11457 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
--rw-r--r--   0        0        0      909 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
--rw-r--r--   0        0        0     7291 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
--rw-r--r--   0        0        0    46400 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/rule.py
--rw-r--r--   0        0        0    15413 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
--rw-r--r--   0        0        0     2290 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
--rw-r--r--   0        0        0    16792 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
--rw-r--r--   0        0        0     6032 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
--rw-r--r--   0        0        0     9990 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
--rw-r--r--   0        0        0     6217 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
--rw-r--r--   0        0        0      834 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/__init__.py
--rw-r--r--   0        0        0     4634 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
--rw-r--r--   0        0        0     1627 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/log_helper.py
--rw-r--r--   0        0        0     3034 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
--rw-r--r--   0        0        0     3414 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
--rw-r--r--   0        0        0    17585 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/tools/cim_field_report.py
--rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.3.0b2/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-06-03 13:57:30.327261 pytest_splunk_addon-5.3.0b3/LICENSE
+-rw-r--r--   0        0        0     2160 2024-06-03 13:58:42.643303 pytest_splunk_addon-5.3.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1886 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/.ignore_splunk_internal_errors
+-rw-r--r--   0        0        0      751 2024-06-03 13:58:42.639303 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/__init__.py
+-rw-r--r--   0        0        0     5364 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/docker_class.py
+-rw-r--r--   0        0        0     8543 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/plugin.py
+-rw-r--r--   0        0        0    33960 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/splunk.py
+-rw-r--r--   0        0        0      579 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
+-rw-r--r--   0        0        0    46781 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
+-rw-r--r--   0        0        0     1220 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/__init__.py
+-rw-r--r--   0        0        0     2791 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_basic.py
+-rw-r--r--   0        0        0     3312 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
+-rw-r--r--   0        0        0     2082 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
+-rw-r--r--   0        0        0     3136 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/fields.py
+-rw-r--r--   0        0        0    13382 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
+-rw-r--r--   0        0        0     2760 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
+-rw-r--r--   0        0        0     2447 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
+-rw-r--r--   0        0        0     5391 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
+-rw-r--r--   0        0        0     6168 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/app_test_generator.py
+-rw-r--r--   0        0        0      754 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
+-rw-r--r--   0        0        0     1251 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
+-rw-r--r--   0        0        0     1130 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
+-rw-r--r--   0        0        0     9586 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
+-rw-r--r--   0        0        0     2351 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
+-rw-r--r--   0        0        0     2801 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
+-rw-r--r--   0        0        0     2442 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
+-rw-r--r--   0        0        0     3553 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
+-rw-r--r--   0        0        0     3699 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
+-rw-r--r--   0        0        0      970 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
+-rw-r--r--   0        0        0     2024 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
+-rw-r--r--   0        0        0     2386 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
+-rw-r--r--   0        0        0     3937 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
+-rw-r--r--   0        0        0     3267 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
+-rw-r--r--   0        0        0     4226 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
+-rw-r--r--   0        0        0     9218 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
+-rw-r--r--   0        0        0     2965 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
+-rw-r--r--   0        0        0    11204 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
+-rw-r--r--   0        0        0    20768 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
+-rw-r--r--   0        0        0     2390 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Alerts.json
+-rw-r--r--   0        0        0     5281 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Authentication.json
+-rw-r--r--   0        0        0     9626 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Certificates.json
+-rw-r--r--   0        0        0     8173 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Change.json
+-rw-r--r--   0        0        0     2814 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/DLP.json
+-rw-r--r--   0        0        0     8598 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Email.json
+-rw-r--r--   0        0        0    18855 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
+-rw-r--r--   0        0        0     5754 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
+-rw-r--r--   0        0        0     4255 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Malware.json
+-rw-r--r--   0        0        0     7633 2024-06-03 13:57:30.335261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
+-rw-r--r--   0        0        0     5599 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
+-rw-r--r--   0        0        0    14817 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
+-rw-r--r--   0        0        0     3862 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Updates.json
+-rw-r--r--   0        0        0     5184 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
+-rw-r--r--   0        0        0     7178 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Web.json
+-rw-r--r--   0        0        0      889 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
+-rw-r--r--   0        0        0      862 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
+-rw-r--r--   0        0        0     7339 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
+-rw-r--r--   0        0        0     5002 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
+-rw-r--r--   0        0        0     4418 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
+-rw-r--r--   0        0        0     4995 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
+-rw-r--r--   0        0        0     3615 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
+-rw-r--r--   0        0        0     3015 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
+-rw-r--r--   0        0        0      812 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
+-rw-r--r--   0        0        0     3305 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
+-rw-r--r--   0        0        0     5420 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
+-rw-r--r--   0        0        0    11040 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
+-rw-r--r--   0        0        0    10360 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
+-rw-r--r--   0        0        0    21984 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
+-rw-r--r--   0        0        0      766 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/__init__.py
+-rw-r--r--   0        0        0      711 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
+-rw-r--r--   0        0        0    11987 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
+-rw-r--r--   0        0        0    11457 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
+-rw-r--r--   0        0        0      909 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
+-rw-r--r--   0        0        0     7291 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
+-rw-r--r--   0        0        0    46400 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/rule.py
+-rw-r--r--   0        0        0    15413 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
+-rw-r--r--   0        0        0     2290 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
+-rw-r--r--   0        0        0    16792 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
+-rw-r--r--   0        0        0     5960 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
+-rw-r--r--   0        0        0     9990 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
+-rw-r--r--   0        0        0     6217 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
+-rw-r--r--   0        0        0      834 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/__init__.py
+-rw-r--r--   0        0        0     4634 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
+-rw-r--r--   0        0        0     1627 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/log_helper.py
+-rw-r--r--   0        0        0     3034 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
+-rw-r--r--   0        0        0     3414 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
+-rw-r--r--   0        0        0      836 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utils.py
+-rw-r--r--   0        0        0    17585 2024-06-03 13:57:30.339261 pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/tools/cim_field_report.py
+-rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.3.0b3/PKG-INFO
```

### Comparing `pytest_splunk_addon-5.3.0b2/LICENSE` & `pytest_splunk_addon-5.3.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pyproject.toml` & `pytest_splunk_addon-5.3.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "pytest-splunk-addon"
-version = "5.3.0-beta.2"
+version = "5.3.0-beta.3"
 description = "A Dynamic test tool for Splunk Apps and Add-ons"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "APACHE-2.0"
 classifiers = [
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
```

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/.ignore_splunk_internal_errors` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/.ignore_splunk_internal_errors`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # limitations under the License.
 #
 # -*- coding: utf-8 -*-
 """Top-level package for splunk-app-test-lib."""
 
 __author__ = """Splunk Inc."""
 __email__ = "addonfactory@splunk.com"
-__version__ = "5.3.0-beta.2"
+__version__ = "5.3.0-beta.3"
```

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/docker_class.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/docker_class.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/plugin.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/splunk.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/splunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from splunksplwrapper.SearchUtil import SearchUtil
 from .standard_lib.event_ingestors import IngestorHelper
 from .docker_class import Services
 from .standard_lib.CIM_Models.datamodel_definition import datamodels
 import configparser
 from filelock import FileLock
 
+from pytest_splunk_addon.standard_lib import utils
+
 RESPONSIVE_SPLUNK_TIMEOUT = 300  # seconds
 
 LOGGER = logging.getLogger("pytest-splunk-addon")
 PYTEST_XDIST_TESTRUNUID = ""
 
 
 def pytest_addoption(parser):
@@ -728,18 +730,15 @@
 
     TODO:
         For splunk_type=external, data will not be ingested as manual configurations are required.
     """
     if request.config.getoption("ingest_events").lower() in ["n", "no", "false", "f"]:
         return
     global PYTEST_XDIST_TESTRUNUID
-    if (
-        "PYTEST_XDIST_WORKER" not in os.environ
-        or os.environ.get("PYTEST_XDIST_WORKER") == "gw0"
-    ):
+    if utils.check_first_worker():
         addon_path = request.config.getoption("splunk_app")
         config_path = request.config.getoption("splunk_data_generator")
         ingest_meta_data = {
             "uf_host": uf.get("uf_host"),
             "uf_port": uf.get("uf_port"),
             "uf_username": uf.get("uf_username"),
             "uf_password": uf.get("uf_password"),
@@ -779,36 +778,30 @@
     `Splunk doc <https://docs.splunk.com/Documentation/Splunk/8.0.6/Indexer/RemovedatafromSplunk#How_to_delete>`_
 
     Args:
         splunk_search_util: Other fixture preparing connection to Splunk Search.
 
     """
     if request.config.getoption("splunk_cleanup"):
-        if (
-            "PYTEST_XDIST_WORKER" not in os.environ
-            or os.environ.get("PYTEST_XDIST_WORKER") == "gw0"
-        ):
+        if utils.check_first_worker():
             LOGGER.info("Running the old events cleanup")
             splunk_search_util.deleteEventsFromIndex()
     else:
         LOGGER.info("Events cleanup was disabled.")
 
 
 @pytest.fixture(scope="session")
 def file_system_prerequisite():
     """
     File system prerequisite before running tests.
     Creating uf_files directory to write tokenized events for uf_file_monitor input.
     """
     UF_FILE_MONTOR_DIR = "uf_files"
     monitor_dir = os.path.join(os.getcwd(), UF_FILE_MONTOR_DIR)
-    if (
-        "PYTEST_XDIST_WORKER" not in os.environ
-        or os.environ.get("PYTEST_XDIST_WORKER") == "gw0"
-    ):
+    if utils.check_first_worker():
         if os.path.exists(monitor_dir):
             shutil.rmtree(monitor_dir, ignore_errors=True)
         os.mkdir(monitor_dir)
 
 
 @pytest.fixture(scope="session")
 def splunk_dm_recommended_fields():
```

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_basic.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/fields.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import re
 from itertools import product
 
 import addonfactory_splunk_conf_parser_lib as conf_parser
 
 from .fields import convert_to_fields
 from .transforms_parser import TransformsParser
+from pytest_splunk_addon.standard_lib import utils
 
 LOGGER = logging.getLogger("pytest-splunk-addon")
 
 
 class PropsParser(object):
     """
     Parses props.conf and extracts the fields.
@@ -106,15 +107,16 @@
             "LOOKUP": self._get_lookup_fields,
         }
         for each_type in method_mapping:
             if re.match(each_type, class_name, re.IGNORECASE):
                 LOGGER.info(f"Matched method of type={each_type}")
                 return method_mapping[each_type]
         else:
-            LOGGER.warning(f"No parser available for {class_name}. Skipping...")
+            if utils.check_first_worker():
+                LOGGER.warning(f"No parser available for {class_name}. Skipping...")
 
     def _get_props_stanzas(self) -> Optional[Generator]:
         """
         Parse the props.conf of the App & yield stanzas.
         For source with | (OR), it will return all combinations
 
         Yields:
```

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/app_test_generator.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/app_test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/data_model.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_set.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/data_set.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Alerts.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Alerts.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Authentication.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Authentication.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Certificates.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Certificates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Change.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Change.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/DLP.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/DLP.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Email.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Email.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Endpoint.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Endpoint.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Malware.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Malware.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998522458628841%*

 * *Differences: {"'objects'": "{0: {'fields': {6: {delete: ['validity']}, 30: {delete: ['validity']}}}}"}*

```diff
@@ -85,16 +85,15 @@
                     "comment": "The 802.11 channel used by a wireless network.",
                     "name": "channel",
                     "type": "not_allowed_in_search"
                 },
                 {
                     "comment": "The destination of the network traffic (the remote host). You can alias this from more specific fields, such as dest_host, dest_ip, or dest_name.",
                     "name": "dest",
-                    "type": "required",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
+                    "type": "required"
                 },
                 {
                     "comment": "The interface that is listening remotely or receiving packets locally. Can also be referred to as the 'egress interface.'",
                     "name": "dest_interface",
                     "type": "optional"
                 },
                 {
@@ -239,16 +238,15 @@
                     "comment": "The session identifier. Multiple transactions build a session.",
                     "name": "session_id",
                     "type": "optional"
                 },
                 {
                     "comment": "The source of the network traffic (the client requesting the connection). You can alias this from more specific fields, such as src_host, src_ip, or src_name.'",
                     "name": "src",
-                    "type": "required",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
+                    "type": "required"
                 },
                 {
                     "comment": "The interface that is listening locally or sending packets remotely. Can also be referred to as the 'ingress interface.'",
                     "name": "src_interface",
                     "type": "optional"
                 },
                 {
```

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Updates.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Updates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Web.json` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/data_models/Web.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/key_fields.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/key_fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/index_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/rule.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/rule.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,30 +16,28 @@
 from . import SampleGenerator
 import os
 import pickle
 from filelock import FileLock
 import json
 import pytest
 
+from pytest_splunk_addon.standard_lib import utils
+
 
 class SampleXdistGenerator:
     def __init__(self, addon_path, config_path=None, process_count=4):
         self.addon_path = addon_path
         self.process_count = process_count
         self.config_path = config_path
 
     def get_samples(self, store_events):
-
         if self.tokenized_event_source == "pregenerated":
             with open(self.event_path, "rb") as file_obj:
                 store_sample = pickle.load(file_obj)
-                if store_events and (
-                    "PYTEST_XDIST_WORKER" not in os.environ
-                    or os.environ.get("PYTEST_XDIST_WORKER") == "gw0"
-                ):
+                if store_events and utils.check_first_worker():
                     try:
                         tokenized_events = store_sample.get("tokenized_events")
                         self.store_events(tokenized_events)
                     except Exception as e:
                         pytest.exit(str(e))
                 return store_sample
```

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/__init__.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/junit_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/junit_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/log_helper.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/log_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/tools/cim_field_report.py` & `pytest_splunk_addon-5.3.0b3/pytest_splunk_addon/tools/cim_field_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b2/PKG-INFO` & `pytest_splunk_addon-5.3.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon
-Version: 5.3.0b2
+Version: 5.3.0b3
 Summary: A Dynamic test tool for Splunk Apps and Add-ons
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

