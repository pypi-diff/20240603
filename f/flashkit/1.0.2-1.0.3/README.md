# Comparing `tmp/flashkit-1.0.2.tar.gz` & `tmp/flashkit-1.0.3.tar.gz`

## Comparing `flashkit-1.0.2.tar` & `flashkit-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 flashkit-1.0.2/lint.sh
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 flashkit-1.0.2/requirements.txt
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/__init__.py
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/cart.py
--rw-r--r--   0        0        0     7587 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/device.py
--rwxr-xr-x   0        0        0     9521 2020-02-02 00:00:00.000000 flashkit-1.0.2/flashkit/flashkit.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 flashkit-1.0.2/.gitignore
--rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 flashkit-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 flashkit-1.0.2/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 flashkit-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 flashkit-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 flashkit-1.0.3/lint.sh
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 flashkit-1.0.3/requirements.txt
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 flashkit-1.0.3/flashkit/__init__.py
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 flashkit-1.0.3/flashkit/cart.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 flashkit-1.0.3/flashkit/device.py
+-rwxr-xr-x   0        0        0     9521 2020-02-02 00:00:00.000000 flashkit-1.0.3/flashkit/flashkit.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 flashkit-1.0.3/.gitignore
+-rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 flashkit-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 flashkit-1.0.3/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 flashkit-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 flashkit-1.0.3/PKG-INFO
```

### Comparing `flashkit-1.0.2/lint.sh` & `flashkit-1.0.3/lint.sh`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.2/flashkit/cart.py` & `flashkit-1.0.3/flashkit/cart.py`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.2/flashkit/device.py` & `flashkit-1.0.3/flashkit/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,14 +49,24 @@
 PAR_MODE8  =  16
 PAR_DEV_ID =  32
 PAR_SINGE  =  64
 PAR_INC    = 128
 
 IO_BLOCK_SIZE = 0x10000
 
+# NOTE: Krikzz Flash Cart MD uses a M29W320ET chip.
+# Weird sequences of writes are commands from table 4 at the end of section 4:
+# https://www.digikey.com/en/htmldatasheets/production/258014/0/0/1/m29w320db-m29w320dt
+# These families of chip appear to be compatible with the official Krikzz carts:
+#  - S29 series from Cypress / Infineon
+#  - IS29 series from ISSI
+# These are NOT compatible:
+#  - MX29 series from Macronix (missing bypass mode)
+#  - AS29 series from Alliance Memory (missing bypass mode)
+
 
 class FlashKitNotFoundException(Exception):
   def __init__(self, device_path: Optional[str] = None):
     if device_path:
       message = 'FlashKit MD not found at {}'.format(device_path)
     else:
       message = 'FlashKit MD not found on any serial port!'
@@ -106,34 +116,25 @@
   def disconnect(self) -> None:
     self.serial.close()
 
   def setDelay(self, delay: int) -> None:
     self.__write2(CMD_DELAY, delay & 0xff)
 
   def readUint16(self, addr: int) -> int:
-    addr >>= 1  # byte to word
-    self.__write2(CMD_ADDR, addr >> 16)
-    self.__write2(CMD_ADDR, addr >> 8)
-    self.__write2(CMD_ADDR, addr)
+    self.setAddr(addr)
     self.__write1(CMD_RD | PAR_SINGE)
     return self.__read2()
 
   def writeUint16(self, addr: int, value: int) -> None:
-    addr >>= 1  # byte to word
-    self.__write2(CMD_ADDR, addr >> 16)
-    self.__write2(CMD_ADDR, addr >> 8)
-    self.__write2(CMD_ADDR, addr)
+    self.setAddr(addr)
     self.__write1(CMD_WR | PAR_SINGE)
     self.__writeWord(value)
 
   def writeUint8(self, addr: int, value: int) -> None:
-    addr >>= 1  # byte to word
-    self.__write2(CMD_ADDR, addr >> 16)
-    self.__write2(CMD_ADDR, addr >> 8)
-    self.__write2(CMD_ADDR, addr)
+    self.setAddr(addr)
     self.__write1(CMD_WR | PAR_SINGE | PAR_MODE8)
     self.__write1(value)
 
   def read(self, length: int) -> bytes:
     data = b''
 
     while length > 0:
@@ -185,21 +186,18 @@
   def flashErase(self, addr: int) -> None:
     self.writeUint16(0x555 * 2, 0xaa)
     self.writeUint16(0x2aa * 2, 0x55)
     self.writeUint16(0x555 * 2, 0x80)
     self.writeUint16(0x555 * 2, 0xaa)
     self.writeUint16(0x2aa * 2, 0x55)
 
-    addr >>= 1  # byte to word
     for i in range(8):
-      self.__write2(CMD_ADDR, addr >> 16)
-      self.__write2(CMD_ADDR, addr >> 8)
-      self.__write2(CMD_ADDR, addr)
+      self.setAddr(addr)
       self.__write2(CMD_WR | PAR_SINGE | PAR_MODE8, 0x30)
-      addr += 4096
+      addr += 8192
 
     self.flashRY()
 
   def flashRY(self) -> None:
     # Boy, I would love to know what this does.
     self.__write2(CMD_RY, CMD_RD | PAR_SINGE)
     self.__read2()
```

### Comparing `flashkit-1.0.2/flashkit/flashkit.py` & `flashkit-1.0.3/flashkit/flashkit.py`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.2/LICENSE.md` & `flashkit-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.2/README.md` & `flashkit-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flashkit-1.0.2/pyproject.toml` & `flashkit-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flashkit"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Joey Parrish", email="joey.parrish@gmail.com" },
 ]
 description = "Drive the Krikzz FlashKit Programmer MD to flash Sega Genesis carts from the command-line."
 readme = "README.md"
 # This comes from the usage of require=True in argparse's add_subparsers()
 requires-python = ">=3.7"
```

### Comparing `flashkit-1.0.2/PKG-INFO` & `flashkit-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashkit
-Version: 1.0.2
+Version: 1.0.3
 Summary: Drive the Krikzz FlashKit Programmer MD to flash Sega Genesis carts from the command-line.
 Project-URL: Homepage, https://github.com/joeyparrish/flashkit-md-py
 Project-URL: Issues, https://github.com/joeyparrish/flashkit-md-py/issues
 Author-email: Joey Parrish <joey.parrish@gmail.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

