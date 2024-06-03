# Comparing `tmp/bus_user-0.3.5.tar.gz` & `tmp/bus_user-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.3.5.tar", last modified: Fri May 31 12:02:11 2024, max compression
+gzip compressed data, was "bus_user-0.3.7.tar", last modified: Mon Jun  3 11:23:34 2024, max compression
```

## Comparing `bus_user-0.3.5.tar` & `bus_user-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 12:02:11.550973 bus_user-0.3.5/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     4169 2024-05-31 12:02:11.550973 bus_user-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3204 2024-05-31 11:59:33.000000 bus_user-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 12:02:11.545672 bus_user-0.3.5/bus_user/
--rw-rw-rw-   0        0        0     2077 2024-05-31 07:59:53.000000 bus_user-0.3.5/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.5/bus_user/history.py
--rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.5/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.5/bus_user/line_parser.py
--rw-rw-rw-   0        0        0    41851 2024-05-31 10:37:16.000000 bus_user-0.3.5/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.5/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    18547 2024-05-31 07:59:53.000000 bus_user-0.3.5/bus_user/serial_server.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:02:11.550973 bus_user-0.3.5/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 12:02:11.000000 bus_user-0.3.5/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 12:02:11.551975 bus_user-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:23:34.149025 bus_user-0.3.7/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     4233 2024-06-03 11:23:34.149025 bus_user-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3268 2024-06-03 09:53:46.000000 bus_user-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:23:34.142597 bus_user-0.3.7/bus_user/
+-rw-rw-rw-   0        0        0     2074 2024-06-03 07:24:45.000000 bus_user-0.3.7/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.7/bus_user/history.py
+-rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.7/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.7/bus_user/line_parser.py
+-rw-rw-rw-   0        0        0    44785 2024-06-03 09:52:45.000000 bus_user-0.3.7/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      711 2024-06-03 08:38:51.000000 bus_user-0.3.7/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    18547 2024-05-31 07:59:53.000000 bus_user-0.3.7/bus_user/serial_server.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:23:34.148026 bus_user-0.3.7/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4233 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 11:23:34.000000 bus_user-0.3.7/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:23:34.150025 bus_user-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.7/setup.py
```

### Comparing `bus_user-0.3.5/LICENSE` & `bus_user-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.5/PKG-INFO` & `bus_user-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.5
+Version: 0.3.7
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.5)
+# bus_user (v0.3.7)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
@@ -45,25 +45,27 @@
     [<VALUE>] - if asked some value, returned without measurement unit
     [FAIL] - any common not specified error
     [FAIL 0123] - any specified error without description
     [FAIL 02 VALUE OUT OF RANGE] - any specified error with description (full variant)
 
 
 ## Features
-1. Serial:  
+1. [SerialClient]:  
+	- keep all found ports in base class!  
+2. Serial:  
 	- Client+Server  
 	- connect with Type__AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
 	- set/get params by SlashOrSpacePath addressing  
 	- handle BackSpace send manually from terminal  
-2. SerialServer values:  
+3. SerialServer values:  
 	- as Callable  
 	- Value_WithUnit  
 	- Value_FromVariants  
 	- list_results  
-3. SerialServer cmd:  
+4. SerialServer cmd:  
 	- NONE is equivalent for SUCCESS  
 	- no need params (like line_parsed as before)  
 	- help - for show all variants (Units/Variants/Callables)!  
 
 
 ********************************************************************************
 ## License
```

### Comparing `bus_user-0.3.5/README.md` & `bus_user-0.3.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bus_user (v0.3.5)
+# bus_user (v0.3.7)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
@@ -23,25 +23,27 @@
     [<VALUE>] - if asked some value, returned without measurement unit
     [FAIL] - any common not specified error
     [FAIL 0123] - any specified error without description
     [FAIL 02 VALUE OUT OF RANGE] - any specified error with description (full variant)
 
 
 ## Features
-1. Serial:  
+1. [SerialClient]:  
+	- keep all found ports in base class!  
+2. Serial:  
 	- Client+Server  
 	- connect with Type__AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
 	- set/get params by SlashOrSpacePath addressing  
 	- handle BackSpace send manually from terminal  
-2. SerialServer values:  
+3. SerialServer values:  
 	- as Callable  
 	- Value_WithUnit  
 	- Value_FromVariants  
 	- list_results  
-3. SerialServer cmd:  
+4. SerialServer cmd:  
 	- NONE is equivalent for SUCCESS  
 	- no need params (like line_parsed as before)  
 	- help - for show all variants (Units/Variants/Callables)!  
 
 
 ********************************************************************************
 ## License
```

### Comparing `bus_user-0.3.5/bus_user/__init__.py` & `bus_user-0.3.7/bus_user/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     TYPE__ADDRESS,
     TYPE__RW_ANSWER,
 
     Type__WrReturn,
     Type__AddressAutoAcceptVariant,
 
     # EXX
-    Exx_SerialAddress_NotConfigured,
+    Exx_SerialAddress_NotApplyed,
     Exx_SerialAddress_NotExists,
     Exx_SerialAddresses_NoVacant,
     Exx_SerialAddresses_NoAutodetected,
     Exx_SerialAddress_AlreadyOpened,
     Exx_SerialAddress_AlreadyOpened_InOtherObject,
     Exx_SerialAddress_OtherError,
     Exx_SerialRead_NotFullLine,
```

### Comparing `bus_user-0.3.5/bus_user/history.py` & `bus_user-0.3.7/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.5/bus_user/i2c_client.py` & `bus_user-0.3.7/bus_user/i2c_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.5/bus_user/line_parser.py` & `bus_user-0.3.7/bus_user/line_parser.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.5/bus_user/serial_client.py` & `bus_user-0.3.7/bus_user/serial_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from serial import Serial
 from serial.tools import list_ports
 
 from . import HistoryIO
 
 
 # =====================================================================================================================
-class Exx_SerialAddress_NotConfigured(Exception):
+class Exx_SerialAddress_NotApplyed(Exception):
     """
         raise SerialException("Port must be configured before it can be used.")
     serial.serialutil.SerialException: Port must be configured before it can be used.
     """
     pass
 
 
@@ -145,15 +145,15 @@
     pass
     pass
 
     # LOGGER --------------------------------------------------
     # LOG_ENABLE = True
 
     # SETTINGS ------------------------------------------------
-    ADDRESS: TYPE__ADDRESS = None
+    _ADDRESS: TYPE__ADDRESS = None
 
     TIMEOUT__READ: float = 0.3       # 0.2 is too short!!! dont touch! in case of reading char by char 0.5 is the best!!! 0.3 is not enough!!!
     # need NONE NOT 0!!! if wait always!!
     BAUDRATE: int = 9600        # 115200
 
     CMDS_DUMP: List[str] = []   # ["IDN", "ADR", "REV", "VIN", ]
     RAISE_CONNECT: bool = True
@@ -171,23 +171,23 @@
     EOL__UNI_SET: bytes = b"\r\n"
 
     _GETATTR_STARTSWITH__SEND: str = "send__"
 
     # test purpose EMULATOR -----------------
     _EMULATOR__CLS: Type['SerialServer_Base'] = None    # IF USED - START it on PAIRED - it is exactly Emulator/Server! no need to use just another serialClient! _EMULATOR__INST could be used for test reason and check values in realtime!!
     _EMULATOR__INST: 'SerialServer_Base' = None
-    _EMULATOR__START: bool = None    # DONT DELETE! it need when you reconnecting! cause of ADDRESS replaced after disconnecting by exact str after PAIRED*
+    _EMULATOR__START: bool = None    # DONT DELETE! it need when you reconnecting! cause of address replaced after disconnecting by exact str after PAIRED*
 
     # AUX -----------------------------------------------------
     history: HistoryIO = None
     _SERIAL: Serial
 
-    ADDRESSES__SYSTEM: List[str] = []
-    ADDRESSES__SHORTED: List[str] = []
-    ADDRESSES__PAIRED: List[Tuple[str, str]] = []
+    ADDRESSES__SYSTEM: dict[str, Union[None, Self]] = {}
+    ADDRESSES__SHORTED: list[str] = []
+    ADDRESSES__PAIRED: list[tuple[str, str]] = []
 
     def __init__(self, address: TYPE__ADDRESS = None):
         super().__init__()
         self._SERIAL = Serial()
         self.history = HistoryIO()
 
         # set only address!!!
@@ -201,53 +201,73 @@
         # self._SERIAL.write_timeout = self._TIMEOUT__WRITE
 
         # self.addresses_system__detect()   # DONT USE in init!!!
         # self.addresses_shorted__detect()   # DONT USE in init!!!
         # self.addresses_paired__detect()   # DONT USE in init!!!
 
     def __del__(self):
+        self._address__release()
         self.disconnect()
 
+    @property
+    def ADDRESS(self) -> TYPE__ADDRESS:
+        return self._ADDRESS
+
+    @ADDRESS.setter
+    def ADDRESS(self, value: TYPE__ADDRESS) -> None:
+        self._address__release()
+        self._ADDRESS = value
+
+    @classmethod
+    @property
+    def ADDRESSES__SYSTEM_FREE(cls) -> list[str]:
+        cls.addresses_system__detect()
+        result = []
+        for port_name, port_owner in cls.ADDRESSES__SYSTEM.items():
+            if port_owner is None:
+                result.append(port_name)
+        return result
+
     def check__connected(self) -> bool:
         try:
             return self._SERIAL.is_open
         except:
             return False
 
     # =================================================================================================================
     def cmd_prefix__set(self) -> None:
         """
         OVERWRITE IF NEED/USED!
         """
         # self.PREFIX = ""
         return
 
-    def _clear_buffer__read(self) -> None:
+    def _buffers_clear__read(self) -> None:
         try:
             self.read_lines(_timeout=0.3)
         except:
             pass
 
-    def _clear_buffer__write(self) -> None:
+    def _buffers_clear__write(self) -> None:
         """useful to drop old previous incorrect send msg! in other words it is clear/reinit write buffer!
 
         here we need just finish line by correct/exact EOL if it was previously send without it or with incorrect.
         """
         try:
             self.write_eol()
         except:
             pass
 
-    def clear_buffers(self) -> None:
+    def buffers_clear(self) -> None:
         """useful to drop old previous incorrect send msg! in other words it is clear/reinit write buffer!
 
         here we need just finish line by correct/exact EOL if it was previously send without it or with incorrect.
         """
-        self._clear_buffer__write()
-        self._clear_buffer__read()
+        self._buffers_clear__write()
+        self._buffers_clear__read()
 
     # CONNECT =========================================================================================================
     def disconnect(self) -> None:
         try:
             self._SERIAL.close()
         except:
             pass
@@ -281,16 +301,16 @@
             address = self.address_get__first_free__shorted()
         elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__ANSWER_VALID:
             address = self.address_get__first_free__answer_valid()
         elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__PAIRED:
             address = self.address_get__first_free__paired()
 
         if address is None or isinstance(address, Type__AddressAutoAcceptVariant):
-            msg = "Exx_SerialAddress_NotConfigured"
-            exx = Exx_SerialAddress_NotConfigured()
+            msg = "Exx_SerialAddress_NotApplyed"
+            exx = Exx_SerialAddress_NotApplyed()
             need_open = False
 
         # need_open ==========================================================
         # CHANGE PORT OR USE SAME ---------------------------------
         if need_open:
             if self._SERIAL.port != address:
                 # close old
@@ -321,15 +341,15 @@
                     msg = f"[ERROR] PORT NOT EXISTS IN SYSTEM {self._SERIAL}"
                     exx = Exx_SerialAddress_NotExists(repr(_exx))
 
                     # self.detect_available_ports()
 
                 elif "Port must be configured before" in str(_exx):
                     msg = f"[ERROR] PORT NOT CONFIGURED {self._SERIAL}"
-                    exx = Exx_SerialAddress_NotConfigured(repr(_exx))
+                    exx = Exx_SerialAddress_NotApplyed(repr(_exx))
 
                 elif "PermissionError" in str(_exx):
                     msg = f"[ERROR] PORT ALREADY OPENED {self._SERIAL}"
                     exx = Exx_SerialAddress_AlreadyOpened(repr(_exx))
 
                 else:
                     msg = f"[ERROR] PORT OTHER ERROR {self._SERIAL}"
@@ -348,16 +368,15 @@
 
         # OK -----------------------------
         if not _touch_connection:
             if not self.connect__validation():
                 self.disconnect()
                 return False
 
-            self.LOGGER.info(f"[{self._SERIAL.port}][OK] connected {self._SERIAL}")
-            self.ADDRESS = self._SERIAL.port
+            self._address__occupy()
             self.emulator_start()
 
         self.cmd_prefix__set()
         return True
 
     def connect__validation(self) -> bool:
         """
@@ -374,76 +393,126 @@
 
         if self._EMULATOR__CLS:
             self._EMULATOR__INST = self._EMULATOR__CLS(self.address_paired__get())
 
         if self._EMULATOR__INST.connect():
             self._EMULATOR__INST.start()
             self._EMULATOR__INST.wait__cycle_active()
-            self._clear_buffer__read()
+            self._buffers_clear__read()
 
-    # ADDRESS =========================================================================================================
+    # address =========================================================================================================
     """
     THIS IS USED for applying by SIMPLE WAY just exact address! 
     """
     pass
     pass
     pass
     pass
     pass
     pass
     pass
 
-    # dont move to CLASSMETHOD!!!
+    # OCCUPATION ------------------------------------------------------------------------------------------------------
+    def _address__occupy(self) -> None:
+        if not self._SERIAL.port:
+            return
+
+        # clear old lock -------------
+        # for address, owner in SerialClient.ADDRESSES__SYSTEM.items():
+        #     if owner is self and address != self._SERIAL.port:
+        #         SerialClient.ADDRESSES__SYSTEM[address] = None
+
+        self._address__release()
+
+        # set new lock -------------
+        SerialClient.ADDRESSES__SYSTEM[self._SERIAL.port] = self
+        self.ADDRESS = self._SERIAL.port
+        self.LOGGER.info(f"[{self._SERIAL.port}][OK] connected/locked/occupy {self._SERIAL}")
+
+    def _address__release(self) -> None:
+        if self in SerialClient.ADDRESSES__SYSTEM.values():
+            for address, owner in SerialClient.ADDRESSES__SYSTEM.items():
+                if owner is self:
+                    SerialClient.ADDRESSES__SYSTEM[address] = None
+                    break
+
+    @classmethod
+    def _addresses__release(cls) -> None:
+        """
+        make all ports vacant for autodetect
+        """
+        SerialClient.ADDRESSES__SYSTEM = dict.fromkeys(SerialClient.ADDRESSES__SYSTEM, None)
+
+    def address_check__resolved(self) -> bool:
+        return isinstance(self.ADDRESS, str)
+
+    def address_check__occupied(self, address: str) -> bool:
+        owner = self.ADDRESSES__SYSTEM[address]
+        return owner is not None\
+
+    # AUTODETECT ------------------------------------------------------------------------------------------------------
+    pass    # dont move this all to CLASSMETHOD!!!
+
     def address_get__first_free(self) -> str | None:
         result = None
-        for address in self.addresses_system__detect():
+        for address, owner in self.addresses_system__detect().items():
+            if owner is not None and owner is not self:
+                continue
+
             if self.connect(address=address, _raise=False, _touch_connection=True):
                 result = address
 
             self.disconnect()
             if result:
                 break
 
         msg = f"[{result=}]_address_apply__first_free"
         if result:
             self.LOGGER.info(msg)
         else:
-            self.LOGGER.warn(msg)
+            self.LOGGER.warning(msg)
 
         return result
 
     def address_get__first_free__shorted(self) -> str | None:
         """
         dont overwrite! dont mess with address__autodetect_logic!
         used to find exact device in all comport by some special logic like IDN/NAME value
         """
         result = None
         for address in self.addresses_shorted__detect():
+            owner = self.ADDRESSES__SYSTEM[address]
+            if owner is not None and owner is not self:
+                continue
+
             if self.connect(address=address, _raise=False, _touch_connection=True):
                 result = address
 
             self.disconnect()
             if result:
                 break
 
         msg = f"[{result=}]_address_apply__first_free__shorted"
         if result:
             self.LOGGER.info(msg)
         else:
-            self.LOGGER.warn(msg)
+            self.LOGGER.warning(msg)
 
         return result
 
     def address_get__first_free__answer_valid(self) -> str | None:
         """
         dont overwrite! dont mess with address__autodetect_logic!
         used to find exact device in all comport by some special logic like IDN/NAME value
         """
         result = None
-        for address in self.addresses_system__detect():
+        for address, owner in self.addresses_system__detect().items():
+            if owner is not None and owner is not self:
+                continue
+
             if self.connect(address=address, _raise=False, _touch_connection=True):
                 try:
                     if self.address__answer_validation():
                         result = address
                 except Exception as exx:
                     print(f"finding address {exx!r}")
                     pass
@@ -452,15 +521,15 @@
                 if result:
                     break
 
         msg = f"[{result=}]_address_apply__first_free__answer_valid"
         if result:
             self.LOGGER.info(msg)
         else:
-            self.LOGGER.warn(msg)
+            self.LOGGER.warning(msg)
 
         return result
 
     def address_get__first_free__paired(self) -> str | None:
         """
         connect only for first address!
         need for occupy addresses by several servers before starting main process!!!
@@ -488,59 +557,50 @@
                 break
 
         # FINISH -------------
         msg = f"[{result=}]address_get__first_free__paired"
         if result:
             self.LOGGER.info(msg)
         else:
-            self.LOGGER.warn(msg)
+            self.LOGGER.warning(msg)
 
         return result
 
-    # -----------------------------------------------------------------------------------------------------------------
+    # VALIDATION ------------------------------------------------------------------------------------------------------
     def address__answer_validation(self) -> bool | None | NoReturn:
         """
         overwrite for you case!
         used to find exact device in all comport by some special logic like IDN/NAME value.
 
         IDEA:
         1. this func will exec on every accessible address
         2. if this func return True - address would be accepted!
         3. raiseExx/NoReturn - equivalent as False!
         """
 
-    def address__answer_validation__shorted(self) -> bool | None:
+    def _address__answer_validation__shorted(self) -> bool | None:
+        """
+        this is the internal method! for autodetect shorted address
+        """
         load = "FIND__SHORTED"
         return self.write_read__last_validate(load, load)
 
-    # DETECT PORTS ====================================================================================================
-    pass
-    pass
-    pass
-    pass
-    pass
-    pass
-    pass
-
-    def address_check__resolved(self) -> bool:
-        return isinstance(self.ADDRESS, str)
-
-    # -----------------------------------------------------------------------------------------------------------------
+    # DETECT ----------------------------------------------------------------------------------------------------------
     def address__check_exists(self) -> bool:
         try:
             self.connect(_raise=True, _touch_connection=True)
             self.disconnect()
         except Exx_SerialAddress_NotExists:
             return False
         except:
             return False
         return True
 
     @classmethod
-    def addresses_system__detect(cls) -> List[str]:
+    def addresses_system__detect(cls) -> dict[str, Union[None, Self]]:
         if SerialClient.ADDRESSES__SYSTEM:
             return SerialClient.ADDRESSES__SYSTEM
 
         # WORK -------------------------------------------------------
         result = cls._addresses_system__detect_1__standard_method()
         for port in cls._addresses_system__detect_2__direct_access():
             if port not in result:
@@ -548,16 +608,16 @@
 
         # result -------------------------------------------------------
         if result:
             print(f"[OK] detected serial ports {result}")
         else:
             print("[WARN] detected no serial ports")
 
-        SerialClient.ADDRESSES__SYSTEM = result
-        return result
+        SerialClient.ADDRESSES__SYSTEM = dict.fromkeys(result, None)
+        return SerialClient.ADDRESSES__SYSTEM
 
     @staticmethod
     def _addresses_system__detect_1__standard_method() -> Union[List[str], NoReturn]:
         """
         WINDOWS - USB
             ==========OBJECTINFO.PRINT==========================================================================
             str=COM8 - PL2303HXA PHASED OUT SINCE 2012. PLEASE CONTACT YOUR SUPPLIER.
@@ -628,17 +688,14 @@
         return result
 
     @staticmethod
     def _addresses_system__detect_2__direct_access() -> Union[List[str], NoReturn]:
         """Определяет список портов (НЕОТКРЫТЫХ+ОТКРЫТЫХ!!!) - способом 2 (слепым тестом подключения и анализом исключений)
         Всегда срабатывает!
         """
-        _lock_port = None
-        # _lock_port = Serial(port="COM7", timeout=5)   # test reason! finding exx already opened!
-
         if sys.platform.startswith('win'):
             attempt_list = ['COM%s' % (i + 1) for i in range(256)]
         elif sys.platform.startswith('linux') or sys.platform.startswith('cygwin'):
             # this excludes your current terminal "/dev/tty"
             attempt_list = glob.glob('/dev/tty[A-Za-z]*')
         elif sys.platform.startswith('darwin'):
             attempt_list = glob.glob('/dev/tty.*')
@@ -646,86 +703,84 @@
             raise EnvironmentError('[ERROR]Unsupported platform')
 
         result: List[str] = []
         for name in attempt_list:
             if SerialClient(address=name).address__check_exists():
                 result.append(name)
 
-        if _lock_port:
-            _lock_port.close()
         return result
 
     @classmethod
     def addresses_shorted__detect(cls) -> List[str]:
         if SerialClient.ADDRESSES__SHORTED:
             return SerialClient.ADDRESSES__SHORTED
 
         # WORK ----------------------------------------------
         result = []
         for address in cls.addresses_system__detect():
             obj = cls()
             if obj.connect(address=address, _raise=False, _touch_connection=True):
-                if obj.address__answer_validation__shorted():
+                if obj._address__answer_validation__shorted():
                     result.append(address)
                 obj.disconnect()
 
         SerialClient.ADDRESSES__SHORTED = result
-        print(f"{cls.ADDRESSES__SHORTED=}")
+        print(f"{SerialClient.ADDRESSES__SHORTED=}")
         return result
 
     @classmethod
     def addresses_paired__detect(cls) -> list[tuple[str, str]]:
-        # print(f"111111{cls.ADDRESSES__PAIRED=}")
-
         if SerialClient.ADDRESSES__PAIRED:
             return SerialClient.ADDRESSES__PAIRED
 
         # WORK ----------------------------------------------
         load = "EXPECT_ANSWER__PAIRED"
         result = []
-        instances_free = []
+        instances_free_remain = []
+
+        system_ports = cls.addresses_system__detect()
 
-        addresses__system = cls.addresses_system__detect()
-        for address in addresses__system:
-            instance = cls(address)
-            if instance.connect(_raise=False, _touch_connection=True):
-                instances_free.append(instance)
+        for address in system_ports:
+            instance = cls()
+            if instance.connect(address=address, _raise=False, _touch_connection=True):
+                instances_free_remain.append(instance)
 
-        while len(instances_free) > 1:
-            main = instances_free.pop(0)
+        while len(instances_free_remain) > 1:
+            main = instances_free_remain.pop(0)
             main._write(load)
             main.disconnect()
 
-            for index, slave in enumerate(instances_free):
-                if slave.read_line(_timeout=0.3) == load:
-                    result.append((main.ADDRESS, slave.ADDRESS))
+            for index, slave in enumerate(instances_free_remain):
+                read_lines = slave.read_lines(_timeout=0.3)
+                if read_lines and read_lines[-1] == load:
+                    result.append((main._SERIAL.port, slave._SERIAL.port))
                     slave.disconnect()
-                    instances_free.pop(index)
+                    instances_free_remain.pop(index)
                     break
 
-        for remain in instances_free:
+        for remain in instances_free_remain:
             remain.disconnect()
 
-        cls.ADDRESSES__PAIRED = result
-        print(f"{cls.ADDRESSES__PAIRED=}")
+        SerialClient.ADDRESSES__PAIRED = result
+        print(f"{SerialClient.ADDRESSES__PAIRED=}")
         return result
 
     def addresses_paired__get_used(self) -> Optional[Tuple[str, str]]:
         for pair in self.addresses_paired__detect():
             if self._SERIAL.port in pair:
                 return pair
 
     def address_paired__get(self) -> str | None:
-        if not self.ADDRESSES__PAIRED:
-            self.addresses_paired__detect()
+        if not SerialClient.ADDRESSES__PAIRED:
+            SerialClient.addresses_paired__detect()
 
-        if not isinstance(self.ADDRESS, str):
+        if not self.address_check__resolved():
             return
 
-        for pair in self.ADDRESSES__PAIRED:
+        for pair in SerialClient.ADDRESSES__PAIRED:
             if self.ADDRESS in pair:
                 addr1, addr2 = pair
                 if self.ADDRESS == addr1:
                     return addr2
                 else:
                     return addr1
 
@@ -1020,32 +1075,33 @@
         return always last_output
         """
         return self.write_read(data=data, prefix=prefix, args=args, kwargs=kwargs).last_output
 
     def write_read__last_validate(
             self,
             input: Union[AnyStr, list[AnyStr]] | None,
-            expect: Union[str, list[str]],
+            expect: str,
             prefix: Optional[str] = None,
             args: Optional[List] = None,
             kwargs: Optional[Dict] = None,
     ) -> bool:
         """
         created specially for address__answer_validation
         """
-        self.clear_buffers()
-        time.sleep(1)
         if input:
+            self.buffers_clear()
             output_last = self.write_read__last(data=input, prefix=prefix, args=args, kwargs=kwargs)
         else:
             outputs = self.read_lines()
-            output_last = None
             if outputs:
                 output_last = outputs[-1]
-        return output_last == expect
+            else:
+                output_last = ""
+
+        return output_last.lower() == expect.lower()
 
     def dump_cmds(self, cmds: List[str] = None) -> Union[HistoryIO, NoReturn]:
         """
         useful to get results for standard cmds list
         if you need to read all params from device!
         """
         cmds = cmds or self.CMDS_DUMP
@@ -1082,12 +1138,29 @@
         """
         if self._GETATTR_STARTSWITH__SEND and item.startswith(self._GETATTR_STARTSWITH__SEND):
             item = item.replace(self._GETATTR_STARTSWITH__SEND, "")
         return lambda *args, **kwargs: self.write_read__last(data=self._create_cmd_line(cmd=item, args=args, kwargs=kwargs))
 
 
 # =====================================================================================================================
+class SerialClient_FirstFree(SerialClient):
+    _ADDRESS = Type__AddressAutoAcceptVariant.FIRST_FREE
+
+
+class SerialClient_FirstFree_Shorted(SerialClient):
+    _ADDRESS = Type__AddressAutoAcceptVariant.FIRST_FREE__SHORTED
+
+
+class SerialClient_FirstFree_Paired(SerialClient):
+    _ADDRESS = Type__AddressAutoAcceptVariant.FIRST_FREE__PAIRED
+
+
+class SerialClient_FirstFree_AnswerValid(SerialClient):
+    _ADDRESS = Type__AddressAutoAcceptVariant.FIRST_FREE__ANSWER_VALID
+
+
+# =====================================================================================================================
 if __name__ == "__main__":
     pass
 
 
 # =====================================================================================================================
```

### Comparing `bus_user-0.3.5/bus_user/serial_server.py` & `bus_user-0.3.7/bus_user/serial_server.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.5/bus_user.egg-info/PKG-INFO` & `bus_user-0.3.7/bus_user.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.5
+Version: 0.3.7
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.5)
+# bus_user (v0.3.7)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
@@ -45,25 +45,27 @@
     [<VALUE>] - if asked some value, returned without measurement unit
     [FAIL] - any common not specified error
     [FAIL 0123] - any specified error without description
     [FAIL 02 VALUE OUT OF RANGE] - any specified error with description (full variant)
 
 
 ## Features
-1. Serial:  
+1. [SerialClient]:  
+	- keep all found ports in base class!  
+2. Serial:  
 	- Client+Server  
 	- connect with Type__AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
 	- set/get params by SlashOrSpacePath addressing  
 	- handle BackSpace send manually from terminal  
-2. SerialServer values:  
+3. SerialServer values:  
 	- as Callable  
 	- Value_WithUnit  
 	- Value_FromVariants  
 	- list_results  
-3. SerialServer cmd:  
+4. SerialServer cmd:  
 	- NONE is equivalent for SUCCESS  
 	- no need params (like line_parsed as before)  
 	- help - for show all variants (Units/Variants/Callables)!  
 
 
 ********************************************************************************
 ## License
```

### Comparing `bus_user-0.3.5/setup.py` & `bus_user-0.3.7/setup.py`

 * *Files identical despite different names*

