# Comparing `tmp/ado_wrapper-1.8.5.tar.gz` & `tmp/ado_wrapper-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.8.5.tar", max compression
+gzip compressed data, was "ado_wrapper-1.9.0.tar", max compression
```

## Comparing `ado_wrapper-1.8.5.tar` & `ado_wrapper-1.9.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.8.5/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.8.5/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.8.5/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.8.5/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.8.5/ado_wrapper/client.py
--rw-r--r--   0        0        0    21892 2024-05-07 18:26:17.266989 ado_wrapper-1.8.5/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3537 2024-05-06 10:01:09.344505 ado_wrapper-1.8.5/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.8.5/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.8.5/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.8.5/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.8.5/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3791 2024-05-06 09:59:23.335964 ado_wrapper-1.8.5/ado_wrapper/resources/agent_pools.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.8.5/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3520 2024-05-15 12:17:11.865100 ado_wrapper-1.8.5/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.8.5/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.8.5/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.8.5/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.8.5/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15632 2024-05-31 16:42:45.204130 ado_wrapper-1.8.5/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.8.5/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.8.5/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.8.5/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10768 2024-05-07 11:42:12.821826 ado_wrapper-1.8.5/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0    12706 2024-05-15 10:28:55.220198 ado_wrapper-1.8.5/ado_wrapper/resources/repo_user_permission.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.8.5/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.8.5/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.8.5/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.8.5/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.8.5/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9459 2024-05-06 09:44:07.348306 ado_wrapper-1.8.5/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.8.5/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.8.5/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-31 16:43:16.418854 ado_wrapper-1.8.5/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.9.0/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.9.0/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.9.0/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.9.0/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.9.0/ado_wrapper/client.py
+-rw-r--r--   0        0        0    23257 2024-06-01 20:49:54.644821 ado_wrapper-1.9.0/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3536 2024-06-03 15:03:53.559820 ado_wrapper-1.9.0/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.9.0/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.9.0/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.9.0/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.9.0/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.9.0/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.9.0/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1226 2024-05-31 17:30:29.723838 ado_wrapper-1.9.0/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3791 2024-06-03 15:02:05.975568 ado_wrapper-1.9.0/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.9.0/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     5269 2024-06-03 15:04:03.232216 ado_wrapper-1.9.0/ado_wrapper/resources/audit_log.py
+-rw-r--r--   0        0        0     3522 2024-06-03 15:04:00.072684 ado_wrapper-1.9.0/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    15269 2024-05-06 13:26:32.155840 ado_wrapper-1.9.0/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.9.0/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.9.0/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3268 2024-05-07 17:20:44.533690 ado_wrapper-1.9.0/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15596 2024-06-03 15:00:47.772746 ado_wrapper-1.9.0/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.9.0/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14012 2024-05-06 16:33:39.036236 ado_wrapper-1.9.0/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.9.0/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10759 2024-06-03 15:02:27.964438 ado_wrapper-1.9.0/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0    12706 2024-05-15 10:28:55.220198 ado_wrapper-1.9.0/ado_wrapper/resources/repo_user_permission.py
+-rw-r--r--   0        0        0     3011 2024-05-31 17:27:55.782517 ado_wrapper-1.9.0/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.9.0/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.9.0/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8326 2024-05-07 18:19:31.197732 ado_wrapper-1.9.0/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.9.0/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9490 2024-06-01 20:39:54.305909 ado_wrapper-1.9.0/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.9.0/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     5003 2024-06-01 20:39:42.825462 ado_wrapper-1.9.0/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-06-03 15:04:41.478047 ado_wrapper-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.9.0/PKG-INFO
```

### Comparing `ado_wrapper-1.8.5/LICENSE` & `ado_wrapper-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/README.md` & `ado_wrapper-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/__main__.py` & `ado_wrapper-1.9.0/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/client.py` & `ado_wrapper-1.9.0/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/dumps.py` & `ado_wrapper-1.9.0/ado_wrapper/dumps.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,41 @@
     "originId": "<32_char_uuid>",
     "displayName": "<First> <Last>",
     "_links": {"self": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Users/<user_descriptor>"}, "memberships": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Memberships/<user_descriptor>"}, "membershipState": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/MembershipStates/<user_descriptor>"}, "storageKey": {"href": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/StorageKeys/<user_descriptor>"}, "avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}},
     "url": "https://vssps.dev.azure.com/{ado_client.org}/_apis/Graph/Users/<user_descriptor>",
     "descriptor": "<user_descriptor>",
 }
 
+AUDIT_LOG_DUMP = {
+    'id': '999999999999999999;00000000-0000-0000-0000-000000000000;00000000-0000-0000-0000-000000000000',
+    'correlationId': '00000000-0000-0000-0000-000000000000',
+    'activityId': '00000000-0000-0000-0000-000000000000',
+    'actorCUID': '00000000-0000-0000-0000-000000000000',
+    'actorUserId': '00000000-0000-0000-0000-000000000000', # Same as above
+    'actorClientId': '00000000-0000-0000-0000-000000000000',
+    'actorUPN': 'first.last@example.com',
+    'authenticationMechanism': 'PAT_Unscoped authorizationId:<32_char_uuid>',
+    'timestamp': '2024-01-01T01:01:01.01Z',
+    'scopeType': 'organization',
+    'scopeDisplayName': '<org_name> (Organization)',
+    'scopeId': '00000000-0000-0000-0000-000000000000',
+    'projectId': '00000000-0000-0000-0000-000000000000',
+    'projectName': None,
+    'ipAddress': '128.128.128.128',
+    'userAgent': 'VSServices/128.128.123456.0 (NetStandard; Linux 5.10.215-203.850.amzn2.x86_64 #1 SMP Tue Apr 23 20:32:19 UTC 2024) VstsAgentCore-l',
+    'actionId': 'Library.AgentAdded', 'data': {...},
+    'details': 'Added agent <agent_name> to pool <pool_name>.',
+    'area': 'Library',
+    'category': 'modify',
+    'categoryDisplayName': 'Modify',
+    'actorDisplayName': 'First Last',
+    'actorImageUrl': 'https://dev.azure.com/vfuk-digital/_apis/GraphProfile/MemberAvatars/<User Descriptor>'
+}
+
+
 BRANCH_DUMP = {
     "name": "refs/heads/test-branch",
     "objectId": "<object_id>",
     "creator": {"displayName": "<First> <Last>", "url": "https://spsprodweu5.vssps.visualstudio.com/<some_id>/_apis/Identities/<user_id>", "_links": {"avatar": {"href": "https://dev.azure.com/{ado_client.org}/_apis/GraphProfile/MemberAvatars/<user_descriptor>"}}, "id": "<user_id>", "uniqueName": "<first.last@company.com>", "imageUrl": "https://dev.azure.com/{ado_client.org}/_api/_common/identityImage?id=<user_id>", "descriptor": "<user_descriptor>"},
     "url": "https://dev.azure.com/{ado_client.org}/{ado_client.project_id}/_apis/git/repositories/<repo_id>/refs?filter=heads%2Ftest-branch",
 }
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/generate_docs.py` & `ado_wrapper-1.9.0/ado_wrapper/generate_docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 sorted_pairs = dict(sorted({string: value for string, value in globals().items() if string[0].isupper()}.items()))
 
 for class_name, value in sorted_pairs.items():
     # if class_name != "Build":
     #     continue
     function_data = {
         key: value for key, value in dict(inspect.getmembers(value)).items()
-        if not key.startswith("_") and key not in ignored_functions and 
+        if not key.startswith("_") and key not in ignored_functions and
         key not in dataclass_attributes(globals()[class_name])  # fmt: skip
     }
     if not function_data:
         continue
     string += f"-----\n# {class_name}\n<details>\n\n```py\n"
     for function_name, function_args in function_data.items():  # fmt: skip
         try:
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.9.0/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.9.0/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.9.0/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ado_wrapper.resources.agent_pools import AgentPool
 from ado_wrapper.resources.annotated_tags import AnnotatedTag
+from ado_wrapper.resources.audit_log import AuditLog
 from ado_wrapper.resources.branches import Branch
 from ado_wrapper.resources.builds import Build, BuildDefinition
 from ado_wrapper.resources.commits import Commit
 from ado_wrapper.resources.environment import Environment, PipelineAuthorisation
 from ado_wrapper.resources.groups import Group
 from ado_wrapper.resources.merge_policies import (
     MergeBranchPolicy,
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/agent_pools.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/agent_pools.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     def get_by_id(cls, ado_client: AdoClient, agent_pool_id: str) -> AgentPool:
         return super().get_by_url(
             ado_client,
             f"/_apis/distributedtask/pools/{agent_pool_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(
-        cls, ado_client: AdoClient, name: str, agent_cloud_id: str | None, auto_provision: bool, auto_size: bool,  # type: ignore[override]
+    def create(  # type: ignore[override]
+        cls, ado_client: AdoClient, name: str, agent_cloud_id: str | None, auto_provision: bool, auto_size: bool,
         auto_update: bool, is_hosted: bool, size: int, target_size: int | None  # fmt: skip
     ) -> AgentPool:
         raise NotImplementedError
         # PAYLOAD = {
         #     "name": name, "agentCloudId": agent_cloud_id, "autoProvision": auto_provision, "autoSize": auto_size,
         #     "autoUpdate": auto_update, "isHosted": is_hosted, "size": size, "targetSize": target_size,
         # }
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/branches.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Literal
 
 from ado_wrapper.state_managed_abc import StateManagedResource
-from ado_wrapper.resources.users import Member 
+from ado_wrapper.resources.users import Member
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 BranchEditableAttribute = Literal["name"]
 
 
@@ -23,18 +23,18 @@
     name: str = field(metadata={"editable": True})
     repo_id: str = field(repr=False)
     creator: Member = field(repr=False)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, str | dict[str, str]]) -> Branch:
         return cls(
-            data["objectId"],
+            str(data["objectId"]),
             data["name"].removeprefix("refs/heads/"),  # type: ignore[union-attr]
             data["url"].split("/")[-2],  # type: ignore[union-attr]
-            Member.from_request_payload(data["creator"]),  # type: ignore[union-attr]
+            Member.from_request_payload(data["creator"]),  # type: ignore[arg-type]
         )
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, repo_id: str, branch_id: str) -> Branch:  # type: ignore[override]
         for branch in cls.get_all_by_repo(ado_client, repo_id):
             if branch.branch_id == branch_id:
                 return branch
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/builds.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/commits.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/environment.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/groups.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/merge_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         if request.status_code == 400:
             raise ConfigurationError(f"Error adding default reviewer {request.text}")
         assert request.status_code == 200, f"Error setting branch policy: {request.text}"
 
     @staticmethod
     def remove_default_reviewer(ado_client: AdoClient, repo_id: str, reviewer_id: str, branch_name: str = "main") -> None:
         policies = MergePolicies.get_default_reviewers_by_repo_id(ado_client, repo_id, branch_name)
-        policy_id = [x for x in policies if x.required_reviewer_id == reviewer_id][0].policy_id if policies is not None else None  # type: ignore[comparison-overlap]  # fmt: skip
+        policy_id = [x for x in policies if x.required_reviewer_id == reviewer_id][0].policy_id if policies is not None else None  # fmt: skip
         if not policy_id:
             return
         request = ado_client.session.delete(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/policy/configurations/{policy_id}?api-version=7.1",
         )
         assert request.status_code == 204, "Error removing required reviewer"
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/projects.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/releases.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/repo.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,16 @@
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> Repo | None:  # type: ignore[return]
-        return cls.get_by_abstract_filter(ado_client, lambda repo: repo.name == repo_name)  # type: ignore[return-type]
+    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> Repo | None:
+        return cls.get_by_abstract_filter(ado_client, lambda repo: repo.name == repo_name)  # type: ignore[attr-defined, return-value]
 
     def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
         request = ado_client.session.get(
             f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?path={file_path}&versionType={'Branch'}&version={branch_name}&api-version=7.1",
         )
         if request.status_code == 404:
             raise ResourceNotFound(f"File {file_path} not found in repo {self.repo_id}")
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/repo_user_permission.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/repo_user_permission.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/searches.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/searches.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     from ado_wrapper.client import AdoClient
 
 SortDirections = Literal["ASC", "DESC"]
 
 
 @dataclass
 class Search:
+    """ https://learn.microsoft.com/en-us/rest/api/azure/devops/search/code-search-results/fetch-code-search-results?view=azure-devops-rest-7.1&tabs=HTTP """
     repository_name: str
     path: str
     file_name: str = field(repr=False)
     project: str = field(repr=False)
     repository_id: str = field(repr=False)
     branch_name: str = field(repr=False)
     matches: list[Hit] = field(default_factory=list, repr=False)
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/teams.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/users.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.9.0/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.9.0/ado_wrapper/state_managed_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, fields
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Callable, Literal
 
 from ado_wrapper.plan_resources.plan_resource import PlannedStateManagedResource
 from ado_wrapper.utils import (
-    DeletionFailed, ResourceAlreadyExists, ResourceNotFound, UpdateFailed,
+    DeletionFailed, ResourceAlreadyExists, ResourceNotFound, UpdateFailed, InvalidPermissionError,
     extract_id, get_internal_field_names, get_resource_variables,  # fmt: skip
 )
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
 
@@ -87,15 +87,15 @@
         if ado_client.plan_mode:
             return PlannedStateManagedResource.create(cls, ado_client, url, payload)
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}" + url
         request = ado_client.session.post(url, json=payload or {})  # Create a brand new dict
         if request.status_code >= 300:
             if request.status_code in [401, 403]:
-                raise PermissionError(f"You do not have permission to create this {cls.__name__}! {request.text}")
+                raise InvalidPermissionError(f"You do not have permission to create this {cls.__name__}! {request.text}")
             if request.status_code == 409:
                 raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
             raise ValueError(f"Error creating {cls.__name__}: {request.status_code} - {request.text}")
         resource = cls.from_request_payload(request.json())
         if refetch:
             resource = cls.get_by_id(ado_client, extract_id(resource))
         ado_client.state_manager.add_resource_to_state(cls.__name__, extract_id(resource), resource.to_json())  # type: ignore[arg-type]
```

### Comparing `ado_wrapper-1.8.5/ado_wrapper/state_manager.py` & `ado_wrapper-1.9.0/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.8.5/ado_wrapper/utils.py` & `ado_wrapper-1.9.0/ado_wrapper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,31 +121,35 @@
     pass
 
 
 class ConfigurationError(Exception):
     pass
 
 
+class InvalidPermissionError(Exception):
+    pass
+
+
 def requires_initialisation(ado_client: "AdoClient") -> None:
     """Certain services/endpoints require the ado_project_id, which isn't set if bypass_initialisation is set to False."""
     if not ado_client.ado_project_id:
         raise ConfigurationError(
             "The client has not been initialised. Please disable `bypass_initialisation` in AdoClient before using this function."
         )
 
 
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
     """This returns a mapping of resource name (str) to the class type of the resource. This is used to dynamically create instances of resources."""
     from ado_wrapper.resources import (  # type: ignore[attr-defined]  # pylint: disable=possibly-unused-variable
-        AgentPool, AnnotatedTag, Branch, Build, BuildDefinition, Commit, Environment, Group, MergePolicies, MergeBranchPolicy,
-        MergePolicyDefaultReviewer, Project, PullRequest, Release, ReleaseDefinition, Repo, BuildRepository, Team,
-        AdoUser, Member, ServiceEndpoint, Reviewer, VariableGroup,  # fmt: skip
+        AgentPool, AnnotatedTag, AuditLog, Branch, Build, BuildDefinition, Commit, Environment, Group, MergePolicies,
+        MergeBranchPolicy, MergePolicyDefaultReviewer, Project, PullRequest, Release, ReleaseDefinition, Repo, BuildRepository,
+        Team, AdoUser, Member, ServiceEndpoint, Reviewer, VariableGroup,  # fmt: skip
     )
 
     return locals()
 
 
 ResourceType = Literal[
-    "AgentPool", "AnnotatedTag", "Branch", "Build", "BuildDefinition", "Commit", "Environment", "Group", "MergePolicies", "MergeBranchPolicy",
-    "MergePolicyDefaultReviewer", "Project", "PullRequest", "Release", "ReleaseDefinition",
+    "AgentPool", "AnnotatedTag", "AuditLog", "Branch", "Build", "BuildDefinition", "Commit", "Environment", "Group", "MergePolicies",
+    "MergeBranchPolicy", "MergePolicyDefaultReviewer", "Project", "PullRequest", "Release", "ReleaseDefinition",
     "Repo", "Team", "AdoUser", "Member", "ServiceEndpoint", "Reviewer", "VariableGroup"  # fmt: skip
 ]
```

### Comparing `ado_wrapper-1.8.5/pyproject.toml` & `ado_wrapper-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.8.5"
+version = "1.9.0"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.8.5/PKG-INFO` & `ado_wrapper-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.8.5
+Version: 1.9.0
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

