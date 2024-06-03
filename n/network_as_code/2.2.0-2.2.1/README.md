# Comparing `tmp/network_as_code-2.2.0.tar.gz` & `tmp/network_as_code-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network_as_code-2.2.0.tar", max compression
+gzip compressed data, was "network_as_code-2.2.1.tar", max compression
```

## Comparing `network_as_code-2.2.0.tar` & `network_as_code-2.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11335 2024-04-26 11:56:06.646438 network_as_code-2.2.0/LICENSE
--rw-r--r--   0        0        0      634 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/__init__.py
--rw-r--r--   0        0        0      635 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/api/__init__.py
--rw-r--r--   0        0        0     6904 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/api/client.py
--rw-r--r--   0        0        0     2445 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/api/congestion_api.py
--rw-r--r--   0        0        0     3931 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/api/device_status_api.py
--rw-r--r--   0        0        0     2026 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/api/location_api.py
--rw-r--r--   0        0        0     5671 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/api/qod_api.py
--rw-r--r--   0        0        0     7400 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/api/slice_api.py
--rw-r--r--   0        0        0     2317 2024-04-26 11:56:06.646438 network_as_code-2.2.0/network_as_code/client.py
--rw-r--r--   0        0        0     2202 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/errors/__init__.py
--rw-r--r--   0        0        0      572 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/errors/error_handler.py
--rw-r--r--   0        0        0      702 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/models/__init__.py
--rw-r--r--   0        0        0     1123 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/models/congestion.py
--rw-r--r--   0        0        0    11867 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/models/device.py
--rw-r--r--   0        0        0     1988 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/models/device_status.py
--rw-r--r--   0        0        0     1257 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/models/location.py
--rw-r--r--   0        0        0     4229 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/models/session.py
--rw-r--r--   0        0        0    15525 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/models/slice.py
--rw-r--r--   0        0        0      766 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/namespaces/__init__.py
--rw-r--r--   0        0        0     2082 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/namespaces/device.py
--rw-r--r--   0        0        0     4853 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/namespaces/device_status.py
--rw-r--r--   0        0        0     3270 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/namespaces/insights.py
--rw-r--r--   0        0        0      855 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/namespaces/namespace.py
--rw-r--r--   0        0        0     1149 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/namespaces/session.py
--rw-r--r--   0        0        0    10644 2024-04-26 11:56:06.650438 network_as_code-2.2.0/network_as_code/namespaces/slice.py
--rw-r--r--   0        0        0     1402 2024-04-26 11:56:06.650438 network_as_code-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 network_as_code-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-06-03 12:00:17.975365 network_as_code-2.2.1/LICENSE
+-rw-r--r--   0        0        0      634 2024-06-03 12:00:17.975365 network_as_code-2.2.1/network_as_code/__init__.py
+-rw-r--r--   0        0        0      635 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/api/__init__.py
+-rw-r--r--   0        0        0     6904 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/api/client.py
+-rw-r--r--   0        0        0     2542 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/api/congestion_api.py
+-rw-r--r--   0        0        0     3299 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/api/device_status_api.py
+-rw-r--r--   0        0        0     2112 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/api/location_api.py
+-rw-r--r--   0        0        0     4803 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/api/qod_api.py
+-rw-r--r--   0        0        0     6996 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/api/slice_api.py
+-rw-r--r--   0        0        0     2317 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/client.py
+-rw-r--r--   0        0        0     2202 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/errors/__init__.py
+-rw-r--r--   0        0        0      572 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/errors/error_handler.py
+-rw-r--r--   0        0        0      702 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/models/__init__.py
+-rw-r--r--   0        0        0     1144 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/models/congestion.py
+-rw-r--r--   0        0        0    11338 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/models/device.py
+-rw-r--r--   0        0        0     2122 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/models/device_status.py
+-rw-r--r--   0        0        0     1313 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/models/location.py
+-rw-r--r--   0        0        0     4094 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/models/session.py
+-rw-r--r--   0        0        0    15610 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/models/slice.py
+-rw-r--r--   0        0        0      766 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/namespaces/__init__.py
+-rw-r--r--   0        0        0     2082 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/namespaces/device.py
+-rw-r--r--   0        0        0     5064 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/namespaces/device_status.py
+-rw-r--r--   0        0        0     3270 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/namespaces/insights.py
+-rw-r--r--   0        0        0      855 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/namespaces/namespace.py
+-rw-r--r--   0        0        0     1149 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/namespaces/session.py
+-rw-r--r--   0        0        0    10778 2024-06-03 12:00:17.979365 network_as_code-2.2.1/network_as_code/namespaces/slice.py
+-rw-r--r--   0        0        0     1103 2024-06-03 12:00:17.979365 network_as_code-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 network_as_code-2.2.1/PKG-INFO
```

### Comparing `network_as_code-2.2.0/LICENSE` & `network_as_code-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/__init__.py` & `network_as_code-2.2.1/network_as_code/errors/error_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .client import NetworkAsCodeClient
 
-__version__ = "2.2.0"
```

### Comparing `network_as_code-2.2.0/network_as_code/api/__init__.py` & `network_as_code-2.2.1/network_as_code/api/__init__.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/api/client.py` & `network_as_code-2.2.1/network_as_code/api/client.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/api/congestion_api.py` & `network_as_code-2.2.1/network_as_code/api/congestion_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import pdb
 from typing import Optional
 import httpx
 
 from ..errors import error_handler
 
 class CongestionAPI:
     def __init__(self, base_url: str, rapid_key: str, rapid_host: str):
         self.client = httpx.Client(
             base_url=base_url,
             headers={"X-RapidAPI-Host": rapid_host, "X-RapidAPI-Key": rapid_key},
         )
 
     def fetch_congestion(self, device, start: Optional[str] = None, end: Optional[str] = None) -> dict:
         body = {
-            "device": device.to_json_dict()
+            "device": device.model_dump(mode='json', by_alias=True, exclude_none=True)
         }
 
         if start:
             body["start"] = start
 
         if end:
             body["end"] = end
@@ -40,15 +41,15 @@
 
         error_handler(response)
 
         return response.json()
 
     def subscribe(self, device, notification_url: str, subscription_expire_time: str, notification_auth_token: Optional[str] = None) -> dict:
         body = {
-            "device": device.to_json_dict(),
+            "device": device.model_dump(mode='json', by_alias=True, exclude_none=True),
             "webhook": {
                 "notificationUrl": notification_url
             },
             "subscriptionExpireTime": subscription_expire_time
         }
 
         if notification_auth_token:
```

### Comparing `network_as_code-2.2.0/network_as_code/api/device_status_api.py` & `network_as_code-2.2.1/network_as_code/api/device_status_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import httpx
 
 from typing import Optional
-import datetime
 
 from ..errors import error_handler
 
 
 def delete_none(_dict):
     """Delete None values recursively from all of the dictionaries"""
     for key, value in list(_dict.items()):
@@ -58,38 +57,26 @@
         assert device.network_access_id != "None"
 
         res = self.client.post(
             "/subscriptions",
             json=delete_none(
                 {
                     "subscriptionDetail": {
-                        "device": {
-                            "phoneNumber": device.phone_number,
-                            "networkAccessIdentifier": device.network_access_identifier,
-                            "ipv4Address": {
-                                "publicAddress": device.ipv4_address.public_address,
-                                "privateAddress": device.ipv4_address.private_address,
-                                "publicPort": device.ipv4_address.public_port,
-                            }
-                            if device.ipv4_address
-                            else None,
-                            "ipv6Address": device.ipv6_address,
-                        },
+                        "device": device.model_dump(mode='json', by_alias=True),
                         "type": event_type,
                     },
                     "maxNumberOfReports": max_number_of_reports,
                     "subscriptionExpireTime": subscription_expire_time,
                     "webhook": {
                         "notificationUrl": notification_url,
                         "notificationAuthToken": notification_auth_token,
                     },
                 }
             ),
         )
-
         error_handler(res)
 
         return res.json()
 
     def get_subscription(self, id: str):
         res = self.client.get(f"/subscriptions/{id}")
```

### Comparing `network_as_code-2.2.0/network_as_code/api/location_api.py` & `network_as_code-2.2.1/network_as_code/api/location_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.client = httpx.Client(
             base_url=base_url,
             headers={"X-RapidAPI-Host": rapid_host, "X-RapidAPI-Key": rapid_key},
         )
 
     def verify_location(self, latitude, longitude, device, radius, max_age=60):
         body = {
-            "device": device.to_json_dict(),
+            "device": device.model_dump(mode='json', by_alias=True, exclude_none=True),
             "area": {
                 "areaType": "Circle",
                 "center": {"latitude": latitude, "longitude": longitude},
                 "radius": radius,
             },
         }
 
@@ -50,15 +50,15 @@
     def __init__(self, base_url: str, rapid_key: str, rapid_host: str):
         self.client = httpx.Client(
             base_url=base_url,
             headers={"X-RapidAPI-Host": rapid_host, "X-RapidAPI-Key": rapid_key},
         )
 
     def get_location(self, device, max_age=60):
-        body = {"device": device.to_json_dict()}
+        body = {"device": device.model_dump(mode='json', by_alias=True, exclude_none=True)}
 
         if max_age:
             body["maxAge"] = cast(int, max_age)
 
         response = self.client.post(url="/retrieve", json=body)
 
         error_handler(response)
```

### Comparing `network_as_code-2.2.0/network_as_code/api/slice_api.py` & `network_as_code-2.2.1/network_as_code/api/slice_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pdb
 from typing import Union
-import json
-import os
 import httpx
 
 from typing import Optional, Any
 from pydantic import BaseModel
 
 from ..errors import error_handler
 
@@ -30,16 +27,16 @@
     A class representing the `Throughput` API field.
 
     #### Public Attributes:
             guaranteed (float): the guaranteed throughput in kbps
             maximum (float): the maximum throughput in kbps
     """
 
-    guaranteed: Optional[float]
-    maximum: Optional[float]
+    guaranteed: Optional[float] = None
+    maximum: Optional[float] = None
 
 
 class SliceAPI:
     def __init__(self, base_url: str, rapid_key: str, rapid_host: str) -> None:
         self.client = httpx.Client(
             base_url=base_url,
             headers={
@@ -63,15 +60,15 @@
             device_downlink_throughput: Optional[Throughput] = None,
             device_uplink_throughput: Optional[Throughput] = None,
             max_data_connections: Optional[int] = None,
             max_devices: Optional[int] = None,
     ):
         body = {
             "networkIdentifier": dict(network_id),
-            "sliceInfo": self.convert_slice_info_obj(slice_info),
+            "sliceInfo": slice_info.model_dump(mode='json', by_alias=True, exclude_none=True),
             "notificationUrl": notification_url,
         }
 
         if name:
             body["name"] = name
 
         if area_of_service:
@@ -83,45 +80,37 @@
         if max_data_connections:
             body["maxDataConnections"] = max_data_connections
 
         if max_devices:
             body["maxDevices"] = max_devices
 
         if slice_downlink_throughput:
-            body["sliceDownlinkThroughput"] = self.convert_throughput_obj(
-                slice_downlink_throughput
-            )
+            body["sliceDownlinkThroughput"] = slice_downlink_throughput.model_dump(mode='json')
 
         if slice_uplink_throughput:
-            body["sliceUplinkThroughput"] = self.convert_throughput_obj(
-                slice_uplink_throughput
-            )
+            body["sliceUplinkThroughput"] = slice_uplink_throughput.model_dump(mode='json')
 
         if device_uplink_throughput:
-            body["deviceUplinkThroughput"] = self.convert_throughput_obj(
-                device_uplink_throughput
-            )
+            body["deviceUplinkThroughput"] = device_uplink_throughput.model_dump(mode='json')
 
         if device_downlink_throughput:
-            body["deviceDownlinkThroughput"] = self.convert_throughput_obj(
-                device_downlink_throughput
-            )
+            body["deviceDownlinkThroughput"] = device_downlink_throughput.model_dump(mode='json')
 
         if modify:
             if name is None:
                 raise ValueError('Name is mandatory for modify')
             response = self.client.put(url=f"/slices/{name}", json=body)
         else:
             response = self.client.post(url="/slices", json=body)
 
         error_handler(response)
 
         return response
 
-    def getAll(self):
+    def get_all(self):
         res = self.client.get(
             url="/slices",
         )
 
         error_handler(res)
 
         return res
@@ -154,28 +143,22 @@
             url=f"/slices/{slice_id}",
         )
 
         error_handler(res)
 
         return res
 
-    def convert_area_of_service_obj(self, areaOfService):
+    def convert_area_of_service_obj(self, area_of_service):
         polygons = []
 
-        for point in areaOfService.polygon:
+        for point in area_of_service.polygon:
             polygons.append({"lat": point.latitude, "lon": point.longitude})
 
         return {"polygon": polygons}
 
-    def convert_slice_info_obj(self, slice_info):
-        return { "serviceType": slice_info.service_type, "differentiator": slice_info.differentiator}
-
-    def convert_throughput_obj(self, throughput: Throughput):
-        return {k: float(v) for k, v in dict(throughput).items()}
-
 
 def delete_none(_dict):
     """Delete None values recursively from all of the dictionaries"""
     for key, value in list(_dict.items()):
         if isinstance(value, dict):
             delete_none(value)
         elif value is None:
@@ -196,16 +179,16 @@
         )
 
     def attach(
         self,
         device,
         slice_id: str,
         traffic_categories: Union[any, None],
-        notificationUrl: Union[str,None],
-        notificationAuthToken: str
+        notification_url: Union[str,None],
+        notification_auth_token: str
     ):
         payload = {
                 "device": {
                         "phoneNumber": device.phone_number,
                         "ipv4Address": {
                             "publicAddress": device.ipv4_address.public_address,
                             "privateAddress": device.ipv4_address.private_address,
@@ -214,16 +197,16 @@
                         "ipv6Address": device.ipv6_address
                     },
                 "sliceId": slice_id,
                 "traffic_categories": {
                     "apps": traffic_categories.apps.__dict__
                 },
                 "webhook": {
-                    "notificationUrl": notificationUrl,
-                    "notificationAuthToken": notificationAuthToken
+                    "notificationUrl": notification_url,
+                    "notificationAuthToken": notification_auth_token
                 }
         }
 
         res = self.client.post(
             url=f"/attachments",
             json=delete_none(payload),
         )
@@ -251,9 +234,7 @@
         return res
 
     def detach(self, id):
         res = self.client.delete(
             url=f"/attachments/{id}"
         )
         error_handler(res)
-
-
```

### Comparing `network_as_code-2.2.0/network_as_code/client.py` & `network_as_code-2.2.1/network_as_code/client.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/errors/__init__.py` & `network_as_code-2.2.1/network_as_code/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/errors/error_handler.py` & `network_as_code-2.2.1/network_as_code/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,8 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .client import NetworkAsCodeClient
 
+__version__ = "2.2.1"
```

### Comparing `network_as_code-2.2.0/network_as_code/models/__init__.py` & `network_as_code-2.2.1/network_as_code/models/__init__.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/models/congestion.py` & `network_as_code-2.2.1/network_as_code/models/congestion.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 from datetime import datetime
 from pydantic import BaseModel, PrivateAttr
 from typing import Optional
 from network_as_code.api.client import APIClient
 
 class CongestionSubscription(BaseModel):
-    id: Optional[str]
+    id: Optional[str] = None
     _api: APIClient = PrivateAttr()
-    starts_at: Optional[datetime]
-    expires_at: Optional[datetime]
+    starts_at: Optional[datetime] = None
+    expires_at: Optional[datetime] = None
 
     def __init__(self, api: APIClient, **data):
         super().__init__(**data)
         self._api = api
 
     def delete(self):
         self._api.congestion.delete_subscription(self.id)
```

### Comparing `network_as_code-2.2.0/network_as_code/models/device.py` & `network_as_code-2.2.1/network_as_code/models/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pdb
-from pydantic import BaseModel, EmailStr, PrivateAttr, ValidationError
+from pydantic import BaseModel, EmailStr, Field, PrivateAttr, ValidationError
 from typing import List, Union, Optional
 from datetime import datetime
 
 
 from ..api import APIClient
 from ..models.session import QoDSession, PortsSpec
 from ..models.location import CivicAddress, Location
 from ..models.congestion import Congestion
 from ..errors import NotFound
 
 class RoamingStatus(BaseModel):
     roaming: bool
-    country_code: Optional[int]
-    country_name: Optional[List[str]]
+    country_code: Optional[int] = None
+    country_name: Optional[List[str]] = None
 
 class Event(BaseModel):
     """
     A class representing the `Event` model.
 
     #### Public Attributes:
             target (float): the `target` of an event object.
@@ -48,17 +48,17 @@
 
     #### Public Attributes:
             public_address (float): the `public_address` of a device IPv4 address object.
             private_address (float): the `private_address` of a device IPv4 address object.
             public_port (Optional[CivicAddress]): the `public_port` of a device IPv4 address object.
     """
 
-    public_address: Optional[str]
-    private_address: Optional[str]
-    public_port: Optional[int]
+    public_address: Optional[str] = Field(None, serialization_alias="publicAddress")
+    private_address: Optional[str] = Field(None, serialization_alias="privateAddress")
+    public_port: Optional[int] = Field(None, serialization_alias="publicPort")
 
 
 class Device(BaseModel):
     """
     A class representing the `Device` model.
 
     #### Private Attributes:
@@ -81,18 +81,18 @@
         get_connectivity (ConnectivityData): Retrieve device connectivity status data
         update_connectivity (ConnectivityData): Update device connectivity status data
         delete_connectivity (): Delete device connectivity status
     """
 
     _api: APIClient = PrivateAttr()
     _sessions: List[QoDSession] = PrivateAttr()
-    network_access_identifier: Union[str, None]
-    phone_number: Union[str, None]
-    ipv4_address: Union[DeviceIpv4Addr, None]
-    ipv6_address: Union[str, None]
+    network_access_identifier: Union[str, None] = Field(None, serialization_alias='networkAccessIdentifier')
+    phone_number: Union[str, None] = Field(None, serialization_alias='phoneNumber')
+    ipv4_address: Union[DeviceIpv4Addr, None] = Field(None, serialization_alias='ipv4Address')
+    ipv6_address: Union[str, None] = Field(None, serialization_alias='ipv6Address')
 
     def __init__(self, api: APIClient, **data) -> None:
         super().__init__(**data)
         self._api = api
         self._sessions = []
 
     @property
@@ -129,18 +129,15 @@
         """
         # Checks if at least one parameter is set
         if not service_ipv4 and not service_ipv6:
             raise ValueError("At least one of IP parameters must be provided")
 
 
         session = self._api.sessions.create_session(
-            self.network_access_identifier,
-            self.ipv4_address,
-            self.ipv6_address,
-            self.phone_number,
+            self,
             profile,
             service_ipv4,
             service_ipv6,
             device_ports,
             service_ports,
             duration,
             notification_url,
@@ -251,25 +248,25 @@
         """
         return self._api.location_verify.verify_location(
             latitude, longitude, self, radius, max_age
         )
 
     def get_connectivity(self):
         """Get the connectivity status for the device as a string"""
-        status = self._api.devicestatus.get_connectivity(self.to_json_dict())["connectivityStatus"]
+        status = self._api.devicestatus.get_connectivity(self.model_dump(mode='json', by_alias=True, exclude_none=True))["connectivityStatus"]
 
         return status
 
     def get_roaming(self) -> RoamingStatus:
         """Get the roaming status for the device
 
         #### Returns
         Object of RoamingStatus class, which contains the roaming status, country code and country name
         """
-        status = self._api.devicestatus.get_roaming(self.to_json_dict())
+        status = self._api.devicestatus.get_roaming(self.model_dump(mode='json', by_alias=True, exclude_none=True))
 
         return RoamingStatus(
             roaming=status["roaming"],
             country_code=status.get("countryCode"),
             country_name=status.get("countryName")
         )
 
@@ -285,30 +282,7 @@
         start = start.isoformat() if isinstance(start, datetime) else start
         end = end.isoformat() if isinstance(end, datetime) else end
 
         json = self._api.congestion.fetch_congestion(self, start=start, end=end)
 
         return Congestion(level=json["level"])
 
-    def to_json_dict(self):
-        json_dict = {}
-
-        if self.network_access_identifier:
-            json_dict["networkAccessIdentifier"] = self.network_access_identifier
-
-        if self.ipv4_address:
-            ipv4_address = {}
-            if self.ipv4_address.public_address:
-                ipv4_address["publicAddress"] = self.ipv4_address.public_address
-            if self.ipv4_address.private_address:
-                ipv4_address["privateAddress"] = self.ipv4_address.private_address
-            if self.ipv4_address.public_port:
-                ipv4_address["publicPort"] = self.ipv4_address.public_port
-            json_dict["ipv4Address"] = ipv4_address
-
-        if self.ipv6_address:
-            json_dict["ipv6Address"] = self.ipv6_address
-
-        if self.phone_number:
-            json_dict["phoneNumber"] = self.phone_number
-
-        return json_dict
```

### Comparing `network_as_code-2.2.0/network_as_code/models/device_status.py` & `network_as_code-2.2.1/network_as_code/models/device_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from datetime import datetime
 from os import access
 from pydantic import BaseModel, EmailStr, PrivateAttr, ValidationError
 from typing import List, Union
 
 from ..api import APIClient
 from ..models.device import Device
 from typing import Optional
@@ -31,20 +32,22 @@
     #### Public Attributes:
         max_num_of_reports (str): Number of notifications until the subscription is available
         notification_url (str): Notification URL for session-related events.
         notification_auth_token (optional): Authorization token for notification sending.
         device (Device): Identifier of the device
     """
 
-    id: Optional[str]
+    id: Optional[str] = None
     _api: APIClient = PrivateAttr()
-    max_num_of_reports: Optional[int]
+    max_num_of_reports: Optional[int] = None
     notification_url: str
-    notification_auth_token: Optional[str]
+    notification_auth_token: Optional[str] = None
     device: Device
+    starts_at: Optional[datetime] = None
+    expires_at: Optional[datetime] = None
 
     def __init__(self, api: APIClient, **data) -> None:
         super().__init__(**data)
         self._api = api
 
     def delete(self) -> None:
         """Delete device connectivity status
```

### Comparing `network_as_code-2.2.0/network_as_code/models/location.py` & `network_as_code-2.2.1/network_as_code/models/location.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 # limitations under the License.
 
 from pydantic import BaseModel
 from typing import Optional
 
 
 class CivicAddress(BaseModel):
-    country: Optional[str]
-    a1: Optional[str]
-    a2: Optional[str]
-    a3: Optional[str]
-    a4: Optional[str]
-    a5: Optional[str]
-    a6: Optional[str]
+    country: Optional[str] = None
+    a1: Optional[str] = None
+    a2: Optional[str] = None
+    a3: Optional[str] = None
+    a4: Optional[str] = None
+    a5: Optional[str] = None
+    a6: Optional[str] = None
 
 
 class Location(BaseModel):
     """
     A class representing the `Location` model.
 
     #### Public Attributes:
             longitude (float): the `longitude` of a location object.
             latitude (float): the `latitude` of a location object.
             civic_address (Optional[CivicAddress]): the `civic_address` of a location object.
     """
 
     longitude: float
     latitude: float
-    civic_address: Optional[CivicAddress]
+    civic_address: Optional[CivicAddress] = None
```

### Comparing `network_as_code-2.2.0/network_as_code/models/session.py` & `network_as_code-2.2.1/network_as_code/models/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pydantic import BaseModel, PrivateAttr, Field
+from pydantic import ConfigDict, BaseModel, PrivateAttr, Field
 
 from typing import Union, List
 
 from network_as_code.api.client import APIClient
 
 from ..errors import error_handler
 
@@ -25,17 +25,16 @@
 ALIASES = {"start": "from", "end": "to"}
 
 
 def alias_generator(name: str) -> str:
     return ALIASES.get(name, name)
 
 
-class PortRange(
-    BaseModel, allow_population_by_field_name=True, alias_generator=alias_generator
-):
+class PortRange(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, alias_generator=alias_generator)
     """
     A class representing the `PortRange` model.
 
     #### Public Attributes:
             start (int): the `start` of a port object.
             end (int): the `end` of a port object.
     """
@@ -77,23 +76,18 @@
         duration (timedelta | None): Returns the duration of a given session.
     #### Static Methods:
         convert_session_model (Session): Returns A `Session` instance.
     """
 
     _api: APIClient = PrivateAttr()
     id: str
-    # device_ip: str
-    # device_ports: Union[PortsSpec, None]
-    # service_ip: str
-    # service_ports: Union[PortsSpec, None]
     profile: str
     status: str
-    started_at: Union[datetime, None]
-    expires_at: Union[datetime, None]
-    # notification_url: Union[str, None]
+    started_at: Union[datetime, None] = None
+    expires_at: Union[datetime, None] = None
 
     def __init__(self, api: APIClient, **data) -> None:
         super().__init__(**data)
         self._api = api
 
     def delete(self):
         """
```

### Comparing `network_as_code-2.2.0/network_as_code/models/slice.py` & `network_as_code-2.2.1/network_as_code/models/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,29 +54,29 @@
     A class representing the `SliceInfo` model.
 
     #### Public Attributes:
             service_type (str): the service type of a slice object, Example: `eMBB`
             differentiator (Optional[str]): the differentiator of a slice object.
     """
 
-    service_type: str
-    differentiator: Optional[str]
+    service_type: str = Field(serialization_alias="serviceType")
+    differentiator: Optional[str] = None
 
 
 class Throughput(BaseModel):
     """
     A class representing the `Throughput` model.
 
     #### Public Attributes:
             guaranteed (float): the guaranteed throughput in kbps
             maximum (float): the maximum throughput in kbps
     """
 
-    guaranteed: Optional[float]
-    maximum: Optional[float]
+    guaranteed: Optional[float] = None
+    maximum: Optional[float] = None
 
 
 class Point(BaseModel):
     """
     A class representing the `Point` model.
 
     #### Public Attributes:
@@ -155,27 +155,27 @@
         on_creation ():
         on_event ():
 
     """
 
     _api: APIClient = PrivateAttr()
     _sessions: List[QoDSession] = PrivateAttr()
-    sid: Optional[str]
+    sid: Optional[str] = None
     state: str
     name: Optional[str] = Field(
         None,
         description='Optional short name for the slice. Must be ASCII characters, digits and dash. Like name of an event, such as "Concert-2029-Big-Arena".',
         min_length=4,
         max_length=64,
-        regex="^[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]$",
+        pattern="^[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]$",
     )
     network_identifier: NetworkIdentifier
     slice_info: SliceInfo
     notification_url: str
-    notification_auth_token: Optional[str]
+    notification_auth_token: Optional[str] = None
     area_of_service: Optional[AreaOfService] = Field(
         None, description="Area which the network slice is intended to serve"
     )
     max_data_connections: Optional[int] = Field(
         None,
         description="Maximum number of data connection sessions in the slice.",
         ge=0,
@@ -403,15 +403,15 @@
 
         Assigns the `service_type` and `differentiator`.
         #### Args:
             sliceInfoDict (Dict[str, str]): A Slice Info object with `service_type` and `differentiator` values.
         """
         if sliceInfoDict:
             return SliceInfo(
-                service_type=sliceInfoDict["serviceType"],
+                service_type=str(sliceInfoDict["serviceType"]),
                 differentiator=sliceInfoDict["differentiator"],
             )
         else:
             return None
 
     @staticmethod
     def area_of_service_from_dict(areaOfServiceDict: Optional[Dict[str, List[Dict[str, float]]]]) -> Optional[AreaOfService]:
```

### Comparing `network_as_code-2.2.0/network_as_code/namespaces/__init__.py` & `network_as_code-2.2.1/network_as_code/namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/namespaces/device.py` & `network_as_code-2.2.1/network_as_code/namespaces/device.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/namespaces/device_status.py` & `network_as_code-2.2.1/network_as_code/namespaces/device_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
+import pdb
 from typing import List, Union
 import math
 from . import Namespace
 from ..models.device import Device, DeviceIpv4Addr
 from ..models.device_status import EventSubscription
 
 from urllib.error import HTTPError
@@ -47,34 +48,35 @@
             notification_url (str): Notification URL for session-related events.
             notification_auth_token (optional): Authorization token for notification sending.
             device (Device): Identifier of the device
             max_num_of_reports (Optional[int]) (deprecated): Number of notifications until the subscription is available
             subscription_expire_time (Union[datetime, str, None]): The expiry time of the subscription. Either a datetime object or ISO formatted date string
         """
 
-        connectivity_subscription = EventSubscription(
-            api=self.api,
-            max_num_of_reports=max_num_of_reports,
-            notification_url=notification_url,
-            notification_auth_token=notification_auth_token,
-            device=device,
-        )
-
         # Handle conversion
         if isinstance(subscription_expire_time, datetime):
             subscription_expire_time = subscription_expire_time.isoformat()
 
         connectivity_data = self.api.devicestatus.create_subscription(
             device,
             event_type,
             notification_url,
             notification_auth_token,
             max_num_of_reports,
             subscription_expire_time,
         )
+        connectivity_subscription = EventSubscription(
+            api=self.api,
+            max_num_of_reports=max_num_of_reports,
+            notification_url=notification_url,
+            notification_auth_token=notification_auth_token,
+            device=device,
+            starts_at=connectivity_data["startsAt"] if "startsAt" in connectivity_data else None,
+            expires_at= connectivity_data["expiresAt"] if "expiresAt" in connectivity_data  else None,
+        )
 
         connectivity_subscription.id = connectivity_data["subscriptionId"]
 
         return connectivity_subscription
 
     def get_subscription(self, id: str) -> EventSubscription:
         """Retrieve a single Device Status event subscription by ID
```

### Comparing `network_as_code-2.2.0/network_as_code/namespaces/insights.py` & `network_as_code-2.2.1/network_as_code/namespaces/insights.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/namespaces/namespace.py` & `network_as_code-2.2.1/network_as_code/namespaces/namespace.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/namespaces/session.py` & `network_as_code-2.2.1/network_as_code/namespaces/session.py`

 * *Files identical despite different names*

### Comparing `network_as_code-2.2.0/network_as_code/namespaces/slice.py` & `network_as_code-2.2.1/network_as_code/namespaces/slice.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             area_of_service = area_of_service,
             notification_url = notification_url
         )
         ```
 
         """
 
-        slice = Slice(
+        new_slice = Slice(
             api=self.api,
             sid=None,
             state="NOT_SUBMITTED",
             name=name,
             network_identifier=network_id,
             slice_info=slice_info,
             notification_url=notification_url,
@@ -124,41 +124,41 @@
                 slice_downlink_throughput=self._to_api_throughput(slice_downlink_throughput),
                 slice_uplink_throughput=self._to_api_throughput(slice_uplink_throughput),
                 device_downlink_throughput=self._to_api_throughput(device_downlink_throughput),
                 device_uplink_throughput=self._to_api_throughput(device_uplink_throughput),
                 max_data_connections=max_data_connections,
                 max_devices=max_devices,
             )
-            slice.sid = slice_data.json().get("csi_id")
-            slice.state = slice_data.json()["state"]
+            new_slice.sid = slice_data.json().get("csi_id")
+            new_slice.state = slice_data.json()["state"]
         except HTTPError as e:
             if e.code == 403:
                 raise AuthenticationException(e)
             elif e.code == 404:
                 raise NotFound(e)
             elif e.code >= 500:
                 raise ServiceError(e)
         except ValidationError as e:
             raise InvalidParameter(e)
 
-        return slice
+        return new_slice
 
     def get(self, id: str) -> Union[Slice, None]:
         """Get network slice by id.
 
         #### Args:
             id (str): Resource id.
 
         #### Example:
             ```python
             fetched_slice = nac_client.slices.get(id)
             ```
         """
         slice_data = self.api.slicing.get(id).json()
-        slice = Slice(
+        existing_slice = Slice(
             api=self.api,
             sid=slice_data.get("csi_id"),
             state=slice_data["state"],
             name=slice_data["slice"]["name"],
             network_identifier=Slice.network_identifier_from_dict(
                 slice_data["slice"]["networkIdentifier"]
             ),
@@ -182,37 +182,37 @@
             device_uplink_throughput=Slice.throughput(
                 slice_data["slice"].get("deviceUplinkThroughput")
             ),
         )
 
         attachments = self.api.slice_attach.get_attachments().json()
 
-        slice_attachments = [attachment for attachment in attachments if attachment['resource']['sliceId'] == slice.name]
+        slice_attachments = [attachment for attachment in attachments if attachment['resource']['sliceId'] == existing_slice.name]
 
-        slice.set_attachments(slice_attachments)
+        existing_slice.set_attachments(slice_attachments)
         
-        return slice
+        return existing_slice
 
     def getAll(self) -> List[Slice]:
         """Get All slices by id.
 
         #### Args:
             None
 
         #### Example:
             ```python
             fetched_slices = nac_client.slices.getAll()
             ```
         """
-        slice_data = self.api.slicing.getAll()
+        slice_data = self.api.slicing.get_all()
 
         
         slices = [
-            self._convert_to_slice_model(slice)
-            for slice in slice_data.json()
+            self._convert_to_slice_model(slice_json)
+            for slice_json in slice_data.json()
         ]
 
         return slices
 
 
     def get_attachment(
         self,
@@ -241,47 +241,47 @@
         #### Example:
             ```python
             nac_client.slices.get_all_attachments()
             ```
         """
         return self.api.slice_attach.get_attachments().json()
 
-    def _convert_to_slice_model(self, slice):
+    def _convert_to_slice_model(self, slice_json):
         slice_instance = Slice(
                 api=self.api,
-                state=slice["state"],
-                name=slice["slice"]["name"],
-                sid=slice.get("csi_id"),
+                state=slice_json["state"],
+                name=slice_json["slice"]["name"],
+                sid=slice_json.get("csi_id"),
                 network_identifier=Slice.network_identifier_from_dict(
-                    slice["slice"]["networkIdentifier"]
+                    slice_json["slice"]["networkIdentifier"]
                 ),
-                slice_info=Slice.slice_info_from_dict(slice["slice"]["sliceInfo"]),
-                notification_url=slice["slice"]["notificationUrl"],
+                slice_info=Slice.slice_info_from_dict(slice_json["slice"]["sliceInfo"]),
+                notification_url=slice_json["slice"]["notificationUrl"],
                 area_of_service=Slice.area_of_service_from_dict(
-                    slice["slice"].get("areaOfService")
+                    slice_json["slice"].get("areaOfService")
                 ),
-                max_data_connections=slice["slice"].get("maxDataConnections"),
-                max_devices=slice["slice"].get("maxDevices"),
+                max_data_connections=slice_json["slice"].get("maxDataConnections"),
+                max_devices=slice_json["slice"].get("maxDevices"),
                 slice_downlink_throughput=Slice.throughput(
-                    slice["slice"].get("sliceDownlinkThroughput")
+                    slice_json["slice"].get("sliceDownlinkThroughput")
                 ),
                 slice_uplink_throughput=Slice.throughput(
-                    slice["slice"].get("sliceUplinkThroughput")
+                    slice_json["slice"].get("sliceUplinkThroughput")
                 ),
                 device_downlink_throughput=Slice.throughput(
-                    slice["slice"].get("deviceDownlinkThroughput")
+                    slice_json["slice"].get("deviceDownlinkThroughput")
                 ),
                 device_uplink_throughput=Slice.throughput(
-                    slice["slice"].get("deviceUplinkThroughput")
+                    slice_json["slice"].get("deviceUplinkThroughput")
                 ),
             )
         
         attachments = self.api.slice_attach.get_attachments().json()
         
         slice_attachments = [attachment for attachment in attachments if attachment['resource']['sliceId'] == slice_instance.name]
 
         slice_instance.set_attachments(slice_attachments)
 
         return slice_instance
         
         
-        
+
```

### Comparing `network_as_code-2.2.0/pyproject.toml` & `network_as_code-2.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 [tool.poetry]
 name = "network_as_code"
-version = "2.2.0"
+version = "2.2.1"
 description = ""
 authors = ["Sami Lahtinen <sami.lahtinen@nokia.com>", "Pavel Garmuyev <pavel.garmuyev@nokia.com>"]
 packages = [
     { include = "network_as_code" },
 ]
 license = "Apache-2.0"
 
-[[tool.poetry.source]]
-name = "internal"
-url = "https://repo.lab.pl.alcatel-lucent.com/api/pypi/python/simple/"
-priority = "default"
-
-[[tool.poetry.source]]
-name = "extra"
-url = "https://artifactory-espoo1.int.net.nokia.com/artifactory/api/pypi/hybrid-pypi-local/simple"
-priority = "supplemental"
-
 [tool.pyright]
 include = ["network_as_code"]
 exclude = ["**/__pycache__", "**/.pytest_cache", "**/.*"]
 pythonVersion = "^3.9"
 pythonPlatform = "Linux"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = {extras = ["email"], version = "^1.10.2"}
+pydantic = {extras = ["email"], version = "^2.7.1"}
 httpx = "^0.24.1"
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.271"
 pytest-asyncio = "^0.19.0"
 pdoc = "^13.0.0"
 pytest = "^7.2.2"
```

### Comparing `network_as_code-2.2.0/PKG-INFO` & `network_as_code-2.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: network_as_code
-Version: 2.2.0
+Version: 2.2.1
 Summary: 
 License: Apache-2.0
 Author: Sami Lahtinen
 Author-email: sami.lahtinen@nokia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: pydantic[email] (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic[email] (>=2.7.1,<3.0.0)
```

