# Comparing `tmp/pyftms-0.2.4.tar.gz` & `tmp/pyftms-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftms-0.2.4.tar", max compression
+gzip compressed data, was "pyftms-0.2.5.tar", max compression
```

## Comparing `pyftms-0.2.4.tar` & `pyftms-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11374 2024-06-02 15:02:37.402598 pyftms-0.2.4/LICENSE
--rw-r--r--   0        0        0      792 2024-06-02 15:02:37.402598 pyftms-0.2.4/README.md
--rw-r--r--   0        0        0     1604 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/__init__.py
--rw-r--r--   0        0        0      939 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/__main__.py
--rw-r--r--   0        0        0     3573 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/__init__.py
--rw-r--r--   0        0        0      695 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/__init__.py
--rw-r--r--   0        0        0     8214 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/controller.py
--rw-r--r--   0        0        0     6245 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/event.py
--rw-r--r--   0        0        0     2039 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/backends/updater.py
--rw-r--r--   0        0        0    11045 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/client.py
--rw-r--r--   0        0        0     4841 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/const.py
--rw-r--r--   0        0        0      867 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/__init__.py
--rw-r--r--   0        0        0      599 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/cross_trainer.py
--rw-r--r--   0        0        0      576 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/indoor_bike.py
--rw-r--r--   0        0        0      542 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/rower.py
--rw-r--r--   0        0        0      553 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/machines/treadmill.py
--rw-r--r--   0        0        0    10506 2024-06-02 15:02:37.402598 pyftms-0.2.4/pyftms/client/manager.py
--rw-r--r--   0        0        0      685 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/__init__.py
--rw-r--r--   0        0        0     1216 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/device_info.py
--rw-r--r--   0        0        0     5838 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/features.py
--rw-r--r--   0        0        0     2448 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/client/properties/machine_type.py
--rw-r--r--   0        0        0     1117 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/__init__.py
--rw-r--r--   0        0        0     2530 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/common.py
--rw-r--r--   0        0        0     8956 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/control_point.py
--rw-r--r--   0        0        0     6446 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/machine_status.py
--rw-r--r--   0        0        0      374 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/__init__.py
--rw-r--r--   0        0        0     2823 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/common.py
--rw-r--r--   0        0        0     3075 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/cross_trainer.py
--rw-r--r--   0        0        0     2324 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/indoor_bike.py
--rw-r--r--   0        0        0     2973 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/rower.py
--rw-r--r--   0        0        0     2701 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/realtime_data/treadmill.py
--rw-r--r--   0        0        0     1350 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/spin_down.py
--rw-r--r--   0        0        0     2194 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/models/training_status.py
--rw-r--r--   0        0        0      471 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/__init__.py
--rw-r--r--   0        0        0      783 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/list.py
--rw-r--r--   0        0        0     7662 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/model.py
--rw-r--r--   0        0        0     2080 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/num.py
--rw-r--r--   0        0        0      594 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyftms/serializer/serializer.py
--rw-r--r--   0        0        0      480 2024-06-02 15:02:37.406598 pyftms-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 pyftms-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11374 2024-06-02 16:30:37.024206 pyftms-0.2.5/LICENSE
+-rw-r--r--   0        0        0      792 2024-06-02 16:30:37.024206 pyftms-0.2.5/README.md
+-rw-r--r--   0        0        0     1604 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/__init__.py
+-rw-r--r--   0        0        0      939 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/__main__.py
+-rw-r--r--   0        0        0     3573 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/__init__.py
+-rw-r--r--   0        0        0      695 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/backends/__init__.py
+-rw-r--r--   0        0        0     8214 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/backends/controller.py
+-rw-r--r--   0        0        0     6245 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/backends/event.py
+-rw-r--r--   0        0        0     2039 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/backends/updater.py
+-rw-r--r--   0        0        0    11045 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/client.py
+-rw-r--r--   0        0        0     4841 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/const.py
+-rw-r--r--   0        0        0      867 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/machines/__init__.py
+-rw-r--r--   0        0        0      599 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/machines/cross_trainer.py
+-rw-r--r--   0        0        0      576 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/machines/indoor_bike.py
+-rw-r--r--   0        0        0      542 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/machines/rower.py
+-rw-r--r--   0        0        0      553 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/machines/treadmill.py
+-rw-r--r--   0        0        0    10506 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/manager.py
+-rw-r--r--   0        0        0      685 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/properties/__init__.py
+-rw-r--r--   0        0        0     1216 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/properties/device_info.py
+-rw-r--r--   0        0        0     5838 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/properties/features.py
+-rw-r--r--   0        0        0     2448 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/client/properties/machine_type.py
+-rw-r--r--   0        0        0     1117 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/__init__.py
+-rw-r--r--   0        0        0     2530 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/common.py
+-rw-r--r--   0        0        0     8956 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/control_point.py
+-rw-r--r--   0        0        0     6446 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/machine_status.py
+-rw-r--r--   0        0        0      374 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/realtime_data/__init__.py
+-rw-r--r--   0        0        0     2823 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/realtime_data/common.py
+-rw-r--r--   0        0        0     3075 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/realtime_data/cross_trainer.py
+-rw-r--r--   0        0        0     2324 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/realtime_data/indoor_bike.py
+-rw-r--r--   0        0        0     2973 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/realtime_data/rower.py
+-rw-r--r--   0        0        0     2701 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/realtime_data/treadmill.py
+-rw-r--r--   0        0        0     1350 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/spin_down.py
+-rw-r--r--   0        0        0     2194 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/models/training_status.py
+-rw-r--r--   0        0        0      471 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/serializer/__init__.py
+-rw-r--r--   0        0        0      783 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/serializer/list.py
+-rw-r--r--   0        0        0     7651 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/serializer/model.py
+-rw-r--r--   0        0        0     2080 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/serializer/num.py
+-rw-r--r--   0        0        0      594 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyftms/serializer/serializer.py
+-rw-r--r--   0        0        0      480 2024-06-02 16:30:37.024206 pyftms-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 pyftms-0.2.5/PKG-INFO
```

### Comparing `pyftms-0.2.4/LICENSE` & `pyftms-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/README.md` & `pyftms-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/__init__.py` & `pyftms-0.2.5/pyftms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/__main__.py` & `pyftms-0.2.5/pyftms/__main__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/__init__.py` & `pyftms-0.2.5/pyftms/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/backends/__init__.py` & `pyftms-0.2.5/pyftms/client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/backends/controller.py` & `pyftms-0.2.5/pyftms/client/backends/controller.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/backends/event.py` & `pyftms-0.2.5/pyftms/client/backends/event.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/backends/updater.py` & `pyftms-0.2.5/pyftms/client/backends/updater.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/client.py` & `pyftms-0.2.5/pyftms/client/client.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/const.py` & `pyftms-0.2.5/pyftms/client/const.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/machines/__init__.py` & `pyftms-0.2.5/pyftms/client/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/machines/cross_trainer.py` & `pyftms-0.2.5/pyftms/client/machines/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/machines/indoor_bike.py` & `pyftms-0.2.5/pyftms/client/machines/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/machines/rower.py` & `pyftms-0.2.5/pyftms/client/machines/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/machines/treadmill.py` & `pyftms-0.2.5/pyftms/client/machines/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/manager.py` & `pyftms-0.2.5/pyftms/client/manager.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/properties/__init__.py` & `pyftms-0.2.5/pyftms/client/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/properties/device_info.py` & `pyftms-0.2.5/pyftms/client/properties/device_info.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/properties/features.py` & `pyftms-0.2.5/pyftms/client/properties/features.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/client/properties/machine_type.py` & `pyftms-0.2.5/pyftms/client/properties/machine_type.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/__init__.py` & `pyftms-0.2.5/pyftms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/common.py` & `pyftms-0.2.5/pyftms/models/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/control_point.py` & `pyftms-0.2.5/pyftms/models/control_point.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/machine_status.py` & `pyftms-0.2.5/pyftms/models/machine_status.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/realtime_data/common.py` & `pyftms-0.2.5/pyftms/models/realtime_data/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/realtime_data/cross_trainer.py` & `pyftms-0.2.5/pyftms/models/realtime_data/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/realtime_data/indoor_bike.py` & `pyftms-0.2.5/pyftms/models/realtime_data/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/realtime_data/rower.py` & `pyftms-0.2.5/pyftms/models/realtime_data/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/realtime_data/treadmill.py` & `pyftms-0.2.5/pyftms/models/realtime_data/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/spin_down.py` & `pyftms-0.2.5/pyftms/models/spin_down.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/models/training_status.py` & `pyftms-0.2.5/pyftms/models/training_status.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/serializer/list.py` & `pyftms-0.2.5/pyftms/serializer/list.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/serializer/model.py` & `pyftms-0.2.5/pyftms/serializer/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     def _get_features(cls, features: int) -> tuple[str, ...]:
         result = []
 
         def _get_cls_features(cls):
             for field in dc.fields(cls):
                 meta, tp = cast(ModelMeta, field.metadata), field.type
 
-                if not meta:
+                if not meta or field.name == "code":
                     continue
 
                 if get_origin(tp) in (Optional, Union, UnionType):
                     if (tp := get_args(tp)[0]) is None:
                         raise TypeError("Failed to get first type.")
 
                 if (bit := meta.get("features_bit")) is None or features & (1 << bit):
@@ -187,15 +187,15 @@
                         _get_cls_features(tp)
                         continue
 
                     result.append(field.name)
 
         _get_cls_features(cls)
 
-        return tuple(result[1:])  # skip 'mask' or 'code' field
+        return tuple(result)
 
     def __post_init__(self, *args, **kwargs):
         for field in dc.fields(self):
             if (val := getattr(self, field.name)) is None:
                 continue
 
             meta = cast(ModelMeta, field.metadata)
```

### Comparing `pyftms-0.2.4/pyftms/serializer/num.py` & `pyftms-0.2.5/pyftms/serializer/num.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/pyftms/serializer/serializer.py` & `pyftms-0.2.5/pyftms/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.4/PKG-INFO` & `pyftms-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyftms
-Version: 0.2.4
+Version: 0.2.5
 Summary: PyFTMS - Python Fitness Machine Service client library.
 Author: Sergey V. DUDANOV
 Author-email: sergey.dudanov@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

