# Comparing `tmp/alibabacloud_cloudsso20210515-1.5.2.tar.gz` & `tmp/alibabacloud_cloudsso20210515-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudsso20210515-1.5.2.tar", last modified: Thu Apr 25 02:36:39 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cloudsso20210515-1.6.0.tar", last modified: Mon Jun  3 09:17:01 2024, max compression
```

## Comparing `alibabacloud_cloudsso20210515-1.5.2.tar` & `alibabacloud_cloudsso20210515-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/
--rw-r--r--   0 root         (0) root         (0)      928 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   398446 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515/client.py
--rw-r--r--   0 root         (0) root         (0)   552763 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-04-25 02:36:39.000000 alibabacloud_cloudsso20210515-1.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/
+-rw-r--r--   0 root         (0) root         (0)      999 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   451632 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515/client.py
+-rw-r--r--   0 root         (0) root         (0)   559685 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-06-03 09:17:01.000000 alibabacloud_cloudsso20210515-1.6.0/setup.py
```

### Comparing `alibabacloud_cloudsso20210515-1.5.2/ChangeLog.md` & `alibabacloud_cloudsso20210515-1.6.0/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-25 Version: 1.5.2
+- Generated python 2021-05-15 for cloudsso.
+
 2024-04-22 Version: 1.5.1
 - Update API GetDirectoryStatistics: update response param.
 
 
 2024-03-29 Version: 1.5.0
 - Support API GetLoginPreference.
 - Support API GetPasswordPolicy.
```

### Comparing `alibabacloud_cloudsso20210515-1.5.2/LICENSE` & `alibabacloud_cloudsso20210515-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515-1.5.2/PKG-INFO` & `alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_cloudsso20210515
-Version: 1.5.2
+Name: alibabacloud-cloudsso20210515
+Version: 1.6.0
 Summary: Alibaba Cloud cloudsso (20210515) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudsso20210515-1.5.2/README-CN.md` & `alibabacloud_cloudsso20210515-1.6.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515-1.5.2/README.md` & `alibabacloud_cloudsso20210515-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515/client.py` & `alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 
     def add_external_samlid_pcertificate_with_options(
         self,
         request: cloudsso_20210515_models.AddExternalSAMLIdPCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.AddExternalSAMLIdPCertificateResponse:
         """
-        You can add up to two SAML signing certificates.
-        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61****`.
+        @summary Adds a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description You can add up to two SAML signing certificates.
+        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61***`.
         
         @param request: AddExternalSAMLIdPCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddExternalSAMLIdPCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -81,16 +83,18 @@
 
     async def add_external_samlid_pcertificate_with_options_async(
         self,
         request: cloudsso_20210515_models.AddExternalSAMLIdPCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.AddExternalSAMLIdPCertificateResponse:
         """
-        You can add up to two SAML signing certificates.
-        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61****`.
+        @summary Adds a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description You can add up to two SAML signing certificates.
+        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61***`.
         
         @param request: AddExternalSAMLIdPCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddExternalSAMLIdPCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -118,44 +122,50 @@
         )
 
     def add_external_samlid_pcertificate(
         self,
         request: cloudsso_20210515_models.AddExternalSAMLIdPCertificateRequest,
     ) -> cloudsso_20210515_models.AddExternalSAMLIdPCertificateResponse:
         """
-        You can add up to two SAML signing certificates.
-        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61****`.
+        @summary Adds a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description You can add up to two SAML signing certificates.
+        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61***`.
         
         @param request: AddExternalSAMLIdPCertificateRequest
         @return: AddExternalSAMLIdPCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.add_external_samlid_pcertificate_with_options(request, runtime)
 
     async def add_external_samlid_pcertificate_async(
         self,
         request: cloudsso_20210515_models.AddExternalSAMLIdPCertificateRequest,
     ) -> cloudsso_20210515_models.AddExternalSAMLIdPCertificateResponse:
         """
-        You can add up to two SAML signing certificates.
-        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61****`.
+        @summary Adds a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description You can add up to two SAML signing certificates.
+        This topic provides an example on how to add a SAML signing certificate to the directory `d-00fc2p61***`.
         
         @param request: AddExternalSAMLIdPCertificateRequest
         @return: AddExternalSAMLIdPCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.add_external_samlid_pcertificate_with_options_async(request, runtime)
 
     def add_permission_policy_to_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationResponse:
         """
-        This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Adds a policy to an access configuration.
+        
+        @description This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: AddPermissionPolicyToAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddPermissionPolicyToAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -190,15 +200,17 @@
 
     async def add_permission_policy_to_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationResponse:
         """
-        This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Adds a policy to an access configuration.
+        
+        @description This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: AddPermissionPolicyToAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddPermissionPolicyToAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -232,43 +244,49 @@
         )
 
     def add_permission_policy_to_access_configuration(
         self,
         request: cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationResponse:
         """
-        This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Adds a policy to an access configuration.
+        
+        @description This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: AddPermissionPolicyToAccessConfigurationRequest
         @return: AddPermissionPolicyToAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.add_permission_policy_to_access_configuration_with_options(request, runtime)
 
     async def add_permission_policy_to_access_configuration_async(
         self,
         request: cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.AddPermissionPolicyToAccessConfigurationResponse:
         """
-        This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Adds a policy to an access configuration.
+        
+        @description This topic provides an example on how to add the system policy `AliyunECSFullAccess` to the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: AddPermissionPolicyToAccessConfigurationRequest
         @return: AddPermissionPolicyToAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.add_permission_policy_to_access_configuration_with_options_async(request, runtime)
 
     def add_user_to_group_with_options(
         self,
         request: cloudsso_20210515_models.AddUserToGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.AddUserToGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
-        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk****` to the group `g-00jqzghi2n3o5hkh****`.
+        @summary Adds a user to a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
+        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk***` to the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: AddUserToGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddUserToGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -299,16 +317,18 @@
 
     async def add_user_to_group_with_options_async(
         self,
         request: cloudsso_20210515_models.AddUserToGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.AddUserToGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
-        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk****` to the group `g-00jqzghi2n3o5hkh****`.
+        @summary Adds a user to a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
+        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk***` to the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: AddUserToGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AddUserToGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -338,45 +358,51 @@
         )
 
     def add_user_to_group(
         self,
         request: cloudsso_20210515_models.AddUserToGroupRequest,
     ) -> cloudsso_20210515_models.AddUserToGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
-        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk****` to the group `g-00jqzghi2n3o5hkh****`.
+        @summary Adds a user to a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
+        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk***` to the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: AddUserToGroupRequest
         @return: AddUserToGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.add_user_to_group_with_options(request, runtime)
 
     async def add_user_to_group_async(
         self,
         request: cloudsso_20210515_models.AddUserToGroupRequest,
     ) -> cloudsso_20210515_models.AddUserToGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
-        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk****` to the group `g-00jqzghi2n3o5hkh****`.
+        @summary Adds a user to a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot add a user to a group that is synchronized by using SCIM.
+        This topic provides an example of how to add the user `u-00q8wbq42wiltcrk***` to the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: AddUserToGroupRequest
         @return: AddUserToGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.add_user_to_group_with_options_async(request, runtime)
 
     def clear_external_samlidentity_provider_with_options(
         self,
         request: cloudsso_20210515_models.ClearExternalSAMLIdentityProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ClearExternalSAMLIdentityProviderResponse:
         """
-        If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
-        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61****`.
+        @summary Clears the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
+        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: ClearExternalSAMLIdentityProviderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ClearExternalSAMLIdentityProviderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -403,16 +429,18 @@
 
     async def clear_external_samlidentity_provider_with_options_async(
         self,
         request: cloudsso_20210515_models.ClearExternalSAMLIdentityProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ClearExternalSAMLIdentityProviderResponse:
         """
-        If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
-        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61****`.
+        @summary Clears the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
+        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: ClearExternalSAMLIdentityProviderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ClearExternalSAMLIdentityProviderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -438,46 +466,52 @@
         )
 
     def clear_external_samlidentity_provider(
         self,
         request: cloudsso_20210515_models.ClearExternalSAMLIdentityProviderRequest,
     ) -> cloudsso_20210515_models.ClearExternalSAMLIdentityProviderResponse:
         """
-        If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
-        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61****`.
+        @summary Clears the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
+        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: ClearExternalSAMLIdentityProviderRequest
         @return: ClearExternalSAMLIdentityProviderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.clear_external_samlidentity_provider_with_options(request, runtime)
 
     async def clear_external_samlidentity_provider_async(
         self,
         request: cloudsso_20210515_models.ClearExternalSAMLIdentityProviderRequest,
     ) -> cloudsso_20210515_models.ClearExternalSAMLIdentityProviderResponse:
         """
-        If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
-        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61****`.
+        @summary Clears the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description If single sign-on (SSO) logon is disabled, you can clear the configurations of a SAML IdP. If SSO logon is enabled, you cannot clear the configurations.
+        This topic provides an example on how to clear the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: ClearExternalSAMLIdentityProviderRequest
         @return: ClearExternalSAMLIdentityProviderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.clear_external_samlidentity_provider_with_options_async(request, runtime)
 
     def create_access_assignment_with_options(
         self,
         request: cloudsso_20210515_models.CreateAccessAssignmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](~~266726~~).
-        This topic provides an example on how to assign access permissions on the account `114240524784****` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
+        @summary Assigns access permissions on an account in your resource directory to a user or a group by using an access configuration.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](https://help.aliyun.com/document_detail/266726.html).
+        This topic provides an example on how to assign access permissions on the account `114240524784***` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
         
         @param request: CreateAccessAssignmentRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAccessAssignmentResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -514,17 +548,19 @@
 
     async def create_access_assignment_with_options_async(
         self,
         request: cloudsso_20210515_models.CreateAccessAssignmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](~~266726~~).
-        This topic provides an example on how to assign access permissions on the account `114240524784****` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
+        @summary Assigns access permissions on an account in your resource directory to a user or a group by using an access configuration.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](https://help.aliyun.com/document_detail/266726.html).
+        This topic provides an example on how to assign access permissions on the account `114240524784***` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
         
         @param request: CreateAccessAssignmentRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAccessAssignmentResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -560,46 +596,52 @@
         )
 
     def create_access_assignment(
         self,
         request: cloudsso_20210515_models.CreateAccessAssignmentRequest,
     ) -> cloudsso_20210515_models.CreateAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](~~266726~~).
-        This topic provides an example on how to assign access permissions on the account `114240524784****` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
+        @summary Assigns access permissions on an account in your resource directory to a user or a group by using an access configuration.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](https://help.aliyun.com/document_detail/266726.html).
+        This topic provides an example on how to assign access permissions on the account `114240524784***` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
         
         @param request: CreateAccessAssignmentRequest
         @return: CreateAccessAssignmentResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_access_assignment_with_options(request, runtime)
 
     async def create_access_assignment_async(
         self,
         request: cloudsso_20210515_models.CreateAccessAssignmentRequest,
     ) -> cloudsso_20210515_models.CreateAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](~~266726~~).
-        This topic provides an example on how to assign access permissions on the account `114240524784****` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
+        @summary Assigns access permissions on an account in your resource directory to a user or a group by using an access configuration.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        For more information about how to assign permissions on an account in your resource directory, see [Overview of multi-account authorization](https://help.aliyun.com/document_detail/266726.html).
+        This topic provides an example on how to assign access permissions on the account `114240524784***` in your resource directory to the CloudSSO user `u-00q8wbq42wiltcrk****` by using the access configuration `ac-00jhtfl8thteu6uj****`. After the call is successful, the CloudSSO user can access resources within the account in the resource directory.
         
         @param request: CreateAccessAssignmentRequest
         @return: CreateAccessAssignmentResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_access_assignment_with_options_async(request, runtime)
 
     def create_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.CreateAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateAccessConfigurationResponse:
         """
-        For more information about access configurations, see [Overview of access configurations](~~266737~~).
+        @summary Creates an access configuration.
+        
+        @description For more information about access configurations, see [Overview of access configurations](https://help.aliyun.com/document_detail/266737.html).
         This topic provides an example on how to create an access configuration named `ECS-Admin`.
         
         @param request: CreateAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
@@ -635,15 +677,17 @@
 
     async def create_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.CreateAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateAccessConfigurationResponse:
         """
-        For more information about access configurations, see [Overview of access configurations](~~266737~~).
+        @summary Creates an access configuration.
+        
+        @description For more information about access configurations, see [Overview of access configurations](https://help.aliyun.com/document_detail/266737.html).
         This topic provides an example on how to create an access configuration named `ECS-Admin`.
         
         @param request: CreateAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
@@ -678,44 +722,50 @@
         )
 
     def create_access_configuration(
         self,
         request: cloudsso_20210515_models.CreateAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.CreateAccessConfigurationResponse:
         """
-        For more information about access configurations, see [Overview of access configurations](~~266737~~).
+        @summary Creates an access configuration.
+        
+        @description For more information about access configurations, see [Overview of access configurations](https://help.aliyun.com/document_detail/266737.html).
         This topic provides an example on how to create an access configuration named `ECS-Admin`.
         
         @param request: CreateAccessConfigurationRequest
         @return: CreateAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_access_configuration_with_options(request, runtime)
 
     async def create_access_configuration_async(
         self,
         request: cloudsso_20210515_models.CreateAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.CreateAccessConfigurationResponse:
         """
-        For more information about access configurations, see [Overview of access configurations](~~266737~~).
+        @summary Creates an access configuration.
+        
+        @description For more information about access configurations, see [Overview of access configurations](https://help.aliyun.com/document_detail/266737.html).
         This topic provides an example on how to create an access configuration named `ECS-Admin`.
         
         @param request: CreateAccessConfigurationRequest
         @return: CreateAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_access_configuration_with_options_async(request, runtime)
 
     def create_directory_with_options(
         self,
         request: cloudsso_20210515_models.CreateDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateDirectoryResponse:
         """
-        A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
+        @summary Creates a directory.
+        
+        @description A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
         To create a directory, you must select a region. Alibaba Cloud stores data in the directory only in the region that you select. However, you can deploy Alibaba Cloud resources including Elastic Compute Service (ECS) instances and ApsaraDB RDS instances in other regions. You can also use your cloud account for logons and access the Alibaba Cloud resources in other regions. You can select a region to create a directory based on your security compliance requirements and the geographic location of specific users. If you do not have strict security compliance requirements, we recommend that you select a region that is the closest to the geographical location of the specific users. This way, access to cloud resources is accelerated. You can create the CloudSSO directory in the China (Shanghai), China (Hong Kong), US (Silicon Valley), or Germany (Frankfurt) region.
         This topic provides an example on how to create a directory named `example` in the China (Shanghai) region.
         ## Limits
         - You can create only one directory for a management account.
         - If you want to change the region of a directory, you must delete the directory and then create a directory in a different region.
         
         @param request: CreateDirectoryRequest
@@ -747,15 +797,17 @@
 
     async def create_directory_with_options_async(
         self,
         request: cloudsso_20210515_models.CreateDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateDirectoryResponse:
         """
-        A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
+        @summary Creates a directory.
+        
+        @description A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
         To create a directory, you must select a region. Alibaba Cloud stores data in the directory only in the region that you select. However, you can deploy Alibaba Cloud resources including Elastic Compute Service (ECS) instances and ApsaraDB RDS instances in other regions. You can also use your cloud account for logons and access the Alibaba Cloud resources in other regions. You can select a region to create a directory based on your security compliance requirements and the geographic location of specific users. If you do not have strict security compliance requirements, we recommend that you select a region that is the closest to the geographical location of the specific users. This way, access to cloud resources is accelerated. You can create the CloudSSO directory in the China (Shanghai), China (Hong Kong), US (Silicon Valley), or Germany (Frankfurt) region.
         This topic provides an example on how to create a directory named `example` in the China (Shanghai) region.
         ## Limits
         - You can create only one directory for a management account.
         - If you want to change the region of a directory, you must delete the directory and then create a directory in a different region.
         
         @param request: CreateDirectoryRequest
@@ -786,15 +838,17 @@
         )
 
     def create_directory(
         self,
         request: cloudsso_20210515_models.CreateDirectoryRequest,
     ) -> cloudsso_20210515_models.CreateDirectoryResponse:
         """
-        A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
+        @summary Creates a directory.
+        
+        @description A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
         To create a directory, you must select a region. Alibaba Cloud stores data in the directory only in the region that you select. However, you can deploy Alibaba Cloud resources including Elastic Compute Service (ECS) instances and ApsaraDB RDS instances in other regions. You can also use your cloud account for logons and access the Alibaba Cloud resources in other regions. You can select a region to create a directory based on your security compliance requirements and the geographic location of specific users. If you do not have strict security compliance requirements, we recommend that you select a region that is the closest to the geographical location of the specific users. This way, access to cloud resources is accelerated. You can create the CloudSSO directory in the China (Shanghai), China (Hong Kong), US (Silicon Valley), or Germany (Frankfurt) region.
         This topic provides an example on how to create a directory named `example` in the China (Shanghai) region.
         ## Limits
         - You can create only one directory for a management account.
         - If you want to change the region of a directory, you must delete the directory and then create a directory in a different region.
         
         @param request: CreateDirectoryRequest
@@ -804,15 +858,17 @@
         return self.create_directory_with_options(request, runtime)
 
     async def create_directory_async(
         self,
         request: cloudsso_20210515_models.CreateDirectoryRequest,
     ) -> cloudsso_20210515_models.CreateDirectoryResponse:
         """
-        A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
+        @summary Creates a directory.
+        
+        @description A directory is a CloudSSO instance. Before you can use CloudSSO, you must create a directory. The directory is used to manage all CloudSSO resources.
         To create a directory, you must select a region. Alibaba Cloud stores data in the directory only in the region that you select. However, you can deploy Alibaba Cloud resources including Elastic Compute Service (ECS) instances and ApsaraDB RDS instances in other regions. You can also use your cloud account for logons and access the Alibaba Cloud resources in other regions. You can select a region to create a directory based on your security compliance requirements and the geographic location of specific users. If you do not have strict security compliance requirements, we recommend that you select a region that is the closest to the geographical location of the specific users. This way, access to cloud resources is accelerated. You can create the CloudSSO directory in the China (Shanghai), China (Hong Kong), US (Silicon Valley), or Germany (Frankfurt) region.
         This topic provides an example on how to create a directory named `example` in the China (Shanghai) region.
         ## Limits
         - You can create only one directory for a management account.
         - If you want to change the region of a directory, you must delete the directory and then create a directory in a different region.
         
         @param request: CreateDirectoryRequest
@@ -823,15 +879,17 @@
 
     def create_group_with_options(
         self,
         request: cloudsso_20210515_models.CreateGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateGroupResponse:
         """
-        This topic provides an example on how to create a group named `TestGroup`.
+        @summary Creates a group.
+        
+        @description This topic provides an example on how to create a group named `TestGroup`.
         
         @param request: CreateGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -862,15 +920,17 @@
 
     async def create_group_with_options_async(
         self,
         request: cloudsso_20210515_models.CreateGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateGroupResponse:
         """
-        This topic provides an example on how to create a group named `TestGroup`.
+        @summary Creates a group.
+        
+        @description This topic provides an example on how to create a group named `TestGroup`.
         
         @param request: CreateGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -900,43 +960,49 @@
         )
 
     def create_group(
         self,
         request: cloudsso_20210515_models.CreateGroupRequest,
     ) -> cloudsso_20210515_models.CreateGroupResponse:
         """
-        This topic provides an example on how to create a group named `TestGroup`.
+        @summary Creates a group.
+        
+        @description This topic provides an example on how to create a group named `TestGroup`.
         
         @param request: CreateGroupRequest
         @return: CreateGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_group_with_options(request, runtime)
 
     async def create_group_async(
         self,
         request: cloudsso_20210515_models.CreateGroupRequest,
     ) -> cloudsso_20210515_models.CreateGroupResponse:
         """
-        This topic provides an example on how to create a group named `TestGroup`.
+        @summary Creates a group.
+        
+        @description This topic provides an example on how to create a group named `TestGroup`.
         
         @param request: CreateGroupRequest
         @return: CreateGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_group_with_options_async(request, runtime)
 
     def create_scimserver_credential_with_options(
         self,
         request: cloudsso_20210515_models.CreateSCIMServerCredentialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateSCIMServerCredentialResponse:
         """
-        SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
-        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61****`.
+        @summary Creates a Cross-domain Identity Management (SCIM) credential.
+        
+        @description SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
+        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61***`.
         
         @param request: CreateSCIMServerCredentialRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSCIMServerCredentialResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -963,16 +1029,18 @@
 
     async def create_scimserver_credential_with_options_async(
         self,
         request: cloudsso_20210515_models.CreateSCIMServerCredentialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateSCIMServerCredentialResponse:
         """
-        SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
-        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61****`.
+        @summary Creates a Cross-domain Identity Management (SCIM) credential.
+        
+        @description SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
+        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61***`.
         
         @param request: CreateSCIMServerCredentialRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSCIMServerCredentialResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -998,44 +1066,50 @@
         )
 
     def create_scimserver_credential(
         self,
         request: cloudsso_20210515_models.CreateSCIMServerCredentialRequest,
     ) -> cloudsso_20210515_models.CreateSCIMServerCredentialResponse:
         """
-        SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
-        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61****`.
+        @summary Creates a Cross-domain Identity Management (SCIM) credential.
+        
+        @description SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
+        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61***`.
         
         @param request: CreateSCIMServerCredentialRequest
         @return: CreateSCIMServerCredentialResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_scimserver_credential_with_options(request, runtime)
 
     async def create_scimserver_credential_async(
         self,
         request: cloudsso_20210515_models.CreateSCIMServerCredentialRequest,
     ) -> cloudsso_20210515_models.CreateSCIMServerCredentialResponse:
         """
-        SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
-        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61****`.
+        @summary Creates a Cross-domain Identity Management (SCIM) credential.
+        
+        @description SCIM credentials are required for SCIM synchronization. You can create up to two SCIM credentials.
+        This topic provides an example on how to create a SCIM credential within the directory `d-00fc2p61***`.
         
         @param request: CreateSCIMServerCredentialRequest
         @return: CreateSCIMServerCredentialResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_scimserver_credential_with_options_async(request, runtime)
 
     def create_user_with_options(
         self,
         request: cloudsso_20210515_models.CreateUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateUserResponse:
         """
-        This topic provides an example on how to create a user named `Alice`.
+        @summary Creates a user.
+        
+        @description This topic provides an example on how to create a user named `Alice`.
         
         @param request: CreateUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1076,15 +1150,17 @@
 
     async def create_user_with_options_async(
         self,
         request: cloudsso_20210515_models.CreateUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateUserResponse:
         """
-        This topic provides an example on how to create a user named `Alice`.
+        @summary Creates a user.
+        
+        @description This topic provides an example on how to create a user named `Alice`.
         
         @param request: CreateUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1124,40 +1200,51 @@
         )
 
     def create_user(
         self,
         request: cloudsso_20210515_models.CreateUserRequest,
     ) -> cloudsso_20210515_models.CreateUserResponse:
         """
-        This topic provides an example on how to create a user named `Alice`.
+        @summary Creates a user.
+        
+        @description This topic provides an example on how to create a user named `Alice`.
         
         @param request: CreateUserRequest
         @return: CreateUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_user_with_options(request, runtime)
 
     async def create_user_async(
         self,
         request: cloudsso_20210515_models.CreateUserRequest,
     ) -> cloudsso_20210515_models.CreateUserResponse:
         """
-        This topic provides an example on how to create a user named `Alice`.
+        @summary Creates a user.
+        
+        @description This topic provides an example on how to create a user named `Alice`.
         
         @param request: CreateUserRequest
         @return: CreateUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_user_with_options_async(request, runtime)
 
     def create_user_provisioning_with_options(
         self,
         request: cloudsso_20210515_models.CreateUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateUserProvisioningResponse:
+        """
+        @summary Creates a Resource Access Management (RAM) user provisioning.
+        
+        @param request: CreateUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deletion_strategy):
             query['DeletionStrategy'] = request.deletion_strategy
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.directory_id):
@@ -1192,14 +1279,21 @@
         )
 
     async def create_user_provisioning_with_options_async(
         self,
         request: cloudsso_20210515_models.CreateUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.CreateUserProvisioningResponse:
+        """
+        @summary Creates a Resource Access Management (RAM) user provisioning.
+        
+        @param request: CreateUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deletion_strategy):
             query['DeletionStrategy'] = request.deletion_strategy
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.directory_id):
@@ -1233,32 +1327,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_user_provisioning(
         self,
         request: cloudsso_20210515_models.CreateUserProvisioningRequest,
     ) -> cloudsso_20210515_models.CreateUserProvisioningResponse:
+        """
+        @summary Creates a Resource Access Management (RAM) user provisioning.
+        
+        @param request: CreateUserProvisioningRequest
+        @return: CreateUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_user_provisioning_with_options(request, runtime)
 
     async def create_user_provisioning_async(
         self,
         request: cloudsso_20210515_models.CreateUserProvisioningRequest,
     ) -> cloudsso_20210515_models.CreateUserProvisioningResponse:
+        """
+        @summary Creates a Resource Access Management (RAM) user provisioning.
+        
+        @param request: CreateUserProvisioningRequest
+        @return: CreateUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_user_provisioning_with_options_async(request, runtime)
 
     def delete_access_assignment_with_options(
         self,
         request: cloudsso_20210515_models.DeleteAccessAssignmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to remove the access permissions on the account `114240524784****` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes the access permissions on an account in a resource directory.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to remove the access permissions on the account `114240524784***` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
         
         @param request: DeleteAccessAssignmentRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccessAssignmentResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1297,16 +1405,18 @@
 
     async def delete_access_assignment_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteAccessAssignmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to remove the access permissions on the account `114240524784****` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes the access permissions on an account in a resource directory.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to remove the access permissions on the account `114240524784***` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
         
         @param request: DeleteAccessAssignmentRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccessAssignmentResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1344,46 +1454,52 @@
         )
 
     def delete_access_assignment(
         self,
         request: cloudsso_20210515_models.DeleteAccessAssignmentRequest,
     ) -> cloudsso_20210515_models.DeleteAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to remove the access permissions on the account `114240524784****` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes the access permissions on an account in a resource directory.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to remove the access permissions on the account `114240524784***` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
         
         @param request: DeleteAccessAssignmentRequest
         @return: DeleteAccessAssignmentResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_access_assignment_with_options(request, runtime)
 
     async def delete_access_assignment_async(
         self,
         request: cloudsso_20210515_models.DeleteAccessAssignmentRequest,
     ) -> cloudsso_20210515_models.DeleteAccessAssignmentResponse:
         """
-        When you call this operation, an asynchronous task is created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to remove the access permissions on the account `114240524784****` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes the access permissions on an account in a resource directory.
+        
+        @description When you call this operation, an asynchronous task is created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to remove the access permissions on the account `114240524784***` in the resource directory from the CloudSSO user `u-00q8wbq42wiltcrk****`. The access permissions are assigned by using the access configuration `ac-00jhtfl8thteu6uj****`.
         
         @param request: DeleteAccessAssignmentRequest
         @return: DeleteAccessAssignmentResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_access_assignment_with_options_async(request, runtime)
 
     def delete_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.DeleteAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteAccessConfigurationResponse:
         """
-        This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
+        @summary Deletes an access configuration.
+        
+        @description This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
         ## Prerequisites
-        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](~~338352~~).
+        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](https://help.aliyun.com/document_detail/338352.html).
         
         @param request: DeleteAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1414,17 +1530,19 @@
 
     async def delete_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteAccessConfigurationResponse:
         """
-        This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
+        @summary Deletes an access configuration.
+        
+        @description This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
         ## Prerequisites
-        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](~~338352~~).
+        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](https://help.aliyun.com/document_detail/338352.html).
         
         @param request: DeleteAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1454,54 +1572,60 @@
         )
 
     def delete_access_configuration(
         self,
         request: cloudsso_20210515_models.DeleteAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.DeleteAccessConfigurationResponse:
         """
-        This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
+        @summary Deletes an access configuration.
+        
+        @description This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
         ## Prerequisites
-        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](~~338352~~).
+        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](https://help.aliyun.com/document_detail/338352.html).
         
         @param request: DeleteAccessConfigurationRequest
         @return: DeleteAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_access_configuration_with_options(request, runtime)
 
     async def delete_access_configuration_async(
         self,
         request: cloudsso_20210515_models.DeleteAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.DeleteAccessConfigurationResponse:
         """
-        This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
+        @summary Deletes an access configuration.
+        
+        @description This topic provides an example on how to delete the access configuration whose ID is `ac-001j9mcm3k7335bc***`.
         ## Prerequisites
-        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](~~338352~~).
+        The access configuration that you want to delete is de-provisioned from the accounts in your resource directory. For more information, see [DeprovisionAccessConfiguration](https://help.aliyun.com/document_detail/338352.html).
         
         @param request: DeleteAccessConfigurationRequest
         @return: DeleteAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_access_configuration_with_options_async(request, runtime)
 
     def delete_directory_with_options(
         self,
         request: cloudsso_20210515_models.DeleteDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteDirectoryResponse:
         """
-        This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
+        @summary Deletes a directory.
+        
+        @description This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
         ## Prerequisites
         No resources are contained in the directory that you want to delete.
-        *   Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Users are deleted. For more information, see [DeleteUser](~~341671~~).
-        *   Groups are deleted. For more information, see [DeleteGroup](~~341821~~).
-        *   Access configurations are deleted. For more information, see [DeleteAccessConfiguration](~~336907~~).
-        *   System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](~~341842~~).
-        *   SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](~~341573~~).
+        Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Users are deleted. For more information, see [DeleteUser](https://help.aliyun.com/document_detail/341671.html).
+        Groups are deleted. For more information, see [DeleteGroup](https://help.aliyun.com/document_detail/341821.html).
+        Access configurations are deleted. For more information, see [DeleteAccessConfiguration](https://help.aliyun.com/document_detail/336907.html).
+        System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](https://help.aliyun.com/document_detail/341842.html).
+        SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](https://help.aliyun.com/document_detail/341573.html).
         
         @param request: DeleteDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1528,23 +1652,25 @@
 
     async def delete_directory_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteDirectoryResponse:
         """
-        This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
+        @summary Deletes a directory.
+        
+        @description This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
         ## Prerequisites
         No resources are contained in the directory that you want to delete.
-        *   Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Users are deleted. For more information, see [DeleteUser](~~341671~~).
-        *   Groups are deleted. For more information, see [DeleteGroup](~~341821~~).
-        *   Access configurations are deleted. For more information, see [DeleteAccessConfiguration](~~336907~~).
-        *   System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](~~341842~~).
-        *   SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](~~341573~~).
+        Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Users are deleted. For more information, see [DeleteUser](https://help.aliyun.com/document_detail/341671.html).
+        Groups are deleted. For more information, see [DeleteGroup](https://help.aliyun.com/document_detail/341821.html).
+        Access configurations are deleted. For more information, see [DeleteAccessConfiguration](https://help.aliyun.com/document_detail/336907.html).
+        System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](https://help.aliyun.com/document_detail/341842.html).
+        SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](https://help.aliyun.com/document_detail/341573.html).
         
         @param request: DeleteDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1570,62 +1696,68 @@
         )
 
     def delete_directory(
         self,
         request: cloudsso_20210515_models.DeleteDirectoryRequest,
     ) -> cloudsso_20210515_models.DeleteDirectoryResponse:
         """
-        This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
+        @summary Deletes a directory.
+        
+        @description This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
         ## Prerequisites
         No resources are contained in the directory that you want to delete.
-        *   Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Users are deleted. For more information, see [DeleteUser](~~341671~~).
-        *   Groups are deleted. For more information, see [DeleteGroup](~~341821~~).
-        *   Access configurations are deleted. For more information, see [DeleteAccessConfiguration](~~336907~~).
-        *   System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](~~341842~~).
-        *   SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](~~341573~~).
+        Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Users are deleted. For more information, see [DeleteUser](https://help.aliyun.com/document_detail/341671.html).
+        Groups are deleted. For more information, see [DeleteGroup](https://help.aliyun.com/document_detail/341821.html).
+        Access configurations are deleted. For more information, see [DeleteAccessConfiguration](https://help.aliyun.com/document_detail/336907.html).
+        System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](https://help.aliyun.com/document_detail/341842.html).
+        SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](https://help.aliyun.com/document_detail/341573.html).
         
         @param request: DeleteDirectoryRequest
         @return: DeleteDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_directory_with_options(request, runtime)
 
     async def delete_directory_async(
         self,
         request: cloudsso_20210515_models.DeleteDirectoryRequest,
     ) -> cloudsso_20210515_models.DeleteDirectoryResponse:
         """
-        This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
+        @summary Deletes a directory.
+        
+        @description This topic provides an example on how to delete a directory whose ID is `d-00fc2p61***`.
         ## Prerequisites
         No resources are contained in the directory that you want to delete.
-        *   Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Users are deleted. For more information, see [DeleteUser](~~341671~~).
-        *   Groups are deleted. For more information, see [DeleteGroup](~~341821~~).
-        *   Access configurations are deleted. For more information, see [DeleteAccessConfiguration](~~336907~~).
-        *   System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](~~341842~~).
-        *   SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](~~341573~~).
+        Access permissions on the accounts in your resource directory are removed from all users and groups. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Users are deleted. For more information, see [DeleteUser](https://help.aliyun.com/document_detail/341671.html).
+        Groups are deleted. For more information, see [DeleteGroup](https://help.aliyun.com/document_detail/341821.html).
+        Access configurations are deleted. For more information, see [DeleteAccessConfiguration](https://help.aliyun.com/document_detail/336907.html).
+        System for Cross-domain Identity Management (SCIM) credentials are deleted. For more information, see [DeleteSCIMServerCredential](https://help.aliyun.com/document_detail/341842.html).
+        SSO logon configurations are deleted. For more information, see [ClearExternalSAMLIdentityProvider](https://help.aliyun.com/document_detail/341573.html).
         
         @param request: DeleteDirectoryRequest
         @return: DeleteDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_directory_with_options_async(request, runtime)
 
     def delete_group_with_options(
         self,
         request: cloudsso_20210515_models.DeleteGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
+        @summary Deletes a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
         ## Prerequisites
         The group that you want to delete is not associated with the following resources. If the group is associated with the resources, the deletion fails.
-        *   Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](~~335116~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](~~338350~~).
+        Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
         
         @param request: DeleteGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1654,19 +1786,21 @@
 
     async def delete_group_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
+        @summary Deletes a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
         ## Prerequisites
         The group that you want to delete is not associated with the following resources. If the group is associated with the resources, the deletion fails.
-        *   Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](~~335116~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](~~338350~~).
+        Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
         
         @param request: DeleteGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1694,50 +1828,56 @@
         )
 
     def delete_group(
         self,
         request: cloudsso_20210515_models.DeleteGroupRequest,
     ) -> cloudsso_20210515_models.DeleteGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
+        @summary Deletes a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
         ## Prerequisites
         The group that you want to delete is not associated with the following resources. If the group is associated with the resources, the deletion fails.
-        *   Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](~~335116~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](~~338350~~).
+        Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
         
         @param request: DeleteGroupRequest
         @return: DeleteGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_group_with_options(request, runtime)
 
     async def delete_group_async(
         self,
         request: cloudsso_20210515_models.DeleteGroupRequest,
     ) -> cloudsso_20210515_models.DeleteGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
+        @summary Deletes a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a group that is synchronized by using SCIM.
         ## Prerequisites
         The group that you want to delete is not associated with the following resources. If the group is associated with the resources, the deletion fails.
-        *   Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](~~335116~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](~~338350~~).
+        Users: You must remove users from the group. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the group. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
         
         @param request: DeleteGroupRequest
         @return: DeleteGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_group_with_options_async(request, runtime)
 
     def delete_mfadevice_for_user_with_options(
         self,
         request: cloudsso_20210515_models.DeleteMFADeviceForUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteMFADeviceForUserResponse:
         """
-        This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
+        @summary Unbinds a multi-factor authentication (MFA) device from a user.
+        
+        @description This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
         
         @param request: DeleteMFADeviceForUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteMFADeviceForUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1768,15 +1908,17 @@
 
     async def delete_mfadevice_for_user_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteMFADeviceForUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteMFADeviceForUserResponse:
         """
-        This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
+        @summary Unbinds a multi-factor authentication (MFA) device from a user.
+        
+        @description This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
         
         @param request: DeleteMFADeviceForUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteMFADeviceForUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1806,43 +1948,49 @@
         )
 
     def delete_mfadevice_for_user(
         self,
         request: cloudsso_20210515_models.DeleteMFADeviceForUserRequest,
     ) -> cloudsso_20210515_models.DeleteMFADeviceForUserResponse:
         """
-        This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
+        @summary Unbinds a multi-factor authentication (MFA) device from a user.
+        
+        @description This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
         
         @param request: DeleteMFADeviceForUserRequest
         @return: DeleteMFADeviceForUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_mfadevice_for_user_with_options(request, runtime)
 
     async def delete_mfadevice_for_user_async(
         self,
         request: cloudsso_20210515_models.DeleteMFADeviceForUserRequest,
     ) -> cloudsso_20210515_models.DeleteMFADeviceForUserResponse:
         """
-        This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
+        @summary Unbinds a multi-factor authentication (MFA) device from a user.
+        
+        @description This topic provides an example on how to unbind the MFA device `mfa-00ujhet8pycljj7j***` from the user `u-00q8wbq42wiltcrk****`.
         
         @param request: DeleteMFADeviceForUserRequest
         @return: DeleteMFADeviceForUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mfadevice_for_user_with_options_async(request, runtime)
 
     def delete_scimserver_credential_with_options(
         self,
         request: cloudsso_20210515_models.DeleteSCIMServerCredentialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteSCIMServerCredentialResponse:
         """
-        After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
-        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi****`.
+        @summary Deletes a Cross-domain Identity Management (SCIM) credential.
+        
+        @description After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
+        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`.
         
         @param request: DeleteSCIMServerCredentialRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSCIMServerCredentialResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1871,16 +2019,18 @@
 
     async def delete_scimserver_credential_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteSCIMServerCredentialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteSCIMServerCredentialResponse:
         """
-        After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
-        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi****`.
+        @summary Deletes a Cross-domain Identity Management (SCIM) credential.
+        
+        @description After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
+        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`.
         
         @param request: DeleteSCIMServerCredentialRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSCIMServerCredentialResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1908,49 +2058,55 @@
         )
 
     def delete_scimserver_credential(
         self,
         request: cloudsso_20210515_models.DeleteSCIMServerCredentialRequest,
     ) -> cloudsso_20210515_models.DeleteSCIMServerCredentialResponse:
         """
-        After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
-        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi****`.
+        @summary Deletes a Cross-domain Identity Management (SCIM) credential.
+        
+        @description After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
+        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`.
         
         @param request: DeleteSCIMServerCredentialRequest
         @return: DeleteSCIMServerCredentialResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_scimserver_credential_with_options(request, runtime)
 
     async def delete_scimserver_credential_async(
         self,
         request: cloudsso_20210515_models.DeleteSCIMServerCredentialRequest,
     ) -> cloudsso_20210515_models.DeleteSCIMServerCredentialResponse:
         """
-        After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
-        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi****`.
+        @summary Deletes a Cross-domain Identity Management (SCIM) credential.
+        
+        @description After a SCIM credential is deleted, the synchronization task that uses the SCIM credential fails.
+        This topic provides an example on how to delete the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`.
         
         @param request: DeleteSCIMServerCredentialRequest
         @return: DeleteSCIMServerCredentialResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_scimserver_credential_with_options_async(request, runtime)
 
     def delete_user_with_options(
         self,
         request: cloudsso_20210515_models.DeleteUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteUserResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
+        @summary Deletes a user.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
         ## Prerequisites
         The user that you want to delete is not associated with the following resources. If the user is associated with the resources, the deletion fails.
-        *   Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](~~341675~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](~~335116~~).
+        Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](https://help.aliyun.com/document_detail/341675.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
         
         @param request: DeleteUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1979,20 +2135,22 @@
 
     async def delete_user_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteUserResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
+        @summary Deletes a user.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
         ## Prerequisites
         The user that you want to delete is not associated with the following resources. If the user is associated with the resources, the deletion fails.
-        *   Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](~~341675~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](~~335116~~).
+        Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](https://help.aliyun.com/document_detail/341675.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
         
         @param request: DeleteUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2020,50 +2178,61 @@
         )
 
     def delete_user(
         self,
         request: cloudsso_20210515_models.DeleteUserRequest,
     ) -> cloudsso_20210515_models.DeleteUserResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
+        @summary Deletes a user.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
         ## Prerequisites
         The user that you want to delete is not associated with the following resources. If the user is associated with the resources, the deletion fails.
-        *   Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](~~341675~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](~~335116~~).
+        Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](https://help.aliyun.com/document_detail/341675.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
         
         @param request: DeleteUserRequest
         @return: DeleteUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_user_with_options(request, runtime)
 
     async def delete_user_async(
         self,
         request: cloudsso_20210515_models.DeleteUserRequest,
     ) -> cloudsso_20210515_models.DeleteUserResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
+        @summary Deletes a user.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot delete a user that is synchronized by using SCIM.
         ## Prerequisites
         The user that you want to delete is not associated with the following resources. If the user is associated with the resources, the deletion fails.
-        *   Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](~~341675~~).
-        *   Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](~~338350~~).
-        *   Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](~~335116~~).
+        Multi-factor authentication (MFA) devices: You must unbind the MFA devices from the user. For more information, see [DeleteMFADeviceForUser](https://help.aliyun.com/document_detail/341675.html).
+        Access permissions: You must remove the access permissions on the accounts in your resource directory from the user. For more information, see [DeleteAccessAssignment](https://help.aliyun.com/document_detail/338350.html).
+        Groups: You must remove the user from groups. For more information, see [RemoveUserFromGroup](https://help.aliyun.com/document_detail/335116.html).
         
         @param request: DeleteUserRequest
         @return: DeleteUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_user_with_options_async(request, runtime)
 
     def delete_user_provisioning_with_options(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning.
+        
+        @param request: DeleteUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deletion_strategy):
             query['DeletionStrategy'] = request.deletion_strategy
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.user_provisioning_id):
@@ -2088,14 +2257,21 @@
         )
 
     async def delete_user_provisioning_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning.
+        
+        @param request: DeleteUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.deletion_strategy):
             query['DeletionStrategy'] = request.deletion_strategy
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.user_provisioning_id):
@@ -2119,29 +2295,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_user_provisioning(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningRequest,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning.
+        
+        @param request: DeleteUserProvisioningRequest
+        @return: DeleteUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_user_provisioning_with_options(request, runtime)
 
     async def delete_user_provisioning_async(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningRequest,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning.
+        
+        @param request: DeleteUserProvisioningRequest
+        @return: DeleteUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_user_provisioning_with_options_async(request, runtime)
 
     def delete_user_provisioning_event_with_options(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningEventResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: DeleteUserProvisioningEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserProvisioningEventResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.event_id):
             query['EventId'] = request.event_id
         if not UtilClient.is_unset(request.user_provisioning_id):
@@ -2166,14 +2361,21 @@
         )
 
     async def delete_user_provisioning_event_with_options_async(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningEventResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: DeleteUserProvisioningEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserProvisioningEventResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.event_id):
             query['EventId'] = request.event_id
         if not UtilClient.is_unset(request.user_provisioning_id):
@@ -2197,32 +2399,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_user_provisioning_event(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningEventRequest,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningEventResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: DeleteUserProvisioningEventRequest
+        @return: DeleteUserProvisioningEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_user_provisioning_event_with_options(request, runtime)
 
     async def delete_user_provisioning_event_async(
         self,
         request: cloudsso_20210515_models.DeleteUserProvisioningEventRequest,
     ) -> cloudsso_20210515_models.DeleteUserProvisioningEventResponse:
+        """
+        @summary Deletes a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: DeleteUserProvisioningEventRequest
+        @return: DeleteUserProvisioningEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_user_provisioning_event_with_options_async(request, runtime)
 
     def deprovision_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.DeprovisionAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeprovisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj****` from the account `114240524784****` in your resource directory.
+        @summary De-provisions an access configuration from an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj***` from the account `114240524784****` in your resource directory.
         
         @param request: DeprovisionAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeprovisionAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2255,16 +2471,18 @@
 
     async def deprovision_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.DeprovisionAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DeprovisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj****` from the account `114240524784****` in your resource directory.
+        @summary De-provisions an access configuration from an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj***` from the account `114240524784****` in your resource directory.
         
         @param request: DeprovisionAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeprovisionAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2296,43 +2514,145 @@
         )
 
     def deprovision_access_configuration(
         self,
         request: cloudsso_20210515_models.DeprovisionAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.DeprovisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj****` from the account `114240524784****` in your resource directory.
+        @summary De-provisions an access configuration from an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj***` from the account `114240524784****` in your resource directory.
         
         @param request: DeprovisionAccessConfigurationRequest
         @return: DeprovisionAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.deprovision_access_configuration_with_options(request, runtime)
 
     async def deprovision_access_configuration_async(
         self,
         request: cloudsso_20210515_models.DeprovisionAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.DeprovisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj****` from the account `114240524784****` in your resource directory.
+        @summary De-provisions an access configuration from an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to de-provision the access configuration `ac-00jhtfl8thteu6uj***` from the account `114240524784****` in your resource directory.
         
         @param request: DeprovisionAccessConfigurationRequest
         @return: DeprovisionAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.deprovision_access_configuration_with_options_async(request, runtime)
 
+    def disable_delegate_account_with_options(
+        self,
+        request: cloudsso_20210515_models.DisableDelegateAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudsso_20210515_models.DisableDelegateAccountResponse:
+        """
+        @summary DisableDelegateAccount
+        
+        @param request: DisableDelegateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableDelegateAccountResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account_id):
+            query['AccountId'] = request.account_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DisableDelegateAccount',
+            version='2021-05-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudsso_20210515_models.DisableDelegateAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def disable_delegate_account_with_options_async(
+        self,
+        request: cloudsso_20210515_models.DisableDelegateAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudsso_20210515_models.DisableDelegateAccountResponse:
+        """
+        @summary DisableDelegateAccount
+        
+        @param request: DisableDelegateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableDelegateAccountResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account_id):
+            query['AccountId'] = request.account_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DisableDelegateAccount',
+            version='2021-05-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudsso_20210515_models.DisableDelegateAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def disable_delegate_account(
+        self,
+        request: cloudsso_20210515_models.DisableDelegateAccountRequest,
+    ) -> cloudsso_20210515_models.DisableDelegateAccountResponse:
+        """
+        @summary DisableDelegateAccount
+        
+        @param request: DisableDelegateAccountRequest
+        @return: DisableDelegateAccountResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.disable_delegate_account_with_options(request, runtime)
+
+    async def disable_delegate_account_async(
+        self,
+        request: cloudsso_20210515_models.DisableDelegateAccountRequest,
+    ) -> cloudsso_20210515_models.DisableDelegateAccountResponse:
+        """
+        @summary DisableDelegateAccount
+        
+        @param request: DisableDelegateAccountRequest
+        @return: DisableDelegateAccountResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.disable_delegate_account_with_options_async(request, runtime)
+
     def disable_service_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DisableServiceResponse:
         """
-        If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
+        @summary Disables CloudSSO.
+        
+        @description If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
         
         @param request: DisableServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DisableServiceResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -2352,15 +2672,17 @@
         )
 
     async def disable_service_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.DisableServiceResponse:
         """
-        If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
+        @summary Disables CloudSSO.
+        
+        @description If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
         
         @param request: DisableServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DisableServiceResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -2377,36 +2699,138 @@
         return TeaCore.from_map(
             cloudsso_20210515_models.DisableServiceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def disable_service(self) -> cloudsso_20210515_models.DisableServiceResponse:
         """
-        If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
+        @summary Disables CloudSSO.
+        
+        @description If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
         
         @return: DisableServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.disable_service_with_options(runtime)
 
     async def disable_service_async(self) -> cloudsso_20210515_models.DisableServiceResponse:
         """
-        If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
+        @summary Disables CloudSSO.
+        
+        @description If your CloudSSO has no directory, you can disable CloudSSO based on your business requirements. After you disable CloudSSO, you can enable it at any time.
         
         @return: DisableServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.disable_service_with_options_async(runtime)
 
+    def enable_delegate_account_with_options(
+        self,
+        request: cloudsso_20210515_models.EnableDelegateAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudsso_20210515_models.EnableDelegateAccountResponse:
+        """
+        @summary EnableDelegateAccount
+        
+        @param request: EnableDelegateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableDelegateAccountResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account_id):
+            query['AccountId'] = request.account_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='EnableDelegateAccount',
+            version='2021-05-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudsso_20210515_models.EnableDelegateAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def enable_delegate_account_with_options_async(
+        self,
+        request: cloudsso_20210515_models.EnableDelegateAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> cloudsso_20210515_models.EnableDelegateAccountResponse:
+        """
+        @summary EnableDelegateAccount
+        
+        @param request: EnableDelegateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableDelegateAccountResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account_id):
+            query['AccountId'] = request.account_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='EnableDelegateAccount',
+            version='2021-05-15',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloudsso_20210515_models.EnableDelegateAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def enable_delegate_account(
+        self,
+        request: cloudsso_20210515_models.EnableDelegateAccountRequest,
+    ) -> cloudsso_20210515_models.EnableDelegateAccountResponse:
+        """
+        @summary EnableDelegateAccount
+        
+        @param request: EnableDelegateAccountRequest
+        @return: EnableDelegateAccountResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.enable_delegate_account_with_options(request, runtime)
+
+    async def enable_delegate_account_async(
+        self,
+        request: cloudsso_20210515_models.EnableDelegateAccountRequest,
+    ) -> cloudsso_20210515_models.EnableDelegateAccountResponse:
+        """
+        @summary EnableDelegateAccount
+        
+        @param request: EnableDelegateAccountRequest
+        @return: EnableDelegateAccountResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.enable_delegate_account_with_options_async(request, runtime)
+
     def enable_service_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.EnableServiceResponse:
         """
-        You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](~~262819~~).
+        @summary Enables CloudSSO.
+        
+        @description You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](https://help.aliyun.com/document_detail/262819.html).
         If you call this operation, you agree to the [Alibaba Cloud International Website Product Terms of Service](https://www.alibabacloud.com/help/doc-detail/42416.htm).
         
         @param request: EnableServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableServiceResponse
         """
         req = open_api_models.OpenApiRequest()
@@ -2427,15 +2851,17 @@
         )
 
     async def enable_service_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.EnableServiceResponse:
         """
-        You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](~~262819~~).
+        @summary Enables CloudSSO.
+        
+        @description You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](https://help.aliyun.com/document_detail/262819.html).
         If you call this operation, you agree to the [Alibaba Cloud International Website Product Terms of Service](https://www.alibabacloud.com/help/doc-detail/42416.htm).
         
         @param request: EnableServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableServiceResponse
         """
         req = open_api_models.OpenApiRequest()
@@ -2453,39 +2879,45 @@
         return TeaCore.from_map(
             cloudsso_20210515_models.EnableServiceResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_service(self) -> cloudsso_20210515_models.EnableServiceResponse:
         """
-        You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](~~262819~~).
+        @summary Enables CloudSSO.
+        
+        @description You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](https://help.aliyun.com/document_detail/262819.html).
         If you call this operation, you agree to the [Alibaba Cloud International Website Product Terms of Service](https://www.alibabacloud.com/help/doc-detail/42416.htm).
         
         @return: EnableServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.enable_service_with_options(runtime)
 
     async def enable_service_async(self) -> cloudsso_20210515_models.EnableServiceResponse:
         """
-        You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](~~262819~~).
+        @summary Enables CloudSSO.
+        
+        @description You can call this operation only if your account belongs to the management account that is used to enable a resource directory and has permissions to enable CloudSSO. For more information, see [Enable CloudSSO](https://help.aliyun.com/document_detail/262819.html).
         If you call this operation, you agree to the [Alibaba Cloud International Website Product Terms of Service](https://www.alibabacloud.com/help/doc-detail/42416.htm).
         
         @return: EnableServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.enable_service_with_options_async(runtime)
 
     def get_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.GetAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
+        @summary Queries information about an access configuration.
+        
+        @description This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
         
         @param request: GetAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2514,15 +2946,17 @@
 
     async def get_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.GetAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
+        @summary Queries information about an access configuration.
+        
+        @description This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
         
         @param request: GetAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2550,42 +2984,48 @@
         )
 
     def get_access_configuration(
         self,
         request: cloudsso_20210515_models.GetAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.GetAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
+        @summary Queries information about an access configuration.
+        
+        @description This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
         
         @param request: GetAccessConfigurationRequest
         @return: GetAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_access_configuration_with_options(request, runtime)
 
     async def get_access_configuration_async(
         self,
         request: cloudsso_20210515_models.GetAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.GetAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
+        @summary Queries information about an access configuration.
+        
+        @description This topic provides an example on how to query the information about the access configuration whose ID is `ac-00ccule7tadaijxc***`.
         
         @param request: GetAccessConfigurationRequest
         @return: GetAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_access_configuration_with_options_async(request, runtime)
 
     def get_directory_with_options(
         self,
         request: cloudsso_20210515_models.GetDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetDirectoryResponse:
         """
-        This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
+        @summary Queries information about a directory.
+        
+        @description This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
         
         @param request: GetDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2612,15 +3052,17 @@
 
     async def get_directory_with_options_async(
         self,
         request: cloudsso_20210515_models.GetDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetDirectoryResponse:
         """
-        This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
+        @summary Queries information about a directory.
+        
+        @description This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
         
         @param request: GetDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2646,43 +3088,49 @@
         )
 
     def get_directory(
         self,
         request: cloudsso_20210515_models.GetDirectoryRequest,
     ) -> cloudsso_20210515_models.GetDirectoryResponse:
         """
-        This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
+        @summary Queries information about a directory.
+        
+        @description This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
         
         @param request: GetDirectoryRequest
         @return: GetDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_directory_with_options(request, runtime)
 
     async def get_directory_async(
         self,
         request: cloudsso_20210515_models.GetDirectoryRequest,
     ) -> cloudsso_20210515_models.GetDirectoryResponse:
         """
-        This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
+        @summary Queries information about a directory.
+        
+        @description This topic provides an example on how to query information about the directory whose ID is `d-00fc2p61***`.
         
         @param request: GetDirectoryRequest
         @return: GetDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_directory_with_options_async(request, runtime)
 
     def get_directory_samlservice_provider_info_with_options(
         self,
         request: cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
-        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61****`.
+        @summary Queries information about a Security Assertion Markup Language (SAML) service provider (SP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
+        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61***`.
         
         @param request: GetDirectorySAMLServiceProviderInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDirectorySAMLServiceProviderInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2709,16 +3157,18 @@
 
     async def get_directory_samlservice_provider_info_with_options_async(
         self,
         request: cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
-        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61****`.
+        @summary Queries information about a Security Assertion Markup Language (SAML) service provider (SP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
+        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61***`.
         
         @param request: GetDirectorySAMLServiceProviderInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDirectorySAMLServiceProviderInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2744,45 +3194,51 @@
         )
 
     def get_directory_samlservice_provider_info(
         self,
         request: cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoRequest,
     ) -> cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
-        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61****`.
+        @summary Queries information about a Security Assertion Markup Language (SAML) service provider (SP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
+        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61***`.
         
         @param request: GetDirectorySAMLServiceProviderInfoRequest
         @return: GetDirectorySAMLServiceProviderInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_directory_samlservice_provider_info_with_options(request, runtime)
 
     async def get_directory_samlservice_provider_info_async(
         self,
         request: cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoRequest,
     ) -> cloudsso_20210515_models.GetDirectorySAMLServiceProviderInfoResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
-        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61****`.
+        @summary Queries information about a Security Assertion Markup Language (SAML) service provider (SP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an identity provider (IdP).
+        This topic provides an example on how to query the information about the SP within the directory `d-00fc2p61***`.
         
         @param request: GetDirectorySAMLServiceProviderInfoRequest
         @return: GetDirectorySAMLServiceProviderInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_directory_samlservice_provider_info_with_options_async(request, runtime)
 
     def get_directory_statistics_with_options(
         self,
         request: cloudsso_20210515_models.GetDirectoryStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetDirectoryStatisticsResponse:
         """
-        ### [](#)
-        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61****`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
+        @summary Queries the statistics of a directory.
+        
+        @description ### [](#)
+        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61***`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
         ### [](#qps)Limit
         You can call this operation up to 100 times per second per account. This operation is globally limited to 100 times per second across all accounts. If the number of the calls per second exceeds a limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limits when you call this operation.
         
         @param request: GetDirectoryStatisticsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDirectoryStatisticsResponse
         """
@@ -2811,16 +3267,18 @@
 
     async def get_directory_statistics_with_options_async(
         self,
         request: cloudsso_20210515_models.GetDirectoryStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetDirectoryStatisticsResponse:
         """
-        ### [](#)
-        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61****`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
+        @summary Queries the statistics of a directory.
+        
+        @description ### [](#)
+        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61***`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
         ### [](#qps)Limit
         You can call this operation up to 100 times per second per account. This operation is globally limited to 100 times per second across all accounts. If the number of the calls per second exceeds a limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limits when you call this operation.
         
         @param request: GetDirectoryStatisticsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDirectoryStatisticsResponse
         """
@@ -2848,32 +3306,36 @@
         )
 
     def get_directory_statistics(
         self,
         request: cloudsso_20210515_models.GetDirectoryStatisticsRequest,
     ) -> cloudsso_20210515_models.GetDirectoryStatisticsResponse:
         """
-        ### [](#)
-        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61****`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
+        @summary Queries the statistics of a directory.
+        
+        @description ### [](#)
+        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61***`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
         ### [](#qps)Limit
         You can call this operation up to 100 times per second per account. This operation is globally limited to 100 times per second across all accounts. If the number of the calls per second exceeds a limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limits when you call this operation.
         
         @param request: GetDirectoryStatisticsRequest
         @return: GetDirectoryStatisticsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_directory_statistics_with_options(request, runtime)
 
     async def get_directory_statistics_async(
         self,
         request: cloudsso_20210515_models.GetDirectoryStatisticsRequest,
     ) -> cloudsso_20210515_models.GetDirectoryStatisticsResponse:
         """
-        ### [](#)
-        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61****`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
+        @summary Queries the statistics of a directory.
+        
+        @description ### [](#)
+        This topic provides an example on how to query the statistics of a directory whose ID is `d-00fc2p61***`. The statistics include the number of users, quota for users, number of groups, quota for groups, number of access configurations, quota for access configurations, quota for system policies that can be configured for an access configuration, number of access permissions that are assigned, number of System for Cross-domain Identity Management (SCIM) credentials, number of asynchronous tasks, status of single sign-on (SSO), and status of SCIM synchronization.
         ### [](#qps)Limit
         You can call this operation up to 100 times per second per account. This operation is globally limited to 100 times per second across all accounts. If the number of the calls per second exceeds a limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limits when you call this operation.
         
         @param request: GetDirectoryStatisticsRequest
         @return: GetDirectoryStatisticsResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2881,15 +3343,17 @@
 
     def get_external_samlidentity_provider_with_options(
         self,
         request: cloudsso_20210515_models.GetExternalSAMLIdentityProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetExternalSAMLIdentityProviderResponse:
         """
-        This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
+        @summary Queries the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: GetExternalSAMLIdentityProviderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetExternalSAMLIdentityProviderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2916,15 +3380,17 @@
 
     async def get_external_samlidentity_provider_with_options_async(
         self,
         request: cloudsso_20210515_models.GetExternalSAMLIdentityProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetExternalSAMLIdentityProviderResponse:
         """
-        This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
+        @summary Queries the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: GetExternalSAMLIdentityProviderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetExternalSAMLIdentityProviderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2950,42 +3416,48 @@
         )
 
     def get_external_samlidentity_provider(
         self,
         request: cloudsso_20210515_models.GetExternalSAMLIdentityProviderRequest,
     ) -> cloudsso_20210515_models.GetExternalSAMLIdentityProviderResponse:
         """
-        This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
+        @summary Queries the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: GetExternalSAMLIdentityProviderRequest
         @return: GetExternalSAMLIdentityProviderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_external_samlidentity_provider_with_options(request, runtime)
 
     async def get_external_samlidentity_provider_async(
         self,
         request: cloudsso_20210515_models.GetExternalSAMLIdentityProviderRequest,
     ) -> cloudsso_20210515_models.GetExternalSAMLIdentityProviderResponse:
         """
-        This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
+        @summary Queries the configurations of a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description This topic provides an example on how to query the configurations of the SAML IdP within the directory `d-00fc2p61***`.
         
         @param request: GetExternalSAMLIdentityProviderRequest
         @return: GetExternalSAMLIdentityProviderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_external_samlidentity_provider_with_options_async(request, runtime)
 
     def get_group_with_options(
         self,
         request: cloudsso_20210515_models.GetGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetGroupResponse:
         """
-        This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
+        @summary Queries information about a group.
+        
+        @description This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
         
         @param request: GetGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3014,15 +3486,17 @@
 
     async def get_group_with_options_async(
         self,
         request: cloudsso_20210515_models.GetGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetGroupResponse:
         """
-        This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
+        @summary Queries information about a group.
+        
+        @description This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
         
         @param request: GetGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3050,40 +3524,51 @@
         )
 
     def get_group(
         self,
         request: cloudsso_20210515_models.GetGroupRequest,
     ) -> cloudsso_20210515_models.GetGroupResponse:
         """
-        This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
+        @summary Queries information about a group.
+        
+        @description This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
         
         @param request: GetGroupRequest
         @return: GetGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_group_with_options(request, runtime)
 
     async def get_group_async(
         self,
         request: cloudsso_20210515_models.GetGroupRequest,
     ) -> cloudsso_20210515_models.GetGroupResponse:
         """
-        This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
+        @summary Queries information about a group.
+        
+        @description This topic provides an example on how to query the information about the group `g-00jqzghi2n3o5hkh***` in the directory `d-00fc2p61****`.
         
         @param request: GetGroupRequest
         @return: GetGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_group_with_options_async(request, runtime)
 
     def get_login_preference_with_options(
         self,
         request: cloudsso_20210515_models.GetLoginPreferenceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetLoginPreferenceResponse:
+        """
+        @summary Queries the logon preference of CloudSSO users.
+        
+        @param request: GetLoginPreferenceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetLoginPreferenceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3104,14 +3589,21 @@
         )
 
     async def get_login_preference_with_options_async(
         self,
         request: cloudsso_20210515_models.GetLoginPreferenceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetLoginPreferenceResponse:
+        """
+        @summary Queries the logon preference of CloudSSO users.
+        
+        @param request: GetLoginPreferenceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetLoginPreferenceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3131,32 +3623,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_login_preference(
         self,
         request: cloudsso_20210515_models.GetLoginPreferenceRequest,
     ) -> cloudsso_20210515_models.GetLoginPreferenceResponse:
+        """
+        @summary Queries the logon preference of CloudSSO users.
+        
+        @param request: GetLoginPreferenceRequest
+        @return: GetLoginPreferenceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_login_preference_with_options(request, runtime)
 
     async def get_login_preference_async(
         self,
         request: cloudsso_20210515_models.GetLoginPreferenceRequest,
     ) -> cloudsso_20210515_models.GetLoginPreferenceResponse:
+        """
+        @summary Queries the logon preference of CloudSSO users.
+        
+        @param request: GetLoginPreferenceRequest
+        @return: GetLoginPreferenceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_login_preference_with_options_async(request, runtime)
 
     def get_mfaauthentication_setting_info_with_options(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingInfoResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk****`.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk***`.
         
         @param request: GetMFAAuthenticationSettingInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetMFAAuthenticationSettingInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3183,16 +3689,18 @@
 
     async def get_mfaauthentication_setting_info_with_options_async(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingInfoResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk****`.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk***`.
         
         @param request: GetMFAAuthenticationSettingInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetMFAAuthenticationSettingInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3218,45 +3726,51 @@
         )
 
     def get_mfaauthentication_setting_info(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingInfoRequest,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingInfoResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk****`.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk***`.
         
         @param request: GetMFAAuthenticationSettingInfoRequest
         @return: GetMFAAuthenticationSettingInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_mfaauthentication_setting_info_with_options(request, runtime)
 
     async def get_mfaauthentication_setting_info_async(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingInfoRequest,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingInfoResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk****`.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to query the MFA setting of all CloudSSO users that belong to the directory named `00q8wbq42wiltcrk***`.
         
         @param request: GetMFAAuthenticationSettingInfoRequest
         @return: GetMFAAuthenticationSettingInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_mfaauthentication_setting_info_with_options_async(request, runtime)
 
     def get_mfaauthentication_settings_with_options(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingsResponse:
         """
-        > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](~~611286~~) operation to query more detailed information.
-        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61****`. The returned result shows that MFA is enabled for all the users.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](https://help.aliyun.com/document_detail/611286.html) operation to query more detailed information.
+        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61***`. The returned result shows that MFA is enabled for all the users.
         
         @param request: GetMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3283,16 +3797,18 @@
 
     async def get_mfaauthentication_settings_with_options_async(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingsResponse:
         """
-        > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](~~611286~~) operation to query more detailed information.
-        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61****`. The returned result shows that MFA is enabled for all the users.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](https://help.aliyun.com/document_detail/611286.html) operation to query more detailed information.
+        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61***`. The returned result shows that MFA is enabled for all the users.
         
         @param request: GetMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3318,44 +3834,50 @@
         )
 
     def get_mfaauthentication_settings(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingsResponse:
         """
-        > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](~~611286~~) operation to query more detailed information.
-        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61****`. The returned result shows that MFA is enabled for all the users.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](https://help.aliyun.com/document_detail/611286.html) operation to query more detailed information.
+        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61***`. The returned result shows that MFA is enabled for all the users.
         
         @param request: GetMFAAuthenticationSettingsRequest
         @return: GetMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_mfaauthentication_settings_with_options(request, runtime)
 
     async def get_mfaauthentication_settings_async(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationSettingsResponse:
         """
-        > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](~~611286~~) operation to query more detailed information.
-        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61****`. The returned result shows that MFA is enabled for all the users.
+        @summary Queries the multi-factor authentication (MFA) setting of all users.
+        
+        @description > This operation is no longer maintained and updated. You can call the [GetMFAAuthenticationSettingInfo](https://help.aliyun.com/document_detail/611286.html) operation to query more detailed information.
+        This topic provides an example on how to query the MFA setting of the users that belong to the directory named `d-00fc2p61***`. The returned result shows that MFA is enabled for all the users.
         
         @param request: GetMFAAuthenticationSettingsRequest
         @return: GetMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_mfaauthentication_settings_with_options_async(request, runtime)
 
     def get_mfaauthentication_status_with_options(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationStatusResponse:
         """
-        This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
+        @summary Checks whether multi-factor authentication (MFA) is enabled for users.
+        
+        @description This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
         
         @param request: GetMFAAuthenticationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetMFAAuthenticationStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3382,15 +3904,17 @@
 
     async def get_mfaauthentication_status_with_options_async(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationStatusResponse:
         """
-        This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
+        @summary Checks whether multi-factor authentication (MFA) is enabled for users.
+        
+        @description This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
         
         @param request: GetMFAAuthenticationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetMFAAuthenticationStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3416,40 +3940,51 @@
         )
 
     def get_mfaauthentication_status(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationStatusRequest,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationStatusResponse:
         """
-        This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
+        @summary Checks whether multi-factor authentication (MFA) is enabled for users.
+        
+        @description This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
         
         @param request: GetMFAAuthenticationStatusRequest
         @return: GetMFAAuthenticationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_mfaauthentication_status_with_options(request, runtime)
 
     async def get_mfaauthentication_status_async(
         self,
         request: cloudsso_20210515_models.GetMFAAuthenticationStatusRequest,
     ) -> cloudsso_20210515_models.GetMFAAuthenticationStatusResponse:
         """
-        This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
+        @summary Checks whether multi-factor authentication (MFA) is enabled for users.
+        
+        @description This topic provides an example on how to check whether MFA is enabled for users in the directory whose ID is `00fc2p61***`. The returned result shows that MFA is in the Enabled state.
         
         @param request: GetMFAAuthenticationStatusRequest
         @return: GetMFAAuthenticationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_mfaauthentication_status_with_options_async(request, runtime)
 
     def get_password_policy_with_options(
         self,
         request: cloudsso_20210515_models.GetPasswordPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetPasswordPolicyResponse:
+        """
+        @summary Queries the password policy of CloudSSO users.
+        
+        @param request: GetPasswordPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPasswordPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3470,14 +4005,21 @@
         )
 
     async def get_password_policy_with_options_async(
         self,
         request: cloudsso_20210515_models.GetPasswordPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetPasswordPolicyResponse:
+        """
+        @summary Queries the password policy of CloudSSO users.
+        
+        @param request: GetPasswordPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPasswordPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3497,31 +4039,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_password_policy(
         self,
         request: cloudsso_20210515_models.GetPasswordPolicyRequest,
     ) -> cloudsso_20210515_models.GetPasswordPolicyResponse:
+        """
+        @summary Queries the password policy of CloudSSO users.
+        
+        @param request: GetPasswordPolicyRequest
+        @return: GetPasswordPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_password_policy_with_options(request, runtime)
 
     async def get_password_policy_async(
         self,
         request: cloudsso_20210515_models.GetPasswordPolicyRequest,
     ) -> cloudsso_20210515_models.GetPasswordPolicyResponse:
+        """
+        @summary Queries the password policy of CloudSSO users.
+        
+        @param request: GetPasswordPolicyRequest
+        @return: GetPasswordPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_password_policy_with_options_async(request, runtime)
 
     def get_scimsynchronization_status_with_options(
         self,
         request: cloudsso_20210515_models.GetSCIMSynchronizationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetSCIMSynchronizationStatusResponse:
         """
-        This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
+        @summary Queries the status of System for Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
         
         @param request: GetSCIMSynchronizationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetSCIMSynchronizationStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3548,15 +4104,17 @@
 
     async def get_scimsynchronization_status_with_options_async(
         self,
         request: cloudsso_20210515_models.GetSCIMSynchronizationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetSCIMSynchronizationStatusResponse:
         """
-        This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
+        @summary Queries the status of System for Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
         
         @param request: GetSCIMSynchronizationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetSCIMSynchronizationStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3582,39 +4140,50 @@
         )
 
     def get_scimsynchronization_status(
         self,
         request: cloudsso_20210515_models.GetSCIMSynchronizationStatusRequest,
     ) -> cloudsso_20210515_models.GetSCIMSynchronizationStatusResponse:
         """
-        This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
+        @summary Queries the status of System for Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
         
         @param request: GetSCIMSynchronizationStatusRequest
         @return: GetSCIMSynchronizationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_scimsynchronization_status_with_options(request, runtime)
 
     async def get_scimsynchronization_status_async(
         self,
         request: cloudsso_20210515_models.GetSCIMSynchronizationStatusRequest,
     ) -> cloudsso_20210515_models.GetSCIMSynchronizationStatusResponse:
         """
-        This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
+        @summary Queries the status of System for Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description This topic provides an example on how to query the status of SCIM synchronization within the directory `d-00fc2p61***`. The returned result shows that SCIM synchronization is in the Enabled state.
         
         @param request: GetSCIMSynchronizationStatusRequest
         @return: GetSCIMSynchronizationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_scimsynchronization_status_with_options_async(request, runtime)
 
     def get_service_status_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetServiceStatusResponse:
+        """
+        @summary Queries the status of CloudSSO.
+        
+        @param request: GetServiceStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceStatusResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetServiceStatus',
             version='2021-05-15',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -3628,14 +4197,21 @@
             self.call_api(params, req, runtime)
         )
 
     async def get_service_status_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetServiceStatusResponse:
+        """
+        @summary Queries the status of CloudSSO.
+        
+        @param request: GetServiceStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetServiceStatusResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetServiceStatus',
             version='2021-05-15',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -3646,28 +4222,40 @@
         )
         return TeaCore.from_map(
             cloudsso_20210515_models.GetServiceStatusResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def get_service_status(self) -> cloudsso_20210515_models.GetServiceStatusResponse:
+        """
+        @summary Queries the status of CloudSSO.
+        
+        @return: GetServiceStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_service_status_with_options(runtime)
 
     async def get_service_status_async(self) -> cloudsso_20210515_models.GetServiceStatusResponse:
+        """
+        @summary Queries the status of CloudSSO.
+        
+        @return: GetServiceStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_service_status_with_options_async(runtime)
 
     def get_task_with_options(
         self,
         request: cloudsso_20210515_models.GetTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetTaskResponse:
         """
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
+        @summary Queries information about an asynchronous task.
+        
+        @description This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3696,15 +4284,17 @@
 
     async def get_task_with_options_async(
         self,
         request: cloudsso_20210515_models.GetTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetTaskResponse:
         """
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
+        @summary Queries information about an asynchronous task.
+        
+        @description This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3732,43 +4322,49 @@
         )
 
     def get_task(
         self,
         request: cloudsso_20210515_models.GetTaskRequest,
     ) -> cloudsso_20210515_models.GetTaskResponse:
         """
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
+        @summary Queries information about an asynchronous task.
+        
+        @description This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskRequest
         @return: GetTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_task_with_options(request, runtime)
 
     async def get_task_async(
         self,
         request: cloudsso_20210515_models.GetTaskRequest,
     ) -> cloudsso_20210515_models.GetTaskResponse:
         """
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
+        @summary Queries information about an asynchronous task.
+        
+        @description This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskRequest
         @return: GetTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_task_with_options_async(request, runtime)
 
     def get_task_status_with_options(
         self,
         request: cloudsso_20210515_models.GetTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetTaskStatusResponse:
         """
-        You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](~~340670~~) operation.
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5****`.
+        @summary Queries the status of an asynchronous task.
+        
+        @description You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation.
+        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetTaskStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3797,16 +4393,18 @@
 
     async def get_task_status_with_options_async(
         self,
         request: cloudsso_20210515_models.GetTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetTaskStatusResponse:
         """
-        You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](~~340670~~) operation.
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5****`.
+        @summary Queries the status of an asynchronous task.
+        
+        @description You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation.
+        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetTaskStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3834,44 +4432,50 @@
         )
 
     def get_task_status(
         self,
         request: cloudsso_20210515_models.GetTaskStatusRequest,
     ) -> cloudsso_20210515_models.GetTaskStatusResponse:
         """
-        You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](~~340670~~) operation.
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5****`.
+        @summary Queries the status of an asynchronous task.
+        
+        @description You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation.
+        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskStatusRequest
         @return: GetTaskStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_task_status_with_options(request, runtime)
 
     async def get_task_status_async(
         self,
         request: cloudsso_20210515_models.GetTaskStatusRequest,
     ) -> cloudsso_20210515_models.GetTaskStatusResponse:
         """
-        You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](~~340670~~) operation.
-        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5****`.
+        @summary Queries the status of an asynchronous task.
+        
+        @description You can call the GetTaskStatus operation to query the status of an asynchronous task. If you want to query more information about an asynchronous task, call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation.
+        This topic provides an example on how to query the information about the task whose ID is `t-shfqw1u1edszvxw5***`.
         
         @param request: GetTaskStatusRequest
         @return: GetTaskStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_task_status_with_options_async(request, runtime)
 
     def get_user_with_options(
         self,
         request: cloudsso_20210515_models.GetUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserResponse:
         """
-        This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
+        @summary Queries information about a user.
+        
+        @description This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
         
         @param request: GetUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3900,15 +4504,17 @@
 
     async def get_user_with_options_async(
         self,
         request: cloudsso_20210515_models.GetUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserResponse:
         """
-        This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
+        @summary Queries information about a user.
+        
+        @description This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
         
         @param request: GetUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3936,40 +4542,51 @@
         )
 
     def get_user(
         self,
         request: cloudsso_20210515_models.GetUserRequest,
     ) -> cloudsso_20210515_models.GetUserResponse:
         """
-        This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
+        @summary Queries information about a user.
+        
+        @description This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
         
         @param request: GetUserRequest
         @return: GetUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_user_with_options(request, runtime)
 
     async def get_user_async(
         self,
         request: cloudsso_20210515_models.GetUserRequest,
     ) -> cloudsso_20210515_models.GetUserResponse:
         """
-        This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
+        @summary Queries information about a user.
+        
+        @description This topic provides an example on how to query information about the user whose ID is `u-00q8wbq42wiltcrk***` in the `d-00fc2p61****` directory.
         
         @param request: GetUserRequest
         @return: GetUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_with_options_async(request, runtime)
 
     def get_user_id_with_options(
         self,
         tmp_req: cloudsso_20210515_models.GetUserIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserIdResponse:
+        """
+        @summary Queries the ID of a user in a resource directory by using the ExternalId parameter.
+        
+        @param tmp_req: GetUserIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserIdResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = cloudsso_20210515_models.GetUserIdShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.external_id):
             request.external_id_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.external_id, 'ExternalId', 'json')
         query = {}
         if not UtilClient.is_unset(request.directory_id):
@@ -3996,14 +4613,21 @@
         )
 
     async def get_user_id_with_options_async(
         self,
         tmp_req: cloudsso_20210515_models.GetUserIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserIdResponse:
+        """
+        @summary Queries the ID of a user in a resource directory by using the ExternalId parameter.
+        
+        @param tmp_req: GetUserIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserIdResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = cloudsso_20210515_models.GetUserIdShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.external_id):
             request.external_id_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.external_id, 'ExternalId', 'json')
         query = {}
         if not UtilClient.is_unset(request.directory_id):
@@ -4029,31 +4653,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_id(
         self,
         request: cloudsso_20210515_models.GetUserIdRequest,
     ) -> cloudsso_20210515_models.GetUserIdResponse:
+        """
+        @summary Queries the ID of a user in a resource directory by using the ExternalId parameter.
+        
+        @param request: GetUserIdRequest
+        @return: GetUserIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_id_with_options(request, runtime)
 
     async def get_user_id_async(
         self,
         request: cloudsso_20210515_models.GetUserIdRequest,
     ) -> cloudsso_20210515_models.GetUserIdResponse:
+        """
+        @summary Queries the ID of a user in a resource directory by using the ExternalId parameter.
+        
+        @param request: GetUserIdRequest
+        @return: GetUserIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_id_with_options_async(request, runtime)
 
     def get_user_mfaauthentication_settings_with_options(
         self,
         request: cloudsso_20210515_models.GetUserMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserMFAAuthenticationSettingsResponse:
         """
-        This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
+        @summary Queries the multi-factor authentication (MFA) setting of a single user.
+        
+        @description This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
         
         @param request: GetUserMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetUserMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4082,15 +4720,17 @@
 
     async def get_user_mfaauthentication_settings_with_options_async(
         self,
         request: cloudsso_20210515_models.GetUserMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserMFAAuthenticationSettingsResponse:
         """
-        This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
+        @summary Queries the multi-factor authentication (MFA) setting of a single user.
+        
+        @description This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
         
         @param request: GetUserMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetUserMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4118,40 +4758,51 @@
         )
 
     def get_user_mfaauthentication_settings(
         self,
         request: cloudsso_20210515_models.GetUserMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.GetUserMFAAuthenticationSettingsResponse:
         """
-        This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
+        @summary Queries the multi-factor authentication (MFA) setting of a single user.
+        
+        @description This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
         
         @param request: GetUserMFAAuthenticationSettingsRequest
         @return: GetUserMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_user_mfaauthentication_settings_with_options(request, runtime)
 
     async def get_user_mfaauthentication_settings_async(
         self,
         request: cloudsso_20210515_models.GetUserMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.GetUserMFAAuthenticationSettingsResponse:
         """
-        This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
+        @summary Queries the multi-factor authentication (MFA) setting of a single user.
+        
+        @description This topic provides an example on how to query the MFA setting of the user named `u-00q8wbq42wiltcrk***`. The returned result shows that MFA is enabled for the user.
         
         @param request: GetUserMFAAuthenticationSettingsRequest
         @return: GetUserMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_mfaauthentication_settings_with_options_async(request, runtime)
 
     def get_user_provisioning_with_options(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.user_provisioning_id):
             query['UserProvisioningId'] = request.user_provisioning_id
         req = open_api_models.OpenApiRequest(
@@ -4174,14 +4825,21 @@
         )
 
     async def get_user_provisioning_with_options_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.user_provisioning_id):
             query['UserProvisioningId'] = request.user_provisioning_id
         req = open_api_models.OpenApiRequest(
@@ -4203,29 +4861,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_provisioning(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningRequest
+        @return: GetUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_provisioning_with_options(request, runtime)
 
     async def get_user_provisioning_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningRequest
+        @return: GetUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_provisioning_with_options_async(request, runtime)
 
     def get_user_provisioning_configuration_with_options(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningConfigurationResponse:
+        """
+        @summary Queries the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningConfigurationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningConfigurationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4246,14 +4923,21 @@
         )
 
     async def get_user_provisioning_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningConfigurationResponse:
+        """
+        @summary Queries the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningConfigurationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningConfigurationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4273,29 +4957,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_provisioning_configuration(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningConfigurationRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningConfigurationResponse:
+        """
+        @summary Queries the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningConfigurationRequest
+        @return: GetUserProvisioningConfigurationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_provisioning_configuration_with_options(request, runtime)
 
     async def get_user_provisioning_configuration_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningConfigurationRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningConfigurationResponse:
+        """
+        @summary Queries the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningConfigurationRequest
+        @return: GetUserProvisioningConfigurationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_provisioning_configuration_with_options_async(request, runtime)
 
     def get_user_provisioning_event_with_options(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningEventResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: GetUserProvisioningEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningEventResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.event_id):
             query['EventId'] = request.event_id
         req = open_api_models.OpenApiRequest(
@@ -4318,14 +5021,21 @@
         )
 
     async def get_user_provisioning_event_with_options_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningEventResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: GetUserProvisioningEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningEventResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.event_id):
             query['EventId'] = request.event_id
         req = open_api_models.OpenApiRequest(
@@ -4347,29 +5057,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_provisioning_event(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningEventRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningEventResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: GetUserProvisioningEventRequest
+        @return: GetUserProvisioningEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_provisioning_event_with_options(request, runtime)
 
     async def get_user_provisioning_event_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningEventRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningEventResponse:
+        """
+        @summary Queries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: GetUserProvisioningEventRequest
+        @return: GetUserProvisioningEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_provisioning_event_with_options_async(request, runtime)
 
     def get_user_provisioning_rd_account_statistics_with_options(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsResponse:
+        """
+        @summary Queries statistics of Resource Access Management (RAM) user provisioning events that are created for the member in a resource directory.
+        
+        @param request: GetUserProvisioningRdAccountStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningRdAccountStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.rd_member_id):
             query['RdMemberId'] = request.rd_member_id
         req = open_api_models.OpenApiRequest(
@@ -4392,14 +5121,21 @@
         )
 
     async def get_user_provisioning_rd_account_statistics_with_options_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsResponse:
+        """
+        @summary Queries statistics of Resource Access Management (RAM) user provisioning events that are created for the member in a resource directory.
+        
+        @param request: GetUserProvisioningRdAccountStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningRdAccountStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.rd_member_id):
             query['RdMemberId'] = request.rd_member_id
         req = open_api_models.OpenApiRequest(
@@ -4421,29 +5157,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_provisioning_rd_account_statistics(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsResponse:
+        """
+        @summary Queries statistics of Resource Access Management (RAM) user provisioning events that are created for the member in a resource directory.
+        
+        @param request: GetUserProvisioningRdAccountStatisticsRequest
+        @return: GetUserProvisioningRdAccountStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_provisioning_rd_account_statistics_with_options(request, runtime)
 
     async def get_user_provisioning_rd_account_statistics_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningRdAccountStatisticsResponse:
+        """
+        @summary Queries statistics of Resource Access Management (RAM) user provisioning events that are created for the member in a resource directory.
+        
+        @param request: GetUserProvisioningRdAccountStatisticsRequest
+        @return: GetUserProvisioningRdAccountStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_provisioning_rd_account_statistics_with_options_async(request, runtime)
 
     def get_user_provisioning_statistics_with_options(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningStatisticsResponse:
+        """
+        @summary Queries the statistics of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.user_provisioning_id):
             query['UserProvisioningId'] = request.user_provisioning_id
         req = open_api_models.OpenApiRequest(
@@ -4466,14 +5221,21 @@
         )
 
     async def get_user_provisioning_statistics_with_options_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.GetUserProvisioningStatisticsResponse:
+        """
+        @summary Queries the statistics of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserProvisioningStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.user_provisioning_id):
             query['UserProvisioningId'] = request.user_provisioning_id
         req = open_api_models.OpenApiRequest(
@@ -4495,31 +5257,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_provisioning_statistics(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningStatisticsRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningStatisticsResponse:
+        """
+        @summary Queries the statistics of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningStatisticsRequest
+        @return: GetUserProvisioningStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_provisioning_statistics_with_options(request, runtime)
 
     async def get_user_provisioning_statistics_async(
         self,
         request: cloudsso_20210515_models.GetUserProvisioningStatisticsRequest,
     ) -> cloudsso_20210515_models.GetUserProvisioningStatisticsResponse:
+        """
+        @summary Queries the statistics of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: GetUserProvisioningStatisticsRequest
+        @return: GetUserProvisioningStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_provisioning_statistics_with_options_async(request, runtime)
 
     def list_access_assignments_with_options(
         self,
         request: cloudsso_20210515_models.ListAccessAssignmentsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListAccessAssignmentsResponse:
         """
-        This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
+        @summary Queries the access permissions that are assigned.
+        
+        @description This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
         
         @param request: ListAccessAssignmentsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAccessAssignmentsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4560,15 +5336,17 @@
 
     async def list_access_assignments_with_options_async(
         self,
         request: cloudsso_20210515_models.ListAccessAssignmentsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListAccessAssignmentsResponse:
         """
-        This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
+        @summary Queries the access permissions that are assigned.
+        
+        @description This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
         
         @param request: ListAccessAssignmentsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAccessAssignmentsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4608,42 +5386,48 @@
         )
 
     def list_access_assignments(
         self,
         request: cloudsso_20210515_models.ListAccessAssignmentsRequest,
     ) -> cloudsso_20210515_models.ListAccessAssignmentsResponse:
         """
-        This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
+        @summary Queries the access permissions that are assigned.
+        
+        @description This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
         
         @param request: ListAccessAssignmentsRequest
         @return: ListAccessAssignmentsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_access_assignments_with_options(request, runtime)
 
     async def list_access_assignments_async(
         self,
         request: cloudsso_20210515_models.ListAccessAssignmentsRequest,
     ) -> cloudsso_20210515_models.ListAccessAssignmentsResponse:
         """
-        This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
+        @summary Queries the access permissions that are assigned.
+        
+        @description This topic provides an example on how to query the assigned access permissions on the account `114240524784***` in your resource directory. The returned result shows that access permissions on the account in your resource directory is assigned to one user.
         
         @param request: ListAccessAssignmentsRequest
         @return: ListAccessAssignmentsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_access_assignments_with_options_async(request, runtime)
 
     def list_access_configuration_provisionings_with_options(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationProvisioningsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListAccessConfigurationProvisioningsResponse:
         """
-        This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
+        @summary Queries the access configurations that are provisioned.
+        
+        @description This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
         
         @param request: ListAccessConfigurationProvisioningsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAccessConfigurationProvisioningsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4682,15 +5466,17 @@
 
     async def list_access_configuration_provisionings_with_options_async(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationProvisioningsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListAccessConfigurationProvisioningsResponse:
         """
-        This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
+        @summary Queries the access configurations that are provisioned.
+        
+        @description This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
         
         @param request: ListAccessConfigurationProvisioningsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAccessConfigurationProvisioningsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4728,42 +5514,48 @@
         )
 
     def list_access_configuration_provisionings(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationProvisioningsRequest,
     ) -> cloudsso_20210515_models.ListAccessConfigurationProvisioningsResponse:
         """
-        This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
+        @summary Queries the access configurations that are provisioned.
+        
+        @description This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
         
         @param request: ListAccessConfigurationProvisioningsRequest
         @return: ListAccessConfigurationProvisioningsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_access_configuration_provisionings_with_options(request, runtime)
 
     async def list_access_configuration_provisionings_async(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationProvisioningsRequest,
     ) -> cloudsso_20210515_models.ListAccessConfigurationProvisioningsResponse:
         """
-        This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
+        @summary Queries the access configurations that are provisioned.
+        
+        @description This topic provides an example on how to query the accounts for which the access permission `ac-00ccule7tadaijxc***` is provisioned. The returned result shows that the access configuration is provisioned for two accounts in your resource directory.
         
         @param request: ListAccessConfigurationProvisioningsRequest
         @return: ListAccessConfigurationProvisioningsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_access_configuration_provisionings_with_options_async(request, runtime)
 
     def list_access_configurations_with_options(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListAccessConfigurationsResponse:
         """
-        This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
+        @summary Queries access configurations.
+        
+        @description This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
         
         @param request: ListAccessConfigurationsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAccessConfigurationsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4798,15 +5590,17 @@
 
     async def list_access_configurations_with_options_async(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListAccessConfigurationsResponse:
         """
-        This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
+        @summary Queries access configurations.
+        
+        @description This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
         
         @param request: ListAccessConfigurationsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListAccessConfigurationsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4840,41 +5634,47 @@
         )
 
     def list_access_configurations(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationsRequest,
     ) -> cloudsso_20210515_models.ListAccessConfigurationsResponse:
         """
-        This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
+        @summary Queries access configurations.
+        
+        @description This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
         
         @param request: ListAccessConfigurationsRequest
         @return: ListAccessConfigurationsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_access_configurations_with_options(request, runtime)
 
     async def list_access_configurations_async(
         self,
         request: cloudsso_20210515_models.ListAccessConfigurationsRequest,
     ) -> cloudsso_20210515_models.ListAccessConfigurationsResponse:
         """
-        This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
+        @summary Queries access configurations.
+        
+        @description This topic provides an example on how to query the access configurations within the directory `d-00fc2p61***`. The returned result shows that the directory contains the `VPC-Admin` and `ECS-Admin` access configurations.
         
         @param request: ListAccessConfigurationsRequest
         @return: ListAccessConfigurationsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_access_configurations_with_options_async(request, runtime)
 
     def list_directories_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListDirectoriesResponse:
         """
-        This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
+        @summary Queries directories.
+        
+        @description This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
         
         @param request: ListDirectoriesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListDirectoriesResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -4894,15 +5694,17 @@
         )
 
     async def list_directories_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListDirectoriesResponse:
         """
-        This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
+        @summary Queries directories.
+        
+        @description This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
         
         @param request: ListDirectoriesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListDirectoriesResponse
         """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
@@ -4919,37 +5721,43 @@
         return TeaCore.from_map(
             cloudsso_20210515_models.ListDirectoriesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_directories(self) -> cloudsso_20210515_models.ListDirectoriesResponse:
         """
-        This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
+        @summary Queries directories.
+        
+        @description This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
         
         @return: ListDirectoriesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_directories_with_options(runtime)
 
     async def list_directories_async(self) -> cloudsso_20210515_models.ListDirectoriesResponse:
         """
-        This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
+        @summary Queries directories.
+        
+        @description This topic provides an example on how to query the directories within your Alibaba Cloud account. The returned result shows that only one directory with the ID `d-00fc2p61***` is created within your Alibaba Cloud account.
         
         @return: ListDirectoriesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_directories_with_options_async(runtime)
 
     def list_external_samlid_pcertificates_with_options(
         self,
         request: cloudsso_20210515_models.ListExternalSAMLIdPCertificatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListExternalSAMLIdPCertificatesResponse:
         """
-        This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
+        @summary Queries Security Assertion Markup Language (SAML) signing certificates.
+        
+        @description This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
         
         @param request: ListExternalSAMLIdPCertificatesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListExternalSAMLIdPCertificatesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4976,15 +5784,17 @@
 
     async def list_external_samlid_pcertificates_with_options_async(
         self,
         request: cloudsso_20210515_models.ListExternalSAMLIdPCertificatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListExternalSAMLIdPCertificatesResponse:
         """
-        This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
+        @summary Queries Security Assertion Markup Language (SAML) signing certificates.
+        
+        @description This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
         
         @param request: ListExternalSAMLIdPCertificatesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListExternalSAMLIdPCertificatesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5010,42 +5820,48 @@
         )
 
     def list_external_samlid_pcertificates(
         self,
         request: cloudsso_20210515_models.ListExternalSAMLIdPCertificatesRequest,
     ) -> cloudsso_20210515_models.ListExternalSAMLIdPCertificatesResponse:
         """
-        This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
+        @summary Queries Security Assertion Markup Language (SAML) signing certificates.
+        
+        @description This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
         
         @param request: ListExternalSAMLIdPCertificatesRequest
         @return: ListExternalSAMLIdPCertificatesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_external_samlid_pcertificates_with_options(request, runtime)
 
     async def list_external_samlid_pcertificates_async(
         self,
         request: cloudsso_20210515_models.ListExternalSAMLIdPCertificatesRequest,
     ) -> cloudsso_20210515_models.ListExternalSAMLIdPCertificatesResponse:
         """
-        This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
+        @summary Queries Security Assertion Markup Language (SAML) signing certificates.
+        
+        @description This topic provides an example on how to query the SAML signing certificates within the directory `d-00fc2p61***`. The returned result shows that the directory contains one SAML signing certificate.
         
         @param request: ListExternalSAMLIdPCertificatesRequest
         @return: ListExternalSAMLIdPCertificatesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_external_samlid_pcertificates_with_options_async(request, runtime)
 
     def list_group_members_with_options(
         self,
         request: cloudsso_20210515_models.ListGroupMembersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListGroupMembersResponse:
         """
-        This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
+        @summary Queries the users in a group.
+        
+        @description This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
         
         @param request: ListGroupMembersRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListGroupMembersResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5078,15 +5894,17 @@
 
     async def list_group_members_with_options_async(
         self,
         request: cloudsso_20210515_models.ListGroupMembersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListGroupMembersResponse:
         """
-        This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
+        @summary Queries the users in a group.
+        
+        @description This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
         
         @param request: ListGroupMembersRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListGroupMembersResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5118,42 +5936,48 @@
         )
 
     def list_group_members(
         self,
         request: cloudsso_20210515_models.ListGroupMembersRequest,
     ) -> cloudsso_20210515_models.ListGroupMembersResponse:
         """
-        This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
+        @summary Queries the users in a group.
+        
+        @description This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
         
         @param request: ListGroupMembersRequest
         @return: ListGroupMembersResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_group_members_with_options(request, runtime)
 
     async def list_group_members_async(
         self,
         request: cloudsso_20210515_models.ListGroupMembersRequest,
     ) -> cloudsso_20210515_models.ListGroupMembersResponse:
         """
-        This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
+        @summary Queries the users in a group.
+        
+        @description This topic provides an example on how to query the users in the group `g-00jqzghi2n3o5hkh***`. The returned result shows that the group contains the user `Alice` and the user `user1`.
         
         @param request: ListGroupMembersRequest
         @return: ListGroupMembersResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_group_members_with_options_async(request, runtime)
 
     def list_groups_with_options(
         self,
         request: cloudsso_20210515_models.ListGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListGroupsResponse:
         """
-        This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
+        @summary Queries groups.
+        
+        @description This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
         
         @param request: ListGroupsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListGroupsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5188,15 +6012,17 @@
 
     async def list_groups_with_options_async(
         self,
         request: cloudsso_20210515_models.ListGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListGroupsResponse:
         """
-        This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
+        @summary Queries groups.
+        
+        @description This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
         
         @param request: ListGroupsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListGroupsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5230,42 +6056,48 @@
         )
 
     def list_groups(
         self,
         request: cloudsso_20210515_models.ListGroupsRequest,
     ) -> cloudsso_20210515_models.ListGroupsResponse:
         """
-        This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
+        @summary Queries groups.
+        
+        @description This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
         
         @param request: ListGroupsRequest
         @return: ListGroupsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_groups_with_options(request, runtime)
 
     async def list_groups_async(
         self,
         request: cloudsso_20210515_models.ListGroupsRequest,
     ) -> cloudsso_20210515_models.ListGroupsResponse:
         """
-        This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
+        @summary Queries groups.
+        
+        @description This topic provides an example on how to query the groups in the directory `d-00fc2p61***`. The returned result shows that the directory contains three groups. The groups `group1` and `group2` are synchronized from an external identity provider (IdP). The group `TestGroup` is manually created in CloudSSO.
         
         @param request: ListGroupsRequest
         @return: ListGroupsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_groups_with_options_async(request, runtime)
 
     def list_joined_groups_for_user_with_options(
         self,
         request: cloudsso_20210515_models.ListJoinedGroupsForUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListJoinedGroupsForUserResponse:
         """
-        This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
+        @summary Queries the groups to which a user is added.
+        
+        @description This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
         
         @param request: ListJoinedGroupsForUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListJoinedGroupsForUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5298,15 +6130,17 @@
 
     async def list_joined_groups_for_user_with_options_async(
         self,
         request: cloudsso_20210515_models.ListJoinedGroupsForUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListJoinedGroupsForUserResponse:
         """
-        This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
+        @summary Queries the groups to which a user is added.
+        
+        @description This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
         
         @param request: ListJoinedGroupsForUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListJoinedGroupsForUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5338,42 +6172,48 @@
         )
 
     def list_joined_groups_for_user(
         self,
         request: cloudsso_20210515_models.ListJoinedGroupsForUserRequest,
     ) -> cloudsso_20210515_models.ListJoinedGroupsForUserResponse:
         """
-        This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
+        @summary Queries the groups to which a user is added.
+        
+        @description This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
         
         @param request: ListJoinedGroupsForUserRequest
         @return: ListJoinedGroupsForUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_joined_groups_for_user_with_options(request, runtime)
 
     async def list_joined_groups_for_user_async(
         self,
         request: cloudsso_20210515_models.ListJoinedGroupsForUserRequest,
     ) -> cloudsso_20210515_models.ListJoinedGroupsForUserResponse:
         """
-        This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
+        @summary Queries the groups to which a user is added.
+        
+        @description This topic provides an example on how to query the groups to which the user `u-00q8wbq42wiltcrk***` is added. The returned result shows that the user is added to both the `TestGroup` and the `group1` groups.
         
         @param request: ListJoinedGroupsForUserRequest
         @return: ListJoinedGroupsForUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_joined_groups_for_user_with_options_async(request, runtime)
 
     def list_mfadevices_for_user_with_options(
         self,
         request: cloudsso_20210515_models.ListMFADevicesForUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListMFADevicesForUserResponse:
         """
-        This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
+        @summary Queries the multi-factor authentication (MFA) devices that are bound to a user. Up to two MFA devices can be bound to a user.
+        
+        @description This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
         
         @param request: ListMFADevicesForUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListMFADevicesForUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5402,15 +6242,17 @@
 
     async def list_mfadevices_for_user_with_options_async(
         self,
         request: cloudsso_20210515_models.ListMFADevicesForUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListMFADevicesForUserResponse:
         """
-        This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
+        @summary Queries the multi-factor authentication (MFA) devices that are bound to a user. Up to two MFA devices can be bound to a user.
+        
+        @description This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
         
         @param request: ListMFADevicesForUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListMFADevicesForUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5438,42 +6280,48 @@
         )
 
     def list_mfadevices_for_user(
         self,
         request: cloudsso_20210515_models.ListMFADevicesForUserRequest,
     ) -> cloudsso_20210515_models.ListMFADevicesForUserResponse:
         """
-        This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
+        @summary Queries the multi-factor authentication (MFA) devices that are bound to a user. Up to two MFA devices can be bound to a user.
+        
+        @description This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
         
         @param request: ListMFADevicesForUserRequest
         @return: ListMFADevicesForUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_mfadevices_for_user_with_options(request, runtime)
 
     async def list_mfadevices_for_user_async(
         self,
         request: cloudsso_20210515_models.ListMFADevicesForUserRequest,
     ) -> cloudsso_20210515_models.ListMFADevicesForUserResponse:
         """
-        This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
+        @summary Queries the multi-factor authentication (MFA) devices that are bound to a user. Up to two MFA devices can be bound to a user.
+        
+        @description This topic provides an example on how to query the MFA devices that are bound to the user `u-00q8wbq42wiltcrk***`. The returned result shows that the MFA device named `Alice-MFA1` is bound to the user.
         
         @param request: ListMFADevicesForUserRequest
         @return: ListMFADevicesForUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_mfadevices_for_user_with_options_async(request, runtime)
 
     def list_permission_policies_in_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
+        @summary Queries the policies that are created for an access configuration.
+        
+        @description This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
         
         @param request: ListPermissionPoliciesInAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListPermissionPoliciesInAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5504,15 +6352,17 @@
 
     async def list_permission_policies_in_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
+        @summary Queries the policies that are created for an access configuration.
+        
+        @description This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
         
         @param request: ListPermissionPoliciesInAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListPermissionPoliciesInAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5542,42 +6392,48 @@
         )
 
     def list_permission_policies_in_access_configuration(
         self,
         request: cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
+        @summary Queries the policies that are created for an access configuration.
+        
+        @description This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
         
         @param request: ListPermissionPoliciesInAccessConfigurationRequest
         @return: ListPermissionPoliciesInAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_permission_policies_in_access_configuration_with_options(request, runtime)
 
     async def list_permission_policies_in_access_configuration_async(
         self,
         request: cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.ListPermissionPoliciesInAccessConfigurationResponse:
         """
-        This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
+        @summary Queries the policies that are created for an access configuration.
+        
+        @description This topic provides an example on how to query the policies that are created for the access configuration `ac-00jhtfl8thteu6uj***`. The returned result shows that the access configuration contains one system policy and one inline policy.
         
         @param request: ListPermissionPoliciesInAccessConfigurationRequest
         @return: ListPermissionPoliciesInAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_permission_policies_in_access_configuration_with_options_async(request, runtime)
 
     def list_scimserver_credentials_with_options(
         self,
         request: cloudsso_20210515_models.ListSCIMServerCredentialsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListSCIMServerCredentialsResponse:
         """
-        This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
+        @summary Queries Cross-domain Identity Management (SCIM) credentials.
+        
+        @description This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
         
         @param request: ListSCIMServerCredentialsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListSCIMServerCredentialsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5604,15 +6460,17 @@
 
     async def list_scimserver_credentials_with_options_async(
         self,
         request: cloudsso_20210515_models.ListSCIMServerCredentialsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListSCIMServerCredentialsResponse:
         """
-        This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
+        @summary Queries Cross-domain Identity Management (SCIM) credentials.
+        
+        @description This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
         
         @param request: ListSCIMServerCredentialsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListSCIMServerCredentialsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5638,42 +6496,48 @@
         )
 
     def list_scimserver_credentials(
         self,
         request: cloudsso_20210515_models.ListSCIMServerCredentialsRequest,
     ) -> cloudsso_20210515_models.ListSCIMServerCredentialsResponse:
         """
-        This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
+        @summary Queries Cross-domain Identity Management (SCIM) credentials.
+        
+        @description This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
         
         @param request: ListSCIMServerCredentialsRequest
         @return: ListSCIMServerCredentialsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_scimserver_credentials_with_options(request, runtime)
 
     async def list_scimserver_credentials_async(
         self,
         request: cloudsso_20210515_models.ListSCIMServerCredentialsRequest,
     ) -> cloudsso_20210515_models.ListSCIMServerCredentialsResponse:
         """
-        This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
+        @summary Queries Cross-domain Identity Management (SCIM) credentials.
+        
+        @description This topic provides an example on how to query the SCIM credentials within the `d-00fc2p61***` directory.
         
         @param request: ListSCIMServerCredentialsRequest
         @return: ListSCIMServerCredentialsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_scimserver_credentials_with_options_async(request, runtime)
 
     def list_tasks_with_options(
         self,
         request: cloudsso_20210515_models.ListTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListTasksResponse:
         """
-        By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
+        @summary Queries asynchronous tasks.
+        
+        @description By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
         This topic provides an example on how to query the tasks within the previous 24 hours.
         
         @param request: ListTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTasksResponse
         """
         UtilClient.validate_model(request)
@@ -5721,15 +6585,17 @@
 
     async def list_tasks_with_options_async(
         self,
         request: cloudsso_20210515_models.ListTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListTasksResponse:
         """
-        By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
+        @summary Queries asynchronous tasks.
+        
+        @description By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
         This topic provides an example on how to query the tasks within the previous 24 hours.
         
         @param request: ListTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTasksResponse
         """
         UtilClient.validate_model(request)
@@ -5776,42 +6642,53 @@
         )
 
     def list_tasks(
         self,
         request: cloudsso_20210515_models.ListTasksRequest,
     ) -> cloudsso_20210515_models.ListTasksResponse:
         """
-        By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
+        @summary Queries asynchronous tasks.
+        
+        @description By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
         This topic provides an example on how to query the tasks within the previous 24 hours.
         
         @param request: ListTasksRequest
         @return: ListTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_tasks_with_options(request, runtime)
 
     async def list_tasks_async(
         self,
         request: cloudsso_20210515_models.ListTasksRequest,
     ) -> cloudsso_20210515_models.ListTasksResponse:
         """
-        By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
+        @summary Queries asynchronous tasks.
+        
+        @description By default, this operation queries the tasks within the previous 24 hours. This operation allows you to query the tasks within a maximum of 7 days. You can specify the start time of the query by using `Filter`.
         This topic provides an example on how to query the tasks within the previous 24 hours.
         
         @param request: ListTasksRequest
         @return: ListTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_tasks_with_options_async(request, runtime)
 
     def list_user_provisioning_events_with_options(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningEventsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListUserProvisioningEventsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisioning events.
+        
+        @param request: ListUserProvisioningEventsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserProvisioningEventsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -5838,14 +6715,21 @@
         )
 
     async def list_user_provisioning_events_with_options_async(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningEventsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListUserProvisioningEventsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisioning events.
+        
+        @param request: ListUserProvisioningEventsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserProvisioningEventsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -5871,29 +6755,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_user_provisioning_events(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningEventsRequest,
     ) -> cloudsso_20210515_models.ListUserProvisioningEventsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisioning events.
+        
+        @param request: ListUserProvisioningEventsRequest
+        @return: ListUserProvisioningEventsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_user_provisioning_events_with_options(request, runtime)
 
     async def list_user_provisioning_events_async(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningEventsRequest,
     ) -> cloudsso_20210515_models.ListUserProvisioningEventsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisioning events.
+        
+        @param request: ListUserProvisioningEventsRequest
+        @return: ListUserProvisioningEventsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_provisioning_events_with_options_async(request, runtime)
 
     def list_user_provisionings_with_options(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListUserProvisioningsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisionings.
+        
+        @param request: ListUserProvisioningsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserProvisioningsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -5926,14 +6829,21 @@
         )
 
     async def list_user_provisionings_with_options_async(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListUserProvisioningsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisionings.
+        
+        @param request: ListUserProvisioningsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserProvisioningsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
@@ -5965,31 +6875,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_user_provisionings(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningsRequest,
     ) -> cloudsso_20210515_models.ListUserProvisioningsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisionings.
+        
+        @param request: ListUserProvisioningsRequest
+        @return: ListUserProvisioningsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_user_provisionings_with_options(request, runtime)
 
     async def list_user_provisionings_async(
         self,
         request: cloudsso_20210515_models.ListUserProvisioningsRequest,
     ) -> cloudsso_20210515_models.ListUserProvisioningsResponse:
+        """
+        @summary Queries Resource Access Management (RAM) user provisionings.
+        
+        @param request: ListUserProvisioningsRequest
+        @return: ListUserProvisioningsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_provisionings_with_options_async(request, runtime)
 
     def list_users_with_options(
         self,
         request: cloudsso_20210515_models.ListUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListUsersResponse:
         """
-        This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
+        @summary Queries users.
+        
+        @description This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
         
         @param request: ListUsersRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListUsersResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6026,15 +6950,17 @@
 
     async def list_users_with_options_async(
         self,
         request: cloudsso_20210515_models.ListUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ListUsersResponse:
         """
-        This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
+        @summary Queries users.
+        
+        @description This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
         
         @param request: ListUsersRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListUsersResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6070,43 +6996,49 @@
         )
 
     def list_users(
         self,
         request: cloudsso_20210515_models.ListUsersRequest,
     ) -> cloudsso_20210515_models.ListUsersResponse:
         """
-        This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
+        @summary Queries users.
+        
+        @description This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
         
         @param request: ListUsersRequest
         @return: ListUsersResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_users_with_options(request, runtime)
 
     async def list_users_async(
         self,
         request: cloudsso_20210515_models.ListUsersRequest,
     ) -> cloudsso_20210515_models.ListUsersResponse:
         """
-        This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
+        @summary Queries users.
+        
+        @description This topic provides an example on how to query users in the `d-00fc2p61***` directory. The returned result shows that the directory contains two users. The user `AliceLee` is synchronized from an external identity provider (IdP). The user `user1` is manually created within CloudSSO.
         
         @param request: ListUsersRequest
         @return: ListUsersResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_users_with_options_async(request, runtime)
 
     def provision_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.ProvisionAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ProvisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj****` for the account `114240524784****` in your resource directory.
+        @summary Provisions an access configuration for an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj***` for the account `114240524784****` in your resource directory.
         
         @param request: ProvisionAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ProvisionAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6139,16 +7071,18 @@
 
     async def provision_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.ProvisionAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ProvisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj****` for the account `114240524784****` in your resource directory.
+        @summary Provisions an access configuration for an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj***` for the account `114240524784****` in your resource directory.
         
         @param request: ProvisionAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ProvisionAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6180,44 +7114,50 @@
         )
 
     def provision_access_configuration(
         self,
         request: cloudsso_20210515_models.ProvisionAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.ProvisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj****` for the account `114240524784****` in your resource directory.
+        @summary Provisions an access configuration for an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj***` for the account `114240524784****` in your resource directory.
         
         @param request: ProvisionAccessConfigurationRequest
         @return: ProvisionAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.provision_access_configuration_with_options(request, runtime)
 
     async def provision_access_configuration_async(
         self,
         request: cloudsso_20210515_models.ProvisionAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.ProvisionAccessConfigurationResponse:
         """
-        When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](~~340670~~) operation to query the progress of the task based on the value of the `TaskId` response parameter.
-        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj****` for the account `114240524784****` in your resource directory.
+        @summary Provisions an access configuration for an account in your resource directory.
+        
+        @description When you call this operation, an asynchronous task is automatically created. You can call the [GetTask](https://help.aliyun.com/document_detail/340670.html) operation to query the progress of the task based on the value of the `TaskId` response parameter.
+        This topic provides an example on how to provision the access configuration `ac-00jhtfl8thteu6uj***` for the account `114240524784****` in your resource directory.
         
         @param request: ProvisionAccessConfigurationRequest
         @return: ProvisionAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.provision_access_configuration_with_options_async(request, runtime)
 
     def remove_external_samlid_pcertificate_with_options(
         self,
         request: cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateResponse:
         """
-        This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
+        @summary Removes a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
         
         @param request: RemoveExternalSAMLIdPCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemoveExternalSAMLIdPCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6246,15 +7186,17 @@
 
     async def remove_external_samlid_pcertificate_with_options_async(
         self,
         request: cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateResponse:
         """
-        This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
+        @summary Removes a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
         
         @param request: RemoveExternalSAMLIdPCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemoveExternalSAMLIdPCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6282,43 +7224,49 @@
         )
 
     def remove_external_samlid_pcertificate(
         self,
         request: cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateRequest,
     ) -> cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateResponse:
         """
-        This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
+        @summary Removes a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
         
         @param request: RemoveExternalSAMLIdPCertificateRequest
         @return: RemoveExternalSAMLIdPCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.remove_external_samlid_pcertificate_with_options(request, runtime)
 
     async def remove_external_samlid_pcertificate_async(
         self,
         request: cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateRequest,
     ) -> cloudsso_20210515_models.RemoveExternalSAMLIdPCertificateResponse:
         """
-        This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
+        @summary Removes a Security Assertion Markup Language (SAML) signing certificate.
+        
+        @description This topic provides an example on how to remove the SAML signing certificate whose ID is `idp-c-00dt9gnl7fmjaw9c***`.
         
         @param request: RemoveExternalSAMLIdPCertificateRequest
         @return: RemoveExternalSAMLIdPCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.remove_external_samlid_pcertificate_with_options_async(request, runtime)
 
     def remove_permission_policy_from_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationResponse:
         """
-        After you remove an inline policy from an access configuration, the policy cannot be restored.
-        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes a policy from an access configuration.
+        
+        @description After you remove an inline policy from an access configuration, the policy cannot be restored.
+        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: RemovePermissionPolicyFromAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemovePermissionPolicyFromAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6351,16 +7299,18 @@
 
     async def remove_permission_policy_from_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationResponse:
         """
-        After you remove an inline policy from an access configuration, the policy cannot be restored.
-        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes a policy from an access configuration.
+        
+        @description After you remove an inline policy from an access configuration, the policy cannot be restored.
+        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: RemovePermissionPolicyFromAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemovePermissionPolicyFromAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6392,45 +7342,51 @@
         )
 
     def remove_permission_policy_from_access_configuration(
         self,
         request: cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationResponse:
         """
-        After you remove an inline policy from an access configuration, the policy cannot be restored.
-        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes a policy from an access configuration.
+        
+        @description After you remove an inline policy from an access configuration, the policy cannot be restored.
+        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: RemovePermissionPolicyFromAccessConfigurationRequest
         @return: RemovePermissionPolicyFromAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.remove_permission_policy_from_access_configuration_with_options(request, runtime)
 
     async def remove_permission_policy_from_access_configuration_async(
         self,
         request: cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.RemovePermissionPolicyFromAccessConfigurationResponse:
         """
-        After you remove an inline policy from an access configuration, the policy cannot be restored.
-        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj****`.
+        @summary Removes a policy from an access configuration.
+        
+        @description After you remove an inline policy from an access configuration, the policy cannot be restored.
+        This topic provides an example on how to remove the system policy `AliyunECSFullAccess` from the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: RemovePermissionPolicyFromAccessConfigurationRequest
         @return: RemovePermissionPolicyFromAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.remove_permission_policy_from_access_configuration_with_options_async(request, runtime)
 
     def remove_user_from_group_with_options(
         self,
         request: cloudsso_20210515_models.RemoveUserFromGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RemoveUserFromGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
-        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk****` from the group `g-00jqzghi2n3o5hkh****`.
+        @summary Removes a user from a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
+        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk***` from the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: RemoveUserFromGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemoveUserFromGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6461,16 +7417,18 @@
 
     async def remove_user_from_group_with_options_async(
         self,
         request: cloudsso_20210515_models.RemoveUserFromGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RemoveUserFromGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
-        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk****` from the group `g-00jqzghi2n3o5hkh****`.
+        @summary Removes a user from a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
+        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk***` from the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: RemoveUserFromGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemoveUserFromGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6500,46 +7458,52 @@
         )
 
     def remove_user_from_group(
         self,
         request: cloudsso_20210515_models.RemoveUserFromGroupRequest,
     ) -> cloudsso_20210515_models.RemoveUserFromGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
-        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk****` from the group `g-00jqzghi2n3o5hkh****`.
+        @summary Removes a user from a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
+        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk***` from the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: RemoveUserFromGroupRequest
         @return: RemoveUserFromGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.remove_user_from_group_with_options(request, runtime)
 
     async def remove_user_from_group_async(
         self,
         request: cloudsso_20210515_models.RemoveUserFromGroupRequest,
     ) -> cloudsso_20210515_models.RemoveUserFromGroupResponse:
         """
-        If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
-        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk****` from the group `g-00jqzghi2n3o5hkh****`.
+        @summary Removes a user from a group.
+        
+        @description If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot remove a user from a group that is synchronized by using SCIM.
+        This topic provides an example on how to remove the user `u-00q8wbq42wiltcrk***` from the group `g-00jqzghi2n3o5hkh****`.
         
         @param request: RemoveUserFromGroupRequest
         @return: RemoveUserFromGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.remove_user_from_group_with_options_async(request, runtime)
 
     def reset_user_password_with_options(
         self,
         request: cloudsso_20210515_models.ResetUserPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ResetUserPasswordResponse:
         """
-        If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
+        @summary Resets the password of a user.
+        
+        @description If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
         >  After you enable SSO logon, your password cannot be reset.
-        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk****`. The new password is automatically generated by the system.
+        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk***`. The new password is automatically generated by the system.
         
         @param request: ResetUserPasswordRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetUserPasswordResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6574,17 +7538,19 @@
 
     async def reset_user_password_with_options_async(
         self,
         request: cloudsso_20210515_models.ResetUserPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.ResetUserPasswordResponse:
         """
-        If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
+        @summary Resets the password of a user.
+        
+        @description If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
         >  After you enable SSO logon, your password cannot be reset.
-        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk****`. The new password is automatically generated by the system.
+        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk***`. The new password is automatically generated by the system.
         
         @param request: ResetUserPasswordRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetUserPasswordResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6618,44 +7584,55 @@
         )
 
     def reset_user_password(
         self,
         request: cloudsso_20210515_models.ResetUserPasswordRequest,
     ) -> cloudsso_20210515_models.ResetUserPasswordResponse:
         """
-        If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
+        @summary Resets the password of a user.
+        
+        @description If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
         >  After you enable SSO logon, your password cannot be reset.
-        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk****`. The new password is automatically generated by the system.
+        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk***`. The new password is automatically generated by the system.
         
         @param request: ResetUserPasswordRequest
         @return: ResetUserPasswordResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.reset_user_password_with_options(request, runtime)
 
     async def reset_user_password_async(
         self,
         request: cloudsso_20210515_models.ResetUserPasswordRequest,
     ) -> cloudsso_20210515_models.ResetUserPasswordResponse:
         """
-        If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
+        @summary Resets the password of a user.
+        
+        @description If you forget your password or your password expires or is at risk, you must contact a CloudSSO administrator to reset your password.
         >  After you enable SSO logon, your password cannot be reset.
-        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk****`. The new password is automatically generated by the system.
+        This topic provides an example on how to reset the password of the user `u-00q8wbq42wiltcrk***`. The new password is automatically generated by the system.
         
         @param request: ResetUserPasswordRequest
         @return: ResetUserPasswordResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.reset_user_password_with_options_async(request, runtime)
 
     def retry_user_provisioning_event_with_options(
         self,
         request: cloudsso_20210515_models.RetryUserProvisioningEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RetryUserProvisioningEventResponse:
+        """
+        @summary Retries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: RetryUserProvisioningEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RetryUserProvisioningEventResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.duplication_strategy):
             query['DuplicationStrategy'] = request.duplication_strategy
         if not UtilClient.is_unset(request.event_id):
@@ -6680,14 +7657,21 @@
         )
 
     async def retry_user_provisioning_event_with_options_async(
         self,
         request: cloudsso_20210515_models.RetryUserProvisioningEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.RetryUserProvisioningEventResponse:
+        """
+        @summary Retries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: RetryUserProvisioningEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RetryUserProvisioningEventResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.duplication_strategy):
             query['DuplicationStrategy'] = request.duplication_strategy
         if not UtilClient.is_unset(request.event_id):
@@ -6711,39 +7695,53 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def retry_user_provisioning_event(
         self,
         request: cloudsso_20210515_models.RetryUserProvisioningEventRequest,
     ) -> cloudsso_20210515_models.RetryUserProvisioningEventResponse:
+        """
+        @summary Retries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: RetryUserProvisioningEventRequest
+        @return: RetryUserProvisioningEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.retry_user_provisioning_event_with_options(request, runtime)
 
     async def retry_user_provisioning_event_async(
         self,
         request: cloudsso_20210515_models.RetryUserProvisioningEventRequest,
     ) -> cloudsso_20210515_models.RetryUserProvisioningEventResponse:
+        """
+        @summary Retries a Resource Access Management (RAM) user provisioning event.
+        
+        @param request: RetryUserProvisioningEventRequest
+        @return: RetryUserProvisioningEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.retry_user_provisioning_event_with_options_async(request, runtime)
 
     def set_external_samlidentity_provider_with_options(
         self,
         request: cloudsso_20210515_models.SetExternalSAMLIdentityProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetExternalSAMLIdentityProviderResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
+        @summary Configures a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
         You can use one of the following methods to configure a SAML IdP. You can obtain the required metadata file or parameter values from your IdP.
-        *   Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
-        *   Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
+        Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
+        Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
         If you have configured a SAML IdP, the existing configurations are replaced after you call this operation.
-        *   If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
-        *   If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
+        If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
+        If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
         >  If SSO logon is enabled, new configurations immediately take effect. Take note of the impacts on the production environment.
-        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61****`.
+        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61***`.
         
         @param request: SetExternalSAMLIdentityProviderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetExternalSAMLIdentityProviderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6782,23 +7780,25 @@
 
     async def set_external_samlidentity_provider_with_options_async(
         self,
         request: cloudsso_20210515_models.SetExternalSAMLIdentityProviderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetExternalSAMLIdentityProviderResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
+        @summary Configures a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
         You can use one of the following methods to configure a SAML IdP. You can obtain the required metadata file or parameter values from your IdP.
-        *   Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
-        *   Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
+        Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
+        Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
         If you have configured a SAML IdP, the existing configurations are replaced after you call this operation.
-        *   If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
-        *   If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
+        If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
+        If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
         >  If SSO logon is enabled, new configurations immediately take effect. Take note of the impacts on the production environment.
-        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61****`.
+        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61***`.
         
         @param request: SetExternalSAMLIdentityProviderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetExternalSAMLIdentityProviderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6836,56 +7836,67 @@
         )
 
     def set_external_samlidentity_provider(
         self,
         request: cloudsso_20210515_models.SetExternalSAMLIdentityProviderRequest,
     ) -> cloudsso_20210515_models.SetExternalSAMLIdentityProviderResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
+        @summary Configures a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
         You can use one of the following methods to configure a SAML IdP. You can obtain the required metadata file or parameter values from your IdP.
-        *   Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
-        *   Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
+        Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
+        Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
         If you have configured a SAML IdP, the existing configurations are replaced after you call this operation.
-        *   If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
-        *   If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
+        If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
+        If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
         >  If SSO logon is enabled, new configurations immediately take effect. Take note of the impacts on the production environment.
-        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61****`.
+        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61***`.
         
         @param request: SetExternalSAMLIdentityProviderRequest
         @return: SetExternalSAMLIdentityProviderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_external_samlidentity_provider_with_options(request, runtime)
 
     async def set_external_samlidentity_provider_async(
         self,
         request: cloudsso_20210515_models.SetExternalSAMLIdentityProviderRequest,
     ) -> cloudsso_20210515_models.SetExternalSAMLIdentityProviderResponse:
         """
-        During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
+        @summary Configures a Security Assertion Markup Language (SAML) identity provider (IdP).
+        
+        @description During SAML 2.0-based single sign-on (SSO) logon, CloudSSO is an SP, and the identity management system of an enterprise is an IdP.
         You can use one of the following methods to configure a SAML IdP. You can obtain the required metadata file or parameter values from your IdP.
-        *   Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
-        *   Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
+        Use the metadata file. You can specify the `EncodedMetadataDocument` parameter to upload the metadata file.
+        Manually configure the IdP. You can manually specify the following parameters for your IdP: `EntityId`, `LoginUrl`, `WantRequestSigned`, and `X509Certificate`.
         If you have configured a SAML IdP, the existing configurations are replaced after you call this operation.
-        *   If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
-        *   If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
+        If the IdP is configured by using the metadata file, all existing configurations are replaced with new configurations.
+        If the IdP is manually configured, the original parameter values that are different from the new parameter values are replaced.
         >  If SSO logon is enabled, new configurations immediately take effect. Take note of the impacts on the production environment.
-        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61****`.
+        This topic provides an example on how to configure an IdP by using the metadata file within the directory `d-00fc2p61***`.
         
         @param request: SetExternalSAMLIdentityProviderRequest
         @return: SetExternalSAMLIdentityProviderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_external_samlidentity_provider_with_options_async(request, runtime)
 
     def set_login_preference_with_options(
         self,
         request: cloudsso_20210515_models.SetLoginPreferenceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetLoginPreferenceResponse:
+        """
+        @summary Configures the logon preference of CloudSSO users.
+        
+        @param request: SetLoginPreferenceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetLoginPreferenceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.login_network_masks):
             query['LoginNetworkMasks'] = request.login_network_masks
         req = open_api_models.OpenApiRequest(
@@ -6908,14 +7919,21 @@
         )
 
     async def set_login_preference_with_options_async(
         self,
         request: cloudsso_20210515_models.SetLoginPreferenceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetLoginPreferenceResponse:
+        """
+        @summary Configures the logon preference of CloudSSO users.
+        
+        @param request: SetLoginPreferenceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetLoginPreferenceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.login_network_masks):
             query['LoginNetworkMasks'] = request.login_network_masks
         req = open_api_models.OpenApiRequest(
@@ -6937,31 +7955,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_login_preference(
         self,
         request: cloudsso_20210515_models.SetLoginPreferenceRequest,
     ) -> cloudsso_20210515_models.SetLoginPreferenceResponse:
+        """
+        @summary Configures the logon preference of CloudSSO users.
+        
+        @param request: SetLoginPreferenceRequest
+        @return: SetLoginPreferenceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_login_preference_with_options(request, runtime)
 
     async def set_login_preference_async(
         self,
         request: cloudsso_20210515_models.SetLoginPreferenceRequest,
     ) -> cloudsso_20210515_models.SetLoginPreferenceResponse:
+        """
+        @summary Configures the logon preference of CloudSSO users.
+        
+        @param request: SetLoginPreferenceRequest
+        @return: SetLoginPreferenceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_login_preference_with_options_async(request, runtime)
 
     def set_mfaauthentication_status_with_options(
         self,
         request: cloudsso_20210515_models.SetMFAAuthenticationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetMFAAuthenticationStatusResponse:
         """
-        If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
+        @summary Enables or disables multi-factor authentication (MFA) for users in a directory.
+        
+        @description If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
         This topic provides an example on how to enable MFA for users.
         
         @param request: SetMFAAuthenticationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetMFAAuthenticationStatusResponse
         """
         UtilClient.validate_model(request)
@@ -6991,15 +8023,17 @@
 
     async def set_mfaauthentication_status_with_options_async(
         self,
         request: cloudsso_20210515_models.SetMFAAuthenticationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetMFAAuthenticationStatusResponse:
         """
-        If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
+        @summary Enables or disables multi-factor authentication (MFA) for users in a directory.
+        
+        @description If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
         This topic provides an example on how to enable MFA for users.
         
         @param request: SetMFAAuthenticationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetMFAAuthenticationStatusResponse
         """
         UtilClient.validate_model(request)
@@ -7028,42 +8062,53 @@
         )
 
     def set_mfaauthentication_status(
         self,
         request: cloudsso_20210515_models.SetMFAAuthenticationStatusRequest,
     ) -> cloudsso_20210515_models.SetMFAAuthenticationStatusResponse:
         """
-        If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
+        @summary Enables or disables multi-factor authentication (MFA) for users in a directory.
+        
+        @description If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
         This topic provides an example on how to enable MFA for users.
         
         @param request: SetMFAAuthenticationStatusRequest
         @return: SetMFAAuthenticationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_mfaauthentication_status_with_options(request, runtime)
 
     async def set_mfaauthentication_status_async(
         self,
         request: cloudsso_20210515_models.SetMFAAuthenticationStatusRequest,
     ) -> cloudsso_20210515_models.SetMFAAuthenticationStatusResponse:
         """
-        If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
+        @summary Enables or disables multi-factor authentication (MFA) for users in a directory.
+        
+        @description If a CloudSSO administrator enables username-password logon for users, CloudSSO automatically enables MFA to improve security. The administrator can call this operation to enable or disable MFA based on the business requirements.
         This topic provides an example on how to enable MFA for users.
         
         @param request: SetMFAAuthenticationStatusRequest
         @return: SetMFAAuthenticationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_mfaauthentication_status_with_options_async(request, runtime)
 
     def set_password_policy_with_options(
         self,
         request: cloudsso_20210515_models.SetPasswordPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetPasswordPolicyResponse:
+        """
+        @summary Configures a password policy for CloudSSO users.
+        
+        @param request: SetPasswordPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetPasswordPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.max_login_attempts):
             query['MaxLoginAttempts'] = request.max_login_attempts
         if not UtilClient.is_unset(request.max_password_age):
@@ -7096,14 +8141,21 @@
         )
 
     async def set_password_policy_with_options_async(
         self,
         request: cloudsso_20210515_models.SetPasswordPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetPasswordPolicyResponse:
+        """
+        @summary Configures a password policy for CloudSSO users.
+        
+        @param request: SetPasswordPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SetPasswordPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.max_login_attempts):
             query['MaxLoginAttempts'] = request.max_login_attempts
         if not UtilClient.is_unset(request.max_password_age):
@@ -7135,34 +8187,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def set_password_policy(
         self,
         request: cloudsso_20210515_models.SetPasswordPolicyRequest,
     ) -> cloudsso_20210515_models.SetPasswordPolicyResponse:
+        """
+        @summary Configures a password policy for CloudSSO users.
+        
+        @param request: SetPasswordPolicyRequest
+        @return: SetPasswordPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.set_password_policy_with_options(request, runtime)
 
     async def set_password_policy_async(
         self,
         request: cloudsso_20210515_models.SetPasswordPolicyRequest,
     ) -> cloudsso_20210515_models.SetPasswordPolicyResponse:
+        """
+        @summary Configures a password policy for CloudSSO users.
+        
+        @param request: SetPasswordPolicyRequest
+        @return: SetPasswordPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.set_password_policy_with_options_async(request, runtime)
 
     def set_scimsynchronization_status_with_options(
         self,
         request: cloudsso_20210515_models.SetSCIMSynchronizationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetSCIMSynchronizationStatusResponse:
         """
-        You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
-        *   After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
-        *   After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
-        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61****`.
+        @summary Enables or disables Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
+        After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
+        After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
+        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61***`.
         
         @param request: SetSCIMSynchronizationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetSCIMSynchronizationStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7191,18 +8257,20 @@
 
     async def set_scimsynchronization_status_with_options_async(
         self,
         request: cloudsso_20210515_models.SetSCIMSynchronizationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.SetSCIMSynchronizationStatusResponse:
         """
-        You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
-        *   After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
-        *   After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
-        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61****`.
+        @summary Enables or disables Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
+        After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
+        After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
+        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61***`.
         
         @param request: SetSCIMSynchronizationStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SetSCIMSynchronizationStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7230,49 +8298,55 @@
         )
 
     def set_scimsynchronization_status(
         self,
         request: cloudsso_20210515_models.SetSCIMSynchronizationStatusRequest,
     ) -> cloudsso_20210515_models.SetSCIMSynchronizationStatusResponse:
         """
-        You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
-        *   After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
-        *   After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
-        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61****`.
+        @summary Enables or disables Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
+        After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
+        After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
+        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61***`.
         
         @param request: SetSCIMSynchronizationStatusRequest
         @return: SetSCIMSynchronizationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.set_scimsynchronization_status_with_options(request, runtime)
 
     async def set_scimsynchronization_status_async(
         self,
         request: cloudsso_20210515_models.SetSCIMSynchronizationStatusRequest,
     ) -> cloudsso_20210515_models.SetSCIMSynchronizationStatusResponse:
         """
-        You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
-        *   After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
-        *   After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
-        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61****`.
+        @summary Enables or disables Cross-domain Identity Management (SCIM) synchronization.
+        
+        @description You can synchronize users or groups from an external identity provider (IdP) that supports SCIM 2.0 to CloudSSO only after SCIM synchronization is enabled. If you disable SCIM synchronization, you can no longer synchronize users or groups to CloudSSO. The following list describes the impacts after SCIM synchronization is enabled or disabled:
+        After you enable SCIM synchronization, you cannot modify or delete the users or groups that are synchronized to CloudSSO by using SCIM. In addition, you cannot add users to or remove users from the groups. However, you can change the passwords of the users and enable or disable the logon of the users.
+        After you disable SCIM synchronization, you can modify and delete the users and groups that are synchronized to CloudSSO by using SCIM. You can also add users to or remove users from the groups.
+        This topic provides an example on how to enable SCIM synchronization within the directory `d-00fc2p61***`.
         
         @param request: SetSCIMSynchronizationStatusRequest
         @return: SetSCIMSynchronizationStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.set_scimsynchronization_status_with_options_async(request, runtime)
 
     def update_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.UpdateAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateAccessConfigurationResponse:
         """
-        You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
-        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj****` to `https://cloudsso.console.aliyun.com`.
+        @summary Modifies information about an access configuration.
+        
+        @description You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
+        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj***` to `https://cloudsso.console.aliyun.com`.
         
         @param request: UpdateAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7307,16 +8381,18 @@
 
     async def update_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateAccessConfigurationResponse:
         """
-        You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
-        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj****` to `https://cloudsso.console.aliyun.com`.
+        @summary Modifies information about an access configuration.
+        
+        @description You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
+        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj***` to `https://cloudsso.console.aliyun.com`.
         
         @param request: UpdateAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7350,44 +8426,50 @@
         )
 
     def update_access_configuration(
         self,
         request: cloudsso_20210515_models.UpdateAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.UpdateAccessConfigurationResponse:
         """
-        You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
-        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj****` to `https://cloudsso.console.aliyun.com`.
+        @summary Modifies information about an access configuration.
+        
+        @description You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
+        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj***` to `https://cloudsso.console.aliyun.com`.
         
         @param request: UpdateAccessConfigurationRequest
         @return: UpdateAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_access_configuration_with_options(request, runtime)
 
     async def update_access_configuration_async(
         self,
         request: cloudsso_20210515_models.UpdateAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.UpdateAccessConfigurationResponse:
         """
-        You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
-        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj****` to `https://cloudsso.console.aliyun.com`.
+        @summary Modifies information about an access configuration.
+        
+        @description You can modify the `Description`, `SessionDuration`, and `RelayState` parameters for an access configuration.
+        This topic provides an example on how to change the initial web page in the access configuration `ac-00jhtfl8thteu6uj***` to `https://cloudsso.console.aliyun.com`.
         
         @param request: UpdateAccessConfigurationRequest
         @return: UpdateAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_access_configuration_with_options_async(request, runtime)
 
     def update_directory_with_options(
         self,
         request: cloudsso_20210515_models.UpdateDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateDirectoryResponse:
         """
-        After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
+        @summary Changes the name of a directory.
+        
+        @description After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
         This topic provides an example on how to change the name of a directory to `new-example`.
         
         @param request: UpdateDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDirectoryResponse
         """
         UtilClient.validate_model(request)
@@ -7417,15 +8499,17 @@
 
     async def update_directory_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateDirectoryResponse:
         """
-        After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
+        @summary Changes the name of a directory.
+        
+        @description After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
         This topic provides an example on how to change the name of a directory to `new-example`.
         
         @param request: UpdateDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateDirectoryResponse
         """
         UtilClient.validate_model(request)
@@ -7454,46 +8538,52 @@
         )
 
     def update_directory(
         self,
         request: cloudsso_20210515_models.UpdateDirectoryRequest,
     ) -> cloudsso_20210515_models.UpdateDirectoryResponse:
         """
-        After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
+        @summary Changes the name of a directory.
+        
+        @description After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
         This topic provides an example on how to change the name of a directory to `new-example`.
         
         @param request: UpdateDirectoryRequest
         @return: UpdateDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_directory_with_options(request, runtime)
 
     async def update_directory_async(
         self,
         request: cloudsso_20210515_models.UpdateDirectoryRequest,
     ) -> cloudsso_20210515_models.UpdateDirectoryResponse:
         """
-        After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
+        @summary Changes the name of a directory.
+        
+        @description After you change the name of a directory, the URL that is used to log on to the Cloud SSO user portal is changed. You must notify the Cloud SSO users of the correct URL.
         This topic provides an example on how to change the name of a directory to `new-example`.
         
         @param request: UpdateDirectoryRequest
         @return: UpdateDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_directory_with_options_async(request, runtime)
 
     def update_group_with_options(
         self,
         request: cloudsso_20210515_models.UpdateGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateGroupResponse:
         """
-        You can modify `GroupName` and `Description` for a group.
+        @summary Modifies information about a group.
+        
+        @description You can modify `GroupName` and `Description` for a group.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a group that is synchronized by using SCIM.
-        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh****` to `NewTestGroup`.
+        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh***` to `NewTestGroup`.
         
         @param request: UpdateGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7526,17 +8616,19 @@
 
     async def update_group_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateGroupResponse:
         """
-        You can modify `GroupName` and `Description` for a group.
+        @summary Modifies information about a group.
+        
+        @description You can modify `GroupName` and `Description` for a group.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a group that is synchronized by using SCIM.
-        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh****` to `NewTestGroup`.
+        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh***` to `NewTestGroup`.
         
         @param request: UpdateGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateGroupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7568,46 +8660,52 @@
         )
 
     def update_group(
         self,
         request: cloudsso_20210515_models.UpdateGroupRequest,
     ) -> cloudsso_20210515_models.UpdateGroupResponse:
         """
-        You can modify `GroupName` and `Description` for a group.
+        @summary Modifies information about a group.
+        
+        @description You can modify `GroupName` and `Description` for a group.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a group that is synchronized by using SCIM.
-        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh****` to `NewTestGroup`.
+        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh***` to `NewTestGroup`.
         
         @param request: UpdateGroupRequest
         @return: UpdateGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_group_with_options(request, runtime)
 
     async def update_group_async(
         self,
         request: cloudsso_20210515_models.UpdateGroupRequest,
     ) -> cloudsso_20210515_models.UpdateGroupResponse:
         """
-        You can modify `GroupName` and `Description` for a group.
+        @summary Modifies information about a group.
+        
+        @description You can modify `GroupName` and `Description` for a group.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a group that is synchronized by using SCIM.
-        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh****` to `NewTestGroup`.
+        This topic provides an example on how to change the name of the group `g-00jqzghi2n3o5hkh***` to `NewTestGroup`.
         
         @param request: UpdateGroupRequest
         @return: UpdateGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_group_with_options_async(request, runtime)
 
     def update_inline_policy_for_access_configuration_with_options(
         self,
         request: cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationResponse:
         """
-        This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Modifies an inline policy that is created for an access configuration.
+        
+        @description This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: UpdateInlinePolicyForAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateInlinePolicyForAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7640,15 +8738,17 @@
 
     async def update_inline_policy_for_access_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationResponse:
         """
-        This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Modifies an inline policy that is created for an access configuration.
+        
+        @description This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: UpdateInlinePolicyForAccessConfigurationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateInlinePolicyForAccessConfigurationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7680,43 +8780,49 @@
         )
 
     def update_inline_policy_for_access_configuration(
         self,
         request: cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationResponse:
         """
-        This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Modifies an inline policy that is created for an access configuration.
+        
+        @description This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: UpdateInlinePolicyForAccessConfigurationRequest
         @return: UpdateInlinePolicyForAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_inline_policy_for_access_configuration_with_options(request, runtime)
 
     async def update_inline_policy_for_access_configuration_async(
         self,
         request: cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationRequest,
     ) -> cloudsso_20210515_models.UpdateInlinePolicyForAccessConfigurationResponse:
         """
-        This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
+        @summary Modifies an inline policy that is created for an access configuration.
+        
+        @description This topic provides an example on how to modify an inline policy that is created for the access configuration `ac-00jhtfl8thteu6uj***`.
         
         @param request: UpdateInlinePolicyForAccessConfigurationRequest
         @return: UpdateInlinePolicyForAccessConfigurationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_inline_policy_for_access_configuration_with_options_async(request, runtime)
 
     def update_mfaauthentication_settings_with_options(
         self,
         request: cloudsso_20210515_models.UpdateMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateMFAAuthenticationSettingsResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61****`.
+        @summary Modifies the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61***`.
         
         @param request: UpdateMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7747,16 +8853,18 @@
 
     async def update_mfaauthentication_settings_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateMFAAuthenticationSettingsResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61****`.
+        @summary Modifies the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61***`.
         
         @param request: UpdateMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7786,44 +8894,50 @@
         )
 
     def update_mfaauthentication_settings(
         self,
         request: cloudsso_20210515_models.UpdateMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.UpdateMFAAuthenticationSettingsResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61****`.
+        @summary Modifies the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61***`.
         
         @param request: UpdateMFAAuthenticationSettingsRequest
         @return: UpdateMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_mfaauthentication_settings_with_options(request, runtime)
 
     async def update_mfaauthentication_settings_async(
         self,
         request: cloudsso_20210515_models.UpdateMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.UpdateMFAAuthenticationSettingsResponse:
         """
-        If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
-        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61****`.
+        @summary Modifies the multi-factor authentication (MFA) setting of all users.
+        
+        @description If you enable username-password logon for CloudSSO users, you can also configure MFA for the users.
+        This topic provides an example on how to enable MFA for all CloudSSO users that belong to the directory named `d-00fc2p61***`.
         
         @param request: UpdateMFAAuthenticationSettingsRequest
         @return: UpdateMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_mfaauthentication_settings_with_options_async(request, runtime)
 
     def update_scimserver_credential_status_with_options(
         self,
         request: cloudsso_20210515_models.UpdateSCIMServerCredentialStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateSCIMServerCredentialStatusResponse:
         """
-        This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
+        @summary Enables or disables a Cross-domain Identity Management (SCIM) credential.
+        
+        @description This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
         
         @param request: UpdateSCIMServerCredentialStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateSCIMServerCredentialStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7854,15 +8968,17 @@
 
     async def update_scimserver_credential_status_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateSCIMServerCredentialStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateSCIMServerCredentialStatusResponse:
         """
-        This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
+        @summary Enables or disables a Cross-domain Identity Management (SCIM) credential.
+        
+        @description This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
         
         @param request: UpdateSCIMServerCredentialStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateSCIMServerCredentialStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7892,44 +9008,50 @@
         )
 
     def update_scimserver_credential_status(
         self,
         request: cloudsso_20210515_models.UpdateSCIMServerCredentialStatusRequest,
     ) -> cloudsso_20210515_models.UpdateSCIMServerCredentialStatusResponse:
         """
-        This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
+        @summary Enables or disables a Cross-domain Identity Management (SCIM) credential.
+        
+        @description This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
         
         @param request: UpdateSCIMServerCredentialStatusRequest
         @return: UpdateSCIMServerCredentialStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_scimserver_credential_status_with_options(request, runtime)
 
     async def update_scimserver_credential_status_async(
         self,
         request: cloudsso_20210515_models.UpdateSCIMServerCredentialStatusRequest,
     ) -> cloudsso_20210515_models.UpdateSCIMServerCredentialStatusResponse:
         """
-        This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
+        @summary Enables or disables a Cross-domain Identity Management (SCIM) credential.
+        
+        @description This topic provides an example on how to disable the SCIM credential whose ID is `scimcred-004whl0kvfwcypbi***`. After the SCIM credential is disabled, the synchronization task that uses the SCIM credential fails. You can call this operation again to enable the SCIM credential.
         
         @param request: UpdateSCIMServerCredentialStatusRequest
         @return: UpdateSCIMServerCredentialStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_scimserver_credential_status_with_options_async(request, runtime)
 
     def update_user_with_options(
         self,
         request: cloudsso_20210515_models.UpdateUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserResponse:
         """
-        You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
+        @summary Modifies information about a user.
+        
+        @description You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a user that is synchronized by using SCIM.
-        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk****` to `AliceLee@example.com`.
+        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk***` to `AliceLee@example.com`.
         
         @param request: UpdateUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7968,17 +9090,19 @@
 
     async def update_user_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserResponse:
         """
-        You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
+        @summary Modifies information about a user.
+        
+        @description You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a user that is synchronized by using SCIM.
-        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk****` to `AliceLee@example.com`.
+        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk***` to `AliceLee@example.com`.
         
         @param request: UpdateUserRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateUserResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8016,48 +9140,54 @@
         )
 
     def update_user(
         self,
         request: cloudsso_20210515_models.UpdateUserRequest,
     ) -> cloudsso_20210515_models.UpdateUserResponse:
         """
-        You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
+        @summary Modifies information about a user.
+        
+        @description You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a user that is synchronized by using SCIM.
-        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk****` to `AliceLee@example.com`.
+        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk***` to `AliceLee@example.com`.
         
         @param request: UpdateUserRequest
         @return: UpdateUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_user_with_options(request, runtime)
 
     async def update_user_async(
         self,
         request: cloudsso_20210515_models.UpdateUserRequest,
     ) -> cloudsso_20210515_models.UpdateUserResponse:
         """
-        You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
+        @summary Modifies information about a user.
+        
+        @description You can modify `FirstName`, `LastName`, `DisplayName`, `Email`, and `Description` for a user. You cannot modify `UserName` for a user.
         >  If System for Cross-domain Identity Management (SCIM) synchronization is enabled, you cannot modify the information about a user that is synchronized by using SCIM.
-        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk****` to `AliceLee@example.com`.
+        This topic provides an example on how to change the email address of the user whose ID is `u-00q8wbq42wiltcrk***` to `AliceLee@example.com`.
         
         @param request: UpdateUserRequest
         @return: UpdateUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_with_options_async(request, runtime)
 
     def update_user_mfaauthentication_settings_with_options(
         self,
         request: cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsResponse:
         """
-        If you call the [UpdateMFAAuthenticationSettings](~~450134~~) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
+        @summary Modifies the multi-factor authentication (MFA) setting of a single user.
+        
+        @description If you call the [UpdateMFAAuthenticationSettings](https://help.aliyun.com/document_detail/450134.html) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
         By default, the MFAAuthenticationSettings parameter is set to `Enabled` for a new user.
-        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk****`.
+        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk***`.
         
         @param request: UpdateUserMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateUserMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8088,17 +9218,19 @@
 
     async def update_user_mfaauthentication_settings_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsResponse:
         """
-        If you call the [UpdateMFAAuthenticationSettings](~~450134~~) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
+        @summary Modifies the multi-factor authentication (MFA) setting of a single user.
+        
+        @description If you call the [UpdateMFAAuthenticationSettings](https://help.aliyun.com/document_detail/450134.html) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
         By default, the MFAAuthenticationSettings parameter is set to `Enabled` for a new user.
-        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk****`.
+        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk***`.
         
         @param request: UpdateUserMFAAuthenticationSettingsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateUserMFAAuthenticationSettingsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8128,44 +9260,55 @@
         )
 
     def update_user_mfaauthentication_settings(
         self,
         request: cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsResponse:
         """
-        If you call the [UpdateMFAAuthenticationSettings](~~450134~~) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
+        @summary Modifies the multi-factor authentication (MFA) setting of a single user.
+        
+        @description If you call the [UpdateMFAAuthenticationSettings](https://help.aliyun.com/document_detail/450134.html) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
         By default, the MFAAuthenticationSettings parameter is set to `Enabled` for a new user.
-        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk****`.
+        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk***`.
         
         @param request: UpdateUserMFAAuthenticationSettingsRequest
         @return: UpdateUserMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_user_mfaauthentication_settings_with_options(request, runtime)
 
     async def update_user_mfaauthentication_settings_async(
         self,
         request: cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsRequest,
     ) -> cloudsso_20210515_models.UpdateUserMFAAuthenticationSettingsResponse:
         """
-        If you call the [UpdateMFAAuthenticationSettings](~~450134~~) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
+        @summary Modifies the multi-factor authentication (MFA) setting of a single user.
+        
+        @description If you call the [UpdateMFAAuthenticationSettings](https://help.aliyun.com/document_detail/450134.html) operation to set the MFAAuthenticationSettings parameter to `Byuser`, user-specific settings are applied. Then, you must call the UpdateUserMFAAuthenticationSettings operation to configure MFA for each user.
         By default, the MFAAuthenticationSettings parameter is set to `Enabled` for a new user.
-        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk****`.
+        This topic provides an example on how to enable MFA for the user named `u-00q8wbq42wiltcrk***`.
         
         @param request: UpdateUserMFAAuthenticationSettingsRequest
         @return: UpdateUserMFAAuthenticationSettingsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_mfaauthentication_settings_with_options_async(request, runtime)
 
     def update_user_provisioning_with_options(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningResponse:
+        """
+        @summary Modifies a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.new_deletion_strategy):
             query['NewDeletionStrategy'] = request.new_deletion_strategy
         if not UtilClient.is_unset(request.new_description):
@@ -8194,14 +9337,21 @@
         )
 
     async def update_user_provisioning_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningResponse:
+        """
+        @summary Modifies a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserProvisioningResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.new_deletion_strategy):
             query['NewDeletionStrategy'] = request.new_deletion_strategy
         if not UtilClient.is_unset(request.new_description):
@@ -8229,29 +9379,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_user_provisioning(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningRequest,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningResponse:
+        """
+        @summary Modifies a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningRequest
+        @return: UpdateUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_user_provisioning_with_options(request, runtime)
 
     async def update_user_provisioning_async(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningRequest,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningResponse:
+        """
+        @summary Modifies a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningRequest
+        @return: UpdateUserProvisioningResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_provisioning_with_options_async(request, runtime)
 
     def update_user_provisioning_configuration_with_options(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningConfigurationResponse:
+        """
+        @summary Modifies the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningConfigurationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserProvisioningConfigurationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.new_default_landing_page):
             query['NewDefaultLandingPage'] = request.new_default_landing_page
         if not UtilClient.is_unset(request.new_session_duration):
@@ -8276,14 +9445,21 @@
         )
 
     async def update_user_provisioning_configuration_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningConfigurationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningConfigurationResponse:
+        """
+        @summary Modifies the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningConfigurationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserProvisioningConfigurationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.directory_id):
             query['DirectoryId'] = request.directory_id
         if not UtilClient.is_unset(request.new_default_landing_page):
             query['NewDefaultLandingPage'] = request.new_default_landing_page
         if not UtilClient.is_unset(request.new_session_duration):
@@ -8307,31 +9483,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_user_provisioning_configuration(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningConfigurationRequest,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningConfigurationResponse:
+        """
+        @summary Modifies the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningConfigurationRequest
+        @return: UpdateUserProvisioningConfigurationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_user_provisioning_configuration_with_options(request, runtime)
 
     async def update_user_provisioning_configuration_async(
         self,
         request: cloudsso_20210515_models.UpdateUserProvisioningConfigurationRequest,
     ) -> cloudsso_20210515_models.UpdateUserProvisioningConfigurationResponse:
+        """
+        @summary Modifies the global configurations of a Resource Access Management (RAM) user provisioning.
+        
+        @param request: UpdateUserProvisioningConfigurationRequest
+        @return: UpdateUserProvisioningConfigurationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_provisioning_configuration_with_options_async(request, runtime)
 
     def update_user_status_with_options(
         self,
         request: cloudsso_20210515_models.UpdateUserStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserStatusResponse:
         """
-        This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
+        @summary Changes the status of a user.
+        
+        @description This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
         
         @param request: UpdateUserStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateUserStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8362,15 +9552,17 @@
 
     async def update_user_status_with_options_async(
         self,
         request: cloudsso_20210515_models.UpdateUserStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cloudsso_20210515_models.UpdateUserStatusResponse:
         """
-        This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
+        @summary Changes the status of a user.
+        
+        @description This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
         
         @param request: UpdateUserStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateUserStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8400,27 +9592,31 @@
         )
 
     def update_user_status(
         self,
         request: cloudsso_20210515_models.UpdateUserStatusRequest,
     ) -> cloudsso_20210515_models.UpdateUserStatusResponse:
         """
-        This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
+        @summary Changes the status of a user.
+        
+        @description This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
         
         @param request: UpdateUserStatusRequest
         @return: UpdateUserStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.update_user_status_with_options(request, runtime)
 
     async def update_user_status_async(
         self,
         request: cloudsso_20210515_models.UpdateUserStatusRequest,
     ) -> cloudsso_20210515_models.UpdateUserStatusResponse:
         """
-        This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
+        @summary Changes the status of a user.
+        
+        @description This topic provides an example on how to change the status of the user whose ID is `u-00q8wbq42wiltcrk***` to Disabled. Users in the Disabled state cannot log on to the CloudSSO user portal.
         
         @param request: UpdateUserStatusRequest
         @return: UpdateUserStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_status_with_options_async(request, runtime)
```

### Comparing `alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515/models.py` & `alibabacloud_cloudsso20210515-1.6.0/alibabacloud_cloudsso20210515/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         self.access_configuration_id = access_configuration_id
         # The ID of the directory.
         self.directory_id = directory_id
         # The configurations of the inline policy.
         # 
         # The value can be up to 4,096 characters in length.
         # 
-        # If you set `PermissionPolicyType` to `Inline`, you must specify this parameter. For more information about the syntax and structure of RAM policies, see [Policy syntax and structure](~~93739~~).
+        # If you set `PermissionPolicyType` to `Inline`, you must specify this parameter. For more information about the syntax and structure of RAM policies, see [Policy syntax and structure](https://help.aliyun.com/document_detail/93739.html).
         self.inline_policy_document = inline_policy_document
         # The name of the policy.
         # 
         # *   If you set `PermissionPolicyType` to `System`, you must set this parameter to the name of the system policy. You can obtain the name of the system policy from RAM.
         # *   If you set `PermissionPolicyType` to `Inline`, you must set this parameter to the name of the inline policy. A custom value is supported.
         self.permission_policy_name = permission_policy_name
         # The type of the policy. Valid values:
@@ -1132,15 +1132,15 @@
         # 
         # The description can be up to 1,024 characters in length.
         self.description = description
         # The ID of the directory.
         self.directory_id = directory_id
         # The name of the group.
         # 
-        # The name can contain letters, digits, underscores (\_), hyphens (-), and periods (.).
+        # The name can contain letters, digits, underscores (_), hyphens (-), and periods (.).
         # 
         # The name can be up to 128 characters in length.
         self.group_name = group_name
 
     def validate(self):
         pass
 
@@ -1788,16 +1788,16 @@
         # The conflict handling policy. The policy is used when a RAM user has the same username as the CloudSSO user who is synchronized to RAM. Valid values:
         # 
         # *   KeepBoth: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system creates a RAM user whose username is the username of the CloudSSO user plus the suffix `_sso`.
         # *   TakeOver: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system replaces the RAM user with the CloudSSO user.
         self.duplication_strategy = duplication_strategy
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If you set the `PrincipalType` parameter to `Group`, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If you set the `PrincipalType` parameter to `User`, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If you set the `PrincipalType` parameter to `Group`, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If you set the `PrincipalType` parameter to `User`, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity type of the RAM user provisioning. Valid values:
         # 
         # *   User: The identity of the RAM user provisioning is a CloudSSO user.
         # *   Group: The identity of the RAM user provisioning is a CloudSSO user group.
         self.principal_type = principal_type
         # The ID of the object for which you create the RAM user provisioning. The value is fixed as the ID of the member in the resource directory.
@@ -1889,16 +1889,16 @@
         # *   KeepBoth: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system creates a RAM user whose username is the username of the CloudSSO user plus the suffix `_sso`.
         # *   TakeOver: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system replaces the RAM user with the CloudSSO user.
         self.duplication_strategy = duplication_strategy
         # The ID of the Alibaba Cloud account to which the resource directory belongs.
         self.owner_pk = owner_pk
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity name of the RAM user provisioning. Valid values:
         # 
         # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user group.
         # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user.
         self.principal_name = principal_name
         # The identity type of the RAM user provisioning. Valid values:
@@ -2368,15 +2368,15 @@
         # The ID of the access configuration.
         self.access_configuration_id = access_configuration_id
         # The ID of the directory.
         self.directory_id = directory_id
         # Specifies whether to forcibly remove system policies and inline policies. Valid values:
         # 
         # *   true: When you delete the access configuration, the associated system policies and inline policies are forcibly removed.
-        # *   false: When you delete the access configuration, the associated system policies and inline policies are not forcibly removed. This is the default value. If these policies exist in the access configuration, the deletion fails. Before you delete the access configuration, you must remove the system policies and inline policies. For more information, see [RemovePermissionPolicyFromAccessConfiguration](~~336904~~).
+        # *   false: When you delete the access configuration, the associated system policies and inline policies are not forcibly removed. This is the default value. If these policies exist in the access configuration, the deletion fails. Before you delete the access configuration, you must remove the system policies and inline policies. For more information, see [RemovePermissionPolicyFromAccessConfiguration](https://help.aliyun.com/document_detail/336904.html).
         self.force_remove_permission_policies = force_remove_permission_policies
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2680,15 +2680,15 @@
         mfadevice_id: str = None,
         user_id: str = None,
     ):
         # The ID of the directory.
         self.directory_id = directory_id
         # The ID of the MFA device.
         # 
-        # You can call the [ListMFADevicesForUser](~~333531~~) operation to query the IDs of MFA devices.
+        # You can call the [ListMFADevicesForUser](https://help.aliyun.com/document_detail/333531.html) operation to query the IDs of MFA devices.
         self.mfadevice_id = mfadevice_id
         # The ID of the user.
         self.user_id = user_id
 
     def validate(self):
         pass
 
@@ -3445,14 +3445,109 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeprovisionAccessConfigurationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DisableDelegateAccountRequest(TeaModel):
+    def __init__(
+        self,
+        account_id: str = None,
+    ):
+        self.account_id = account_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_id is not None:
+            result['AccountId'] = self.account_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountId') is not None:
+            self.account_id = m.get('AccountId')
+        return self
+
+
+class DisableDelegateAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DisableDelegateAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DisableDelegateAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DisableDelegateAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DisableServiceResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
         # The ID of the request.
         self.request_id = request_id
@@ -3514,14 +3609,109 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DisableServiceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class EnableDelegateAccountRequest(TeaModel):
+    def __init__(
+        self,
+        account_id: str = None,
+    ):
+        self.account_id = account_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_id is not None:
+            result['AccountId'] = self.account_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountId') is not None:
+            self.account_id = m.get('AccountId')
+        return self
+
+
+class EnableDelegateAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class EnableDelegateAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: EnableDelegateAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = EnableDelegateAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class EnableServiceResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
         # The ID of the request.
         self.request_id = request_id
@@ -4904,15 +5094,15 @@
         self,
         mfa_authentication_advance_settings: str = None,
         operation_for_risk_login: str = None,
     ):
         # The MFA policy of all users. Valid values:
         # 
         # *   Enabled: MFA is enabled for all users.
-        # *   Byuser: User-specific settings are applied. For more information about how to configure MFA for a single user, see [UpdateUserMFAAuthenticationSettings](~~450135~~).
+        # *   Byuser: User-specific settings are applied. For more information about how to configure MFA for a single user, see [UpdateUserMFAAuthenticationSettings](https://help.aliyun.com/document_detail/450135.html).
         # *   Disabled: MFA is disabled for all users.
         # *   OnlyRiskyLogin: MFA is required only for unusual logons.
         self.mfa_authentication_advance_settings = mfa_authentication_advance_settings
         # The MFA policy for unusual logons. Valid values:
         # 
         # *   Autonomous: MFA is prompted for users who initiated unusual logons. However, the users are allowed to skip MFA. If an MFA device is bound to a user who initiated an unusual logon, the user must pass MFA.
         # *   EnforceVerify: MFA is required. If no MFA devices are bound to a user who initiated an unusual logon, the user must bind an MFA device. If an MFA device is already bound to a user who initiated an unusual logon, the user must pass MFA.
@@ -6171,15 +6361,15 @@
 
 class GetUserRequest(TeaModel):
     def __init__(
         self,
         directory_id: str = None,
         user_id: str = None,
     ):
-        # The ID of the directory.
+        # The ID of the resource directory.
         self.directory_id = directory_id
         # The ID of the user.
         self.user_id = user_id
 
     def validate(self):
         pass
 
@@ -6206,15 +6396,17 @@
 
 class GetUserResponseBodyUserExternalId(TeaModel):
     def __init__(
         self,
         id: str = None,
         issuer: str = None,
     ):
+        # The identifier of the user that is synchronized from an external IdP.
         self.id = id
+        # The method for external identity synchronization. Only System for Cross-domain Identity Management (SCIM) synchronization is supported.
         self.issuer = issuer
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6249,22 +6441,23 @@
         last_name: str = None,
         provision_type: str = None,
         status: str = None,
         update_time: str = None,
         user_id: str = None,
         user_name: str = None,
     ):
-        # The time when the user was created.
+        # The time when the user was created. The value is displayed in UTC.
         self.create_time = create_time
         # The description of the user.
         self.description = description
         # The display name of the user.
         self.display_name = display_name
         # The email address of the user.
         self.email = email
+        # The identifier information about the user synchronized from an external IdP.
         self.external_id = external_id
         # The first name of the user.
         self.first_name = first_name
         # The last name of the user.
         self.last_name = last_name
         # The type of the user. Valid values:
         # 
@@ -6272,15 +6465,15 @@
         # *   Synchronized: The user is synchronized from an external identity provider (IdP).
         self.provision_type = provision_type
         # The status of the user. Valid values:
         # 
         # *   Enabled: The logon of the user is enabled.
         # *   Disabled: The logon of the user is disabled.
         self.status = status
-        # The time when the information about the user was modified.
+        # The time when the information about the user was modified. The value is displayed in UTC.
         self.update_time = update_time
         # The ID of the user.
         self.user_id = user_id
         # The name of the user.
         self.user_name = user_name
 
     def validate(self):
@@ -6351,15 +6544,15 @@
 
 class GetUserResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         user: GetUserResponseBodyUser = None,
     ):
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
         # The information about the user.
         self.user = user
 
     def validate(self):
         if self.user:
             self.user.validate()
@@ -6429,15 +6622,17 @@
 
 class GetUserIdRequestExternalId(TeaModel):
     def __init__(
         self,
         id: str = None,
         issuer: str = None,
     ):
+        # The identifier of the user that is synchronized from an external IdP.
         self.id = id
+        # The method for external identity synchronization. Only System for Cross-domain Identity Management (SCIM) synchronization is supported.
         self.issuer = issuer
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6462,15 +6657,17 @@
 
 class GetUserIdRequest(TeaModel):
     def __init__(
         self,
         directory_id: str = None,
         external_id: GetUserIdRequestExternalId = None,
     ):
+        # The ID of the resource directory.
         self.directory_id = directory_id
+        # The identifier information about the user that is synchronized from an external identity provider (IdP).
         self.external_id = external_id
 
     def validate(self):
         if self.external_id:
             self.external_id.validate()
 
     def to_map(self):
@@ -6497,15 +6694,17 @@
 
 class GetUserIdShrinkRequest(TeaModel):
     def __init__(
         self,
         directory_id: str = None,
         external_id_shrink: str = None,
     ):
+        # The ID of the resource directory.
         self.directory_id = directory_id
+        # The identifier information about the user that is synchronized from an external identity provider (IdP).
         self.external_id_shrink = external_id_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6530,15 +6729,17 @@
 
 class GetUserIdResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         user_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
+        # The ID of the CloudSSO user.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6787,16 +6988,16 @@
         # *   KeepBoth: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system creates a RAM user whose username is the username of the CloudSSO user plus the suffix `_sso`.
         # *   TakeOver: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system replaces the RAM user with the CloudSSO user.
         self.duplication_strategy = duplication_strategy
         # The ID of the Alibaba Cloud account to which the resource directory belongs.
         self.owner_pk = owner_pk
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity name of the RAM user provisioning. Valid values:
         # 
         # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user group.
         # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user.
         self.principal_name = principal_name
         # The identity type of the RAM user provisioning. Valid values:
@@ -7227,16 +7428,16 @@
         self.error_info = error_info
         # The ID of the RAM user provisioning event.
         self.event_id = event_id
         # The time at which the RAM user provisioning event was last executed.
         self.latest_async_time = latest_async_time
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity name of the RAM user provisioning. Valid values:
         # 
         # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user group.
         # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user.
         self.principal_name = principal_name
         # The identity type of the RAM user provisioning. Valid values:
@@ -8438,15 +8639,15 @@
         next_token: str = None,
         status_notifications: str = None,
     ):
         # The ID of the directory.
         self.directory_id = directory_id
         # The filter condition.
         # 
-        # Specify the value in the \<Attribute> \<Operator> \<Value> format. The value is not case sensitive. You can set \<Attribute> only to AccessConfigurationName and \<Operator> only to eq or sw. The value eq indicates Equals. The value sw indicates Starts With.
+        # Specify the value in the \\<Attribute> \\<Operator> \\<Value> format. The value is not case sensitive. You can set \\<Attribute> only to AccessConfigurationName and \\<Operator> only to eq or sw. The value eq indicates Equals. The value sw indicates Starts With.
         # 
         # For example, if you set Filter to AccessConfigurationName sw test, the operation queries all access configurations whose names start with test. If you set Filter to AccessConfigurationName eq TestAccessConfiguration, the operation queries the access configuration whose name is TestAccessConfiguration.
         self.filter = filter
         # The number of entries to return on each page.
         # 
         # Valid values: 1 to 100.
         # 
@@ -10856,16 +11057,16 @@
         self.error_info = error_info
         # The ID of the RAM user provisioning event.
         self.event_id = event_id
         # The time at which the RAM user provisioning event was last executed.
         self.latest_async_time = latest_async_time
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity name of the RAM user provisioning. Valid values:
         # 
         # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user group.
         # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user.
         self.principal_name = principal_name
         # The identity type of the RAM user provisioning. Valid values:
@@ -11128,16 +11329,16 @@
         self.max_results = max_results
         # The token that is used to initiate the next request. If this is your first time to call this operation, you do not need to specify the `NextToken` parameter.
         # 
         # When you call this operation for the first time, if the total number of entries to return is larger than the value of `MaxResults`, the entries are truncated. The system returns entries based on the value of `MaxResults`, and does not return the excess entries. In this case, the value of the response parameter `IsTruncated` is `true`, and `NextToken` is returned. In the next call, you can use the value of `NextToken` and maintain the settings of the other request parameters to query the excess entries. You can repeat the call until the value of `IsTruncated` becomes `false`. This way, all entries are returned.
         self.next_token = next_token
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity type of the RAM user provisioning. Valid values:
         # 
         # *   User: The identity of the RAM user provisioning is a CloudSSO user.
         # *   Group: The identity of the RAM user provisioning is a CloudSSO user group.
         self.principal_type = principal_type
         # The ID of the object for which you create the RAM user provisioning. The value is fixed as the ID of the member in the resource directory.
@@ -11225,16 +11426,16 @@
         # *   KeepBoth: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system creates a RAM user whose username is the username of the CloudSSO user plus the suffix `_sso`.
         # *   TakeOver: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system replaces the RAM user with the CloudSSO user.
         self.duplication_strategy = duplication_strategy
         # The ID of the Alibaba Cloud account to which the resource directory belongs.
         self.owner_pk = owner_pk
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity name of the RAM user provisioning. Valid values:
         # 
         # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user group.
         # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user.
         self.principal_name = principal_name
         # The identity type of the RAM user provisioning. Valid values:
@@ -11467,38 +11668,38 @@
         directory_id: str = None,
         filter: str = None,
         max_results: int = None,
         next_token: str = None,
         provision_type: str = None,
         status: str = None,
     ):
-        # The ID of the directory.
+        # The ID of the resource directory.
         self.directory_id = directory_id
         # The filter condition.
         # 
-        # Specify the value in the `<Attribute> <Operator> <Value>` format. The value is not case-sensitive. You can set `<Attribute>` only to `UserName` and `Operator` only to `eq` or `sw`. The value eq indicates Equals, and the value sw indicates Starts With.
+        # You must specify the value in the `<Attribute> <Operator> <Value>` format. The value is not case-sensitive. You can set `<Attribute>` only to `UserName` and `Operator` only to `eq` or `sw`. The value eq indicates Equals, and the value sw indicates Start With.
         # 
-        # For example, if you set Filter to UserName sw test, the operation queries the users whose names start with test. If you set Filter to UserName eq testuser, the operation queries the user whose name is `testuser`.
+        # For example, if you set the Filter parameter to UserName sw test, the operation queries the users whose names start with test. If you set the Filter parameter to UserName eq testuser, the operation queries the user whose name is `testuser`.
         self.filter = filter
-        # The number of entries to return on each page.
+        # The number of entries per page.
         # 
         # Valid values: 1 to 100.
         # 
         # Default value: 10.
         self.max_results = max_results
-        # The token to return for the next page. If this is your first time to call this operation, you do not need to specify `NextToken`.
+        # The pagination token that is used in the next request to retrieve a new page of results. You do not need to specify this parameter for the first request. You must specify the token that is obtained from the previous query as the value of the `NextToken` parameter.
         # 
-        # When you call this operation for the first time, if the total number of entries to return exceeds the value of `MaxResults`, the entries are truncated. Only the entries that match the value of `MaxResults` are returned, and the excess entries are not returned. In this case, the value of the response parameter `IsTruncated` is `true`, and `NextToken` is returned. In the next call, you can use the value of `NextToken` and maintain the settings of the other request parameters to query the excess entries. You can repeat the call until the value of `IsTruncated` becomes `false`. This way, all entries are returned.
+        # When you call this operation for the first time, if the total number of entries to return is larger than the value of the `MaxResults` parameter, the entries are truncated. The system returns entries based on the value of the `MaxResults` parameter, and does not return the excess entries. In this case, the value of the response parameter `IsTruncated` is `true`, and the `NextToken` parameter is returned. In the next call, you can use the value of the `NextToken` parameter and maintain the settings of the other request parameters to query the excess entries. You can repeat the call until the value of the `IsTruncated` parameter becomes `false`. This way, all entries are returned.
         self.next_token = next_token
-        # The type of the user. The type can be used to filter users. Valid values:
+        # The type of the user. The parameter can be used to filter users. Valid values:
         # 
         # *   Manual: The user is manually created.
-        # *   Synchronized: The user is synchronized from an external IdP.
+        # *   Synchronized: The user is synchronized from an external identity provider (IdP).
         self.provision_type = provision_type
-        # The status of the user. The status can be used to filter users. Valid values:
+        # The status of the user. The parameter can be used to filter users. Valid values:
         # 
         # *   Enabled: The logon of the user is enabled.
         # *   Disabled: The logon of the user is disabled.
         self.status = status
 
     def validate(self):
         pass
@@ -11542,15 +11743,17 @@
 
 class ListUsersResponseBodyUsersExternalId(TeaModel):
     def __init__(
         self,
         id: str = None,
         issuer: str = None,
     ):
+        # The identifier of the user that is synchronized from an external IdP.
         self.id = id
+        # The method for external identity synchronization. Only System for Cross-domain Identity Management (SCIM) synchronization is supported.
         self.issuer = issuer
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11585,22 +11788,23 @@
         last_name: str = None,
         provision_type: str = None,
         status: str = None,
         update_time: str = None,
         user_id: str = None,
         user_name: str = None,
     ):
-        # The time when the user was created.
+        # The time when the user was created. The value is displayed in UTC.
         self.create_time = create_time
         # The description of the user.
         self.description = description
         # The display name of the user.
         self.display_name = display_name
         # The email address of the user.
         self.email = email
+        # The identifier information about the user synchronized from an external IdP.
         self.external_id = external_id
         # The first name of the user.
         self.first_name = first_name
         # The last name of the user.
         self.last_name = last_name
         # The type of the user. Valid values:
         # 
@@ -11608,15 +11812,15 @@
         # *   Synchronized: The user is synchronized from an external IdP.
         self.provision_type = provision_type
         # The status of the user. Valid values:
         # 
         # *   Enabled: The logon of the user is enabled.
         # *   Disabled: The logon of the user is disabled.
         self.status = status
-        # The time when the information about the user was modified.
+        # The time when the information about the user was modified. The value is displayed in UTC.
         self.update_time = update_time
         # The ID of the user.
         self.user_id = user_id
         # The name of the user.
         self.user_name = user_name
 
     def validate(self):
@@ -11693,24 +11897,24 @@
         next_token: str = None,
         request_id: str = None,
         total_counts: int = None,
         users: List[ListUsersResponseBodyUsers] = None,
     ):
         # Indicates whether the queried entries are truncated. Valid values:
         # 
-        # *   true: The queried entries are truncated.
-        # *   false: The queried entries are not truncated.
+        # *   true
+        # *   false
         self.is_truncated = is_truncated
-        # The number of entries returned per page.
+        # The number of entries per page.
         self.max_results = max_results
-        # The token that is returned for the next page.
+        # The pagination token that is used in the next request to retrieve a new page of results.
         # 
-        # >  This parameter is returned only when the value of `IsTruncated` is `true`.
+        # >  This parameter is returned only when the `IsTruncated` parameter is `true`.
         self.next_token = next_token
-        # The ID of the request.
+        # The request ID.
         self.request_id = request_id
         # The total number of entries returned.
         self.total_counts = total_counts
         # The users.
         self.users = users
 
     def validate(self):
@@ -12034,15 +12238,15 @@
     def __init__(
         self,
         certificate_id: str = None,
         directory_id: str = None,
     ):
         # The ID of the certificate.
         # 
-        # You can call the [ListExternalSAMLIdPCertificates](~~341629~~) operation to query the IDs of certificates.
+        # You can call the [ListExternalSAMLIdPCertificates](https://help.aliyun.com/document_detail/341629.html) operation to query the IDs of certificates.
         self.certificate_id = certificate_id
         # The ID of the directory.
         self.directory_id = directory_id
 
     def validate(self):
         pass
 
@@ -13955,15 +14159,15 @@
         self.directory_id = directory_id
         # The name of the inline policy.
         self.inline_policy_name = inline_policy_name
         # The new configurations of the inline policy.
         # 
         # The value can be up to 4,096 characters in length.
         # 
-        # For more information about the syntax and structure of RAM policies, see [Policy syntax and structure](~~93739~~).
+        # For more information about the syntax and structure of RAM policies, see [Policy syntax and structure](https://help.aliyun.com/document_detail/93739.html).
         self.new_inline_policy_document = new_inline_policy_document
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14071,15 +14275,15 @@
         operation_for_risk_login: str = None,
     ):
         # The ID of the directory.
         self.directory_id = directory_id
         # Specifies whether to enable MFA for all users. Valid value:
         # 
         # - Enabled: enables MFA for all users.
-        # - Byuser: uses user-specific settings. For more information about how to configure MFA for a single user, see [UpdateUserMFAAuthenticationSettings](~~450135~~).
+        # - Byuser: uses user-specific settings. For more information about how to configure MFA for a single user, see [UpdateUserMFAAuthenticationSettings](https://help.aliyun.com/document_detail/450135.html).
         # - Disabled: disables MFA for all users.
         # - OnlyRiskyLogin: MFA is required only for unusual logons.
         self.mfaauthentication_settings = mfaauthentication_settings
         # Specifies whether MFA is required for users who initiated unusual logons. Valid value:
         # 
         # - Autonomous: MFA is prompted for users who initiated unusual logons. However, the users are allowed to skip MFA. If an MFA device is bound to a user who initiated an unusual logon, the user must pass MFA.
         # 
@@ -14836,16 +15040,16 @@
         # *   KeepBoth: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system creates a RAM user whose username is the username of the CloudSSO user plus the suffix `_sso`.
         # *   TakeOver: When a CloudSSO user is synchronized to RAM, if a RAM user who has the same username as the CloudSSO user exists, the system replaces the RAM user with the CloudSSO user.
         self.duplication_strategy = duplication_strategy
         # The ID of the Alibaba Cloud account to which the resource directory belongs.
         self.owner_pk = owner_pk
         # The identity ID of the RAM user provisioning. Valid values:
         # 
-        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\*\*\*\*\*\*\*\*).
-        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\*\*\*\*\*\*\*\*).
+        # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user group (g-\\*\\*\\*\\*\\*\\*\\*\\*).
+        # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the ID of a CloudSSO user (u-\\*\\*\\*\\*\\*\\*\\*\\*).
         self.principal_id = principal_id
         # The identity name of the RAM user provisioning. Valid values:
         # 
         # *   If `Group` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user group.
         # *   If `User` is returned for the `PrincipalType` parameter, the value of this parameter is the name of a CloudSSO user.
         self.principal_name = principal_name
         # The identity type of the RAM user provisioning. Valid values:
```

### Comparing `alibabacloud_cloudsso20210515-1.5.2/alibabacloud_cloudsso20210515.egg-info/PKG-INFO` & `alibabacloud_cloudsso20210515-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-cloudsso20210515
-Version: 1.5.2
+Name: alibabacloud_cloudsso20210515
+Version: 1.6.0
 Summary: Alibaba Cloud cloudsso (20210515) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudsso20210515-1.5.2/setup.py` & `alibabacloud_cloudsso20210515-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudsso20210515.
 
-Created on 25/04/2024
+Created on 03/06/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudsso20210515"
 NAME = "alibabacloud_cloudsso20210515" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud cloudsso (20210515) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

