# Comparing `tmp/edgeimpulse_api-1.50.15.tar.gz` & `tmp/edgeimpulse_api-1.50.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.50.15.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.50.6.tar", max compression
```

## Comparing `edgeimpulse_api-1.50.15.tar` & `edgeimpulse_api-1.50.6.tar`

### file list

```diff
@@ -1,951 +1,944 @@
--rw-r--r--   0        0        0      377 2024-06-03 12:25:21.842135 edgeimpulse_api-1.50.15/README.md
--rw-r--r--   0        0        0    91060 2024-06-03 12:26:18.482247 edgeimpulse_api-1.50.15/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     2172 2024-06-03 12:25:21.846135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   383679 2024-06-03 12:25:21.846135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0    11231 2024-06-03 12:25:21.846135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2024-06-03 12:25:21.846135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    67927 2024-06-03 12:25:21.846135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0    72480 2024-06-03 12:25:21.846135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    80789 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   139045 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0    19442 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/email_verification_api.py
--rw-r--r--   0        0        0     6435 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0     5996 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/feature_flags_api.py
--rw-r--r--   0        0        0    11921 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   239795 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   154112 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2024-06-03 12:25:21.850135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    17897 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    85275 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   197840 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    92715 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   331750 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    80882 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_data_campaigns_api.py
--rw-r--r--   0        0        0    58661 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    53291 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2024-06-03 12:25:21.854135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   505508 2024-06-03 12:25:21.870135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    60377 2024-06-03 12:25:21.870135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0   276748 2024-06-03 12:25:21.870135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   420887 2024-06-03 12:25:21.870135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    35671 2024-06-03 12:25:21.870135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2024-06-03 12:25:21.870135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45692 2024-06-03 12:25:21.870135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   276756 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    88434 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1982 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/activate_user_or_verify_email_request.py
--rw-r--r--   0        0        0     2052 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2299 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2122 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
--rw-r--r--   0        0        0     2806 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2794 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     2469 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2152 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     4230 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2359 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2042 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
--rw-r--r--   0        0        0     2269 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     4940 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     6169 2024-06-03 12:25:21.874135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2659 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_project_api_key_request.py
--rw-r--r--   0        0        0     2370 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     2123 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/additional_metric.py
--rw-r--r--   0        0        0     1940 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
--rw-r--r--   0        0        0     1961 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2661 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_organization_api_key_request.py
--rw-r--r--   0        0        0     2542 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_organization_user_request.py
--rw-r--r--   0        0        0     2246 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
--rw-r--r--   0        0        0     2344 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_project_api_key_request.py
--rw-r--r--   0        0        0     2044 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     2146 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     2097 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_user_request.py
--rw-r--r--   0        0        0     6067 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3259 2024-06-03 12:25:21.878136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     7529 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     5318 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2386 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_create_organization_data_export_request.py
--rw-r--r--   0        0        0     2262 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     2718 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_create_project_request.py
--rw-r--r--   0        0        0     1905 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_enable_feature_request.py
--rw-r--r--   0        0        0     2546 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migration_response.py
--rw-r--r--   0        0        0     2222 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
--rw-r--r--   0        0        0     2735 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migrations_response.py
--rw-r--r--   0        0        0     2428 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
--rw-r--r--   0        0        0     2318 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
--rw-r--r--   0        0        0     2022 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
--rw-r--r--   0        0        0     2217 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3148 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
--rw-r--r--   0        0        0     2647 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2323 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
--rw-r--r--   0        0        0     3029 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2729 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     3046 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     3409 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2479 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_trial_response.py
--rw-r--r--   0        0        0     2155 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_trial_response_all_of.py
--rw-r--r--   0        0        0     2208 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     2452 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2807 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     2878 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     4245 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     3084 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     5590 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_start_enterprise_trial_request.py
--rw-r--r--   0        0        0     2031 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_start_enterprise_trial_request_all_of.py
--rw-r--r--   0        0        0     2158 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_toggle_data_migration_request.py
--rw-r--r--   0        0        0     2397 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_organization_data_export_request.py
--rw-r--r--   0        0        0     3936 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2504 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_trial_request.py
--rw-r--r--   0        0        0     2015 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2830 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2525 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0      512 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_capacity.py
--rw-r--r--   0        0        0     2512 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_gmm_metadata.py
--rw-r--r--   0        0        0     2212 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
--rw-r--r--   0        0        0     5499 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     5221 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
--rw-r--r--   0        0        0     2151 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
--rw-r--r--   0        0        0     4079 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3188 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_result.py
--rw-r--r--   0        0        0     3029 2024-06-03 12:25:21.882135 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     3358 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/application_budget.py
--rw-r--r--   0        0        0      506 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     2449 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/auto_labeler_segment.py
--rw-r--r--   0        0        0     1895 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0      499 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/billing_cycle.py
--rw-r--r--   0        0        0      505 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/block_display_category.py
--rw-r--r--   0        0        0      604 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/block_type.py
--rw-r--r--   0        0        0     2044 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2459 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
--rw-r--r--   0        0        0     2041 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     5025 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     4725 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     2996 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of_additional_metrics_by_learn_block.py
--rw-r--r--   0        0        0     3255 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     4064 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_for_variants200_response.py
--rw-r--r--   0        0        0     4026 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3759 2024-06-03 12:25:21.886136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     6252 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2755 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3984 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_multiple_variants.py
--rw-r--r--   0        0        0     3706 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_multiple_variants_all_of.py
--rw-r--r--   0        0        0     2768 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_variant_results.py
--rw-r--r--   0        0        0     3816 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_v2200_response.py
--rw-r--r--   0        0        0     3004 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     3495 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_data.py
--rw-r--r--   0        0        0     3114 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_issue.py
--rw-r--r--   0        0        0     3241 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
--rw-r--r--   0        0        0     2484 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
--rw-r--r--   0        0        0     2183 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2850 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_response.py
--rw-r--r--   0        0        0     2319 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
--rw-r--r--   0        0        0     6569 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_user_request.py
--rw-r--r--   0        0        0     4092 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
--rw-r--r--   0        0        0     2491 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2155 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_usage_report_body.py
--rw-r--r--   0        0        0     2185 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     4834 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_pro_tier_user_request.py
--rw-r--r--   0        0        0     2434 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_pro_tier_user_request_all_of.py
--rw-r--r--   0        0        0     2504 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     4197 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4384 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2094 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/created_updated_by_user.py
--rw-r--r--   0        0        0     2051 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     2368 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/cross_validation_data.py
--rw-r--r--   0        0        0     3412 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/cross_validation_data_scores_inner.py
--rw-r--r--   0        0        0     4054 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign.py
--rw-r--r--   0        0        0     2989 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_dashboard.py
--rw-r--r--   0        0        0     2786 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_graph.py
--rw-r--r--   0        0        0     3352 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
--rw-r--r--   0        0        0     2047 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
--rw-r--r--   0        0        0     1934 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_link.py
--rw-r--r--   0        0        0     1957 2024-06-03 12:25:21.890136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_query.py
--rw-r--r--   0        0        0     3292 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2379 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/delete_user_request.py
--rw-r--r--   0        0        0     2230 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2408 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4397 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5950 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      755 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2248 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_created_response.py
--rw-r--r--   0        0        0     2032 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_request.py
--rw-r--r--   0        0        0     2134 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_request_update.py
--rw-r--r--   0        0        0     2113 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_response.py
--rw-r--r--   0        0        0     2864 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2564 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     4816 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0      516 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_debug_stream_type.py
--rw-r--r--   0        0        0     2811 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_inference_info.py
--rw-r--r--   0        0        0     2199 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     3660 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     4216 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2024-06-03 12:25:21.898136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4848 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2376 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5462 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5820 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     1963 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_named_axis.py
--rw-r--r--   0        0        0     3019 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3697 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3418 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4579 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     4312 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     4224 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/enterprise_trial.py
--rw-r--r--   0        0        0     2960 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
--rw-r--r--   0        0        0     2885 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/entitlement_limits.py
--rw-r--r--   0        0        0     2367 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/entity_created_response.py
--rw-r--r--   0        0        0     2077 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/entity_created_response_all_of.py
--rw-r--r--   0        0        0     2656 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2366 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_block_response.py
--rw-r--r--   0        0        0     2060 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_block_response_all_of.py
--rw-r--r--   0        0        0     2511 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2116 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_keras_block_data_request.py
--rw-r--r--   0        0        0     2373 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0      586 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/feature.py
--rw-r--r--   0        0        0     2206 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2764 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_imported_from_response.py
--rw-r--r--   0        0        0     2457 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
--rw-r--r--   0        0        0     2156 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
--rw-r--r--   0        0        0     2698 2024-06-03 12:25:21.902136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3527 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response.py
--rw-r--r--   0        0        0     3260 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
--rw-r--r--   0        0        0     2588 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
--rw-r--r--   0        0        0     2183 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
--rw-r--r--   0        0        0     3237 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_segment_info_response.py
--rw-r--r--   0        0        0     2948 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_segment_info_response_all_of.py
--rw-r--r--   0        0        0     2345 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
--rw-r--r--   0        0        0     2078 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
--rw-r--r--   0        0        0     3400 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     2752 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response.py
--rw-r--r--   0        0        0     2455 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response_all_of.py
--rw-r--r--   0        0        0     4251 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
--rw-r--r--   0        0        0     2859 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
--rw-r--r--   0        0        0     2456 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_code_response.py
--rw-r--r--   0        0        0     2177 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
--rw-r--r--   0        0        0     2350 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_status_response.py
--rw-r--r--   0        0        0     2045 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
--rw-r--r--   0        0        0     2788 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_feature_flags_response.py
--rw-r--r--   0        0        0     2488 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_feature_flags_response_all_of.py
--rw-r--r--   0        0        0     2118 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
--rw-r--r--   0        0        0     3930 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2429 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_records_request.py
--rw-r--r--   0        0        0     2007 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_records_request_range.py
--rw-r--r--   0        0        0     2454 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     3070 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2580 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_label_noise_data_response.py
--rw-r--r--   0        0        0     2256 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
--rw-r--r--   0        0        0     3358 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
--rw-r--r--   0        0        0     3578 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     3300 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2887 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_model_variants_response.py
--rw-r--r--   0        0        0     2597 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_model_variants_response_all_of.py
--rw-r--r--   0        0        0     2572 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2556 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_bucket_response.py
--rw-r--r--   0        0        0     2232 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2701 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2377 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     2890 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
--rw-r--r--   0        0        0     2583 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
--rw-r--r--   0        0        0     3158 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2939 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaigns_response.py
--rw-r--r--   0        0        0     2632 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
--rw-r--r--   0        0        0     2601 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_export_response.py
--rw-r--r--   0        0        0     2277 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
--rw-r--r--   0        0        0     2982 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_exports_response.py
--rw-r--r--   0        0        0     2682 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
--rw-r--r--   0        0        0     2561 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2024-06-03 12:25:21.906136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3532 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2690 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2373 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
--rw-r--r--   0        0        0     2627 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2310 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
--rw-r--r--   0        0        0     2603 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2906 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     2589 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2541 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2612 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2905 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     4031 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2694 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_target_constraints_response.py
--rw-r--r--   0        0        0     2404 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_target_constraints_response_all_of.py
--rw-r--r--   0        0        0     2414 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3543 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     3276 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0    10235 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     7461 2024-06-03 12:25:21.910136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0      642 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/image_input_scaling.py
--rw-r--r--   0        0        0     3738 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8958 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2627 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2323 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     4172 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     2066 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_created_by_user.py
--rw-r--r--   0        0        0     5203 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details.py
--rw-r--r--   0        0        0     2736 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details_all_of.py
--rw-r--r--   0        0        0     2613 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details_response.py
--rw-r--r--   0        0        0     2316 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details_response_all_of.py
--rw-r--r--   0        0        0     2257 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_failure_details.py
--rw-r--r--   0        0        0     2657 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_logs_response.py
--rw-r--r--   0        0        0     2350 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_logs_response_all_of.py
--rw-r--r--   0        0        0     3297 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_metrics_response.py
--rw-r--r--   0        0        0     3007 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_metrics_response_all_of.py
--rw-r--r--   0        0        0      546 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_parent_type_enum.py
--rw-r--r--   0        0        0     2944 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_state.py
--rw-r--r--   0        0        0     1966 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_state_execution_details.py
--rw-r--r--   0        0        0      598 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_status.py
--rw-r--r--   0        0        0     2965 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_step.py
--rw-r--r--   0        0        0     2713 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     1961 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py
--rw-r--r--   0        0        0     1993 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_custom_metric.py
--rw-r--r--   0        0        0     2510 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5436 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     5169 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     6114 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     4495 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2024-06-03 12:25:21.914136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      635 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_mode.py
--rw-r--r--   0        0        0      562 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0      524 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_variant_enum.py
--rw-r--r--   0        0        0    11377 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0    11110 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2024-06-03 12:25:21.918136 edgeimpulse_api-1.50.15/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     3482 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      933 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2619 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2312 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2767 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_enterprise_trials_response.py
--rw-r--r--   0        0        0     2467 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
--rw-r--r--   0        0        0     2813 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2752 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2445 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2902 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2857 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2819 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2024-06-03 12:25:21.958137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2988 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2688 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     2786 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     2512 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2872 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2593 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     3122 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2822 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2553 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     2615 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_tuner_runs_response.py
--rw-r--r--   0        0        0     2308 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
--rw-r--r--   0        0        0     3933 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2367 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_analytics_event_request.py
--rw-r--r--   0        0        0     2900 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2528 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/memory_spec.py
--rw-r--r--   0        0        0     2746 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/metrics_all_variants_response.py
--rw-r--r--   0        0        0     2449 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2128 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/metrics_for_model_variant.py
--rw-r--r--   0        0        0     2430 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/migration.py
--rw-r--r--   0        0        0      571 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_engine_short_enum.py
--rw-r--r--   0        0        0     3010 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2784 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/neighbors_data.py
--rw-r--r--   0        0        0     3584 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/neighbors_score.py
--rw-r--r--   0        0        0     2736 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
--rw-r--r--   0        0        0     2687 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      775 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6491 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6949 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2056 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     5546 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     5279 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3284 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2273 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2749 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2425 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4717 2024-06-03 12:25:21.962137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     5965 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2700 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     2835 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_dataset_request.py
--rw-r--r--   0        0        0     2493 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
--rw-r--r--   0        0        0     2820 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_bucket.py
--rw-r--r--   0        0        0     2711 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_compute_time_usage.py
--rw-r--r--   0        0        0     9492 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0      605 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
--rw-r--r--   0        0        0     2262 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_path_filter.py
--rw-r--r--   0        0        0     7464 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2754 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0    10387 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2744 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     3483 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     2559 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_request.py
--rw-r--r--   0        0        0     2327 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
--rw-r--r--   0        0        0     3041 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_response.py
--rw-r--r--   0        0        0     2741 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
--rw-r--r--   0        0        0     2468 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
--rw-r--r--   0        0        0     3483 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_export.py
--rw-r--r--   0        0        0     3476 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2303 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     4007 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     2800 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_dataset_bucket.py
--rw-r--r--   0        0        0     6005 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     4962 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     7063 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     6864 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     6574 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     3915 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
--rw-r--r--   0        0        0     2267 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
--rw-r--r--   0        0        0     2338 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
--rw-r--r--   0        0        0     2458 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0     2101 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_performance.py
--rw-r--r--   0        0        0      525 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_member_role.py
--rw-r--r--   0        0        0     2639 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     4480 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6143 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4129 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     5330 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     6532 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     7562 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     8670 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3918 2024-06-03 12:25:21.970137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     3351 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_usage_report.py
--rw-r--r--   0        0        0     5030 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2294 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_user_all_of.py
--rw-r--r--   0        0        0     2104 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1870 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2491 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2537 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2403 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/preview_default_files_in_folder_request.py
--rw-r--r--   0        0        0     3734 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/preview_default_files_in_folder_response.py
--rw-r--r--   0        0        0     3467 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2955 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     3117 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     3042 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     7873 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     4693 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6854 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1943 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_dismiss_notification_request.py
--rw-r--r--   0        0        0     2680 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    14783 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    14516 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     4174 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     3200 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     2715 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_model_variant.py
--rw-r--r--   0        0        0     3554 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4127 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0      576 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_tier_enum.py
--rw-r--r--   0        0        0     2804 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2487 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0     2253 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
--rw-r--r--   0        0        0      606 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_type.py
--rw-r--r--   0        0        0     2316 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0      504 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_visibility.py
--rw-r--r--   0        0        0     4991 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/public_organization_transformation_block.py
--rw-r--r--   0        0        0      588 2024-06-03 12:25:21.974137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/public_project_tier_availability.py
--rw-r--r--   0        0        0     2664 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     2028 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/request_email_verification_request.py
--rw-r--r--   0        0        0     1873 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1896 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/resource_range.py
--rw-r--r--   0        0        0     1985 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2421 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/run_auto_labeler_request.py
--rw-r--r--   0        0        0     2669 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0    11134 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2517 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
--rw-r--r--   0        0        0     2071 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
--rw-r--r--   0        0        0     2341 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
--rw-r--r--   0        0        0     2024 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3346 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     9364 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     1905 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     2531 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_sample_structured_labels_request.py
--rw-r--r--   0        0        0     1915 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     2098 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_classify_job_request.py
--rw-r--r--   0        0        0     2292 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_device_debug_stream_response.py
--rw-r--r--   0        0        0     1975 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py
--rw-r--r--   0        0        0     2178 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py
--rw-r--r--   0        0        0     5388 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_enterprise_trial_request.py
--rw-r--r--   0        0        0     2226 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2795 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1926 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/stop_device_debug_stream_request.py
--rw-r--r--   0        0        0     1967 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     3394 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2270 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/structured_label.py
--rw-r--r--   0        0        0     4399 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_constraints.py
--rw-r--r--   0        0        0     2923 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_constraints_device.py
--rw-r--r--   0        0        0     2347 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_memory.py
--rw-r--r--   0        0        0     3751 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_processor.py
--rw-r--r--   0        0        0     2433 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2721 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2024-06-03 12:25:21.978137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     1921 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/time_series_data_point.py
--rw-r--r--   0        0        0     2031 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     5380 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      548 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/transformation_job_operates_on_enum.py
--rw-r--r--   0        0        0      588 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2462 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_run.py
--rw-r--r--   0        0        0     2570 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     4991 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2739 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     1935 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
--rw-r--r--   0        0        0     2211 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_trial_impulse.py
--rw-r--r--   0        0        0     2028 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2882 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2828 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2913 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     4154 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2158 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2977 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2518 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
--rw-r--r--   0        0        0     2881 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2024-06-03 12:25:21.982138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2953 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     5266 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     6072 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0    12462 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2895 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     1865 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_tuner_run_request.py
--rw-r--r--   0        0        0     2641 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2393 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
--rw-r--r--   0        0        0     2237 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
--rw-r--r--   0        0        0     2125 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2155 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
--rw-r--r--   0        0        0     2059 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_request.py
--rw-r--r--   0        0        0     2403 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/upgrade_subscription_request.py
--rw-r--r--   0        0        0     2168 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     4478 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     1956 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
--rw-r--r--   0        0        0     1922 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_dismiss_notification_request.py
--rw-r--r--   0        0        0     2192 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     2425 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
--rw-r--r--   0        0        0     2119 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
--rw-r--r--   0        0        0     4725 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0      686 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_projects_sort_order.py
--rw-r--r--   0        0        0     2144 2024-06-03 12:25:21.986137 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
--rw-r--r--   0        0        0     2480 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
--rw-r--r--   0        0        0     2191 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
--rw-r--r--   0        0        0     2695 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_subscription_metrics_response.py
--rw-r--r--   0        0        0     2398 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_subscription_metrics_response_all_of.py
--rw-r--r--   0        0        0     3225 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_subscription_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0      573 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_tier_enum.py
--rw-r--r--   0        0        0     1844 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     3049 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2633 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_email_response.py
--rw-r--r--   0        0        0     2354 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_email_response_all_of.py
--rw-r--r--   0        0        0     2708 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     3432 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     3155 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1961 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
--rw-r--r--   0        0        0     1937 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     8565 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2085 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
--rw-r--r--   0        0        0     2120 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
--rw-r--r--   0        0        0     2885 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2024-06-03 12:25:21.990138 edgeimpulse_api-1.50.15/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0     1020 2024-06-03 12:26:18.478247 edgeimpulse_api-1.50.15/pyproject.toml
--rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 edgeimpulse_api-1.50.15/PKG-INFO
+-rw-r--r--   0        0        0      377 2024-05-23 15:15:15.651653 edgeimpulse_api-1.50.6/README.md
+-rw-r--r--   0        0        0    90385 2024-05-23 15:16:18.866267 edgeimpulse_api-1.50.6/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-23 15:15:15.651653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   385743 2024-05-23 15:15:15.655653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0    11231 2024-05-23 15:15:15.655653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2024-05-23 15:15:15.655653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    67927 2024-05-23 15:15:15.655653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0    72480 2024-05-23 15:15:15.655653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    80789 2024-05-23 15:15:15.655653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   139045 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0    19442 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/email_verification_api.py
+-rw-r--r--   0        0        0     6435 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0     5996 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/feature_flags_api.py
+-rw-r--r--   0        0        0    11921 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   239795 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   154112 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    17897 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    85275 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   197840 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    92715 2024-05-23 15:15:15.659653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   331750 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    80882 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_data_campaigns_api.py
+-rw-r--r--   0        0        0    58661 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    53291 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   505317 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    60377 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0   276748 2024-05-23 15:15:15.663653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   420887 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    35671 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45692 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   270581 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    87760 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1982 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/activate_user_or_verify_email_request.py
+-rw-r--r--   0        0        0     2052 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2299 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2122 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2806 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2794 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     2469 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2152 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     4230 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2359 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2042 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
+-rw-r--r--   0        0        0     2269 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2024-05-23 15:15:15.667653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     4940 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     6169 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2659 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_project_api_key_request.py
+-rw-r--r--   0        0        0     2370 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     1940 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
+-rw-r--r--   0        0        0     1961 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2661 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2542 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_organization_user_request.py
+-rw-r--r--   0        0        0     2246 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
+-rw-r--r--   0        0        0     2344 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_project_api_key_request.py
+-rw-r--r--   0        0        0     2044 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2146 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     2097 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_user_request.py
+-rw-r--r--   0        0        0     6067 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3259 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     7529 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     5318 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2386 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_create_organization_data_export_request.py
+-rw-r--r--   0        0        0     2262 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     2718 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_create_project_request.py
+-rw-r--r--   0        0        0     1905 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_enable_feature_request.py
+-rw-r--r--   0        0        0     2546 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migration_response.py
+-rw-r--r--   0        0        0     2222 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
+-rw-r--r--   0        0        0     2735 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migrations_response.py
+-rw-r--r--   0        0        0     2428 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
+-rw-r--r--   0        0        0     2318 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
+-rw-r--r--   0        0        0     2022 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
+-rw-r--r--   0        0        0     2217 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3148 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
+-rw-r--r--   0        0        0     2647 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2323 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
+-rw-r--r--   0        0        0     3029 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2729 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     3046 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     3409 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     2452 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2507 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_trial_response.py
+-rw-r--r--   0        0        0     2183 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
+-rw-r--r--   0        0        0     2807 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     2878 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     4245 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     3084 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2158 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_toggle_data_migration_request.py
+-rw-r--r--   0        0        0     2397 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_organization_data_export_request.py
+-rw-r--r--   0        0        0     3936 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2830 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2532 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_user_trial_request.py
+-rw-r--r--   0        0        0     2525 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0      512 2024-05-23 15:15:15.671653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_capacity.py
+-rw-r--r--   0        0        0     2512 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_gmm_metadata.py
+-rw-r--r--   0        0        0     2212 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
+-rw-r--r--   0        0        0     5499 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     5221 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
+-rw-r--r--   0        0        0     2151 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
+-rw-r--r--   0        0        0     4079 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3188 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_result.py
+-rw-r--r--   0        0        0     3029 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     3358 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/application_budget.py
+-rw-r--r--   0        0        0      506 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     2449 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/auto_labeler_segment.py
+-rw-r--r--   0        0        0     1895 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0      499 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/billing_cycle.py
+-rw-r--r--   0        0        0      505 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/block_display_category.py
+-rw-r--r--   0        0        0      604 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/block_type.py
+-rw-r--r--   0        0        0     2044 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2459 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
+-rw-r--r--   0        0        0     2041 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     4041 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3741 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     4064 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_for_variants200_response.py
+-rw-r--r--   0        0        0     4026 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3759 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     6252 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2755 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3984 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_multiple_variants.py
+-rw-r--r--   0        0        0     3706 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_multiple_variants_all_of.py
+-rw-r--r--   0        0        0     2768 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_variant_results.py
+-rw-r--r--   0        0        0     3816 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_v2200_response.py
+-rw-r--r--   0        0        0     3004 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     3495 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_data.py
+-rw-r--r--   0        0        0     3114 2024-05-23 15:15:15.675653 edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_issue.py
+-rw-r--r--   0        0        0     3241 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
+-rw-r--r--   0        0        0     2484 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
+-rw-r--r--   0        0        0     2183 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2850 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_response.py
+-rw-r--r--   0        0        0     2319 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
+-rw-r--r--   0        0        0     6569 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_user_request.py
+-rw-r--r--   0        0        0     4092 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
+-rw-r--r--   0        0        0     2491 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2155 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_usage_report_body.py
+-rw-r--r--   0        0        0     2185 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2504 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     4446 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4384 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2094 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/created_updated_by_user.py
+-rw-r--r--   0        0        0     2051 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     2368 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/cross_validation_data.py
+-rw-r--r--   0        0        0     3412 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/cross_validation_data_scores_inner.py
+-rw-r--r--   0        0        0     4054 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign.py
+-rw-r--r--   0        0        0     2989 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_dashboard.py
+-rw-r--r--   0        0        0     2786 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_graph.py
+-rw-r--r--   0        0        0     3352 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
+-rw-r--r--   0        0        0     2047 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
+-rw-r--r--   0        0        0     1934 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_link.py
+-rw-r--r--   0        0        0     1957 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_query.py
+-rw-r--r--   0        0        0     3292 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2379 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/delete_user_request.py
+-rw-r--r--   0        0        0     2230 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2408 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4397 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5950 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2024-05-23 15:15:15.715652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      755 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2248 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_created_response.py
+-rw-r--r--   0        0        0     2032 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_request.py
+-rw-r--r--   0        0        0     2134 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_request_update.py
+-rw-r--r--   0        0        0     2113 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_response.py
+-rw-r--r--   0        0        0     2864 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2564 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     4816 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0      516 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_debug_stream_type.py
+-rw-r--r--   0        0        0     2811 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_inference_info.py
+-rw-r--r--   0        0        0     2199 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     3660 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     4216 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4848 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2376 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5462 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5820 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     1963 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_named_axis.py
+-rw-r--r--   0        0        0     3019 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3697 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3418 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4579 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     4312 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     4235 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/enterprise_trial.py
+-rw-r--r--   0        0        0     2960 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
+-rw-r--r--   0        0        0     2885 2024-05-23 15:15:15.719652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/entitlement_limits.py
+-rw-r--r--   0        0        0     2367 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/entity_created_response.py
+-rw-r--r--   0        0        0     2077 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/entity_created_response_all_of.py
+-rw-r--r--   0        0        0     2656 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2366 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_block_response.py
+-rw-r--r--   0        0        0     2060 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_block_response_all_of.py
+-rw-r--r--   0        0        0     2511 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2116 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_keras_block_data_request.py
+-rw-r--r--   0        0        0     2373 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0      586 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/feature.py
+-rw-r--r--   0        0        0     2206 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2764 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_imported_from_response.py
+-rw-r--r--   0        0        0     2457 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
+-rw-r--r--   0        0        0     2156 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
+-rw-r--r--   0        0        0     2698 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3527 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response.py
+-rw-r--r--   0        0        0     3260 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
+-rw-r--r--   0        0        0     2588 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
+-rw-r--r--   0        0        0     2183 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
+-rw-r--r--   0        0        0     3237 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_segment_info_response.py
+-rw-r--r--   0        0        0     2948 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_segment_info_response_all_of.py
+-rw-r--r--   0        0        0     2345 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
+-rw-r--r--   0        0        0     2078 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
+-rw-r--r--   0        0        0     3400 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     2752 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response.py
+-rw-r--r--   0        0        0     2455 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response_all_of.py
+-rw-r--r--   0        0        0     4251 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
+-rw-r--r--   0        0        0     2859 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2456 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_code_response.py
+-rw-r--r--   0        0        0     2177 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
+-rw-r--r--   0        0        0     2350 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_status_response.py
+-rw-r--r--   0        0        0     2045 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
+-rw-r--r--   0        0        0     2788 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_feature_flags_response.py
+-rw-r--r--   0        0        0     2488 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_feature_flags_response_all_of.py
+-rw-r--r--   0        0        0     2118 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
+-rw-r--r--   0        0        0     3930 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2429 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_records_request.py
+-rw-r--r--   0        0        0     2007 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_records_request_range.py
+-rw-r--r--   0        0        0     2454 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     3070 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2580 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_label_noise_data_response.py
+-rw-r--r--   0        0        0     2256 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
+-rw-r--r--   0        0        0     3358 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
+-rw-r--r--   0        0        0     3578 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     3300 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2887 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_model_variants_response.py
+-rw-r--r--   0        0        0     2597 2024-05-23 15:15:15.723652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_model_variants_response_all_of.py
+-rw-r--r--   0        0        0     2572 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2556 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_bucket_response.py
+-rw-r--r--   0        0        0     2232 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2701 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2377 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     2890 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
+-rw-r--r--   0        0        0     2583 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
+-rw-r--r--   0        0        0     3158 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2939 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaigns_response.py
+-rw-r--r--   0        0        0     2632 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
+-rw-r--r--   0        0        0     2601 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_export_response.py
+-rw-r--r--   0        0        0     2277 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
+-rw-r--r--   0        0        0     2982 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_exports_response.py
+-rw-r--r--   0        0        0     2682 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
+-rw-r--r--   0        0        0     2561 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3532 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2690 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2373 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
+-rw-r--r--   0        0        0     2627 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2310 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
+-rw-r--r--   0        0        0     2603 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2906 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     2589 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2541 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2612 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2905 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     4031 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2694 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_target_constraints_response.py
+-rw-r--r--   0        0        0     2404 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_target_constraints_response_all_of.py
+-rw-r--r--   0        0        0     2414 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3543 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     3276 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0    10235 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     7461 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2024-05-23 15:15:15.727652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0      642 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/image_input_scaling.py
+-rw-r--r--   0        0        0     3738 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8958 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2627 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2323 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     4172 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     2066 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_created_by_user.py
+-rw-r--r--   0        0        0     5203 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details.py
+-rw-r--r--   0        0        0     2736 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details_all_of.py
+-rw-r--r--   0        0        0     2613 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details_response.py
+-rw-r--r--   0        0        0     2316 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details_response_all_of.py
+-rw-r--r--   0        0        0     2257 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_failure_details.py
+-rw-r--r--   0        0        0     2657 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_logs_response.py
+-rw-r--r--   0        0        0     2350 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_logs_response_all_of.py
+-rw-r--r--   0        0        0     3297 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_metrics_response.py
+-rw-r--r--   0        0        0     3007 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_metrics_response_all_of.py
+-rw-r--r--   0        0        0      546 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_parent_type_enum.py
+-rw-r--r--   0        0        0     2944 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_state.py
+-rw-r--r--   0        0        0     1966 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_state_execution_details.py
+-rw-r--r--   0        0        0      598 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_status.py
+-rw-r--r--   0        0        0     2965 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_step.py
+-rw-r--r--   0        0        0     2713 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     1961 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py
+-rw-r--r--   0        0        0     1993 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_custom_metric.py
+-rw-r--r--   0        0        0     2510 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5707 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     5440 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     5421 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     4495 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0      524 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_variant_enum.py
+-rw-r--r--   0        0        0    11377 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0    11110 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     3482 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      933 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2619 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2312 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2767 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_enterprise_trials_response.py
+-rw-r--r--   0        0        0     2467 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
+-rw-r--r--   0        0        0     2813 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2752 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2445 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2902 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-05-23 15:15:15.731652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2857 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2819 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2988 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2688 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     2786 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     2512 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2872 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2593 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     3122 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2822 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2553 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     2615 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_tuner_runs_response.py
+-rw-r--r--   0        0        0     2308 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
+-rw-r--r--   0        0        0     3933 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2367 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_analytics_event_request.py
+-rw-r--r--   0        0        0     2900 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2528 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/memory_spec.py
+-rw-r--r--   0        0        0     2746 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/metrics_all_variants_response.py
+-rw-r--r--   0        0        0     2449 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2128 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/metrics_for_model_variant.py
+-rw-r--r--   0        0        0     2430 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/migration.py
+-rw-r--r--   0        0        0      571 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_engine_short_enum.py
+-rw-r--r--   0        0        0     3010 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2784 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/neighbors_data.py
+-rw-r--r--   0        0        0     3584 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/neighbors_score.py
+-rw-r--r--   0        0        0     2736 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
+-rw-r--r--   0        0        0     2687 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2024-05-23 15:15:15.735652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      775 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6491 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6949 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2056 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     5546 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     5279 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3284 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2273 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2749 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2425 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4717 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     5965 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2700 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2835 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2493 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2820 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_bucket.py
+-rw-r--r--   0        0        0     2711 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_compute_time_usage.py
+-rw-r--r--   0        0        0     9492 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0      605 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
+-rw-r--r--   0        0        0     2262 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_path_filter.py
+-rw-r--r--   0        0        0     7464 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2754 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0    10387 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2744 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3483 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     2559 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_request.py
+-rw-r--r--   0        0        0     2327 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
+-rw-r--r--   0        0        0     3041 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_response.py
+-rw-r--r--   0        0        0     2741 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
+-rw-r--r--   0        0        0     2468 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
+-rw-r--r--   0        0        0     3483 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_export.py
+-rw-r--r--   0        0        0     3476 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2303 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     4007 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2800 2024-05-23 15:15:15.739652 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     6005 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     4962 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     7063 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     6864 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     6574 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     3915 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
+-rw-r--r--   0        0        0     2267 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
+-rw-r--r--   0        0        0     2338 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
+-rw-r--r--   0        0        0     2458 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0     2101 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_performance.py
+-rw-r--r--   0        0        0      525 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_member_role.py
+-rw-r--r--   0        0        0     2639 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     4480 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6143 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4129 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5330 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     6532 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     7562 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     8670 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3918 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     3351 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_usage_report.py
+-rw-r--r--   0        0        0     5030 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2294 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_user_all_of.py
+-rw-r--r--   0        0        0     2104 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1839 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2491 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2537 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2403 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/preview_default_files_in_folder_request.py
+-rw-r--r--   0        0        0     3734 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/preview_default_files_in_folder_response.py
+-rw-r--r--   0        0        0     3467 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2955 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     3117 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     3042 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     7873 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     4693 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6854 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1943 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2680 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2024-05-23 15:15:15.743651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    14783 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    14516 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     4174 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     3200 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     2715 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_model_variant.py
+-rw-r--r--   0        0        0     3554 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4127 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0      576 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_tier_enum.py
+-rw-r--r--   0        0        0     2804 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2487 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0     2253 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
+-rw-r--r--   0        0        0      606 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_type.py
+-rw-r--r--   0        0        0     2316 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0      504 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_visibility.py
+-rw-r--r--   0        0        0     4991 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/public_organization_transformation_block.py
+-rw-r--r--   0        0        0      588 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/public_project_tier_availability.py
+-rw-r--r--   0        0        0     2664 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     2028 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/request_email_verification_request.py
+-rw-r--r--   0        0        0     1873 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1896 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/resource_range.py
+-rw-r--r--   0        0        0     1985 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2421 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/run_auto_labeler_request.py
+-rw-r--r--   0        0        0     2669 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0    11134 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2517 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
+-rw-r--r--   0        0        0     2071 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
+-rw-r--r--   0        0        0     2341 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
+-rw-r--r--   0        0        0     2024 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3346 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     9364 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     1905 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     2531 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_sample_structured_labels_request.py
+-rw-r--r--   0        0        0     1915 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     2098 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_classify_job_request.py
+-rw-r--r--   0        0        0     2292 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_device_debug_stream_response.py
+-rw-r--r--   0        0        0     1975 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py
+-rw-r--r--   0        0        0     2178 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py
+-rw-r--r--   0        0        0     5388 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_enterprise_trial_request.py
+-rw-r--r--   0        0        0     2226 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2024-05-23 15:15:15.747651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2795 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1926 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/stop_device_debug_stream_request.py
+-rw-r--r--   0        0        0     1967 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     3394 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2270 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/structured_label.py
+-rw-r--r--   0        0        0     4399 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_constraints.py
+-rw-r--r--   0        0        0     2923 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_constraints_device.py
+-rw-r--r--   0        0        0     2347 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_memory.py
+-rw-r--r--   0        0        0     3751 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_processor.py
+-rw-r--r--   0        0        0     2433 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     1921 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/time_series_data_point.py
+-rw-r--r--   0        0        0     2031 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     5380 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      548 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/transformation_job_operates_on_enum.py
+-rw-r--r--   0        0        0      588 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2462 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_run.py
+-rw-r--r--   0        0        0     2570 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     4991 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2739 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     1935 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
+-rw-r--r--   0        0        0     2211 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial_impulse.py
+-rw-r--r--   0        0        0     2028 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2828 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2913 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     4154 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2158 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2977 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2518 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2881 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2953 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     5266 2024-05-23 15:15:15.751651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     6072 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0    12462 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     1865 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_tuner_run_request.py
+-rw-r--r--   0        0        0     2641 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2393 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
+-rw-r--r--   0        0        0     2237 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
+-rw-r--r--   0        0        0     2125 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2155 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
+-rw-r--r--   0        0        0     2059 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_request.py
+-rw-r--r--   0        0        0     2403 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/upgrade_subscription_request.py
+-rw-r--r--   0        0        0     2168 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     4478 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     1956 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     1922 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2192 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     2425 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
+-rw-r--r--   0        0        0     2119 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0     4725 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0      686 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_projects_sort_order.py
+-rw-r--r--   0        0        0     2144 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     2480 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
+-rw-r--r--   0        0        0     2191 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0     2695 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_subscription_metrics_response.py
+-rw-r--r--   0        0        0     2398 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_subscription_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3225 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_subscription_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0      573 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_tier_enum.py
+-rw-r--r--   0        0        0     1844 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     3049 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2633 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_email_response.py
+-rw-r--r--   0        0        0     2354 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_email_response_all_of.py
+-rw-r--r--   0        0        0     2708 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     3432 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     3155 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1961 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
+-rw-r--r--   0        0        0     1937 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     8565 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2085 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
+-rw-r--r--   0        0        0     2120 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
+-rw-r--r--   0        0        0     2885 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2024-05-23 15:15:15.755651 edgeimpulse_api-1.50.6/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0     1019 2024-05-23 15:16:18.862267 edgeimpulse_api-1.50.6/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.50.6/PKG-INFO
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.50.15" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.50.6" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
 from edgeimpulse_api.api.dsp_api import DSPApi
@@ -85,15 +85,14 @@
 from edgeimpulse_api.models.add_organization_transfer_learning_block_request import AddOrganizationTransferLearningBlockRequest
 from edgeimpulse_api.models.add_organization_transfer_learning_block_response import AddOrganizationTransferLearningBlockResponse
 from edgeimpulse_api.models.add_organization_transformation_block_request import AddOrganizationTransformationBlockRequest
 from edgeimpulse_api.models.add_organization_transformation_block_response import AddOrganizationTransformationBlockResponse
 from edgeimpulse_api.models.add_organization_transformation_block_response_all_of import AddOrganizationTransformationBlockResponseAllOf
 from edgeimpulse_api.models.add_project_api_key_request import AddProjectApiKeyRequest
 from edgeimpulse_api.models.add_project_api_key_request_all_of import AddProjectApiKeyRequestAllOf
-from edgeimpulse_api.models.additional_metric import AdditionalMetric
 from edgeimpulse_api.models.admin_add_disallowed_email_domain_request import AdminAddDisallowedEmailDomainRequest
 from edgeimpulse_api.models.admin_add_or_update_sso_domain_id_ps_request import AdminAddOrUpdateSSODomainIdPsRequest
 from edgeimpulse_api.models.admin_add_organization_api_key_request import AdminAddOrganizationApiKeyRequest
 from edgeimpulse_api.models.admin_add_organization_user_request import AdminAddOrganizationUserRequest
 from edgeimpulse_api.models.admin_add_organization_user_request_all_of import AdminAddOrganizationUserRequestAllOf
 from edgeimpulse_api.models.admin_add_project_api_key_request import AdminAddProjectApiKeyRequest
 from edgeimpulse_api.models.admin_add_project_api_key_request_all_of import AdminAddProjectApiKeyRequestAllOf
@@ -125,36 +124,34 @@
 from edgeimpulse_api.models.admin_get_organizations_response_all_of import AdminGetOrganizationsResponseAllOf
 from edgeimpulse_api.models.admin_get_organizations_response_all_of_organizations import AdminGetOrganizationsResponseAllOfOrganizations
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response import AdminGetSSODomainIdPsResponse
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response_all_of import AdminGetSSODomainIdPsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response import AdminGetSSOSettingsResponse
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of import AdminGetSSOSettingsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of_sso_whitelist import AdminGetSSOSettingsResponseAllOfSsoWhitelist
-from edgeimpulse_api.models.admin_get_trial_response import AdminGetTrialResponse
-from edgeimpulse_api.models.admin_get_trial_response_all_of import AdminGetTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response_all_of import AdminGetUserIdsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
 from edgeimpulse_api.models.admin_get_user_response_all_of import AdminGetUserResponseAllOf
+from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
+from edgeimpulse_api.models.admin_get_user_trial_response_all_of import AdminGetUserTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_get_users_response_all_of import AdminGetUsersResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response_all_of_users import AdminGetUsersResponseAllOfUsers
 from edgeimpulse_api.models.admin_list_projects import AdminListProjects
 from edgeimpulse_api.models.admin_list_projects_response import AdminListProjectsResponse
 from edgeimpulse_api.models.admin_organization_info_response import AdminOrganizationInfoResponse
 from edgeimpulse_api.models.admin_organization_info_response_all_of import AdminOrganizationInfoResponseAllOf
-from edgeimpulse_api.models.admin_start_enterprise_trial_request import AdminStartEnterpriseTrialRequest
-from edgeimpulse_api.models.admin_start_enterprise_trial_request_all_of import AdminStartEnterpriseTrialRequestAllOf
 from edgeimpulse_api.models.admin_toggle_data_migration_request import AdminToggleDataMigrationRequest
 from edgeimpulse_api.models.admin_update_organization_data_export_request import AdminUpdateOrganizationDataExportRequest
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
-from edgeimpulse_api.models.admin_update_trial_request import AdminUpdateTrialRequest
 from edgeimpulse_api.models.admin_update_user_permissions_request import AdminUpdateUserPermissionsRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
+from edgeimpulse_api.models.admin_update_user_trial_request import AdminUpdateUserTrialRequest
 from edgeimpulse_api.models.akida_edge_learning_config import AkidaEdgeLearningConfig
 from edgeimpulse_api.models.anomaly_capacity import AnomalyCapacity
 from edgeimpulse_api.models.anomaly_gmm_metadata import AnomalyGmmMetadata
 from edgeimpulse_api.models.anomaly_gmm_metadata_all_of import AnomalyGmmMetadataAllOf
 from edgeimpulse_api.models.anomaly_model_metadata import AnomalyModelMetadata
 from edgeimpulse_api.models.anomaly_model_metadata_all_of import AnomalyModelMetadataAllOf
 from edgeimpulse_api.models.anomaly_model_metadata_all_of_clusters import AnomalyModelMetadataAllOfClusters
@@ -179,15 +176,14 @@
 from edgeimpulse_api.models.build_organization_on_device_model_request import BuildOrganizationOnDeviceModelRequest
 from edgeimpulse_api.models.calculate_data_quality_metrics_request import CalculateDataQualityMetricsRequest
 from edgeimpulse_api.models.change_password_request import ChangePasswordRequest
 from edgeimpulse_api.models.classify_job_response import ClassifyJobResponse
 from edgeimpulse_api.models.classify_job_response_all_of import ClassifyJobResponseAllOf
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy_total_summary import ClassifyJobResponseAllOfAccuracyTotalSummary
-from edgeimpulse_api.models.classify_job_response_all_of_additional_metrics_by_learn_block import ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock
 from edgeimpulse_api.models.classify_job_response_page import ClassifyJobResponsePage
 from edgeimpulse_api.models.classify_job_response_page_all_of import ClassifyJobResponsePageAllOf
 from edgeimpulse_api.models.classify_sample_for_variants200_response import ClassifySampleForVariants200Response
 from edgeimpulse_api.models.classify_sample_response import ClassifySampleResponse
 from edgeimpulse_api.models.classify_sample_response_all_of import ClassifySampleResponseAllOf
 from edgeimpulse_api.models.classify_sample_response_classification import ClassifySampleResponseClassification
 from edgeimpulse_api.models.classify_sample_response_classification_details import ClassifySampleResponseClassificationDetails
@@ -217,16 +213,14 @@
 from edgeimpulse_api.models.create_organization_portal_response import CreateOrganizationPortalResponse
 from edgeimpulse_api.models.create_organization_portal_response_all_of import CreateOrganizationPortalResponseAllOf
 from edgeimpulse_api.models.create_organization_request import CreateOrganizationRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
 from edgeimpulse_api.models.create_organization_response_all_of import CreateOrganizationResponseAllOf
 from edgeimpulse_api.models.create_organization_usage_report_body import CreateOrganizationUsageReportBody
 from edgeimpulse_api.models.create_pipeline_response import CreatePipelineResponse
-from edgeimpulse_api.models.create_pro_tier_user_request import CreateProTierUserRequest
-from edgeimpulse_api.models.create_pro_tier_user_request_all_of import CreateProTierUserRequestAllOf
 from edgeimpulse_api.models.create_project_request import CreateProjectRequest
 from edgeimpulse_api.models.create_project_response import CreateProjectResponse
 from edgeimpulse_api.models.create_project_response_all_of import CreateProjectResponseAllOf
 from edgeimpulse_api.models.create_signed_upload_link_request import CreateSignedUploadLinkRequest
 from edgeimpulse_api.models.create_signed_upload_link_response import CreateSignedUploadLinkResponse
 from edgeimpulse_api.models.create_signed_upload_link_response_all_of import CreateSignedUploadLinkResponseAllOf
 from edgeimpulse_api.models.create_third_party_auth_request import CreateThirdPartyAuthRequest
@@ -533,15 +527,14 @@
 from edgeimpulse_api.models.keras_model_layer_input import KerasModelLayerInput
 from edgeimpulse_api.models.keras_model_layer_output import KerasModelLayerOutput
 from edgeimpulse_api.models.keras_model_metadata import KerasModelMetadata
 from edgeimpulse_api.models.keras_model_metadata_all_of import KerasModelMetadataAllOf
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
 from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner import KerasModelMetadataMetricsOnDevicePerformanceInner
 from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner_tflite import KerasModelMetadataMetricsOnDevicePerformanceInnerTflite
-from edgeimpulse_api.models.keras_model_mode import KerasModelMode
 from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
 from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.keras_response import KerasResponse
 from edgeimpulse_api.models.keras_response_all_of import KerasResponseAllOf
 from edgeimpulse_api.models.keras_visual_layer import KerasVisualLayer
 from edgeimpulse_api.models.keras_visual_layer_type import KerasVisualLayerType
 from edgeimpulse_api.models.last_modification_date_response import LastModificationDateResponse
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/admin_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,28 +36,27 @@
 from edgeimpulse_api.models.admin_get_metrics_response import AdminGetMetricsResponse
 from edgeimpulse_api.models.admin_get_organization_compute_time_usage_response import AdminGetOrganizationComputeTimeUsageResponse
 from edgeimpulse_api.models.admin_get_organization_usage_report_response import AdminGetOrganizationUsageReportResponse
 from edgeimpulse_api.models.admin_get_organization_usage_reports_response import AdminGetOrganizationUsageReportsResponse
 from edgeimpulse_api.models.admin_get_organizations_response import AdminGetOrganizationsResponse
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response import AdminGetSSODomainIdPsResponse
 from edgeimpulse_api.models.admin_get_sso_settings_response import AdminGetSSOSettingsResponse
-from edgeimpulse_api.models.admin_get_trial_response import AdminGetTrialResponse
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
+from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_list_projects_response import AdminListProjectsResponse
 from edgeimpulse_api.models.admin_organization_info_response import AdminOrganizationInfoResponse
-from edgeimpulse_api.models.admin_start_enterprise_trial_request import AdminStartEnterpriseTrialRequest
 from edgeimpulse_api.models.admin_toggle_data_migration_request import AdminToggleDataMigrationRequest
 from edgeimpulse_api.models.admin_update_organization_data_export_request import AdminUpdateOrganizationDataExportRequest
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
-from edgeimpulse_api.models.admin_update_trial_request import AdminUpdateTrialRequest
 from edgeimpulse_api.models.admin_update_user_permissions_request import AdminUpdateUserPermissionsRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
+from edgeimpulse_api.models.admin_update_user_trial_request import AdminUpdateUserTrialRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
 from edgeimpulse_api.models.create_project_response import CreateProjectResponse
 from edgeimpulse_api.models.entity_created_response import EntityCreatedResponse
 from edgeimpulse_api.models.feature import Feature
 from edgeimpulse_api.models.find_user_response import FindUserResponse
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.get_email_verification_code_response import GetEmailVerificationCodeResponse
@@ -65,17 +64,17 @@
 from edgeimpulse_api.models.get_organization_data_export_response import GetOrganizationDataExportResponse
 from edgeimpulse_api.models.get_organization_data_exports_response import GetOrganizationDataExportsResponse
 from edgeimpulse_api.models.job_details_response import JobDetailsResponse
 from edgeimpulse_api.models.job_logs_response import JobLogsResponse
 from edgeimpulse_api.models.job_metrics_response import JobMetricsResponse
 from edgeimpulse_api.models.job_parent_type_enum import JobParentTypeEnum
 from edgeimpulse_api.models.project_info_response import ProjectInfoResponse
+from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.update_project_request import UpdateProjectRequest
-from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
@@ -1518,21 +1517,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_create_trial(self, admin_start_enterprise_trial_request : AdminStartEnterpriseTrialRequest, **kwargs) -> EntityCreatedResponse:  # noqa: E501
+    def admin_create_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], start_enterprise_trial_request : StartEnterpriseTrialRequest, **kwargs) -> EntityCreatedResponse:  # noqa: E501
         """Create user enterprise trial
 
         Admin-only API to create an enterprise trial for a user.
 
-        :param admin_start_enterprise_trial_request: (required)
-        :type admin_start_enterprise_trial_request: AdminStartEnterpriseTrialRequest
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param start_enterprise_trial_request: (required)
+        :type start_enterprise_trial_request: StartEnterpriseTrialRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -1541,24 +1542,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: EntityCreatedResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_create_trial_with_http_info(admin_start_enterprise_trial_request, **kwargs)  # noqa: E501
+        return self._admin_create_user_trial_with_http_info(user_id, start_enterprise_trial_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_create_trial_with_http_info(self, admin_start_enterprise_trial_request : AdminStartEnterpriseTrialRequest, **kwargs):  # noqa: E501
+    def _admin_create_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], start_enterprise_trial_request : StartEnterpriseTrialRequest, **kwargs):  # noqa: E501
         """Create user enterprise trial 
 
         Admin-only API to create an enterprise trial for a user.
 
-        :param admin_start_enterprise_trial_request: (required)
-        :type admin_start_enterprise_trial_request: AdminStartEnterpriseTrialRequest
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param start_enterprise_trial_request: (required)
+        :type start_enterprise_trial_request: StartEnterpriseTrialRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1578,15 +1581,16 @@
                  returns the request thread.
         :rtype: tuple(EntityCreatedResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'admin_start_enterprise_trial_request'
+            'user_id',
+            'start_enterprise_trial_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1597,38 +1601,40 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_create_trial" % _key
+                    " to method admin_create_user_trial" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['admin_start_enterprise_trial_request']:
-            _body_params = _params['admin_start_enterprise_trial_request']
+        if _params['start_enterprise_trial_request']:
+            _body_params = _params['start_enterprise_trial_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1641,15 +1647,15 @@
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "EntityCreatedResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/trials', 'POST',
+            '/api/admin/users/{userId}/trials', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2477,47 +2483,47 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_delete_trial(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Delete enterprise trial
+    def admin_delete_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> StartJobResponse:  # noqa: E501
+        """Delete a user
 
-        Admin-only API to delete an enterprise trial.
+        Admin-only API to delete a user.
 
-        :param enterprise_trial_id: Enterprise trial ID (required)
-        :type enterprise_trial_id: int
+        :param user_id: User ID (required)
+        :type user_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GenericApiResponse
+        :rtype: StartJobResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_delete_trial_with_http_info(enterprise_trial_id, **kwargs)  # noqa: E501
+        return self._admin_delete_user_with_http_info(user_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_delete_trial_with_http_info(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
-        """Delete enterprise trial 
+    def _admin_delete_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
+        """Delete a user 
 
-        Admin-only API to delete an enterprise trial.
+        Admin-only API to delete a user.
 
-        :param enterprise_trial_id: Enterprise trial ID (required)
-        :type enterprise_trial_id: int
+        :param user_id: User ID (required)
+        :type user_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2531,21 +2537,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(StartJobResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'enterprise_trial_id'
+            'user_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -2556,25 +2562,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_delete_trial" % _key
+                    " to method admin_delete_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['enterprise_trial_id']:
-            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -2589,19 +2595,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "GenericApiResponse",
+            '200': "StartJobResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/trials/{enterpriseTrialId}', 'DELETE',
+            '/api/admin/users/{userId}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -2610,47 +2616,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_delete_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> StartJobResponse:  # noqa: E501
-        """Delete a user
+    def admin_delete_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Delete user enterprise trial
 
-        Admin-only API to delete a user.
+        Admin-only API to delete an enterprise trial for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: StartJobResponse
+        :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_delete_user_with_http_info(user_id, **kwargs)  # noqa: E501
+        return self._admin_delete_user_trial_with_http_info(user_id, enterprise_trial_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_delete_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
-        """Delete a user 
+    def _admin_delete_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
+        """Delete user enterprise trial 
 
-        Admin-only API to delete a user.
+        Admin-only API to delete an enterprise trial for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2664,21 +2674,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(StartJobResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'user_id'
+            'user_id',
+            'enterprise_trial_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -2689,25 +2700,27 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_delete_user" % _key
+                    " to method admin_delete_user_trial" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['user_id']:
             _path_params['userId'] = _params['user_id']
+        if _params['enterprise_trial_id']:
+            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -2722,19 +2735,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "StartJobResponse",
+            '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/users/{userId}', 'DELETE',
+            '/api/admin/users/{userId}/trials/{enterpriseTrialId}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -6321,47 +6334,47 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_get_trial(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> AdminGetTrialResponse:  # noqa: E501
-        """Get enterprise trial
+    def admin_get_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> AdminGetUserResponse:  # noqa: E501
+        """Get user
 
-        Admin-only API to get a specific enterprise trial.
+        Admin-only API to get information about a user.
 
-        :param enterprise_trial_id: Enterprise trial ID (required)
-        :type enterprise_trial_id: int
+        :param user_id: User ID (required)
+        :type user_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AdminGetTrialResponse
+        :rtype: AdminGetUserResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_get_trial_with_http_info(enterprise_trial_id, **kwargs)  # noqa: E501
+        return self._admin_get_user_with_http_info(user_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_get_trial_with_http_info(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
-        """Get enterprise trial 
+    def _admin_get_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
+        """Get user 
 
-        Admin-only API to get a specific enterprise trial.
+        Admin-only API to get information about a user.
 
-        :param enterprise_trial_id: Enterprise trial ID (required)
-        :type enterprise_trial_id: int
+        :param user_id: User ID (required)
+        :type user_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -6375,21 +6388,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(AdminGetTrialResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(AdminGetUserResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'enterprise_trial_id'
+            'user_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -6400,25 +6413,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_get_trial" % _key
+                    " to method admin_get_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['enterprise_trial_id']:
-            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -6433,19 +6446,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "AdminGetTrialResponse",
+            '200': "AdminGetUserResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/trials/{enterpriseTrialId}', 'GET',
+            '/api/admin/users/{userId}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -6454,18 +6467,18 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_get_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> AdminGetUserResponse:  # noqa: E501
-        """Get user
+    def admin_get_user_metrics(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> AdminGetUserMetricsResponse:  # noqa: E501
+        """Get user metrics
 
-        Admin-only API to get information about a user.
+        Admin-only API to get marketing metrics about a user.
 
         :param user_id: User ID (required)
         :type user_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -6474,24 +6487,24 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AdminGetUserResponse
+        :rtype: AdminGetUserMetricsResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_get_user_with_http_info(user_id, **kwargs)  # noqa: E501
+        return self._admin_get_user_metrics_with_http_info(user_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_get_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
-        """Get user 
+    def _admin_get_user_metrics_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
+        """Get user metrics 
 
-        Admin-only API to get information about a user.
+        Admin-only API to get marketing metrics about a user.
 
         :param user_id: User ID (required)
         :type user_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -6508,15 +6521,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(AdminGetUserResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(AdminGetUserMetricsResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'user_id'
         ]
@@ -6533,15 +6546,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_get_user" % _key
+                    " to method admin_get_user_metrics" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -6566,19 +6579,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "AdminGetUserResponse",
+            '200': "AdminGetUserMetricsResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/users/{userId}', 'GET',
+            '/api/admin/users/{userId}/metrics', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -6587,47 +6600,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_get_user_metrics(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> AdminGetUserMetricsResponse:  # noqa: E501
-        """Get user metrics
+    def admin_get_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> AdminGetUserTrialResponse:  # noqa: E501
+        """Get user enterprise trial
 
-        Admin-only API to get marketing metrics about a user.
+        Admin-only API to get a specific enterprise trial.
 
         :param user_id: User ID (required)
         :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: AdminGetUserMetricsResponse
+        :rtype: AdminGetUserTrialResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_get_user_metrics_with_http_info(user_id, **kwargs)  # noqa: E501
+        return self._admin_get_user_trial_with_http_info(user_id, enterprise_trial_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_get_user_metrics_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
-        """Get user metrics 
+    def _admin_get_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
+        """Get user enterprise trial 
 
-        Admin-only API to get marketing metrics about a user.
+        Admin-only API to get a specific enterprise trial.
 
         :param user_id: User ID (required)
         :type user_id: int
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -6641,21 +6658,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(AdminGetUserMetricsResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(AdminGetUserTrialResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'user_id'
+            'user_id',
+            'enterprise_trial_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -6666,25 +6684,27 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_get_user_metrics" % _key
+                    " to method admin_get_user_trial" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['user_id']:
             _path_params['userId'] = _params['user_id']
+        if _params['enterprise_trial_id']:
+            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -6699,19 +6719,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "AdminGetUserMetricsResponse",
+            '200': "AdminGetUserTrialResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/users/{userId}/metrics', 'GET',
+            '/api/admin/users/{userId}/trials/{enterpriseTrialId}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -6720,23 +6740,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_get_users(self, active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[UserTierEnum], Field(description="Whether to search for free, community plus, professional, or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs) -> AdminGetUsersResponse:  # noqa: E501
+    def admin_get_users(self, active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[StrictStr], Field(description="Whether to search for free, pro or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs) -> AdminGetUsersResponse:  # noqa: E501
         """Get all users
 
         Admin-only API to get the list of all registered users.
 
         :param active: Whether to search for entities (users, orgs) active in the last X days
         :type active: int
-        :param tier: Whether to search for free, community plus, professional, or enterprise entities (users, projects)
-        :type tier: UserTierEnum
+        :param tier: Whether to search for free, pro or enterprise entities (users, projects)
+        :type tier: str
         :param fields: Comma separated list of fields to fetch in a query
         :type fields: str
         :param sort: Fields and order to sort query by
         :type sort: str
         :param limit: Maximum number of results
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
@@ -6758,23 +6778,23 @@
                  returns the request thread.
         :rtype: AdminGetUsersResponse
         """
         kwargs['_return_http_data_only'] = True
         return self._admin_get_users_with_http_info(active, tier, fields, sort, limit, offset, search, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_get_users_with_http_info(self, active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[UserTierEnum], Field(description="Whether to search for free, community plus, professional, or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs):  # noqa: E501
+    def _admin_get_users_with_http_info(self, active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[StrictStr], Field(description="Whether to search for free, pro or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs):  # noqa: E501
         """Get all users 
 
         Admin-only API to get the list of all registered users.
 
         :param active: Whether to search for entities (users, orgs) active in the last X days
         :type active: int
-        :param tier: Whether to search for free, community plus, professional, or enterprise entities (users, projects)
-        :type tier: UserTierEnum
+        :param tier: Whether to search for free, pro or enterprise entities (users, projects)
+        :type tier: str
         :param fields: Comma separated list of fields to fetch in a query
         :type fields: str
         :param sort: Fields and order to sort query by
         :type sort: str
         :param limit: Maximum number of results
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
@@ -8036,23 +8056,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_update_trial(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], admin_update_trial_request : AdminUpdateTrialRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Update enterprise trial
+    def admin_update_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_request : AdminUpdateUserRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update user
 
-        Admin-only API to update an enterprise trial.
+        Admin-only API to update user properties.
 
-        :param enterprise_trial_id: Enterprise trial ID (required)
-        :type enterprise_trial_id: int
-        :param admin_update_trial_request: (required)
-        :type admin_update_trial_request: AdminUpdateTrialRequest
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param admin_update_user_request: (required)
+        :type admin_update_user_request: AdminUpdateUserRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -8061,26 +8081,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_update_trial_with_http_info(enterprise_trial_id, admin_update_trial_request, **kwargs)  # noqa: E501
+        return self._admin_update_user_with_http_info(user_id, admin_update_user_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_update_trial_with_http_info(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], admin_update_trial_request : AdminUpdateTrialRequest, **kwargs):  # noqa: E501
-        """Update enterprise trial 
+    def _admin_update_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_request : AdminUpdateUserRequest, **kwargs):  # noqa: E501
+        """Update user 
 
-        Admin-only API to update an enterprise trial.
+        Admin-only API to update user properties.
 
-        :param enterprise_trial_id: Enterprise trial ID (required)
-        :type enterprise_trial_id: int
-        :param admin_update_trial_request: (required)
-        :type admin_update_trial_request: AdminUpdateTrialRequest
+        :param user_id: User ID (required)
+        :type user_id: int
+        :param admin_update_user_request: (required)
+        :type admin_update_user_request: AdminUpdateUserRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -8100,16 +8120,16 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'enterprise_trial_id',
-            'admin_update_trial_request'
+            'user_id',
+            'admin_update_user_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -8120,40 +8140,40 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_update_trial" % _key
+                    " to method admin_update_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['enterprise_trial_id']:
-            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['admin_update_trial_request']:
-            _body_params = _params['admin_update_trial_request']
+        if _params['admin_update_user_request']:
+            _body_params = _params['admin_update_user_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -8166,15 +8186,15 @@
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/trials/{enterpriseTrialId}', 'PUT',
+            '/api/admin/users/{userId}', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -8183,23 +8203,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_update_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_request : AdminUpdateUserRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Update user
+    def admin_update_user_permissions(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_permissions_request : AdminUpdateUserPermissionsRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update user permissions
 
-        Admin-only API to update user properties.
+        Admin-only API to update the list of permissions for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param admin_update_user_request: (required)
-        :type admin_update_user_request: AdminUpdateUserRequest
+        :param admin_update_user_permissions_request: (required)
+        :type admin_update_user_permissions_request: AdminUpdateUserPermissionsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -8208,26 +8228,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_update_user_with_http_info(user_id, admin_update_user_request, **kwargs)  # noqa: E501
+        return self._admin_update_user_permissions_with_http_info(user_id, admin_update_user_permissions_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_update_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_request : AdminUpdateUserRequest, **kwargs):  # noqa: E501
-        """Update user 
+    def _admin_update_user_permissions_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_permissions_request : AdminUpdateUserPermissionsRequest, **kwargs):  # noqa: E501
+        """Update user permissions 
 
-        Admin-only API to update user properties.
+        Admin-only API to update the list of permissions for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param admin_update_user_request: (required)
-        :type admin_update_user_request: AdminUpdateUserRequest
+        :param admin_update_user_permissions_request: (required)
+        :type admin_update_user_permissions_request: AdminUpdateUserPermissionsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -8248,15 +8268,15 @@
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'user_id',
-            'admin_update_user_request'
+            'admin_update_user_permissions_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -8267,15 +8287,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_update_user" % _key
+                    " to method admin_update_user_permissions" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -8291,16 +8311,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['admin_update_user_request']:
-            _body_params = _params['admin_update_user_request']
+        if _params['admin_update_user_permissions_request']:
+            _body_params = _params['admin_update_user_permissions_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -8313,15 +8333,15 @@
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/users/{userId}', 'POST',
+            '/api/admin/users/{userId}/permissions', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -8330,23 +8350,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_update_user_permissions(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_permissions_request : AdminUpdateUserPermissionsRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Update user permissions
+    def admin_update_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], admin_update_user_trial_request : AdminUpdateUserTrialRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update user enterprise trial
 
-        Admin-only API to update the list of permissions for a user.
+        Admin-only API to update an enterprise trial for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param admin_update_user_permissions_request: (required)
-        :type admin_update_user_permissions_request: AdminUpdateUserPermissionsRequest
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param admin_update_user_trial_request: (required)
+        :type admin_update_user_trial_request: AdminUpdateUserTrialRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -8355,26 +8377,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_update_user_permissions_with_http_info(user_id, admin_update_user_permissions_request, **kwargs)  # noqa: E501
+        return self._admin_update_user_trial_with_http_info(user_id, enterprise_trial_id, admin_update_user_trial_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_update_user_permissions_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], admin_update_user_permissions_request : AdminUpdateUserPermissionsRequest, **kwargs):  # noqa: E501
-        """Update user permissions 
+    def _admin_update_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], admin_update_user_trial_request : AdminUpdateUserTrialRequest, **kwargs):  # noqa: E501
+        """Update user enterprise trial 
 
-        Admin-only API to update the list of permissions for a user.
+        Admin-only API to update an enterprise trial for a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param admin_update_user_permissions_request: (required)
-        :type admin_update_user_permissions_request: AdminUpdateUserPermissionsRequest
+        :param enterprise_trial_id: Enterprise trial ID (required)
+        :type enterprise_trial_id: int
+        :param admin_update_user_trial_request: (required)
+        :type admin_update_user_trial_request: AdminUpdateUserTrialRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -8395,15 +8419,16 @@
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'user_id',
-            'admin_update_user_permissions_request'
+            'enterprise_trial_id',
+            'admin_update_user_trial_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -8414,40 +8439,42 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_update_user_permissions" % _key
+                    " to method admin_update_user_trial" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['user_id']:
             _path_params['userId'] = _params['user_id']
+        if _params['enterprise_trial_id']:
+            _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['admin_update_user_permissions_request']:
-            _body_params = _params['admin_update_user_permissions_request']
+        if _params['admin_update_user_trial_request']:
+            _body_params = _params['admin_update_user_trial_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -8460,15 +8487,15 @@
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/users/{userId}/permissions', 'POST',
+            '/api/admin/users/{userId}/trials/{enterpriseTrialId}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -8477,19 +8504,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_upgrade_trial(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Upgrade enterprise trial to a full enterprise account
+    def admin_upgrade_user_trial(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Upgrade user enterprise trial to a full enterprise account
 
-        Admin-only API to upgrade a specific enterprise trial to a full enterprise account.
+        Admin-only API to upgrade a specific enterprise trial for a user to a full enterprise account.
 
+        :param user_id: User ID (required)
+        :type user_id: int
         :param enterprise_trial_id: Enterprise trial ID (required)
         :type enterprise_trial_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -8500,22 +8529,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_upgrade_trial_with_http_info(enterprise_trial_id, **kwargs)  # noqa: E501
+        return self._admin_upgrade_user_trial_with_http_info(user_id, enterprise_trial_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_upgrade_trial_with_http_info(self, enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
-        """Upgrade enterprise trial to a full enterprise account 
+    def _admin_upgrade_user_trial_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], enterprise_trial_id : Annotated[StrictInt, Field(..., description="Enterprise trial ID")], **kwargs):  # noqa: E501
+        """Upgrade user enterprise trial to a full enterprise account 
 
-        Admin-only API to upgrade a specific enterprise trial to a full enterprise account.
+        Admin-only API to upgrade a specific enterprise trial for a user to a full enterprise account.
 
+        :param user_id: User ID (required)
+        :type user_id: int
         :param enterprise_trial_id: Enterprise trial ID (required)
         :type enterprise_trial_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -8537,14 +8568,15 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'user_id',
             'enterprise_trial_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -8556,23 +8588,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method admin_upgrade_trial" % _key
+                    " to method admin_upgrade_user_trial" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['user_id']:
+            _path_params['userId'] = _params['user_id']
         if _params['enterprise_trial_id']:
             _path_params['enterpriseTrialId'] = _params['enterprise_trial_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
@@ -8593,15 +8627,15 @@
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/admin/trials/{enterpriseTrialId}/upgrade', 'POST',
+            '/api/admin/users/{userId}/trials/{enterpriseTrialId}/upgrade', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/classify_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/dsp_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/email_verification_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/email_verification_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/feature_flags_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/feature_flags_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/learn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_data_campaigns_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_data_campaigns_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/organizations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
 from edgeimpulse_api.models.update_whitelabel_learning_blocks_request import UpdateWhitelabelLearningBlocksRequest
 from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.upload_readme_image_response import UploadReadmeImageResponse
-from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 from edgeimpulse_api.models.whitelabel_admin_create_organization_request import WhitelabelAdminCreateOrganizationRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -7806,25 +7805,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def whitelabel_admin_get_users(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[UserTierEnum], Field(description="Whether to search for free, community plus, professional, or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs) -> AdminGetUsersResponse:  # noqa: E501
+    def whitelabel_admin_get_users(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[StrictStr], Field(description="Whether to search for free, pro or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs) -> AdminGetUsersResponse:  # noqa: E501
         """White Label Admin - Get all white label users
 
         White label admin only API to get the list of all registered users.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param active: Whether to search for entities (users, orgs) active in the last X days
         :type active: int
-        :param tier: Whether to search for free, community plus, professional, or enterprise entities (users, projects)
-        :type tier: UserTierEnum
+        :param tier: Whether to search for free, pro or enterprise entities (users, projects)
+        :type tier: str
         :param fields: Comma separated list of fields to fetch in a query
         :type fields: str
         :param sort: Fields and order to sort query by
         :type sort: str
         :param limit: Maximum number of results
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
@@ -7846,25 +7845,25 @@
                  returns the request thread.
         :rtype: AdminGetUsersResponse
         """
         kwargs['_return_http_data_only'] = True
         return self._whitelabel_admin_get_users_with_http_info(organization_id, active, tier, fields, sort, limit, offset, search, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _whitelabel_admin_get_users_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[UserTierEnum], Field(description="Whether to search for free, community plus, professional, or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs):  # noqa: E501
+    def _whitelabel_admin_get_users_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], active : Annotated[Optional[StrictInt], Field(description="Whether to search for entities (users, orgs) active in the last X days")] = None, tier : Annotated[Optional[StrictStr], Field(description="Whether to search for free, pro or enterprise entities (users, projects)")] = None, fields : Annotated[Optional[StrictStr], Field(description="Comma separated list of fields to fetch in a query")] = None, sort : Annotated[Optional[StrictStr], Field(description="Fields and order to sort query by")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, search : Annotated[Optional[StrictStr], Field(description="Search query")] = None, **kwargs):  # noqa: E501
         """White Label Admin - Get all white label users 
 
         White label admin only API to get the list of all registered users.
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param active: Whether to search for entities (users, orgs) active in the last X days
         :type active: int
-        :param tier: Whether to search for free, community plus, professional, or enterprise entities (users, projects)
-        :type tier: UserTierEnum
+        :param tier: Whether to search for free, pro or enterprise entities (users, projects)
+        :type tier: str
         :param fields: Comma separated list of fields to fetch in a query
         :type fields: str
         :param sort: Fields and order to sort query by
         :type sort: str
         :param limit: Maximum number of results
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from edgeimpulse_api.models.activate_user_or_verify_email_request import ActivateUserOrVerifyEmailRequest
 from edgeimpulse_api.models.change_password_request import ChangePasswordRequest
 from edgeimpulse_api.models.convert_user_request import ConvertUserRequest
 from edgeimpulse_api.models.create_developer_profile_response import CreateDeveloperProfileResponse
 from edgeimpulse_api.models.create_enterprise_trial_response import CreateEnterpriseTrialResponse
 from edgeimpulse_api.models.create_enterprise_trial_user_request import CreateEnterpriseTrialUserRequest
 from edgeimpulse_api.models.create_evaluation_user_response import CreateEvaluationUserResponse
-from edgeimpulse_api.models.create_pro_tier_user_request import CreateProTierUserRequest
 from edgeimpulse_api.models.create_user_request import CreateUserRequest
 from edgeimpulse_api.models.create_user_response import CreateUserResponse
 from edgeimpulse_api.models.delete_user_request import DeleteUserRequest
 from edgeimpulse_api.models.enterprise_upgrade_or_trial_extension_request import EnterpriseUpgradeOrTrialExtensionRequest
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.get_jwt_response import GetJWTResponse
 from edgeimpulse_api.models.get_user_need_to_set_password_response import GetUserNeedToSetPasswordResponse
@@ -1430,154 +1429,14 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def create_pro_tier_user(self, create_pro_tier_user_request : CreateProTierUserRequest, **kwargs) -> CreateUserResponse:  # noqa: E501
-        """Create Professional Tier user
-
-        Create a new user for the Professional Plan and a new project. Note that the Professional plan will not be enabled until the payment is successful.
-
-        :param create_pro_tier_user_request: (required)
-        :type create_pro_tier_user_request: CreateProTierUserRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: CreateUserResponse
-        """
-        kwargs['_return_http_data_only'] = True
-        return self._create_pro_tier_user_with_http_info(create_pro_tier_user_request, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def _create_pro_tier_user_with_http_info(self, create_pro_tier_user_request : CreateProTierUserRequest, **kwargs):  # noqa: E501
-        """Create Professional Tier user 
-
-        Create a new user for the Professional Plan and a new project. Note that the Professional plan will not be enabled until the payment is successful.
-
-        :param create_pro_tier_user_request: (required)
-        :type create_pro_tier_user_request: CreateProTierUserRequest
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(CreateUserResponse, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'create_pro_tier_user_request'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method create_pro_tier_user" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-
-        # process the query parameters
-        _query_params = []
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-
-        # process the body parameter
-        _body_params = None
-        if _params['create_pro_tier_user_request']:
-            _body_params = _params['create_pro_tier_user_request']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
-        # authentication setting
-        _auth_settings = []  # noqa: E501
-
-        _response_types_map = {
-            '200': "CreateUserResponse",
-        }
-
-        return self.api_client.call_api(
-            '/api-create-pro-user', 'POST',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api/whitelabels_api.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api/whitelabels_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 from edgeimpulse_api.models.add_organization_transfer_learning_block_request import AddOrganizationTransferLearningBlockRequest
 from edgeimpulse_api.models.add_organization_transfer_learning_block_response import AddOrganizationTransferLearningBlockResponse
 from edgeimpulse_api.models.add_organization_transformation_block_request import AddOrganizationTransformationBlockRequest
 from edgeimpulse_api.models.add_organization_transformation_block_response import AddOrganizationTransformationBlockResponse
 from edgeimpulse_api.models.add_organization_transformation_block_response_all_of import AddOrganizationTransformationBlockResponseAllOf
 from edgeimpulse_api.models.add_project_api_key_request import AddProjectApiKeyRequest
 from edgeimpulse_api.models.add_project_api_key_request_all_of import AddProjectApiKeyRequestAllOf
-from edgeimpulse_api.models.additional_metric import AdditionalMetric
 from edgeimpulse_api.models.admin_add_disallowed_email_domain_request import AdminAddDisallowedEmailDomainRequest
 from edgeimpulse_api.models.admin_add_or_update_sso_domain_id_ps_request import AdminAddOrUpdateSSODomainIdPsRequest
 from edgeimpulse_api.models.admin_add_organization_api_key_request import AdminAddOrganizationApiKeyRequest
 from edgeimpulse_api.models.admin_add_organization_user_request import AdminAddOrganizationUserRequest
 from edgeimpulse_api.models.admin_add_organization_user_request_all_of import AdminAddOrganizationUserRequestAllOf
 from edgeimpulse_api.models.admin_add_project_api_key_request import AdminAddProjectApiKeyRequest
 from edgeimpulse_api.models.admin_add_project_api_key_request_all_of import AdminAddProjectApiKeyRequestAllOf
@@ -78,36 +77,34 @@
 from edgeimpulse_api.models.admin_get_organizations_response_all_of import AdminGetOrganizationsResponseAllOf
 from edgeimpulse_api.models.admin_get_organizations_response_all_of_organizations import AdminGetOrganizationsResponseAllOfOrganizations
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response import AdminGetSSODomainIdPsResponse
 from edgeimpulse_api.models.admin_get_sso_domain_id_ps_response_all_of import AdminGetSSODomainIdPsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response import AdminGetSSOSettingsResponse
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of import AdminGetSSOSettingsResponseAllOf
 from edgeimpulse_api.models.admin_get_sso_settings_response_all_of_sso_whitelist import AdminGetSSOSettingsResponseAllOfSsoWhitelist
-from edgeimpulse_api.models.admin_get_trial_response import AdminGetTrialResponse
-from edgeimpulse_api.models.admin_get_trial_response_all_of import AdminGetTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_user_ids_response import AdminGetUserIdsResponse
 from edgeimpulse_api.models.admin_get_user_ids_response_all_of import AdminGetUserIdsResponseAllOf
 from edgeimpulse_api.models.admin_get_user_metrics_response import AdminGetUserMetricsResponse
 from edgeimpulse_api.models.admin_get_user_response import AdminGetUserResponse
 from edgeimpulse_api.models.admin_get_user_response_all_of import AdminGetUserResponseAllOf
+from edgeimpulse_api.models.admin_get_user_trial_response import AdminGetUserTrialResponse
+from edgeimpulse_api.models.admin_get_user_trial_response_all_of import AdminGetUserTrialResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response import AdminGetUsersResponse
 from edgeimpulse_api.models.admin_get_users_response_all_of import AdminGetUsersResponseAllOf
 from edgeimpulse_api.models.admin_get_users_response_all_of_users import AdminGetUsersResponseAllOfUsers
 from edgeimpulse_api.models.admin_list_projects import AdminListProjects
 from edgeimpulse_api.models.admin_list_projects_response import AdminListProjectsResponse
 from edgeimpulse_api.models.admin_organization_info_response import AdminOrganizationInfoResponse
 from edgeimpulse_api.models.admin_organization_info_response_all_of import AdminOrganizationInfoResponseAllOf
-from edgeimpulse_api.models.admin_start_enterprise_trial_request import AdminStartEnterpriseTrialRequest
-from edgeimpulse_api.models.admin_start_enterprise_trial_request_all_of import AdminStartEnterpriseTrialRequestAllOf
 from edgeimpulse_api.models.admin_toggle_data_migration_request import AdminToggleDataMigrationRequest
 from edgeimpulse_api.models.admin_update_organization_data_export_request import AdminUpdateOrganizationDataExportRequest
 from edgeimpulse_api.models.admin_update_organization_request import AdminUpdateOrganizationRequest
-from edgeimpulse_api.models.admin_update_trial_request import AdminUpdateTrialRequest
 from edgeimpulse_api.models.admin_update_user_permissions_request import AdminUpdateUserPermissionsRequest
 from edgeimpulse_api.models.admin_update_user_request import AdminUpdateUserRequest
+from edgeimpulse_api.models.admin_update_user_trial_request import AdminUpdateUserTrialRequest
 from edgeimpulse_api.models.akida_edge_learning_config import AkidaEdgeLearningConfig
 from edgeimpulse_api.models.anomaly_capacity import AnomalyCapacity
 from edgeimpulse_api.models.anomaly_gmm_metadata import AnomalyGmmMetadata
 from edgeimpulse_api.models.anomaly_gmm_metadata_all_of import AnomalyGmmMetadataAllOf
 from edgeimpulse_api.models.anomaly_model_metadata import AnomalyModelMetadata
 from edgeimpulse_api.models.anomaly_model_metadata_all_of import AnomalyModelMetadataAllOf
 from edgeimpulse_api.models.anomaly_model_metadata_all_of_clusters import AnomalyModelMetadataAllOfClusters
@@ -132,15 +129,14 @@
 from edgeimpulse_api.models.build_organization_on_device_model_request import BuildOrganizationOnDeviceModelRequest
 from edgeimpulse_api.models.calculate_data_quality_metrics_request import CalculateDataQualityMetricsRequest
 from edgeimpulse_api.models.change_password_request import ChangePasswordRequest
 from edgeimpulse_api.models.classify_job_response import ClassifyJobResponse
 from edgeimpulse_api.models.classify_job_response_all_of import ClassifyJobResponseAllOf
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy_total_summary import ClassifyJobResponseAllOfAccuracyTotalSummary
-from edgeimpulse_api.models.classify_job_response_all_of_additional_metrics_by_learn_block import ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock
 from edgeimpulse_api.models.classify_job_response_page import ClassifyJobResponsePage
 from edgeimpulse_api.models.classify_job_response_page_all_of import ClassifyJobResponsePageAllOf
 from edgeimpulse_api.models.classify_sample_for_variants200_response import ClassifySampleForVariants200Response
 from edgeimpulse_api.models.classify_sample_response import ClassifySampleResponse
 from edgeimpulse_api.models.classify_sample_response_all_of import ClassifySampleResponseAllOf
 from edgeimpulse_api.models.classify_sample_response_classification import ClassifySampleResponseClassification
 from edgeimpulse_api.models.classify_sample_response_classification_details import ClassifySampleResponseClassificationDetails
@@ -170,16 +166,14 @@
 from edgeimpulse_api.models.create_organization_portal_response import CreateOrganizationPortalResponse
 from edgeimpulse_api.models.create_organization_portal_response_all_of import CreateOrganizationPortalResponseAllOf
 from edgeimpulse_api.models.create_organization_request import CreateOrganizationRequest
 from edgeimpulse_api.models.create_organization_response import CreateOrganizationResponse
 from edgeimpulse_api.models.create_organization_response_all_of import CreateOrganizationResponseAllOf
 from edgeimpulse_api.models.create_organization_usage_report_body import CreateOrganizationUsageReportBody
 from edgeimpulse_api.models.create_pipeline_response import CreatePipelineResponse
-from edgeimpulse_api.models.create_pro_tier_user_request import CreateProTierUserRequest
-from edgeimpulse_api.models.create_pro_tier_user_request_all_of import CreateProTierUserRequestAllOf
 from edgeimpulse_api.models.create_project_request import CreateProjectRequest
 from edgeimpulse_api.models.create_project_response import CreateProjectResponse
 from edgeimpulse_api.models.create_project_response_all_of import CreateProjectResponseAllOf
 from edgeimpulse_api.models.create_signed_upload_link_request import CreateSignedUploadLinkRequest
 from edgeimpulse_api.models.create_signed_upload_link_response import CreateSignedUploadLinkResponse
 from edgeimpulse_api.models.create_signed_upload_link_response_all_of import CreateSignedUploadLinkResponseAllOf
 from edgeimpulse_api.models.create_third_party_auth_request import CreateThirdPartyAuthRequest
@@ -486,15 +480,14 @@
 from edgeimpulse_api.models.keras_model_layer_input import KerasModelLayerInput
 from edgeimpulse_api.models.keras_model_layer_output import KerasModelLayerOutput
 from edgeimpulse_api.models.keras_model_metadata import KerasModelMetadata
 from edgeimpulse_api.models.keras_model_metadata_all_of import KerasModelMetadataAllOf
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
 from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner import KerasModelMetadataMetricsOnDevicePerformanceInner
 from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner_tflite import KerasModelMetadataMetricsOnDevicePerformanceInnerTflite
-from edgeimpulse_api.models.keras_model_mode import KerasModelMode
 from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
 from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.keras_response import KerasResponse
 from edgeimpulse_api.models.keras_response_all_of import KerasResponseAllOf
 from edgeimpulse_api.models.keras_visual_layer import KerasVisualLayer
 from edgeimpulse_api.models.keras_visual_layer_type import KerasVisualLayerType
 from edgeimpulse_api.models.last_modification_date_response import LastModificationDateResponse
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/activate_user_or_verify_email_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/activate_user_or_verify_email_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_api_key_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_project_api_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/additional_metric.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_version_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,58 +14,52 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, StrictStr
 
-class AdditionalMetric(BaseModel):
-    name: StrictStr = ...
-    value: StrictStr = ...
-    tooltip_text: Optional[StrictStr] = Field(None, alias="tooltipText")
-    link: Optional[StrictStr] = None
-    __properties = ["name", "value", "tooltipText", "link"]
+class UpdateVersionRequest(BaseModel):
+    description: Optional[StrictStr] = None
+    __properties = ["description"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdditionalMetric:
-        """Create an instance of AdditionalMetric from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateVersionRequest:
+        """Create an instance of UpdateVersionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdditionalMetric:
-        """Create an instance of AdditionalMetric from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateVersionRequest:
+        """Create an instance of UpdateVersionRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdditionalMetric.construct(**obj)
+            return UpdateVersionRequest.construct(**obj)
 
-        _obj = AdditionalMetric.construct(**{
-            "name": obj.get("name"),
-            "value": obj.get("value"),
-            "tooltip_text": obj.get("tooltipText"),
-            "link": obj.get("link")
+        _obj = UpdateVersionRequest.construct(**{
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_organization_api_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_organization_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_organization_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_project_api_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_add_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_add_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_create_organization_data_export_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_create_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_create_project_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_enable_feature_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_enable_feature_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migration_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migration_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migrations_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migrations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_report_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_trial_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_trial_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 
-class AdminGetTrialResponse(BaseModel):
+class AdminGetUserTrialResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
     trial: EnterpriseTrial = ...
     __properties = ["success", "error", "trial"]
 
     class Config:
         allow_population_by_field_name = True
@@ -36,38 +36,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminGetTrialResponse:
-        """Create an instance of AdminGetTrialResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> AdminGetUserTrialResponse:
+        """Create an instance of AdminGetUserTrialResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of trial
         if self.trial:
             _dict['trial'] = self.trial.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminGetTrialResponse:
-        """Create an instance of AdminGetTrialResponse from a dict"""
+    def from_dict(cls, obj: dict) -> AdminGetUserTrialResponse:
+        """Create an instance of AdminGetUserTrialResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminGetTrialResponse.construct(**obj)
+            return AdminGetUserTrialResponse.construct(**obj)
 
-        _obj = AdminGetTrialResponse.construct(**{
+        _obj = AdminGetUserTrialResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
             "trial": EnterpriseTrial.from_dict(obj.get("trial")) if obj.get("trial") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_trial_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import json
 
 
 
 from pydantic import BaseModel
 from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 
-class AdminGetTrialResponseAllOf(BaseModel):
+class AdminGetUserTrialResponseAllOf(BaseModel):
     trial: EnterpriseTrial = ...
     __properties = ["trial"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
@@ -34,36 +34,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminGetTrialResponseAllOf:
-        """Create an instance of AdminGetTrialResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> AdminGetUserTrialResponseAllOf:
+        """Create an instance of AdminGetUserTrialResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of trial
         if self.trial:
             _dict['trial'] = self.trial.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminGetTrialResponseAllOf:
-        """Create an instance of AdminGetTrialResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> AdminGetUserTrialResponseAllOf:
+        """Create an instance of AdminGetUserTrialResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminGetTrialResponseAllOf.construct(**obj)
+            return AdminGetUserTrialResponseAllOf.construct(**obj)
 
-        _obj = AdminGetTrialResponseAllOf.construct(**{
+        _obj = AdminGetUserTrialResponseAllOf.construct(**{
             "trial": EnterpriseTrial.from_dict(obj.get("trial")) if obj.get("trial") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_start_enterprise_trial_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_enterprise_trial_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,31 +14,30 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+from pydantic import BaseModel, Field, StrictStr, validator
 
-class AdminStartEnterpriseTrialRequest(BaseModel):
+class StartEnterpriseTrialRequest(BaseModel):
     email: Optional[StrictStr] = Field(None, description="Email of the user requesting the trial. If this email is different to the one stored for the user requesting the trial, it will be used to replace the existing one.")
     organization_name: Optional[StrictStr] = Field(None, alias="organizationName", description="Name of the trial organization. All enterprise features are tied to an organization. This organization will be deleted after the trial ends. If no organization name is provided, the user's name will be used.")
     expiration_date: Optional[datetime] = Field(None, alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization. This field is ignored if the trial is requested by a non-admin user, defaulting to 14 days trial.")
     notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text. This field is ignored if the trial is requested by a non-admin user.")
     use_case: Optional[StrictStr] = Field(None, alias="useCase", description="Use case of the trial.")
     user_has_ml_models_in_production: Optional[StrictStr] = Field(None, alias="userHasMLModelsInProduction", description="Whether the user has ML models in production.")
     company_name: Optional[StrictStr] = Field(None, alias="companyName", description="Name of the company requesting the trial.")
     company_size: Optional[StrictStr] = Field(None, alias="companySize", description="Size of the company requesting the trial. This is a range of number of employees.")
     country: Optional[StrictStr] = Field(None, description="Country of the company requesting the trial.")
     state_or_province: Optional[StrictStr] = Field(None, alias="stateOrProvince", description="State or province of the company requesting the trial.")
     redirect_url_origin: Optional[StrictStr] = Field(None, alias="redirectUrlOrigin", description="Origin of the redirect URL returned as result of creating the trial user.")
     redirect_url_query_params: Optional[StrictStr] = Field(None, alias="redirectUrlQueryParams", description="Query parameters to be appended to the redirect URL returned as result of creating the trial user.")
-    user_id: StrictInt = Field(..., alias="userId", description="ID of the user requesting the trial.")
-    __properties = ["email", "organizationName", "expirationDate", "notes", "useCase", "userHasMLModelsInProduction", "companyName", "companySize", "country", "stateOrProvince", "redirectUrlOrigin", "redirectUrlQueryParams", "userId"]
+    __properties = ["email", "organizationName", "expirationDate", "notes", "useCase", "userHasMLModelsInProduction", "companyName", "companySize", "country", "stateOrProvince", "redirectUrlOrigin", "redirectUrlQueryParams"]
 
     @validator('user_has_ml_models_in_production')
     def user_has_ml_models_in_production_validate_enum(cls, v):
         if v is None:
             return v
 
         if v not in ('yes', 'no', 'no, but we will soon'):
@@ -54,45 +53,44 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminStartEnterpriseTrialRequest:
-        """Create an instance of AdminStartEnterpriseTrialRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> StartEnterpriseTrialRequest:
+        """Create an instance of StartEnterpriseTrialRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminStartEnterpriseTrialRequest:
-        """Create an instance of AdminStartEnterpriseTrialRequest from a dict"""
+    def from_dict(cls, obj: dict) -> StartEnterpriseTrialRequest:
+        """Create an instance of StartEnterpriseTrialRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminStartEnterpriseTrialRequest.construct(**obj)
+            return StartEnterpriseTrialRequest.construct(**obj)
 
-        _obj = AdminStartEnterpriseTrialRequest.construct(**{
+        _obj = StartEnterpriseTrialRequest.construct(**{
             "email": obj.get("email"),
             "organization_name": obj.get("organizationName"),
             "expiration_date": obj.get("expirationDate"),
             "notes": obj.get("notes"),
             "use_case": obj.get("useCase"),
             "user_has_ml_models_in_production": obj.get("userHasMLModelsInProduction"),
             "company_name": obj.get("companyName"),
             "company_size": obj.get("companySize"),
             "country": obj.get("country"),
             "state_or_province": obj.get("stateOrProvince"),
             "redirect_url_origin": obj.get("redirectUrlOrigin"),
-            "redirect_url_query_params": obj.get("redirectUrlQueryParams"),
-            "user_id": obj.get("userId")
+            "redirect_url_query_params": obj.get("redirectUrlQueryParams")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_start_enterprise_trial_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/stop_device_debug_stream_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,50 +16,50 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictInt
 
-class AdminStartEnterpriseTrialRequestAllOf(BaseModel):
-    user_id: StrictInt = Field(..., alias="userId", description="ID of the user requesting the trial.")
-    __properties = ["userId"]
+class StopDeviceDebugStreamRequest(BaseModel):
+    stream_id: StrictInt = Field(..., alias="streamId")
+    __properties = ["streamId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminStartEnterpriseTrialRequestAllOf:
-        """Create an instance of AdminStartEnterpriseTrialRequestAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> StopDeviceDebugStreamRequest:
+        """Create an instance of StopDeviceDebugStreamRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminStartEnterpriseTrialRequestAllOf:
-        """Create an instance of AdminStartEnterpriseTrialRequestAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> StopDeviceDebugStreamRequest:
+        """Create an instance of StopDeviceDebugStreamRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminStartEnterpriseTrialRequestAllOf.construct(**obj)
+            return StopDeviceDebugStreamRequest.construct(**obj)
 
-        _obj = AdminStartEnterpriseTrialRequestAllOf.construct(**{
-            "user_id": obj.get("userId")
+        _obj = StopDeviceDebugStreamRequest.construct(**{
+            "stream_id": obj.get("streamId")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_toggle_data_migration_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_toggle_data_migration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_organization_data_export_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_trial_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_user_trial_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class AdminUpdateTrialRequest(BaseModel):
+class AdminUpdateUserTrialRequest(BaseModel):
     expiration_date: Optional[datetime] = Field(None, alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization. This field is ignored if the trial is requested by a non-admin user, defaulting to 14 days trial.")
     notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text. This field is ignored if the trial is requested by a non-admin user.")
     __properties = ["expirationDate", "notes"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
@@ -34,34 +34,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AdminUpdateTrialRequest:
-        """Create an instance of AdminUpdateTrialRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> AdminUpdateUserTrialRequest:
+        """Create an instance of AdminUpdateUserTrialRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AdminUpdateTrialRequest:
-        """Create an instance of AdminUpdateTrialRequest from a dict"""
+    def from_dict(cls, obj: dict) -> AdminUpdateUserTrialRequest:
+        """Create an instance of AdminUpdateUserTrialRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AdminUpdateTrialRequest.construct(**obj)
+            return AdminUpdateUserTrialRequest.construct(**obj)
 
-        _obj = AdminUpdateTrialRequest.construct(**{
+        _obj = AdminUpdateUserTrialRequest.construct(**{
             "expiration_date": obj.get("expirationDate"),
             "notes": obj.get("notes")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_capacity.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_capacity.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_gmm_metadata.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_gmm_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_model_metadata_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_result.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/application_budget.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/application_budget.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/auto_labeler_segment.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/auto_labeler_segment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/block_type.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/calculate_data_quality_metrics_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/calculate_data_quality_metrics_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,28 +16,26 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
-from edgeimpulse_api.models.classify_job_response_all_of_additional_metrics_by_learn_block import ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock
 from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.model_prediction import ModelPrediction
 from edgeimpulse_api.models.model_result import ModelResult
 
 class ClassifyJobResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
     result: List[ModelResult] = ...
     predictions: List[ModelPrediction] = ...
     accuracy: ClassifyJobResponseAllOfAccuracy = ...
-    additional_metrics_by_learn_block: List[ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock] = Field(..., alias="additionalMetricsByLearnBlock")
     available_variants: List[KerasModelVariantEnum] = Field(..., alias="availableVariants", description="List of all model variants for which classification results exist")
-    __properties = ["success", "error", "result", "predictions", "accuracy", "additionalMetricsByLearnBlock", "availableVariants"]
+    __properties = ["success", "error", "result", "predictions", "accuracy", "availableVariants"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -71,21 +69,14 @@
             for _item in self.predictions:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['predictions'] = _items
         # override the default output from pydantic by calling `to_dict()` of accuracy
         if self.accuracy:
             _dict['accuracy'] = self.accuracy.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in additional_metrics_by_learn_block (list)
-        _items = []
-        if self.additional_metrics_by_learn_block:
-            for _item in self.additional_metrics_by_learn_block:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['additionalMetricsByLearnBlock'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ClassifyJobResponse:
         """Create an instance of ClassifyJobResponse from a dict"""
         if obj is None:
             return None
@@ -95,12 +86,11 @@
 
         _obj = ClassifyJobResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
             "result": [ModelResult.from_dict(_item) for _item in obj.get("result")] if obj.get("result") is not None else None,
             "predictions": [ModelPrediction.from_dict(_item) for _item in obj.get("predictions")] if obj.get("predictions") is not None else None,
             "accuracy": ClassifyJobResponseAllOfAccuracy.from_dict(obj.get("accuracy")) if obj.get("accuracy") is not None else None,
-            "additional_metrics_by_learn_block": [ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock.from_dict(_item) for _item in obj.get("additionalMetricsByLearnBlock")] if obj.get("additionalMetricsByLearnBlock") is not None else None,
             "available_variants": obj.get("availableVariants")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,26 +16,24 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
-from edgeimpulse_api.models.classify_job_response_all_of_additional_metrics_by_learn_block import ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock
 from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.model_prediction import ModelPrediction
 from edgeimpulse_api.models.model_result import ModelResult
 
 class ClassifyJobResponseAllOf(BaseModel):
     result: List[ModelResult] = ...
     predictions: List[ModelPrediction] = ...
     accuracy: ClassifyJobResponseAllOfAccuracy = ...
-    additional_metrics_by_learn_block: List[ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock] = Field(..., alias="additionalMetricsByLearnBlock")
     available_variants: List[KerasModelVariantEnum] = Field(..., alias="availableVariants", description="List of all model variants for which classification results exist")
-    __properties = ["result", "predictions", "accuracy", "additionalMetricsByLearnBlock", "availableVariants"]
+    __properties = ["result", "predictions", "accuracy", "availableVariants"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -69,21 +67,14 @@
             for _item in self.predictions:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['predictions'] = _items
         # override the default output from pydantic by calling `to_dict()` of accuracy
         if self.accuracy:
             _dict['accuracy'] = self.accuracy.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in additional_metrics_by_learn_block (list)
-        _items = []
-        if self.additional_metrics_by_learn_block:
-            for _item in self.additional_metrics_by_learn_block:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['additionalMetricsByLearnBlock'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> ClassifyJobResponseAllOf:
         """Create an instance of ClassifyJobResponseAllOf from a dict"""
         if obj is None:
             return None
@@ -91,12 +82,11 @@
         if type(obj) is not dict:
             return ClassifyJobResponseAllOf.construct(**obj)
 
         _obj = ClassifyJobResponseAllOf.construct(**{
             "result": [ModelResult.from_dict(_item) for _item in obj.get("result")] if obj.get("result") is not None else None,
             "predictions": [ModelPrediction.from_dict(_item) for _item in obj.get("predictions")] if obj.get("predictions") is not None else None,
             "accuracy": ClassifyJobResponseAllOfAccuracy.from_dict(obj.get("accuracy")) if obj.get("accuracy") is not None else None,
-            "additional_metrics_by_learn_block": [ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock.from_dict(_item) for _item in obj.get("additionalMetricsByLearnBlock")] if obj.get("additionalMetricsByLearnBlock") is not None else None,
             "available_variants": obj.get("availableVariants")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_all_of_additional_metrics_by_learn_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,65 +13,65 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List
-from pydantic import BaseModel, Field, StrictInt, StrictStr
-from edgeimpulse_api.models.additional_metric import AdditionalMetric
-
-class ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock(BaseModel):
-    learn_block_id: StrictInt = Field(..., alias="learnBlockId")
-    learn_block_name: StrictStr = Field(..., alias="learnBlockName")
-    additional_metrics: List[AdditionalMetric] = Field(..., alias="additionalMetrics")
-    __properties = ["learnBlockId", "learnBlockName", "additionalMetrics"]
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+from edgeimpulse_api.models.add_organization_transformation_block_response_all_of import AddOrganizationTransformationBlockResponseAllOf
+
+class ObjectDetectionLabelQueueResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    samples: List[AddOrganizationTransformationBlockResponseAllOf] = ...
+    __properties = ["success", "error", "samples"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock:
-        """Create an instance of ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock from a JSON string"""
+    def from_json(cls, json_str: str) -> ObjectDetectionLabelQueueResponse:
+        """Create an instance of ObjectDetectionLabelQueueResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in additional_metrics (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in samples (list)
         _items = []
-        if self.additional_metrics:
-            for _item in self.additional_metrics:
+        if self.samples:
+            for _item in self.samples:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['additionalMetrics'] = _items
+            _dict['samples'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock:
-        """Create an instance of ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock from a dict"""
+    def from_dict(cls, obj: dict) -> ObjectDetectionLabelQueueResponse:
+        """Create an instance of ObjectDetectionLabelQueueResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock.construct(**obj)
+            return ObjectDetectionLabelQueueResponse.construct(**obj)
 
-        _obj = ClassifyJobResponseAllOfAdditionalMetricsByLearnBlock.construct(**{
-            "learn_block_id": obj.get("learnBlockId"),
-            "learn_block_name": obj.get("learnBlockName"),
-            "additional_metrics": [AdditionalMetric.from_dict(_item) for _item in obj.get("additionalMetrics")] if obj.get("additionalMetrics") is not None else None
+        _obj = ObjectDetectionLabelQueueResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "samples": [AddOrganizationTransformationBlockResponseAllOf.from_dict(_item) for _item in obj.get("samples")] if obj.get("samples") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_for_variants200_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_for_variants200_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_multiple_variants.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_multiple_variants.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_multiple_variants_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_multiple_variants_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_response_variant_results.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_response_variant_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/classify_sample_v2200_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/classify_sample_v2200_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_issue.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_issue.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_organization_usage_report_body.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_organization_usage_report_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_pro_tier_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,76 +16,74 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class CreateProTierUserRequest(BaseModel):
+class CreateUserRequest(BaseModel):
     name: StrictStr = Field(..., description="Your name")
     username: StrictStr = Field(..., description="Username, minimum 4 and maximum 30 characters. May contain alphanumeric characters, hyphens, underscores and dots. Validated according to `^(?=.{4,30}$)(?![_.])(?!.*[_.]{2})[a-zA-Z0-9._-]+(?<![_.])$`.")
     email: StrictStr = Field(..., description="E-mail address. Will need to be validated before the account will become active.")
     password: Optional[StrictStr] = Field(None, description="Password, minimum length 8 characters.")
     project_name: Optional[StrictStr] = Field(None, alias="projectName", description="A project will automatically be created. Sets the name of the first project. If not set, this will be derived from the username.")
     privacy_policy: StrictBool = Field(..., alias="privacyPolicy", description="Whether the user accepted the privacy policy")
     activation_token: Optional[StrictStr] = Field(None, alias="activationToken", description="Activation token for users created via SSO")
     identity_provider: Optional[StrictStr] = Field(None, alias="identityProvider", description="Unique identifier of the identity provider asserting the identity of this user")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle", description="Job title of the user. Optional field")
     session_id: Optional[StrictStr] = Field(None, alias="sessionId", description="Session ID. Optional field")
     company_name: Optional[StrictStr] = Field(None, alias="companyName", description="ACME Inc.")
     utm_params: Optional[List[Dict[str, Any]]] = Field(None, alias="utmParams", description="List of UTM parameters.")
-    redirect_url_origin: Optional[StrictStr] = Field(None, alias="redirectUrlOrigin", description="Origin of the redirect URL returned as result of creating the professional user.")
-    redirect_url_query_params: Optional[StrictStr] = Field(None, alias="redirectUrlQueryParams", description="Query parameters to be appended to the redirect URL returned as result of creating the professional user.")
-    __properties = ["name", "username", "email", "password", "projectName", "privacyPolicy", "activationToken", "identityProvider", "jobTitle", "sessionId", "companyName", "utmParams", "redirectUrlOrigin", "redirectUrlQueryParams"]
+    no_activation_email: Optional[StrictBool] = Field(None, alias="noActivationEmail", description="If set, no welcome email will be sent for account activation")
+    __properties = ["name", "username", "email", "password", "projectName", "privacyPolicy", "activationToken", "identityProvider", "jobTitle", "sessionId", "companyName", "utmParams", "noActivationEmail"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateProTierUserRequest:
-        """Create an instance of CreateProTierUserRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> CreateUserRequest:
+        """Create an instance of CreateUserRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateProTierUserRequest:
-        """Create an instance of CreateProTierUserRequest from a dict"""
+    def from_dict(cls, obj: dict) -> CreateUserRequest:
+        """Create an instance of CreateUserRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return CreateProTierUserRequest.construct(**obj)
+            return CreateUserRequest.construct(**obj)
 
-        _obj = CreateProTierUserRequest.construct(**{
+        _obj = CreateUserRequest.construct(**{
             "name": obj.get("name"),
             "username": obj.get("username"),
             "email": obj.get("email"),
             "password": obj.get("password"),
             "project_name": obj.get("projectName"),
             "privacy_policy": obj.get("privacyPolicy"),
             "activation_token": obj.get("activationToken"),
             "identity_provider": obj.get("identityProvider"),
             "job_title": obj.get("jobTitle"),
             "session_id": obj.get("sessionId"),
             "company_name": obj.get("companyName"),
             "utm_params": obj.get("utmParams"),
-            "redirect_url_origin": obj.get("redirectUrlOrigin"),
-            "redirect_url_query_params": obj.get("redirectUrlQueryParams")
+            "no_activation_email": obj.get("noActivationEmail")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_pro_tier_user_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_summary.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,55 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
+from typing import List
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class CreateProTierUserRequestAllOf(BaseModel):
-    redirect_url_origin: Optional[StrictStr] = Field(None, alias="redirectUrlOrigin", description="Origin of the redirect URL returned as result of creating the professional user.")
-    redirect_url_query_params: Optional[StrictStr] = Field(None, alias="redirectUrlQueryParams", description="Query parameters to be appended to the redirect URL returned as result of creating the professional user.")
-    __properties = ["redirectUrlOrigin", "redirectUrlQueryParams"]
+class ProjectDataSummary(BaseModel):
+    total_length_ms: float = Field(..., alias="totalLengthMs", description="Total length (in ms.) of all data in the training set")
+    labels: List[StrictStr] = Field(..., description="Labels in the training set")
+    data_count: StrictInt = Field(..., alias="dataCount")
+    __properties = ["totalLengthMs", "labels", "dataCount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateProTierUserRequestAllOf:
-        """Create an instance of CreateProTierUserRequestAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> ProjectDataSummary:
+        """Create an instance of ProjectDataSummary from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateProTierUserRequestAllOf:
-        """Create an instance of CreateProTierUserRequestAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> ProjectDataSummary:
+        """Create an instance of ProjectDataSummary from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return CreateProTierUserRequestAllOf.construct(**obj)
+            return ProjectDataSummary.construct(**obj)
 
-        _obj = CreateProTierUserRequestAllOf.construct(**{
-            "redirect_url_origin": obj.get("redirectUrlOrigin"),
-            "redirect_url_query_params": obj.get("redirectUrlQueryParams")
+        _obj = ProjectDataSummary.construct(**{
+            "total_length_ms": obj.get("totalLengthMs"),
+            "labels": obj.get("labels"),
+            "data_count": obj.get("dataCount")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,75 +13,75 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class CreateUserRequest(BaseModel):
-    name: StrictStr = Field(..., description="Your name")
-    username: StrictStr = Field(..., description="Username, minimum 4 and maximum 30 characters. May contain alphanumeric characters, hyphens, underscores and dots. Validated according to `^(?=.{4,30}$)(?![_.])(?!.*[_.]{2})[a-zA-Z0-9._-]+(?<![_.])$`.")
-    email: StrictStr = Field(..., description="E-mail address. Will need to be validated before the account will become active.")
-    password: Optional[StrictStr] = Field(None, description="Password, minimum length 8 characters.")
-    project_name: Optional[StrictStr] = Field(None, alias="projectName", description="A project will automatically be created. Sets the name of the first project. If not set, this will be derived from the username.")
-    privacy_policy: StrictBool = Field(..., alias="privacyPolicy", description="Whether the user accepted the privacy policy")
-    activation_token: Optional[StrictStr] = Field(None, alias="activationToken", description="Activation token for users created via SSO")
-    identity_provider: Optional[StrictStr] = Field(None, alias="identityProvider", description="Unique identifier of the identity provider asserting the identity of this user")
-    job_title: Optional[StrictStr] = Field(None, alias="jobTitle", description="Job title of the user. Optional field")
-    session_id: Optional[StrictStr] = Field(None, alias="sessionId", description="Session ID. Optional field")
-    company_name: Optional[StrictStr] = Field(None, alias="companyName", description="ACME Inc.")
-    utm_params: Optional[List[Dict[str, Any]]] = Field(None, alias="utmParams", description="List of UTM parameters.")
-    __properties = ["name", "username", "email", "password", "projectName", "privacyPolicy", "activationToken", "identityProvider", "jobTitle", "sessionId", "companyName", "utmParams"]
+class CreateWhitelabelRequest(BaseModel):
+    name: StrictStr = Field(..., description="The name of the white label.")
+    domain: StrictStr = Field(..., description="The domain where the white label lives.")
+    owner_organization_id: StrictInt = Field(..., alias="ownerOrganizationId")
+    identity_providers: Optional[List[StrictStr]] = Field(None, alias="identityProviders", description="The list of allowed identity providers.")
+    allow_password_auth: Optional[StrictBool] = Field(None, alias="allowPasswordAuth", description="Whether this white label accepts password based authentication.")
+    deployment_targets: Optional[List[StrictStr]] = Field(None, alias="deploymentTargets", description="The list of deployment targets to show on the UI")
+    documentation_url: Optional[StrictStr] = Field(None, alias="documentationUrl", description="Custom documentation URL")
+    allow_signup: Optional[StrictBool] = Field(None, alias="allowSignup", description="Whether this white label allow sign ups or not.")
+    allow_free_projects: Optional[StrictBool] = Field(None, alias="allowFreeProjects", description="Whether this white label allows the creation of free projects.")
+    sandboxed: Optional[StrictBool] = Field(None, description="Whether this white label should work in sandboxed mode or not.")
+    expose_public_projects: Optional[StrictBool] = Field(None, alias="exposePublicProjects", description="Whether public projects created in this white label scope should be exposed through the Public Projects API or not.")
+    learning_blocks: Optional[List[StrictStr]] = Field(None, alias="learningBlocks", description="The list of learning block types to show on the UI")
+    __properties = ["name", "domain", "ownerOrganizationId", "identityProviders", "allowPasswordAuth", "deploymentTargets", "documentationUrl", "allowSignup", "allowFreeProjects", "sandboxed", "exposePublicProjects", "learningBlocks"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateUserRequest:
-        """Create an instance of CreateUserRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> CreateWhitelabelRequest:
+        """Create an instance of CreateWhitelabelRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateUserRequest:
-        """Create an instance of CreateUserRequest from a dict"""
+    def from_dict(cls, obj: dict) -> CreateWhitelabelRequest:
+        """Create an instance of CreateWhitelabelRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return CreateUserRequest.construct(**obj)
+            return CreateWhitelabelRequest.construct(**obj)
 
-        _obj = CreateUserRequest.construct(**{
+        _obj = CreateWhitelabelRequest.construct(**{
             "name": obj.get("name"),
-            "username": obj.get("username"),
-            "email": obj.get("email"),
-            "password": obj.get("password"),
-            "project_name": obj.get("projectName"),
-            "privacy_policy": obj.get("privacyPolicy"),
-            "activation_token": obj.get("activationToken"),
-            "identity_provider": obj.get("identityProvider"),
-            "job_title": obj.get("jobTitle"),
-            "session_id": obj.get("sessionId"),
-            "company_name": obj.get("companyName"),
-            "utm_params": obj.get("utmParams")
+            "domain": obj.get("domain"),
+            "owner_organization_id": obj.get("ownerOrganizationId"),
+            "identity_providers": obj.get("identityProviders"),
+            "allow_password_auth": obj.get("allowPasswordAuth"),
+            "deployment_targets": obj.get("deploymentTargets"),
+            "documentation_url": obj.get("documentationUrl"),
+            "allow_signup": obj.get("allowSignup"),
+            "allow_free_projects": obj.get("allowFreeProjects"),
+            "sandboxed": obj.get("sandboxed"),
+            "expose_public_projects": obj.get("exposePublicProjects"),
+            "learning_blocks": obj.get("learningBlocks")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,76 +12,94 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-
-class CreateWhitelabelRequest(BaseModel):
-    name: StrictStr = Field(..., description="The name of the white label.")
-    domain: StrictStr = Field(..., description="The domain where the white label lives.")
-    owner_organization_id: StrictInt = Field(..., alias="ownerOrganizationId")
-    identity_providers: Optional[List[StrictStr]] = Field(None, alias="identityProviders", description="The list of allowed identity providers.")
-    allow_password_auth: Optional[StrictBool] = Field(None, alias="allowPasswordAuth", description="Whether this white label accepts password based authentication.")
-    deployment_targets: Optional[List[StrictStr]] = Field(None, alias="deploymentTargets", description="The list of deployment targets to show on the UI")
-    documentation_url: Optional[StrictStr] = Field(None, alias="documentationUrl", description="Custom documentation URL")
-    allow_signup: Optional[StrictBool] = Field(None, alias="allowSignup", description="Whether this white label allow sign ups or not.")
-    allow_free_projects: Optional[StrictBool] = Field(None, alias="allowFreeProjects", description="Whether this white label allows the creation of free projects.")
-    sandboxed: Optional[StrictBool] = Field(None, description="Whether this white label should work in sandboxed mode or not.")
-    expose_public_projects: Optional[StrictBool] = Field(None, alias="exposePublicProjects", description="Whether public projects created in this white label scope should be exposed through the Public Projects API or not.")
-    learning_blocks: Optional[List[StrictStr]] = Field(None, alias="learningBlocks", description="The list of learning block types to show on the UI")
-    __properties = ["name", "domain", "ownerOrganizationId", "identityProviders", "allowPasswordAuth", "deploymentTargets", "documentationUrl", "allowSignup", "allowFreeProjects", "sandboxed", "exposePublicProjects", "learningBlocks"]
+from edgeimpulse_api.models.permission import Permission
+from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.user_tier_enum import UserTierEnum
+
+class User(BaseModel):
+    id: StrictInt = ...
+    username: StrictStr = ...
+    name: StrictStr = ...
+    email: StrictStr = ...
+    photo: Optional[StrictStr] = None
+    created: datetime = ...
+    last_seen: Optional[datetime] = Field(None, alias="lastSeen")
+    staff_info: StaffInfo = Field(..., alias="staffInfo")
+    pending: StrictBool = ...
+    last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
+    job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
+    permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
+    company_name: Optional[StrictStr] = Field(None, alias="companyName")
+    activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
+    mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
+    stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
+    has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
+    tier: Optional[UserTierEnum] = None
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "tier"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateWhitelabelRequest:
-        """Create an instance of CreateWhitelabelRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> User:
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of staff_info
+        if self.staff_info:
+            _dict['staffInfo'] = self.staff_info.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateWhitelabelRequest:
-        """Create an instance of CreateWhitelabelRequest from a dict"""
+    def from_dict(cls, obj: dict) -> User:
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return CreateWhitelabelRequest.construct(**obj)
+            return User.construct(**obj)
 
-        _obj = CreateWhitelabelRequest.construct(**{
+        _obj = User.construct(**{
+            "id": obj.get("id"),
+            "username": obj.get("username"),
             "name": obj.get("name"),
-            "domain": obj.get("domain"),
-            "owner_organization_id": obj.get("ownerOrganizationId"),
-            "identity_providers": obj.get("identityProviders"),
-            "allow_password_auth": obj.get("allowPasswordAuth"),
-            "deployment_targets": obj.get("deploymentTargets"),
-            "documentation_url": obj.get("documentationUrl"),
-            "allow_signup": obj.get("allowSignup"),
-            "allow_free_projects": obj.get("allowFreeProjects"),
-            "sandboxed": obj.get("sandboxed"),
-            "expose_public_projects": obj.get("exposePublicProjects"),
-            "learning_blocks": obj.get("learningBlocks")
+            "email": obj.get("email"),
+            "photo": obj.get("photo"),
+            "created": obj.get("created"),
+            "last_seen": obj.get("lastSeen"),
+            "staff_info": StaffInfo.from_dict(obj.get("staffInfo")) if obj.get("staffInfo") is not None else None,
+            "pending": obj.get("pending"),
+            "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
+            "job_title": obj.get("jobTitle"),
+            "permissions": obj.get("permissions"),
+            "company_name": obj.get("companyName"),
+            "activated": obj.get("activated"),
+            "mfa_configured": obj.get("mfaConfigured"),
+            "stripe_customer_id": obj.get("stripeCustomerId"),
+            "has_pending_payments": obj.get("hasPendingPayments"),
+            "tier": obj.get("tier")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/created_updated_by_user.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/created_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/cross_validation_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/cross_validation_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/cross_validation_data_scores_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/cross_validation_data_scores_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_dashboard.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_dashboard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_graph.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_link.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_link.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_campaign_query.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_campaign_query.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/delete_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/delete_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_created_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_request_update.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_request_update.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_board_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_board_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_debug_stream_type.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_debug_stream_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_inference_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_inference_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_named_axis.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_named_axis.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/enterprise_trial.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/enterprise_trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class EnterpriseTrial(BaseModel):
     id: StrictInt = Field(..., description="Unique identifier of the trial.")
-    user_id: StrictInt = Field(..., alias="userId", description="ID of the user who created the trial.")
+    user_id: Optional[StrictInt] = Field(None, alias="userId", description="ID of the user who created the trial.")
     organization_id: StrictInt = Field(..., alias="organizationId", description="ID of the organization created for the trial.")
     created: datetime = Field(..., description="Date when the trial was created. Trials start immediately on creation.")
     expiration_date: datetime = Field(..., alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization. This field is ignored if the trial is requested by a non-admin user, defaulting to 14 days trial.")
     notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text. This field is ignored if the trial is requested by a non-admin user.")
     expired_date: Optional[datetime] = Field(..., alias="expiredDate", description="Date when the trial actually expired. This is set when the trial is expired by the system.")
     deleted_date: Optional[datetime] = Field(..., alias="deletedDate", description="Date when the trial was deleted. This is set when the trial is fully  deleted by the system.")
     upgraded_date: Optional[datetime] = Field(..., alias="upgradedDate", description="Date when the trial was upgraded to a full enterprise account.")
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/entitlement_limits.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/entity_created_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/entity_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/entity_created_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/entity_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_block_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_keras_block_data_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_keras_block_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/feature.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/feature.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/generic_api_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_imported_from_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_imported_from_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_imported_from_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_imported_from_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_segment_info_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_segment_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_auto_labeler_segment_info_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_auto_labeler_segment_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_code_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_code_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_code_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_code_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_status_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_email_verification_status_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_email_verification_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_feature_flags_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_feature_flags_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_feature_flags_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_records_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_records_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_records_request_range.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_records_request_range.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_label_noise_data_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_label_noise_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_label_noise_data_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_label_noise_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_model_variants_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_model_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_model_variants_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_model_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_bucket_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaign_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaigns_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_export_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_export_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_export_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_export_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_exports_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_exports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_deploy_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dsp_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transformation_block_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_organization_usage_report_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_target_constraints_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_target_constraints_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_target_constraints_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_target_constraints_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_need_to_set_password_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/image_input_scaling.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/image_input_scaling.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_created_by_user.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_created_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_details_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_details_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_failure_details.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_failure_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_logs_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_logs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_logs_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_logs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_metrics_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_metrics_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_parent_type_enum.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_parent_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_state.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_state.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_state_execution_details.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_state_execution_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_status.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_step.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_custom_metric.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_custom_metric.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,53 +14,56 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
 from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
 from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
-from edgeimpulse_api.models.keras_model_mode import KerasModelMode
 from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
 from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
 
-class KerasModelMetadata(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+class KerasModelMetadataAllOf(BaseModel):
     created: datetime = Field(..., description="Date when the model was trained")
     layers: List[KerasModelLayer] = Field(..., description="Layers of the neural network")
     class_names: List[StrictStr] = Field(..., alias="classNames", description="Labels for the output layer")
     labels: List[StrictStr] = Field(..., description="Original labels in the dataset when features were generated, e.g. used to render the feature explorer.")
     available_model_types: List[KerasModelTypeEnum] = Field(..., alias="availableModelTypes", description="The types of model that are available")
     recommended_model_type: KerasModelTypeEnum = Field(..., alias="recommendedModelType")
     model_validation_metrics: List[KerasModelMetadataMetrics] = Field(..., alias="modelValidationMetrics", description="Metrics for each of the available model types")
     has_trained_model: StrictBool = Field(..., alias="hasTrainedModel")
-    mode: KerasModelMode = ...
+    mode: StrictStr = ...
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     image_input_scaling: ImageInputScaling = Field(..., alias="imageInputScaling")
-    __properties = ["success", "error", "created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
+    __properties = ["created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
+
+    @validator('mode')
+    def mode_validate_enum(cls, v):
+        if v not in ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm'):
+            raise ValueError("must validate the enum values ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm')")
+        return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> KerasModelMetadata:
-        """Create an instance of KerasModelMetadata from a JSON string"""
+    def from_json(cls, json_str: str) -> KerasModelMetadataAllOf:
+        """Create an instance of KerasModelMetadataAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -78,25 +81,23 @@
             for _item in self.model_validation_metrics:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['modelValidationMetrics'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> KerasModelMetadata:
-        """Create an instance of KerasModelMetadata from a dict"""
+    def from_dict(cls, obj: dict) -> KerasModelMetadataAllOf:
+        """Create an instance of KerasModelMetadataAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return KerasModelMetadata.construct(**obj)
+            return KerasModelMetadataAllOf.construct(**obj)
 
-        _obj = KerasModelMetadata.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
+        _obj = KerasModelMetadataAllOf.construct(**{
             "created": obj.get("created"),
             "layers": [KerasModelLayer.from_dict(_item) for _item in obj.get("layers")] if obj.get("layers") is not None else None,
             "class_names": obj.get("classNames"),
             "labels": obj.get("labels"),
             "available_model_types": obj.get("availableModelTypes"),
             "recommended_model_type": obj.get("recommendedModelType"),
             "model_validation_metrics": [KerasModelMetadataMetrics.from_dict(_item) for _item in obj.get("modelValidationMetrics")] if obj.get("modelValidationMetrics") is not None else None,
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,51 +14,58 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
 from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
 from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
-from edgeimpulse_api.models.keras_model_mode import KerasModelMode
 from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
 from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
 
-class KerasModelMetadataAllOf(BaseModel):
+class KerasModelMetadata(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
     created: datetime = Field(..., description="Date when the model was trained")
     layers: List[KerasModelLayer] = Field(..., description="Layers of the neural network")
     class_names: List[StrictStr] = Field(..., alias="classNames", description="Labels for the output layer")
     labels: List[StrictStr] = Field(..., description="Original labels in the dataset when features were generated, e.g. used to render the feature explorer.")
     available_model_types: List[KerasModelTypeEnum] = Field(..., alias="availableModelTypes", description="The types of model that are available")
     recommended_model_type: KerasModelTypeEnum = Field(..., alias="recommendedModelType")
     model_validation_metrics: List[KerasModelMetadataMetrics] = Field(..., alias="modelValidationMetrics", description="Metrics for each of the available model types")
     has_trained_model: StrictBool = Field(..., alias="hasTrainedModel")
-    mode: KerasModelMode = ...
+    mode: StrictStr = ...
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     image_input_scaling: ImageInputScaling = Field(..., alias="imageInputScaling")
-    __properties = ["created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
+    __properties = ["success", "error", "created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
+
+    @validator('mode')
+    def mode_validate_enum(cls, v):
+        if v not in ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm'):
+            raise ValueError("must validate the enum values ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm')")
+        return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> KerasModelMetadataAllOf:
-        """Create an instance of KerasModelMetadataAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> KerasModelMetadata:
+        """Create an instance of KerasModelMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -76,23 +83,25 @@
             for _item in self.model_validation_metrics:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['modelValidationMetrics'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> KerasModelMetadataAllOf:
-        """Create an instance of KerasModelMetadataAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> KerasModelMetadata:
+        """Create an instance of KerasModelMetadata from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return KerasModelMetadataAllOf.construct(**obj)
+            return KerasModelMetadata.construct(**obj)
 
-        _obj = KerasModelMetadataAllOf.construct(**{
+        _obj = KerasModelMetadata.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
             "created": obj.get("created"),
             "layers": [KerasModelLayer.from_dict(_item) for _item in obj.get("layers")] if obj.get("layers") is not None else None,
             "class_names": obj.get("classNames"),
             "labels": obj.get("labels"),
             "available_model_types": obj.get("availableModelTypes"),
             "recommended_model_type": obj.get("recommendedModelType"),
             "model_validation_metrics": [KerasModelMetadataMetrics.from_dict(_item) for _item in obj.get("modelValidationMetrics")] if obj.get("modelValidationMetrics") is not None else None,
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
-from edgeimpulse_api.models.additional_metric import AdditionalMetric
 from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner import KerasModelMetadataMetricsOnDevicePerformanceInner
 from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
 from edgeimpulse_api.models.model_prediction import ModelPrediction
 
 class KerasModelMetadataMetrics(BaseModel):
     type: KerasModelTypeEnum = ...
     loss: float = Field(..., description="The model's loss on the validation set after training")
@@ -33,16 +32,15 @@
     on_device_performance: List[KerasModelMetadataMetricsOnDevicePerformanceInner] = Field(..., alias="onDevicePerformance")
     predictions: Optional[List[ModelPrediction]] = None
     visualization: StrictStr = ...
     is_supported_on_mcu: StrictBool = Field(..., alias="isSupportedOnMcu")
     mcu_support_error: Optional[StrictStr] = Field(None, alias="mcuSupportError")
     profiling_job_id: Optional[StrictInt] = Field(None, alias="profilingJobId", description="If this is set, then we're still profiling this model. Subscribe to job updates to see when it's done (afterward the metadata will be updated).")
     profiling_job_failed: Optional[StrictBool] = Field(None, alias="profilingJobFailed", description="If this is set, then the profiling job failed (get the status by getting the job logs for 'profilingJobId').")
-    additional_metrics: List[AdditionalMetric] = Field(..., alias="additionalMetrics")
-    __properties = ["type", "loss", "accuracy", "confusionMatrix", "report", "onDevicePerformance", "predictions", "visualization", "isSupportedOnMcu", "mcuSupportError", "profilingJobId", "profilingJobFailed", "additionalMetrics"]
+    __properties = ["type", "loss", "accuracy", "confusionMatrix", "report", "onDevicePerformance", "predictions", "visualization", "isSupportedOnMcu", "mcuSupportError", "profilingJobId", "profilingJobFailed"]
 
     @validator('visualization')
     def visualization_validate_enum(cls, v):
         if v not in ('featureExplorer', 'dataExplorer', 'none'):
             raise ValueError("must validate the enum values ('featureExplorer', 'dataExplorer', 'none')")
         return v
 
@@ -79,21 +77,14 @@
         # override the default output from pydantic by calling `to_dict()` of each item in predictions (list)
         _items = []
         if self.predictions:
             for _item in self.predictions:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['predictions'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in additional_metrics (list)
-        _items = []
-        if self.additional_metrics:
-            for _item in self.additional_metrics:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['additionalMetrics'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> KerasModelMetadataMetrics:
         """Create an instance of KerasModelMetadataMetrics from a dict"""
         if obj is None:
             return None
@@ -109,12 +100,11 @@
             "report": obj.get("report"),
             "on_device_performance": [KerasModelMetadataMetricsOnDevicePerformanceInner.from_dict(_item) for _item in obj.get("onDevicePerformance")] if obj.get("onDevicePerformance") is not None else None,
             "predictions": [ModelPrediction.from_dict(_item) for _item in obj.get("predictions")] if obj.get("predictions") is not None else None,
             "visualization": obj.get("visualization"),
             "is_supported_on_mcu": obj.get("isSupportedOnMcu"),
             "mcu_support_error": obj.get("mcuSupportError"),
             "profiling_job_id": obj.get("profilingJobId"),
-            "profiling_job_failed": obj.get("profilingJobFailed"),
-            "additional_metrics": [AdditionalMetric.from_dict(_item) for _item in obj.get("additionalMetrics")] if obj.get("additionalMetrics") is not None else None
+            "profiling_job_failed": obj.get("profilingJobFailed")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_mode.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class KerasModelMode(str, Enum):
+class OrganizationTransferLearningOperatesOn(str, Enum):
     """
     allowed enum values
     """
 
-    CLASSIFICATION = 'classification'
+    OBJECT_DETECTION = 'object_detection'
+    AUDIO = 'audio'
+    IMAGE = 'image'
     REGRESSION = 'regression'
-    OBJECT_DETECTION = 'object-detection'
-    VISUAL_ANOMALY = 'visual-anomaly'
-    ANOMALY_GMM = 'anomaly-gmm'
+    OTHER = 'other'
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_model_variant_enum.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_model_variant_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_enterprise_trials_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_enterprise_trials_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_usage_reports_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_tuner_runs_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_tuner_runs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_tuner_runs_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_tuner_runs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_analytics_event_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_analytics_event_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/memory_spec.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/memory_spec.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/metrics_all_variants_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/metrics_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/metrics_all_variants_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/metrics_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/metrics_for_model_variant.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/metrics_for_model_variant.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/migration.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/migration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_engine_short_enum.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_engine_short_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/neighbors_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/neighbors_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/neighbors_score.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/neighbors_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_job_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,65 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
-from edgeimpulse_api.models.add_organization_transformation_block_response_all_of import AddOrganizationTransformationBlockResponseAllOf
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class ObjectDetectionLabelQueueResponse(BaseModel):
+class StartJobResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    samples: List[AddOrganizationTransformationBlockResponseAllOf] = ...
-    __properties = ["success", "error", "samples"]
+    id: StrictInt = Field(..., description="Job identifier. Status updates will include this identifier.")
+    __properties = ["success", "error", "id"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ObjectDetectionLabelQueueResponse:
-        """Create an instance of ObjectDetectionLabelQueueResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> StartJobResponse:
+        """Create an instance of StartJobResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in samples (list)
-        _items = []
-        if self.samples:
-            for _item in self.samples:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['samples'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ObjectDetectionLabelQueueResponse:
-        """Create an instance of ObjectDetectionLabelQueueResponse from a dict"""
+    def from_dict(cls, obj: dict) -> StartJobResponse:
+        """Create an instance of StartJobResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ObjectDetectionLabelQueueResponse.construct(**obj)
+            return StartJobResponse.construct(**obj)
 
-        _obj = ObjectDetectionLabelQueueResponse.construct(**{
+        _obj = StartJobResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
-            "samples": [AddOrganizationTransformationBlockResponseAllOf.from_dict(_item) for _item in obj.get("samples")] if obj.get("samples") is not None else None
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_dataset_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_add_dataset_request_bucket.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_add_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_bucket.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_compute_time_usage.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_compute_time_usage.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_path_filter.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_path_filter.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_export.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_export.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_dataset_bucket.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_dataset_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_info_response_all_of_performance.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_member_role.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_run_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class OrganizationTransferLearningOperatesOn(str, Enum):
+class TransformationJobStatusEnum(str, Enum):
     """
     allowed enum values
     """
 
-    OBJECT_DETECTION = 'object_detection'
-    AUDIO = 'audio'
-    IMAGE = 'image'
-    REGRESSION = 'regression'
-    OTHER = 'other'
+    WAITING = 'waiting'
+    CREATED = 'created'
+    STARTED = 'started'
+    FINISHED = 'finished'
+    FAILED = 'failed'
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_usage_report.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_usage_report.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/organization_user_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/organization_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameter_set.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/permission.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,17 +32,16 @@
     ADMINMETRICSREAD = 'admin:metrics:read'
     ADMINORGANIZATIONSREAD = 'admin:organizations:read'
     ADMINORGANIZATIONSWRITE = 'admin:organizations:write'
     ADMINORGANIZATIONSMEMBERSWRITE = 'admin:organizations:members:write'
     ADMINPROJECTSMEMBERSWRITE = 'admin:projects:members:write'
     ADMINPROJECTSREAD = 'admin:projects:read'
     ADMINPROJECTSWRITE = 'admin:projects:write'
-    ADMINTRIALSREAD = 'admin:trials:read'
-    ADMINTRIALSWRITE = 'admin:trials:write'
     ADMINUSERSPERMISSIONSWRITE = 'admin:users:permissions:write'
+    ADMINUSERSTRIALSWRITE = 'admin:users:trials:write'
     ADMINUSERSREAD = 'admin:users:read'
     ADMINUSERSWRITE = 'admin:users:write'
     ADMINJOBSREAD = 'admin:jobs:read'
     ADMINEMAILSVERIFICATIONCODEREAD = 'admin:emails:verification:code:read'
     PROJECTSLIMITSWRITE = 'projects:limits:write'
     PROJECTSTRAININGKERASWRITE = 'projects:training:keras:write'
     THIRDPARTYAUTHREAD = 'thirdpartyauth:read'
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/portal_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/preview_default_files_in_folder_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/preview_default_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/preview_default_files_in_folder_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/preview_default_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_collaborator.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,54 +16,52 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class ProjectDataSummary(BaseModel):
-    total_length_ms: float = Field(..., alias="totalLengthMs", description="Total length (in ms.) of all data in the training set")
+class ProjectTrainingDataSummaryResponseAllOfDataSummary(BaseModel):
     labels: List[StrictStr] = Field(..., description="Labels in the training set")
     data_count: StrictInt = Field(..., alias="dataCount")
-    __properties = ["totalLengthMs", "labels", "dataCount"]
+    __properties = ["labels", "dataCount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ProjectDataSummary:
-        """Create an instance of ProjectDataSummary from a JSON string"""
+    def from_json(cls, json_str: str) -> ProjectTrainingDataSummaryResponseAllOfDataSummary:
+        """Create an instance of ProjectTrainingDataSummaryResponseAllOfDataSummary from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ProjectDataSummary:
-        """Create an instance of ProjectDataSummary from a dict"""
+    def from_dict(cls, obj: dict) -> ProjectTrainingDataSummaryResponseAllOfDataSummary:
+        """Create an instance of ProjectTrainingDataSummaryResponseAllOfDataSummary from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ProjectDataSummary.construct(**obj)
+            return ProjectTrainingDataSummaryResponseAllOfDataSummary.construct(**obj)
 
-        _obj = ProjectDataSummary.construct(**{
-            "total_length_ms": obj.get("totalLengthMs"),
+        _obj = ProjectTrainingDataSummaryResponseAllOfDataSummary.construct(**{
             "labels": obj.get("labels"),
             "data_count": obj.get("dataCount")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_dismiss_notification_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_model_variant.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_model_variant.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_public_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_tier_enum.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_tier_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,55 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List
-from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class ProjectTrainingDataSummaryResponseAllOfDataSummary(BaseModel):
-    labels: List[StrictStr] = Field(..., description="Labels in the training set")
-    data_count: StrictInt = Field(..., alias="dataCount")
-    __properties = ["labels", "dataCount"]
+from pydantic import BaseModel
+
+class ScoreTrialResponseAllOfRam(BaseModel):
+    dsp: float = ...
+    learn: float = ...
+    __properties = ["dsp", "learn"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ProjectTrainingDataSummaryResponseAllOfDataSummary:
-        """Create an instance of ProjectTrainingDataSummaryResponseAllOfDataSummary from a JSON string"""
+    def from_json(cls, json_str: str) -> ScoreTrialResponseAllOfRam:
+        """Create an instance of ScoreTrialResponseAllOfRam from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ProjectTrainingDataSummaryResponseAllOfDataSummary:
-        """Create an instance of ProjectTrainingDataSummaryResponseAllOfDataSummary from a dict"""
+    def from_dict(cls, obj: dict) -> ScoreTrialResponseAllOfRam:
+        """Create an instance of ScoreTrialResponseAllOfRam from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ProjectTrainingDataSummaryResponseAllOfDataSummary.construct(**obj)
+            return ScoreTrialResponseAllOfRam.construct(**obj)
 
-        _obj = ProjectTrainingDataSummaryResponseAllOfDataSummary.construct(**{
-            "labels": obj.get("labels"),
-            "data_count": obj.get("dataCount")
+        _obj = ScoreTrialResponseAllOfRam.construct(**{
+            "dsp": obj.get("dsp"),
+            "learn": obj.get("learn")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_type.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/public_organization_transformation_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/public_organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/public_project_tier_availability.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/public_project_tier_availability.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/request_email_verification_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/request_email_verification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/resource_range.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/resource_range.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/run_auto_labeler_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/run_auto_labeler_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,56 +12,56 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
+from datetime import datetime
 
+from pydantic import BaseModel, Field, StrictStr
 
-from pydantic import BaseModel
-
-class ScoreTrialResponseAllOfRam(BaseModel):
-    dsp: float = ...
-    learn: float = ...
-    __properties = ["dsp", "learn"]
+class SocketTokenResponseAllOfToken(BaseModel):
+    socket_token: StrictStr = Field(..., alias="socketToken")
+    expires: datetime = ...
+    __properties = ["socketToken", "expires"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ScoreTrialResponseAllOfRam:
-        """Create an instance of ScoreTrialResponseAllOfRam from a JSON string"""
+    def from_json(cls, json_str: str) -> SocketTokenResponseAllOfToken:
+        """Create an instance of SocketTokenResponseAllOfToken from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ScoreTrialResponseAllOfRam:
-        """Create an instance of ScoreTrialResponseAllOfRam from a dict"""
+    def from_dict(cls, obj: dict) -> SocketTokenResponseAllOfToken:
+        """Create an instance of SocketTokenResponseAllOfToken from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ScoreTrialResponseAllOfRam.construct(**obj)
+            return SocketTokenResponseAllOfToken.construct(**obj)
 
-        _obj = ScoreTrialResponseAllOfRam.construct(**{
-            "dsp": obj.get("dsp"),
-            "learn": obj.get("learn")
+        _obj = SocketTokenResponseAllOfToken.construct(**{
+            "socket_token": obj.get("socketToken"),
+            "expires": obj.get("expires")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/sensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_sample_structured_labels_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_sample_structured_labels_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,56 +12,54 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
 
-from pydantic import BaseModel, Field, StrictStr
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 
-class SocketTokenResponseAllOfToken(BaseModel):
-    socket_token: StrictStr = Field(..., alias="socketToken")
-    expires: datetime = ...
-    __properties = ["socketToken", "expires"]
+class UploadAssetResponseAllOf(BaseModel):
+    url: Optional[StrictStr] = None
+    __properties = ["url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SocketTokenResponseAllOfToken:
-        """Create an instance of SocketTokenResponseAllOfToken from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadAssetResponseAllOf:
+        """Create an instance of UploadAssetResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SocketTokenResponseAllOfToken:
-        """Create an instance of SocketTokenResponseAllOfToken from a dict"""
+    def from_dict(cls, obj: dict) -> UploadAssetResponseAllOf:
+        """Create an instance of UploadAssetResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SocketTokenResponseAllOfToken.construct(**obj)
+            return UploadAssetResponseAllOf.construct(**obj)
 
-        _obj = SocketTokenResponseAllOfToken.construct(**{
-            "socket_token": obj.get("socketToken"),
-            "expires": obj.get("expires")
+        _obj = UploadAssetResponseAllOf.construct(**{
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_classify_job_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_classify_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_device_debug_stream_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_device_debug_stream_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_enterprise_trial_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,39 +13,42 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, validator
-
-class StartEnterpriseTrialRequest(BaseModel):
-    email: Optional[StrictStr] = Field(None, description="Email of the user requesting the trial. If this email is different to the one stored for the user requesting the trial, it will be used to replace the existing one.")
-    organization_name: Optional[StrictStr] = Field(None, alias="organizationName", description="Name of the trial organization. All enterprise features are tied to an organization. This organization will be deleted after the trial ends. If no organization name is provided, the user's name will be used.")
-    expiration_date: Optional[datetime] = Field(None, alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization. This field is ignored if the trial is requested by a non-admin user, defaulting to 14 days trial.")
-    notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text. This field is ignored if the trial is requested by a non-admin user.")
-    use_case: Optional[StrictStr] = Field(None, alias="useCase", description="Use case of the trial.")
-    user_has_ml_models_in_production: Optional[StrictStr] = Field(None, alias="userHasMLModelsInProduction", description="Whether the user has ML models in production.")
-    company_name: Optional[StrictStr] = Field(None, alias="companyName", description="Name of the company requesting the trial.")
-    company_size: Optional[StrictStr] = Field(None, alias="companySize", description="Size of the company requesting the trial. This is a range of number of employees.")
-    country: Optional[StrictStr] = Field(None, description="Country of the company requesting the trial.")
-    state_or_province: Optional[StrictStr] = Field(None, alias="stateOrProvince", description="State or province of the company requesting the trial.")
-    redirect_url_origin: Optional[StrictStr] = Field(None, alias="redirectUrlOrigin", description="Origin of the redirect URL returned as result of creating the trial user.")
-    redirect_url_query_params: Optional[StrictStr] = Field(None, alias="redirectUrlQueryParams", description="Query parameters to be appended to the redirect URL returned as result of creating the trial user.")
-    __properties = ["email", "organizationName", "expirationDate", "notes", "useCase", "userHasMLModelsInProduction", "companyName", "companySize", "country", "stateOrProvince", "redirectUrlOrigin", "redirectUrlQueryParams"]
-
-    @validator('user_has_ml_models_in_production')
-    def user_has_ml_models_in_production_validate_enum(cls, v):
-        if v is None:
-            return v
-
-        if v not in ('yes', 'no', 'no, but we will soon'):
-            raise ValueError("must validate the enum values ('yes', 'no', 'no, but we will soon')")
+from typing import Any, Dict, List, Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
+from edgeimpulse_api.models.tuner_trial_blocks_inner import TunerTrialBlocksInner
+from edgeimpulse_api.models.tuner_trial_dsp_job_id import TunerTrialDspJobId
+from edgeimpulse_api.models.tuner_trial_impulse import TunerTrialImpulse
+
+class TunerTrial(BaseModel):
+    id: StrictStr = ...
+    status: StrictStr = ...
+    last_completed_epoch: Optional[datetime] = Field(None, alias="lastCompletedEpoch")
+    last_completed_training: Optional[datetime] = Field(None, alias="lastCompletedTraining")
+    retries: Optional[StrictInt] = None
+    current_epoch: Optional[StrictInt] = Field(None, alias="currentEpoch")
+    worker_id: Optional[StrictStr] = Field(None, alias="workerId")
+    blocks: List[TunerTrialBlocksInner] = ...
+    impulse: TunerTrialImpulse = ...
+    experiment: Optional[StrictStr] = None
+    original_trial_id: Optional[StrictStr] = None
+    model: Optional[Dict[str, Any]] = None
+    dsp_job_id: Optional[TunerTrialDspJobId] = Field(None, alias="dspJobId")
+    learn_job_id: Optional[float] = Field(None, alias="learnJobId")
+    device_performance: Optional[Dict[str, Any]] = Field(None, alias="devicePerformance")
+    __properties = ["id", "status", "lastCompletedEpoch", "lastCompletedTraining", "retries", "currentEpoch", "workerId", "blocks", "impulse", "experiment", "original_trial_id", "model", "dspJobId", "learnJobId", "devicePerformance"]
+
+    @validator('status')
+    def status_validate_enum(cls, v):
+        if v not in ('pending', 'running', 'completed', 'failed'):
+            raise ValueError("must validate the enum values ('pending', 'running', 'completed', 'failed')")
         return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -53,44 +56,60 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StartEnterpriseTrialRequest:
-        """Create an instance of StartEnterpriseTrialRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> TunerTrial:
+        """Create an instance of TunerTrial from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in blocks (list)
+        _items = []
+        if self.blocks:
+            for _item in self.blocks:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['blocks'] = _items
+        # override the default output from pydantic by calling `to_dict()` of impulse
+        if self.impulse:
+            _dict['impulse'] = self.impulse.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of dsp_job_id
+        if self.dsp_job_id:
+            _dict['dspJobId'] = self.dsp_job_id.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StartEnterpriseTrialRequest:
-        """Create an instance of StartEnterpriseTrialRequest from a dict"""
+    def from_dict(cls, obj: dict) -> TunerTrial:
+        """Create an instance of TunerTrial from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return StartEnterpriseTrialRequest.construct(**obj)
+            return TunerTrial.construct(**obj)
 
-        _obj = StartEnterpriseTrialRequest.construct(**{
-            "email": obj.get("email"),
-            "organization_name": obj.get("organizationName"),
-            "expiration_date": obj.get("expirationDate"),
-            "notes": obj.get("notes"),
-            "use_case": obj.get("useCase"),
-            "user_has_ml_models_in_production": obj.get("userHasMLModelsInProduction"),
-            "company_name": obj.get("companyName"),
-            "company_size": obj.get("companySize"),
-            "country": obj.get("country"),
-            "state_or_province": obj.get("stateOrProvince"),
-            "redirect_url_origin": obj.get("redirectUrlOrigin"),
-            "redirect_url_query_params": obj.get("redirectUrlQueryParams")
+        _obj = TunerTrial.construct(**{
+            "id": obj.get("id"),
+            "status": obj.get("status"),
+            "last_completed_epoch": obj.get("lastCompletedEpoch"),
+            "last_completed_training": obj.get("lastCompletedTraining"),
+            "retries": obj.get("retries"),
+            "current_epoch": obj.get("currentEpoch"),
+            "worker_id": obj.get("workerId"),
+            "blocks": [TunerTrialBlocksInner.from_dict(_item) for _item in obj.get("blocks")] if obj.get("blocks") is not None else None,
+            "impulse": TunerTrialImpulse.from_dict(obj.get("impulse")) if obj.get("impulse") is not None else None,
+            "experiment": obj.get("experiment"),
+            "original_trial_id": obj.get("original_trial_id"),
+            "model": obj.get("model"),
+            "dsp_job_id": TunerTrialDspJobId.from_dict(obj.get("dspJobId")) if obj.get("dspJobId") is not None else None,
+            "learn_job_id": obj.get("learnJobId"),
+            "device_performance": obj.get("devicePerformance")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_sampling_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class StartJobResponse(BaseModel):
+class StartSamplingResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    id: StrictInt = Field(..., description="Job identifier. Status updates will include this identifier.")
+    id: Optional[StrictInt] = None
     __properties = ["success", "error", "id"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -35,35 +35,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StartJobResponse:
-        """Create an instance of StartJobResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> StartSamplingResponse:
+        """Create an instance of StartSamplingResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StartJobResponse:
-        """Create an instance of StartJobResponse from a dict"""
+    def from_dict(cls, obj: dict) -> StartSamplingResponse:
+        """Create an instance of StartSamplingResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return StartJobResponse.construct(**obj)
+            return StartSamplingResponse.construct(**obj)
 
-        _obj = StartJobResponse.construct(**{
+        _obj = StartSamplingResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
             "id": obj.get("id")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,56 +14,52 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, StrictInt
 
-class StartSamplingResponse(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+class StartSamplingResponseAllOf(BaseModel):
     id: Optional[StrictInt] = None
-    __properties = ["success", "error", "id"]
+    __properties = ["id"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StartSamplingResponse:
-        """Create an instance of StartSamplingResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> StartSamplingResponseAllOf:
+        """Create an instance of StartSamplingResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StartSamplingResponse:
-        """Create an instance of StartSamplingResponse from a dict"""
+    def from_dict(cls, obj: dict) -> StartSamplingResponseAllOf:
+        """Create an instance of StartSamplingResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return StartSamplingResponse.construct(**obj)
+            return StartSamplingResponseAllOf.construct(**obj)
 
-        _obj = StartSamplingResponse.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
+        _obj = StartSamplingResponseAllOf.construct(**{
             "id": obj.get("id")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,53 +13,53 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictInt
 
-class StartSamplingResponseAllOf(BaseModel):
-    id: Optional[StrictInt] = None
-    __properties = ["id"]
+from pydantic import BaseModel, StrictStr
+
+class VerifyDspBlockUrlRequest(BaseModel):
+    url: StrictStr = ...
+    __properties = ["url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StartSamplingResponseAllOf:
-        """Create an instance of StartSamplingResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyDspBlockUrlRequest:
+        """Create an instance of VerifyDspBlockUrlRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StartSamplingResponseAllOf:
-        """Create an instance of StartSamplingResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlRequest:
+        """Create an instance of VerifyDspBlockUrlRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return StartSamplingResponseAllOf.construct(**obj)
+            return VerifyDspBlockUrlRequest.construct(**obj)
 
-        _obj = StartSamplingResponseAllOf.construct(**{
-            "id": obj.get("id")
+        _obj = VerifyDspBlockUrlRequest.construct(**{
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/stop_device_debug_stream_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,52 +14,54 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, StrictStr
 
-class StopDeviceDebugStreamRequest(BaseModel):
-    stream_id: StrictInt = Field(..., alias="streamId")
-    __properties = ["streamId"]
+class VerifyResetPasswordRequest(BaseModel):
+    email: StrictStr = ...
+    code: StrictStr = ...
+    __properties = ["email", "code"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StopDeviceDebugStreamRequest:
-        """Create an instance of StopDeviceDebugStreamRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyResetPasswordRequest:
+        """Create an instance of VerifyResetPasswordRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StopDeviceDebugStreamRequest:
-        """Create an instance of StopDeviceDebugStreamRequest from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyResetPasswordRequest:
+        """Create an instance of VerifyResetPasswordRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return StopDeviceDebugStreamRequest.construct(**obj)
+            return VerifyResetPasswordRequest.construct(**obj)
 
-        _obj = StopDeviceDebugStreamRequest.construct(**{
-            "stream_id": obj.get("streamId")
+        _obj = VerifyResetPasswordRequest.construct(**{
+            "email": obj.get("email"),
+            "code": obj.get("code")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/structured_label.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/structured_label.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_constraints.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_constraints.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_constraints_device.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_constraints_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_memory.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/target_processor.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/target_processor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/theme_logos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/time_series_data_point.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/time_series_data_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/transformation_job_operates_on_enum.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/transformation_job_operates_on_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_run.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_trial_dsp_job_id.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial_dsp_job_id.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/tuner_trial_impulse.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/tuner_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_data_campaign_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_dataset_request_bucket.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_organization_transformation_block_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_tuner_run_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_tuner_run_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_asset_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,52 +14,56 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UpdateVersionRequest(BaseModel):
-    description: Optional[StrictStr] = None
-    __properties = ["description"]
+class UploadAssetResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    url: Optional[StrictStr] = None
+    __properties = ["success", "error", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateVersionRequest:
-        """Create an instance of UpdateVersionRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadAssetResponse:
+        """Create an instance of UploadAssetResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateVersionRequest:
-        """Create an instance of UpdateVersionRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UploadAssetResponse:
+        """Create an instance of UploadAssetResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateVersionRequest.construct(**obj)
+            return UploadAssetResponse.construct(**obj)
 
-        _obj = UpdateVersionRequest.construct(**{
-            "description": obj.get("description")
+        _obj = UploadAssetResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/update_whitelabel_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/update_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/upgrade_subscription_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/upgrade_subscription_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UploadAssetResponse(BaseModel):
+class UploadUserPhotoResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    url: Optional[StrictStr] = None
+    url: StrictStr = ...
     __properties = ["success", "error", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -35,35 +35,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadAssetResponse:
-        """Create an instance of UploadAssetResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadUserPhotoResponse:
+        """Create an instance of UploadUserPhotoResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadAssetResponse:
-        """Create an instance of UploadAssetResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UploadUserPhotoResponse:
+        """Create an instance of UploadUserPhotoResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadAssetResponse.construct(**obj)
+            return UploadUserPhotoResponse.construct(**obj)
 
-        _obj = UploadAssetResponse.construct(**{
+        _obj = UploadUserPhotoResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,52 +14,56 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
+from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
 
-class UploadAssetResponseAllOf(BaseModel):
-    url: Optional[StrictStr] = None
-    __properties = ["url"]
+class VerifyDspBlockUrlResponseAllOf(BaseModel):
+    block: Optional[VerifyDspBlockUrlResponseAllOfBlock] = None
+    __properties = ["block"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadAssetResponseAllOf:
-        """Create an instance of UploadAssetResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOf:
+        """Create an instance of VerifyDspBlockUrlResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of block
+        if self.block:
+            _dict['block'] = self.block.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadAssetResponseAllOf:
-        """Create an instance of UploadAssetResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOf:
+        """Create an instance of VerifyDspBlockUrlResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadAssetResponseAllOf.construct(**obj)
+            return VerifyDspBlockUrlResponseAllOf.construct(**obj)
 
-        _obj = UploadAssetResponseAllOf.construct(**{
-            "url": obj.get("url")
+        _obj = VerifyDspBlockUrlResponseAllOf.construct(**{
+            "block": VerifyDspBlockUrlResponseAllOfBlock.from_dict(obj.get("block")) if obj.get("block") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_generate_new_mfa_key_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,54 +16,56 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UploadUserPhotoResponse(BaseModel):
+class UserGenerateNewMfaKeyResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    url: StrictStr = ...
-    __properties = ["success", "error", "url"]
+    key: StrictStr = Field(..., description="Secret key (use SHA-1).")
+    url: StrictStr = Field(..., description="URL that will be converted into a QR code that can be scanned.")
+    __properties = ["success", "error", "key", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadUserPhotoResponse:
-        """Create an instance of UploadUserPhotoResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponse:
+        """Create an instance of UserGenerateNewMfaKeyResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadUserPhotoResponse:
-        """Create an instance of UploadUserPhotoResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponse:
+        """Create an instance of UserGenerateNewMfaKeyResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadUserPhotoResponse.construct(**obj)
+            return UserGenerateNewMfaKeyResponse.construct(**obj)
 
-        _obj = UploadUserPhotoResponse.construct(**{
+        _obj = UserGenerateNewMfaKeyResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
+            "key": obj.get("key"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_dismiss_notification_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_experiment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_generate_new_mfa_key_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,59 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UserGenerateNewMfaKeyResponse(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+from pydantic import BaseModel, Field, StrictStr
+
+class UserGenerateNewMfaKeyResponseAllOf(BaseModel):
     key: StrictStr = Field(..., description="Secret key (use SHA-1).")
     url: StrictStr = Field(..., description="URL that will be converted into a QR code that can be scanned.")
-    __properties = ["success", "error", "key", "url"]
+    __properties = ["key", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponse:
-        """Create an instance of UserGenerateNewMfaKeyResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponseAllOf:
+        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponse:
-        """Create an instance of UserGenerateNewMfaKeyResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponseAllOf:
+        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserGenerateNewMfaKeyResponse.construct(**obj)
+            return UserGenerateNewMfaKeyResponseAllOf.construct(**obj)
 
-        _obj = UserGenerateNewMfaKeyResponse.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
+        _obj = UserGenerateNewMfaKeyResponseAllOf.construct(**{
             "key": obj.get("key"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_set_totp_mfa_key_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,52 +16,52 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr
 
-class UserGenerateNewMfaKeyResponseAllOf(BaseModel):
-    key: StrictStr = Field(..., description="Secret key (use SHA-1).")
-    url: StrictStr = Field(..., description="URL that will be converted into a QR code that can be scanned.")
-    __properties = ["key", "url"]
+class UserSetTotpMfaKeyRequest(BaseModel):
+    key: StrictStr = Field(..., description="Secret key obtained through `userGenerateNewMfaKey`.")
+    totp_token: StrictStr = Field(..., alias="totpToken", description="TOTP token that is valid for the key (to ensure the device is configured correctly)")
+    __properties = ["key", "totpToken"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponseAllOf:
-        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> UserSetTotpMfaKeyRequest:
+        """Create an instance of UserSetTotpMfaKeyRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponseAllOf:
-        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> UserSetTotpMfaKeyRequest:
+        """Create an instance of UserSetTotpMfaKeyRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserGenerateNewMfaKeyResponseAllOf.construct(**obj)
+            return UserSetTotpMfaKeyRequest.construct(**obj)
 
-        _obj = UserGenerateNewMfaKeyResponseAllOf.construct(**{
+        _obj = UserSetTotpMfaKeyRequest.construct(**{
             "key": obj.get("key"),
-            "url": obj.get("url")
+            "totp_token": obj.get("totpToken")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_organization.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_projects_sort_order.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_projects_sort_order.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_set_totp_mfa_key_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_email_response_all_of.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,55 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class UserSetTotpMfaKeyRequest(BaseModel):
-    key: StrictStr = Field(..., description="Secret key obtained through `userGenerateNewMfaKey`.")
-    totp_token: StrictStr = Field(..., alias="totpToken", description="TOTP token that is valid for the key (to ensure the device is configured correctly)")
-    __properties = ["key", "totpToken"]
+class VerifyEmailResponseAllOf(BaseModel):
+    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
+    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
+    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
+    __properties = ["email", "userId", "redirectUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserSetTotpMfaKeyRequest:
-        """Create an instance of UserSetTotpMfaKeyRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyEmailResponseAllOf:
+        """Create an instance of VerifyEmailResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserSetTotpMfaKeyRequest:
-        """Create an instance of UserSetTotpMfaKeyRequest from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyEmailResponseAllOf:
+        """Create an instance of VerifyEmailResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserSetTotpMfaKeyRequest.construct(**obj)
+            return VerifyEmailResponseAllOf.construct(**obj)
 
-        _obj = UserSetTotpMfaKeyRequest.construct(**{
-            "key": obj.get("key"),
-            "totp_token": obj.get("totpToken")
+        _obj = VerifyEmailResponseAllOf.construct(**{
+            "email": obj.get("email"),
+            "user_id": obj.get("userId"),
+            "redirect_url": obj.get("redirectUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_set_totp_mfa_key_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_set_totp_mfa_key_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_subscription_metrics_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_subscription_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_subscription_metrics_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_subscription_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_subscription_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_subscription_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/user_tier_enum.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/user_tier_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,52 +14,56 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class VerifyDspBlockUrlRequest(BaseModel):
-    url: StrictStr = ...
-    __properties = ["url"]
+class VerifyOrganizationBucketResponseAllOfFiles(BaseModel):
+    name: StrictStr = ...
+    size: StrictInt = ...
+    folder_name: StrictStr = Field(..., alias="folderName")
+    __properties = ["name", "size", "folderName"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyDspBlockUrlRequest:
-        """Create an instance of VerifyDspBlockUrlRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOfFiles:
+        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlRequest:
-        """Create an instance of VerifyDspBlockUrlRequest from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOfFiles:
+        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyDspBlockUrlRequest.construct(**obj)
+            return VerifyOrganizationBucketResponseAllOfFiles.construct(**obj)
 
-        _obj = VerifyDspBlockUrlRequest.construct(**{
-            "url": obj.get("url")
+        _obj = VerifyOrganizationBucketResponseAllOfFiles.construct(**{
+            "name": obj.get("name"),
+            "size": obj.get("size"),
+            "folder_name": obj.get("folderName")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,57 +13,71 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel
-from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
-
-class VerifyDspBlockUrlResponseAllOf(BaseModel):
-    block: Optional[VerifyDspBlockUrlResponseAllOfBlock] = None
-    __properties = ["block"]
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+from edgeimpulse_api.models.dsp_named_axis import DSPNamedAxis
+
+class VerifyDspBlockUrlResponseAllOfBlock(BaseModel):
+    title: StrictStr = ...
+    author: StrictStr = ...
+    description: StrictStr = ...
+    name: StrictStr = ...
+    latest_implementation_version: StrictInt = Field(..., alias="latestImplementationVersion")
+    named_axes: Optional[List[DSPNamedAxis]] = Field(None, alias="namedAxes")
+    __properties = ["title", "author", "description", "name", "latestImplementationVersion", "namedAxes"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOf:
-        """Create an instance of VerifyDspBlockUrlResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOfBlock:
+        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of block
-        if self.block:
-            _dict['block'] = self.block.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in named_axes (list)
+        _items = []
+        if self.named_axes:
+            for _item in self.named_axes:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['namedAxes'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOf:
-        """Create an instance of VerifyDspBlockUrlResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOfBlock:
+        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyDspBlockUrlResponseAllOf.construct(**obj)
+            return VerifyDspBlockUrlResponseAllOfBlock.construct(**obj)
 
-        _obj = VerifyDspBlockUrlResponseAllOf.construct(**{
-            "block": VerifyDspBlockUrlResponseAllOfBlock.from_dict(obj.get("block")) if obj.get("block") is not None else None
+        _obj = VerifyDspBlockUrlResponseAllOfBlock.construct(**{
+            "title": obj.get("title"),
+            "author": obj.get("author"),
+            "description": obj.get("description"),
+            "name": obj.get("name"),
+            "latest_implementation_version": obj.get("latestImplementationVersion"),
+            "named_axes": [DSPNamedAxis.from_dict(_item) for _item in obj.get("namedAxes")] if obj.get("namedAxes") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_email_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,71 +13,61 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
-from edgeimpulse_api.models.dsp_named_axis import DSPNamedAxis
-
-class VerifyDspBlockUrlResponseAllOfBlock(BaseModel):
-    title: StrictStr = ...
-    author: StrictStr = ...
-    description: StrictStr = ...
-    name: StrictStr = ...
-    latest_implementation_version: StrictInt = Field(..., alias="latestImplementationVersion")
-    named_axes: Optional[List[DSPNamedAxis]] = Field(None, alias="namedAxes")
-    __properties = ["title", "author", "description", "name", "latestImplementationVersion", "namedAxes"]
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+
+class VerifyEmailResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
+    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
+    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
+    __properties = ["success", "error", "email", "userId", "redirectUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyDspBlockUrlResponseAllOfBlock:
-        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyEmailResponse:
+        """Create an instance of VerifyEmailResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in named_axes (list)
-        _items = []
-        if self.named_axes:
-            for _item in self.named_axes:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['namedAxes'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOfBlock:
-        """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyEmailResponse:
+        """Create an instance of VerifyEmailResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyDspBlockUrlResponseAllOfBlock.construct(**obj)
+            return VerifyEmailResponse.construct(**obj)
 
-        _obj = VerifyDspBlockUrlResponseAllOfBlock.construct(**{
-            "title": obj.get("title"),
-            "author": obj.get("author"),
-            "description": obj.get("description"),
-            "name": obj.get("name"),
-            "latest_implementation_version": obj.get("latestImplementationVersion"),
-            "named_axes": [DSPNamedAxis.from_dict(_item) for _item in obj.get("namedAxes")] if obj.get("namedAxes") is not None else None
+        _obj = VerifyEmailResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "email": obj.get("email"),
+            "user_id": obj.get("userId"),
+            "redirect_url": obj.get("redirectUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_email_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,61 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class VerifyEmailResponse(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
-    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
-    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
-    __properties = ["success", "error", "email", "userId", "redirectUrl"]
+from pydantic import BaseModel, Field, StrictStr
+
+class WhitelabelAllLearningBlocksInner(BaseModel):
+    title: StrictStr = Field(..., description="The name of the learning block")
+    type: StrictStr = Field(..., description="The learning block type")
+    __properties = ["title", "type"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyEmailResponse:
-        """Create an instance of VerifyEmailResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelabelAllLearningBlocksInner:
+        """Create an instance of WhitelabelAllLearningBlocksInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyEmailResponse:
-        """Create an instance of VerifyEmailResponse from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelabelAllLearningBlocksInner:
+        """Create an instance of WhitelabelAllLearningBlocksInner from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyEmailResponse.construct(**obj)
+            return WhitelabelAllLearningBlocksInner.construct(**obj)
 
-        _obj = VerifyEmailResponse.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
-            "email": obj.get("email"),
-            "user_id": obj.get("userId"),
-            "redirect_url": obj.get("redirectUrl")
+        _obj = WhitelabelAllLearningBlocksInner.construct(**{
+            "title": obj.get("title"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_email_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,54 +16,60 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class VerifyEmailResponseAllOf(BaseModel):
-    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
-    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
-    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
-    __properties = ["email", "userId", "redirectUrl"]
+class VerifyOrganizationBucketRequest(BaseModel):
+    access_key: StrictStr = Field(..., alias="accessKey", description="S3 access key")
+    secret_key: StrictStr = Field(..., alias="secretKey", description="S3 secret key")
+    bucket: StrictStr = Field(..., description="S3 bucket")
+    endpoint: StrictStr = Field(..., description="S3 endpoint")
+    region: StrictStr = Field(..., description="S3 region")
+    prefix: Optional[StrictStr] = Field(None, description="Optional prefix in the bucket. Set this if you don't have access to the full bucket for example.")
+    __properties = ["accessKey", "secretKey", "bucket", "endpoint", "region", "prefix"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyEmailResponseAllOf:
-        """Create an instance of VerifyEmailResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationBucketRequest:
+        """Create an instance of VerifyOrganizationBucketRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyEmailResponseAllOf:
-        """Create an instance of VerifyEmailResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketRequest:
+        """Create an instance of VerifyOrganizationBucketRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyEmailResponseAllOf.construct(**obj)
+            return VerifyOrganizationBucketRequest.construct(**obj)
 
-        _obj = VerifyEmailResponseAllOf.construct(**{
-            "email": obj.get("email"),
-            "user_id": obj.get("userId"),
-            "redirect_url": obj.get("redirectUrl")
+        _obj = VerifyOrganizationBucketRequest.construct(**{
+            "access_key": obj.get("accessKey"),
+            "secret_key": obj.get("secretKey"),
+            "bucket": obj.get("bucket"),
+            "endpoint": obj.get("endpoint"),
+            "region": obj.get("region"),
+            "prefix": obj.get("prefix")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_existing_bucket_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,63 +13,53 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
 
-class VerifyOrganizationBucketRequest(BaseModel):
-    access_key: StrictStr = Field(..., alias="accessKey", description="S3 access key")
-    secret_key: StrictStr = Field(..., alias="secretKey", description="S3 secret key")
-    bucket: StrictStr = Field(..., description="S3 bucket")
-    endpoint: StrictStr = Field(..., description="S3 endpoint")
-    region: StrictStr = Field(..., description="S3 region")
-    prefix: Optional[StrictStr] = Field(None, description="Optional prefix in the bucket. Set this if you don't have access to the full bucket for example.")
-    __properties = ["accessKey", "secretKey", "bucket", "endpoint", "region", "prefix"]
+from pydantic import BaseModel, StrictStr
+
+class VerifyOrganizationExistingBucketRequest(BaseModel):
+    prefix: StrictStr = ...
+    __properties = ["prefix"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationBucketRequest:
-        """Create an instance of VerifyOrganizationBucketRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationExistingBucketRequest:
+        """Create an instance of VerifyOrganizationExistingBucketRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketRequest:
-        """Create an instance of VerifyOrganizationBucketRequest from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationExistingBucketRequest:
+        """Create an instance of VerifyOrganizationExistingBucketRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationBucketRequest.construct(**obj)
+            return VerifyOrganizationExistingBucketRequest.construct(**obj)
 
-        _obj = VerifyOrganizationBucketRequest.construct(**{
-            "access_key": obj.get("accessKey"),
-            "secret_key": obj.get("secretKey"),
-            "bucket": obj.get("bucket"),
-            "endpoint": obj.get("endpoint"),
-            "region": obj.get("region"),
+        _obj = VerifyOrganizationExistingBucketRequest.construct(**{
             "prefix": obj.get("prefix")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,57 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class VerifyOrganizationBucketResponseAllOfFiles(BaseModel):
-    name: StrictStr = ...
-    size: StrictInt = ...
-    folder_name: StrictStr = Field(..., alias="folderName")
-    __properties = ["name", "size", "folderName"]
+class WhitelabelAdminCreateOrganizationRequest(BaseModel):
+    organization_name: StrictStr = Field(..., alias="organizationName", description="The name of the organization.")
+    admin_id: Optional[StrictInt] = Field(None, alias="adminId", description="Unique identifier of the administrator of the new organization.")
+    admin_email: Optional[StrictStr] = Field(None, alias="adminEmail", description="Email of the administrator of the new organization.")
+    __properties = ["organizationName", "adminId", "adminEmail"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOfFiles:
-        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelabelAdminCreateOrganizationRequest:
+        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOfFiles:
-        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelabelAdminCreateOrganizationRequest:
+        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationBucketResponseAllOfFiles.construct(**obj)
+            return WhitelabelAdminCreateOrganizationRequest.construct(**obj)
 
-        _obj = VerifyOrganizationBucketResponseAllOfFiles.construct(**{
-            "name": obj.get("name"),
-            "size": obj.get("size"),
-            "folder_name": obj.get("folderName")
+        _obj = WhitelabelAdminCreateOrganizationRequest.construct(**{
+            "organization_name": obj.get("organizationName"),
+            "admin_id": obj.get("adminId"),
+            "admin_email": obj.get("adminEmail")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/verify_organization_existing_bucket_request.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/window_settings_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,53 +13,65 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
-from pydantic import BaseModel, StrictStr
-
-class VerifyOrganizationExistingBucketRequest(BaseModel):
-    prefix: StrictStr = ...
-    __properties = ["prefix"]
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+from edgeimpulse_api.models.window_settings_response_all_of_window_settings import WindowSettingsResponseAllOfWindowSettings
+
+class WindowSettingsResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    window_settings: List[WindowSettingsResponseAllOfWindowSettings] = Field(..., alias="windowSettings")
+    __properties = ["success", "error", "windowSettings"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationExistingBucketRequest:
-        """Create an instance of VerifyOrganizationExistingBucketRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> WindowSettingsResponse:
+        """Create an instance of WindowSettingsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in window_settings (list)
+        _items = []
+        if self.window_settings:
+            for _item in self.window_settings:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['windowSettings'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationExistingBucketRequest:
-        """Create an instance of VerifyOrganizationExistingBucketRequest from a dict"""
+    def from_dict(cls, obj: dict) -> WindowSettingsResponse:
+        """Create an instance of WindowSettingsResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationExistingBucketRequest.construct(**obj)
+            return WindowSettingsResponse.construct(**obj)
 
-        _obj = VerifyOrganizationExistingBucketRequest.construct(**{
-            "prefix": obj.get("prefix")
+        _obj = WindowSettingsResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "window_settings": [WindowSettingsResponseAllOfWindowSettings.from_dict(_item) for _item in obj.get("windowSettings")] if obj.get("windowSettings") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,52 +16,52 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr
 
-class WhitelabelAllLearningBlocksInner(BaseModel):
-    title: StrictStr = Field(..., description="The name of the learning block")
-    type: StrictStr = Field(..., description="The learning block type")
-    __properties = ["title", "type"]
+class WhitelabelCustomDeploymentBlocksInner(BaseModel):
+    name: StrictStr = Field(..., description="The name of the custom deployment block")
+    id: float = Field(..., description="The custom deployment block ID")
+    __properties = ["name", "id"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WhitelabelAllLearningBlocksInner:
-        """Create an instance of WhitelabelAllLearningBlocksInner from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelabelCustomDeploymentBlocksInner:
+        """Create an instance of WhitelabelCustomDeploymentBlocksInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WhitelabelAllLearningBlocksInner:
-        """Create an instance of WhitelabelAllLearningBlocksInner from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelabelCustomDeploymentBlocksInner:
+        """Create an instance of WhitelabelCustomDeploymentBlocksInner from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return WhitelabelAllLearningBlocksInner.construct(**obj)
+            return WhitelabelCustomDeploymentBlocksInner.construct(**obj)
 
-        _obj = WhitelabelAllLearningBlocksInner.construct(**{
-            "title": obj.get("title"),
-            "type": obj.get("type")
+        _obj = WhitelabelCustomDeploymentBlocksInner.construct(**{
+            "name": obj.get("name"),
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,65 +13,65 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
-from edgeimpulse_api.models.window_settings_response_all_of_window_settings import WindowSettingsResponseAllOfWindowSettings
-
-class WindowSettingsResponse(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    window_settings: List[WindowSettingsResponseAllOfWindowSettings] = Field(..., alias="windowSettings")
-    __properties = ["success", "error", "windowSettings"]
+
+from pydantic import BaseModel, Field, StrictBool, StrictInt
+
+class WindowSettingsResponseAllOfWindowSettings(BaseModel):
+    window_size_ms: float = Field(..., alias="windowSizeMs")
+    window_increase_ms: float = Field(..., alias="windowIncreaseMs")
+    window_increase_pct: float = Field(..., alias="windowIncreasePct")
+    zero_pad_percentage: float = Field(..., alias="zeroPadPercentage")
+    window_count: StrictInt = Field(..., alias="windowCount")
+    balance_score: float = Field(..., alias="balanceScore")
+    valid: StrictBool = ...
+    __properties = ["windowSizeMs", "windowIncreaseMs", "windowIncreasePct", "zeroPadPercentage", "windowCount", "balanceScore", "valid"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WindowSettingsResponse:
-        """Create an instance of WindowSettingsResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> WindowSettingsResponseAllOfWindowSettings:
+        """Create an instance of WindowSettingsResponseAllOfWindowSettings from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in window_settings (list)
-        _items = []
-        if self.window_settings:
-            for _item in self.window_settings:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['windowSettings'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WindowSettingsResponse:
-        """Create an instance of WindowSettingsResponse from a dict"""
+    def from_dict(cls, obj: dict) -> WindowSettingsResponseAllOfWindowSettings:
+        """Create an instance of WindowSettingsResponseAllOfWindowSettings from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return WindowSettingsResponse.construct(**obj)
+            return WindowSettingsResponseAllOfWindowSettings.construct(**obj)
 
-        _obj = WindowSettingsResponse.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
-            "window_settings": [WindowSettingsResponseAllOfWindowSettings.from_dict(_item) for _item in obj.get("windowSettings")] if obj.get("windowSettings") is not None else None
+        _obj = WindowSettingsResponseAllOfWindowSettings.construct(**{
+            "window_size_ms": obj.get("windowSizeMs"),
+            "window_increase_ms": obj.get("windowIncreaseMs"),
+            "window_increase_pct": obj.get("windowIncreasePct"),
+            "zero_pad_percentage": obj.get("zeroPadPercentage"),
+            "window_count": obj.get("windowCount"),
+            "balance_score": obj.get("balanceScore"),
+            "valid": obj.get("valid")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.50.6/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.50.15/pyproject.toml` & `edgeimpulse_api-1.50.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.50.15" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.50.6" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `edgeimpulse_api-1.50.15/PKG-INFO` & `edgeimpulse_api-1.50.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.50.15
+Version: 1.50.6
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

