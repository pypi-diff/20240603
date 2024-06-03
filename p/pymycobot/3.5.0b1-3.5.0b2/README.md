# Comparing `tmp/pymycobot-3.5.0b1.tar.gz` & `tmp/pymycobot-3.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.5.0b1.tar", last modified: Wed May 15 03:50:54 2024, max compression
+gzip compressed data, was "pymycobot-3.5.0b2.tar", last modified: Mon Jun  3 01:45:00 2024, max compression
```

## Comparing `pymycobot-3.5.0b1.tar` & `pymycobot-3.5.0b2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.556720 pymycobot-3.5.0b1/
--rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/LICENSE
--rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0    63942 2024-05-15 03:50:54.555721 pymycobot-3.5.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.5.0b1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.519817 pymycobot-3.5.0b1/pymycobot/
--rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     2171 2024-05-15 03:49:56.000000 pymycobot-3.5.0b1/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.5.0b1/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    25589 2024-05-14 06:55:47.000000 pymycobot-3.5.0b1/pymycobot/common.py
--rw-rw-rw-   0        0        0    12842 2024-05-11 02:01:09.000000 pymycobot-3.5.0b1/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/error.py
--rw-rw-rw-   0        0        0    42593 2024-05-11 08:44:46.000000 pymycobot-3.5.0b1/pymycobot/generate.py
--rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.5.0b1/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.5.0b1/pymycobot/log.py
--rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.5.0b1/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mecharmsocket.py
--rw-rw-rw-   0        0        0    14353 2024-05-15 03:44:23.000000 pymycobot-3.5.0b1/pymycobot/mercury.py
--rw-rw-rw-   0        0        0    26397 2024-05-15 03:44:49.000000 pymycobot-3.5.0b1/pymycobot/mercury_api.py
--rw-rw-rw-   0        0        0     6460 2024-04-25 03:16:52.000000 pymycobot-3.5.0b1/pymycobot/mercurychassis.py
--rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.5.0b1/pymycobot/mercurysocket.py
--rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.5.0b1/pymycobot/myagv.py
--rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    16475 2024-05-07 11:28:46.000000 pymycobot-3.5.0b1/pymycobot/myarm_api.py
--rw-rw-rw-   0        0        0      273 2024-04-22 09:29:51.000000 pymycobot-3.5.0b1/pymycobot/myarmc.py
--rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.5.0b1/pymycobot/myarmm.py
--rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/myarmsocket.py
--rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4544 2024-05-13 10:58:22.000000 pymycobot-3.5.0b1/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0    87447 2024-05-11 02:01:09.000000 pymycobot-3.5.0b1/pymycobot/mycobotpro630.py
--rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.5.0b1/pymycobot/public.py
--rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.5.0b1/pymycobot/robot_limit.json
--rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.5.0b1/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.5.0b1/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.554722 pymycobot-3.5.0b1/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    63942 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1093 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 03:50:54.000000 pymycobot-3.5.0b1/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.5.0b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 03:50:54.557721 pymycobot-3.5.0b1/setup.cfg
--rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.5.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 03:50:54.552724 pymycobot-3.5.0b1/tests/
--rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_api.py
--rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_generator.py
--rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_socket.py
--rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.5.0b1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:45:00.023916 pymycobot-3.5.0b2/
+-rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.5.0b2/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.5.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0    63942 2024-06-03 01:45:00.022915 pymycobot-3.5.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.5.0b2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 01:44:59.944405 pymycobot-3.5.0b2/pymycobot/
+-rw-rw-rw-   0        0        0    35096 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     2171 2024-06-03 01:44:41.000000 pymycobot-3.5.0b2/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.5.0b2/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    25779 2024-05-31 10:41:11.000000 pymycobot-3.5.0b2/pymycobot/common.py
+-rw-rw-rw-   0        0        0    12842 2024-05-16 06:06:28.000000 pymycobot-3.5.0b2/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0    16504 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/error.py
+-rw-rw-rw-   0        0        0    42593 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.5.0b2/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.5.0b2/pymycobot/log.py
+-rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.5.0b2/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8459 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mecharmsocket.py
+-rw-rw-rw-   0        0        0     1237 2024-05-30 06:59:16.000000 pymycobot-3.5.0b2/pymycobot/mercury.py
+-rw-rw-rw-   0        0        0    37222 2024-05-31 10:46:19.000000 pymycobot-3.5.0b2/pymycobot/mercury_api.py
+-rw-rw-rw-   0        0        0     6460 2024-05-16 06:06:28.000000 pymycobot-3.5.0b2/pymycobot/mercurychassis.py
+-rw-rw-rw-   0        0        0     6944 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mercurysocket.py
+-rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.5.0b2/pymycobot/myagv.py
+-rw-rw-rw-   0        0        0    11294 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    16475 2024-05-30 05:49:28.000000 pymycobot-3.5.0b2/pymycobot/myarm_api.py
+-rw-rw-rw-   0        0        0      273 2024-05-16 06:06:28.000000 pymycobot-3.5.0b2/pymycobot/myarmc.py
+-rw-rw-rw-   0        0        0     3186 2024-05-16 06:06:28.000000 pymycobot-3.5.0b2/pymycobot/myarmm.py
+-rw-rw-rw-   0        0        0     8871 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/myarmsocket.py
+-rw-rw-rw-   0        0        0    15120 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     6123 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4544 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     9844 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     9524 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0    87447 2024-05-30 05:49:28.000000 pymycobot-3.5.0b2/pymycobot/mycobotpro630.py
+-rw-rw-rw-   0        0        0     8955 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     9916 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     8607 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.5.0b2/pymycobot/public.py
+-rw-rw-rw-   0        0        0     4052 2024-05-30 05:49:28.000000 pymycobot-3.5.0b2/pymycobot/robot_limit.json
+-rw-rw-rw-   0        0        0    22021 2024-05-30 05:49:32.000000 pymycobot-3.5.0b2/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.5.0b2/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:45:00.020916 pymycobot-3.5.0b2/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    63942 2024-06-03 01:44:59.000000 pymycobot-3.5.0b2/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1093 2024-06-03 01:44:59.000000 pymycobot-3.5.0b2/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 01:44:59.000000 pymycobot-3.5.0b2/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-06-03 01:44:59.000000 pymycobot-3.5.0b2/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-03 01:44:59.000000 pymycobot-3.5.0b2/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2024-05-16 06:06:28.000000 pymycobot-3.5.0b2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 01:45:00.024916 pymycobot-3.5.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2024-05-16 06:06:28.000000 pymycobot-3.5.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 01:45:00.018913 pymycobot-3.5.0b2/tests/
+-rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.5.0b2/tests/test_api.py
+-rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.5.0b2/tests/test_generator.py
+-rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.5.0b2/tests/test_socket.py
+-rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.5.0b2/tests/test_utils.py
```

### Comparing `pymycobot-3.5.0b1/LICENSE` & `pymycobot-3.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/PKG-INFO` & `pymycobot-3.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.5.0b1
+Version: 3.5.0b2
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.5.0b1/README.md` & `pymycobot-3.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/Interface.py` & `pymycobot-3.5.0b2/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/__init__.py` & `pymycobot-3.5.0b2/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.5.0b1"
+__version__ = "3.5.0b2"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.5.0b1/pymycobot/bluet.py` & `pymycobot-3.5.0b2/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/common.py` & `pymycobot-3.5.0b2/pymycobot/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     READ_NEXT_ERROR = 0x15
     SET_FRESH_MODE = 0x16
     GET_FRESH_MODE = 0x17
     SET_FREE_MODE = 0x1A
     IS_FREE_MODE = 0x1B
     COBOTX_GET_ANGLE = 0x1C
     COBOTX_IS_GO_ZERO = 0x1D
+    SET_CONTROL_MODE = 0x1E
+    GET_CONTROL_MODE = 0x1F
     FOCUS_ALL_SERVOS = 0x18
     GO_ZERO = 0x19
     SET_BREAK = 0x19
 
     # MDI MODE AND OPERATION
     GET_ANGLES = 0x20
     SEND_ANGLE = 0x21
@@ -123,14 +125,20 @@
     SET_COLOR_MYARM = 0x70
     SET_ELETRIC_GRIPPER = 0x6B
     INIT_ELETRIC_GRIPPER = 0x6C
     SET_GRIPPER_MODE = 0x6D
     GET_GRIPPER_MODE = 0x6E
 
     GET_ACCEI_DATA = 0x73
+    SET_COLLISION_MODE = 0x74
+    SET_COLLISION_THRESHOLD = 0x75
+    GET_COLLISION_THRESHOLD = 0x76
+    SET_TORQUE_COMP = 0x77
+    GET_TORQUE_COMP = 0x78
+    
 
     # Basic
     SET_BASIC_OUTPUT = 0xA0
     GET_BASIC_INPUT = 0xA1
     GET_BASE_INPUT = 0xA2
     MERCURY_ROBOT_STATUS = 0xA2
     MERCURY_ERROR_COUNTS = 0xA3
@@ -631,25 +639,25 @@
                 log_command.append(command)
             elif isinstance(i, str):
                 log_command.append(i)
             else:
                 log_command.append(hex(i))
         self.log.debug("_write: {}".format(log_command))
                 
-        py_version = check_python_version()
+        py_version = DataProcessor.check_python_version()
         if py_version == 2:
             self.sock.sendall("".join([chr(b) for b in command]))
         else:
             if isinstance(command, str):
                 command = command.encode()
             else:
                 command = bytes(command)
             self.sock.sendall(command)
     else:
-        self._serial_port.reset_input_buffer()
+        # self._serial_port.reset_input_buffer()
         command_log = ""
         for i in command:
             command_log += hex(i)[2:] + " "
         self.log.debug("_write: {}".format(command_log))
         self._serial_port.write(command)
         self._serial_port.flush()
 
@@ -690,15 +698,15 @@
                 data = self.sock.recv(1024)
                 if isinstance(data, str):
                     datas = bytearray()
                     for i in data:   
                         datas += hex(ord(i))
             except:
                 data = b""
-        if check_python_version() == 2:
+        if DataProcessor.check_python_version() == 2:
             command_log = ""
             for d in data:
                 command_log += hex(ord(d))[2:] + " "
             self.log.debug("_read : {}".format(command_log))
             # self.log.debug("_read: {}".format([hex(ord(d)) for d in data]))
         else:
             command_log = ""
@@ -715,15 +723,14 @@
         elif genre == ProtocolCode.GET_ACCEI_DATA:
             wait_time = 1
         while True and time.time() - t < wait_time:
             if genre != ProtocolCode.STOP and self.is_stop:
                 break
             # print(genre)
             data = self._serial_port.read()
-            print(genre, data)
             k += 1
             if _class in ["Mercury", "MercurySocket"]:
                 if data_len == 3:
                     datas += data
                     crc = self._serial_port.read(2)
                     if DataProcessor.crc_check(datas) == [v for v in crc]:
                         datas+=crc
@@ -751,15 +758,14 @@
                     if k - 1 == pre:
                         datas += data
                     else:
                         datas = b"\xfe"
                         pre = k
         else:
             datas = b''
-        print("datas", datas)
         if DataProcessor.check_python_version() == 2:
             command_log = ""
             for d in datas:
                 command_log += hex(ord(d))[2:] + " "
             self.log.debug("_read : {}".format(command_log))
         else:
             command_log = ""
```

### Comparing `pymycobot-3.5.0b1/pymycobot/elephantrobot.py` & `pymycobot-3.5.0b2/pymycobot/elephantrobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/error.py` & `pymycobot-3.5.0b2/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/generate.py` & `pymycobot-3.5.0b2/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/log.py` & `pymycobot-3.5.0b2/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mecharmsocket.py` & `pymycobot-3.5.0b2/pymycobot/mecharmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mercury_api.py` & `pymycobot-3.5.0b2/pymycobot/mercury_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,25 +5,296 @@
 import logging
 import time
 import struct
 
 from pymycobot.log import setup_logging
 from pymycobot.error import calibration_parameters
 from pymycobot.generate import CommandGenerator
-from pymycobot.generate import ProtocolCode
+from pymycobot.common import ProtocolCode, write, read
 
 
 class MercuryCommandGenerator(CommandGenerator):
+    _write = write
+    _read = read
     def __init__(self, debug=False):
         super(MercuryCommandGenerator, self).__init__(debug)
         self.calibration_parameters = calibration_parameters
         self.is_stop = False
         self.write_command = []
         self.read_command = []
         
+    def _mesg(self, genre, *args, **kwargs):
+        """
+
+        Args:
+            genre: command type (Command)
+            *args: other data.
+                   It is converted to octal by default.
+                   If the data needs to be encapsulated into hexadecimal,
+                   the array is used to include them. (Data cannot be nested)
+            **kwargs: support `has_reply`
+                has_reply: Whether there is a return value to accept.
+        """
+        real_command, has_reply = super(MercuryCommandGenerator, self)._mesg(genre, *args, **kwargs)
+        is_in_position = False
+        with self.lock:
+            self.write_command.append(genre)
+            self._write(self._flatten(real_command))
+        if genre in [ProtocolCode.SEND_ANGLE, ProtocolCode.SEND_ANGLES, ProtocolCode.SEND_COORD, ProtocolCode.SEND_COORDS, ProtocolCode.JOG_ANGLE, ProtocolCode.JOG_COORD, ProtocolCode.JOG_INCREMENT, ProtocolCode.JOG_INCREMENT_COORD, ProtocolCode.COBOTX_SET_SOLUTION_ANGLES]:
+            has_reply = True
+        if has_reply:
+            t = time.time()
+            wait_time = 0.1   
+            if genre == ProtocolCode.POWER_ON:
+                wait_time = 8
+            elif genre in [ProtocolCode.POWER_OFF, ProtocolCode.RELEASE_ALL_SERVOS, ProtocolCode.FOCUS_ALL_SERVOS,
+                        ProtocolCode.RELEASE_SERVO, ProtocolCode.FOCUS_SERVO, ProtocolCode.STOP]:
+                wait_time = 3
+            elif genre in [ProtocolCode.SEND_ANGLE, ProtocolCode.SEND_ANGLES, ProtocolCode.SEND_COORD, ProtocolCode.SEND_COORDS, ProtocolCode.JOG_ANGLE, ProtocolCode.JOG_COORD, ProtocolCode.JOG_INCREMENT, ProtocolCode.JOG_INCREMENT_COORD, ProtocolCode.COBOTX_SET_SOLUTION_ANGLES]:
+                wait_time = 300
+                is_in_position = True
+            need_break = False
+            while True and time.time() - t < wait_time:
+                for data in self.read_command:
+                    if is_in_position and data == b'\xfe\xfe\x04[\x01\r\x87':
+                        need_break = True
+                        with self.lock:
+                            self.read_command.remove(data)
+                            return 1
+                        break
+                    elif genre == data[3]:
+                        need_break = True
+                        with self.lock:
+                            self.read_command.remove(data)
+                        break
+                if need_break:
+                    break
+                time.sleep(0.01)
+            else:
+                res = []
+            if need_break:
+                res = []
+                data_len = data[2] - 3
+                unique_data = [ProtocolCode.GET_BASIC_INPUT, ProtocolCode.GET_DIGITAL_INPUT]
+                if genre in unique_data:
+                    data_pos = 5
+                    data_len -= 1
+                else:
+                    data_pos = 4
+                valid_data = data[data_pos : data_pos + data_len]
+                if data_len in [6, 8, 12, 14, 16, 24, 26, 60]:
+                    if data_len == 8 and (genre == ProtocolCode.IS_INIT_CALIBRATION):
+                        for v in valid_data:
+                            res.append(v)
+                    elif data_len == 8 and genre == ProtocolCode.GET_DOWN_ENCODERS:
+                        i = 0
+                        while i < data_len:
+                            byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
+                            i+=4
+                            res.append(byte_value)
+                    for header_i in range(0, len(valid_data), 2):
+                        one = valid_data[header_i : header_i + 2]
+                        res.append(self._decode_int16(one))
+                elif data_len == 2:
+                    if genre in [ProtocolCode.IS_SERVO_ENABLE]:
+                        return [self._decode_int8(valid_data[1:2])]
+                    elif genre in [ProtocolCode.GET_ERROR_INFO]:
+                        return [self._decode_int8(valid_data[1:])]
+                    res.append(self._decode_int16(valid_data))
+                elif data_len == 3:
+                    res.append(self._decode_int16(valid_data[1:]))
+                elif data_len == 4:
+                    if genre == ProtocolCode.COBOTX_GET_ANGLE:
+                        byte_value = int.from_bytes(valid_data, byteorder='big', signed=True)
+                        res.append(byte_value)
+                    for i in range(1,4):
+                        res.append(valid_data[i])
+                elif data_len == 7:
+                    error_list = [i for i in valid_data]
+                    for i in error_list:
+                        if i in range(16,23):
+                            res.append(1)
+                        elif i in range(23,29):
+                            res.append(2)
+                        elif i in range(32,112):
+                            res.append(3)
+                        else:
+                            res.append(i)
+                elif data_len == 28:
+                    for i in range(0, data_len, 4):
+                        byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
+                        res.append(byte_value) 
+                elif data_len == 40:
+                    i = 0
+                    while i < data_len:
+                        if i < 28:
+                            byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
+                            res.append(byte_value) 
+                            i+=4
+                        else:
+                            one = valid_data[i : i + 2]
+                            res.append(self._decode_int16(one))
+                            i+=2
+                elif data_len == 30:
+                    i = 0
+                    res = []
+                    while i < 30:
+                        if i < 9 or i >= 23:
+                            res.append(valid_data[i])
+                            i+=1
+                        elif i < 23:
+                            one = valid_data[i : i + 2]
+                            res.append(self._decode_int16(one))
+                            i+=2
+                elif data_len == 38:
+                    i = 0
+                    res = []
+                    while i < data_len:
+                        if i < 10 or i >= 30:
+                            res.append(valid_data[i])
+                            i+=1
+                        elif i < 38:
+                            one = valid_data[i : i + 2]
+                            res.append(self._decode_int16(one))
+                            i+=2
+                elif data_len == 56:
+                    for i in range(0, data_len, 8):
+                        
+                        byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
+                        res.append(byte_value)
+                else:
+                    if genre in [
+                        ProtocolCode.GET_SERVO_VOLTAGES,
+                        ProtocolCode.GET_SERVO_STATUS,
+                        ProtocolCode.GET_SERVO_TEMPS,
+                    ]:
+                        for i in range(data_len):
+                            data1 = self._decode_int8(valid_data[i : i + 1])
+                            res.append(0xFF & data1 if data1 < 0 else data1)
+                    res.append(self._decode_int8(valid_data))
+                if res == []:
+                    return None
+                
+                if genre in [
+                    ProtocolCode.ROBOT_VERSION,
+                    ProtocolCode.GET_ROBOT_ID,
+                    ProtocolCode.IS_POWER_ON,
+                    ProtocolCode.IS_CONTROLLER_CONNECTED,
+                    ProtocolCode.IS_PAUSED,  # TODO have bug: return b''
+                    ProtocolCode.IS_IN_POSITION,
+                    ProtocolCode.IS_MOVING,
+                    ProtocolCode.IS_SERVO_ENABLE,
+                    ProtocolCode.IS_ALL_SERVO_ENABLE,
+                    ProtocolCode.GET_SERVO_DATA,
+                    ProtocolCode.GET_DIGITAL_INPUT,
+                    ProtocolCode.GET_GRIPPER_VALUE,
+                    ProtocolCode.IS_GRIPPER_MOVING,
+                    ProtocolCode.GET_SPEED,
+                    ProtocolCode.GET_ENCODER,
+                    ProtocolCode.GET_BASIC_INPUT,
+                    ProtocolCode.GET_TOF_DISTANCE,
+                    ProtocolCode.GET_END_TYPE,
+                    ProtocolCode.GET_MOVEMENT_TYPE,
+                    ProtocolCode.GET_REFERENCE_FRAME,
+                    ProtocolCode.GET_FRESH_MODE,
+                    ProtocolCode.GET_GRIPPER_MODE,
+                    ProtocolCode.SET_SSID_PWD,
+                    ProtocolCode.COBOTX_IS_GO_ZERO,
+                    ProtocolCode.GET_ERROR_DETECT_MODE,
+                    ProtocolCode.POWER_ON,
+                    ProtocolCode.POWER_OFF,
+                    ProtocolCode.RELEASE_ALL_SERVOS,
+                    ProtocolCode.RELEASE_SERVO,
+                    ProtocolCode.FOCUS_ALL_SERVOS,
+                    ProtocolCode.FOCUS_SERVO,
+                    ProtocolCode.STOP,
+                    ProtocolCode.SET_BREAK,
+                    ProtocolCode.IS_BTN_CLICKED,
+                ]:
+                    return self._process_single(res)
+                elif genre in [ProtocolCode.GET_ANGLES]:
+                    return [self._int2angle(angle) for angle in res]
+                elif genre in [
+                    ProtocolCode.GET_COORDS,
+                    ProtocolCode.MERCURY_GET_BASE_COORDS,
+                    ProtocolCode.GET_TOOL_REFERENCE,
+                    ProtocolCode.GET_WORLD_REFERENCE,
+                ]:
+                    if res:
+                        r = []
+                        for idx in range(3):
+                            r.append(self._int2coord(res[idx]))
+                        for idx in range(3, 6):
+                            r.append(self._int2angle(res[idx]))
+                        return r
+                    else:
+                        return res
+                elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
+                    return [self._int2coord(angle) for angle in res]
+                elif genre in [ProtocolCode.GET_BASIC_VERSION, ProtocolCode.SOFTWARE_VERSION, ProtocolCode.GET_ATOM_VERSION]:
+                    return self._int2coord(self._process_single(res))
+                elif genre in [
+                    ProtocolCode.GET_JOINT_MAX_ANGLE,
+                    ProtocolCode.GET_JOINT_MIN_ANGLE,
+                ]:
+                    return self._int2coord(res[0])
+                elif genre == ProtocolCode.GET_ANGLES_COORDS:
+                    r = []
+                    for index in range(len(res)):
+                        if index < 7:
+                            r.append(self._int2angle(res[index]))
+                        elif index < 10:
+                            r.append(self._int2coord(res[index]))
+                        else:
+                            r.append(self._int2angle(res[index]))
+                    return r
+                elif genre == ProtocolCode.GO_ZERO:
+                    r = []
+                    if res:
+                        if 1 not in res[1:]:
+                            return res[0]
+                        else:
+                            for i in range(1, len(res)):
+                                if res[i] == 1:
+                                    r.append(i)
+                    return r
+                elif genre in [ProtocolCode.COBOTX_GET_ANGLE, ProtocolCode.COBOTX_GET_SOLUTION_ANGLES]:
+                        return self._int2angle(res[0])
+                elif genre == ProtocolCode.MERCURY_ROBOT_STATUS:
+                    if len(res) == 23:
+                        i = 9
+                        for i in range(9, len(res)):
+                            if res[i] != 0:
+                                data = bin(res[i])[2:]
+                                res[i] = []
+                                while len(data) != 16:
+                                    data = "0"+data
+                                for j in range(16):
+                                    if data[j] != "0":
+                                        res[i].append(15-j)
+                        return res
+                    else:
+                        for i in range(10, len(res)):
+                            if res[i] != 0:
+                                data = bin(res[i])[2:]
+                                res[i] = []
+                                while len(data) != 16:
+                                    data = "0"+data
+                                for j in range(16):
+                                    if data[j] != "0":
+                                        res[i].append(15-j)
+                        return res
+                else:
+                    return res
+            else:
+                with self.lock:
+                    self.write_command.remove(genre)
+                return None
+    
+        
     def _process_received(self, data):
         if not data:
             return []
         elif data == b'\xfe\xfe\x04[\x01\r\x87':
             # 水星到位反馈
             return data
         
@@ -37,141 +308,14 @@
                 if cmd_id in self.write_command:
                     break
             header_i += 1
             header_j += 1
         else:
             return []
         return data
-        if arm == 14:
-            data_len = data[header_i + 2] - 3
-            
-        unique_data = [ProtocolCode.GET_BASIC_INPUT, ProtocolCode.GET_DIGITAL_INPUT]
-        if cmd_id == ProtocolCode.GET_DIGITAL_INPUT and arm == 14:
-            data_pos = header_i + 4
-        elif cmd_id in unique_data:
-            if arm == 12:
-                data_pos = header_i + 6
-            else:
-                data_pos = header_i + 5
-            data_len -= 1
-        else:
-            if arm in [6, 7, 14, 8]:
-                data_pos = header_i + 4
-            elif arm == 12:
-                data_pos = header_i + 5
-        valid_data = data[data_pos : data_pos + data_len]
-
-        # process valid data
-        res = []   
-        if data_len in [6, 8, 12, 14, 16, 24, 26, 60]:
-            ignor_t = (
-                ProtocolCode.GET_SERVO_CURRENTS,
-                ProtocolCode.GET_SERVO_TEMPS,
-                ProtocolCode.GET_SERVO_VOLTAGES,
-                ProtocolCode.GET_SERVO_STATUS,
-                ProtocolCode.IS_ALL_SERVO_ENABLE
-            )
-            if data_len == 8 and (
-                    (arm == 14 and cmd_id == ProtocolCode.IS_INIT_CALIBRATION) or
-                    (arm == 8 and cmd_id in ignor_t)
-            ):
-                for v in valid_data:
-                    res.append(v)
-                return res
-            elif data_len == 8 and arm == 14 and cmd_id == ProtocolCode.GET_DOWN_ENCODERS:
-                i = 0
-                while i < data_len:
-                    byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
-                    i+=4
-                    res.append(byte_value)
-                return res
-            for header_i in range(0, len(valid_data), 2):
-                one = valid_data[header_i : header_i + 2]
-                res.append(self._decode_int16(one))
-        elif data_len == 2:
-            if genre in [ProtocolCode.IS_SERVO_ENABLE]:
-                return [self._decode_int8(valid_data[1:2])]
-            elif genre in [ProtocolCode.GET_ERROR_INFO]:
-                return [self._decode_int8(valid_data[1:])]
-            res.append(self._decode_int16(valid_data))
-        elif data_len == 3:
-            res.append(self._decode_int16(valid_data[1:]))
-        elif data_len == 4:
-            if genre == ProtocolCode.COBOTX_GET_ANGLE and arm == 14:
-                byte_value = int.from_bytes(valid_data, byteorder='big', signed=True)
-                res.append(byte_value)
-                return res
-            for i in range(1,4):
-                res.append(valid_data[i])
-        elif data_len == 7:
-            error_list = [i for i in valid_data]
-            for i in error_list:
-                if i in range(16,23):
-                    res.append(1)
-                elif i in range(23,29):
-                    res.append(2)
-                elif i in range(32,112):
-                    res.append(3)
-                else:
-                    res.append(i)
-        elif data_len == 28:
-            for i in range(0, data_len, 4):
-                byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
-                res.append(byte_value) 
-        elif data_len == 40:
-            i = 0
-            while i < data_len:
-                if i < 28:
-                    byte_value = int.from_bytes(valid_data[i:i+4], byteorder='big', signed=True)
-                    res.append(byte_value) 
-                    i+=4
-                else:
-                    one = valid_data[i : i + 2]
-                    res.append(self._decode_int16(one))
-                    i+=2
-        elif data_len == 30:
-            i = 0
-            res = []
-            while i < 30:
-                if i < 9 or i >= 23:
-                    res.append(valid_data[i])
-                    i+=1
-                elif i < 23:
-                    one = valid_data[i : i + 2]
-                    res.append(self._decode_int16(one))
-                    i+=2
-            return res
-        elif data_len == 38:
-            i = 0
-            res = []
-            while i < data_len:
-                if i < 10 or i >= 30:
-                    res.append(valid_data[i])
-                    i+=1
-                elif i < 38:
-                    one = valid_data[i : i + 2]
-                    res.append(self._decode_int16(one))
-                    i+=2
-            return res
-        else:
-            if genre in [
-                ProtocolCode.GET_SERVO_VOLTAGES,
-                ProtocolCode.GET_SERVO_STATUS,
-                ProtocolCode.GET_SERVO_TEMPS,
-            ]:
-                for i in range(data_len):
-                    data1 = self._decode_int8(valid_data[i : i + 1])
-                    res.append(0xFF & data1 if data1 < 0 else data1)
-                return res
-            res.append(self._decode_int8(valid_data))
-        if genre == ProtocolCode.GET_ACCEI_DATA:
-            for i in range(len(res)):
-                res[i] /= 1000
-        return res
-        
         
     def read_thread(self, method=None):
         while True:
             datas = b""
             data_len = -1
             k = 0
             pre = 0
@@ -194,50 +338,58 @@
                     self.log.debug("_read : {}".format(command_log))
                     # self.log.debug("_read: {}".format([hex(ord(d)) for d in data]))
                 else:
                     command_log = ""
                     for d in data:
                         command_log += hex(d)[2:] + " "
                     self.log.debug("_read : {}".format(command_log))
-                return data
+                if data:
+                    res = self._process_received(data)
+                    with self.lock:
+                        self.read_command.append(res)
             else:
                 while True and time.time() - t < wait_time:
-                    data = self._serial_port.read()
-                    k += 1
-                    if data_len == 3:
-                        datas += data
-                        crc = self._serial_port.read(2)
-                        if self.crc_check(datas) == [v for v in crc]:
-                            datas+=crc
-                            break
-                    if data_len == 1 and data == b"\xfa":
-                        datas += data
-                        # if [i for i in datas] == command:
-                        #     datas = b''
-                        #     data_len = -1
-                        #     k = 0
-                        #     pre = 0
-                        #     continue
-                        # break
-                    elif len(datas) == 2:
-                        data_len = struct.unpack("b", data)[0]
-                        datas += data
-                    elif len(datas) > 2 and data_len > 0:
-                        datas += data
-                        data_len -= 1
-                    elif data == b"\xfe":
-                        if datas == b"":
+                    # print("r", end=" ", flush=True)
+                    if self._serial_port.inWaiting() > 0:
+                        data = self._serial_port.read()
+                        k += 1
+                        # print(datas, flush=True)
+                        if data_len == 3:
                             datas += data
-                            pre = k
-                        else:
-                            if k - 1 == pre:
+                            crc = self._serial_port.read(2)
+                            if self.crc_check(datas) == [v for v in crc]:
+                                datas+=crc
+                                break
+                        if data_len == 1 and data == b"\xfa":
+                            datas += data
+                            # if [i for i in datas] == command:
+                            #     datas = b''
+                            #     data_len = -1
+                            #     k = 0
+                            #     pre = 0
+                            #     continue
+                            # break
+                        elif len(datas) == 2:
+                            data_len = struct.unpack("b", data)[0]
+                            datas += data
+                        elif len(datas) > 2 and data_len > 0:
+                            datas += data
+                            data_len -= 1
+                        elif data == b"\xfe":
+                            if datas == b"":
                                 datas += data
-                            else:
-                                datas = b"\xfe"
                                 pre = k
+                            else:
+                                if k - 1 == pre:
+                                    datas += data
+                                else:
+                                    datas = b"\xfe"
+                                    pre = k
+                    # else:
+                    #     print("no data", flush=True)
                 else:
                     datas = b''
                 if datas:
                     res = self._process_received(datas)
                     
                     if self.check_python_version() == 2:
                         command_log = ""
@@ -717,8 +869,69 @@
         return self._mesg(ProtocolCode.GET_POS_OVER, has_reply=True)
     
     def clear_encoders_error(self):
         return self._mesg(ProtocolCode.CLEAR_ENCODERS_ERROR)
     
     def get_down_encoders(self):
         return self._mesg(ProtocolCode.GET_DOWN_ENCODERS, has_reply=True)
+    
+    def set_control_mode(self, mode):
+        """Set robot motion mode
+
+        Args:
+            mode (int): 0 - location mode, 1 - torque mode
+
+        """
+        return self._mesg(ProtocolCode.SET_CONTROL_MODE, mode)
+    
+    def get_control_mode(self):
+        """Get robot motion mode
+
+        Returns:
+            int: 0 - location mode, 1 - torque mode
+        """
+        return self._mesg(ProtocolCode.GET_CONTROL_MODE, has_reply=True)
+    
+    def set_collision_mode(self, mode):
+        """Set collision detection mode
+
+        Args:
+            mode (int): 0 - disable, 1 - enable
+
+        """
+        return self._mesg(ProtocolCode.SET_COLLISION_MODE, mode)
+    
+    def set_collision_threshold(self, joint_id, value=100):
+        """Set joint collision threshold
+
+        Args:
+            joint_id (int): joint ID， range 1 ~ 7
+            value (int): Collision threshold, range is 50 ~ 250, default is 100, the smaller the value, the easier it is to trigger a collision
+        """
+        return self._mesg(ProtocolCode.SET_COLLISION_THRESHOLD, joint_id, value)
+    
+    def get_collision_threshold(self, joint_id):
+        """Get joint collision threshold
+
+        Args:
+            joint_id (int): joint ID， range 1 ~ 7
+        """
+        return self._mesg(ProtocolCode.GET_COLLISION_THRESHOLD, joint_id, has_reply=True)
+    
+    def set_torque_comp(self, joint_id, value=100):
+        """Set joint torque compensation
+
+        Args:
+            joint_id (int): joint ID， range 1 ~ 7
+            value (int): Compensation value, range is 0 ~ 250, default is 100, The smaller the value, the harder it is to drag the joint
+        """
+        return self._mesg(ProtocolCode.SET_TORQUE_COMP, joint_id, value)
+    
+    def get_torque_comp(self, joint_id):
+        """Get joint torque compensation
+
+        Args:
+            joint_id (int): joint ID， range 1 ~ 7
+        """
+        return self._mesg(ProtocolCode.GET_TORQUE_COMP, joint_id, has_reply=True)
+
```

### Comparing `pymycobot-3.5.0b1/pymycobot/mercurychassis.py` & `pymycobot-3.5.0b2/pymycobot/mercurychassis.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mercurysocket.py` & `pymycobot-3.5.0b2/pymycobot/mercurysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/myagv.py` & `pymycobot-3.5.0b2/pymycobot/myagv.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/myarm.py` & `pymycobot-3.5.0b2/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/myarm_api.py` & `pymycobot-3.5.0b2/pymycobot/myarm_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/myarmm.py` & `pymycobot-3.5.0b2/pymycobot/myarmm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/myarmsocket.py` & `pymycobot-3.5.0b2/pymycobot/myarmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mybuddy.py` & `pymycobot-3.5.0b2/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mybuddybluetooth.py` & `pymycobot-3.5.0b2/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mybuddyemoticon.py` & `pymycobot-3.5.0b2/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mybuddysocket.py` & `pymycobot-3.5.0b2/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mycobot.py` & `pymycobot-3.5.0b2/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mycobotpro630.py` & `pymycobot-3.5.0b2/pymycobot/mycobotpro630.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mycobotsocket.py` & `pymycobot-3.5.0b2/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mypalletizer.py` & `pymycobot-3.5.0b2/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/mypalletizersocket.py` & `pymycobot-3.5.0b2/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/public.py` & `pymycobot-3.5.0b2/pymycobot/public.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/robot_limit.json` & `pymycobot-3.5.0b2/pymycobot/robot_limit.json`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/ultraArm.py` & `pymycobot-3.5.0b2/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot/utils.py` & `pymycobot-3.5.0b2/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.5.0b2/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.5.0b1
+Version: 3.5.0b2
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.5.0b1/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.5.0b2/pymycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/setup.py` & `pymycobot-3.5.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/tests/test_api.py` & `pymycobot-3.5.0b2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/tests/test_generator.py` & `pymycobot-3.5.0b2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.5.0b1/tests/test_socket.py` & `pymycobot-3.5.0b2/tests/test_socket.py`

 * *Files identical despite different names*

