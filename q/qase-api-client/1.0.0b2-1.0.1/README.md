# Comparing `tmp/qase_api_client-1.0.0b2.tar.gz` & `tmp/qase_api_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_api_client-1.0.0b2.tar", last modified: Mon May  6 12:24:42 2024, max compression
+gzip compressed data, was "qase_api_client-1.0.1.tar", last modified: Mon Jun  3 07:38:07 2024, max compression
```

## Comparing `qase_api_client-1.0.0b2.tar` & `qase_api_client-1.0.1.tar`

### file list

```diff
@@ -1,343 +1,343 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.408233 qase_api_client-1.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-05-06 12:24:42.408233 qase_api_client-1.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:24:42.408233 qase_api_client-1.0.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.348232 qase_api_client-1.0.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.348232 qase_api_client-1.0.0b2/src/qase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.348232 qase_api_client-1.0.0b2/src/qase/api_client_v1/
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.352232 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45359 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24100 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/authors_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   108138 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/cases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    36006 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    56301 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82977 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/defects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    59746 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/environments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    60458 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/milestones_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    58853 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/plans_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    67944 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/results_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    77144 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    60665 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/shared_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    61289 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/suites_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api/system_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.376232 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/
--rw-r--r--   0 runner    (1001) docker     (127)    11137 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachmentupload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create_value_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue_issues_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/resultcreate_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/tag_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk_cases_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_caseexternal_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/src/qase/api_client_v1/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.404233 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 12:24:42.000000 qase_api_client-1.0.0b2/src/qase_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:42.404233 qase_api_client-1.0.0b2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachment_uploads_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_attachmentupload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_author_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_authors_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_base_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_bulk200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_bulk200_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_cases_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_group_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configuration_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_create_value_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_field_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_fields_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_custom_fields_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defect_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_defects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_environments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_external_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_external_issue_issues_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_hash_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_hash_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_id_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_id_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestone_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_milestones_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_detailed_all_of_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_plans_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_code_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_counts_defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_counts_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_project_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_qql_defect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_qql_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_qql_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_requirement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_create_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_result_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_resultcreate_bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_results_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_public_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_public_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_run_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_runs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_search_response_all_of_result_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_content_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_step_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_shared_steps_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suite_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_suites_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_field_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_field_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_system_fields_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_tag_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_external_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_external_issues_links_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_list_response_all_of_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_case_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_casebulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_casebulk_cases_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_caseexternal_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-06 12:24:36.000000 qase_api_client-1.0.0b2/test/test_test_step_result_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.801532 qase_api_client-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-06-03 07:38:07.801532 qase_api_client-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 07:38:07.801532 qase_api_client-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.741532 qase_api_client-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.741532 qase_api_client-1.0.1/src/qase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.741532 qase_api_client-1.0.1/src/qase/api_client_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12703 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.745532 qase_api_client-1.0.1/src/qase/api_client_v1/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45359 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24100 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/authors_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108138 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/cases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36006 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56301 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82977 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/defects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59746 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60458 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/milestones_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58853 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67944 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/results_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77144 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60665 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/shared_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61289 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api/system_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.773532 qase_api_client-1.0.1/src/qase/api_client_v1/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/attachmentupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/author.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/author_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/author_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/author_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/bulk200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/bulk200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_create_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_fields_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/external_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/external_issue_issues_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/hash_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/hash_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/id_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_code_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_counts_defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_counts_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/qql_defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/qql_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/qql_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/result_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/resultcreate_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_public_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_public_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/search_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/search_response_all_of_result_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_content_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/system_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/system_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/system_field_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_external_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_casebulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_casebulk_cases_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_caseexternal_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step_result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/src/qase/api_client_v1/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.801532 qase_api_client-1.0.1/src/qase_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-06-03 07:38:07.000000 qase_api_client-1.0.1/src/qase_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-06-03 07:38:07.000000 qase_api_client-1.0.1/src/qase_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:38:07.000000 qase_api_client-1.0.1/src/qase_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-03 07:38:07.000000 qase_api_client-1.0.1/src/qase_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-03 07:38:07.000000 qase_api_client-1.0.1/src/qase_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:38:07.801532 qase_api_client-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachment_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachment_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachment_uploads_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_attachmentupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_author.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_author_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_author_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_author_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_authors_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_bulk200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_bulk200_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_cases_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_configuration_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_configuration_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_configuration_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_configuration_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_configuration_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_field_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_field_create_value_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_field_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_field_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_fields_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_custom_fields_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defect_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_defects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_environment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_environment_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_environment_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_environment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_external_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_external_issue_issues_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_hash_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_hash_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_id_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_milestone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_milestone_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_milestone_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_milestone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_milestone_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_milestones_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_detailed_all_of_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_code_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_counts_defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_counts_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_qql_defect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_qql_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_qql_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_create_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_create_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_create_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_result_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_resultcreate_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_results_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_public_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_public_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_runs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_search_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_search_response_all_of_result_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step_content_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_step_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_shared_steps_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suite_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suite_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suite_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suite_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suite_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suite_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_suites_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_system_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_system_field_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_system_field_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_system_fields_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_external_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_external_issues_links_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_list_response_all_of_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_case_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_casebulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_casebulk_cases_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_caseexternal_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_step_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_step_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-03 07:38:02.000000 qase_api_client-1.0.1/test/test_test_step_result_create.py
```

### Comparing `qase_api_client-1.0.0b2/PKG-INFO` & `qase_api_client-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-api-client
-Version: 1.0.0b2
+Version: 1.0.1
 Summary: Qase TestOps API V1 client for Python
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python
 Keywords: OpenAPI,OpenAPI-Generator,Qase.io TestOps API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `qase_api_client-1.0.0b2/README.md` & `qase_api_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/pyproject.toml` & `qase_api_client-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-api-client"
-version = "1.0.0b2"
+version = "1.0.1"
 description = "Qase TestOps API V1 client for Python"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/__init__.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 from qase.api_client_v1.models.author import Author
 from qase.api_client_v1.models.author_list_response import AuthorListResponse
 from qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
 from qase.api_client_v1.models.author_response import AuthorResponse
 from qase.api_client_v1.models.base_response import BaseResponse
 from qase.api_client_v1.models.bulk200_response import Bulk200Response
 from qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
-from qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration import ConfigurationModel
 from qase.api_client_v1.models.configuration_create import ConfigurationCreate
 from qase.api_client_v1.models.configuration_group import ConfigurationGroup
 from qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
 from qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
 from qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
 from qase.api_client_v1.models.custom_field import CustomField
 from qase.api_client_v1.models.custom_field_create import CustomFieldCreate
```

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/__init__.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/attachments_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/authors_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/authors_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/cases_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/cases_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/configurations_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/configurations_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/custom_fields_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/defects_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/defects_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/environments_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/environments_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/milestones_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/milestones_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/plans_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/plans_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/projects_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/results_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/results_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/runs_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/runs_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/search_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/search_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/shared_steps_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/shared_steps_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/suites_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/suites_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api/system_fields_api.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api/system_fields_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api_client.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api_client.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/api_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/api_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/configuration.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/configuration.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/exceptions.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/__init__.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from qase.api_client_v1.models.author import Author
 from qase.api_client_v1.models.author_list_response import AuthorListResponse
 from qase.api_client_v1.models.author_list_response_all_of_result import AuthorListResponseAllOfResult
 from qase.api_client_v1.models.author_response import AuthorResponse
 from qase.api_client_v1.models.base_response import BaseResponse
 from qase.api_client_v1.models.bulk200_response import Bulk200Response
 from qase.api_client_v1.models.bulk200_response_all_of_result import Bulk200ResponseAllOfResult
-from qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration import ConfigurationModel
 from qase.api_client_v1.models.configuration_create import ConfigurationCreate
 from qase.api_client_v1.models.configuration_group import ConfigurationGroup
 from qase.api_client_v1.models.configuration_group_create import ConfigurationGroupCreate
 from qase.api_client_v1.models.configuration_list_response import ConfigurationListResponse
 from qase.api_client_v1.models.configuration_list_response_all_of_result import ConfigurationListResponseAllOfResult
 from qase.api_client_v1.models.custom_field import CustomField
 from qase.api_client_v1.models.custom_field_create import CustomFieldCreate
```

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_get.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_get.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_hash.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_hash.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachment_uploads_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachment_uploads_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/attachmentupload.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/attachmentupload.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/author.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/author_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/author_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/author_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/author_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/base_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/base_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/bulk200_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/bulk200_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/bulk200_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Configuration(BaseModel):
+class ConfigurationModel(BaseModel):
     """
     Configuration
     """ # noqa: E501
     id: Optional[StrictInt] = None
     title: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["id", "title"]
```

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration import ConfigurationModel
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ConfigurationGroup(BaseModel):
     """
     ConfigurationGroup
     """ # noqa: E501
     id: Optional[StrictInt] = None
     title: Optional[StrictStr] = None
-    configurations: Optional[List[Configuration]] = None
+    configurations: Optional[List[ConfigurationModel]] = None
     __properties: ClassVar[List[str]] = ["id", "title", "configurations"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -89,12 +89,12 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
             "title": obj.get("title"),
-            "configurations": [Configuration.from_dict(_item) for _item in obj["configurations"]] if obj.get("configurations") is not None else None
+            "configurations": [ConfigurationModel.from_dict(_item) for _item in obj["configurations"]] if obj.get("configurations") is not None else None
         })
         return _obj
```

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_group_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_group_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/configuration_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_create_value_inner.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_create_value_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_field_value.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_field_value.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_fields_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/custom_fields_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_query.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_query.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_status.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_status.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/defect_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/defect_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/environment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/environment_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/environment_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/external_issue.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/external_issue_issues_inner.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/external_issue_issues_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/hash_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/hash_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/hash_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/id_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/id_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/id_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/milestone_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/milestone_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_detailed.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_detailed_all_of_cases.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_query.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_query.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/plan_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/plan_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_access.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_access.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_code_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_code_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_code_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_counts.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_defects.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_counts_defects.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_counts_runs.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_counts_runs.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/project_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/project_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_defect.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/qql_defect.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_plan.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/qql_plan.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/qql_test_case.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/qql_test_case.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/requirement.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/requirement.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_bulk.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_bulk.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_case.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_case.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_create_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_create_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/result_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/result_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/resultcreate_bulk.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/resultcreate_bulk.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_environment.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_environment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_milestone.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_milestone.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_public.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_public_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_public_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_public_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/run_stats.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/run_stats.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/search_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/search_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/search_response_all_of_result_entities.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/search_response_all_of_result_entities.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_content.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_content_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_content_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/shared_step_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/shared_step_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/suite.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_delete.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_delete.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/suite_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/suite_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/system_field.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/system_field_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/system_field_option.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/system_field_option.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/tag_value.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/tag_value.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_external_issues.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_external_issues_links_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_params.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_params.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_query.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_query.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_response.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_case_update.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_case_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_casebulk.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_casebulk_cases_inner.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_casebulk_cases_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_caseexternal_issues.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_caseexternal_issues.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/models/test_step_result_create.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/models/test_step_result_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase/api_client_v1/rest.py` & `qase_api_client-1.0.1/src/qase/api_client_v1/rest.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/src/qase_api_client.egg-info/PKG-INFO` & `qase_api_client-1.0.1/src/qase_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-api-client
-Version: 1.0.0b2
+Version: 1.0.1
 Summary: Qase TestOps API V1 client for Python
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python
 Keywords: OpenAPI,OpenAPI-Generator,Qase.io TestOps API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `qase_api_client-1.0.0b2/src/qase_api_client.egg-info/SOURCES.txt` & `qase_api_client-1.0.1/src/qase_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachment.py` & `qase_api_client-1.0.1/test/test_attachment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachment_get.py` & `qase_api_client-1.0.1/test/test_attachment_get.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachment_hash.py` & `qase_api_client-1.0.1/test/test_attachment_hash.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachment_list_response.py` & `qase_api_client-1.0.1/test/test_attachment_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachment_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_attachment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachment_response.py` & `qase_api_client-1.0.1/test/test_attachment_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachment_uploads_response.py` & `qase_api_client-1.0.1/test/test_attachment_uploads_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachments_api.py` & `qase_api_client-1.0.1/test/test_attachments_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_attachmentupload.py` & `qase_api_client-1.0.1/test/test_attachmentupload.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_author.py` & `qase_api_client-1.0.1/test/test_author.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_author_list_response.py` & `qase_api_client-1.0.1/test/test_author_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_author_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_author_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_author_response.py` & `qase_api_client-1.0.1/test/test_author_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_authors_api.py` & `qase_api_client-1.0.1/test/test_authors_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_base_response.py` & `qase_api_client-1.0.1/test/test_base_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_bulk200_response.py` & `qase_api_client-1.0.1/test/test_bulk200_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_bulk200_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_bulk200_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_cases_api.py` & `qase_api_client-1.0.1/test/test_cases_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_configuration.py` & `qase_api_client-1.0.1/test/test_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from qase.api_client_v1.models.configuration import Configuration
+from qase.api_client_v1.models.configuration import ConfigurationModel
 
 class TestConfiguration(unittest.TestCase):
     """Configuration unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Configuration:
+    def make_instance(self, include_optional) -> ConfigurationModel:
         """Test Configuration
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `Configuration`
         """
         model = Configuration()
```

### Comparing `qase_api_client-1.0.0b2/test/test_configuration_create.py` & `qase_api_client-1.0.1/test/test_configuration_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_configuration_group.py` & `qase_api_client-1.0.1/test/test_configuration_group.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_configuration_group_create.py` & `qase_api_client-1.0.1/test/test_configuration_group_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_configuration_list_response.py` & `qase_api_client-1.0.1/test/test_configuration_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_configuration_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_configuration_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_configurations_api.py` & `qase_api_client-1.0.1/test/test_configurations_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_field.py` & `qase_api_client-1.0.1/test/test_custom_field.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_field_create.py` & `qase_api_client-1.0.1/test/test_custom_field_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_field_create_value_inner.py` & `qase_api_client-1.0.1/test/test_custom_field_create_value_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_field_list_response.py` & `qase_api_client-1.0.1/test/test_custom_field_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_field_response.py` & `qase_api_client-1.0.1/test/test_custom_field_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_field_update.py` & `qase_api_client-1.0.1/test/test_custom_field_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_field_value.py` & `qase_api_client-1.0.1/test/test_custom_field_value.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_fields_api.py` & `qase_api_client-1.0.1/test/test_custom_fields_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_fields_response.py` & `qase_api_client-1.0.1/test/test_custom_fields_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_custom_fields_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_custom_fields_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect.py` & `qase_api_client-1.0.1/test/test_defect.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect_create.py` & `qase_api_client-1.0.1/test/test_defect_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect_list_response.py` & `qase_api_client-1.0.1/test/test_defect_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_defect_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect_query.py` & `qase_api_client-1.0.1/test/test_defect_query.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect_response.py` & `qase_api_client-1.0.1/test/test_defect_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect_status.py` & `qase_api_client-1.0.1/test/test_defect_status.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defect_update.py` & `qase_api_client-1.0.1/test/test_defect_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_defects_api.py` & `qase_api_client-1.0.1/test/test_defects_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_environment.py` & `qase_api_client-1.0.1/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_environment_create.py` & `qase_api_client-1.0.1/test/test_environment_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_environment_list_response.py` & `qase_api_client-1.0.1/test/test_environment_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_environment_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_environment_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_environment_response.py` & `qase_api_client-1.0.1/test/test_environment_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_environment_update.py` & `qase_api_client-1.0.1/test/test_environment_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_environments_api.py` & `qase_api_client-1.0.1/test/test_environments_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_external_issue.py` & `qase_api_client-1.0.1/test/test_external_issue.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_external_issue_issues_inner.py` & `qase_api_client-1.0.1/test/test_external_issue_issues_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_hash_response.py` & `qase_api_client-1.0.1/test/test_hash_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_hash_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_hash_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_id_response.py` & `qase_api_client-1.0.1/test/test_id_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_id_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_id_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_milestone.py` & `qase_api_client-1.0.1/test/test_milestone.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_milestone_create.py` & `qase_api_client-1.0.1/test/test_milestone_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_milestone_list_response.py` & `qase_api_client-1.0.1/test/test_milestone_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_milestone_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_milestone_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_milestone_response.py` & `qase_api_client-1.0.1/test/test_milestone_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_milestone_update.py` & `qase_api_client-1.0.1/test/test_milestone_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_milestones_api.py` & `qase_api_client-1.0.1/test/test_milestones_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan.py` & `qase_api_client-1.0.1/test/test_plan.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_create.py` & `qase_api_client-1.0.1/test/test_plan_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_detailed.py` & `qase_api_client-1.0.1/test/test_plan_detailed.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_detailed_all_of_cases.py` & `qase_api_client-1.0.1/test/test_plan_detailed_all_of_cases.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_list_response.py` & `qase_api_client-1.0.1/test/test_plan_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_plan_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_query.py` & `qase_api_client-1.0.1/test/test_plan_query.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_response.py` & `qase_api_client-1.0.1/test/test_plan_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plan_update.py` & `qase_api_client-1.0.1/test/test_plan_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_plans_api.py` & `qase_api_client-1.0.1/test/test_plans_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project.py` & `qase_api_client-1.0.1/test/test_project.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_access.py` & `qase_api_client-1.0.1/test/test_project_access.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_code_response.py` & `qase_api_client-1.0.1/test/test_project_code_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_code_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_project_code_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_counts.py` & `qase_api_client-1.0.1/test/test_project_counts.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_counts_defects.py` & `qase_api_client-1.0.1/test/test_project_counts_defects.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_counts_runs.py` & `qase_api_client-1.0.1/test/test_project_counts_runs.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_create.py` & `qase_api_client-1.0.1/test/test_project_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_list_response.py` & `qase_api_client-1.0.1/test/test_project_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_project_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_project_response.py` & `qase_api_client-1.0.1/test/test_project_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_projects_api.py` & `qase_api_client-1.0.1/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_qql_defect.py` & `qase_api_client-1.0.1/test/test_qql_defect.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_qql_plan.py` & `qase_api_client-1.0.1/test/test_qql_plan.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_qql_test_case.py` & `qase_api_client-1.0.1/test/test_qql_test_case.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_requirement.py` & `qase_api_client-1.0.1/test/test_requirement.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_response.py` & `qase_api_client-1.0.1/test/test_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result.py` & `qase_api_client-1.0.1/test/test_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_create.py` & `qase_api_client-1.0.1/test/test_result_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_create_bulk.py` & `qase_api_client-1.0.1/test/test_result_create_bulk.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_create_case.py` & `qase_api_client-1.0.1/test/test_result_create_case.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_create_response.py` & `qase_api_client-1.0.1/test/test_result_create_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_create_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_result_create_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_list_response.py` & `qase_api_client-1.0.1/test/test_result_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_result_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_response.py` & `qase_api_client-1.0.1/test/test_result_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_result_update.py` & `qase_api_client-1.0.1/test/test_result_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_resultcreate_bulk.py` & `qase_api_client-1.0.1/test/test_resultcreate_bulk.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_results_api.py` & `qase_api_client-1.0.1/test/test_results_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run.py` & `qase_api_client-1.0.1/test/test_run.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_create.py` & `qase_api_client-1.0.1/test/test_run_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_environment.py` & `qase_api_client-1.0.1/test/test_run_environment.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_list_response.py` & `qase_api_client-1.0.1/test/test_run_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_run_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_milestone.py` & `qase_api_client-1.0.1/test/test_run_milestone.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_public.py` & `qase_api_client-1.0.1/test/test_run_public.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_public_response.py` & `qase_api_client-1.0.1/test/test_run_public_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_public_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_run_public_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_response.py` & `qase_api_client-1.0.1/test/test_run_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_run_stats.py` & `qase_api_client-1.0.1/test/test_run_stats.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_runs_api.py` & `qase_api_client-1.0.1/test/test_runs_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_search_api.py` & `qase_api_client-1.0.1/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_search_response.py` & `qase_api_client-1.0.1/test/test_search_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_search_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_search_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_search_response_all_of_result_entities.py` & `qase_api_client-1.0.1/test/test_search_response_all_of_result_entities.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step.py` & `qase_api_client-1.0.1/test/test_shared_step.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step_content.py` & `qase_api_client-1.0.1/test/test_shared_step_content.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step_content_create.py` & `qase_api_client-1.0.1/test/test_shared_step_content_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step_create.py` & `qase_api_client-1.0.1/test/test_shared_step_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step_list_response.py` & `qase_api_client-1.0.1/test/test_shared_step_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_shared_step_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step_response.py` & `qase_api_client-1.0.1/test/test_shared_step_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_step_update.py` & `qase_api_client-1.0.1/test/test_shared_step_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_shared_steps_api.py` & `qase_api_client-1.0.1/test/test_shared_steps_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suite.py` & `qase_api_client-1.0.1/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suite_create.py` & `qase_api_client-1.0.1/test/test_suite_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suite_delete.py` & `qase_api_client-1.0.1/test/test_suite_delete.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suite_list_response.py` & `qase_api_client-1.0.1/test/test_suite_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suite_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_suite_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suite_response.py` & `qase_api_client-1.0.1/test/test_suite_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suite_update.py` & `qase_api_client-1.0.1/test/test_suite_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_suites_api.py` & `qase_api_client-1.0.1/test/test_suites_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_system_field.py` & `qase_api_client-1.0.1/test/test_system_field.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_system_field_list_response.py` & `qase_api_client-1.0.1/test/test_system_field_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_system_field_option.py` & `qase_api_client-1.0.1/test/test_system_field_option.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_system_fields_api.py` & `qase_api_client-1.0.1/test/test_system_fields_api.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_tag_value.py` & `qase_api_client-1.0.1/test/test_tag_value.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case.py` & `qase_api_client-1.0.1/test/test_test_case.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_create.py` & `qase_api_client-1.0.1/test/test_test_case_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_external_issues.py` & `qase_api_client-1.0.1/test/test_test_case_external_issues.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_external_issues_links_inner.py` & `qase_api_client-1.0.1/test/test_test_case_external_issues_links_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_list_response.py` & `qase_api_client-1.0.1/test/test_test_case_list_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_list_response_all_of_result.py` & `qase_api_client-1.0.1/test/test_test_case_list_response_all_of_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_params.py` & `qase_api_client-1.0.1/test/test_test_case_params.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_query.py` & `qase_api_client-1.0.1/test/test_test_case_query.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_response.py` & `qase_api_client-1.0.1/test/test_test_case_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_case_update.py` & `qase_api_client-1.0.1/test/test_test_case_update.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_casebulk.py` & `qase_api_client-1.0.1/test/test_test_casebulk.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_casebulk_cases_inner.py` & `qase_api_client-1.0.1/test/test_test_casebulk_cases_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_caseexternal_issues.py` & `qase_api_client-1.0.1/test/test_test_caseexternal_issues.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_step.py` & `qase_api_client-1.0.1/test/test_test_step.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_step_create.py` & `qase_api_client-1.0.1/test/test_test_step_create.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_step_result.py` & `qase_api_client-1.0.1/test/test_test_step_result.py`

 * *Files identical despite different names*

### Comparing `qase_api_client-1.0.0b2/test/test_test_step_result_create.py` & `qase_api_client-1.0.1/test/test_test_step_result_create.py`

 * *Files identical despite different names*

