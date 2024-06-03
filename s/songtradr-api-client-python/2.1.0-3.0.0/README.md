# Comparing `tmp/songtradr_api_client_python-2.1.0.tar.gz` & `tmp/songtradr_api_client_python-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songtradr_api_client_python-2.1.0.tar", last modified: Mon Apr 29 09:02:16 2024, max compression
+gzip compressed data, was "songtradr_api_client_python-3.0.0.tar", last modified: Mon Jun  3 14:40:52 2024, max compression
```

## Comparing `songtradr_api_client_python-2.1.0.tar` & `songtradr_api_client_python-3.0.0.tar`

### file list

```diff
@@ -1,125 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.123218 songtradr_api_client_python-2.1.0/songtradr_api_client_python/
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.127218 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34921 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   126485 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/recording_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   347657 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28037 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.135218 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/image_recognition_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/login_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    46483 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/title_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/track_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/video_recognition_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 09:02:16.000000 songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:16.147219 songtradr_api_client_python-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/test/test_allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    23731 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_image_recognition_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_login_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/test/test_recording_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    20033 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_title_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_track_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-29 09:02:09.000000 songtradr_api_client_python-2.1.0/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-29 09:02:08.000000 songtradr_api_client_python-2.1.0/test/test_video_recognition_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:40:52.088636 songtradr_api_client_python-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-06-03 14:40:52.088636 songtradr_api_client_python-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-03 14:40:52.088636 songtradr_api_client_python-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:40:52.068636 songtradr_api_client_python-3.0.0/songtradr_api_client_python/
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:40:52.068636 songtradr_api_client_python-3.0.0/songtradr_api_client_python/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13437 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/api/allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47621 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/api/recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   276955 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28037 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16424 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:40:52.076636 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46483 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/track_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/video_recognition_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:40:52.084636 songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-06-03 14:40:52.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-06-03 14:40:52.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 14:40:52.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-03 14:40:52.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-03 14:40:52.000000 songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 14:40:52.084636 songtradr_api_client_python-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/test/test_allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23731 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/test/test_recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_track_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-06-03 14:40:43.000000 songtradr_api_client_python-3.0.0/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-06-03 14:40:42.000000 songtradr_api_client_python-3.0.0/test/test_video_recognition_response.py
```

### Comparing `songtradr_api_client_python-2.1.0/PKG-INFO` & `songtradr_api_client_python-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 2.1.0
+Version: 3.0.0
 Summary: Songtradr API
 Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `songtradr_api_client_python-2.1.0/README.md` & `songtradr_api_client_python-3.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.
 
 1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters.
 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.1.0
-- Package version: 2.1.0
-- Generator version: 7.6.0-SNAPSHOT
+- API version: 3.0.0
+- Package version: 3.0.0
+- Generator version: 7.7.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://songtradr.com](https://songtradr.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -110,50 +110,38 @@
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.songtradr.com*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AllowedValuesApi* | [**allowed_musical_features**](docs/AllowedValuesApi.md#allowed_musical_features) | **GET** /api/v1/allowedValues/musicalFeatures | Allowed values for music descriptive parameters to be used in the searchAll endpoint.
-*AllowedValuesApi* | [**genres**](docs/AllowedValuesApi.md#genres) | **GET** /api/v1/allowedValues/genre | Allowed values for genres.
-*AllowedValuesApi* | [**tags**](docs/AllowedValuesApi.md#tags) | **GET** /api/v1/allowedValues/tag | All descriptive tags inside of tag-categories.
-*RecordingApi* | [**prompt_search_recordings**](docs/RecordingApi.md#prompt_search_recordings) | **GET** /api/v1/public/recording/promptSearch | Recordings for query.
-*RecordingApi* | [**recordings_by_ids_with_musical_features**](docs/RecordingApi.md#recordings_by_ids_with_musical_features) | **GET** /api/v1/public/recording/{ids}/musicalFeatures | AI generated moods, musical features and more for recordings.
-*RecordingApi* | [**recordings_by_ids_with_similarities1**](docs/RecordingApi.md#recordings_by_ids_with_similarities1) | **GET** /api/v1/public/recording/{ids}/similarities | Similar recordings for a list of recordings.
 *RecordingApi* | [**recordings_by_ids_with_taggrams1**](docs/RecordingApi.md#recordings_by_ids_with_taggrams1) | **GET** /api/v1/public/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
 *RecordingApi* | [**recordings_by_ids_with_tagstrengths1**](docs/RecordingApi.md#recordings_by_ids_with_tagstrengths1) | **GET** /api/v1/public/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
 *RecordingApi* | [**recordings_medium_by_ids1**](docs/RecordingApi.md#recordings_medium_by_ids1) | **GET** /api/v1/public/recording/m/{ids} | Recordings by IDs with a medium sized response.
-*RecordingApi* | [**search_recordings**](docs/RecordingApi.md#search_recordings) | **GET** /api/v1/public/recording/search | Recordings by contributors, moods, musical features and more.
 *UserApi* | [**delete_user_file**](docs/UserApi.md#delete_user_file) | **DELETE** /api/v1/user/file/{objectKey} | Delete file.
 *UserApi* | [**edit_me**](docs/UserApi.md#edit_me) | **POST** /api/v1/user/me | Edit details for a logged-in user
 *UserApi* | [**forgot_password**](docs/UserApi.md#forgot_password) | **POST** /api/v1/user/forgot-password | Send a password reset email
 *UserApi* | [**init_video_upload**](docs/UserApi.md#init_video_upload) | **POST** /api/v1/user/file/{name}/initVideoUpload | Recognise and upload video. Responds with an object with recognition result.
 *UserApi* | [**initiate_user_file_upload**](docs/UserApi.md#initiate_user_file_upload) | **POST** /api/v1/user/file/{name}/initUpload | Initialize a file upload. Responds with an URL where the file can be uploaded.
-*UserApi* | [**initiate_user_image_upload**](docs/UserApi.md#initiate_user_image_upload) | **POST** /api/v1/user/file/{name}/initImageUpload | Recognise and upload image. Responds with an object with recognition result.
 *UserApi* | [**login**](docs/UserApi.md#login) | **POST** /api/v1/user/login | Login to generate a bearer token.
 *UserApi* | [**me**](docs/UserApi.md#me) | **GET** /api/v1/user/me | Details for a logged-in user
-*UserApi* | [**prompt_search_user_files**](docs/UserApi.md#prompt_search_user_files) | **GET** /api/v1/user/promptSearch | Files for query.
-*UserApi* | [**recordings_by_folder_with_taggrams**](docs/UserApi.md#recordings_by_folder_with_taggrams) | **GET** /api/v1/user/folder/{folderName}/taggrams | Timeseries of AI generated moods, musical features and more for recordings in your folder.
-*UserApi* | [**recordings_by_folder_with_tagstrengths**](docs/UserApi.md#recordings_by_folder_with_tagstrengths) | **GET** /api/v1/user/folder/{folderName}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
-*UserApi* | [**recordings_by_ids_with_similarities**](docs/UserApi.md#recordings_by_ids_with_similarities) | **GET** /api/v1/user/recording/{ids}/similarities | Similar recordings for a list of user recordings.
 *UserApi* | [**recordings_by_ids_with_taggrams**](docs/UserApi.md#recordings_by_ids_with_taggrams) | **GET** /api/v1/user/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
 *UserApi* | [**recordings_by_ids_with_tagstrengths**](docs/UserApi.md#recordings_by_ids_with_tagstrengths) | **GET** /api/v1/user/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
 *UserApi* | [**recordings_medium_by_ids**](docs/UserApi.md#recordings_medium_by_ids) | **GET** /api/v1/user/recording/{ids} | Recordings by IDs with a medium sized response.
 *UserApi* | [**sign_up**](docs/UserApi.md#sign_up) | **POST** /api/v1/user/sign-up | Sign up a new user.
 *UserApi* | [**token**](docs/UserApi.md#token) | **POST** /api/v1/user/token | Generates a new JWT token for the given refresh token
 *UserApi* | [**update_password**](docs/UserApi.md#update_password) | **POST** /api/v1/user/update-password | Update password by using the password reset token
 *UserApi* | [**user_file**](docs/UserApi.md#user_file) | **GET** /api/v1/user/file/{objectKey} | Details and a download link for a file.
 *UserApi* | [**user_files**](docs/UserApi.md#user_files) | **GET** /api/v1/user/files | List and search your own files.
 *UserApi* | [**user_files_status**](docs/UserApi.md#user_files_status) | **GET** /api/v1/user/filesStatus | Status details for files.
 *UserApi* | [**user_files_summary**](docs/UserApi.md#user_files_summary) | **GET** /api/v1/user/filesSummary | Summary fo your files.
 
 
 ## Documentation For Models
 
- - [CategoryMediumDTO](docs/CategoryMediumDTO.md)
  - [CategoryMinimalDTO](docs/CategoryMinimalDTO.md)
  - [ConfigAccessDTO](docs/ConfigAccessDTO.md)
  - [ConfigIdentifierDTO](docs/ConfigIdentifierDTO.md)
  - [ContributorTypeDTO](docs/ContributorTypeDTO.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [FieldSummaryDTO](docs/FieldSummaryDTO.md)
  - [FileDTO](docs/FileDTO.md)
@@ -162,35 +150,29 @@
  - [FileUploadDTO](docs/FileUploadDTO.md)
  - [FileWIthUrlDTO](docs/FileWIthUrlDTO.md)
  - [FilesSummaryDTO](docs/FilesSummaryDTO.md)
  - [ForgotPasswordDTO](docs/ForgotPasswordDTO.md)
  - [GenreDTO](docs/GenreDTO.md)
  - [GenreMinimalDTO](docs/GenreMinimalDTO.md)
  - [GenresSummaryDTO](docs/GenresSummaryDTO.md)
- - [ImageRecognitionResponse](docs/ImageRecognitionResponse.md)
  - [InitPutRecordingAudioDTO](docs/InitPutRecordingAudioDTO.md)
  - [JwtTokenDTO](docs/JwtTokenDTO.md)
  - [LoginDTO](docs/LoginDTO.md)
  - [MusicalFeaturesDTO](docs/MusicalFeaturesDTO.md)
  - [PartySmallDTO](docs/PartySmallDTO.md)
- - [RecordingForSimilaritySearchDTO](docs/RecordingForSimilaritySearchDTO.md)
  - [RecordingGenrePredictionDTO](docs/RecordingGenrePredictionDTO.md)
- - [RecordingListDTO](docs/RecordingListDTO.md)
  - [RecordingMediumDTO](docs/RecordingMediumDTO.md)
- - [RecordingMinimalWithMusicalFeaturesDTO](docs/RecordingMinimalWithMusicalFeaturesDTO.md)
  - [RecordingMinimalWithTaggramsDTO](docs/RecordingMinimalWithTaggramsDTO.md)
  - [RecordingMinimalWithTagstrengthsDTO](docs/RecordingMinimalWithTagstrengthsDTO.md)
  - [RecordingPartyDTO](docs/RecordingPartyDTO.md)
- - [RecordingSmallDTO](docs/RecordingSmallDTO.md)
  - [RecordingTagSmallDTO](docs/RecordingTagSmallDTO.md)
  - [SaveUserDTO](docs/SaveUserDTO.md)
  - [SearchFilterValuesDTO](docs/SearchFilterValuesDTO.md)
  - [SignUpDTO](docs/SignUpDTO.md)
  - [TagDTO](docs/TagDTO.md)
- - [TagSmallDTO](docs/TagSmallDTO.md)
  - [TaggramDTO](docs/TaggramDTO.md)
  - [TagsSummaryDTO](docs/TagsSummaryDTO.md)
  - [TagstrengthDTO](docs/TagstrengthDTO.md)
  - [TitleDTO](docs/TitleDTO.md)
  - [TokenRequest](docs/TokenRequest.md)
  - [TrackDTO](docs/TrackDTO.md)
  - [UpdatePasswordDTO](docs/UpdatePasswordDTO.md)
```

### Comparing `songtradr_api_client_python-2.1.0/pyproject.toml` & `songtradr_api_client_python-3.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "songtradr_api_client_python"
-version = "2.1.0"
+version = "3.0.0"
 description = "Songtradr API"
 authors = ["Songtradr Inc. <info@songtradr.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Songtradr API"]
 include = ["songtradr_api_client_python/py.typed"]
```

### Comparing `songtradr_api_client_python-2.1.0/setup.py` & `songtradr_api_client_python-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "songtradr-api-client-python"
-VERSION = "2.1.0"
+VERSION = "3.0.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/__init__.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2.1.0"
+__version__ = "3.0.0"
 
 # import apis into sdk package
 from songtradr_api_client_python.api.allowed_values_api import AllowedValuesApi
 from songtradr_api_client_python.api.recording_api import RecordingApi
 from songtradr_api_client_python.api.user_api import UserApi
 
 # import ApiClient
@@ -30,15 +30,14 @@
 from songtradr_api_client_python.exceptions import ApiTypeError
 from songtradr_api_client_python.exceptions import ApiValueError
 from songtradr_api_client_python.exceptions import ApiKeyError
 from songtradr_api_client_python.exceptions import ApiAttributeError
 from songtradr_api_client_python.exceptions import ApiException
 
 # import models into sdk package
-from songtradr_api_client_python.models.category_medium_dto import CategoryMediumDTO
 from songtradr_api_client_python.models.category_minimal_dto import CategoryMinimalDTO
 from songtradr_api_client_python.models.config_access_dto import ConfigAccessDTO
 from songtradr_api_client_python.models.config_identifier_dto import ConfigIdentifierDTO
 from songtradr_api_client_python.models.contributor_type_dto import ContributorTypeDTO
 from songtradr_api_client_python.models.error_response import ErrorResponse
 from songtradr_api_client_python.models.field_summary_dto import FieldSummaryDTO
 from songtradr_api_client_python.models.file_dto import FileDTO
@@ -47,35 +46,29 @@
 from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO
 from songtradr_api_client_python.models.file_w_ith_url_dto import FileWIthUrlDTO
 from songtradr_api_client_python.models.files_summary_dto import FilesSummaryDTO
 from songtradr_api_client_python.models.forgot_password_dto import ForgotPasswordDTO
 from songtradr_api_client_python.models.genre_dto import GenreDTO
 from songtradr_api_client_python.models.genre_minimal_dto import GenreMinimalDTO
 from songtradr_api_client_python.models.genres_summary_dto import GenresSummaryDTO
-from songtradr_api_client_python.models.image_recognition_response import ImageRecognitionResponse
 from songtradr_api_client_python.models.init_put_recording_audio_dto import InitPutRecordingAudioDTO
 from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
 from songtradr_api_client_python.models.login_dto import LoginDTO
 from songtradr_api_client_python.models.musical_features_dto import MusicalFeaturesDTO
 from songtradr_api_client_python.models.party_small_dto import PartySmallDTO
-from songtradr_api_client_python.models.recording_for_similarity_search_dto import RecordingForSimilaritySearchDTO
 from songtradr_api_client_python.models.recording_genre_prediction_dto import RecordingGenrePredictionDTO
-from songtradr_api_client_python.models.recording_list_dto import RecordingListDTO
 from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
-from songtradr_api_client_python.models.recording_minimal_with_musical_features_dto import RecordingMinimalWithMusicalFeaturesDTO
 from songtradr_api_client_python.models.recording_minimal_with_taggrams_dto import RecordingMinimalWithTaggramsDTO
 from songtradr_api_client_python.models.recording_minimal_with_tagstrengths_dto import RecordingMinimalWithTagstrengthsDTO
 from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO
-from songtradr_api_client_python.models.recording_small_dto import RecordingSmallDTO
 from songtradr_api_client_python.models.recording_tag_small_dto import RecordingTagSmallDTO
 from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
 from songtradr_api_client_python.models.search_filter_values_dto import SearchFilterValuesDTO
 from songtradr_api_client_python.models.sign_up_dto import SignUpDTO
 from songtradr_api_client_python.models.tag_dto import TagDTO
-from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO
 from songtradr_api_client_python.models.taggram_dto import TaggramDTO
 from songtradr_api_client_python.models.tags_summary_dto import TagsSummaryDTO
 from songtradr_api_client_python.models.tagstrength_dto import TagstrengthDTO
 from songtradr_api_client_python.models.title_dto import TitleDTO
 from songtradr_api_client_python.models.token_request import TokenRequest
 from songtradr_api_client_python.models.track_dto import TrackDTO
 from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api/user_api.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/api/user_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -23,19 +23,17 @@
 from typing_extensions import Annotated
 from songtradr_api_client_python.models.file_list_dto import FileListDTO
 from songtradr_api_client_python.models.file_small_dto import FileSmallDTO
 from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO
 from songtradr_api_client_python.models.file_w_ith_url_dto import FileWIthUrlDTO
 from songtradr_api_client_python.models.files_summary_dto import FilesSummaryDTO
 from songtradr_api_client_python.models.forgot_password_dto import ForgotPasswordDTO
-from songtradr_api_client_python.models.image_recognition_response import ImageRecognitionResponse
 from songtradr_api_client_python.models.init_put_recording_audio_dto import InitPutRecordingAudioDTO
 from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
 from songtradr_api_client_python.models.login_dto import LoginDTO
-from songtradr_api_client_python.models.recording_for_similarity_search_dto import RecordingForSimilaritySearchDTO
 from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
 from songtradr_api_client_python.models.recording_minimal_with_taggrams_dto import RecordingMinimalWithTaggramsDTO
 from songtradr_api_client_python.models.recording_minimal_with_tagstrengths_dto import RecordingMinimalWithTagstrengthsDTO
 from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
 from songtradr_api_client_python.models.sign_up_dto import SignUpDTO
 from songtradr_api_client_python.models.token_request import TokenRequest
 from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO
@@ -1479,298 +1477,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def initiate_user_image_upload(
-        self,
-        name: Annotated[StrictStr, Field(description="The Name of the image that will be uploaded")],
-        url: StrictStr,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ImageRecognitionResponse:
-        """Recognise and upload image. Responds with an object with recognition result.
-
-
-        :param name: The Name of the image that will be uploaded (required)
-        :type name: str
-        :param url: (required)
-        :type url: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._initiate_user_image_upload_serialize(
-            name=name,
-            url=url,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImageRecognitionResponse",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-            '400': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def initiate_user_image_upload_with_http_info(
-        self,
-        name: Annotated[StrictStr, Field(description="The Name of the image that will be uploaded")],
-        url: StrictStr,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ImageRecognitionResponse]:
-        """Recognise and upload image. Responds with an object with recognition result.
-
-
-        :param name: The Name of the image that will be uploaded (required)
-        :type name: str
-        :param url: (required)
-        :type url: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._initiate_user_image_upload_serialize(
-            name=name,
-            url=url,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImageRecognitionResponse",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-            '400': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def initiate_user_image_upload_without_preload_content(
-        self,
-        name: Annotated[StrictStr, Field(description="The Name of the image that will be uploaded")],
-        url: StrictStr,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Recognise and upload image. Responds with an object with recognition result.
-
-
-        :param name: The Name of the image that will be uploaded (required)
-        :type name: str
-        :param url: (required)
-        :type url: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._initiate_user_image_upload_serialize(
-            name=name,
-            url=url,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ImageRecognitionResponse",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-            '400': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _initiate_user_image_upload_serialize(
-        self,
-        name,
-        url,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if name is not None:
-            _path_params['name'] = name
-        # process the query parameters
-        if url is not None:
-            
-            _query_params.append(('url', url))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'bearer-jwt'
-        ]
-
-        return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/api/v1/user/file/{name}/initImageUpload',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def login(
         self,
         login_dto: LoginDTO,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -2292,1363 +2006,14 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def prompt_search_user_files(
-        self,
-        query: Annotated[StrictStr, Field(description="Query.")],
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> FileListDTO:
-        """Files for query.
-
-
-        :param query: Query. (required)
-        :type query: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._prompt_search_user_files_serialize(
-            query=query,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FileListDTO",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def prompt_search_user_files_with_http_info(
-        self,
-        query: Annotated[StrictStr, Field(description="Query.")],
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[FileListDTO]:
-        """Files for query.
-
-
-        :param query: Query. (required)
-        :type query: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._prompt_search_user_files_serialize(
-            query=query,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FileListDTO",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def prompt_search_user_files_without_preload_content(
-        self,
-        query: Annotated[StrictStr, Field(description="Query.")],
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Files for query.
-
-
-        :param query: Query. (required)
-        :type query: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._prompt_search_user_files_serialize(
-            query=query,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FileListDTO",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _prompt_search_user_files_serialize(
-        self,
-        query,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if query is not None:
-            
-            _query_params.append(('query', query))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'bearer-jwt'
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/v1/user/promptSearch',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def recordings_by_folder_with_taggrams(
-        self,
-        folder_name: Annotated[StrictStr, Field(description="Folder name")],
-        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
-        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
-        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
-        from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
-        to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
-        fill_with_zero: Annotated[Optional[StrictBool], Field(description="If set to true, empty timeseries are filled with timeseries of 0.0 values.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
-        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[RecordingMinimalWithTaggramsDTO]:
-        """Timeseries of AI generated moods, musical features and more for recordings in your folder.
-
-
-        :param folder_name: Folder name (required)
-        :type folder_name: str
-        :param category_name: Show only taggrams for one category.
-        :type category_name: str
-        :param tag_name: Show only taggrams for one tag.
-        :type tag_name: str
-        :param genre_name: Show only taggrams for one genre.
-        :type genre_name: str
-        :param from_timestamp: Show only taggrams data starting from from this timestamp in seconds.
-        :type from_timestamp: float
-        :param to_timestamp: Show only taggrams data before this timestamp in seconds.
-        :type to_timestamp: float
-        :param fill_with_zero: If set to true, empty timeseries are filled with timeseries of 0.0 values.
-        :type fill_with_zero: bool
-        :param page: Zero-based page index (0..N)
-        :type page: int
-        :param size: The size of the page to be returned
-        :type size: int
-        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
-        :type sort: List[str]
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_folder_with_taggrams_serialize(
-            folder_name=folder_name,
-            category_name=category_name,
-            tag_name=tag_name,
-            genre_name=genre_name,
-            from_timestamp=from_timestamp,
-            to_timestamp=to_timestamp,
-            fill_with_zero=fill_with_zero,
-            page=page,
-            size=size,
-            sort=sort,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingMinimalWithTaggramsDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def recordings_by_folder_with_taggrams_with_http_info(
-        self,
-        folder_name: Annotated[StrictStr, Field(description="Folder name")],
-        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
-        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
-        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
-        from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
-        to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
-        fill_with_zero: Annotated[Optional[StrictBool], Field(description="If set to true, empty timeseries are filled with timeseries of 0.0 values.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
-        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[RecordingMinimalWithTaggramsDTO]]:
-        """Timeseries of AI generated moods, musical features and more for recordings in your folder.
-
-
-        :param folder_name: Folder name (required)
-        :type folder_name: str
-        :param category_name: Show only taggrams for one category.
-        :type category_name: str
-        :param tag_name: Show only taggrams for one tag.
-        :type tag_name: str
-        :param genre_name: Show only taggrams for one genre.
-        :type genre_name: str
-        :param from_timestamp: Show only taggrams data starting from from this timestamp in seconds.
-        :type from_timestamp: float
-        :param to_timestamp: Show only taggrams data before this timestamp in seconds.
-        :type to_timestamp: float
-        :param fill_with_zero: If set to true, empty timeseries are filled with timeseries of 0.0 values.
-        :type fill_with_zero: bool
-        :param page: Zero-based page index (0..N)
-        :type page: int
-        :param size: The size of the page to be returned
-        :type size: int
-        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
-        :type sort: List[str]
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_folder_with_taggrams_serialize(
-            folder_name=folder_name,
-            category_name=category_name,
-            tag_name=tag_name,
-            genre_name=genre_name,
-            from_timestamp=from_timestamp,
-            to_timestamp=to_timestamp,
-            fill_with_zero=fill_with_zero,
-            page=page,
-            size=size,
-            sort=sort,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingMinimalWithTaggramsDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def recordings_by_folder_with_taggrams_without_preload_content(
-        self,
-        folder_name: Annotated[StrictStr, Field(description="Folder name")],
-        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
-        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
-        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
-        from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
-        to_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data before this timestamp in seconds.")] = None,
-        fill_with_zero: Annotated[Optional[StrictBool], Field(description="If set to true, empty timeseries are filled with timeseries of 0.0 values.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
-        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Timeseries of AI generated moods, musical features and more for recordings in your folder.
-
-
-        :param folder_name: Folder name (required)
-        :type folder_name: str
-        :param category_name: Show only taggrams for one category.
-        :type category_name: str
-        :param tag_name: Show only taggrams for one tag.
-        :type tag_name: str
-        :param genre_name: Show only taggrams for one genre.
-        :type genre_name: str
-        :param from_timestamp: Show only taggrams data starting from from this timestamp in seconds.
-        :type from_timestamp: float
-        :param to_timestamp: Show only taggrams data before this timestamp in seconds.
-        :type to_timestamp: float
-        :param fill_with_zero: If set to true, empty timeseries are filled with timeseries of 0.0 values.
-        :type fill_with_zero: bool
-        :param page: Zero-based page index (0..N)
-        :type page: int
-        :param size: The size of the page to be returned
-        :type size: int
-        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
-        :type sort: List[str]
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_folder_with_taggrams_serialize(
-            folder_name=folder_name,
-            category_name=category_name,
-            tag_name=tag_name,
-            genre_name=genre_name,
-            from_timestamp=from_timestamp,
-            to_timestamp=to_timestamp,
-            fill_with_zero=fill_with_zero,
-            page=page,
-            size=size,
-            sort=sort,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingMinimalWithTaggramsDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _recordings_by_folder_with_taggrams_serialize(
-        self,
-        folder_name,
-        category_name,
-        tag_name,
-        genre_name,
-        from_timestamp,
-        to_timestamp,
-        fill_with_zero,
-        page,
-        size,
-        sort,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-            'sort': 'multi',
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if folder_name is not None:
-            _path_params['folderName'] = folder_name
-        # process the query parameters
-        if category_name is not None:
-            
-            _query_params.append(('categoryName', category_name))
-            
-        if tag_name is not None:
-            
-            _query_params.append(('tagName', tag_name))
-            
-        if genre_name is not None:
-            
-            _query_params.append(('genreName', genre_name))
-            
-        if from_timestamp is not None:
-            
-            _query_params.append(('fromTimestamp', from_timestamp))
-            
-        if to_timestamp is not None:
-            
-            _query_params.append(('toTimestamp', to_timestamp))
-            
-        if fill_with_zero is not None:
-            
-            _query_params.append(('fillWithZero', fill_with_zero))
-            
-        if page is not None:
-            
-            _query_params.append(('page', page))
-            
-        if size is not None:
-            
-            _query_params.append(('size', size))
-            
-        if sort is not None:
-            
-            _query_params.append(('sort', sort))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'bearer-jwt'
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/v1/user/folder/{folderName}/taggrams',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def recordings_by_folder_with_tagstrengths(
-        self,
-        folder_name: Annotated[StrictStr, Field(description="Folder name")],
-        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
-        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
-        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
-        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[RecordingMinimalWithTagstrengthsDTO]:
-        """Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
-
-
-        :param folder_name: Folder name (required)
-        :type folder_name: str
-        :param category_name: Show only taggrams for one category.
-        :type category_name: str
-        :param tag_name: Show only taggrams for one tag.
-        :type tag_name: str
-        :param genre_name: Show only taggrams for one genre.
-        :type genre_name: str
-        :param page: Zero-based page index (0..N)
-        :type page: int
-        :param size: The size of the page to be returned
-        :type size: int
-        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
-        :type sort: List[str]
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_folder_with_tagstrengths_serialize(
-            folder_name=folder_name,
-            category_name=category_name,
-            tag_name=tag_name,
-            genre_name=genre_name,
-            page=page,
-            size=size,
-            sort=sort,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingMinimalWithTagstrengthsDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def recordings_by_folder_with_tagstrengths_with_http_info(
-        self,
-        folder_name: Annotated[StrictStr, Field(description="Folder name")],
-        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
-        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
-        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
-        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[RecordingMinimalWithTagstrengthsDTO]]:
-        """Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
-
-
-        :param folder_name: Folder name (required)
-        :type folder_name: str
-        :param category_name: Show only taggrams for one category.
-        :type category_name: str
-        :param tag_name: Show only taggrams for one tag.
-        :type tag_name: str
-        :param genre_name: Show only taggrams for one genre.
-        :type genre_name: str
-        :param page: Zero-based page index (0..N)
-        :type page: int
-        :param size: The size of the page to be returned
-        :type size: int
-        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
-        :type sort: List[str]
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_folder_with_tagstrengths_serialize(
-            folder_name=folder_name,
-            category_name=category_name,
-            tag_name=tag_name,
-            genre_name=genre_name,
-            page=page,
-            size=size,
-            sort=sort,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingMinimalWithTagstrengthsDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def recordings_by_folder_with_tagstrengths_without_preload_content(
-        self,
-        folder_name: Annotated[StrictStr, Field(description="Folder name")],
-        category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
-        tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
-        genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None,
-        size: Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
-
-
-        :param folder_name: Folder name (required)
-        :type folder_name: str
-        :param category_name: Show only taggrams for one category.
-        :type category_name: str
-        :param tag_name: Show only taggrams for one tag.
-        :type tag_name: str
-        :param genre_name: Show only taggrams for one genre.
-        :type genre_name: str
-        :param page: Zero-based page index (0..N)
-        :type page: int
-        :param size: The size of the page to be returned
-        :type size: int
-        :param sort: Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
-        :type sort: List[str]
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_folder_with_tagstrengths_serialize(
-            folder_name=folder_name,
-            category_name=category_name,
-            tag_name=tag_name,
-            genre_name=genre_name,
-            page=page,
-            size=size,
-            sort=sort,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingMinimalWithTagstrengthsDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _recordings_by_folder_with_tagstrengths_serialize(
-        self,
-        folder_name,
-        category_name,
-        tag_name,
-        genre_name,
-        page,
-        size,
-        sort,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-            'sort': 'multi',
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if folder_name is not None:
-            _path_params['folderName'] = folder_name
-        # process the query parameters
-        if category_name is not None:
-            
-            _query_params.append(('categoryName', category_name))
-            
-        if tag_name is not None:
-            
-            _query_params.append(('tagName', tag_name))
-            
-        if genre_name is not None:
-            
-            _query_params.append(('genreName', genre_name))
-            
-        if page is not None:
-            
-            _query_params.append(('page', page))
-            
-        if size is not None:
-            
-            _query_params.append(('size', size))
-            
-        if sort is not None:
-            
-            _query_params.append(('sort', sort))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'bearer-jwt'
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/v1/user/folder/{folderName}/tagstrengths',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def recordings_by_ids_with_similarities(
-        self,
-        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
-        identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
-        usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[RecordingForSimilaritySearchDTO]:
-        """Similar recordings for a list of user recordings.
-
-
-        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
-        :type ids: str
-        :param identical_only: Whether a result list shall include only identical recordings.
-        :type identical_only: bool
-        :param usage: Filter by recording usage.
-        :type usage: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_ids_with_similarities_serialize(
-            ids=ids,
-            identical_only=identical_only,
-            usage=usage,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingForSimilaritySearchDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def recordings_by_ids_with_similarities_with_http_info(
-        self,
-        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
-        identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
-        usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[RecordingForSimilaritySearchDTO]]:
-        """Similar recordings for a list of user recordings.
-
-
-        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
-        :type ids: str
-        :param identical_only: Whether a result list shall include only identical recordings.
-        :type identical_only: bool
-        :param usage: Filter by recording usage.
-        :type usage: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_ids_with_similarities_serialize(
-            ids=ids,
-            identical_only=identical_only,
-            usage=usage,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingForSimilaritySearchDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def recordings_by_ids_with_similarities_without_preload_content(
-        self,
-        ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
-        identical_only: Annotated[Optional[StrictBool], Field(description="Whether a result list shall include only identical recordings.")] = None,
-        usage: Annotated[Optional[StrictStr], Field(description="Filter by recording usage.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Similar recordings for a list of user recordings.
-
-
-        :param ids: Comma seperated list of IDs. Can be ISRCs or proprietary IDs (required)
-        :type ids: str
-        :param identical_only: Whether a result list shall include only identical recordings.
-        :type identical_only: bool
-        :param usage: Filter by recording usage.
-        :type usage: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._recordings_by_ids_with_similarities_serialize(
-            ids=ids,
-            identical_only=identical_only,
-            usage=usage,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[RecordingForSimilaritySearchDTO]",
-            '401': "ErrorResponse",
-            '429': "ErrorResponse",
-            '500': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _recordings_by_ids_with_similarities_serialize(
-        self,
-        ids,
-        identical_only,
-        usage,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        if ids is not None:
-            _path_params['ids'] = ids
-        # process the query parameters
-        if identical_only is not None:
-            
-            _query_params.append(('identicalOnly', identical_only))
-            
-        if usage is not None:
-            
-            _query_params.append(('usage', usage))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'bearer-jwt'
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/v1/user/recording/{ids}/similarities',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def recordings_by_ids_with_taggrams(
         self,
         ids: Annotated[StrictStr, Field(description="Comma seperated list of IDs. Can be ISRCs or proprietary IDs")],
         category_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one category.")] = None,
         tag_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one tag.")] = None,
         genre_name: Annotated[Optional[StrictStr], Field(description="Show only taggrams for one genre.")] = None,
         from_timestamp: Annotated[Optional[Union[StrictFloat, StrictInt]], Field(description="Show only taggrams data starting from from this timestamp in seconds.")] = None,
@@ -4690,17 +3055,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '403': "ErrorResponse",
             '200': "SignUpDTO",
             '409': "ErrorResponse",
-            '403': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -4762,17 +3127,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '403': "ErrorResponse",
             '200': "SignUpDTO",
             '409': "ErrorResponse",
-            '403': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -4834,17 +3199,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '403': "ErrorResponse",
             '200': "SignUpDTO",
             '409': "ErrorResponse",
-            '403': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -4976,16 +3341,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "JwtTokenDTO",
             '401': "ErrorResponse",
+            '200': "JwtTokenDTO",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -5046,16 +3411,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "JwtTokenDTO",
             '401': "ErrorResponse",
+            '200': "JwtTokenDTO",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -5116,16 +3481,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "JwtTokenDTO",
             '401': "ErrorResponse",
+            '200': "JwtTokenDTO",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -5537,16 +3902,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FileWIthUrlDTO",
             '400': "ErrorResponse",
+            '200': "FileWIthUrlDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -5607,16 +3972,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FileWIthUrlDTO",
             '400': "ErrorResponse",
+            '200': "FileWIthUrlDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -5677,16 +4042,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "FileWIthUrlDTO",
             '400': "ErrorResponse",
+            '200': "FileWIthUrlDTO",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
@@ -5801,15 +4166,14 @@
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
         pretzel_station_suitability: Optional[StrictStr] = None,
-        similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
         extension: Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None,
@@ -5927,16 +4291,14 @@
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
         :param pretzel_station_suitability:
         :type pretzel_station_suitability: str
-        :param similar_to_recording:
-        :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
         :type bpm_min: int
         :param bpm_max: Search for a maximal bpm.
@@ -6029,15 +4391,14 @@
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             pretzel_station_suitability=pretzel_station_suitability,
-            similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
             extension=extension,
@@ -6118,15 +4479,14 @@
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
         pretzel_station_suitability: Optional[StrictStr] = None,
-        similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
         extension: Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None,
@@ -6244,16 +4604,14 @@
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
         :param pretzel_station_suitability:
         :type pretzel_station_suitability: str
-        :param similar_to_recording:
-        :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
         :type bpm_min: int
         :param bpm_max: Search for a maximal bpm.
@@ -6346,15 +4704,14 @@
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             pretzel_station_suitability=pretzel_station_suitability,
-            similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
             extension=extension,
@@ -6435,15 +4792,14 @@
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
         pretzel_station_suitability: Optional[StrictStr] = None,
-        similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
         extension: Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None,
@@ -6561,16 +4917,14 @@
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
         :param pretzel_station_suitability:
         :type pretzel_station_suitability: str
-        :param similar_to_recording:
-        :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
         :type bpm_min: int
         :param bpm_max: Search for a maximal bpm.
@@ -6663,15 +5017,14 @@
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             pretzel_station_suitability=pretzel_station_suitability,
-            similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
             extension=extension,
@@ -6747,15 +5100,14 @@
         audience_region,
         audience_gender,
         origin_decade,
         curateability,
         use_case,
         channel_suitability,
         pretzel_station_suitability,
-        similar_to_recording,
         songtradr_track_id,
         usage_name,
         bpm_min,
         bpm_max,
         name,
         folder,
         extension,
@@ -6983,18 +5335,14 @@
             
             _query_params.append(('channelSuitability', channel_suitability))
             
         if pretzel_station_suitability is not None:
             
             _query_params.append(('pretzelStationSuitability', pretzel_station_suitability))
             
-        if similar_to_recording is not None:
-            
-            _query_params.append(('similarToRecording', similar_to_recording))
-            
         if songtradr_track_id is not None:
             
             _query_params.append(('songtradrTrackId', songtradr_track_id))
             
         if usage_name is not None:
             
             _query_params.append(('usageName', usage_name))
@@ -7428,15 +5776,14 @@
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
         pretzel_station_suitability: Optional[StrictStr] = None,
-        similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
         extension: Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None,
@@ -7549,16 +5896,14 @@
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
         :param pretzel_station_suitability:
         :type pretzel_station_suitability: str
-        :param similar_to_recording:
-        :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
         :type bpm_min: int
         :param bpm_max: Search for a maximal bpm.
@@ -7644,15 +5989,14 @@
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             pretzel_station_suitability=pretzel_station_suitability,
-            similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
             extension=extension,
@@ -7729,15 +6073,14 @@
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
         pretzel_station_suitability: Optional[StrictStr] = None,
-        similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
         extension: Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None,
@@ -7850,16 +6193,14 @@
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
         :param pretzel_station_suitability:
         :type pretzel_station_suitability: str
-        :param similar_to_recording:
-        :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
         :type bpm_min: int
         :param bpm_max: Search for a maximal bpm.
@@ -7945,15 +6286,14 @@
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             pretzel_station_suitability=pretzel_station_suitability,
-            similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
             extension=extension,
@@ -8030,15 +6370,14 @@
         audience_region: Optional[StrictStr] = None,
         audience_gender: Optional[StrictStr] = None,
         origin_decade: Optional[StrictStr] = None,
         curateability: Optional[StrictStr] = None,
         use_case: Optional[StrictStr] = None,
         channel_suitability: Optional[StrictStr] = None,
         pretzel_station_suitability: Optional[StrictStr] = None,
-        similar_to_recording: Optional[StrictStr] = None,
         songtradr_track_id: Optional[StrictStr] = None,
         usage_name: Optional[StrictStr] = None,
         bpm_min: Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None,
         bpm_max: Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None,
         name: Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None,
         folder: Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None,
         extension: Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None,
@@ -8151,16 +6490,14 @@
         :type curateability: str
         :param use_case:
         :type use_case: str
         :param channel_suitability:
         :type channel_suitability: str
         :param pretzel_station_suitability:
         :type pretzel_station_suitability: str
-        :param similar_to_recording:
-        :type similar_to_recording: str
         :param songtradr_track_id:
         :type songtradr_track_id: str
         :param usage_name:
         :type usage_name: str
         :param bpm_min: Search for a minimal bpm.
         :type bpm_min: int
         :param bpm_max: Search for a maximal bpm.
@@ -8246,15 +6583,14 @@
             audience_region=audience_region,
             audience_gender=audience_gender,
             origin_decade=origin_decade,
             curateability=curateability,
             use_case=use_case,
             channel_suitability=channel_suitability,
             pretzel_station_suitability=pretzel_station_suitability,
-            similar_to_recording=similar_to_recording,
             songtradr_track_id=songtradr_track_id,
             usage_name=usage_name,
             bpm_min=bpm_min,
             bpm_max=bpm_max,
             name=name,
             folder=folder,
             extension=extension,
@@ -8326,15 +6662,14 @@
         audience_region,
         audience_gender,
         origin_decade,
         curateability,
         use_case,
         channel_suitability,
         pretzel_station_suitability,
-        similar_to_recording,
         songtradr_track_id,
         usage_name,
         bpm_min,
         bpm_max,
         name,
         folder,
         extension,
@@ -8554,18 +6889,14 @@
             
             _query_params.append(('channelSuitability', channel_suitability))
             
         if pretzel_station_suitability is not None:
             
             _query_params.append(('pretzelStationSuitability', pretzel_station_suitability))
             
-        if similar_to_recording is not None:
-            
-            _query_params.append(('similarToRecording', similar_to_recording))
-            
         if songtradr_track_id is not None:
             
             _query_params.append(('songtradrTrackId', songtradr_track_id))
             
         if usage_name is not None:
             
             _query_params.append(('usageName', usage_name))
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_client.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -85,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.1.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.0.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/api_response.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/api_response.py`

 * *Files identical despite different names*

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/configuration.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -375,16 +375,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.1.0\n"\
-               "SDK Package Version: 2.1.0".\
+               "Version of the API: 3.0.0\n"\
+               "SDK Package Version: 3.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/exceptions.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/__init__.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 
 # flake8: noqa
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
-from songtradr_api_client_python.models.category_medium_dto import CategoryMediumDTO
 from songtradr_api_client_python.models.category_minimal_dto import CategoryMinimalDTO
 from songtradr_api_client_python.models.config_access_dto import ConfigAccessDTO
 from songtradr_api_client_python.models.config_identifier_dto import ConfigIdentifierDTO
 from songtradr_api_client_python.models.contributor_type_dto import ContributorTypeDTO
 from songtradr_api_client_python.models.error_response import ErrorResponse
 from songtradr_api_client_python.models.field_summary_dto import FieldSummaryDTO
 from songtradr_api_client_python.models.file_dto import FileDTO
@@ -28,35 +27,29 @@
 from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO
 from songtradr_api_client_python.models.file_w_ith_url_dto import FileWIthUrlDTO
 from songtradr_api_client_python.models.files_summary_dto import FilesSummaryDTO
 from songtradr_api_client_python.models.forgot_password_dto import ForgotPasswordDTO
 from songtradr_api_client_python.models.genre_dto import GenreDTO
 from songtradr_api_client_python.models.genre_minimal_dto import GenreMinimalDTO
 from songtradr_api_client_python.models.genres_summary_dto import GenresSummaryDTO
-from songtradr_api_client_python.models.image_recognition_response import ImageRecognitionResponse
 from songtradr_api_client_python.models.init_put_recording_audio_dto import InitPutRecordingAudioDTO
 from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
 from songtradr_api_client_python.models.login_dto import LoginDTO
 from songtradr_api_client_python.models.musical_features_dto import MusicalFeaturesDTO
 from songtradr_api_client_python.models.party_small_dto import PartySmallDTO
-from songtradr_api_client_python.models.recording_for_similarity_search_dto import RecordingForSimilaritySearchDTO
 from songtradr_api_client_python.models.recording_genre_prediction_dto import RecordingGenrePredictionDTO
-from songtradr_api_client_python.models.recording_list_dto import RecordingListDTO
 from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
-from songtradr_api_client_python.models.recording_minimal_with_musical_features_dto import RecordingMinimalWithMusicalFeaturesDTO
 from songtradr_api_client_python.models.recording_minimal_with_taggrams_dto import RecordingMinimalWithTaggramsDTO
 from songtradr_api_client_python.models.recording_minimal_with_tagstrengths_dto import RecordingMinimalWithTagstrengthsDTO
 from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO
-from songtradr_api_client_python.models.recording_small_dto import RecordingSmallDTO
 from songtradr_api_client_python.models.recording_tag_small_dto import RecordingTagSmallDTO
 from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
 from songtradr_api_client_python.models.search_filter_values_dto import SearchFilterValuesDTO
 from songtradr_api_client_python.models.sign_up_dto import SignUpDTO
 from songtradr_api_client_python.models.tag_dto import TagDTO
-from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO
 from songtradr_api_client_python.models.taggram_dto import TaggramDTO
 from songtradr_api_client_python.models.tags_summary_dto import TagsSummaryDTO
 from songtradr_api_client_python.models.tagstrength_dto import TagstrengthDTO
 from songtradr_api_client_python.models.title_dto import TitleDTO
 from songtradr_api_client_python.models.token_request import TokenRequest
 from songtradr_api_client_python.models.track_dto import TrackDTO
 from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_medium_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_tag_small_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List
+from songtradr_api_client_python.models.tag_dto import TagDTO
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CategoryMediumDTO(BaseModel):
+class RecordingTagSmallDTO(BaseModel):
     """
-    A category of tags with its underlying tags.
+    Tag information in with a small field-set.
     """ # noqa: E501
-    id: StrictInt
-    name: StrictStr
-    tags: Optional[List[TagSmallDTO]] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "tags"]
+    tag: TagDTO
+    __properties: ClassVar[List[str]] = ["tag"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CategoryMediumDTO from a JSON string"""
+        """Create an instance of RecordingTagSmallDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,33 +66,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
-        _items = []
-        if self.tags:
-            for _item in self.tags:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tags'] = _items
+        # override the default output from pydantic by calling `to_dict()` of tag
+        if self.tag:
+            _dict['tag'] = self.tag.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CategoryMediumDTO from a dict"""
+        """Create an instance of RecordingTagSmallDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "name": obj.get("name"),
-            "tags": [TagSmallDTO.from_dict(_item) for _item in obj["tags"]] if obj.get("tags") is not None else None
+            "tag": TagDTO.from_dict(obj["tag"]) if obj.get("tag") is not None else None
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/category_minimal_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/category_minimal_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_access_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/config_access_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/config_identifier_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/config_identifier_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/contributor_type_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/contributor_type_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/error_response.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/field_summary_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/field_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_list_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_list_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_small_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -29,25 +29,25 @@
     Reduced details on a file that has been uploaded for auto-tagging or audio-recognition purposes.
     """ # noqa: E501
     folder: StrictStr
     name: StrictStr
     id: StrictInt
     extension: StrictStr = Field(description="extension of the file")
     error_message: Optional[StrictStr] = None
-    fingerprint_status: Optional[StrictStr] = Field(default=None, description="status of the audio recognition", alias="fingerprintStatus")
-    object_key: StrictStr = Field(alias="objectKey")
     upload_start_time: Optional[datetime] = Field(default=None, alias="uploadStartTime")
     upload_end_time: Optional[datetime] = Field(default=None, alias="uploadEndTime")
+    fingerprint_status: Optional[StrictStr] = Field(default=None, description="status of the audio recognition", alias="fingerprintStatus")
     fingerprint_start_time: Optional[datetime] = Field(default=None, alias="fingerprintStartTime")
     fingerprint_end_time: Optional[datetime] = Field(default=None, alias="fingerprintEndTime")
     inference_status: Optional[StrictStr] = Field(default=None, description="status of the auto-tagging", alias="inferenceStatus")
     inference_start_time: Optional[datetime] = Field(default=None, alias="inferenceStartTime")
     inference_end_time: Optional[datetime] = Field(default=None, alias="inferenceEndTime")
+    object_key: StrictStr = Field(alias="objectKey")
     error_time: Optional[datetime] = None
-    __properties: ClassVar[List[str]] = ["folder", "name", "id", "extension", "error_message", "fingerprintStatus", "objectKey", "uploadStartTime", "uploadEndTime", "fingerprintStartTime", "fingerprintEndTime", "inferenceStatus", "inferenceStartTime", "inferenceEndTime", "error_time"]
+    __properties: ClassVar[List[str]] = ["folder", "name", "id", "extension", "error_message", "uploadStartTime", "uploadEndTime", "fingerprintStatus", "fingerprintStartTime", "fingerprintEndTime", "inferenceStatus", "inferenceStartTime", "inferenceEndTime", "objectKey", "error_time"]
 
     @field_validator('extension')
     def extension_validate_enum(cls, value):
         """Validates the enum"""
         if value not in set(['mp3', 'wav', 'flac']):
             raise ValueError("must be one of enum values ('mp3', 'wav', 'flac')")
         return value
@@ -124,21 +124,21 @@
 
         _obj = cls.model_validate({
             "folder": obj.get("folder"),
             "name": obj.get("name"),
             "id": obj.get("id"),
             "extension": obj.get("extension"),
             "error_message": obj.get("error_message"),
-            "fingerprintStatus": obj.get("fingerprintStatus"),
-            "objectKey": obj.get("objectKey"),
             "uploadStartTime": obj.get("uploadStartTime"),
             "uploadEndTime": obj.get("uploadEndTime"),
+            "fingerprintStatus": obj.get("fingerprintStatus"),
             "fingerprintStartTime": obj.get("fingerprintStartTime"),
             "fingerprintEndTime": obj.get("fingerprintEndTime"),
             "inferenceStatus": obj.get("inferenceStatus"),
             "inferenceStartTime": obj.get("inferenceStartTime"),
             "inferenceEndTime": obj.get("inferenceEndTime"),
+            "objectKey": obj.get("objectKey"),
             "error_time": obj.get("error_time")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_upload_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_upload_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/file_w_ith_url_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/file_w_ith_url_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/files_summary_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/files_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/forgot_password_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/forgot_password_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/genre_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genre_minimal_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/genre_minimal_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/genres_summary_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/genres_summary_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/image_recognition_response.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/video_recognition_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,17 +19,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ImageRecognitionResponse(BaseModel):
+class VideoRecognitionResponse(BaseModel):
     """
-    ImageRecognitionResponse
+    VideoRecognitionResponse
     """ # noqa: E501
     labels: Optional[List[Dict[str, Any]]] = None
     faces: Optional[List[Dict[str, Any]]] = None
     __properties: ClassVar[List[str]] = ["labels", "faces"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ImageRecognitionResponse from a JSON string"""
+        """Create an instance of VideoRecognitionResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ImageRecognitionResponse from a dict"""
+        """Create an instance of VideoRecognitionResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/init_put_recording_audio_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/jwt_token_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/jwt_token_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/login_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/login_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/musical_features_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,30 +24,14 @@
 from typing_extensions import Self
 
 class MusicalFeaturesDTO(BaseModel):
     """
     AI generated musical features of a recording.
     """ # noqa: E501
     space: Optional[StrictStr] = Field(default=None, description="Search for space")
-    valence_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="valenceAffinity")
-    tempo_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="tempoAffinity")
-    scale_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="scaleAffinity")
-    timbre_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="timbreAffinity")
-    roughness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="roughnessAffinity")
-    harmony_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="harmonyAffinity")
-    texture_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="textureAffinity")
-    groovyness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="groovynessAffinity")
-    space_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="spaceAffinity")
-    loudness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="loudnessAffinity")
-    key_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="keyAffinity")
-    channel_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="channelSuitabilityAffinity")
-    arousal_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="arousalAffinity")
-    pleasantness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="pleasantnessAffinity")
-    engagement_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="engagementAffinity")
-    energy_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="energyAffinity")
     language_of_performance: Optional[StrictStr] = Field(default=None, alias="languageOfPerformance")
     arousal: Optional[StrictStr] = Field(default=None, description="Search for an arousal")
     dominant_instrument: Optional[StrictStr] = Field(default=None, description="Search for a dominant instrument", alias="dominantInstrument")
     energy: Optional[StrictStr] = Field(default=None, description="Search for energy")
     engagement: Optional[StrictStr] = Field(default=None, description="Search for an engagement")
     groovyness: Optional[StrictStr] = Field(default=None, description="Search for groovyness")
     harmony: Optional[StrictStr] = Field(default=None, description="Search for a degree of harmoniousness")
@@ -112,15 +96,31 @@
     language_of_performance_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="languageOfPerformanceAffinity")
     curateability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="curateabilityAffinity")
     use_case_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="useCaseAffinity")
     industry_suitability: Optional[StrictStr] = Field(default=None, description="Search for Industry suitability", alias="industrySuitability")
     industry_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="industrySuitabilityAffinity")
     pretzel_station_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="pretzelStationSuitabilityAffinity")
     audience_region: Optional[StrictStr] = Field(default=None, alias="audienceRegion")
-    __properties: ClassVar[List[str]] = ["space", "valenceAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "loudnessAffinity", "keyAffinity", "channelSuitabilityAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "languageOfPerformance", "arousal", "dominantInstrument", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "primarySoundCharacter", "rhythm", "roughness", "scale", "key", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "curateability", "useCase", "channelSuitability", "pretzelStationSuitability", "loudness", "bpm", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "primarySoundCharacterAffinity", "tonalityAffinity", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "pretzelStationSuitabilityAffinity", "audienceRegion"]
+    valence_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="valenceAffinity")
+    arousal_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="arousalAffinity")
+    pleasantness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="pleasantnessAffinity")
+    engagement_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="engagementAffinity")
+    energy_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="energyAffinity")
+    tempo_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="tempoAffinity")
+    scale_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="scaleAffinity")
+    timbre_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="timbreAffinity")
+    roughness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="roughnessAffinity")
+    harmony_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="harmonyAffinity")
+    texture_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="textureAffinity")
+    groovyness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="groovynessAffinity")
+    space_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="spaceAffinity")
+    loudness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="loudnessAffinity")
+    key_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="keyAffinity")
+    channel_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, alias="channelSuitabilityAffinity")
+    __properties: ClassVar[List[str]] = ["space", "languageOfPerformance", "arousal", "dominantInstrument", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "primarySoundCharacter", "rhythm", "roughness", "scale", "key", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "curateability", "useCase", "channelSuitability", "pretzelStationSuitability", "loudness", "bpm", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "primarySoundCharacterAffinity", "tonalityAffinity", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "pretzelStationSuitabilityAffinity", "audienceRegion", "valenceAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "loudnessAffinity", "keyAffinity", "channelSuitabilityAffinity"]
 
     @field_validator('space')
     def space_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -606,30 +606,14 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "space": obj.get("space"),
-            "valenceAffinity": obj.get("valenceAffinity"),
-            "tempoAffinity": obj.get("tempoAffinity"),
-            "scaleAffinity": obj.get("scaleAffinity"),
-            "timbreAffinity": obj.get("timbreAffinity"),
-            "roughnessAffinity": obj.get("roughnessAffinity"),
-            "harmonyAffinity": obj.get("harmonyAffinity"),
-            "textureAffinity": obj.get("textureAffinity"),
-            "groovynessAffinity": obj.get("groovynessAffinity"),
-            "spaceAffinity": obj.get("spaceAffinity"),
-            "loudnessAffinity": obj.get("loudnessAffinity"),
-            "keyAffinity": obj.get("keyAffinity"),
-            "channelSuitabilityAffinity": obj.get("channelSuitabilityAffinity"),
-            "arousalAffinity": obj.get("arousalAffinity"),
-            "pleasantnessAffinity": obj.get("pleasantnessAffinity"),
-            "engagementAffinity": obj.get("engagementAffinity"),
-            "energyAffinity": obj.get("energyAffinity"),
             "languageOfPerformance": obj.get("languageOfPerformance"),
             "arousal": obj.get("arousal"),
             "dominantInstrument": obj.get("dominantInstrument"),
             "energy": obj.get("energy"),
             "engagement": obj.get("engagement"),
             "groovyness": obj.get("groovyness"),
             "harmony": obj.get("harmony"),
@@ -693,12 +677,28 @@
             "originDecadeAffinity": obj.get("originDecadeAffinity"),
             "languageOfPerformanceAffinity": obj.get("languageOfPerformanceAffinity"),
             "curateabilityAffinity": obj.get("curateabilityAffinity"),
             "useCaseAffinity": obj.get("useCaseAffinity"),
             "industrySuitability": obj.get("industrySuitability"),
             "industrySuitabilityAffinity": obj.get("industrySuitabilityAffinity"),
             "pretzelStationSuitabilityAffinity": obj.get("pretzelStationSuitabilityAffinity"),
-            "audienceRegion": obj.get("audienceRegion")
+            "audienceRegion": obj.get("audienceRegion"),
+            "valenceAffinity": obj.get("valenceAffinity"),
+            "arousalAffinity": obj.get("arousalAffinity"),
+            "pleasantnessAffinity": obj.get("pleasantnessAffinity"),
+            "engagementAffinity": obj.get("engagementAffinity"),
+            "energyAffinity": obj.get("energyAffinity"),
+            "tempoAffinity": obj.get("tempoAffinity"),
+            "scaleAffinity": obj.get("scaleAffinity"),
+            "timbreAffinity": obj.get("timbreAffinity"),
+            "roughnessAffinity": obj.get("roughnessAffinity"),
+            "harmonyAffinity": obj.get("harmonyAffinity"),
+            "textureAffinity": obj.get("textureAffinity"),
+            "groovynessAffinity": obj.get("groovynessAffinity"),
+            "spaceAffinity": obj.get("spaceAffinity"),
+            "loudnessAffinity": obj.get("loudnessAffinity"),
+            "keyAffinity": obj.get("keyAffinity"),
+            "channelSuitabilityAffinity": obj.get("channelSuitabilityAffinity")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/party_small_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/party_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_for_similarity_search_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictFloat, StrictInt
-from typing import Any, ClassVar, Dict, List, Union
-from songtradr_api_client_python.models.recording_small_dto import RecordingSmallDTO
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from songtradr_api_client_python.models.tagstrength_dto import TagstrengthDTO
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RecordingForSimilaritySearchDTO(BaseModel):
+class RecordingMinimalWithTagstrengthsDTO(BaseModel):
     """
-    List of recordings with with a mid-sized field set.
+    Recording in its minimal form, but with AI-predicted musical features.
     """ # noqa: E501
-    recording: RecordingSmallDTO
-    score: Union[StrictFloat, StrictInt]
-    __properties: ClassVar[List[str]] = ["recording", "score"]
+    isrc: StrictStr
+    tagstrengths: Optional[List[TagstrengthDTO]] = None
+    __properties: ClassVar[List[str]] = ["isrc", "tagstrengths"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecordingForSimilaritySearchDTO from a JSON string"""
+        """Create an instance of RecordingMinimalWithTagstrengthsDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,28 +67,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of recording
-        if self.recording:
-            _dict['recording'] = self.recording.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in tagstrengths (list)
+        _items = []
+        if self.tagstrengths:
+            for _item in self.tagstrengths:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tagstrengths'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecordingForSimilaritySearchDTO from a dict"""
+        """Create an instance of RecordingMinimalWithTagstrengthsDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "recording": RecordingSmallDTO.from_dict(obj["recording"]) if obj.get("recording") is not None else None,
-            "score": obj.get("score")
+            "isrc": obj.get("isrc"),
+            "tagstrengths": [TagstrengthDTO.from_dict(_item) for _item in obj["tagstrengths"]] if obj.get("tagstrengths") is not None else None
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_genre_prediction_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_list_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/tags_summary_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt
-from typing import Any, ClassVar, Dict, List
-from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from songtradr_api_client_python.models.category_minimal_dto import CategoryMinimalDTO
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RecordingListDTO(BaseModel):
+class TagsSummaryDTO(BaseModel):
     """
-    List of recordings with with a mid-sized field set.
+    Summary of tags occuring in files.
     """ # noqa: E501
-    recordings: List[RecordingMediumDTO]
-    has_next_page: StrictBool = Field(alias="hasNextPage")
-    current_page_number: StrictInt = Field(alias="currentPageNumber")
-    total_results: StrictInt = Field(alias="totalResults")
-    __properties: ClassVar[List[str]] = ["recordings", "hasNextPage", "currentPageNumber", "totalResults"]
+    name: StrictStr
+    categories: Optional[List[CategoryMinimalDTO]] = None
+    total: StrictInt
+    __properties: ClassVar[List[str]] = ["name", "categories", "total"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecordingListDTO from a JSON string"""
+        """Create an instance of TagsSummaryDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,34 +68,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in recordings (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in categories (list)
         _items = []
-        if self.recordings:
-            for _item in self.recordings:
+        if self.categories:
+            for _item in self.categories:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['recordings'] = _items
+            _dict['categories'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecordingListDTO from a dict"""
+        """Create an instance of TagsSummaryDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "recordings": [RecordingMediumDTO.from_dict(_item) for _item in obj["recordings"]] if obj.get("recordings") is not None else None,
-            "hasNextPage": obj.get("hasNextPage"),
-            "currentPageNumber": obj.get("currentPageNumber"),
-            "totalResults": obj.get("totalResults")
+            "name": obj.get("name"),
+            "categories": [CategoryMinimalDTO.from_dict(_item) for _item in obj["categories"]] if obj.get("categories") is not None else None,
+            "total": obj.get("total")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_medium_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_medium_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -32,25 +32,25 @@
 from typing_extensions import Self
 
 class RecordingMediumDTO(BaseModel):
     """
     Recording with a mid-sized field set.
     """ # noqa: E501
     isrc: StrictStr
+    recording_party_entities: Optional[List[RecordingPartyDTO]] = Field(default=None, alias="recordingPartyEntities")
     genres: Optional[List[GenreDTO]] = None
     language_of_performance: Optional[StrictStr] = Field(default=None, alias="languageOfPerformance")
     release_date: Optional[datetime] = Field(default=None, alias="releaseDate")
-    recording_party_entities: Optional[List[RecordingPartyDTO]] = Field(default=None, alias="recordingPartyEntities")
     titles: Optional[List[TitleDTO]] = None
     tracks: Optional[List[TrackDTO]] = None
     musical_features: Optional[MusicalFeaturesDTO] = Field(default=None, alias="musicalFeatures")
     spotify_id: Optional[StrictStr] = Field(default=None, alias="spotifyId")
     tags: Optional[List[RecordingTagSmallDTO]] = None
     genre_predictions: Optional[List[RecordingGenrePredictionDTO]] = Field(default=None, alias="genrePredictions")
-    __properties: ClassVar[List[str]] = ["isrc", "genres", "languageOfPerformance", "releaseDate", "recordingPartyEntities", "titles", "tracks", "musicalFeatures", "spotifyId", "tags", "genrePredictions"]
+    __properties: ClassVar[List[str]] = ["isrc", "recordingPartyEntities", "genres", "languageOfPerformance", "releaseDate", "titles", "tracks", "musicalFeatures", "spotifyId", "tags", "genrePredictions"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -83,28 +83,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
-        _items = []
-        if self.genres:
-            for _item in self.genres:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['genres'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in recording_party_entities (list)
         _items = []
         if self.recording_party_entities:
             for _item in self.recording_party_entities:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['recordingPartyEntities'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
+        _items = []
+        if self.genres:
+            for _item in self.genres:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['genres'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
         _items = []
         if self.titles:
             for _item in self.titles:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['titles'] = _items
@@ -141,18 +141,18 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "isrc": obj.get("isrc"),
+            "recordingPartyEntities": [RecordingPartyDTO.from_dict(_item) for _item in obj["recordingPartyEntities"]] if obj.get("recordingPartyEntities") is not None else None,
             "genres": [GenreDTO.from_dict(_item) for _item in obj["genres"]] if obj.get("genres") is not None else None,
             "languageOfPerformance": obj.get("languageOfPerformance"),
             "releaseDate": obj.get("releaseDate"),
-            "recordingPartyEntities": [RecordingPartyDTO.from_dict(_item) for _item in obj["recordingPartyEntities"]] if obj.get("recordingPartyEntities") is not None else None,
             "titles": [TitleDTO.from_dict(_item) for _item in obj["titles"]] if obj.get("titles") is not None else None,
             "tracks": [TrackDTO.from_dict(_item) for _item in obj["tracks"]] if obj.get("tracks") is not None else None,
             "musicalFeatures": MusicalFeaturesDTO.from_dict(obj["musicalFeatures"]) if obj.get("musicalFeatures") is not None else None,
             "spotifyId": obj.get("spotifyId"),
             "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj["tags"]] if obj.get("tags") is not None else None,
             "genrePredictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj["genrePredictions"]] if obj.get("genrePredictions") is not None else None
         })
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from songtradr_api_client_python.models.musical_features_dto import MusicalFeaturesDTO
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
+from songtradr_api_client_python.models.taggram_dto import TaggramDTO
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RecordingMinimalWithMusicalFeaturesDTO(BaseModel):
+class RecordingMinimalWithTaggramsDTO(BaseModel):
     """
     Recording in its minimal form, but with AI-predicted musical features.
     """ # noqa: E501
     isrc: StrictStr
-    musical_features: Optional[List[MusicalFeaturesDTO]] = Field(default=None, alias="musicalFeatures")
-    __properties: ClassVar[List[str]] = ["isrc", "musicalFeatures"]
+    timestamps: Optional[List[Union[StrictFloat, StrictInt]]] = Field(default=None, description="Points in time in seconds. Each value refers to the taggrams values of the same index.")
+    taggrams: Optional[List[TaggramDTO]] = None
+    __properties: ClassVar[List[str]] = ["isrc", "timestamps", "taggrams"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecordingMinimalWithMusicalFeaturesDTO from a JSON string"""
+        """Create an instance of RecordingMinimalWithTaggramsDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,32 +68,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in musical_features (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in taggrams (list)
         _items = []
-        if self.musical_features:
-            for _item in self.musical_features:
+        if self.taggrams:
+            for _item in self.taggrams:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['musicalFeatures'] = _items
+            _dict['taggrams'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecordingMinimalWithMusicalFeaturesDTO from a dict"""
+        """Create an instance of RecordingMinimalWithTaggramsDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "isrc": obj.get("isrc"),
-            "musicalFeatures": [MusicalFeaturesDTO.from_dict(_item) for _item in obj["musicalFeatures"]] if obj.get("musicalFeatures") is not None else None
+            "timestamps": obj.get("timestamps"),
+            "taggrams": [TaggramDTO.from_dict(_item) for _item in obj["taggrams"]] if obj.get("taggrams") is not None else None
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/track_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from songtradr_api_client_python.models.taggram_dto import TaggramDTO
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RecordingMinimalWithTaggramsDTO(BaseModel):
+class TrackDTO(BaseModel):
     """
-    Recording in its minimal form, but with AI-predicted musical features.
+    A track that connects from recording to a product with a mid-sized field set.
     """ # noqa: E501
-    isrc: StrictStr
-    timestamps: Optional[List[Union[StrictFloat, StrictInt]]] = Field(default=None, description="Points in time in seconds. Each value refers to the taggrams values of the same index.")
-    taggrams: Optional[List[TaggramDTO]] = None
-    __properties: ClassVar[List[str]] = ["isrc", "timestamps", "taggrams"]
+    songtradr_track_id: Optional[StrictStr] = Field(default=None, alias="songtradrTrackId")
+    __properties: ClassVar[List[str]] = ["songtradrTrackId"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecordingMinimalWithTaggramsDTO from a JSON string"""
+        """Create an instance of TrackDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,33 +65,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in taggrams (list)
-        _items = []
-        if self.taggrams:
-            for _item in self.taggrams:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['taggrams'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecordingMinimalWithTaggramsDTO from a dict"""
+        """Create an instance of TrackDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "isrc": obj.get("isrc"),
-            "timestamps": obj.get("timestamps"),
-            "taggrams": [TaggramDTO.from_dict(_item) for _item in obj["taggrams"]] if obj.get("taggrams") is not None else None
+            "songtradrTrackId": obj.get("songtradrTrackId")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/taggram_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from songtradr_api_client_python.models.tagstrength_dto import TagstrengthDTO
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RecordingMinimalWithTagstrengthsDTO(BaseModel):
+class TaggramDTO(BaseModel):
     """
-    Recording in its minimal form, but with AI-predicted musical features.
+    A TaggramDTO for recordings.
     """ # noqa: E501
-    isrc: StrictStr
-    tagstrengths: Optional[List[TagstrengthDTO]] = None
-    __properties: ClassVar[List[str]] = ["isrc", "tagstrengths"]
+    timeseries: List[Union[StrictFloat, StrictInt]] = Field(description="Values represent the strength of presence of the corresponding category, tag or genre.")
+    category_name: StrictStr = Field(alias="categoryName")
+    tag_name: Optional[StrictStr] = Field(default=None, alias="tagName")
+    genre_name: Optional[StrictStr] = Field(default=None, alias="genreName")
+    scale: Optional[List[StrictInt]] = None
+    __properties: ClassVar[List[str]] = ["timeseries", "categoryName", "tagName", "genreName", "scale"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecordingMinimalWithTagstrengthsDTO from a JSON string"""
+        """Create an instance of TaggramDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,32 +69,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in tagstrengths (list)
-        _items = []
-        if self.tagstrengths:
-            for _item in self.tagstrengths:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tagstrengths'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecordingMinimalWithTagstrengthsDTO from a dict"""
+        """Create an instance of TaggramDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "isrc": obj.get("isrc"),
-            "tagstrengths": [TagstrengthDTO.from_dict(_item) for _item in obj["tagstrengths"]] if obj.get("tagstrengths") is not None else None
+            "timeseries": obj.get("timeseries"),
+            "categoryName": obj.get("categoryName"),
+            "tagName": obj.get("tagName"),
+            "genreName": obj.get("genreName"),
+            "scale": obj.get("scale")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_party_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/recording_party_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_small_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/title_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO
-from songtradr_api_client_python.models.title_dto import TitleDTO
-from songtradr_api_client_python.models.track_dto import TrackDTO
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RecordingSmallDTO(BaseModel):
+class TitleDTO(BaseModel):
     """
-    Recording with a small field set.
+    A Title for recordings or products.
     """ # noqa: E501
-    duration: Optional[StrictInt] = None
-    isrc: StrictStr
-    parties: Optional[List[RecordingPartyDTO]] = None
-    titles: Optional[List[TitleDTO]] = None
-    tracks: Optional[List[TrackDTO]] = None
-    __properties: ClassVar[List[str]] = ["duration", "isrc", "parties", "titles", "tracks"]
+    title_text: StrictStr = Field(alias="titleText")
+    __properties: ClassVar[List[str]] = ["titleText"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -51,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecordingSmallDTO from a JSON string"""
+        """Create an instance of TitleDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,49 +65,24 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
-        _items = []
-        if self.parties:
-            for _item in self.parties:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['parties'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
-        _items = []
-        if self.titles:
-            for _item in self.titles:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['titles'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
-        _items = []
-        if self.tracks:
-            for _item in self.tracks:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tracks'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecordingSmallDTO from a dict"""
+        """Create an instance of TitleDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "duration": obj.get("duration"),
-            "isrc": obj.get("isrc"),
-            "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj["parties"]] if obj.get("parties") is not None else None,
-            "titles": [TitleDTO.from_dict(_item) for _item in obj["titles"]] if obj.get("titles") is not None else None,
-            "tracks": [TrackDTO.from_dict(_item) for _item in obj["tracks"]] if obj.get("tracks") is not None else None
+            "titleText": obj.get("titleText")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/recording_tag_small_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/update_password_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
-from songtradr_api_client_python.models.tag_dto import TagDTO
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RecordingTagSmallDTO(BaseModel):
+class UpdatePasswordDTO(BaseModel):
     """
-    Tag information in with a small field-set.
+    UpdatePasswordDTO
     """ # noqa: E501
-    tag: TagDTO
-    __properties: ClassVar[List[str]] = ["tag"]
+    token: StrictStr
+    password: StrictStr
+    __properties: ClassVar[List[str]] = ["token", "password"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RecordingTagSmallDTO from a JSON string"""
+        """Create an instance of UpdatePasswordDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,27 +66,25 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of tag
-        if self.tag:
-            _dict['tag'] = self.tag.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RecordingTagSmallDTO from a dict"""
+        """Create an instance of UpdatePasswordDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "tag": TagDTO.from_dict(obj["tag"]) if obj.get("tag") is not None else None
+            "token": obj.get("token"),
+            "password": obj.get("password")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/save_user_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/save_user_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/search_filter_values_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/search_filter_values_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/sign_up_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/sign_up_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/tag_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/tag_small_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/tagstrength_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TagSmallDTO(BaseModel):
+class TagstrengthDTO(BaseModel):
     """
-    A tag for recordings with a reduced field-set.
+    A TaggramDTO for recordings.
     """ # noqa: E501
-    id: StrictInt
-    name: StrictStr
-    __properties: ClassVar[List[str]] = ["id", "name"]
+    strength: Union[StrictFloat, StrictInt] = Field(description="Strength of presence of the corresponding category, tag or genre.")
+    category_name: StrictStr = Field(alias="categoryName")
+    tag_name: Optional[StrictStr] = Field(default=None, alias="tagName")
+    genre_name: Optional[StrictStr] = Field(default=None, alias="genreName")
+    scale: Optional[List[StrictInt]] = None
+    __properties: ClassVar[List[str]] = ["strength", "categoryName", "tagName", "genreName", "scale"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TagSmallDTO from a JSON string"""
+        """Create an instance of TagstrengthDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +73,24 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TagSmallDTO from a dict"""
+        """Create an instance of TagstrengthDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "name": obj.get("name")
+            "strength": obj.get("strength"),
+            "categoryName": obj.get("categoryName"),
+            "tagName": obj.get("tagName"),
+            "genreName": obj.get("genreName"),
+            "scale": obj.get("scale")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/taggram_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/token_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TaggramDTO(BaseModel):
+class TokenRequest(BaseModel):
     """
-    A TaggramDTO for recordings.
+    TokenRequest
     """ # noqa: E501
-    timeseries: List[Union[StrictFloat, StrictInt]] = Field(description="Values represent the strength of presence of the corresponding category, tag or genre.")
-    category_name: StrictStr = Field(alias="categoryName")
-    tag_name: Optional[StrictStr] = Field(default=None, alias="tagName")
-    genre_name: Optional[StrictStr] = Field(default=None, alias="genreName")
-    scale: Optional[List[StrictInt]] = None
-    __properties: ClassVar[List[str]] = ["timeseries", "categoryName", "tagName", "genreName", "scale"]
+    refresh_token: StrictStr = Field(alias="refreshToken")
+    __properties: ClassVar[List[str]] = ["refreshToken"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -48,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TaggramDTO from a JSON string"""
+        """Create an instance of TokenRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,24 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TaggramDTO from a dict"""
+        """Create an instance of TokenRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "timeseries": obj.get("timeseries"),
-            "categoryName": obj.get("categoryName"),
-            "tagName": obj.get("tagName"),
-            "genreName": obj.get("genreName"),
-            "scale": obj.get("scale")
+            "refreshToken": obj.get("refreshToken")
         })
         return _obj
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/title_dto.py` & `songtradr_api_client_python-3.0.0/test/test_recording_tag_small_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,65 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
-
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
-from typing import Optional, Set
-from typing_extensions import Self
-
-class TitleDTO(BaseModel):
-    """
-    A Title for recordings or products.
-    """ # noqa: E501
-    title_text: StrictStr = Field(alias="titleText")
-    __properties: ClassVar[List[str]] = ["titleText"]
-
-    model_config = ConfigDict(
-        populate_by_name=True,
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TitleDTO from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+import unittest
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        return _dict
+from songtradr_api_client_python.models.recording_tag_small_dto import RecordingTagSmallDTO
+
+class TestRecordingTagSmallDTO(unittest.TestCase):
+    """RecordingTagSmallDTO unit test stubs"""
+
+    def setUp(self):
+        pass
 
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TitleDTO from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "titleText": obj.get("titleText")
-        })
-        return _obj
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> RecordingTagSmallDTO:
+        """Test RecordingTagSmallDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RecordingTagSmallDTO`
+        """
+        model = RecordingTagSmallDTO()
+        if include_optional:
+            return RecordingTagSmallDTO(
+                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                    id = 56, 
+                    name = '', 
+                    categories = [
+                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                            category_name = '', )
+                        ], )
+            )
+        else:
+            return RecordingTagSmallDTO(
+                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                    id = 56, 
+                    name = '', 
+                    categories = [
+                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                            category_name = '', )
+                        ], ),
+        )
+        """
 
+    def testRecordingTagSmallDTO(self):
+        """Test RecordingTagSmallDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/token_request.py` & `songtradr_api_client_python-3.0.0/test/test_recording_party_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,61 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
-
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
-from typing import Optional, Set
-from typing_extensions import Self
-
-class TokenRequest(BaseModel):
-    """
-    TokenRequest
-    """ # noqa: E501
-    refresh_token: StrictStr = Field(alias="refreshToken")
-    __properties: ClassVar[List[str]] = ["refreshToken"]
-
-    model_config = ConfigDict(
-        populate_by_name=True,
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TokenRequest from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+import unittest
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        return _dict
+from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO
+
+class TestRecordingPartyDTO(unittest.TestCase):
+    """RecordingPartyDTO unit test stubs"""
+
+    def setUp(self):
+        pass
 
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TokenRequest from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "refreshToken": obj.get("refreshToken")
-        })
-        return _obj
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> RecordingPartyDTO:
+        """Test RecordingPartyDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RecordingPartyDTO`
+        """
+        model = RecordingPartyDTO()
+        if include_optional:
+            return RecordingPartyDTO(
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', ),
+                contributor_types = [
+                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                        type_name = '', )
+                    ]
+            )
+        else:
+            return RecordingPartyDTO(
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', ),
+        )
+        """
 
+    def testRecordingPartyDTO(self):
+        """Test RecordingPartyDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/update_password_dto.py` & `songtradr_api_client_python-3.0.0/test/test_file_upload_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,64 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
-
-from pydantic import BaseModel, ConfigDict, StrictStr
-from typing import Any, ClassVar, Dict, List
-from typing import Optional, Set
-from typing_extensions import Self
-
-class UpdatePasswordDTO(BaseModel):
-    """
-    UpdatePasswordDTO
-    """ # noqa: E501
-    token: StrictStr
-    password: StrictStr
-    __properties: ClassVar[List[str]] = ["token", "password"]
-
-    model_config = ConfigDict(
-        populate_by_name=True,
-        validate_assignment=True,
-        protected_namespaces=(),
-    )
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UpdatePasswordDTO from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+import unittest
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        return _dict
+from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO
+
+class TestFileUploadDTO(unittest.TestCase):
+    """FileUploadDTO unit test stubs"""
+
+    def setUp(self):
+        pass
 
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UpdatePasswordDTO from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "token": obj.get("token"),
-            "password": obj.get("password")
-        })
-        return _obj
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> FileUploadDTO:
+        """Test FileUploadDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `FileUploadDTO`
+        """
+        model = FileUploadDTO()
+        if include_optional:
+            return FileUploadDTO(
+                identifiers = [
+                    songtradr_api_client_python.models.config_identifier_dto.ConfigIdentifierDTO(
+                        identifier_type = '', 
+                        identifier_value = '', )
+                    ],
+                flags = [
+                    ''
+                    ],
+                access = [
+                    songtradr_api_client_python.models.config_access_dto.ConfigAccessDTO(
+                        accessor_id = 'full', 
+                        rights = 'full', )
+                    ]
+            )
+        else:
+            return FileUploadDTO(
+        )
+        """
 
+    def testFileUploadDTO(self):
+        """Test FileUploadDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/models/user_dto.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/models/user_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python/rest.py` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/PKG-INFO` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 2.1.0
+Version: 3.0.0
 Summary: Songtradr API
 Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `songtradr_api_client_python-2.1.0/songtradr_api_client_python.egg-info/SOURCES.txt` & `songtradr_api_client_python-3.0.0/songtradr_api_client_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 songtradr_api_client_python.egg-info/requires.txt
 songtradr_api_client_python.egg-info/top_level.txt
 songtradr_api_client_python/api/__init__.py
 songtradr_api_client_python/api/allowed_values_api.py
 songtradr_api_client_python/api/recording_api.py
 songtradr_api_client_python/api/user_api.py
 songtradr_api_client_python/models/__init__.py
-songtradr_api_client_python/models/category_medium_dto.py
 songtradr_api_client_python/models/category_minimal_dto.py
 songtradr_api_client_python/models/config_access_dto.py
 songtradr_api_client_python/models/config_identifier_dto.py
 songtradr_api_client_python/models/contributor_type_dto.py
 songtradr_api_client_python/models/error_response.py
 songtradr_api_client_python/models/field_summary_dto.py
 songtradr_api_client_python/models/file_dto.py
@@ -32,46 +31,39 @@
 songtradr_api_client_python/models/file_upload_dto.py
 songtradr_api_client_python/models/file_w_ith_url_dto.py
 songtradr_api_client_python/models/files_summary_dto.py
 songtradr_api_client_python/models/forgot_password_dto.py
 songtradr_api_client_python/models/genre_dto.py
 songtradr_api_client_python/models/genre_minimal_dto.py
 songtradr_api_client_python/models/genres_summary_dto.py
-songtradr_api_client_python/models/image_recognition_response.py
 songtradr_api_client_python/models/init_put_recording_audio_dto.py
 songtradr_api_client_python/models/jwt_token_dto.py
 songtradr_api_client_python/models/login_dto.py
 songtradr_api_client_python/models/musical_features_dto.py
 songtradr_api_client_python/models/party_small_dto.py
-songtradr_api_client_python/models/recording_for_similarity_search_dto.py
 songtradr_api_client_python/models/recording_genre_prediction_dto.py
-songtradr_api_client_python/models/recording_list_dto.py
 songtradr_api_client_python/models/recording_medium_dto.py
-songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
 songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
 songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
 songtradr_api_client_python/models/recording_party_dto.py
-songtradr_api_client_python/models/recording_small_dto.py
 songtradr_api_client_python/models/recording_tag_small_dto.py
 songtradr_api_client_python/models/save_user_dto.py
 songtradr_api_client_python/models/search_filter_values_dto.py
 songtradr_api_client_python/models/sign_up_dto.py
 songtradr_api_client_python/models/tag_dto.py
-songtradr_api_client_python/models/tag_small_dto.py
 songtradr_api_client_python/models/taggram_dto.py
 songtradr_api_client_python/models/tags_summary_dto.py
 songtradr_api_client_python/models/tagstrength_dto.py
 songtradr_api_client_python/models/title_dto.py
 songtradr_api_client_python/models/token_request.py
 songtradr_api_client_python/models/track_dto.py
 songtradr_api_client_python/models/update_password_dto.py
 songtradr_api_client_python/models/user_dto.py
 songtradr_api_client_python/models/video_recognition_response.py
 test/test_allowed_values_api.py
-test/test_category_medium_dto.py
 test/test_category_minimal_dto.py
 test/test_config_access_dto.py
 test/test_config_identifier_dto.py
 test/test_contributor_type_dto.py
 test/test_error_response.py
 test/test_field_summary_dto.py
 test/test_file_dto.py
@@ -80,36 +72,30 @@
 test/test_file_upload_dto.py
 test/test_file_w_ith_url_dto.py
 test/test_files_summary_dto.py
 test/test_forgot_password_dto.py
 test/test_genre_dto.py
 test/test_genre_minimal_dto.py
 test/test_genres_summary_dto.py
-test/test_image_recognition_response.py
 test/test_init_put_recording_audio_dto.py
 test/test_jwt_token_dto.py
 test/test_login_dto.py
 test/test_musical_features_dto.py
 test/test_party_small_dto.py
 test/test_recording_api.py
-test/test_recording_for_similarity_search_dto.py
 test/test_recording_genre_prediction_dto.py
-test/test_recording_list_dto.py
 test/test_recording_medium_dto.py
-test/test_recording_minimal_with_musical_features_dto.py
 test/test_recording_minimal_with_taggrams_dto.py
 test/test_recording_minimal_with_tagstrengths_dto.py
 test/test_recording_party_dto.py
-test/test_recording_small_dto.py
 test/test_recording_tag_small_dto.py
 test/test_save_user_dto.py
 test/test_search_filter_values_dto.py
 test/test_sign_up_dto.py
 test/test_tag_dto.py
-test/test_tag_small_dto.py
 test/test_taggram_dto.py
 test/test_tags_summary_dto.py
 test/test_tagstrength_dto.py
 test/test_title_dto.py
 test/test_token_request.py
 test/test_track_dto.py
 test/test_update_password_dto.py
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_allowed_values_api.py` & `songtradr_api_client_python-3.0.0/test/test_allowed_values_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -30,24 +30,10 @@
     def test_allowed_musical_features(self) -> None:
         """Test case for allowed_musical_features
 
         Allowed values for music descriptive parameters to be used in the searchAll endpoint.
         """
         pass
 
-    def test_genres(self) -> None:
-        """Test case for genres
-
-        Allowed values for genres.
-        """
-        pass
-
-    def test_tags(self) -> None:
-        """Test case for tags
-
-        All descriptive tags inside of tag-categories.
-        """
-        pass
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_category_medium_dto.py` & `songtradr_api_client_python-3.0.0/test/test_tag_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.category_medium_dto import CategoryMediumDTO
+from songtradr_api_client_python.models.tag_dto import TagDTO
 
-class TestCategoryMediumDTO(unittest.TestCase):
-    """CategoryMediumDTO unit test stubs"""
+class TestTagDTO(unittest.TestCase):
+    """TagDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CategoryMediumDTO:
-        """Test CategoryMediumDTO
+    def make_instance(self, include_optional) -> TagDTO:
+        """Test TagDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CategoryMediumDTO`
+        # uncomment below to create an instance of `TagDTO`
         """
-        model = CategoryMediumDTO()
+        model = TagDTO()
         if include_optional:
-            return CategoryMediumDTO(
+            return TagDTO(
                 id = 56,
                 name = '',
-                tags = [
-                    songtradr_api_client_python.models.tag_small_dto.TagSmallDTO(
-                        id = 56, 
-                        name = '', )
+                categories = [
+                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                        category_name = '', )
                     ]
             )
         else:
-            return CategoryMediumDTO(
+            return TagDTO(
                 id = 56,
                 name = '',
         )
         """
 
-    def testCategoryMediumDTO(self):
-        """Test CategoryMediumDTO"""
+    def testTagDTO(self):
+        """Test TagDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_category_minimal_dto.py` & `songtradr_api_client_python-3.0.0/test/test_category_minimal_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_config_access_dto.py` & `songtradr_api_client_python-3.0.0/test/test_config_access_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_config_identifier_dto.py` & `songtradr_api_client_python-3.0.0/test/test_config_identifier_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_contributor_type_dto.py` & `songtradr_api_client_python-3.0.0/test/test_contributor_type_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_error_response.py` & `songtradr_api_client_python-3.0.0/test/test_error_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_field_summary_dto.py` & `songtradr_api_client_python-3.0.0/test/test_field_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_file_dto.py` & `songtradr_api_client_python-3.0.0/test/test_file_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -48,57 +48,41 @@
                 fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 inference_status = 'processing',
                 inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
                     isrc = '', 
-                    genres = [
-                        songtradr_api_client_python.models.genre_dto.GenreDTO(
-                            id = 56, 
-                            name = '', )
-                        ], 
-                    language_of_performance = '', 
-                    release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     recording_party_entities = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
                                 ], )
                         ], 
+                    genres = [
+                        songtradr_api_client_python.models.genre_dto.GenreDTO(
+                            id = 56, 
+                            name = '', )
+                        ], 
+                    language_of_performance = '', 
+                    release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], 
                     tracks = [
                         songtradr_api_client_python.models.track_dto.TrackDTO(
                             songtradr_track_id = '', )
                         ], 
                     musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        valence_affinity = 1.337, 
-                        tempo_affinity = 1.337, 
-                        scale_affinity = 1.337, 
-                        timbre_affinity = 1.337, 
-                        roughness_affinity = 1.337, 
-                        harmony_affinity = 1.337, 
-                        texture_affinity = 1.337, 
-                        groovyness_affinity = 1.337, 
-                        space_affinity = 1.337, 
-                        loudness_affinity = 1.337, 
-                        key_affinity = 1.337, 
-                        channel_suitability_affinity = 1.337, 
-                        arousal_affinity = 1.337, 
-                        pleasantness_affinity = 1.337, 
-                        engagement_affinity = 1.337, 
-                        energy_affinity = 1.337, 
                         language_of_performance = 'en', 
                         arousal = 'very calm', 
                         dominant_instrument = 'piano', 
                         energy = 'very quiet', 
                         engagement = 'very unengaging', 
                         groovyness = 'very steady', 
                         harmony = 'very dissonant', 
@@ -162,15 +146,31 @@
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
                         pretzel_station_suitability_affinity = 1.337, 
-                        audience_region = 'Australia and New Zealand', ), 
+                        audience_region = 'Australia and New Zealand', 
+                        valence_affinity = 1.337, 
+                        arousal_affinity = 1.337, 
+                        pleasantness_affinity = 1.337, 
+                        engagement_affinity = 1.337, 
+                        energy_affinity = 1.337, 
+                        tempo_affinity = 1.337, 
+                        scale_affinity = 1.337, 
+                        timbre_affinity = 1.337, 
+                        roughness_affinity = 1.337, 
+                        harmony_affinity = 1.337, 
+                        texture_affinity = 1.337, 
+                        groovyness_affinity = 1.337, 
+                        space_affinity = 1.337, 
+                        loudness_affinity = 1.337, 
+                        key_affinity = 1.337, 
+                        channel_suitability_affinity = 1.337, ), 
                     spotify_id = '', 
                     tags = [
                         songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                             tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                 id = 56, 
                                 name = '', 
                                 categories = [
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_file_list_dto.py` & `songtradr_api_client_python-3.0.0/test/test_file_list_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -50,57 +50,41 @@
                         fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_status = 'processing', 
                         inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
                             isrc = '', 
-                            genres = [
-                                songtradr_api_client_python.models.genre_dto.GenreDTO(
-                                    id = 56, 
-                                    name = '', )
-                                ], 
-                            language_of_performance = '', 
-                            release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                     party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                         id = '', 
                                         full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                             type_name = '', )
                                         ], )
                                 ], 
+                            genres = [
+                                songtradr_api_client_python.models.genre_dto.GenreDTO(
+                                    id = 56, 
+                                    name = '', )
+                                ], 
+                            language_of_performance = '', 
+                            release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             tracks = [
                                 songtradr_api_client_python.models.track_dto.TrackDTO(
                                     songtradr_track_id = '', )
                                 ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                valence_affinity = 1.337, 
-                                tempo_affinity = 1.337, 
-                                scale_affinity = 1.337, 
-                                timbre_affinity = 1.337, 
-                                roughness_affinity = 1.337, 
-                                harmony_affinity = 1.337, 
-                                texture_affinity = 1.337, 
-                                groovyness_affinity = 1.337, 
-                                space_affinity = 1.337, 
-                                loudness_affinity = 1.337, 
-                                key_affinity = 1.337, 
-                                channel_suitability_affinity = 1.337, 
-                                arousal_affinity = 1.337, 
-                                pleasantness_affinity = 1.337, 
-                                engagement_affinity = 1.337, 
-                                energy_affinity = 1.337, 
                                 language_of_performance = 'en', 
                                 arousal = 'very calm', 
                                 dominant_instrument = 'piano', 
                                 energy = 'very quiet', 
                                 engagement = 'very unengaging', 
                                 groovyness = 'very steady', 
                                 harmony = 'very dissonant', 
@@ -164,15 +148,31 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 pretzel_station_suitability_affinity = 1.337, 
-                                audience_region = 'Australia and New Zealand', ), 
+                                audience_region = 'Australia and New Zealand', 
+                                valence_affinity = 1.337, 
+                                arousal_affinity = 1.337, 
+                                pleasantness_affinity = 1.337, 
+                                engagement_affinity = 1.337, 
+                                energy_affinity = 1.337, 
+                                tempo_affinity = 1.337, 
+                                scale_affinity = 1.337, 
+                                timbre_affinity = 1.337, 
+                                roughness_affinity = 1.337, 
+                                harmony_affinity = 1.337, 
+                                texture_affinity = 1.337, 
+                                groovyness_affinity = 1.337, 
+                                space_affinity = 1.337, 
+                                loudness_affinity = 1.337, 
+                                key_affinity = 1.337, 
+                                channel_suitability_affinity = 1.337, ), 
                             spotify_id = '', 
                             tags = [
                                 songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                     tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                         id = 56, 
                                         name = '', 
                                         categories = [
@@ -210,57 +210,41 @@
                         fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_status = 'processing', 
                         inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
                             isrc = '', 
-                            genres = [
-                                songtradr_api_client_python.models.genre_dto.GenreDTO(
-                                    id = 56, 
-                                    name = '', )
-                                ], 
-                            language_of_performance = '', 
-                            release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                     party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                         id = '', 
                                         full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                             type_name = '', )
                                         ], )
                                 ], 
+                            genres = [
+                                songtradr_api_client_python.models.genre_dto.GenreDTO(
+                                    id = 56, 
+                                    name = '', )
+                                ], 
+                            language_of_performance = '', 
+                            release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             tracks = [
                                 songtradr_api_client_python.models.track_dto.TrackDTO(
                                     songtradr_track_id = '', )
                                 ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                valence_affinity = 1.337, 
-                                tempo_affinity = 1.337, 
-                                scale_affinity = 1.337, 
-                                timbre_affinity = 1.337, 
-                                roughness_affinity = 1.337, 
-                                harmony_affinity = 1.337, 
-                                texture_affinity = 1.337, 
-                                groovyness_affinity = 1.337, 
-                                space_affinity = 1.337, 
-                                loudness_affinity = 1.337, 
-                                key_affinity = 1.337, 
-                                channel_suitability_affinity = 1.337, 
-                                arousal_affinity = 1.337, 
-                                pleasantness_affinity = 1.337, 
-                                engagement_affinity = 1.337, 
-                                energy_affinity = 1.337, 
                                 language_of_performance = 'en', 
                                 arousal = 'very calm', 
                                 dominant_instrument = 'piano', 
                                 energy = 'very quiet', 
                                 engagement = 'very unengaging', 
                                 groovyness = 'very steady', 
                                 harmony = 'very dissonant', 
@@ -324,15 +308,31 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 pretzel_station_suitability_affinity = 1.337, 
-                                audience_region = 'Australia and New Zealand', ), 
+                                audience_region = 'Australia and New Zealand', 
+                                valence_affinity = 1.337, 
+                                arousal_affinity = 1.337, 
+                                pleasantness_affinity = 1.337, 
+                                engagement_affinity = 1.337, 
+                                energy_affinity = 1.337, 
+                                tempo_affinity = 1.337, 
+                                scale_affinity = 1.337, 
+                                timbre_affinity = 1.337, 
+                                roughness_affinity = 1.337, 
+                                harmony_affinity = 1.337, 
+                                texture_affinity = 1.337, 
+                                groovyness_affinity = 1.337, 
+                                space_affinity = 1.337, 
+                                loudness_affinity = 1.337, 
+                                key_affinity = 1.337, 
+                                channel_suitability_affinity = 1.337, ), 
                             spotify_id = '', 
                             tags = [
                                 songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                     tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                         id = 56, 
                                         name = '', 
                                         categories = [
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_file_small_dto.py` & `songtradr_api_client_python-3.0.0/test/test_file_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -37,23 +37,23 @@
         if include_optional:
             return FileSmallDTO(
                 folder = '',
                 name = '',
                 id = 56,
                 extension = 'mp3',
                 error_message = '',
-                fingerprint_status = 'processing',
-                object_key = '',
                 upload_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 upload_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                fingerprint_status = 'processing',
                 fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 inference_status = 'processing',
                 inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                object_key = '',
                 error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else:
             return FileSmallDTO(
                 folder = '',
                 name = '',
                 id = 56,
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_file_upload_dto.py` & `songtradr_api_client_python-3.0.0/test/test_jwt_token_dto.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,56 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO
+from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
 
-class TestFileUploadDTO(unittest.TestCase):
-    """FileUploadDTO unit test stubs"""
+class TestJwtTokenDTO(unittest.TestCase):
+    """JwtTokenDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> FileUploadDTO:
-        """Test FileUploadDTO
+    def make_instance(self, include_optional) -> JwtTokenDTO:
+        """Test JwtTokenDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `FileUploadDTO`
+        # uncomment below to create an instance of `JwtTokenDTO`
         """
-        model = FileUploadDTO()
+        model = JwtTokenDTO()
         if include_optional:
-            return FileUploadDTO(
-                identifiers = [
-                    songtradr_api_client_python.models.config_identifier_dto.ConfigIdentifierDTO(
-                        identifier_type = '', 
-                        identifier_value = '', )
-                    ],
-                flags = [
-                    ''
-                    ],
-                access = [
-                    songtradr_api_client_python.models.config_access_dto.ConfigAccessDTO(
-                        accessor_id = 'full', 
-                        rights = 'full', )
-                    ]
+            return JwtTokenDTO(
+                jwt_token = '',
+                expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                refresh_token = ''
             )
         else:
-            return FileUploadDTO(
+            return JwtTokenDTO(
+                jwt_token = '',
+                expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
         )
         """
 
-    def testFileUploadDTO(self):
-        """Test FileUploadDTO"""
+    def testJwtTokenDTO(self):
+        """Test JwtTokenDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_file_w_ith_url_dto.py` & `songtradr_api_client_python-3.0.0/test/test_file_w_ith_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -49,57 +49,41 @@
                     fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_status = 'processing', 
                     inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
                         isrc = '', 
-                        genres = [
-                            songtradr_api_client_python.models.genre_dto.GenreDTO(
-                                id = 56, 
-                                name = '', )
-                            ], 
-                        language_of_performance = '', 
-                        release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                     id = '', 
                                     full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                         type_name = '', )
                                     ], )
                             ], 
+                        genres = [
+                            songtradr_api_client_python.models.genre_dto.GenreDTO(
+                                id = 56, 
+                                name = '', )
+                            ], 
+                        language_of_performance = '', 
+                        release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         tracks = [
                             songtradr_api_client_python.models.track_dto.TrackDTO(
                                 songtradr_track_id = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            valence_affinity = 1.337, 
-                            tempo_affinity = 1.337, 
-                            scale_affinity = 1.337, 
-                            timbre_affinity = 1.337, 
-                            roughness_affinity = 1.337, 
-                            harmony_affinity = 1.337, 
-                            texture_affinity = 1.337, 
-                            groovyness_affinity = 1.337, 
-                            space_affinity = 1.337, 
-                            loudness_affinity = 1.337, 
-                            key_affinity = 1.337, 
-                            channel_suitability_affinity = 1.337, 
-                            arousal_affinity = 1.337, 
-                            pleasantness_affinity = 1.337, 
-                            engagement_affinity = 1.337, 
-                            energy_affinity = 1.337, 
                             language_of_performance = 'en', 
                             arousal = 'very calm', 
                             dominant_instrument = 'piano', 
                             energy = 'very quiet', 
                             engagement = 'very unengaging', 
                             groovyness = 'very steady', 
                             harmony = 'very dissonant', 
@@ -163,15 +147,31 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             pretzel_station_suitability_affinity = 1.337, 
-                            audience_region = 'Australia and New Zealand', ), 
+                            audience_region = 'Australia and New Zealand', 
+                            valence_affinity = 1.337, 
+                            arousal_affinity = 1.337, 
+                            pleasantness_affinity = 1.337, 
+                            engagement_affinity = 1.337, 
+                            energy_affinity = 1.337, 
+                            tempo_affinity = 1.337, 
+                            scale_affinity = 1.337, 
+                            timbre_affinity = 1.337, 
+                            roughness_affinity = 1.337, 
+                            harmony_affinity = 1.337, 
+                            texture_affinity = 1.337, 
+                            groovyness_affinity = 1.337, 
+                            space_affinity = 1.337, 
+                            loudness_affinity = 1.337, 
+                            key_affinity = 1.337, 
+                            channel_suitability_affinity = 1.337, ), 
                         spotify_id = '', 
                         tags = [
                             songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                     id = 56, 
                                     name = '', 
                                     categories = [
@@ -205,57 +205,41 @@
                     fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_status = 'processing', 
                     inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
                         isrc = '', 
-                        genres = [
-                            songtradr_api_client_python.models.genre_dto.GenreDTO(
-                                id = 56, 
-                                name = '', )
-                            ], 
-                        language_of_performance = '', 
-                        release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                     id = '', 
                                     full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                         type_name = '', )
                                     ], )
                             ], 
+                        genres = [
+                            songtradr_api_client_python.models.genre_dto.GenreDTO(
+                                id = 56, 
+                                name = '', )
+                            ], 
+                        language_of_performance = '', 
+                        release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         tracks = [
                             songtradr_api_client_python.models.track_dto.TrackDTO(
                                 songtradr_track_id = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            valence_affinity = 1.337, 
-                            tempo_affinity = 1.337, 
-                            scale_affinity = 1.337, 
-                            timbre_affinity = 1.337, 
-                            roughness_affinity = 1.337, 
-                            harmony_affinity = 1.337, 
-                            texture_affinity = 1.337, 
-                            groovyness_affinity = 1.337, 
-                            space_affinity = 1.337, 
-                            loudness_affinity = 1.337, 
-                            key_affinity = 1.337, 
-                            channel_suitability_affinity = 1.337, 
-                            arousal_affinity = 1.337, 
-                            pleasantness_affinity = 1.337, 
-                            engagement_affinity = 1.337, 
-                            energy_affinity = 1.337, 
                             language_of_performance = 'en', 
                             arousal = 'very calm', 
                             dominant_instrument = 'piano', 
                             energy = 'very quiet', 
                             engagement = 'very unengaging', 
                             groovyness = 'very steady', 
                             harmony = 'very dissonant', 
@@ -319,15 +303,31 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             pretzel_station_suitability_affinity = 1.337, 
-                            audience_region = 'Australia and New Zealand', ), 
+                            audience_region = 'Australia and New Zealand', 
+                            valence_affinity = 1.337, 
+                            arousal_affinity = 1.337, 
+                            pleasantness_affinity = 1.337, 
+                            engagement_affinity = 1.337, 
+                            energy_affinity = 1.337, 
+                            tempo_affinity = 1.337, 
+                            scale_affinity = 1.337, 
+                            timbre_affinity = 1.337, 
+                            roughness_affinity = 1.337, 
+                            harmony_affinity = 1.337, 
+                            texture_affinity = 1.337, 
+                            groovyness_affinity = 1.337, 
+                            space_affinity = 1.337, 
+                            loudness_affinity = 1.337, 
+                            key_affinity = 1.337, 
+                            channel_suitability_affinity = 1.337, ), 
                         spotify_id = '', 
                         tags = [
                             songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                                 tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                                     id = 56, 
                                     name = '', 
                                     categories = [
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_files_summary_dto.py` & `songtradr_api_client_python-3.0.0/test/test_files_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_forgot_password_dto.py` & `songtradr_api_client_python-3.0.0/test/test_forgot_password_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_genre_dto.py` & `songtradr_api_client_python-3.0.0/test/test_genre_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_genre_minimal_dto.py` & `songtradr_api_client_python-3.0.0/test/test_genre_minimal_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_genres_summary_dto.py` & `songtradr_api_client_python-3.0.0/test/test_genres_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_image_recognition_response.py` & `songtradr_api_client_python-3.0.0/test/test_video_recognition_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.image_recognition_response import ImageRecognitionResponse
+from songtradr_api_client_python.models.video_recognition_response import VideoRecognitionResponse
 
-class TestImageRecognitionResponse(unittest.TestCase):
-    """ImageRecognitionResponse unit test stubs"""
+class TestVideoRecognitionResponse(unittest.TestCase):
+    """VideoRecognitionResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ImageRecognitionResponse:
-        """Test ImageRecognitionResponse
+    def make_instance(self, include_optional) -> VideoRecognitionResponse:
+        """Test VideoRecognitionResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ImageRecognitionResponse`
+        # uncomment below to create an instance of `VideoRecognitionResponse`
         """
-        model = ImageRecognitionResponse()
+        model = VideoRecognitionResponse()
         if include_optional:
-            return ImageRecognitionResponse(
+            return VideoRecognitionResponse(
                 labels = [
-                    songtradr_api_client_python.models.label.Label()
+                    songtradr_api_client_python.models.label_detection.LabelDetection()
                     ],
                 faces = [
-                    songtradr_api_client_python.models.face_detail.FaceDetail()
+                    songtradr_api_client_python.models.face_detection.FaceDetection()
                     ]
             )
         else:
-            return ImageRecognitionResponse(
+            return VideoRecognitionResponse(
         )
         """
 
-    def testImageRecognitionResponse(self):
-        """Test ImageRecognitionResponse"""
+    def testVideoRecognitionResponse(self):
+        """Test VideoRecognitionResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_init_put_recording_audio_dto.py` & `songtradr_api_client_python-3.0.0/test/test_init_put_recording_audio_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_jwt_token_dto.py` & `songtradr_api_client_python-3.0.0/test/test_tags_summary_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
+from songtradr_api_client_python.models.tags_summary_dto import TagsSummaryDTO
 
-class TestJwtTokenDTO(unittest.TestCase):
-    """JwtTokenDTO unit test stubs"""
+class TestTagsSummaryDTO(unittest.TestCase):
+    """TagsSummaryDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> JwtTokenDTO:
-        """Test JwtTokenDTO
+    def make_instance(self, include_optional) -> TagsSummaryDTO:
+        """Test TagsSummaryDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `JwtTokenDTO`
+        # uncomment below to create an instance of `TagsSummaryDTO`
         """
-        model = JwtTokenDTO()
+        model = TagsSummaryDTO()
         if include_optional:
-            return JwtTokenDTO(
-                jwt_token = '',
-                expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                refresh_token = ''
+            return TagsSummaryDTO(
+                name = '',
+                categories = [
+                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                        category_name = '', )
+                    ],
+                total = 56
             )
         else:
-            return JwtTokenDTO(
-                jwt_token = '',
-                expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+            return TagsSummaryDTO(
+                name = '',
+                total = 56,
         )
         """
 
-    def testJwtTokenDTO(self):
-        """Test JwtTokenDTO"""
+    def testTagsSummaryDTO(self):
+        """Test TagsSummaryDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_login_dto.py` & `songtradr_api_client_python-3.0.0/test/test_login_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_musical_features_dto.py` & `songtradr_api_client_python-3.0.0/test/test_musical_features_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -33,30 +33,14 @@
             optional params are included """
         # uncomment below to create an instance of `MusicalFeaturesDTO`
         """
         model = MusicalFeaturesDTO()
         if include_optional:
             return MusicalFeaturesDTO(
                 space = 'very compact',
-                valence_affinity = 1.337,
-                tempo_affinity = 1.337,
-                scale_affinity = 1.337,
-                timbre_affinity = 1.337,
-                roughness_affinity = 1.337,
-                harmony_affinity = 1.337,
-                texture_affinity = 1.337,
-                groovyness_affinity = 1.337,
-                space_affinity = 1.337,
-                loudness_affinity = 1.337,
-                key_affinity = 1.337,
-                channel_suitability_affinity = 1.337,
-                arousal_affinity = 1.337,
-                pleasantness_affinity = 1.337,
-                engagement_affinity = 1.337,
-                energy_affinity = 1.337,
                 language_of_performance = 'en',
                 arousal = 'very calm',
                 dominant_instrument = 'piano',
                 energy = 'very quiet',
                 engagement = 'very unengaging',
                 groovyness = 'very steady',
                 harmony = 'very dissonant',
@@ -120,15 +104,31 @@
                 origin_decade_affinity = 1.337,
                 language_of_performance_affinity = 1.337,
                 curateability_affinity = 1.337,
                 use_case_affinity = 1.337,
                 industry_suitability = 'Automobiles and Parts',
                 industry_suitability_affinity = 1.337,
                 pretzel_station_suitability_affinity = 1.337,
-                audience_region = 'Australia and New Zealand'
+                audience_region = 'Australia and New Zealand',
+                valence_affinity = 1.337,
+                arousal_affinity = 1.337,
+                pleasantness_affinity = 1.337,
+                engagement_affinity = 1.337,
+                energy_affinity = 1.337,
+                tempo_affinity = 1.337,
+                scale_affinity = 1.337,
+                timbre_affinity = 1.337,
+                roughness_affinity = 1.337,
+                harmony_affinity = 1.337,
+                texture_affinity = 1.337,
+                groovyness_affinity = 1.337,
+                space_affinity = 1.337,
+                loudness_affinity = 1.337,
+                key_affinity = 1.337,
+                channel_suitability_affinity = 1.337
             )
         else:
             return MusicalFeaturesDTO(
         )
         """
 
     def testMusicalFeaturesDTO(self):
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_party_small_dto.py` & `songtradr_api_client_python-3.0.0/test/test_party_small_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_recording_api.py` & `songtradr_api_client_python-3.0.0/test/test_save_user_dto.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,58 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.api.recording_api import RecordingApi
+from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
 
+class TestSaveUserDTO(unittest.TestCase):
+    """SaveUserDTO unit test stubs"""
 
-class TestRecordingApi(unittest.TestCase):
-    """RecordingApi unit test stubs"""
-
-    def setUp(self) -> None:
-        self.api = RecordingApi()
-
-    def tearDown(self) -> None:
-        pass
-
-    def test_prompt_search_recordings(self) -> None:
-        """Test case for prompt_search_recordings
-
-        Recordings for query.
-        """
-        pass
-
-    def test_recordings_by_ids_with_musical_features(self) -> None:
-        """Test case for recordings_by_ids_with_musical_features
-
-        AI generated moods, musical features and more for recordings.
-        """
-        pass
-
-    def test_recordings_by_ids_with_similarities1(self) -> None:
-        """Test case for recordings_by_ids_with_similarities1
-
-        Similar recordings for a list of recordings.
-        """
-        pass
-
-    def test_recordings_by_ids_with_taggrams1(self) -> None:
-        """Test case for recordings_by_ids_with_taggrams1
-
-        Timeseries of AI generated moods, musical features and more for a list of recordings.
-        """
-        pass
-
-    def test_recordings_by_ids_with_tagstrengths1(self) -> None:
-        """Test case for recordings_by_ids_with_tagstrengths1
-
-        Strengths as numerical representations for AI generated moods, musical features and more for recordings.
-        """
-        pass
-
-    def test_recordings_medium_by_ids1(self) -> None:
-        """Test case for recordings_medium_by_ids1
-
-        Recordings by IDs with a medium sized response.
-        """
-        pass
-
-    def test_search_recordings(self) -> None:
-        """Test case for search_recordings
-
-        Recordings by contributors, moods, musical features and more.
-        """
+    def setUp(self):
         pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> SaveUserDTO:
+        """Test SaveUserDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SaveUserDTO`
+        """
+        model = SaveUserDTO()
+        if include_optional:
+            return SaveUserDTO(
+                system = 'musicube',
+                email_address = '',
+                password = '',
+                full_name = '',
+                company_name = '',
+                language = 'en'
+            )
+        else:
+            return SaveUserDTO(
+                email_address = '',
+        )
+        """
+
+    def testSaveUserDTO(self):
+        """Test SaveUserDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_recording_genre_prediction_dto.py` & `songtradr_api_client_python-3.0.0/test/test_recording_genre_prediction_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_recording_medium_dto.py` & `songtradr_api_client_python-3.0.0/test/test_recording_medium_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -33,57 +33,41 @@
             optional params are included """
         # uncomment below to create an instance of `RecordingMediumDTO`
         """
         model = RecordingMediumDTO()
         if include_optional:
             return RecordingMediumDTO(
                 isrc = '',
-                genres = [
-                    songtradr_api_client_python.models.genre_dto.GenreDTO(
-                        id = 56, 
-                        name = '', )
-                    ],
-                language_of_performance = '',
-                release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 recording_party_entities = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                         party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                             id = '', 
                             full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                 type_name = '', )
                             ], )
                     ],
+                genres = [
+                    songtradr_api_client_python.models.genre_dto.GenreDTO(
+                        id = 56, 
+                        name = '', )
+                    ],
+                language_of_performance = '',
+                release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 titles = [
                     songtradr_api_client_python.models.title_dto.TitleDTO(
                         title_text = '', )
                     ],
                 tracks = [
                     songtradr_api_client_python.models.track_dto.TrackDTO(
                         songtradr_track_id = '', )
                     ],
                 musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                     space = 'very compact', 
-                    valence_affinity = 1.337, 
-                    tempo_affinity = 1.337, 
-                    scale_affinity = 1.337, 
-                    timbre_affinity = 1.337, 
-                    roughness_affinity = 1.337, 
-                    harmony_affinity = 1.337, 
-                    texture_affinity = 1.337, 
-                    groovyness_affinity = 1.337, 
-                    space_affinity = 1.337, 
-                    loudness_affinity = 1.337, 
-                    key_affinity = 1.337, 
-                    channel_suitability_affinity = 1.337, 
-                    arousal_affinity = 1.337, 
-                    pleasantness_affinity = 1.337, 
-                    engagement_affinity = 1.337, 
-                    energy_affinity = 1.337, 
                     language_of_performance = 'en', 
                     arousal = 'very calm', 
                     dominant_instrument = 'piano', 
                     energy = 'very quiet', 
                     engagement = 'very unengaging', 
                     groovyness = 'very steady', 
                     harmony = 'very dissonant', 
@@ -147,15 +131,31 @@
                     origin_decade_affinity = 1.337, 
                     language_of_performance_affinity = 1.337, 
                     curateability_affinity = 1.337, 
                     use_case_affinity = 1.337, 
                     industry_suitability = 'Automobiles and Parts', 
                     industry_suitability_affinity = 1.337, 
                     pretzel_station_suitability_affinity = 1.337, 
-                    audience_region = 'Australia and New Zealand', ),
+                    audience_region = 'Australia and New Zealand', 
+                    valence_affinity = 1.337, 
+                    arousal_affinity = 1.337, 
+                    pleasantness_affinity = 1.337, 
+                    engagement_affinity = 1.337, 
+                    energy_affinity = 1.337, 
+                    tempo_affinity = 1.337, 
+                    scale_affinity = 1.337, 
+                    timbre_affinity = 1.337, 
+                    roughness_affinity = 1.337, 
+                    harmony_affinity = 1.337, 
+                    texture_affinity = 1.337, 
+                    groovyness_affinity = 1.337, 
+                    space_affinity = 1.337, 
+                    loudness_affinity = 1.337, 
+                    key_affinity = 1.337, 
+                    channel_suitability_affinity = 1.337, ),
                 spotify_id = '',
                 tags = [
                     songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
                         tag = songtradr_api_client_python.models.tag_dto.TagDTO(
                             id = 56, 
                             name = '', 
                             categories = [
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_taggrams_dto.py` & `songtradr_api_client_python-3.0.0/test/test_recording_minimal_with_taggrams_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_recording_minimal_with_tagstrengths_dto.py` & `songtradr_api_client_python-3.0.0/test/test_recording_minimal_with_tagstrengths_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_recording_party_dto.py` & `songtradr_api_client_python-3.0.0/test/test_track_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO
+from songtradr_api_client_python.models.track_dto import TrackDTO
 
-class TestRecordingPartyDTO(unittest.TestCase):
-    """RecordingPartyDTO unit test stubs"""
+class TestTrackDTO(unittest.TestCase):
+    """TrackDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> RecordingPartyDTO:
-        """Test RecordingPartyDTO
+    def make_instance(self, include_optional) -> TrackDTO:
+        """Test TrackDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `RecordingPartyDTO`
+        # uncomment below to create an instance of `TrackDTO`
         """
-        model = RecordingPartyDTO()
+        model = TrackDTO()
         if include_optional:
-            return RecordingPartyDTO(
-                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                    id = '', 
-                    full_name = '', ),
-                contributor_types = [
-                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
-                        type_name = '', )
-                    ]
+            return TrackDTO(
+                songtradr_track_id = ''
             )
         else:
-            return RecordingPartyDTO(
-                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
-                    id = '', 
-                    full_name = '', ),
+            return TrackDTO(
         )
         """
 
-    def testRecordingPartyDTO(self):
-        """Test RecordingPartyDTO"""
+    def testTrackDTO(self):
+        """Test TrackDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_recording_tag_small_dto.py` & `songtradr_api_client_python-3.0.0/test/test_taggram_dto.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.recording_tag_small_dto import RecordingTagSmallDTO
+from songtradr_api_client_python.models.taggram_dto import TaggramDTO
 
-class TestRecordingTagSmallDTO(unittest.TestCase):
-    """RecordingTagSmallDTO unit test stubs"""
+class TestTaggramDTO(unittest.TestCase):
+    """TaggramDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> RecordingTagSmallDTO:
-        """Test RecordingTagSmallDTO
+    def make_instance(self, include_optional) -> TaggramDTO:
+        """Test TaggramDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `RecordingTagSmallDTO`
+        # uncomment below to create an instance of `TaggramDTO`
         """
-        model = RecordingTagSmallDTO()
+        model = TaggramDTO()
         if include_optional:
-            return RecordingTagSmallDTO(
-                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                    id = 56, 
-                    name = '', 
-                    categories = [
-                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                            category_name = '', )
-                        ], )
+            return TaggramDTO(
+                timeseries = [
+                    1.337
+                    ],
+                category_name = '',
+                tag_name = '',
+                genre_name = '',
+                scale = [
+                    56
+                    ]
             )
         else:
-            return RecordingTagSmallDTO(
-                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                    id = 56, 
-                    name = '', 
-                    categories = [
-                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                            category_name = '', )
-                        ], ),
+            return TaggramDTO(
+                timeseries = [
+                    1.337
+                    ],
+                category_name = '',
         )
         """
 
-    def testRecordingTagSmallDTO(self):
-        """Test RecordingTagSmallDTO"""
+    def testTaggramDTO(self):
+        """Test TaggramDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_save_user_dto.py` & `songtradr_api_client_python-3.0.0/test/test_tagstrength_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
+from songtradr_api_client_python.models.tagstrength_dto import TagstrengthDTO
 
-class TestSaveUserDTO(unittest.TestCase):
-    """SaveUserDTO unit test stubs"""
+class TestTagstrengthDTO(unittest.TestCase):
+    """TagstrengthDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SaveUserDTO:
-        """Test SaveUserDTO
+    def make_instance(self, include_optional) -> TagstrengthDTO:
+        """Test TagstrengthDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SaveUserDTO`
+        # uncomment below to create an instance of `TagstrengthDTO`
         """
-        model = SaveUserDTO()
+        model = TagstrengthDTO()
         if include_optional:
-            return SaveUserDTO(
-                system = 'musicube',
-                email_address = '',
-                password = '',
-                full_name = '',
-                company_name = '',
-                language = 'en'
+            return TagstrengthDTO(
+                strength = 1.337,
+                category_name = '',
+                tag_name = '',
+                genre_name = '',
+                scale = [
+                    56
+                    ]
             )
         else:
-            return SaveUserDTO(
-                email_address = '',
+            return TagstrengthDTO(
+                strength = 1.337,
+                category_name = '',
         )
         """
 
-    def testSaveUserDTO(self):
-        """Test SaveUserDTO"""
+    def testTagstrengthDTO(self):
+        """Test TagstrengthDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_search_filter_values_dto.py` & `songtradr_api_client_python-3.0.0/test/test_search_filter_values_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_sign_up_dto.py` & `songtradr_api_client_python-3.0.0/test/test_sign_up_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_tag_dto.py` & `songtradr_api_client_python-3.0.0/test/test_token_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.tag_dto import TagDTO
+from songtradr_api_client_python.models.token_request import TokenRequest
 
-class TestTagDTO(unittest.TestCase):
-    """TagDTO unit test stubs"""
+class TestTokenRequest(unittest.TestCase):
+    """TokenRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> TagDTO:
-        """Test TagDTO
+    def make_instance(self, include_optional) -> TokenRequest:
+        """Test TokenRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `TagDTO`
+        # uncomment below to create an instance of `TokenRequest`
         """
-        model = TagDTO()
+        model = TokenRequest()
         if include_optional:
-            return TagDTO(
-                id = 56,
-                name = '',
-                categories = [
-                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                        category_name = '', )
-                    ]
+            return TokenRequest(
+                refresh_token = ''
             )
         else:
-            return TagDTO(
-                id = 56,
-                name = '',
+            return TokenRequest(
+                refresh_token = '',
         )
         """
 
-    def testTagDTO(self):
-        """Test TagDTO"""
+    def testTokenRequest(self):
+        """Test TokenRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_tag_small_dto.py` & `songtradr_api_client_python-3.0.0/test/test_title_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO
+from songtradr_api_client_python.models.title_dto import TitleDTO
 
-class TestTagSmallDTO(unittest.TestCase):
-    """TagSmallDTO unit test stubs"""
+class TestTitleDTO(unittest.TestCase):
+    """TitleDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> TagSmallDTO:
-        """Test TagSmallDTO
+    def make_instance(self, include_optional) -> TitleDTO:
+        """Test TitleDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `TagSmallDTO`
+        # uncomment below to create an instance of `TitleDTO`
         """
-        model = TagSmallDTO()
+        model = TitleDTO()
         if include_optional:
-            return TagSmallDTO(
-                id = 56,
-                name = ''
+            return TitleDTO(
+                title_text = ''
             )
         else:
-            return TagSmallDTO(
-                id = 56,
-                name = '',
+            return TitleDTO(
+                title_text = '',
         )
         """
 
-    def testTagSmallDTO(self):
-        """Test TagSmallDTO"""
+    def testTitleDTO(self):
+        """Test TitleDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_taggram_dto.py` & `songtradr_api_client_python-3.0.0/test/test_update_password_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.taggram_dto import TaggramDTO
+from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO
 
-class TestTaggramDTO(unittest.TestCase):
-    """TaggramDTO unit test stubs"""
+class TestUpdatePasswordDTO(unittest.TestCase):
+    """UpdatePasswordDTO unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> TaggramDTO:
-        """Test TaggramDTO
+    def make_instance(self, include_optional) -> UpdatePasswordDTO:
+        """Test UpdatePasswordDTO
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `TaggramDTO`
+        # uncomment below to create an instance of `UpdatePasswordDTO`
         """
-        model = TaggramDTO()
+        model = UpdatePasswordDTO()
         if include_optional:
-            return TaggramDTO(
-                timeseries = [
-                    1.337
-                    ],
-                category_name = '',
-                tag_name = '',
-                genre_name = '',
-                scale = [
-                    56
-                    ]
+            return UpdatePasswordDTO(
+                token = '',
+                password = ''
             )
         else:
-            return TaggramDTO(
-                timeseries = [
-                    1.337
-                    ],
-                category_name = '',
+            return UpdatePasswordDTO(
+                token = '',
+                password = '',
         )
         """
 
-    def testTaggramDTO(self):
-        """Test TaggramDTO"""
+    def testUpdatePasswordDTO(self):
+        """Test UpdatePasswordDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_tags_summary_dto.py` & `songtradr_api_client_python-3.0.0/test/test_recording_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from songtradr_api_client_python.models.tags_summary_dto import TagsSummaryDTO
+from songtradr_api_client_python.api.recording_api import RecordingApi
 
-class TestTagsSummaryDTO(unittest.TestCase):
-    """TagsSummaryDTO unit test stubs"""
 
-    def setUp(self):
+class TestRecordingApi(unittest.TestCase):
+    """RecordingApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = RecordingApi()
+
+    def tearDown(self) -> None:
         pass
 
-    def tearDown(self):
+    def test_recordings_by_ids_with_taggrams1(self) -> None:
+        """Test case for recordings_by_ids_with_taggrams1
+
+        Timeseries of AI generated moods, musical features and more for a list of recordings.
+        """
         pass
 
-    def make_instance(self, include_optional) -> TagsSummaryDTO:
-        """Test TagsSummaryDTO
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `TagsSummaryDTO`
+    def test_recordings_by_ids_with_tagstrengths1(self) -> None:
+        """Test case for recordings_by_ids_with_tagstrengths1
+
+        Strengths as numerical representations for AI generated moods, musical features and more for recordings.
         """
-        model = TagsSummaryDTO()
-        if include_optional:
-            return TagsSummaryDTO(
-                name = '',
-                categories = [
-                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                        category_name = '', )
-                    ],
-                total = 56
-            )
-        else:
-            return TagsSummaryDTO(
-                name = '',
-                total = 56,
-        )
+        pass
+
+    def test_recordings_medium_by_ids1(self) -> None:
+        """Test case for recordings_medium_by_ids1
+
+        Recordings by IDs with a medium sized response.
         """
+        pass
 
-    def testTagsSummaryDTO(self):
-        """Test TagsSummaryDTO"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_user_api.py` & `songtradr_api_client_python-3.0.0/test/test_user_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -58,63 +58,28 @@
     def test_initiate_user_file_upload(self) -> None:
         """Test case for initiate_user_file_upload
 
         Initialize a file upload. Responds with an URL where the file can be uploaded.
         """
         pass
 
-    def test_initiate_user_image_upload(self) -> None:
-        """Test case for initiate_user_image_upload
-
-        Recognise and upload image. Responds with an object with recognition result.
-        """
-        pass
-
     def test_login(self) -> None:
         """Test case for login
 
         Login to generate a bearer token.
         """
         pass
 
     def test_me(self) -> None:
         """Test case for me
 
         Details for a logged-in user
         """
         pass
 
-    def test_prompt_search_user_files(self) -> None:
-        """Test case for prompt_search_user_files
-
-        Files for query.
-        """
-        pass
-
-    def test_recordings_by_folder_with_taggrams(self) -> None:
-        """Test case for recordings_by_folder_with_taggrams
-
-        Timeseries of AI generated moods, musical features and more for recordings in your folder.
-        """
-        pass
-
-    def test_recordings_by_folder_with_tagstrengths(self) -> None:
-        """Test case for recordings_by_folder_with_tagstrengths
-
-        Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
-        """
-        pass
-
-    def test_recordings_by_ids_with_similarities(self) -> None:
-        """Test case for recordings_by_ids_with_similarities
-
-        Similar recordings for a list of user recordings.
-        """
-        pass
-
     def test_recordings_by_ids_with_taggrams(self) -> None:
         """Test case for recordings_by_ids_with_taggrams
 
         Timeseries of AI generated moods, musical features and more for a list of recordings.
         """
         pass
```

### Comparing `songtradr_api_client_python-2.1.0/test/test_user_dto.py` & `songtradr_api_client_python-3.0.0/test/test_user_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
-    The version of the OpenAPI document: 2.1.0
+    The version of the OpenAPI document: 3.0.0
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

