# Comparing `tmp/circuitpython_tool-0.9.0.tar.gz` & `tmp/circuitpython_tool-0.9.1.tar.gz`

## Comparing `circuitpython_tool-0.9.0.tar` & `circuitpython_tool-0.9.1.tar`

### file list

```diff
@@ -1,48 +1,51 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/.flake8
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/docs/README.md
--rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/docs/images/devices.svg
--rw-r--r--   0        0        0    33937 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/docs/images/usage.svg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/async_iter.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/dirs.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/iter.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/request_cache.py
--rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/cli/__init__.py
--rw-r--r--   0        0        0    10326 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/cli/commands.py
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/cli/params.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/cli/shared_state.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/cli/uf2_commands.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/fs/__init__.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/fs/fs.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/fs/inotify.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/__init__.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/device.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/fake_device.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/partition.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/query.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/real_device.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/shell.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/udev.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/hw/uf2_device.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/static/README.md
--rw-r--r--   0        0        0    25600 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/static/flash_nuke.uf2
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/tools/command_graph.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/tools/inotify_cli.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/tools/shell_completer.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/uf2/__init__.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/uf2/block.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/src/circuitpython_tool/uf2/board.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/test_async_iter.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/test_iter.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/cli/test_commands.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/fs/test_fs.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/fs/test_inotify.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/hw/test_fake_device.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/hw/test_real_device.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/hw/test_udev.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/uf2/test_block.py
--rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/tests/uf2/test_board.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/LICENSE
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/.flake8
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/docs/README.md
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/docs/images/completion_uf2_install.svg
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/docs/images/completion_uf2_locales.svg
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/docs/images/completion_upload.svg
+-rw-r--r--   0        0        0    11162 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/docs/images/devices.svg
+-rw-r--r--   0        0        0    29507 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/docs/images/usage.svg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/async_iter.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/dirs.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/iter.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/request_cache.py
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/cli/__init__.py
+-rw-r--r--   0        0        0    10326 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/cli/commands.py
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/cli/params.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/cli/shared_state.py
+-rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/cli/uf2_commands.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/fs/__init__.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/fs/fs.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/fs/inotify.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/__init__.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/device.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/fake_device.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/partition.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/query.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/real_device.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/shell.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/udev.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/hw/uf2_device.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/static/README.md
+-rw-r--r--   0        0        0    25600 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/static/flash_nuke.uf2
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/tools/command_graph.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/tools/inotify_cli.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/tools/shell_completer.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/uf2/__init__.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/uf2/block.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/src/circuitpython_tool/uf2/board.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/test_async_iter.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/test_iter.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/fs/test_fs.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/fs/test_inotify.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/hw/test_fake_device.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/hw/test_real_device.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/hw/test_udev.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/uf2/test_block.py
+-rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/tests/uf2/test_board.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 circuitpython_tool-0.9.1/PKG-INFO
```

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/async_iter.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/async_iter.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/request_cache.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/request_cache.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/cli/__init__.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/cli/commands.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/cli/commands.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/cli/params.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/cli/params.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/cli/uf2_commands.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/cli/uf2_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
                 output_file.write(chunk)
     finally:
         with get_console().status(
             "Closed destination file. Waiting for copy to complete."
         ):
             output_file.close()
     print("Install complete.")
+    # TODO(dhrosa): Show user status of newly setup device
 
 
 @uf2.command
 @argument("device", type=DeviceParam(), required=True)
 def restart(device: Device) -> None:
     """Restart selected device into UF2 bootloader."""
     print("Selected CircuitPython device: ", device)
```

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/fs/fs.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/fs/fs.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/fs/inotify.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/fs/inotify.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/hw/device.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/hw/device.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/hw/fake_device.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/hw/fake_device.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/hw/partition.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/hw/partition.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/hw/query.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/hw/query.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/hw/real_device.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/hw/real_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Device implementation for real CircuitPython devices."""
 
 import logging
 import os
 import re
 import termios
-from dataclasses import replace
+from dataclasses import dataclass, replace
 from pathlib import Path
 
 from . import partition
 from .device import BootInfo, Device
 from .udev import UsbDevice
 
 logger = logging.getLogger(__name__)
@@ -54,34 +54,51 @@
             raise ValueError(f"Unable to parse board id from line: {board_id_line}")
         return BootInfo(version_match[1], board_id_match[1])
 
     @staticmethod
     def all() -> set["RealDevice"]:
         """Finds all USB CircuitPython devices."""
 
-        # Maps (vendor, model, serial) to RealDevice instances.
-        devices: dict[tuple[str, str, str], RealDevice] = {}
+        @dataclass(frozen=True)
+        class Key:
+            vendor_id: str
+            model_id: str
+            serial: str
+
+            @staticmethod
+            def from_usb_device(usb_device: UsbDevice) -> "Key":
+                return Key(usb_device.vendor_id, usb_device.model_id, usb_device.serial)
 
+        devices: dict[Key, RealDevice] = {}
         usb_devices = UsbDevice.all()
 
         # Find CIRCUITPY partition devices.
         for usb_device in usb_devices:
             if usb_device.partition_label != "CIRCUITPY":
                 continue
             device = RealDevice(
                 vendor=usb_device.vendor,
                 model=usb_device.model,
                 serial=usb_device.serial,
                 partition_path=usb_device.path,
             )
-            devices[device.key] = device
+            devices[Key.from_usb_device(usb_device)] = device
 
         # Find corresponding serial devices.
         for usb_device in usb_devices:
             if not usb_device.is_tty:
                 continue
-            key = usb_device.vendor, usb_device.model, usb_device.serial
+            key = Key.from_usb_device(usb_device)
             if key not in devices:
                 continue
-            devices[key] = replace(devices[key], serial_path=usb_device.path)
+            # Take the descriptor strings from the serial device preferentially.
+            # In my experience with the Raspberry Pi Pico, these strings are
+            # more descriptive too.
+            devices[key] = replace(
+                devices[key],
+                vendor=usb_device.vendor,
+                model=usb_device.model,
+                serial=usb_device.serial,
+                serial_path=usb_device.path,
+            )
 
         return set(devices.values())
```

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/hw/shell.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/hw/shell.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/hw/uf2_device.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/hw/uf2_device.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/static/README.md` & `circuitpython_tool-0.9.1/src/circuitpython_tool/static/README.md`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/static/flash_nuke.uf2` & `circuitpython_tool-0.9.1/src/circuitpython_tool/static/flash_nuke.uf2`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/tools/command_graph.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/tools/command_graph.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/tools/inotify_cli.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/tools/inotify_cli.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/tools/shell_completer.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/tools/shell_completer.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/uf2/block.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/uf2/block.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/src/circuitpython_tool/uf2/board.py` & `circuitpython_tool-0.9.1/src/circuitpython_tool/uf2/board.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/tests/test_async_iter.py` & `circuitpython_tool-0.9.1/tests/test_async_iter.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/tests/cli/test_commands.py` & `circuitpython_tool-0.9.1/tests/cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/tests/fs/test_fs.py` & `circuitpython_tool-0.9.1/tests/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/tests/fs/test_inotify.py` & `circuitpython_tool-0.9.1/tests/fs/test_inotify.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/tests/hw/test_fake_device.py` & `circuitpython_tool-0.9.1/tests/hw/test_fake_device.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/tests/hw/test_udev.py` & `circuitpython_tool-0.9.1/tests/hw/test_udev.py`

 * *Files 22% similar despite different names*

```diff
@@ -53,77 +53,93 @@
 
 def test_db_usb_entries(fake_udev: list[list[str]]) -> None:
     fake_udev.append(
         [
             "E: DEVNAME=/devices/with_serial",
             "E: SUBSYSTEM=block",
             "E: ID_BUS=usb",
+            "E: ID_USB_VENDOR_ID=0001",
             "E: ID_USB_VENDOR=vendor1",
+            "E: ID_USB_MODEL_ID=1000",
             "E: ID_USB_MODEL=model1",
             "E: ID_USB_SERIAL=serial1",
         ]
     )
 
     fake_udev.append(
         [
             "E: DEVNAME=/devices/with_short_serial",
             "E: SUBSYSTEM=block",
             "E: ID_BUS=usb",
+            "E: ID_USB_VENDOR_ID=0002",
             "E: ID_USB_VENDOR=vendor2",
+            "E: ID_USB_MODEL_ID=2000",
             "E: ID_USB_MODEL=model2",
             "E: ID_USB_SERIAL_SHORT=serial2",
         ]
     )
 
     fake_udev.append(
         [
             "E: DEVNAME=/devices/with_fs_label",
             "E: SUBSYSTEM=block",
             "E: ID_BUS=usb",
+            "E: ID_USB_VENDOR_ID=0003",
             "E: ID_USB_VENDOR=vendor3",
+            "E: ID_USB_MODEL_ID=3000",
             "E: ID_USB_MODEL=model3",
             "E: ID_USB_SERIAL=serial3",
             "E: ID_FS_LABEL=fs_label",
         ]
     )
 
     fake_udev.append(
         [
             "E: DEVNAME=/devices/tty",
             "E: SUBSYSTEM=tty",
             "E: ID_BUS=usb",
+            "E: ID_USB_VENDOR_ID=0004",
             "E: ID_USB_VENDOR=vendor4",
+            "E: ID_USB_MODEL_ID=4000",
             "E: ID_USB_MODEL=model4",
             "E: ID_USB_SERIAL=serial4",
         ]
     )
 
     assert UsbDevice.all() == [
         UsbDevice(
             path=Path("/devices/with_serial"),
+            vendor_id="0001",
             vendor="vendor1",
+            model_id="1000",
             model="model1",
             serial="serial1",
             partition_label=None,
         ),
         UsbDevice(
             path=Path("/devices/with_short_serial"),
+            vendor_id="0002",
             vendor="vendor2",
+            model_id="2000",
             model="model2",
             serial="serial2",
             partition_label=None,
         ),
         UsbDevice(
             path=Path("/devices/with_fs_label"),
+            vendor_id="0003",
             vendor="vendor3",
+            model_id="3000",
             model="model3",
             serial="serial3",
             partition_label="fs_label",
         ),
         UsbDevice(
             path=Path("/devices/tty"),
+            vendor_id="0004",
             vendor="vendor4",
+            model_id="4000",
             model="model4",
             serial="serial4",
             is_tty=True,
         ),
     ]
```

### Comparing `circuitpython_tool-0.9.0/tests/uf2/test_block.py` & `circuitpython_tool-0.9.1/tests/uf2/test_block.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/tests/uf2/test_board.py` & `circuitpython_tool-0.9.1/tests/uf2/test_board.py`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/LICENSE` & `circuitpython_tool-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython_tool-0.9.0/pyproject.toml` & `circuitpython_tool-0.9.1/pyproject.toml`

 * *Files identical despite different names*

