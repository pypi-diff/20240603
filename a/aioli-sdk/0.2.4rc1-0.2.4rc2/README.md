# Comparing `tmp/aioli_sdk-0.2.4rc1.tar.gz` & `tmp/aioli_sdk-0.2.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli_sdk-0.2.4rc1.tar", last modified: Fri May 31 07:14:22 2024, max compression
+gzip compressed data, was "aioli_sdk-0.2.4rc2.tar", last modified: Mon Jun  3 07:13:05 2024, max compression
```

## Comparing `aioli_sdk-0.2.4rc1.tar` & `aioli_sdk-0.2.4rc2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.775475 aioli_sdk-0.2.4rc1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-05-31 07:14:22.775475 aioli_sdk-0.2.4rc1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.767475 aioli_sdk-0.2.4rc1/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.767475 aioli_sdk-0.2.4rc1/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8466 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14634 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13780 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.767475 aioli_sdk-0.2.4rc1/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30332 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3168 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.767475 aioli_sdk-0.2.4rc1/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.767475 aioli_sdk-0.2.4rc1/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.775475 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-05-31 07:14:22.000000 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-31 07:14:22.000000 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-31 07:14:22.000000 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-31 07:14:22.000000 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-31 07:14:20.000000 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-31 07:14:22.000000 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-31 07:14:22.000000 aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.771475 aioli_sdk-0.2.4rc1/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3217 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.771475 aioli_sdk-0.2.4rc1/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22812 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84658 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10514 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92236 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    66585 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43081 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105943 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61884 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25049 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14924 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5596 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:22.771475 aioli_sdk-0.2.4rc1/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2279 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3383 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3985 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3661 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7355 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5067 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5177 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2787 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3774 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2641 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2535 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4129 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/model_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6262 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5739 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2939 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3365 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2835 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3295 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2648 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5550 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5293 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3931 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3386 2024-05-31 07:14:18.000000 aioli_sdk-0.2.4rc1/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8439 2024-05-31 07:14:19.000000 aioli_sdk-0.2.4rc1/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-31 07:14:22.775475 aioli_sdk-0.2.4rc1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-05-31 07:08:58.000000 aioli_sdk-0.2.4rc1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.580336 aioli_sdk-0.2.4rc2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-06-03 07:13:05.580336 aioli_sdk-0.2.4rc2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.572337 aioli_sdk-0.2.4rc2/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.572337 aioli_sdk-0.2.4rc2/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1597 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8466 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14634 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13780 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.572337 aioli_sdk-0.2.4rc2/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30332 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3168 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.572337 aioli_sdk-0.2.4rc2/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.572337 aioli_sdk-0.2.4rc2/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.580336 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-06-03 07:13:05.000000 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-06-03 07:13:05.000000 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-06-03 07:13:05.000000 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-06-03 07:13:05.000000 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-06-03 07:13:03.000000 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-06-03 07:13:05.000000 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-06-03 07:13:05.000000 aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.576336 aioli_sdk-0.2.4rc2/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3217 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.576336 aioli_sdk-0.2.4rc2/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22812 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    86560 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10514 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92236 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    66585 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43081 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105943 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61884 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25049 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14924 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5596 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:05.580336 aioli_sdk-0.2.4rc2/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2279 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3383 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3985 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3661 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7785 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5067 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5177 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2787 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3774 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2641 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2535 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4129 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/model_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6262 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5739 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2939 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3365 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2835 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3295 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2648 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5550 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5293 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3931 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3386 2024-06-03 07:13:01.000000 aioli_sdk-0.2.4rc2/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8439 2024-06-03 07:13:02.000000 aioli_sdk-0.2.4rc2/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-06-03 07:13:05.580336 aioli_sdk-0.2.4rc2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-06-03 07:07:49.000000 aioli_sdk-0.2.4rc2/setup.py
```

### Comparing `aioli_sdk-0.2.4rc1/PKG-INFO` & `aioli_sdk-0.2.4rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4rc1
+Version: 0.2.4rc2
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/_util.py` & `aioli_sdk-0.2.4rc2/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/cli.py` & `aioli_sdk-0.2.4rc2/aioli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/deployment.py` & `aioli_sdk-0.2.4rc2/aioli/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/errors.py` & `aioli_sdk-0.2.4rc2/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/model.py` & `aioli_sdk-0.2.4rc2/aioli/cli/model.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/registry.py` & `aioli_sdk-0.2.4rc2/aioli/cli/registry.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/render.py` & `aioli_sdk-0.2.4rc2/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/role.py` & `aioli_sdk-0.2.4rc2/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/sso.py` & `aioli_sdk-0.2.4rc2/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/test/conftest.py` & `aioli_sdk-0.2.4rc2/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/test/test_cli.py` & `aioli_sdk-0.2.4rc2/aioli/cli/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/user.py` & `aioli_sdk-0.2.4rc2/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/cli/version.py` & `aioli_sdk-0.2.4rc2/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/api/authentication.py` & `aioli_sdk-0.2.4rc2/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/api/certs.py` & `aioli_sdk-0.2.4rc2/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/api/errors.py` & `aioli_sdk-0.2.4rc2/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/api/request.py` & `aioli_sdk-0.2.4rc2/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/check.py` & `aioli_sdk-0.2.4rc2/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/constants.py` & `aioli_sdk-0.2.4rc2/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/declarative_argparse.py` & `aioli_sdk-0.2.4rc2/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/requests.py` & `aioli_sdk-0.2.4rc2/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/common/util.py` & `aioli_sdk-0.2.4rc2/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli/util.py` & `aioli_sdk-0.2.4rc2/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/PKG-INFO` & `aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4rc1
+Version: 0.2.4rc2
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4rc1/aioli_sdk.egg-info/SOURCES.txt` & `aioli_sdk-0.2.4rc2/aioli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/__init__.py` & `aioli_sdk-0.2.4rc2/aiolirest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/authentication_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/deployments_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/deployments_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -53,14 +53,15 @@
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
     def deployments_get(
         self,
+        last_event: Annotated[Optional[StrictStr], Field(description="Include the most recent event for each deployment.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -70,14 +71,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[Deployment]:
         """Get all deployments.
 
         Return the properties of all configured deployments.
 
+        :param last_event: Include the most recent event for each deployment.
+        :type last_event: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -93,14 +96,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._deployments_get_serialize(
+            last_event=last_event,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -118,14 +122,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def deployments_get_with_http_info(
         self,
+        last_event: Annotated[Optional[StrictStr], Field(description="Include the most recent event for each deployment.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -135,14 +140,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[Deployment]]:
         """Get all deployments.
 
         Return the properties of all configured deployments.
 
+        :param last_event: Include the most recent event for each deployment.
+        :type last_event: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -158,14 +165,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._deployments_get_serialize(
+            last_event=last_event,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -183,14 +191,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def deployments_get_without_preload_content(
         self,
+        last_event: Annotated[Optional[StrictStr], Field(description="Include the most recent event for each deployment.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -200,14 +209,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get all deployments.
 
         Return the properties of all configured deployments.
 
+        :param last_event: Include the most recent event for each deployment.
+        :type last_event: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -223,14 +234,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._deployments_get_serialize(
+            last_event=last_event,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -243,14 +255,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _deployments_get_serialize(
         self,
+        last_event,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -264,14 +277,18 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if last_event is not None:
+            
+            _query_params.append(('lastEvent', last_event))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -572,14 +589,15 @@
 
 
 
     @validate_call
     def deployments_id_events_get(
         self,
         id: Annotated[StrictStr, Field(description="Deployment ID")],
+        last_event: Annotated[Optional[StrictStr], Field(description="Limit resposne to only the most recent event.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -587,18 +605,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[EventInfo]:
         """Get recent, significant events related to the service progressing towards the next status.
 
-        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most-recent to oldest.
+        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most recent to oldest.
 
         :param id: Deployment ID (required)
         :type id: str
+        :param last_event: Limit resposne to only the most recent event.
+        :type last_event: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -615,14 +635,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._deployments_id_events_get_serialize(
             id=id,
+            last_event=last_event,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -642,14 +663,15 @@
         ).data
 
 
     @validate_call
     def deployments_id_events_get_with_http_info(
         self,
         id: Annotated[StrictStr, Field(description="Deployment ID")],
+        last_event: Annotated[Optional[StrictStr], Field(description="Limit resposne to only the most recent event.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -657,18 +679,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[EventInfo]]:
         """Get recent, significant events related to the service progressing towards the next status.
 
-        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most-recent to oldest.
+        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most recent to oldest.
 
         :param id: Deployment ID (required)
         :type id: str
+        :param last_event: Limit resposne to only the most recent event.
+        :type last_event: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -685,14 +709,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._deployments_id_events_get_serialize(
             id=id,
+            last_event=last_event,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -712,14 +737,15 @@
         )
 
 
     @validate_call
     def deployments_id_events_get_without_preload_content(
         self,
         id: Annotated[StrictStr, Field(description="Deployment ID")],
+        last_event: Annotated[Optional[StrictStr], Field(description="Limit resposne to only the most recent event.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -727,18 +753,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get recent, significant events related to the service progressing towards the next status.
 
-        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most-recent to oldest.
+        Returns recent, significant events related to the service progressing towards the next status. The events returned are ordered from most recent to oldest.
 
         :param id: Deployment ID (required)
         :type id: str
+        :param last_event: Limit resposne to only the most recent event.
+        :type last_event: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -755,14 +783,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._deployments_id_events_get_serialize(
             id=id,
+            last_event=last_event,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -777,14 +806,15 @@
         )
         return response_data.response
 
 
     def _deployments_id_events_get_serialize(
         self,
         id,
+        last_event,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -800,14 +830,18 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
+        if last_event is not None:
+            
+            _query_params.append(('lastEvent', last_event))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/information_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/packaged_models_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/packaged_models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/registries_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/registries_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/roles_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/templates_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api/users_api.py` & `aioli_sdk-0.2.4rc2/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api_client.py` & `aioli_sdk-0.2.4rc2/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/api_response.py` & `aioli_sdk-0.2.4rc2/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/configuration.py` & `aioli_sdk-0.2.4rc2/aiolirest/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.2.4-rc1\n"\
+               "Version of the API: 0.2.4-rc2\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/exceptions.py` & `aioli_sdk-0.2.4rc2/aiolirest/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/__init__.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/auto_scaling_template.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/auto_scaling_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/autoscaling.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/autoscaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/configuration_resources.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/configuration_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/deployment.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/deployment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,14 +20,15 @@
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
 from aiolirest.models.autoscaling import Autoscaling
 from aiolirest.models.deployment_state import DeploymentState
+from aiolirest.models.event_info import EventInfo
 from aiolirest.models.security import Security
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class Deployment(BaseModel):
@@ -37,23 +38,24 @@
     arguments: Optional[List[StrictStr]] = Field(default=None, description="Arguments to be added to the service command line")
     auto_scaling: Optional[Autoscaling] = Field(default=None, alias="autoScaling")
     canary_traffic_percent: Optional[StrictInt] = Field(default=None, description="Percent traffic to pass to new model version", alias="canaryTrafficPercent")
     cluster_name: Optional[StrictStr] = Field(default=None, description="Name of the cluster.", alias="clusterName")
     environment: Optional[Dict[str, StrictStr]] = Field(default=None, description="Environment variables added to the service")
     goal_status: Optional[StrictStr] = Field(default='Ready', description="Specifies the intended status to be achieved by the deployment.  Supported values are: * `Ready` - The inference serivce will be deployed to enable inference calls. * `Paused` - The inference serivce will be stopped and no longer accept calls.  The default is `Ready`.", alias="goalStatus")
     id: Optional[StrictStr] = Field(default=None, description="The ID of the deployment. This is a read-only property and is automatically assigned on creation.")
+    last_event: Optional[EventInfo] = Field(default=None, alias="lastEvent")
     model: StrictStr = Field(description="PackagedModel name or ID to be deployed.")
     modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the deployment. This is a read-only field and is automatically updated.", alias="modifiedAt")
     name: StrictStr = Field(description="The deployment name.  It must be a valid subdomain name and consist of lower case alphanumeric characters, '-' or '.', and must start and end with an alphanumeric character.")
     namespace: Optional[StrictStr] = Field(default=None, description="The Kubernetes namespace to be used for the deployment.")
     secondary_state: Optional[DeploymentState] = Field(default=None, alias="secondaryState")
     security: Optional[Security] = None
     state: Optional[DeploymentState] = None
     status: Optional[StrictStr] = Field(default=None, description="Summary status of the deployed service. * `Deploying` - Service configuration is in progress. * `Failed` - The service configuration failed. * `Ready` - The service has been successfully configured and is serving. * `Updating` - A new service revision is being rolledout. * `UpdateFailed` - The current service revision failed to rollout due to an error.   The prior version is still serving requests. * `Deleting` - The deployed service is being removed. * `Paused` - The deployed service has been stopped by the user or an external action. * `Unknown` - Unable to determined the status.  This is a read-only property. Must be one of the values: (Deploying,Ready,Updating,UpdateFailed,Failed,Deleting,Paused,Unknown).")
-    __properties: ClassVar[List[str]] = ["arguments", "autoScaling", "canaryTrafficPercent", "clusterName", "environment", "goalStatus", "id", "model", "modifiedAt", "name", "namespace", "secondaryState", "security", "state", "status"]
+    __properties: ClassVar[List[str]] = ["arguments", "autoScaling", "canaryTrafficPercent", "clusterName", "environment", "goalStatus", "id", "lastEvent", "model", "modifiedAt", "name", "namespace", "secondaryState", "security", "state", "status"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -86,14 +88,17 @@
             exclude={
             },
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of auto_scaling
         if self.auto_scaling:
             _dict['autoScaling'] = self.auto_scaling.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of last_event
+        if self.last_event:
+            _dict['lastEvent'] = self.last_event.to_dict()
         # override the default output from pydantic by calling `to_dict()` of secondary_state
         if self.secondary_state:
             _dict['secondaryState'] = self.secondary_state.to_dict()
         # override the default output from pydantic by calling `to_dict()` of security
         if self.security:
             _dict['security'] = self.security.to_dict()
         # override the default output from pydantic by calling `to_dict()` of state
@@ -114,14 +119,15 @@
             "arguments": obj.get("arguments"),
             "autoScaling": Autoscaling.from_dict(obj.get("autoScaling")) if obj.get("autoScaling") is not None else None,
             "canaryTrafficPercent": obj.get("canaryTrafficPercent"),
             "clusterName": obj.get("clusterName"),
             "environment": obj.get("environment"),
             "goalStatus": obj.get("goalStatus") if obj.get("goalStatus") is not None else 'Ready',
             "id": obj.get("id"),
+            "lastEvent": EventInfo.from_dict(obj.get("lastEvent")) if obj.get("lastEvent") is not None else None,
             "model": obj.get("model"),
             "modifiedAt": obj.get("modifiedAt"),
             "name": obj.get("name"),
             "namespace": obj.get("namespace"),
             "secondaryState": DeploymentState.from_dict(obj.get("secondaryState")) if obj.get("secondaryState") is not None else None,
             "security": Security.from_dict(obj.get("security")) if obj.get("security") is not None else None,
             "state": DeploymentState.from_dict(obj.get("state")) if obj.get("state") is not None else None,
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/deployment_model_version.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/deployment_model_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/deployment_request.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/deployment_state.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/deployment_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/error_response.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/event_info.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/event_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/failure_info.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/failure_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/login_request.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/login_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/login_response.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/model_auth_token.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/model_auth_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/model_response.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/observability.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/observability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/packaged_model.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/packaged_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/packaged_model_request.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/packaged_model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/resource_profile.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/resource_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/resources_template.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/resources_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/role.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/role_assignment.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/role_assignments.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/role_assignments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/security.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/security.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/success_response.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/success_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/trained_model_registry.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/trained_model_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/trained_model_registry_request.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/trained_model_registry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/user.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/user_patch_request.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/user_patch_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/models/user_request.py` & `aioli_sdk-0.2.4rc2/aiolirest/models/user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/aiolirest/rest.py` & `aioli_sdk-0.2.4rc2/aiolirest/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-rc1
+    The version of the OpenAPI document: 0.2.4-rc2
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4rc1/setup.py` & `aioli_sdk-0.2.4rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.4-rc1",
+    version="0.2.4-rc2",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

