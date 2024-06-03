# Comparing `tmp/lscsde_workspace_mgmt-0.1.4.tar.gz` & `tmp/lscsde_workspace_mgmt-0.1.5.tar.gz`

## Comparing `lscsde_workspace_mgmt-0.1.4.tar` & `lscsde_workspace_mgmt-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/.git
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/_version.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/exceptions.py
--rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/k8sio.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/managers.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/models.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/objects.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/LICENSE
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/README.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/.git
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/_version.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/exceptions.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/k8sio.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/managers.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/models.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/objects.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/LICENSE
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/README.md
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.5/PKG-INFO
```

### Comparing `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/exceptions.py` & `lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/k8sio.py` & `lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/k8sio.py`

 * *Files 4% similar despite different names*

```diff
@@ -362,20 +362,34 @@
         return [self.adaptor.validate_python(item) for item in result["items"]]
     
     async def list_by_username(self, binding_client : AnalyticsWorkspaceBindingClient, namespace : str, username : str):
         bindings = await binding_client.list_by_username(
             namespace = namespace,
             username = username
             )
-        bound_workspaces = list(set([x.spec.workspace for x in bindings]))
+        bound_workspaces = {x.metadata.name:x.spec for x in bindings}
         workspaces = []
-        for bound_workspace in bound_workspaces:
+        for bound_workspace in bound_workspaces.keys():
             try:
-                workspace = await self.get(namespace = namespace, name = bound_workspace)
-                workspaces.append(workspace)
+                workspace_name : str = bound_workspaces[bound_workspace].workspace
+
+                if workspace_name not in [x.metadata.name for x in workspaces]:
+                    workspace = await self.get(namespace = namespace, name = workspace_name)
+                    
+                    if workspace != None:
+                        if bound_workspaces[bound_workspace].expires < workspace.spec.validity.expires:
+                            workspace.spec.validity.expires = bound_workspaces[bound_workspace].expires
+
+                        workspaces.append(workspace)
+                else:
+                    for workspace in workspaces:
+                        if workspace.metadata.name == workspace_name:
+                            if bound_workspaces[bound_workspace].expires < workspace.spec.validity.expires:
+                                workspace.spec.validity.expires = bound_workspaces[bound_workspace].expires
+    
             except ApiException as e:
                 if e.status == 404:
                     self.log.error(f"Workspace {bound_workspace} referenced by user {username} on {namespace} does not exist")
                 else:
                     raise e    
         
         return workspaces
```

### Comparing `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/managers.py` & `lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from .k8sio import (
     AnalyticsWorkspaceClient,
     AnalyticsWorkspaceBindingClient,
     EventClient,
     PersistentVolumeClaimClient,
     V1ObjectMeta,
     V1Pod
@@ -37,21 +38,21 @@
         permitted_workspaces : dict[str, AnalyticsWorkspace] = {}
         for workspace in workspaces:
             if workspace.metadata.name not in permitted_workspaces:
                 permitted_workspaces[workspace.metadata.name] = workspace
 
         return permitted_workspaces
 
-    async def get_permitted_workspaces(self, namespace : str, username : str):
+    async def get_permitted_workspaces(self, namespace : str, username : str, date_now = datetime.today()):
         permitted_workspaces = await self.get_workspaces_for_user(namespace, username)
         sorted_workspaces = sorted(
             permitted_workspaces.values(), key=lambda x: x.spec.display_name
         )
         converter = AnalyticsWorkspaceConverter()
-        return [converter.to_workspace_dict(item) for item in sorted_workspaces]
+        return [converter.to_workspace_dict(item, date_now = date_now) for item in sorted_workspaces]
         
     async def mount_workspace(self, pod : V1Pod, storage_class_name, mount_prefix, storage_prefix : str = "", read_only : bool = False, mount_path = ""):
         metadata : V1ObjectMeta = pod.metadata
         namespace = metadata.namespace
         name = metadata.name
         workspace_name = metadata.labels.get("workspace")
```

### Comparing `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/models.py` & `lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/models.py`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.4/src/lscsde_workspace_mgmt/objects.py` & `lscsde_workspace_mgmt-0.1.5/src/lscsde_workspace_mgmt/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     JupyterWorkspaceStorage,
     KubernetesMetadata,
     VirtualMachineWorkspaceSpec,
     KubernetesHelper
 )
 
 class AnalyticsWorkspaceConverter:
-    def days_until_expiry(self, time_str):
+    def days_until_expiry(self, time_str, date_now = datetime.today()):
         ws_end_date = datetime.strptime(time_str, "%Y-%m-%d")
-        ws_days_left: timedelta = ws_end_date - datetime.today()
+        ws_days_left: timedelta = ws_end_date - date_now
         return ws_days_left
     
-    def to_workspace_dict(self, workspace : AnalyticsWorkspace):
+    def to_workspace_dict(self, workspace : AnalyticsWorkspace, date_now = datetime.today()):
         contents = {}
         contents["display_name"] = workspace.spec.display_name
         contents["description"] = workspace.spec.description
         
         if workspace.spec.jupyter_workspace:
             contents["kubespawner_override"] = {}
             contents["kubespawner_override"]["image"] = workspace.spec.jupyter_workspace.image
@@ -66,9 +66,9 @@
 
             if workspace.spec.jupyter_workspace.tolerations:
                 contents["kubespawner_override"]["tolerations"] = workspace.spec.jupyter_workspace.tolerations
             
         contents["slug"] = workspace.metadata.name
         contents["start_date"] = workspace.spec.validity.available_from
         contents["end_date"] = workspace.spec.validity.expires
-        contents["ws_days_left"] = self.days_until_expiry(workspace.spec.validity.expires)
+        contents["ws_days_left"] = self.days_until_expiry(workspace.spec.validity.expires, date_now=date_now)
         return contents
```

### Comparing `lscsde_workspace_mgmt-0.1.4/.gitignore` & `lscsde_workspace_mgmt-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.4/LICENSE` & `lscsde_workspace_mgmt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.4/pyproject.toml` & `lscsde_workspace_mgmt-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.4/PKG-INFO` & `lscsde_workspace_mgmt-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lscsde_workspace_mgmt
-Version: 0.1.4
+Version: 0.1.5
 Summary: LSCSDE Workspace Management
 Project-URL: Homepage, https://github.com/lsc-sde/py-lscsde-workspace-mgmt
 Project-URL: Issues, https://github.com/lsc-sde/py-lscsde-workspace-mgmt/issues
 Author-email: Shaun Turner <shaun.turner1@nhs.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

