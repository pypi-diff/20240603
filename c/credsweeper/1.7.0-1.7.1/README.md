# Comparing `tmp/credsweeper-1.7.0.tar.gz` & `tmp/credsweeper-1.7.1.tar.gz`

## Comparing `credsweeper-1.7.0.tar` & `credsweeper-1.7.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/__init__.py
--rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/__main__.py
--rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/py.typed
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/__init__.py
--rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/constants.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/keyword_checklist.py
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/common/morpheme_checklist.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/config/__init__.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/config/config.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/candidate.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/candidate_key.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/credential_manager.py
--rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/credentials/line_data.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0        0        0    13915 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/docx_scanner.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/eml_scanner.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/jks_scanner.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/pkcs12_scanner.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/deep_scanner/zip_scanner.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/__init__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/abstract_provider.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/content_provider.py
--rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/descriptor.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/files_provider.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/patches_provider.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/filter.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/line_git_binary_check.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_atlassian_token_check.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base64_data_check.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base64_encoded_pem_check.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_base64_key_check.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_entropy_base64_check.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_github_check.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_hex_number_check.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_ip_check.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_jfrog_token_check.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_length_check.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_method_check.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_not_part_encoded_check.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_number_check.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_base64_check.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_token_check.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/variable_not_allowed_pattern_check.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/group.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/filters/group/weird_base64_token.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/logger/__init__.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/logger/logger.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/__init__.py
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/features.py
--rw-r--r--   0        0        0  5036009 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/ml_model/model_config.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/rules/__init__.py
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/rules/config.yaml
--rw-r--r--   0        0        0    10564 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/rules/rule.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/__init__.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scanner.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/secret/config.json
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/secret/log.yaml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/__init__.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/entropy_validator.py
--rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/pem_key_detector.py
--rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/utils/util.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/apply_validation.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/github_token_validation.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 credsweeper-1.7.0/credsweeper/validations/validation.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 credsweeper-1.7.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 credsweeper-1.7.0/LICENSE
--rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 credsweeper-1.7.0/README.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 credsweeper-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 credsweeper-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/__init__.py
+-rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/__main__.py
+-rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/py.typed
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/common/__init__.py
+-rw-r--r--   0        0        0     6058 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/common/constants.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/common/morpheme_checklist.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/config/__init__.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/config/config.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/credentials/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/credentials/candidate.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/credentials/line_data.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0        0        0    13915 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/docx_scanner.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/eml_scanner.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/jks_scanner.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/pkcs12_scanner.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/deep_scanner/zip_scanner.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/abstract_provider.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/descriptor.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/patches_provider.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/filter.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/line_git_binary_check.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_atlassian_token_check.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_base64_encoded_pem_check.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_base64_key_check.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_github_check.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_hex_number_check.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_ip_check.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_jfrog_token_check.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_length_check.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_method_check.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_number_check.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_token_check.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/variable_not_allowed_pattern_check.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/group.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/logger/__init__.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/logger/logger.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/ml_model/__init__.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/ml_model/features.py
+-rw-r--r--   0        0        0  5036009 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/ml_model/model_config.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/rules/__init__.py
+-rw-r--r--   0        0        0    26836 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/rules/config.yaml
+-rw-r--r--   0        0        0    10564 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/rules/rule.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/scanner/__init__.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/scanner/scanner.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/secret/config.json
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/secret/log.yaml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/utils/__init__.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/utils/entropy_validator.py
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/utils/pem_key_detector.py
+-rw-r--r--   0        0        0    24067 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/utils/util.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/apply_validation.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 credsweeper-1.7.1/credsweeper/validations/validation.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 credsweeper-1.7.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 credsweeper-1.7.1/LICENSE
+-rw-r--r--   0        0        0     9026 2020-02-02 00:00:00.000000 credsweeper-1.7.1/README.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 credsweeper-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 credsweeper-1.7.1/PKG-INFO
```

### Comparing `credsweeper-1.7.0/credsweeper/__init__.py` & `credsweeper-1.7.1/credsweeper/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
```

### Comparing `credsweeper-1.7.0/credsweeper/__main__.py` & `credsweeper-1.7.1/credsweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/app.py` & `credsweeper-1.7.1/credsweeper/app.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/common/constants.py` & `credsweeper-1.7.1/credsweeper/common/constants.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/common/keyword_checklist.py` & `credsweeper-1.7.1/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.7.1/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.7.1/credsweeper/common/morpheme_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/config/config.py` & `credsweeper-1.7.1/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.7.1/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/credentials/candidate.py` & `credsweeper-1.7.1/credsweeper/credentials/candidate.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.7.1/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/credentials/candidate_key.py` & `credsweeper-1.7.1/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/credentials/credential_manager.py` & `credsweeper-1.7.1/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/credentials/line_data.py` & `credsweeper-1.7.1/credsweeper/credentials/line_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import re
+from functools import cached_property
 from typing import Any, Dict, Optional, Tuple
 
-from credsweeper.common.constants import MAX_LINE_LENGTH
+from credsweeper.common.constants import MAX_LINE_LENGTH, CHUNKS_OVERLAP_SIZE
 from credsweeper.config import Config
 from credsweeper.utils import Util
 from credsweeper.utils.entropy_validator import EntropyValidator
 
 
 class LineData:
     """Object to treat and store scanned line related data.
@@ -26,15 +27,16 @@
 
     """
 
     comment_starts = ["//", "*", "#", "/*", "<!––", "%{", "%", "...", "(*", "--", "--[[", "#="]
     bash_param_split = re.compile("\\s+(\\-|\\||\\>|\\w+?\\>|\\&)")
     # some symbols e.g. double quotes cannot be in URL string https://www.ietf.org/rfc/rfc1738.txt
     # \ - was added for case of url in escaped string \u0026amp; - means escaped & in HTML
-    url_detect_regex = re.compile(r".*\w{3,33}://[\w;,/?:@&=+$%.!~*'()#\\-]+$")
+    url_scheme_part_regex = re.compile(r"[0-9A-Za-z.-]{3}")
+    url_chars_not_allowed_pattern = re.compile(r'[\s"<>\[\]^~`{|}]')
 
     INITIAL_WRONG_POSITION = -3
     EXCEPTION_POSITION = -2
 
     def __init__(
             self,  #
             config: Config,  #
@@ -68,14 +70,35 @@
         self.variable_start = LineData.INITIAL_WRONG_POSITION
         self.variable_end = LineData.INITIAL_WRONG_POSITION
         self.value_leftquote: Optional[str] = None
         self.value_rightquote: Optional[str] = None
 
         self.initialize(match_obj)
 
+    @cached_property
+    def line_len(self) -> int:
+        """cached property"""
+        return len(self.line)
+
+    @cached_property
+    def search_start(self) -> int:
+        """Decides from which position of line should be searched a pattern for line filters"""
+        if MAX_LINE_LENGTH >= self.line_len or CHUNKS_OVERLAP_SIZE > self.value_start:
+            return 0
+        else:
+            return self.value_start - CHUNKS_OVERLAP_SIZE
+
+    @cached_property
+    def search_end(self) -> int:
+        """Decides to which position of line should be searched a pattern for line filters"""
+        if MAX_LINE_LENGTH >= self.line_len or CHUNKS_OVERLAP_SIZE + self.value_end > self.line_len:
+            return self.line_len
+        else:
+            return self.value_end + CHUNKS_OVERLAP_SIZE
+
     def initialize(self, match_obj: Optional[re.Match] = None) -> None:
         """Apply regex to the candidate line and set internal fields based on match."""
         if not isinstance(match_obj, re.Match) and isinstance(self.pattern, re.Pattern):
             match_obj = self.pattern.search(self.line, endpos=MAX_LINE_LENGTH)
         if match_obj is None:
             return
 
@@ -100,38 +123,57 @@
         self.value_leftquote = get_group_from_match_obj(match_obj, "value_leftquote")
         self.value_rightquote = get_group_from_match_obj(match_obj, "value_rightquote")
         self.sanitize_value()
         self.sanitize_variable()
 
     def sanitize_value(self):
         """Clean found value from extra artifacts"""
-        _value = self.value
-        self.clean_url_parameters()
-        self.clean_bash_parameters()
-        self.check_value_pos(_value)
+        if self.variable and self.value:
+            # sanitize is actual step for keyword pattern only
+            _value = self.value
+            self.clean_url_parameters()
+            self.clean_bash_parameters()
+            self.check_value_pos(_value)
 
     def check_value_pos(self, value: str) -> None:
         """checks and corrects value_start, value_end in case of self.value was shrink"""
         if 0 <= self.value_start and 0 <= self.value_end and len(self.value) < len(value):
             start = value.find(self.value)
             self.value_start += start
             self.value_end = self.value_start + len(self.value)
 
     def clean_url_parameters(self) -> None:
         """Clean url address from 'query parameters'.
 
         If line seem to be a URL - split by & character.
         Variable should be right most value after & or ? ([-1]). And value should be left most before & ([0])
         """
-        line_before_value = self.line[:self.value_start]
-        if self.url_detect_regex.match(line_before_value):
-            if self.variable:
-                self.variable = self.variable.split('&')[-1].split('?')[-1].split(';')[-1]
-            if self.value:
-                self.value = self.value.split('&')[0].split(';')[0]
+        # search only in 8000 bytes before value because a URL length does not exceed in common
+        line_before_value = self.line[:self.value_start][-MAX_LINE_LENGTH:]
+        url_pos = -1
+        find_pos = 0
+        while find_pos < self.value_start:
+            # find rightmost pattern
+            find_pos = line_before_value.find("://", find_pos)
+            if -1 == find_pos:
+                break
+            else:
+                url_pos = find_pos
+                find_pos += 3
+        if 3 > url_pos:
+            return
+        if not self.url_scheme_part_regex.match(line_before_value, pos=url_pos - 3, endpos=url_pos):
+            # check for scheme naming - must be matched
+            return
+        # use line only after ://
+        if self.url_chars_not_allowed_pattern.search(line_before_value, pos=url_pos + 3):
+            return
+        # all checks have passed - line before the value may be a URL
+        self.variable = self.variable.rsplit('&', 1)[-1].rsplit('?', 1)[-1].rsplit(';', 1)[-1]
+        self.value = self.value.split('&', maxsplit=1)[0].split(';', maxsplit=1)[0]
 
     def clean_bash_parameters(self) -> None:
         """Split variable and value by bash special characters, if line assumed to be CLI command."""
         if self.variable and self.variable.startswith("-") and self.value:
             value_spl = self.bash_param_split.split(self.value)
             # If variable name starts with `-` (usual case for args in CLI)
             #  and value can be split by bash special characters
```

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/byte_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/deep_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/docx_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/docx_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/eml_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/eml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/html_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/jks_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/jks_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/pkcs12_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/pkcs12_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.7.1/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/__init__.py` & `credsweeper-1.7.1/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/abstract_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/abstract_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/analysis_target.py` & `credsweeper-1.7.1/credsweeper/file_handler/analysis_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,22 @@
 
     @cached_property
     def line_strip_len(self) -> int:
         """cached value"""
         return len(self.line_strip)
 
     @cached_property
-    def line_strip_lower(self) -> str:
+    def line_lower(self) -> str:
         """cached value"""
-        return self.line_strip.lower()
+        return self.line.lower()
+
+    @cached_property
+    def line_lower_strip(self) -> str:
+        """cached value"""
+        return self.line_lower.strip()
 
     @cached_property
     def lines(self) -> List[str]:
         """cached value"""
         return self.__lines
 
     @cached_property
```

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/content_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/data_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.7.1/credsweeper/file_handler/file_path_extractor.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/files_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/patches_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/patches_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.7.1/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/__init__.py` & `credsweeper-1.7.1/credsweeper/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/filter.py` & `credsweeper-1.7.1/credsweeper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/line_git_binary_check.py` & `credsweeper-1.7.1/credsweeper/filters/line_git_binary_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if line_data.line is None:
             return True
-        line = line_data.line.strip()
+        if 66 < target.line_strip_len:
+            return False
+        line = target.line_strip
         len_line = len(line)
 
         # https://github.com/git/git/blob/master/base85.c
 
         if 6 <= len_line and 0 == ((len_line - 1) % 5) and LineGitBinaryCheck.base85string.match(line):
             size = ord(line[0])
             if 65 <= size <= 90:  # A-Z
```

### Comparing `credsweeper-1.7.0/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.7.1/credsweeper/filters/line_specific_key_check.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from credsweeper.utils import Util
 
 
 class LineSpecificKeyCheck(Filter):
     """Check that values from list below is not in candidate line."""
 
     NOT_ALLOWED = [r"example", r"enc\(", r"enc\[", r"true", r"false"]
-    NOT_ALLOWED_PATTERN = re.compile(  #
-        Util.get_regex_combine_or(NOT_ALLOWED),  #
-        flags=re.IGNORECASE)
+    NOT_ALLOWED_PATTERN = re.compile(Util.get_regex_combine_or(NOT_ALLOWED))
 
     def __init__(self, config: Config = None) -> None:
         pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
@@ -28,11 +26,11 @@
         Return:
             True, if need to filter candidate and False if left
 
         """
         if line_data.line is None:
             return True
 
-        if self.NOT_ALLOWED_PATTERN.search(line_data.line):
+        if self.NOT_ALLOWED_PATTERN.search(target.line_lower, line_data.search_start, line_data.search_end):
             return True
 
         return False
```

### Comparing `credsweeper-1.7.0/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.7.1/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_atlassian_token_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_atlassian_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_base32_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_base64_data_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_base64_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_base64_encoded_pem_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_base64_encoded_pem_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_base64_key_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_base64_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_couple_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_entropy_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_entropy_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_entropy_base64_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_entropy_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_github_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_github_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_grafana_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_hex_number_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_hex_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_ip_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_number_check.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import contextlib
-import ipaddress
+import re
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueIPCheck(Filter):
-    """Filter out some of insensible IP"""
+class ValueNumberCheck(Filter):
+    """Check value if it a value in hex or decimal representation"""
 
-    FALSE_POSITIVE_MARKERS = ["version", "oid", "section", "rfc"]
+    HEX_VALUE_REGEX = re.compile("^(0x)?[0-9a-f]{1,128}[ul]{0,3}$")
+    DEC_VALUE_REGEX = re.compile("^-?[0-9]{1,20}[ul]{0,3}$")
 
     def __init__(self, config: Config = None) -> None:
         pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
@@ -24,21 +24,13 @@
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-
-        with contextlib.suppress(Exception):
-            ip = ipaddress.ip_address(line_data.value)
-            if 4 == ip.version:
-                # use line_strip_lower due the property should be cached already
-                line_strip_lower = target.line_strip_lower
-                for i in ValueIPCheck.FALSE_POSITIVE_MARKERS:
-                    if i in line_strip_lower:
-                        return True
-            if ip.is_loopback or ip.is_private or ip.is_reserved or ip.is_link_local or ip.is_multicast:
-                return True
-            return False
-
-        return True
+        value = line_data.value.lower()
+        if 22 > len(value) and ValueNumberCheck.HEX_VALUE_REGEX.match(value):
+            return True
+        if ValueNumberCheck.DEC_VALUE_REGEX.match(value):
+            return True
+        return False
```

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_jfrog_token_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_jfrog_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_json_web_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_length_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_method_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_method_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_not_part_encoded_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_not_part_encoded_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_number_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_token_check.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class ValueNumberCheck(Filter):
-    """Check value if it a value in hex or decimal representation"""
+class ValueTokenCheck(Filter):
+    """Check if first substring of token is shorter than 5.
 
-    HEX_VALUE_REGEX = re.compile("^(0x)?[0-9a-f]+[ul]*$")
-    DEC_VALUE_REGEX = re.compile("^-?[0-9]+[ul]*$")
+    Split candidate value into substrings using ` ;`{})(<>[]` separators. Check if first substring is shorter than 5
+
+    Examples:
+        "my password"
+        "12);password"
+
+    """
+
+    SPLIT_PATTERN = r" |;|\)|\(|{|}|<|>|\[|\]|`"
 
     def __init__(self, config: Config = None) -> None:
         pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
 
@@ -24,13 +31,18 @@
 
         Return:
             True, if need to filter candidate and False if left
 
         """
         if not line_data.value:
             return True
-        value = line_data.value.lower()
-        if 22 > len(value) and ValueNumberCheck.HEX_VALUE_REGEX.match(value):
-            return True
-        if ValueNumberCheck.DEC_VALUE_REGEX.match(value):
+
+        tokens = re.split(self.SPLIT_PATTERN, line_data.value, maxsplit=1)
+        # If tokens have length of 1 - pattern is not present in the value and original value returned from `.split(`
+        if len(tokens) < 2:
+            return False
+
+        token = tokens[0]
+        if len(token) < 5:
             return True
+
         return False
```

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_split_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_token_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_token_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_token_base64_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_token_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.7.1/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.7.1/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/group/__init__.py` & `credsweeper-1.7.1/credsweeper/filters/group/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/group/group.py` & `credsweeper-1.7.1/credsweeper/filters/group/group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/group/password_keyword.py` & `credsweeper-1.7.1/credsweeper/filters/group/password_keyword.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.7.1/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.7.1/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.7.1/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/filters/group/weird_base64_token.py` & `credsweeper-1.7.1/credsweeper/filters/group/weird_base64_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/logger/logger.py` & `credsweeper-1.7.1/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/ml_model/features.py` & `credsweeper-1.7.1/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.7.1/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.7.1/credsweeper/ml_model/ml_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/ml_model/model_config.json` & `credsweeper-1.7.1/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/rules/config.yaml` & `credsweeper-1.7.1/credsweeper/rules/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     - doc
 
 - name: IP_ID_PASSWORD_TRIPLE
   severity: medium
   confidence: moderate
   type: pattern
   values:
-    - (^|\s|(?P<variable>(?i:\bip[\s/]+id[\s/]+pw[\s/:]*))|(?P<url>://))(?P<ip>[0-2]?[0-9]{1,2}\.[0-2]?[0-9]{1,2}\.[0-2]?[0-9]{1,2}\.[0-2]?[0-9]{1,2})((\s*\()?|(?(variable)[\s,/]+|(?(url)[,]|[,/])))\s*\w[\w.-]{3,80}[\s,/]+(?P<value>(?(url)(?-i:(?P<a>[A-Z])|(?P<b>[a-z])|(?P<c>[0-9_+=~!@#$%^&*;?-])){7,31}(?(a)(?(b)(?(c)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x)|(?-i:(?P<e>[A-Z])|(?P<f>[a-z])|(?P<g>[0-9/_+=~!@#$%^&*;?-])){7,31}(?(e)(?(f)(?(g)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x)))(?:\s|[^/]|$)
+    - (^|\s|(?P<variable>(?i:\bip[\s/]{1,80}id[\s/]{1,80}pw[\s/:]{0,80}))|(?P<url>://))(?P<ip>[0-2]?[0-9]{1,2}\.[0-2]?[0-9]{1,2}\.[0-2]?[0-9]{1,2}\.[0-2]?[0-9]{1,2})((\s*\()?|(?(variable)[\s,/]{1,80}|(?(url)[,]|[,/])))\s*\w[\w.-]{3,80}[\s,/]{1,80}(?P<value>(?(url)(?-i:(?P<a>[A-Z])|(?P<b>[a-z])|(?P<c>[0-9_+=~!@#$%^&*;?-])){7,31}(?(a)(?(b)(?(c)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x)|(?-i:(?P<e>[A-Z])|(?P<f>[a-z])|(?P<g>[0-9/_+=~!@#$%^&*;?-])){7,31}(?(e)(?(f)(?(g)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x)))(?:\s|[^/]|$)
   filter_type:
     - ValueAllowlistCheck
     - ValuePatternCheck
     - ValueDictionaryKeywordCheck
   min_line_len: 10
   required_substrings:
     - "."
@@ -68,15 +68,15 @@
     - doc
 
 - name: ID_PAIR_PASSWD_PAIR
   severity: medium
   confidence: moderate
   type: pattern
   values:
-    - (?P<ddash>--)?(?P<variable>\w*(?i:pa[as]swords?|passwd?|pwd|\bp/w|\bpw|비밀번호|비번|패스워드|암호))\s*?(?(ddash)[ =]|[:=/>-]{1,2})\s*(?P<quote>[`'\"]+)?(?P<value>(?-i:(?P<a>[A-Z])|(?P<b>[a-z])|(?P<c>[0-9/_+=~!@#$%^&*;:?-])){4,31}(?(a)(?(b)(?(c)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x))(?(quote)(?P=quote)|(\s|$))
+    - (?P<ddash>--)?(?P<variable>\w*(?i:pa[as]swords?|passwd?|pwd|\bp/w|\bpw|비밀번호|비번|패스워드|암호))\s*?(?(ddash)[ =]|[:=/>-]{1,2})\s*(?P<quote>[`'\"]{1,8})?(?P<value>(?-i:(?P<a>[A-Z])|(?P<b>[a-z])|(?P<c>[0-9/_+=~!@#$%^&*;:?-])){4,31}(?(a)(?(b)(?(c)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x))(?(quote)(?P=quote)|(\s|$))
     - (?P<ddash>--)?(?P<variable>(?i:user\s*)?(?i:id|login|account|root|admin|user|name|wifi|role|host|default|계정|아이디))\s*?(?(ddash)[ =]|[ :=])\s*?(?P<value>\S+)
   filter_type:
     - ValueAllowlistCheck
     - ValuePatternCheck
   min_line_len: 10
   required_substrings:
     - pass
@@ -91,15 +91,15 @@
     - doc
 
 - name: ID_PASSWD_PAIR
   severity: medium
   confidence: moderate
   type: pattern
   values:
-    - (?P<variable>[\w.-]*(?i:(?P<id>\bid\b)|id\b|user|name|계정|아이디)[\w.-]*(?(id)[ :(/]+|[:(/]+)(?i:pa[as]swo?r?ds?|pwd?|비밀번호|비번|패스워드|암호))\)?(\s*->\s*|[ =:)(/]+|\s+is\s+|\s+are\s+|\s*는\s*|\s*은\s*|\s*설정은\s*)\(?(?P<id_value>[\w.-]{2,31})[ :\(/\"',]+(?P<value>(?-i:(?P<a>[A-Z])|(?P<b>[a-z])|(?P<c>[0-9/_+=~!@#$%^&*;:?-])){4,31}(?(a)(?(b)(?(c)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x))
+    - (?P<variable>[\w.-]{0,80}(?i:(?P<id>\bid\b)|id\b|user|name|계정|아이디)[\w.-]{0,80}(?(id)[ :(/]{1,80}|[:(/]{1,80})(?i:pa[as]swo?r?ds?|pwd?|비밀번호|비번|패스워드|암호))\)?(\s*->\s*|[ =:)(/]{1,80}|\s+is\s+|\s+are\s+|\s*는\s*|\s*은\s*|\s*설정은\s*)\(?(?P<id_value>[\w.-]{2,31})[ :\(/\"',]{1,80}(?P<value>(?-i:(?P<a>[A-Z])|(?P<b>[a-z])|(?P<c>[0-9/_+=~!@#$%^&*;:?-])){4,31}(?(a)(?(b)(?(c)(\S|$)|(?!x)x)|(?!x)x)|(?!x)x))
   filter_type:
     - ValueAllowlistCheck
     - ValuePatternCheck
     - ValueDictionaryKeywordCheck
   min_line_len: 10
   required_substrings:
     - pw
@@ -242,15 +242,15 @@
     - doc
 
 - name: Github Old Token
   severity: high
   confidence: moderate
   type: pattern
   values:
-    - (?i)((git)[\w\-]*(token|key|api)[\w\-]*(\s)*(=|:|:=)(\s)*(["']?)(?P<value>[a-z|\d]{40})(["']?))
+    - (?i)((git)[\w\-]{0,80}(token|key|api)[\w\-]{0,80}(\s)*(=|:|:=)(\s)*(["']?)(?P<value>[a-z|\d]{40})(["']?))
   filter_type: GeneralPattern
   use_ml: true
   validations:
     - GithubTokenValidation
   required_substrings:
     - git
   min_line_len: 47
@@ -421,26 +421,26 @@
     - doc
 
 - name: PEM Private Key
   severity: high
   confidence: strong
   type: pem_key
   values:
-    - (?P<value>-----BEGIN\s(?!ENCRYPTED)[^-]*PRIVATE[^-]*KEY[^-]{0,40}-----(.+-----END[^-]+KEY[^-]{0,40}-----)?)
+    - (?P<value>-----BEGIN\s(?!ENCRYPTED)[^-]{0,80}PRIVATE[^-]{0,80}KEY[^-]{0,40}-----(.+-----END[^-]{1,80}KEY[^-]{0,40}-----)?)
   min_line_len: 27
   target:
     - code
     - doc
 
 - name: BASE64 encoded PEM Private Key
   severity: high
   confidence: strong
   type: pattern
   values:
-    - (?P<value>[0-9A-Za-z_/+-]*LS0t(LS1CRUdJTiB|LUJFR0lOI|QkVHSU4g)[0-9A-Za-z_/+-]{0,11}(UFJJVkFURSBLRVkt|QUklWQVRFIEtFWS0t|FBSSVZBVEUgS0VZ)[0-9A-Za-z_/+-]+LS0t[0-9A-Za-z_/+-]+)
+    - (?P<value>[0-9A-Za-z_/+-]{0,8000}LS0t(LS1CRUdJTiB|LUJFR0lOI|QkVHSU4g)[0-9A-Za-z_/+-]{0,11}(UFJJVkFURSBLRVkt|QUklWQVRFIEtFWS0t|FBSSVZBVEUgS0VZ)[0-9A-Za-z_/+-]{1,8000}LS0t[0-9A-Za-z_/+-]{1,8000})
   filter_type:
     - ValueBase64EncodedPem
   min_line_len: 300
   required_substrings:
     - UFJJVkFURSBLRVkt
     - QUklWQVRFIEtFWS0t
     - FBSSVZBVEUgS0VZ
@@ -654,15 +654,15 @@
     - doc
 
 - name: URL Credentials
   severity: high
   confidence: moderate
   type: pattern
   values:
-    - (?P<value_leftquote>["'])?(?P<variable>\w{2,80}://)[\w%.:-]*(?P<separator>:)(?P<value>[^\s/\@:]{3,80})@[\w.-]+\\*(?P<value_rightquote>["'])?
+    - (?P<value_leftquote>["'])?(?P<variable>\w{2,80}://)[\w%.:-]{0,80}(?P<separator>:)(?P<value>[^\s/\@:]{3,80})@[\w.-]{1,800}\\{0,8}(?P<value_rightquote>["'])?
   filter_type: UrlCredentialsGroup
   use_ml: true
   required_substrings:
     - ://
   min_line_len: 10
   target:
     - code
@@ -761,15 +761,15 @@
     - doc
 
 - name: Firebase Domain
   severity: info
   confidence: moderate
   type: pattern
   values:
-    - (?<![0-9A-Za-z_])(?P<value>[a-z0-9.-]+\.firebaseio\.com|[a-z0-9.-]+\.firebaseapp\.com)
+    - (?<![0-9A-Za-z_])(?P<value>[a-z0-9.-]{1,80}\.firebaseio\.com|[a-z0-9.-]{1,80}\.firebaseapp\.com)
   filter_type: GeneralPattern
   required_substrings:
     - .firebase
   min_line_len: 16
   target:
     - code
     - doc
@@ -848,15 +848,15 @@
     - doc
 
 - name: Azure Access Token
   severity: high
   confidence: strong
   type: pattern
   values:
-    - (?<![0-9A-Za-z_+-])(?P<value>eyJ[A-Za-z0-9_=-]{50,500}\.eyJ[A-Za-z0-9_=-]+\.[A-Za-z0-9_=-]+)
+    - (?<![0-9A-Za-z_+-])(?P<value>eyJ[A-Za-z0-9_=-]{50,500}\.eyJ[A-Za-z0-9_=-]{1,8000}\.[A-Za-z0-9_=-]{1,8000})
   filter_type:
     - ValueJsonWebTokenCheck
   required_substrings:
     - eyJ
   min_line_len: 148
   target:
     - code
```

### Comparing `credsweeper-1.7.0/credsweeper/rules/rule.py` & `credsweeper-1.7.1/credsweeper/rules/rule.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/scanner/scanner.py` & `credsweeper-1.7.1/credsweeper/scanner/scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             if not (matched_keyword or matched_pem_key or matched_pattern or matched_multi):
                 # target may be skipped only with length because not all rules have required_substrings
                 logger.debug("Skip too short (%d) line %s:%d", target_line_stripped_len, target.file_path,
                              target.line_num)
                 continue
 
             # use lower case for required substring
-            target_line_stripped_lower = target.line_strip_lower
+            target_line_stripped_lower = target.line_lower_strip
             # cached value to skip the same regex verifying
             matched_regex: Dict[re.Pattern, bool] = {}
 
             for rule, scanner in self.yield_rule_scanner(target_line_stripped_len, matched_pattern, matched_keyword,
                                                          matched_pem_key, matched_multi):
                 if rule.has_required_substrings \
                         and not self._substring_check(rule.required_substrings, target_line_stripped_lower):
```

### Comparing `credsweeper-1.7.0/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.7.1/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.7.1/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.7.1/credsweeper/scanner/scan_type/scan_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import re
 from abc import ABC, abstractmethod
-from typing import List, Optional, Tuple, Dict
+from typing import List, Optional, Tuple, Dict, Set
 
 from credsweeper.common.constants import RuleType, MAX_LINE_LENGTH, CHUNK_STEP_SIZE, CHUNKS_OVERLAP_SIZE
 from credsweeper.config import Config
 from credsweeper.credentials import Candidate, LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 from credsweeper.rules import Rule
@@ -58,14 +58,34 @@
             if filter_.run(line_data, target):
                 logger.debug("Filtered line with filter: %s in file: %s:%d  in line: %s value: %s",
                              filter_.__class__.__name__, line_data.path, line_data.line_num, line_data.line,
                              line_data.value)
                 return True
         return False
 
+    @staticmethod
+    def get_chunks(line_len: int) -> Set[Tuple[int, int]]:
+        """Returns chunks positions for given line length"""
+        chunks = {(0, line_len if MAX_LINE_LENGTH > line_len else MAX_LINE_LENGTH)}
+        # case for oversize line
+        next_offset = CHUNK_STEP_SIZE
+        while line_len > next_offset + CHUNKS_OVERLAP_SIZE:
+            # the target is too long for single "finditer" - it will be scanned by chunks
+            if line_len < next_offset + MAX_LINE_LENGTH:
+                # best overlap for tail
+                chunks.add((line_len - MAX_LINE_LENGTH, line_len))
+                break
+            else:
+                # the chunk is not the last
+                chunk_end = line_len if next_offset + MAX_LINE_LENGTH > line_len \
+                    else next_offset + MAX_LINE_LENGTH
+                chunks.add((next_offset, chunk_end))
+                next_offset += CHUNK_STEP_SIZE
+        return chunks
+
     @classmethod
     def get_line_data_list(
             cls,  #
             config: Config,  #
             target: AnalysisTarget,  #
             pattern: re.Pattern,  #
             filters: List[Filter]) -> List[LineData]:
@@ -78,45 +98,33 @@
             filters: Filters to use
 
         Return:
             List of LineData objects if pattern a line and filters do not remove current line. Empty otherwise
 
         """
         line_data_list: List[LineData] = []
-        # starting positions for continuously searching for overlapping pattern
-        offsets = {0}
-        # case for oversize line
-        next_offset = CHUNK_STEP_SIZE
-        while target.line_len > next_offset + CHUNKS_OVERLAP_SIZE:
-            # the target is too long for single "finditer" - it will be scanned by chunks
-            if target.line_len < next_offset + MAX_LINE_LENGTH:
-                # best overlap for tail
-                offsets.add(target.line_len - MAX_LINE_LENGTH)
-                break
-            else:
-                # the chunk is not the last
-                offsets.add(next_offset)
-                next_offset += CHUNK_STEP_SIZE
+        # start - end positions for continuously searching for overlapping pattern
+        offsets = cls.get_chunks(target.line_len)
 
         # used to avoid duplicates for overlap cases only if line is oversize
         purged_line_data: Optional[Dict[Tuple[int, int, int, int, int, int, int], LineData]] = {} if 1 < len(offsets) \
             else None
 
         while offsets:
-            offset = offsets.pop()
-            for _match in pattern.finditer(target.line, pos=offset, endpos=offset + MAX_LINE_LENGTH):
+            offset_start, offset_end = offsets.pop()
+            for _match in pattern.finditer(target.line, pos=offset_start, endpos=offset_end):
                 logger.debug("Valid line for pattern: %s in file: %s:%d in line: %s", pattern.pattern, target.file_path,
                              target.line_num, target.line)
                 line_data = LineData(config, target.line, target.line_pos, target.line_num, target.file_path,
                                      target.file_type, target.info, pattern, _match)
 
                 if config.use_filters and cls.filtering(config, target, line_data, filters):
                     if 0 < line_data.variable_end:
                         # may be next matched item will be not filtered - let search it after variable
-                        offsets.add(line_data.variable_end)
+                        offsets.add((line_data.variable_end, offset_end))
                     continue
                 line_data_list.append(line_data)
 
         if isinstance(purged_line_data, dict) and 1 < len(line_data_list):
             # workaround for removing duplicates in case of oversize line only
             for i in line_data_list:
                 ld_key = (i.line_num, i.value_start, i.value_end, i.separator_start, i.separator_end, i.variable_start,
```

### Comparing `credsweeper-1.7.0/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.7.1/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/secret/config.json` & `credsweeper-1.7.1/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/secret/log.yaml` & `credsweeper-1.7.1/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/utils/entropy_validator.py` & `credsweeper-1.7.1/credsweeper/utils/entropy_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/utils/pem_key_detector.py` & `credsweeper-1.7.1/credsweeper/utils/pem_key_detector.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/utils/util.py` & `credsweeper-1.7.1/credsweeper/utils/util.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/__init__.py` & `credsweeper-1.7.1/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/apply_validation.py` & `credsweeper-1.7.1/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/github_token_validation.py` & `credsweeper-1.7.1/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.7.1/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.7.1/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.7.1/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.7.1/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.7.1/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.7.1/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.7.1/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/credsweeper/validations/validation.py` & `credsweeper-1.7.1/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/.gitignore` & `credsweeper-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/LICENSE` & `credsweeper-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/README.md` & `credsweeper-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/pyproject.toml` & `credsweeper-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.7.0/PKG-INFO` & `credsweeper-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: credsweeper
-Version: 1.7.0
+Version: 1.7.1
 Summary: Credential Sweeper
 Project-URL: Homepage, https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

