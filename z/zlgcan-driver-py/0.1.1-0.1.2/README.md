# Comparing `tmp/zlgcan_driver_py-0.1.1.tar.gz` & `tmp/zlgcan_driver_py-0.1.2.tar.gz`

## Comparing `zlgcan_driver_py-0.1.1.tar` & `zlgcan_driver_py-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 zlgcan_driver_py-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     2498 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     2441 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/.gitignore
--rw-r--r--   0     1001      127     7651 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/LICENSE.txt
--rw-r--r--   0     1001      127     2892 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/README.md
--rw-r--r--   0     1001      127       11 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/requirements.txt
--rw-r--r--   0     1001      127    10888 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127       21 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/zlgcan/__init__.py
--rw-r--r--   0     1001      127     8229 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/zlgcan/zlgcan.py
--rw-r--r--   0     1001      127    12717 2024-05-31 10:27:44.000000 zlgcan_driver_py-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127      733 2024-05-31 10:27:41.000000 zlgcan_driver_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 zlgcan_driver_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 zlgcan_driver_py-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     2498 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     2441 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/.gitignore
+-rw-r--r--   0     1001      127     7651 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/LICENSE.txt
+-rw-r--r--   0     1001      127     2892 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/README.md
+-rw-r--r--   0     1001      127       11 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/requirements.txt
+-rw-r--r--   0     1001      127    11023 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127       21 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/zlgcan/__init__.py
+-rw-r--r--   0     1001      127     8248 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/zlgcan/zlgcan.py
+-rw-r--r--   0     1001      127    12717 2024-06-03 01:21:58.000000 zlgcan_driver_py-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127      733 2024-06-03 01:21:53.000000 zlgcan_driver_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 zlgcan_driver_py-0.1.2/PKG-INFO
```

### Comparing `zlgcan_driver_py-0.1.1/.github/workflows/CI.yml` & `zlgcan_driver_py-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `zlgcan_driver_py-0.1.1/.gitignore` & `zlgcan_driver_py-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zlgcan_driver_py-0.1.1/LICENSE.txt` & `zlgcan_driver_py-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zlgcan_driver_py-0.1.1/README.md` & `zlgcan_driver_py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zlgcan_driver_py-0.1.1/src/lib.rs` & `zlgcan_driver_py-0.1.2/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,22 @@
 #[pyclass]
 #[derive(Default, Clone)]
 struct ZDeriveInfoPy {
     pub(crate) canfd: bool,
     pub(crate) channels: u8,
 }
 
+#[pymethods]
+impl ZDeriveInfoPy {
+    #[new]
+    fn new(canfd: bool, channels: u8) -> Self {
+        Self { canfd, channels }
+    }
+}
+
 impl Into<DeriveInfo> for ZDeriveInfoPy {
     fn into(self) -> DeriveInfo {
         DeriveInfo::new(self.canfd, self.channels)
     }
 }
 
 #[pyclass]
```

### Comparing `zlgcan_driver_py-0.1.1/zlgcan/zlgcan.py` & `zlgcan_driver_py-0.1.2/zlgcan/zlgcan.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,25 @@
 
 from can import CanError, CanInitializationError, Message
 from can.bus import LOG
 
 from typing import Optional, Union, Sequence, Deque, Tuple, List, Dict
 try:
     from zlgcan_driver_py import ZCanChlCfgPy, ZCanMessagePy, ZDeriveInfoPy, ZCanChlCfgFactoryWrap, ZCanDriverWrap, \
-        convert_to_python, convert_from_python, set_message_mode, zlgcan_cfg_factory_can, zlgcan_open, zlgcan_device_info, \
-        zlgcan_init_can, zlgcan_clear_can_buffer, zlgcan_send, zlgcan_recv, zlgcan_close
-except ImportError:
+        convert_to_python, convert_from_python, set_message_mode, zlgcan_cfg_factory_can, zlgcan_open, \
+        zlgcan_device_info, zlgcan_init_can, zlgcan_clear_can_buffer, zlgcan_send, zlgcan_recv, zlgcan_close
+except ModuleNotFoundError:
     import sys
     import platform
     _system_bit, _ = platform.architecture()
     _platform = sys.platform
     not_support = CanError(f"The system {_platform}'.'{_system_bit} is not supported!")
-    require_lib = CanError("Please install library zlgcan-driver-py!")
+    require_lib = CanError("Please install library `zlgcan-driver-py`!")
     raise {
-        "win32": {
-            {"32bit": not_support}.get(_system_bit, require_lib)
-        },
+        "win32": {"32bit": not_support}.get(_system_bit, require_lib),
         "darwin": not_support,
         "linux": {"32bit": not_support}.get(_system_bit, require_lib)
     }.get(_platform, not_support)
 
 
 class ZCanTxMode:
     NORMAL = 0  # 正常发送
@@ -196,18 +194,17 @@
         super().shutdown()
         if hasattr(self, "device"):
             zlgcan_close(self.device)
 
     def poll_received_messages(self, timeout):
         for channel in self.channels:
             raw_msgs: list[ZCanMessagePy] = zlgcan_recv(self.device, channel, timeout)
-            # print(len(raw_msgs))
-            for raw_msg in raw_msgs:
-                self.rx_queue.append(convert_to_python(raw_msg))
-            # self.rx_queue.extend(map(lambda raw_msg: convert_to_python(raw_msg), raw_msgs))
+            # for raw_msg in raw_msgs:
+            #     self.rx_queue.append(convert_to_python(raw_msg))
+            self.rx_queue.extend(map(lambda raw_msg: convert_to_python(raw_msg), raw_msgs))
 
     def _recv_from_queue(self) -> Tuple[Message, bool]:
         """Return a message from the internal receive queue"""
         msg = self.rx_queue.popleft()
         return msg, False
 
     def _recv_internal(
@@ -225,22 +222,23 @@
 
             if self.rx_queue:
                 return self._recv_from_queue()
 
         return None, False
 
 
-# with ZCanBus(interface="zlgcan", device_type=ZCANDeviceType.ZCAN_USBCANFD_200U,
-#              configs=[{'bitrate': 500000, 'resistance': 1}, {'bitrate': 1000000, 'resistance': 1}]) as bus:
-#     bus.send(can.Message(
-#         arbitration_id=0x7DF,
-#         is_extended_id=False,
-#         channel=0,
-#         data=[0x02, 0x10, 0x03, ],
-#         dlc=3,
-#     ), tx_mode=ZCanTxMode.SELF_SR)
-#
-#     start = time.monotonic()
-#     while time.monotonic() - start < 0.1:
-#         _msg = bus.recv()
-#         print(_msg)
+if __name__ == '__main__':
+    with ZCanBus(interface="zlgcan", device_type=ZCANDeviceType.ZCAN_USBCANFD_200U,
+                 configs=[{'bitrate': 500000, 'resistance': 1}, {'bitrate': 1000000, 'resistance': 1}]) as bus:
+        # bus.send(can.Message(
+        #     arbitration_id=0x7DF,
+        #     is_extended_id=False,
+        #     channel=0,
+        #     data=[0x02, 0x10, 0x03, ],
+        #     dlc=3,
+        # ), tx_mode=ZCanTxMode.SELF_SR)
+
+        start = time.monotonic()
+        while time.monotonic() - start < 0.1:
+            _msg = bus.recv()
+            print(_msg)
```

### Comparing `zlgcan_driver_py-0.1.1/Cargo.lock` & `zlgcan_driver_py-0.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -153,17 +153,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.84"
+version = "1.0.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
+checksum = "22244ce15aa966053a896d1accb3a6e68469b97c7f33f284b99f0d576879fc23"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -435,15 +435,15 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "zlgcan-driver-py"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "pyo3",
  "zlgcan_common",
  "zlgcan_driver",
 ]
 
 [[package]]
```

### Comparing `zlgcan_driver_py-0.1.1/pyproject.toml` & `zlgcan_driver_py-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zlgcan_driver_py-0.1.1/PKG-INFO` & `zlgcan_driver_py-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zlgcan-driver-py
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: python-can
 License-File: LICENSE.txt
 Summary: Python wrapper for zlgcan-driver-rs.
 Author: Smith Jesse
```

