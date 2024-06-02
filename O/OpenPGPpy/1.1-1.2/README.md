# Comparing `tmp/OpenPGPpy-1.1-py3-none-any.whl.zip` & `tmp/OpenPGPpy-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 24748 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      306 b- defN 20-Dec-16 13:16 OpenPGPpy/__init__.py
--rw-rw-rw-  2.0 fat     3261 b- defN 22-Feb-02 11:37 OpenPGPpy/der_coding.py
--rw-rw-rw-  2.0 fat    22169 b- defN 22-Feb-07 18:20 OpenPGPpy/openpgp_card.py
--rw-rw-rw-  2.0 fat    31852 b- defN 23-Feb-27 09:29 OpenPGPpy-1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12853 b- defN 23-Feb-27 09:29 OpenPGPpy-1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-27 09:29 OpenPGPpy-1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Feb-27 09:29 OpenPGPpy-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      628 b- defN 23-Feb-27 09:29 OpenPGPpy-1.1.dist-info/RECORD
-8 files, 71171 bytes uncompressed, 23662 bytes compressed:  66.8%
+Zip file size: 24908 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      306 b- defN 24-May-30 21:59 OpenPGPpy/__init__.py
+-rw-rw-rw-  2.0 fat     3128 b- defN 24-May-31 13:36 OpenPGPpy/der_coding.py
+-rw-rw-rw-  2.0 fat    23485 b- defN 24-May-31 22:50 OpenPGPpy/openpgp_card.py
+-rw-rw-rw-  2.0 fat    31852 b- defN 24-Jun-02 21:59 OpenPGPpy-1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13063 b- defN 24-Jun-02 21:59 OpenPGPpy-1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-02 21:59 OpenPGPpy-1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Jun-02 21:59 OpenPGPpy-1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      628 b- defN 24-Jun-02 21:59 OpenPGPpy-1.2.dist-info/RECORD
+8 files, 72564 bytes uncompressed, 23822 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: OpenPGPpy/der_coding.py
 Comment: 
 
 Filename: OpenPGPpy/openpgp_card.py
 Comment: 
 
-Filename: OpenPGPpy-1.1.dist-info/LICENSE
+Filename: OpenPGPpy-1.2.dist-info/LICENSE
 Comment: 
 
-Filename: OpenPGPpy-1.1.dist-info/METADATA
+Filename: OpenPGPpy-1.2.dist-info/METADATA
 Comment: 
 
-Filename: OpenPGPpy-1.1.dist-info/WHEEL
+Filename: OpenPGPpy-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: OpenPGPpy-1.1.dist-info/top_level.txt
+Filename: OpenPGPpy-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenPGPpy-1.1.dist-info/RECORD
+Filename: OpenPGPpy-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## OpenPGPpy/der_coding.py

```diff
@@ -13,14 +13,15 @@
 # GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 
 
 def encode_int(intarray):
     """Encode a bytes array to a DER integer (bytes list)."""
+    # Add the integer TL header
     if intarray[0] >= 128:
         return [2, len(intarray) + 1, 0, *intarray]
     if intarray[0] == 0:
         return encode_int(intarray[1:])
     return [2, len(intarray), *intarray]
 
 
@@ -30,21 +31,15 @@
     int_r = encode_int(sigdata[:ec_size_bytes])
     int_s = encode_int(sigdata[ec_size_bytes:])
     return bytes([0x30, len(int_r) + len(int_s), *int_r, *int_s])
 
 
 def intlist_to_hex(bytes_list):
     """Returns an hex string representing bytes."""
-    if bytes == [] or bytes == b"":
-        return ""
-    else:
-        pformat = "%-0.2X"
-        return (
-            "".join(map(lambda a: pformat % ((a + 256) % 256), bytes_list))
-        ).rstrip()
+    return bytes(bytes_list).hex().upper()
 
 
 def decode_dos(data, start_index):
     """Basic ASN1 BER/DER decoder for a single DO."""
     i = start_index
     if data[i] & 31 == 31:
         # Tag has 2 bytes
```

## OpenPGPpy/openpgp_card.py

```diff
@@ -1,12 +1,12 @@
 #
 # -*- coding: utf-8 -*-
 
 # OpenPGPpy OpenPGPcard : OpenPGP smartcard communication library for Python
-# Copyright (C) 2020-2022  BitLogiK
+# Copyright (C) 2020-2024  BitLogiK
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, version 3 of the License.
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
@@ -19,14 +19,15 @@
 import time
 from .der_coding import encode_der, decode_do
 
 
 try:
     from smartcard.System import readers
     from smartcard.util import toBytes, toHexString
+    from smartcard.scard import SCARD_SHARE_EXCLUSIVE
     from smartcard.Exceptions import CardConnectionException
 except ModuleNotFoundError as exc:
     raise ModuleNotFoundError("pyscard not installed ?") from exc
 
 
 logger = getLogger(__name__)
 
@@ -101,29 +102,24 @@
         if len(args_list[1]) != 4 or not ishex(args_list[1]):
             raise BadInputException("filehex provided must be 2 or 4 hex chars")
         return func(*args_list)
 
     return func_wrapper
 
 
-def to_list(binstr):
-    return toBytes(binstr.hex())
-
-
 def print_list(liststr):
     """Output a list pretty in the debug logger."""
     for item in liststr:
         logger.debug(" - %s", item)
 
 
 # Core class OpenPGPcard
 
 
 class OpenPGPcard:
-
     AppID = toBytes("D27600012401")
     default_manufacturer_name = "- unknown -"
     manufacturer_list = {
         0x0001: "PPC Card Systems",
         0x0002: "Prism",
         0x0003: "OpenFortress",
         0x0004: "Wewid",
@@ -150,15 +146,15 @@
     }
 
     def __init__(self, reader_index=None):
         applet_detected = False
         readers_list = readers()
         if len(readers_list) > 0:
             if reader_index is None:
-                logger.debug("Trying to reach the OpenPGP app in all readers")
+                logger.debug("Trying to reach an OpenPGP app in all readers")
             logger.debug("Available readers :")
             print_list(readers_list)
             if reader_index is not None:
                 if not isinstance(reader_index, int):
                     raise ValueError("reader_index must be int.")
                 if reader_index < 0:
                     raise ValueError("reader_index is a positive index, starts at 0.")
@@ -168,15 +164,15 @@
                     raise ConnectionException("Reader index out of readers detected")
                 logger.debug("Using reader index #%i", reader_index)
             for reader in readers_list:
                 applet_detected = False
                 try:
                     logger.debug("Trying with reader : %s", reader)
                     self.connection = reader.createConnection()
-                    self.connection.connect()
+                    self.connection.connect(mode=SCARD_SHARE_EXCLUSIVE)
                     apdu_select = [0x00, 0xA4, 0x04, 0x00]
                     self.send_apdu(apdu_select, OpenPGPcard.AppID)
                     applet_detected = hasattr(self, "connection")
                 except Exception:
                     logger.debug("Fail with this reader")
                     if reader_index is not None:
                         raise ConnectionException("No OpenPGP applet on this reader.")
@@ -250,44 +246,77 @@
                 apdu += [exp_resp_len >> 8, exp_resp_len & 255]
             elif exp_resp_len == APDU_LONG:
                 # Le long : max response len 65535 bytes
                 apdu += [0, 0]
             else:
                 raise DataException("Expected data response too large")
         logger.debug(
-            f" Sending 0x{apdu_header[1]:X} command with {len_data} bytes data"
+            " Sending 0x%02X command with %i bytes data", apdu_header[1], len_data
         )
         if exp_resp_len > 0:
-            logger.debug(f"  with Le={exp_resp_len}")
-        logger.debug(f"-> {toHexString(apdu)}")
+            logger.debug("  with Le=%i", exp_resp_len)
+        logger.debug("-> %s", toHexString(apdu))
         t_env = time.time()
         try:
             data, sw_byte1, sw_byte2 = self.connection.transmit(apdu)
         except CardConnectionException:
             raise ConnectionException(
-                "Error when communicating with the OpenGPG device."
+                "Error while communicating with the OpenGPG device."
             )
         t_ans = (time.time() - t_env) * 1000
         logger.debug(
-            " Received %i bytes data : SW 0x%02X%02X - duration: %.1f ms"
-            % (len(data), sw_byte1, sw_byte2, t_ans)
+            " Received %i bytes data : SW 0x%02X%02X - duration: %.1f ms",
+            len(data),
+            sw_byte1,
+            sw_byte2,
+            t_ans,
         )
         if len(data) > 0:
-            logger.debug(f"<- {toHexString(data)}")
-        while sw_byte1 == 0x61:
+            logger.debug("<- %s", toHexString(data))
+        if sw_byte1 == 0x6C:
+            # T=0 : re-read card with correct Le
+            if len(apdu) == 4:
+                apdu += [0]
+            apdu[-1] = sw_byte2
+            logger.debug(
+                " Sending 0x%02X command again with %i bytes data",
+                apdu_header[1],
+                len_data,
+            )
+            logger.debug("-> %s", toHexString(apdu))
             t_env = time.time()
-            datacompl, sw_byte1, sw_byte2 = self.connection.transmit(
-                [0x00, 0xC0, 0, 0, 0]
+            try:
+                data, sw_byte1, sw_byte2 = self.connection.transmit(apdu)
+            except CardConnectionException as exc:
+                raise ConnectionException(
+                    "Error while communicating T=0 with the OpenGPG device."
+                ) from exc
+            t_ans = (time.time() - t_env) * 1000
+            logger.debug(
+                " Read %i bytes data : SW 0x%02X%02X - %.1f ms",
+                len(data),
+                sw_byte1,
+                sw_byte2,
+                t_ans,
             )
+            logger.debug("<- %s", toHexString(data))
+        while sw_byte1 in [0x61, 0x9F, 0x9E]:
+            logger.debug("Sending GET RESPONSE for %i bytes", sw_byte2)
+            t_env = time.time()
+            apdu = [0x00, 0xC0, 0, 0, sw_byte2]
+            datacompl, sw_byte1, sw_byte2 = self.connection.transmit(apdu)
             t_ans = (time.time() - t_env) * 1000
             logger.debug(
-                " Received remaining %i bytes : 0x%02X%02X - duration: %.1f ms"
-                % (len(datacompl), sw_byte1, sw_byte2, t_ans)
+                " Received remaining %i bytes : 0x%02X%02X - duration: %.1f ms",
+                len(datacompl),
+                sw_byte1,
+                sw_byte2,
+                t_ans,
             )
-            logger.debug(f"<- {toHexString(datacompl)}")
+            logger.debug("<- %s", toHexString(datacompl))
             data += datacompl
         if sw_byte1 == 0x63 and sw_byte2 & 0xF0 == 0xC0:
             raise PinException(sw_byte2 - 0xC0)
         if sw_byte1 != 0x90 or sw_byte2 != 0x00:
             raise PGPCardException(sw_byte1, sw_byte2)
         return data
 
@@ -302,15 +331,15 @@
         ]
         data = toBytes("60 04 5C 02" + filehex)
         self.send_apdu(apdu_command, data)
 
     @check_hex
     def get_data(self, filehex, data_hex=""):
         """Binary read / ISO read the object"""
-        logger.debug(f"Read Data {data_hex} in 0x{filehex}")
+        logger.debug("Read Data %s in 0x%s", data_hex, filehex)
         param_1 = int(filehex[0:2], 16)
         param_2 = int(filehex[2:4], 16)
         apdu_command = [0x00, 0xCA, param_1, param_2]
         if len(data_hex) == 2:
             data_hex = "00" + data_hex
         dataresp = self.send_apdu(apdu_command, toBytes(data_hex), self.longer)
         return dataresp
@@ -320,15 +349,15 @@
         logger.debug("Read next data %s", data_hex)
         apdu_command = [0x00, 0xCC, param_1, param_2]
         blkdata = self.send_apdu(apdu_command, toBytes(data_hex))
         return blkdata
 
     @check_hex
     def put_data(self, filehex, data_hex=""):
-        logger.debug(f"Put data {data_hex} in 0x{filehex}")
+        logger.debug("Put data %s in 0x%s", data_hex, filehex)
         param_1 = int(filehex[0:2], 16)
         param_2 = int(filehex[2:4], 16)
         apdu_command = [0x00, 0xDA, param_1, param_2]  # or 0xDB command
         blkdata = self.send_apdu(apdu_command, toBytes(data_hex))
         return blkdata
 
     def get_identifier(self):
@@ -346,19 +375,17 @@
         self.manufacturer_id = f"0x{resp[8]:02X}{resp[9]:02X}"
         manufacturer_id_int = int(self.manufacturer_id, 16)
         if manufacturer_id_int in OpenPGPcard.manufacturer_list:
             self.manufacturer = OpenPGPcard.manufacturer_list[manufacturer_id_int]
         else:
             self.manufacturer = OpenPGPcard.default_manufacturer_name
         self.serial = int.from_bytes(resp[10:14], "big")
-        if self.pgpvermaj >= 3:
-            self.longer = APDU_LONG
-        logger.debug(f"PGP version : {self.pgpverstr}")
-        logger.debug(f"Manufacturer : {self.manufacturer} ({self.manufacturer_id})")
-        logger.debug(f"Serial : {self.serial}")
+        logger.debug("PGP version : %s", self.pgpverstr)
+        logger.debug("Manufacturer : %s (%s)", self.manufacturer, self.manufacturer_id)
+        logger.debug("Serial : %s", self.serial)
 
     def get_length(self):
         """Extended length info DO 7F66 : 0202 xxxx 0202 xxxx
         Also bit 7 in Application Data "0x73"
         """
         self.max_cmd = 256
         self.max_rsp = 256
@@ -368,14 +395,16 @@
                 self.max_cmd = int.from_bytes(resp[2:4], "big")
                 self.max_rsp = int.from_bytes(resp[6:8], "big")
             elif len(resp) == 11 and resp[:3] == [0x7F, 0x66, 8]:  # Constructed DO
                 self.max_cmd = int.from_bytes(resp[5:7], "big")
                 self.max_rsp = int.from_bytes(resp[9:11], "big")
             else:
                 raise DataException("Extended length info incorrect format.")
+            if self.max_cmd > APDU_SHORT and self.max_rsp > APDU_SHORT:
+                self.longer = APDU_LONG
 
     def get_pwstatus(self):
         return self.get_data("C4")
 
     def get_features(self):
         """Features optional DO 7F74"""
         self.display = False
@@ -443,14 +472,15 @@
             if exc.sw_code == 0x6D00:
                 # Retry after 3 seconds
                 time.sleep(3)
                 # Select again the applet
                 self.send_apdu([0x00, 0xA4, 0x04, 0x00], OpenPGPcard.AppID)
                 time.sleep(1)
                 return self.get_application_data()
+            raise exc
         app_rel_data = decode_do(resp)
         if resp[0] == 0x6E:
             app_rel_data = app_rel_data["6E"]
         # Set the attribute about max PW length
         pwstatus_data = bytes.fromhex(app_rel_data["73"]["C4"])
         if pwstatus_data[1] < 128:
             self.pw1_maxlen = pwstatus_data[1]
@@ -490,20 +520,20 @@
                 if exc.sw_code == 0x6983:
                     return 0
                 if exc.sw_code != 0x6A80:
                     raise exc
         # Fallback to PW status "C4"
         resp = self.get_pwstatus()
         if len(resp) != 7:
-            raise PGPCardException("Bad PW status status data")
+            raise ConnectionException("Bad PW status status data")
         if pin_bank == 1:
             return resp[4]
         elif pin_bank == 3:
             return resp[6]
-        raise PGPCardException("Only PW1 and PW3 are available for status")
+        raise ConnectionException("Only PW1 and PW3 are available for status")
 
     def change_pin(self, old_pin, new_pin, pin_index):
         """Change PIN index number (index : 1 or 3)."""
         if pin_index not in (3, 1):
             raise DataException("Bad PIN index, must be 1 or 3.")
         old_pin_bin = old_pin.encode("utf8")
         new_pin_bin = new_pin.encode("utf8")
@@ -511,25 +541,25 @@
         if pin_index == 3:
             pin_min_len = 8
         if len(old_pin_bin) < pin_min_len or len(new_pin_bin) < pin_min_len:
             raise BadInputException(
                 f"Bad PIN #{pin_index} length, must be {pin_min_len} bytes."
             )
         data = old_pin_bin + new_pin_bin
-        self.send_apdu([0, 0x24, 0, 0x80 + pin_index], to_list(data))
+        self.send_apdu([0, 0x24, 0, 0x80 + pin_index], list(data))
 
     def verify_pin(self, pin_bank, pin_string):
         """Verify PIN code : pin_bank is 1, 2 or 3 for SW1, SW2 or SW3
         Call CHANGE REFERENCE DATA card command
         """
         if pin_bank not in (1, 2, 3):
             raise DataException("Bad PIN index, must be 1, 2 or 3.")
         if pin_string:
             self.send_apdu(
-                [0, 0x20, 0, 0x80 + pin_bank], to_list(pin_string.encode("utf8"))
+                [0, 0x20, 0, 0x80 + pin_bank], list(pin_string.encode("utf8"))
             )
         else:
             self.send_apdu([0, 0x20, 0, 0x80 + pin_bank], [])
 
     @check_hex
     def gen_key(self, keypos_hex):
         """Generate an asymmetric key pair in keypos slot address
@@ -546,30 +576,30 @@
         """Get the public part of the key pair in keypos slot address"""
         return bytes(
             self.send_apdu([0, 0x47, 0x81, 0], toBytes(keypos_hex), self.longer)
         )
 
     def sign(self, data):
         """Sign data, with Compute Digital Signature command"""
-        return bytes(self.send_apdu([0, 0x2A, 0x9E, 0x9A], to_list(data)))
+        return bytes(self.send_apdu([0, 0x2A, 0x9E, 0x9A], list(data)))
 
     def sign_ec_der(self, hashdata):
         """Sign with ECDSA hash data and output signature as ASN1 DER encoded
         hashdata is the same size in bits of the EC key
         """
         return encode_der(self.sign(hashdata))
 
     def encipher(self):
         """Call ENC command
         ToDo
         """
         raise NotImplementedError()
 
     def decipher(self, data):
-        return bytes(self.send_apdu([0, 0x2A, 0x80, 0x86], to_list(data)))
+        return bytes(self.send_apdu([0, 0x2A, 0x80, 0x86], list(data)))
 
     def decipher_25519(self, ext_pubkey):
         """For ECDH with Curve25519
         ext_pubkey is a 32 bytes "x" public key
         """
         data_field = b"\xA6\x12\x7F\x49\x22\x86\x20" + ext_pubkey
         return self.decipher(data_field)
```

## Comparing `OpenPGPpy-1.1.dist-info/LICENSE` & `OpenPGPpy-1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `OpenPGPpy-1.1.dist-info/METADATA` & `OpenPGPpy-1.2.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,285 +1,279 @@
-Metadata-Version: 2.1
-Name: OpenPGPpy
-Version: 1.1
-Summary: OpenPGP smartcard communication library
-Home-page: https://github.com/bitlogik/OpenPGPpy
-Author: BitLogiK
-Author-email: contact@bitlogik.fr
-License: GPLv3
-Keywords: cryptography security openpgp hardware
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: Topic :: Communications :: Email
-Classifier: Topic :: Security :: Cryptography
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: pyscard (==2.0.3)
-Provides-Extra: dev
-Requires-Dist: PyNaCl (==1.5.0) ; extra == 'dev'
-
-
-# OpenPGPpy
-
-
-### OpenPGP smartcard communication library
-
-A Python3 library to operate an OpenPGP device.
-
-Provides access methods in Python to an OpenPGP card application, as defined in  
-https://gnupg.org/ftp/specs/OpenPGP-smart-card-application-3.3.pdf
-
-No need to have GnuPG or similar binary, with OpenPGPpy one can setup and use an OpenPGP device (such as Yubico 5) right away in Python.
-
-
-## Installation and requirements
-
-Works with Python >= 3.6.
-
-Requires PCSCd on Linux
-
-Ubuntu / Debian  
-`(sudo) apt-get install python3-pip python3-pyscard python3-setuptools pcscd`
-
-Fedora / CentOS / RHEL  
-`yum install python3-pip python3-pyscard python3-setuptools pcsc-lite-ccid`
-
-On some Linux, starts PCSCd service
-```
-(sudo) systemctl start pcscd
-(sudo) systemctl enable pcscd
-```
-
-It uses Pyscard, but this is listed in pip dependencies. So Pyscard is automatically installed when you install this package. In Linux, We recommend to install Pyscard using the distro package manager (see above).
-
-### Installation of this library
-
-Easiest way :  
-`python3 -m pip install OpenPGPpy`  
-
-From sources, download and run in this directory :  
-`python3 -m pip  install .`
-
-### Use
-
-Instanciate a device with `OpenPGPpy.OpenPGPcard()`, then use methods functions of this object.
-
-OpenPGPcard() throws an PGPCardException exception if no OpenPGP device can be found.
-
-Basic example :
-
-```
-import OpenPGPpy
-mydevice = OpenPGPpy.OpenPGPcard()
-mydevice.verify_pin(1, "123456")
-mydevice.sign(hash_or_msg_to_sign)
-```
-
-See demo and interface methods to get the full functions and details.
-
-#### Demo
-
-There are some demonstration scripts provided in the *demo* directory. They provide examples on how to use this library.
-
-* reset.py : resets the OpenPGP device.
-* decrypt.py : Generates an X25519 key pair that is used to DECipher data (compute X25519 ECDH).
-* sign.py : Generates a 256k1 key pair, then uses it to sign data.
-* signEd.py : Generates a Ed25519 key pair, then uses it to sign data.
-
-The *decrypt.py* and *signEd.py* scripts require the pynacl library to check the device responses. This can be installed with the "dev" dependencies part of this package `python3 -m pip  install .["dev"]` or just `python3 -m pip install pynacl`.
-
-The *sign.py* script requires openssl binary in the user path to check the device responses.
-
-*sign* and *signEd* can't be used together. Perform a reset of the card between one and the other.
-
-Default PIN password for OpenPGP devices :  
-PIN1 : "123456"  
-PIN2 : "123456"  
-PIN3 : "12345678"
-
-
-**Breaking changes** in v0.6 :
-* The debug argument is removed from the instanciate method, and from the class object attribute. Now this library uses logger.debug(). Use a standard logger in your app and you'll get or print the debug traces from this library. It was previsouly printed out in the standard ouput, now it is always output in the logger debug.
-* The get_application_data method returns a Python object, instead of the bytes array raw response from the device. The raw response is internally ASN1-BER decoded, with hex data strings for DOs content.
-
-## Interface Methods
-
-`OpenPGPcard( reader_index=None )`  
-Initializes the OpenPGP device object.  
-Connects to all readers seeking for an OpenPGP card, selects the app and loads its capabilities.  
-reader_index = None : the constructor will use the first OpenPGP card available in any readers slots detected.  
-reader_index = positive integer : will try to use the given reader/card at the given index (starts at 0).
-
-The created object has the following attributes :
-* .name : str, name of the device (or the card reader used)
-* .pgpvermaj : int, OpenPGP application major version (2 or 3)
-* .pgpvermin : int, OpenPGP application minor version
-* .pgpverstr : string, OpenPGP application version "maj.min"
-* .manufacturer_id : string, hex string of the manufacturer ID "0xXXXX"
-* .manufacturer : string, name of the manufacturer (or "- unknown -")
-* .serial : int, serial number
-* .max_cmd : int, maximum command length
-* .max_rsp : int, maximum response length
-* .pw1_maxlen: int, maximum PIN1 length
-* .pw3_maxlen: int, maximum PIN3 length
-* .display : bool, has a display?
-* .bio : bool, has a biometric sensor?
-* .button : bool, has a button?
-* .keypad : bool, has a keypad?
-* .led : bool, has a LED?
-* .speaker : bool, has a speaker?
-* .mic : bool, has a microphone?
-* .touchscreen : bool, has a touchscreen?
-
-`OpenPGPcard.send_apdu( apduHeader, Data, ExpLongResp=0 )`  
-Sends full raw APDU, not supposed to be used by your scripts.  
-apduHeader and Data are lists of integers or bytesarray.  
-apduHeader is [ INS, CLA, P1, P2 ] ISO7816 APDU header, without length info (Lc nor Le).  
-Data is bytes list of the command data  
-ExpLongResp is optional integer, the expected response length. Required when sending a short command and receiving long data back.  
-In case data are cut in parts with "61" code, it automatically sends "C0" command to get remaining data and recontructs the full data.  
-Extended frame length is automatically managed.  
-*Note* if an extended data frame response is expected from a short command, the query command must be called with the ExpLongResp argument equals to 65536. Because the ISO7816 standard only allows symmetric type of communication (extended sent, extended received), and this is the easy way to force the command to be sent with an extended format.  
-Throws PGPCardException if answer status is not 0x9000.  
-Throws ConnectionException if the device is no more available.  
-Returns a bytearray of the card answer.
-
-`OpenPGPcard.select_data( filehex, param_1=0, param_2=4 )`  
-Selects a data object ("DO").  
-filehex is 1 or 2 bytes object address in hex (2-4 string hex).
-
-`OpenPGPcard.get_data( filehex )`  
-Reads a data object ("DO").  
-filehex is 1 or 2 bytes object address in hex (2-4 string hex).  
-Mostly used internally by others methods.
-
-`OpenPGPcard.get_next_data( filehex, param_1=0, param_2=0 )`  
-Continue reading in data object ("DO").  
-filehex is 1 or 2 bytes object address in hex (2-4 string hex).  
-
-`OpenPGPcard.put_data( filehex, data_hex="" )`  
-Write data_hex in data object ("DO").  
-filehex is 1 or 2 bytes object address in hex (2-4 string hex).  
-Used in OpenPGP to configure the device, like key type or user info.
-
-`OpenPGPcard.get_identifier()`  
-Reads and decode the Full Application Identifier (data object 0x4F).  
-Internally called at instanciation.
-
-`OpenPGPcard.get_length()`  
-Only for OpenPGP v3. Reads and decode the Extended Length Info (data object "7F66").  
-Internally called at instanciation. The max attributes loaded are not yet used by others methods.
-
-`OpenPGPcard.get_features()`  
-Reads and decode the optional General Feature Management (data object "7F74").  
-Internally called at instanciation. If not present, all features are supposed to be unavailable (attributes are False by default).
-
-`OpenPGPcard.display_features()`  
-Prints the General Feature Management attributes.
-Internally used by get_features for debug output.
-
-`OpenPGPcard.get_historical_bytes()`  
-Raw read of the Historical Bytes (data object "5F52").
-
-`OpenPGPcard.get_application_data()`  
-Get the Application Related Data (data object "6E").  
-Return the content of the "6E" data object as a Python object with hex encodings data.
-
-`OpenPGPcard.get_pwstatus()`  
-Get the PW Status (data object "C4").  
-Return the content of the "C4" data object as raw bytearray data.
-
-`OpenPGPcard.terminate_df()`  
-Send the TERMINATE DF command. Used to reset the card.
-
-`OpenPGPcard.activate_file()`  
-Send the ACTIVATE FILE command. Used to reset the card.
-
-`OpenPGPcard.reset( pin3 )`  
-Fully reset the device. Requires the "PUK" PIN #3 as a string.
-
-`OpenPGPcard.get_random( data_length )`  
-Reads random data from the device, using the GET CHALLENGE command (data_length bytes long).
-
-`OpenPGPcard.change_pin( old_pin, new_pin, pin_bank )`  
-Change the PIN in the bank 1 or 3 (PIN1 or PIN3). old_pin and new_pin are strings.  
-Minimum PIN length is 6 chars for PIN1, 8 chars for PIN3.
-
-`OpenPGPcard.verify_pin( pin_bank, pin )`  
-Verify the PIN code : pin_bank is 1, 2 or 3 for respectively SW1, SW2 or SW3. pin is a string with the PIN.
-
-`OpenPGPcard.get_pin_status( pin_bank )`  
-Reads PIN status : returns remaining tries left for the given PIN bank address (1, 2 or 3).  
-Return value is the number of remaining tries before the PIN block.  
-Return value is 0 : PIN is blocked (no more tries).  
-Return value is 9000 : PIN has been verified (OK).
-
-`OpenPGPcard.gen_key( keypos_hex )`  
-Generates an assymetric key pair in a keypos slot address, by calling the GENERATE ASYMMETRIC KEY PAIR command. keypos_hex is the key object address (Control Reference Template) as 4 chars string (2 bytes address) : "B600" for sign key, "B800" for de/crypt key, "A400" for auth key.  
-Usually, the device reponds with the related public key of the key generated.  
-Requires the PIN3 "PUK" verified.
-
-`OpenPGPcard.get_public_key( keypos_hex )`  
-Reads the public key in keypos slot address, by calling the GENERATE ASYMMETRIC KEY PAIR command (with the read pubkey flag). keypos_hex is the key object address (Control Reference Template) as 4 chars string "hex" (2 bytes address) : "B600" for sign key ref1, "B800" for de/crypt key ref2, "A400" for auth key ref3.  
-Requires the related PIN verified.
-
-`OpenPGPcard.sign( data )`  
-Signs data with the internal device SIGn key (Ref1), calling the COMPUTE DIGITAL SIGNATURE command.  
-data is in bytes "binary" format. With ECDSA, data is the hash to sign.  
-Requires the PIN1 verified.  
-See the OpenPGP application standard for more details about data format.
-
-`OpenPGPcard.sign_ec_der( datahash )`
-ECDSA signs with the internal device SIGn key the hash datahash (bytes) and outputs the signature as ASN1 DER encoded (bytes). Requires the SIG key to be an EC type key pair ("13..." in "C1").  
-Requires the PIN1 verified.
-
-`OpenPGPcard.decipher( data )`  
-Decrypts data with the internal device DECryption key (Ref2), calling the DECIPHER command.  
-data is in bytes "binary" format.  
-For RSA : decrypts data, data input must be formatted according to PKCS#1 before encryption (device is checking padding conformance).  
-For EC : performs an ECDH with the provided public key in data and the internal device DECryption private key.  
-Requires the PIN2 verified.  
-See the OpenPGP application standard for more details.
-
-`OpenPGPcard.decipher_25519( external_publickey )`  
-Decrypts data with the internal device DECryption key with X25519 (Curve25519 ECDH). Obviously, requires the DEC key to be a Curve25519 key pair ("122B060104019755010501" in "C2"). As DECIPHER with EC, the device doesn\'t decrypt data, but computes the private "shared" symmetric key with ECDH. Still quite like RSA where the decrypted data is also the private shared symmetric key.  
-external_publickey argument is "x" 32 bytes, as bytes. It performs an ECDH with the provided public key and the internal device DECryption private key.  
-Requires the PIN2 verified.  
-
-
-## License
-
-Copyright (C) 2020-2021  BitLogiK SAS
-
-This program is free software: you can redistribute it and/or modify  
-it under the terms of the GNU General Public License as published by  
-the Free Software Foundation, version 3 of the License.
-
-This program is distributed in the hope that it will be useful,  
-but WITHOUT ANY WARRANTY; without even the implied warranty of  
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  
-See the GNU General Public License for more details.
-
-
-## ToDo
-
-* Secure Messaging
-* Verify
-* Sign helpers (RSA Tag/DSI)
-* Encipher
-* Make it more user friendly with more abstraction layers and data list, for example set_key(2, "X25519") sends PUT_DATA("122B060104019755010501") in "C2"
-
-
-## Support
-
-Open an issue in the Github repository for help about its use.
-
-
-
-
+Metadata-Version: 2.1
+Name: OpenPGPpy
+Version: 1.2
+Summary: OpenPGP smartcard communication library
+Home-page: https://github.com/bitlogik/OpenPGPpy
+Author: BitLogiK
+Author-email: contact@bitlogik.fr
+License: GPLv3
+Keywords: cryptography security openpgp hardware
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: Communications :: Email
+Classifier: Topic :: Security :: Cryptography
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Hardware
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyscard ==2.0.8
+Provides-Extra: dev
+Requires-Dist: PyNaCl ==1.5.0 ; extra == 'dev'
+
+# OpenPGPpy
+
+### OpenPGP smartcard communication library
+
+A Python3 library to operate an OpenPGP device.
+
+Provides access methods in Python to an OpenPGP card application, as defined in  
+https://gnupg.org/ftp/specs/OpenPGP-smart-card-application-3.3.pdf
+
+No need to have GnuPG or similar binary, with OpenPGPpy one can setup and use an OpenPGP device (such as Yubico 5) right away in Python.
+
+## Installation and requirements
+
+Works with Python >= 3.6.
+
+Requires PCSCd on Linux
+
+Ubuntu / Debian  
+`(sudo) apt-get install python3-pip python3-pyscard python3-setuptools pcscd`
+
+Fedora / CentOS / RHEL  
+`yum install python3-pip python3-pyscard python3-setuptools pcsc-lite-ccid`
+
+On some Linux, starts PCSCd service
+
+```
+(sudo) systemctl start pcscd
+(sudo) systemctl enable pcscd
+```
+
+It uses Pyscard, and this is listed in pip dependencies. So Pyscard is automatically installed when you install this package. In Linux, We recommend to install Pyscard using the distro package manager (see above).
+
+### Installation of this library
+
+Easiest way :  
+`python3 -m pip install OpenPGPpy`  
+
+From sources, download and run in this directory :  
+`python3 -m pip install .`
+
+### Use
+
+Instanciate a device with `OpenPGPpy.OpenPGPcard()`, then use methods functions of this object.
+
+OpenPGPcard() throws an PGPCardException exception if no OpenPGP device can be found.
+
+Basic example :
+
+```
+import OpenPGPpy
+mydevice = OpenPGPpy.OpenPGPcard()
+mydevice.verify_pin(1, "123456")
+mydevice.sign(hash_or_msg_to_sign)
+```
+
+See demo and interface methods to get the full functions and details.
+
+#### Demo
+
+There are some demonstration scripts provided in the *demo* directory. They provide examples on how to use this library.
+
+* reset.py : resets the OpenPGP device.
+* decrypt.py : Generates an X25519 key pair that is used to DECipher data (compute X25519 ECDH).
+* sign.py : Generates a 256k1 key pair, then uses it to sign data.
+* signEd.py : Generates a Ed25519 key pair, then uses it to sign data.
+
+The *decrypt.py* and *signEd.py* scripts require the pynacl library to check the device responses. This can be installed with the "dev" dependencies part of this package `python3 -m pip  install .["dev"]` or just `python3 -m pip install pynacl`.
+
+The *sign.py* script requires openssl binary in the user path to check the device responses.
+
+*sign* and *signEd* can't be used together. Perform a reset of the card between one and the other.
+
+Default PIN password for OpenPGP devices :  
+PIN1 : "123456"  
+PIN2 : "123456"  
+PIN3 : "12345678"
+
+**Breaking changes** in v0.6 :
+
+* The debug argument is removed from the instanciate method, and from the class object attribute. Now this library uses logger.debug(). Use a standard logger in your app and you'll get or print the debug traces from this library. It was previsouly printed out in the standard ouput, now it is always output in the logger debug.
+* The get_application_data method returns a Python object, instead of the bytes array raw response from the device. The raw response is internally ASN1-BER decoded, with hex data strings for DOs content.
+
+## Interface Methods
+
+`OpenPGPcard( reader_index=None )`  
+Initializes the OpenPGP device object.  
+Connects to all readers seeking for an OpenPGP card, selects the app and loads its capabilities.  
+reader_index = None : the constructor will use the first OpenPGP card available in any readers slots detected.  
+reader_index = positive integer : will try to use the given reader/card at the given index (starts at 0).
+
+The created object has the following attributes :
+
+* .name : str, name of the device (or the card reader used)
+* .pgpvermaj : int, OpenPGP application major version (2 or 3)
+* .pgpvermin : int, OpenPGP application minor version
+* .pgpverstr : string, OpenPGP application version "maj.min"
+* .manufacturer_id : string, hex string of the manufacturer ID "0xXXXX"
+* .manufacturer : string, name of the manufacturer (or "- unknown -")
+* .serial : int, serial number
+* .max_cmd : int, maximum command length
+* .max_rsp : int, maximum response length
+* .pw1_maxlen: int, maximum PIN1 length
+* .pw3_maxlen: int, maximum PIN3 length
+* .display : bool, has a display?
+* .bio : bool, has a biometric sensor?
+* .button : bool, has a button?
+* .keypad : bool, has a keypad?
+* .led : bool, has a LED?
+* .speaker : bool, has a speaker?
+* .mic : bool, has a microphone?
+* .touchscreen : bool, has a touchscreen?
+
+`OpenPGPcard.send_apdu( apduHeader, Data, ExpLongResp=0 )`  
+Sends full raw APDU, not supposed to be used by your scripts.  
+apduHeader and Data are lists of integers or bytesarray.  
+apduHeader is [ INS, CLA, P1, P2 ] ISO7816 APDU header, without length info (Lc nor Le).  
+Data is bytes list of the command data  
+ExpLongResp is optional integer, the expected response length. Required when sending a short command and receiving long data back.  
+In case data are cut in parts with "61" code, it automatically sends "C0" command to get remaining data and recontructs the full data.  
+Extended frame length is automatically managed.  
+*Note* if an extended data frame response is expected from a short command, the query command must be called with the ExpLongResp argument equals to 65536. Because the ISO7816 standard only allows symmetric type of communication (extended sent, extended received), and this is the easy way to force the command to be sent with an extended format.  
+Throws PGPCardException if answer status is not 0x9000.  
+Throws ConnectionException if the device is no more available.  
+Returns a bytearray of the card answer.
+
+`OpenPGPcard.select_data( filehex, param_1=0, param_2=4 )`  
+Selects a data object ("DO").  
+filehex is 1 or 2 bytes object address in hex (2-4 string hex).
+
+`OpenPGPcard.get_data( filehex )`  
+Reads a data object ("DO").  
+filehex is 1 or 2 bytes object address in hex (2-4 string hex).  
+Mostly used internally by others methods.
+
+`OpenPGPcard.get_next_data( filehex, param_1=0, param_2=0 )`  
+Continue reading in data object ("DO").  
+filehex is 1 or 2 bytes object address in hex (2-4 string hex).  
+
+`OpenPGPcard.put_data( filehex, data_hex="" )`  
+Write data_hex in data object ("DO").  
+filehex is 1 or 2 bytes object address in hex (2-4 string hex).  
+Used in OpenPGP to configure the device, like key type or user info.
+
+`OpenPGPcard.get_identifier()`  
+Reads and decode the Full Application Identifier (data object 0x4F).  
+Internally called at instanciation.
+
+`OpenPGPcard.get_length()`  
+Only for OpenPGP v3. Reads and decode the Extended Length Info (data object "7F66").  
+Internally called at instanciation.
+
+`OpenPGPcard.get_features()`  
+Reads and decode the optional General Feature Management (data object "7F74").  
+Internally called at instanciation. If not present, all features are supposed to be unavailable (attributes are False by default).
+
+`OpenPGPcard.display_features()`  
+Prints the General Feature Management attributes.
+Internally used by get_features for debug output.
+
+`OpenPGPcard.get_historical_bytes()`  
+Raw read of the Historical Bytes (data object "5F52").
+
+`OpenPGPcard.get_application_data()`  
+Get the Application Related Data (data object "6E").  
+Return the content of the "6E" data object as a Python object with hex encodings data.
+
+`OpenPGPcard.get_pwstatus()`  
+Get the PW Status (data object "C4").  
+Return the content of the "C4" data object as raw bytearray data.
+
+`OpenPGPcard.terminate_df()`  
+Send the TERMINATE DF command. Used to reset the card.
+
+`OpenPGPcard.activate_file()`  
+Send the ACTIVATE FILE command. Used to reset the card.
+
+`OpenPGPcard.reset( pin3 )`  
+Fully reset the device. Requires the "PUK" PIN #3 as a string.
+
+`OpenPGPcard.get_random( data_length )`  
+Reads random data from the device, using the GET CHALLENGE command (data_length bytes long).
+
+`OpenPGPcard.change_pin( old_pin, new_pin, pin_bank )`  
+Change the PIN in the bank 1 or 3 (PIN1 or PIN3). old_pin and new_pin are strings.  
+Minimum PIN length is 6 chars for PIN1, 8 chars for PIN3.
+
+`OpenPGPcard.verify_pin( pin_bank, pin )`  
+Verify the PIN code : pin_bank is 1, 2 or 3 for respectively SW1, SW2 or SW3. pin is a string with the PIN.
+
+`OpenPGPcard.get_pin_status( pin_bank )`  
+Reads PIN status : returns remaining tries left for the given PIN bank address (1, 2 or 3).  
+Return value is the number of remaining tries before the PIN block.  
+Return value is 0 : PIN is blocked (no more tries).  
+Return value is 9000 : PIN has been verified (OK).
+
+`OpenPGPcard.gen_key( keypos_hex )`  
+Generates an assymetric key pair in a keypos slot address, by calling the GENERATE ASYMMETRIC KEY PAIR command. keypos_hex is the key object address (Control Reference Template) as 4 chars string (2 bytes address) : "B600" for sign key, "B800" for de/crypt key, "A400" for auth key.  
+Usually, the device reponds with the related public key of the key generated.  
+Requires the PIN3 "PUK" verified.
+
+`OpenPGPcard.get_public_key( keypos_hex )`  
+Reads the public key in keypos slot address, by calling the GENERATE ASYMMETRIC KEY PAIR command (with the read pubkey flag). keypos_hex is the key object address (Control Reference Template) as 4 chars string "hex" (2 bytes address) : "B600" for sign key ref1, "B800" for de/crypt key ref2, "A400" for auth key ref3.  
+Requires the related PIN verified.
+
+`OpenPGPcard.sign( data )`  
+Signs data with the internal device SIGn key (Ref1), calling the COMPUTE DIGITAL SIGNATURE command.  
+data is in bytes "binary" format. With ECDSA, data is the hash to sign.  
+Requires the PIN1 verified.  
+See the OpenPGP application standard for more details about data format.
+
+`OpenPGPcard.sign_ec_der( datahash )`
+ECDSA signs with the internal device SIGn key the hash datahash (bytes) and outputs the signature as ASN1 DER encoded (bytes). Requires the SIG key to be an EC type key pair ("13..." in "C1").  
+Requires the PIN1 verified.
+
+`OpenPGPcard.decipher( data )`  
+Decrypts data with the internal device DECryption key (Ref2), calling the DECIPHER command.  
+data is in bytes "binary" format.  
+For RSA : decrypts data, data input must be formatted according to PKCS#1 before encryption (device is checking padding conformance).  
+For EC : performs an ECDH with the provided public key in data and the internal device DECryption private key.  
+Requires the PIN2 verified.  
+See the OpenPGP application standard for more details.
+
+`OpenPGPcard.decipher_25519( external_publickey )`  
+Decrypts data with the internal device DECryption key with X25519 (Curve25519 ECDH). Obviously, requires the DEC key to be a Curve25519 key pair ("122B060104019755010501" in "C2"). As DECIPHER with EC, the device doesn\'t decrypt data, but computes the private "shared" symmetric key with ECDH. Still quite like RSA where the decrypted data is also the private shared symmetric key.  
+external_publickey argument is "x" 32 bytes, as bytes. It performs an ECDH with the provided public key and the internal device DECryption private key.  
+Requires the PIN2 verified.  
+
+## License
+
+Copyright (C) 2020-2024  BitLogiK SAS
+
+This program is free software: you can redistribute it and/or modify  
+it under the terms of the GNU General Public License as published by  
+the Free Software Foundation, version 3 of the License.
+
+This program is distributed in the hope that it will be useful,  
+but WITHOUT ANY WARRANTY; without even the implied warranty of  
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  
+See the GNU General Public License for more details.
+
+## ToDo
+
+* Secure Messaging
+* Verify
+* Sign helpers (RSA Tag/DSI)
+* Encipher
+* Make it more user friendly with more abstraction layers and data list, for example set_key(2, "X25519") sends PUT_DATA("122B060104019755010501") in "C2"
+
+## Support
+
+Open an issue in the Github repository for help about its use.
+
+
```

