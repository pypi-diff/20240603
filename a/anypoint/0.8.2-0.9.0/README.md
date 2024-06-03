# Comparing `tmp/anypoint-0.8.2.tar.gz` & `tmp/anypoint-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anypoint-0.8.2.tar", last modified: Sat Aug  5 06:17:30 2023, max compression
+gzip compressed data, was "anypoint-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `anypoint-0.8.2.tar` & `anypoint-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       43 2023-01-26 15:38:20.500388 anypoint-0.8.2/.gitignore
--rw-r--r--   0        0        0     1099 2022-05-21 00:47:41.295000 anypoint-0.8.2/LICENSE
--rw-r--r--   0        0        0      751 2022-09-07 21:46:25.244226 anypoint-0.8.2/README.md
--rw-r--r--   0        0        0      131 2023-08-05 06:15:49.464558 anypoint-0.8.2/anypoint/__init__.py
--rw-r--r--   0        0        0     2351 2023-03-02 13:59:25.439392 anypoint-0.8.2/anypoint/anypoint.py
--rw-r--r--   0        0        0        0 2022-08-27 14:54:48.596500 anypoint-0.8.2/anypoint/api/__init__.py
--rw-r--r--   0        0        0      745 2023-04-25 15:26:47.707954 anypoint-0.8.2/anypoint/api/api_manager.py
--rw-r--r--   0        0        0     2864 2022-11-09 03:58:06.056091 anypoint-0.8.2/anypoint/api/application.py
--rw-r--r--   0        0        0      244 2022-08-27 15:04:56.867694 anypoint-0.8.2/anypoint/api/environment.py
--rw-r--r--   0        0        0     1466 2023-04-25 15:26:47.739211 anypoint-0.8.2/anypoint/api/monitoring.py
--rw-r--r--   0        0        0     2272 2023-03-02 16:38:46.733880 anypoint-0.8.2/anypoint/api/mq.py
--rw-r--r--   0        0        0     1374 2022-10-27 16:26:23.957360 anypoint-0.8.2/anypoint/api/organization.py
--rw-r--r--   0        0        0     1540 2022-08-28 14:51:16.009115 anypoint-0.8.2/anypoint/authentication.py
--rw-r--r--   0        0        0       93 2022-06-17 22:51:42.220249 anypoint-0.8.2/anypoint/constants.py
--rw-r--r--   0        0        0        0 2022-06-17 21:08:31.328547 anypoint-0.8.2/anypoint/http_client/__init__.py
--rw-r--r--   0        0        0     2246 2023-08-05 06:17:10.822776 anypoint-0.8.2/anypoint/http_client/client.py
--rw-r--r--   0        0        0        0 2022-06-17 20:51:46.804411 anypoint-0.8.2/anypoint/models/__init__.py
--rw-r--r--   0        0        0     1983 2022-10-25 01:24:56.305742 anypoint-0.8.2/anypoint/models/api.py
--rw-r--r--   0        0        0     2591 2022-11-09 03:56:28.180823 anypoint-0.8.2/anypoint/models/application.py
--rw-r--r--   0        0        0     3049 2023-03-05 17:20:15.142643 anypoint-0.8.2/anypoint/models/destination.py
--rw-r--r--   0        0        0     1717 2023-03-02 16:38:29.249783 anypoint-0.8.2/anypoint/models/environment.py
--rw-r--r--   0        0        0     6061 2022-11-23 14:16:51.793610 anypoint-0.8.2/anypoint/models/organization.py
--rw-r--r--   0        0        0     1506 2022-08-29 14:43:07.718672 anypoint-0.8.2/anypoint/models/statistics.py
--rw-r--r--   0        0        0     1672 2022-06-27 22:28:00.338479 anypoint-0.8.2/anypoint/models/worker.py
--rw-r--r--   0        0        0      146 2022-06-17 22:52:02.909907 anypoint-0.8.2/anypoint/utils.py
--rw-r--r--   0        0        0      424 2022-10-24 23:37:47.032214 anypoint-0.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-17 19:46:08.652410 anypoint-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 anypoint-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-04-11 22:27:00.710143 anypoint-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1099 2024-04-11 22:27:00.710143 anypoint-0.9.0/LICENSE
+-rw-r--r--   0        0        0      891 2024-04-11 22:27:00.710143 anypoint-0.9.0/README.md
+-rw-r--r--   0        0        0      131 2024-04-11 23:01:38.943920 anypoint-0.9.0/anypoint/__init__.py
+-rw-r--r--   0        0        0     2351 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/anypoint.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/api/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/api/api_manager.py
+-rw-r--r--   0        0        0     3884 2024-04-12 00:36:02.366137 anypoint-0.9.0/anypoint/api/application.py
+-rw-r--r--   0        0        0      255 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/api/environment.py
+-rw-r--r--   0        0        0     2106 2024-04-11 22:57:44.783165 anypoint-0.9.0/anypoint/api/monitoring.py
+-rw-r--r--   0        0        0     2320 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/api/mq.py
+-rw-r--r--   0        0        0     1410 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/api/organization.py
+-rw-r--r--   0        0        0     1596 2024-04-11 23:45:42.644172 anypoint-0.9.0/anypoint/authentication.py
+-rw-r--r--   0        0        0       96 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/http_client/__init__.py
+-rw-r--r--   0        0        0     2246 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/http_client/client.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:27:00.710143 anypoint-0.9.0/anypoint/models/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-11 22:27:00.725789 anypoint-0.9.0/anypoint/models/api.py
+-rw-r--r--   0        0        0     5018 2024-04-12 00:49:48.624236 anypoint-0.9.0/anypoint/models/application.py
+-rw-r--r--   0        0        0     2859 2024-04-11 22:27:00.725789 anypoint-0.9.0/anypoint/models/destination.py
+-rw-r--r--   0        0        0     2156 2024-04-12 00:30:47.509019 anypoint-0.9.0/anypoint/models/environment.py
+-rw-r--r--   0        0        0     6165 2024-04-11 22:27:00.725789 anypoint-0.9.0/anypoint/models/organization.py
+-rw-r--r--   0        0        0     1552 2024-04-11 22:27:00.725789 anypoint-0.9.0/anypoint/models/statistics.py
+-rw-r--r--   0        0        0     1716 2024-04-11 22:27:00.725789 anypoint-0.9.0/anypoint/models/worker.py
+-rw-r--r--   0        0        0      153 2024-04-11 22:27:00.725789 anypoint-0.9.0/anypoint/utils.py
+-rw-r--r--   0        0        0      424 2024-04-11 22:27:00.725789 anypoint-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 22:27:00.725789 anypoint-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 anypoint-0.9.0/PKG-INFO
```

### Comparing `anypoint-0.8.2/LICENSE` & `anypoint-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.2/anypoint/anypoint.py` & `anypoint-0.9.0/anypoint/anypoint.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.2/anypoint/api/api_manager.py` & `anypoint-0.9.0/anypoint/api/api_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from __future__ import annotations
-
-import logging
-import typing
-from typing import List
-
-
-from anypoint.models.api import Asset
-
-if typing.TYPE_CHECKING:
-    from anypoint import Anypoint
-
-
-class ApiManagerApi:
-    def __init__(self, client: Anypoint, log: logging.Logger):
-        self._client = client
-        self._log = log
-
-    def get_apis(self, organization_id: str, environment_id: str) -> List[Asset]:
-        path = f"/apimanager/api/v1/organizations/{organization_id}/environments/{environment_id}/apis"
-        assets = self._client.request(path).get("assets", [])
-        with open("assets.json", "w") as f:
-            import json
-            json.dump(assets, f, indent=2)
-        return [Asset(asset, self) for asset in assets]
+from __future__ import annotations
+
+import logging
+import typing
+from typing import List
+
+from anypoint.models.api import Asset
+
+if typing.TYPE_CHECKING:
+    from anypoint import Anypoint
+
+
+class ApiManagerApi:
+    def __init__(self, client: Anypoint, log: logging.Logger):
+        self._client = client
+        self._log = log
+
+    def get_apis(self, organization_id: str, environment_id: str) -> List[Asset]:
+        path = f"/apimanager/api/v1/organizations/{organization_id}/environments/{environment_id}/apis"
+        assets = self._client.request(path).get("assets", [])
+        with open("assets.json", "w") as f:
+            import json
+            json.dump(assets, f, indent=2)
+        return [Asset(asset, self) for asset in assets]
```

### Comparing `anypoint-0.8.2/anypoint/api/mq.py` & `anypoint-0.9.0/anypoint/api/mq.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import logging
-from datetime import datetime
-from typing import List, Optional, TYPE_CHECKING
-
-from anypoint.models.destination import Destination, Queue
-
-if TYPE_CHECKING:
-    from anypoint import Anypoint
-
-# Fri, 11 Jul 2015 08:49:37 GMT
-DATE_FORMAT = "%a, %d %b %Y %H:%M:%S %Z"
-
-
-class MQApi:
-
-    def __init__(self, anypoint: "Anypoint", log: logging.Logger):
-        self._client = anypoint
-        self._log = log
-
-    def get_destinations(self, organization_id: str, environment_id: str, region: str) -> List[Destination]:
-        #  https://anypoint.mulesoft.com/mq/admin/api/v1/organizations/{organizationId}/environments/{environmentId}/regions/{regionId}/destinations
-        path = f"/mq/admin/api/v1/organizations/{organization_id}/environments/{environment_id}/regions/{region}/destinations"
-        data = self._client.request(path)
-        return [Destination(d, self._client, organization_id, environment_id, region) for d in data]
-
-    def get_queues(self, organization_id: str, environment_id: str, region: str, destinations: List[str]):
-        # curl -X GET "https://anypoint.mulesoft.com/mq/stats/api/v1/organizations/ORGANIZATION_ID/environments/ENVIRONMENT_ID/regions/REGION_URL/queues?destinationIds=DESTINATION_ID" \
-        path = f"/mq/stats/api/v1/organizations/{organization_id}/environments/{environment_id}/regions/{region}/queues"
-        params = {
-            "destinationIds": ",".join(destinations) if destinations else None
-        }
-        return self._client.request(path, parameters=params)
-
-    def get_queue(self,
-                  organization_id: str,
-                  environment_id: str,
-                  region: str,
-                  destination_id: str,
-                  start_date: Optional[datetime] = None,
-                  end_date: Optional[datetime] = None) -> Queue:
-        path = f"/mq/stats/api/v1/organizations/{organization_id}/environments/{environment_id}/regions/{region}/queues/{destination_id}"
-        params = {
-            "startDate": start_date.strftime(DATE_FORMAT) if start_date else None,
-            "endDate": end_date.strftime(DATE_FORMAT) if end_date else None,
-            "period": 86400
-        }
-        data = self._client.request(path, parameters=params)
-        return Queue(data)
+import logging
+from datetime import datetime
+from typing import List, Optional, TYPE_CHECKING
+
+from anypoint.models.destination import Destination, Queue
+
+if TYPE_CHECKING:
+    from anypoint import Anypoint
+
+# Fri, 11 Jul 2015 08:49:37 GMT
+DATE_FORMAT = "%a, %d %b %Y %H:%M:%S %Z"
+
+
+class MQApi:
+
+    def __init__(self, anypoint: "Anypoint", log: logging.Logger):
+        self._client = anypoint
+        self._log = log
+
+    def get_destinations(self, organization_id: str, environment_id: str, region: str) -> List[Destination]:
+        #  https://anypoint.mulesoft.com/mq/admin/api/v1/organizations/{organizationId}/environments/{environmentId}/regions/{regionId}/destinations
+        path = f"/mq/admin/api/v1/organizations/{organization_id}/environments/{environment_id}/regions/{region}/destinations"
+        data = self._client.request(path)
+        return [Destination(d, self._client, organization_id, environment_id, region) for d in data]
+
+    def get_queues(self, organization_id: str, environment_id: str, region: str, destinations: List[str]):
+        # curl -X GET "https://anypoint.mulesoft.com/mq/stats/api/v1/organizations/ORGANIZATION_ID/environments/ENVIRONMENT_ID/regions/REGION_URL/queues?destinationIds=DESTINATION_ID" \
+        path = f"/mq/stats/api/v1/organizations/{organization_id}/environments/{environment_id}/regions/{region}/queues"
+        params = {
+            "destinationIds": ",".join(destinations) if destinations else None
+        }
+        return self._client.request(path, parameters=params)
+
+    def get_queue(self,
+                  organization_id: str,
+                  environment_id: str,
+                  region: str,
+                  destination_id: str,
+                  start_date: Optional[datetime] = None,
+                  end_date: Optional[datetime] = None) -> Queue:
+        path = f"/mq/stats/api/v1/organizations/{organization_id}/environments/{environment_id}/regions/{region}/queues/{destination_id}"
+        params = {
+            "startDate": start_date.strftime(DATE_FORMAT) if start_date else None,
+            "endDate": end_date.strftime(DATE_FORMAT) if end_date else None,
+            "period": 86400
+        }
+        data = self._client.request(path, parameters=params)
+        return Queue(data)
```

### Comparing `anypoint-0.8.2/anypoint/api/organization.py` & `anypoint-0.9.0/anypoint/api/organization.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import logging
-from typing import Generator, Optional, TYPE_CHECKING
-
-from anypoint.models.environment import Environment
-from anypoint.models.organization import Organization
-
-if TYPE_CHECKING:
-    from anypoint import Anypoint
-
-
-class OrganizationApi:
-    def __init__(self, client: "Anypoint", log: logging.Logger):
-        self._client = client
-        self._log = log
-
-    def get_organization(self, org_id: Optional[str] = None) -> Organization:
-        if org_id is None:
-            data = self._client.me()
-            data = data.get("user", {}).get("organization", {})
-        else:
-            path = f"/accounts/api/organizations/{org_id}"
-            data = self._client.request(path)
-        return Organization(data, self)
-
-    def get_environments(self, organization_id: str) -> Generator[Environment, None, None]:
-        path = f"/accounts/api/organizations/{organization_id}/environments"
-        data = self._client.request(path)
-        for env in data.get("data", []):
-            env["organization_id"] = organization_id
-            yield Environment(env, self._client)
-
-    def get_environment_organization(self, environment_id: str) -> Organization:
-        path = f"/cloudhub/api/organization"
-        headers = {"X-ANYPNT-ENV-ID": environment_id}
-        data = self._client.request(path, headers=headers)
-        return Organization(data, self)
+import logging
+from typing import Generator, Optional, TYPE_CHECKING
+
+from anypoint.models.environment import Environment
+from anypoint.models.organization import Organization
+
+if TYPE_CHECKING:
+    from anypoint import Anypoint
+
+
+class OrganizationApi:
+    def __init__(self, client: "Anypoint", log: logging.Logger):
+        self._client = client
+        self._log = log
+
+    def get_organization(self, org_id: Optional[str] = None) -> Organization:
+        if org_id is None:
+            data = self._client.me()
+            data = data.get("user", {}).get("organization", {})
+        else:
+            path = f"/accounts/api/organizations/{org_id}"
+            data = self._client.request(path)
+        return Organization(data, self)
+
+    def get_environments(self, organization_id: str) -> Generator[Environment, None, None]:
+        path = f"/accounts/api/organizations/{organization_id}/environments"
+        data = self._client.request(path)
+        for env in data.get("data", []):
+            env["organization_id"] = organization_id
+            yield Environment(env, self._client)
+
+    def get_environment_organization(self, environment_id: str) -> Organization:
+        path = f"/cloudhub/api/organization"
+        headers = {"X-ANYPNT-ENV-ID": environment_id}
+        data = self._client.request(path, headers=headers)
+        return Organization(data, self)
```

### Comparing `anypoint-0.8.2/anypoint/http_client/client.py` & `anypoint-0.9.0/anypoint/http_client/client.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.2/anypoint/models/api.py` & `anypoint-0.9.0/anypoint/models/api.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from __future__ import annotations
-
-from typing import List, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from anypoint.api.api_manager import ApiManagerApi
-
-
-class Asset:
-    def __init__(self, raw_json, client: ApiManagerApi):
-        self.id = raw_json.get("id")
-        self.org_id = raw_json.get("organizationId")
-        self.name = raw_json.get("name")
-        self.exchange_asset_name = raw_json.get("exchangeAssetName")
-        self.group_id = raw_json.get("groupId")
-        self.asset_id = raw_json.get("assetId")
-        self.apis: List[Api] = [Api(raw_data, client) for raw_data in raw_json.get("apis", [])]
-
-    def __repr__(self):
-        return f"Asset({self.id}, {self.asset_id})"
-
-
-class Api:
-    def __init__(self, raw_json, client: ApiManagerApi):
-        self.org_id = raw_json.get("organizationId")
-        self.id = raw_json.get("id")
-        self.instance_label = raw_json.get("instanceLabel")
-        self.group_id = raw_json.get("groupId")
-        self.asset_id = raw_json.get("assetId")
-        self.asset_version = raw_json.get("assetVersion")
-        self.product_version = raw_json.get("productVersion")
-        self.description = raw_json.get("description")
-        self.tags = raw_json.get("tags")
-        self.order = raw_json.get("order")
-        self.provider_id = raw_json.get("providerId")
-        self.deprecated = raw_json.get("deprecated")
-        self.last_active_date = raw_json.get("lastActiveDate")
-        self.endpoint_uri = raw_json.get("endpointUri")
-        self.environment_id = raw_json.get("environmentId")
-        self.is_public = raw_json.get("isPublic")
-        self.stage = raw_json.get("stage")
-        self.technology = raw_json.get("technology")
-        self.pinned = raw_json.get("pinned")
-        self.active_contracts_count = raw_json.get("activeContractsCount")
-        self.autodiscovery_instance_name = raw_json.get("autodiscoveryInstanceName")
-
-    def __repr__(self):
-        return f"Api({self.id}, {self.instance_label})"
+from __future__ import annotations
+
+from typing import List, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from anypoint.api.api_manager import ApiManagerApi
+
+
+class Asset:
+    def __init__(self, raw_json, client: ApiManagerApi):
+        self.id = raw_json.get("id")
+        self.org_id = raw_json.get("organizationId")
+        self.name = raw_json.get("name")
+        self.exchange_asset_name = raw_json.get("exchangeAssetName")
+        self.group_id = raw_json.get("groupId")
+        self.asset_id = raw_json.get("assetId")
+        self.apis: List[Api] = [Api(raw_data, client) for raw_data in raw_json.get("apis", [])]
+
+    def __repr__(self):
+        return f"Asset({self.id}, {self.asset_id})"
+
+
+class Api:
+    def __init__(self, raw_json, client: ApiManagerApi):
+        self.org_id = raw_json.get("organizationId")
+        self.id = raw_json.get("id")
+        self.instance_label = raw_json.get("instanceLabel")
+        self.group_id = raw_json.get("groupId")
+        self.asset_id = raw_json.get("assetId")
+        self.asset_version = raw_json.get("assetVersion")
+        self.product_version = raw_json.get("productVersion")
+        self.description = raw_json.get("description")
+        self.tags = raw_json.get("tags")
+        self.order = raw_json.get("order")
+        self.provider_id = raw_json.get("providerId")
+        self.deprecated = raw_json.get("deprecated")
+        self.last_active_date = raw_json.get("lastActiveDate")
+        self.endpoint_uri = raw_json.get("endpointUri")
+        self.environment_id = raw_json.get("environmentId")
+        self.is_public = raw_json.get("isPublic")
+        self.stage = raw_json.get("stage")
+        self.technology = raw_json.get("technology")
+        self.pinned = raw_json.get("pinned")
+        self.active_contracts_count = raw_json.get("activeContractsCount")
+        self.autodiscovery_instance_name = raw_json.get("autodiscoveryInstanceName")
+
+    def __repr__(self):
+        return f"Api({self.id}, {self.instance_label})"
```

### Comparing `anypoint-0.8.2/anypoint/models/destination.py` & `anypoint-0.9.0/anypoint/models/destination.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Optional, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from anypoint import Anypoint
-
-
-class Destination:
-    def __init__(self, raw_json, client: Anypoint, organization_id: str, environment_id: str, region_id: str):
-        self.organization_id = organization_id
-        self.environment_id = environment_id
-        self.region_id = region_id
-
-        self.encrypted: bool = raw_json.get("encrypted")
-        self.type: str = raw_json.get("type")
-        self.queue_id: str = raw_json.get("queueId")
-        self.dead_letter_sources: str = raw_json.get("deadLetterSources")
-        self.fifo: bool = raw_json.get("fifo")
-        self.default_ttl: int = raw_json.get("defaultTtl")
-        self.default_lock_ttl: int = raw_json.get("defaultLockTtl")
-        self.default_delivery_delay: int = raw_json.get("defaultDeliveryDelay")
-        self.max_deliveries: int = raw_json.get("maxDeliveries")
-        self.dead_letter_queue_id: str = raw_json.get("deadLetterQueueId")
-
-        self._data = raw_json
-        self._client = client
-
-    def __repr__(self):
-        return f"Destination({self.queue_id}, {self.type})"
-
-    def get_queue(self, start_date: Optional[datetime] = None, end_date: Optional[datetime] = None):
-        return self._client.mq.get_queue(self.organization_id, self.environment_id, self.region_id, self.queue_id, start_date, end_date)
-
-
-class Queue:
-    def __init__(self, raw_json):
-        # {'destination': 'CUSTOMER-CREATE-SFMC-Q', 'messages': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 144}], 'inflightMessages': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}], 'messagesVisible': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 144}], 'messagesSent': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 57}], 'messagesReceived': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}], 'messagesAcked': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}]}
-        self.destination: str = raw_json.get("destination")
-        # Grab the value of the first item in the list
-        self.messages = raw_json.get("messages", [{}])[0].get("value") if raw_json.get("messages") else 0
-        self.inflight_messages = raw_json.get("inflightMessages", [{}])[0].get("value") if raw_json.get("inflightMessages") else 0
-        self.messages_visible = raw_json.get("messagesVisible", [{}])[0].get("value") if raw_json.get("messagesVisible") else 0
-        self.messages_sent = raw_json.get("messagesSent", [{}])[0].get("value") if raw_json.get("messagesSent") else 0
-        self.messages_received = raw_json.get("messagesReceived", [{}])[0].get("value") if raw_json.get("messagesReceived") else 0
-        self.messages_acked = raw_json.get("messagesAcked", [{}])[0].get("value") if raw_json.get("messagesAcked") else 0
-
-    def __repr__(self):
-        return f"Queue({self.destination}, {self.messages=}, {self.inflight_messages=}, {self.messages_visible=}, {self.messages_sent=}, {self.messages_received=}, {self.messages_acked=})"
+from __future__ import annotations
+
+from datetime import datetime
+from typing import Optional, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from anypoint import Anypoint
+
+
+class Destination:
+    def __init__(self, raw_json, client: Anypoint, organization_id: str, environment_id: str, region_id: str):
+        self.organization_id = organization_id
+        self.environment_id = environment_id
+        self.region_id = region_id
+
+        self.encrypted: bool = raw_json.get("encrypted")
+        self.type: str = raw_json.get("type")
+        self.queue_id: str = raw_json.get("queueId")
+        self.dead_letter_sources: str = raw_json.get("deadLetterSources")
+        self.fifo: bool = raw_json.get("fifo")
+        self.default_ttl: int = raw_json.get("defaultTtl")
+        self.default_lock_ttl: int = raw_json.get("defaultLockTtl")
+        self.default_delivery_delay: int = raw_json.get("defaultDeliveryDelay")
+        self.max_deliveries: int = raw_json.get("maxDeliveries")
+        self.dead_letter_queue_id: str = raw_json.get("deadLetterQueueId")
+
+        self._data = raw_json
+        self._client = client
+
+    def __repr__(self):
+        return f"Destination({self.queue_id}, {self.type})"
+
+    def get_queue(self, start_date: Optional[datetime] = None, end_date: Optional[datetime] = None):
+        return self._client.mq.get_queue(self.organization_id, self.environment_id, self.region_id, self.queue_id, start_date, end_date)
+
+
+class Queue:
+    def __init__(self, raw_json):
+        # {'destination': 'CUSTOMER-CREATE-SFMC-Q', 'messages': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 144}], 'inflightMessages': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}], 'messagesVisible': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 144}], 'messagesSent': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 57}], 'messagesReceived': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}], 'messagesAcked': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}]}
+        self.destination: str = raw_json.get("destination")
+        # Grab the value of the first item in the list
+        self.messages = raw_json.get("messages", [{}])[0].get("value")
+        self.inflight_messages = raw_json.get("inflightMessages", [{}])[0].get("value")
+        self.messages_visible = raw_json.get("messagesVisible", [{}])[0].get("value")
+        self.messages_sent = raw_json.get("messagesSent", [{}])[0].get("value")
+        self.messages_received = raw_json.get("messagesReceived", [{}])[0].get("value")
+        self.messages_acked = raw_json.get("messagesAcked", [{}])[0].get("value")
+
+    def __repr__(self):
+        return f"Queue({self.destination}, {self.messages=}, {self.inflight_messages=}, {self.messages_visible=}, {self.messages_sent=}, {self.messages_received=}, {self.messages_acked=})"
+
```

### Comparing `anypoint-0.8.2/anypoint/models/organization.py` & `anypoint-0.9.0/anypoint/models/organization.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-from typing import List, TYPE_CHECKING
-
-from anypoint.models.environment import Environment
-
-if TYPE_CHECKING:
-    from anypoint.api.organization import OrganizationApi
-
-
-class Organization:
-    def __init__(self, raw_json, client: "OrganizationApi"):
-        self.id: str = raw_json.get("id")
-        self.name: str = raw_json.get("name")
-        self.owner_id: str = raw_json.get("ownerId")
-        self.created_at: str = raw_json.get("createdAt")
-        self.updated_at: str = raw_json.get("updatedAt")
-        self.is_federated: bool = raw_json.get("isFederated")
-        self.org_type: str = raw_json.get("orgType")
-        self.domain: str = raw_json.get("domain")
-        self.is_root: bool = raw_json.get("isRoot")
-        self.is_master: bool = raw_json.get("isMaster")
-        self.mfa_required: str = raw_json.get("mfaRequired")
-        self.entitlements: "Entitlements" = Entitlements(raw_json.get("entitlements", {}))
-
-        self._data = raw_json
-        self._api_client = client
-
-        usage = raw_json.get("usage", {})
-        self.standard_connectors = usage.get("standardConnectors", 0)
-        self.premium_connectors = usage.get("premiumConnectors", 0)
-        self.production_applications = usage.get("productionApplications", 0)
-        self.sandbox_applications = usage.get("sandboxApplications", 0)
-        self.design_applications = usage.get("designApplications", 0)
-        self.production_workers = usage.get("productionWorkers", 0)
-        self.sandbox_workers = usage.get("sandboxWorkers", 0)
-        self.design_workers = usage.get("designWorkers", 0)
-        self.static_ips = usage.get("staticIps", 0)
-        self.vpcs = usage.get("vpcs", 0)
-        self.vpns = usage.get("vpns", 0)
-        self.network_connections = usage.get("networkConnections", 0)
-        self.load_balancers = usage.get("loadbalancers", 0)
-        self.load_balancer_workers = usage.get("loadbalancerWorkers", 0)
-        self.deployment_groups = usage.get("deploymentGroups", 0)
-
-    def get_environments(self) -> List[Environment]:
-        return list(self._api_client.get_environments(self.id))
-
-
-class Entitlements:
-    def __init__(self, raw_json: dict):
-        self.create_environments: bool = raw_json.get("createEnvironments")
-        self.global_deployment: bool = raw_json.get("globalDeployment")
-        self.create_sub_orgs: bool = raw_json.get("createSubOrgs")
-        self.hybrid: dict = raw_json.get("hybrid", {})
-        self.hybrid_insight: bool = raw_json.get("hybridInsight")
-        self.hybrid_auto_discover_properties: bool = raw_json.get("hybridAutoDiscoverProperties")
-        self.v_cores_production: dict = raw_json.get("vCoresProduction", {})
-        self.v_cores_sandbox: dict = raw_json.get("vCoresSandbox", {})
-        self.v_cores_design: dict = raw_json.get("vCoresDesign", {})
-        self.static_ips: dict = raw_json.get("staticIps", {})
-        self.vpcs: dict = raw_json.get("vpcs", {})
-        self.vpns: dict = raw_json.get("vpns", {})
-        self.network_connections: dict = raw_json.get("networkConnections", {})
-        self.worker_logging_override: dict = raw_json.get("workerLoggingOverride", {})
-        self.mq_messages: dict = raw_json.get("mqMessages", {})
-        self.mq_requests: dict = raw_json.get("mqRequests", {})
-        self.object_store_request_units: dict = raw_json.get("objectStoreRequestUnits", {})
-        self.object_store_keys: dict = raw_json.get("objectStoreKeys", {})
-        self.mq_advanced_features: dict = raw_json.get("mqAdvancedFeatures", {})
-        self.gateways: dict = raw_json.get("gateways", {})
-        self.design_center: dict = raw_json.get("designCenter", {})
-        self.partners_production: dict = raw_json.get("partnersProduction", {})
-        self.partners_sandbox: dict = raw_json.get("partnersSandbox", {})
-        self.trading_partners_production: dict = raw_json.get("tradingPartnersProduction", {})
-        self.trading_partners_sandbox: dict = raw_json.get("tradingPartnersSandbox", {})
-        self.load_balancer: dict = raw_json.get("loadBalancer", {})
-        self.external_identity: bool = raw_json.get("externalIdentity", {})
-        self.autoscaling: bool = raw_json.get("autoscaling", {})
-        self.arm_alerts: bool = raw_json.get("armAlerts", {})
-        self.apis: dict = raw_json.get("apis", {})
-        self.api_monitoring: dict = raw_json.get("apiMonitoring", {})
-        self.api_community_manager: dict = raw_json.get("apiCommunityManager", {})
-        self.api_experience_hub: dict = raw_json.get("apiExperienceHub", {})
-        self.monitoring_center: dict = raw_json.get("monitoringCenter", {})
-        self.api_query: dict = raw_json.get("apiQuery", {})
-        self.api_query_c360: dict = raw_json.get("apiQueryC360", {})
-        self.api_governance: dict = raw_json.get("apiGovernance", {})
-        self.crowd: dict = raw_json.get("crowd", {})
-        self.cam: dict = raw_json.get("cam", {})
-        self.exchange2: dict = raw_json.get("exchange2", {})
-        self.crowd_self_service_migration: dict = raw_json.get("crowdSelfServiceMigration", {})
-        self.kpi_dashboard: dict = raw_json.get("kpiDashboard", {})
-        self.pcf: bool = raw_json.get("pcf", {})
-        self.app_viz: bool = raw_json.get("appViz", {})
-        self.runtime_fabric: bool = raw_json.get("runtimeFabric", {})
-        self.anypoint_security_tokenization: dict = raw_json.get("anypointSecurityTokenization", {})
-        self.anypoint_security_edge_policies: dict = raw_json.get("anypointSecurityEdgePolicies", {})
-        self.runtime_fabric_cloud: dict = raw_json.get("runtimeFabricCloud", {})
-        self.service_mesh: dict = raw_json.get("serviceMesh", {})
-        self.flex_gateway: dict = raw_json.get("flexGateway", {})
-        self.api_catalog: dict = raw_json.get("apiCatalog", {})
-        self.composer: dict = raw_json.get("composer", {})
-        self.mule_dx_web_ide: dict = raw_json.get("muleDxWebIde", {})
-        self.messaging: dict = raw_json.get("messaging", {})
-        self.worker_clouds: dict = raw_json.get("workerClouds", {})
+from typing import List, TYPE_CHECKING
+
+from anypoint.models.environment import Environment
+
+if TYPE_CHECKING:
+    from anypoint.api.organization import OrganizationApi
+
+
+class Organization:
+    def __init__(self, raw_json, client: "OrganizationApi"):
+        self.id: str = raw_json.get("id")
+        self.name: str = raw_json.get("name")
+        self.owner_id: str = raw_json.get("ownerId")
+        self.created_at: str = raw_json.get("createdAt")
+        self.updated_at: str = raw_json.get("updatedAt")
+        self.is_federated: bool = raw_json.get("isFederated")
+        self.org_type: str = raw_json.get("orgType")
+        self.domain: str = raw_json.get("domain")
+        self.is_root: bool = raw_json.get("isRoot")
+        self.is_master: bool = raw_json.get("isMaster")
+        self.mfa_required: str = raw_json.get("mfaRequired")
+        self.entitlements: "Entitlements" = Entitlements(raw_json.get("entitlements", {}))
+
+        self._data = raw_json
+        self._api_client = client
+
+        usage = raw_json.get("usage", {})
+        self.standard_connectors = usage.get("standardConnectors", 0)
+        self.premium_connectors = usage.get("premiumConnectors", 0)
+        self.production_applications = usage.get("productionApplications", 0)
+        self.sandbox_applications = usage.get("sandboxApplications", 0)
+        self.design_applications = usage.get("designApplications", 0)
+        self.production_workers = usage.get("productionWorkers", 0)
+        self.sandbox_workers = usage.get("sandboxWorkers", 0)
+        self.design_workers = usage.get("designWorkers", 0)
+        self.static_ips = usage.get("staticIps", 0)
+        self.vpcs = usage.get("vpcs", 0)
+        self.vpns = usage.get("vpns", 0)
+        self.network_connections = usage.get("networkConnections", 0)
+        self.load_balancers = usage.get("loadbalancers", 0)
+        self.load_balancer_workers = usage.get("loadbalancerWorkers", 0)
+        self.deployment_groups = usage.get("deploymentGroups", 0)
+
+    def get_environments(self) -> List[Environment]:
+        return list(self._api_client.get_environments(self.id))
+
+
+class Entitlements:
+    def __init__(self, raw_json: dict):
+        self.create_environments: bool = raw_json.get("createEnvironments")
+        self.global_deployment: bool = raw_json.get("globalDeployment")
+        self.create_sub_orgs: bool = raw_json.get("createSubOrgs")
+        self.hybrid: dict = raw_json.get("hybrid", {})
+        self.hybrid_insight: bool = raw_json.get("hybridInsight")
+        self.hybrid_auto_discover_properties: bool = raw_json.get("hybridAutoDiscoverProperties")
+        self.v_cores_production: dict = raw_json.get("vCoresProduction", {})
+        self.v_cores_sandbox: dict = raw_json.get("vCoresSandbox", {})
+        self.v_cores_design: dict = raw_json.get("vCoresDesign", {})
+        self.static_ips: dict = raw_json.get("staticIps", {})
+        self.vpcs: dict = raw_json.get("vpcs", {})
+        self.vpns: dict = raw_json.get("vpns", {})
+        self.network_connections: dict = raw_json.get("networkConnections", {})
+        self.worker_logging_override: dict = raw_json.get("workerLoggingOverride", {})
+        self.mq_messages: dict = raw_json.get("mqMessages", {})
+        self.mq_requests: dict = raw_json.get("mqRequests", {})
+        self.object_store_request_units: dict = raw_json.get("objectStoreRequestUnits", {})
+        self.object_store_keys: dict = raw_json.get("objectStoreKeys", {})
+        self.mq_advanced_features: dict = raw_json.get("mqAdvancedFeatures", {})
+        self.gateways: dict = raw_json.get("gateways", {})
+        self.design_center: dict = raw_json.get("designCenter", {})
+        self.partners_production: dict = raw_json.get("partnersProduction", {})
+        self.partners_sandbox: dict = raw_json.get("partnersSandbox", {})
+        self.trading_partners_production: dict = raw_json.get("tradingPartnersProduction", {})
+        self.trading_partners_sandbox: dict = raw_json.get("tradingPartnersSandbox", {})
+        self.load_balancer: dict = raw_json.get("loadBalancer", {})
+        self.external_identity: bool = raw_json.get("externalIdentity", {})
+        self.autoscaling: bool = raw_json.get("autoscaling", {})
+        self.arm_alerts: bool = raw_json.get("armAlerts", {})
+        self.apis: dict = raw_json.get("apis", {})
+        self.api_monitoring: dict = raw_json.get("apiMonitoring", {})
+        self.api_community_manager: dict = raw_json.get("apiCommunityManager", {})
+        self.api_experience_hub: dict = raw_json.get("apiExperienceHub", {})
+        self.monitoring_center: dict = raw_json.get("monitoringCenter", {})
+        self.api_query: dict = raw_json.get("apiQuery", {})
+        self.api_query_c360: dict = raw_json.get("apiQueryC360", {})
+        self.api_governance: dict = raw_json.get("apiGovernance", {})
+        self.crowd: dict = raw_json.get("crowd", {})
+        self.cam: dict = raw_json.get("cam", {})
+        self.exchange2: dict = raw_json.get("exchange2", {})
+        self.crowd_self_service_migration: dict = raw_json.get("crowdSelfServiceMigration", {})
+        self.kpi_dashboard: dict = raw_json.get("kpiDashboard", {})
+        self.pcf: bool = raw_json.get("pcf", {})
+        self.app_viz: bool = raw_json.get("appViz", {})
+        self.runtime_fabric: bool = raw_json.get("runtimeFabric", {})
+        self.anypoint_security_tokenization: dict = raw_json.get("anypointSecurityTokenization", {})
+        self.anypoint_security_edge_policies: dict = raw_json.get("anypointSecurityEdgePolicies", {})
+        self.runtime_fabric_cloud: dict = raw_json.get("runtimeFabricCloud", {})
+        self.service_mesh: dict = raw_json.get("serviceMesh", {})
+        self.flex_gateway: dict = raw_json.get("flexGateway", {})
+        self.api_catalog: dict = raw_json.get("apiCatalog", {})
+        self.composer: dict = raw_json.get("composer", {})
+        self.mule_dx_web_ide: dict = raw_json.get("muleDxWebIde", {})
+        self.messaging: dict = raw_json.get("messaging", {})
+        self.worker_clouds: dict = raw_json.get("workerClouds", {})
```

### Comparing `anypoint-0.8.2/anypoint/models/statistics.py` & `anypoint-0.9.0/anypoint/models/statistics.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from datetime import datetime
-from typing import List, Union
-
-
-class Statistic:
-    def __init__(self, timestamp: str, value: int):
-        self.timestamp: datetime = datetime.fromtimestamp(int(timestamp) / 1000)
-        self.value: int = value
-
-    def __repr__(self):
-        return f"Statistic({self.timestamp}, {self.value})"
-
-
-class DashboardStatistics:
-    def __init__(self, data: dict):
-        self.events: List[Statistic] = []
-        for timestamp, value in data.get("events").items():
-            self.events.append(Statistic(timestamp, value))
-
-        self.workers: List[Worker] = []
-        for worker in data.get("workerStatistics"):
-            self.workers.append(Worker(worker))
-
-        self._data = data
-
-    def __repr__(self):
-        return f"DashboardStatistics({self._data})"
-
-
-class WorkerMetric:
-    def __init__(self, metric_id: str, datapoints: Union[dict, float, int]):
-        self.metric_id: str = metric_id
-        self.statistics: List[Statistic] = []
-
-        if not isinstance(datapoints, dict):
-            datapoints = {f"{int(datetime.now().timestamp() * 1000)}": datapoints}
-        for timestamp, value in datapoints.items():
-            self.statistics.append(Statistic(timestamp, value))
-
-
-class Worker:
-    def __init__(self, data: dict):
-        self.id: str = data["id"]
-        self.metrics: List[WorkerMetric] = []
-        for metric_id, datapoints in data.get("statistics", {}).items():
-            self.metrics.append(WorkerMetric(metric_id, datapoints))
+from datetime import datetime
+from typing import List, Union
+
+
+class Statistic:
+    def __init__(self, timestamp: str, value: int):
+        self.timestamp: datetime = datetime.fromtimestamp(int(timestamp) / 1000)
+        self.value: int = value
+
+    def __repr__(self):
+        return f"Statistic({self.timestamp}, {self.value})"
+
+
+class DashboardStatistics:
+    def __init__(self, data: dict):
+        self.events: List[Statistic] = []
+        for timestamp, value in data.get("events").items():
+            self.events.append(Statistic(timestamp, value))
+
+        self.workers: List[Worker] = []
+        for worker in data.get("workerStatistics"):
+            self.workers.append(Worker(worker))
+
+        self._data = data
+
+    def __repr__(self):
+        return f"DashboardStatistics({self._data})"
+
+
+class WorkerMetric:
+    def __init__(self, metric_id: str, datapoints: Union[dict, float, int]):
+        self.metric_id: str = metric_id
+        self.statistics: List[Statistic] = []
+
+        if not isinstance(datapoints, dict):
+            datapoints = {f"{int(datetime.now().timestamp() * 1000)}": datapoints}
+        for timestamp, value in datapoints.items():
+            self.statistics.append(Statistic(timestamp, value))
+
+
+class Worker:
+    def __init__(self, data: dict):
+        self.id: str = data["id"]
+        self.metrics: List[WorkerMetric] = []
+        for metric_id, datapoints in data.get("statistics", {}).items():
+            self.metrics.append(WorkerMetric(metric_id, datapoints))
```

### Comparing `anypoint-0.8.2/anypoint/models/worker.py` & `anypoint-0.9.0/anypoint/models/worker.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from anypoint import Anypoint
-
-
-class Worker:
-    def __init__(self, raw_json, client: "Anypoint"):
-        self.id = raw_json.get("id")
-        self.host = raw_json.get("host")
-        self.port = raw_json.get("port")
-        self.status = raw_json.get("status")
-        self.deployed_region = raw_json.get("deployedRegion")
-
-        self._data = raw_json
-        self._api_client = client
-
-    def __repr__(self):
-        return f"Worker({self.id})"
-
-
-class WorkerStatistic:
-    def __init__(self, raw_json, client: "Anypoint"):
-        self.id = raw_json.get("id")
-        self.disk_read_bytes = self.get_latest_value("diskReadBytes")
-        self.disk_write_bytes = self.get_latest_value("diskWriteBytes")
-        self.network_in = self.get_latest_value("networkIn")
-        self.network_out = self.get_latest_value("networkOut")
-        self.memory_total_used = self.get_latest_value("memoryTotalUsed")
-        self.memory_percent_used = self.get_latest_value("memoryPercentageUsed")
-        self.cpu = self.get_latest_value("cpu")
-        self.memory_total_max = raw_json.get("statistics", {})["memoryTotalMax"] if "memoryTotalMax" in raw_json.get(
-            "statistics", {}) else -1
-
-        self._data = raw_json
-        self._api_client = client
-
-    def get_latest_value(self, metric_name) -> float:
-        if metric_name in self._data["statistics"] and self._data["statistics"][metric_name]:
-            return list(self._data["statistics"][metric_name].values())[-1]
-        return -1
-
-    def __repr__(self):
-        return f"Worker {self.id} CPU: {self.cpu}%, MEM: {self.memory_percent_used:.2f}%"
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from anypoint import Anypoint
+
+
+class Worker:
+    def __init__(self, raw_json, client: "Anypoint"):
+        self.id = raw_json.get("id")
+        self.host = raw_json.get("host")
+        self.port = raw_json.get("port")
+        self.status = raw_json.get("status")
+        self.deployed_region = raw_json.get("deployedRegion")
+
+        self._data = raw_json
+        self._api_client = client
+
+    def __repr__(self):
+        return f"Worker({self.id})"
+
+
+class WorkerStatistic:
+    def __init__(self, raw_json, client: "Anypoint"):
+        self.id = raw_json.get("id")
+        self.disk_read_bytes = self.get_latest_value("diskReadBytes")
+        self.disk_write_bytes = self.get_latest_value("diskWriteBytes")
+        self.network_in = self.get_latest_value("networkIn")
+        self.network_out = self.get_latest_value("networkOut")
+        self.memory_total_used = self.get_latest_value("memoryTotalUsed")
+        self.memory_percent_used = self.get_latest_value("memoryPercentageUsed")
+        self.cpu = self.get_latest_value("cpu")
+        self.memory_total_max = raw_json.get("statistics", {})["memoryTotalMax"] if "memoryTotalMax" in raw_json.get(
+            "statistics", {}) else -1
+
+        self._data = raw_json
+        self._api_client = client
+
+    def get_latest_value(self, metric_name) -> float:
+        if metric_name in self._data["statistics"] and self._data["statistics"][metric_name]:
+            return list(self._data["statistics"][metric_name].values())[-1]
+        return -1
+
+    def __repr__(self):
+        return f"Worker {self.id} CPU: {self.cpu}%, MEM: {self.memory_percent_used:.2f}%"
```

