# Comparing `tmp/pymyenergi-0.1.1.tar.gz` & `tmp/pymyenergi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymyenergi-0.1.1.tar", last modified: Mon Mar 11 20:23:55 2024, max compression
+gzip compressed data, was "pymyenergi-0.2.0.tar", last modified: Mon Jun  3 11:37:56 2024, max compression
```

## Comparing `pymyenergi-0.1.1.tar` & `pymyenergi-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:23:55.078359 pymyenergi-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-03-11 20:23:55.078359 pymyenergi-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:23:55.074359 pymyenergi-0.1.1/pymyenergi/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/base_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/ct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/eddi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/harvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/libbi.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/pymyenergi/zappi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:23:55.078359 pymyenergi-0.1.1/pymyenergi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-03-11 20:23:55.000000 pymyenergi-0.1.1/pymyenergi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-11 20:23:55.000000 pymyenergi-0.1.1/pymyenergi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 20:23:55.000000 pymyenergi-0.1.1/pymyenergi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-11 20:23:55.000000 pymyenergi-0.1.1/pymyenergi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 20:23:55.000000 pymyenergi-0.1.1/pymyenergi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-11 20:23:55.000000 pymyenergi-0.1.1/pymyenergi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-11 20:23:55.078359 pymyenergi-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:23:55.078359 pymyenergi-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/tests/test_eddi.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/tests/test_harvi.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/tests/test_libbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-11 20:23:49.000000 pymyenergi-0.1.1/tests/test_zappi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:37:56.033929 pymyenergi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-06-03 11:37:56.033929 pymyenergi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:37:56.029929 pymyenergi-0.2.0/pymyenergi/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/base_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12350 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/ct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/eddi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/harvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/libbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/pymyenergi/zappi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:37:56.033929 pymyenergi-0.2.0/pymyenergi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-06-03 11:37:56.000000 pymyenergi-0.2.0/pymyenergi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-06-03 11:37:56.000000 pymyenergi-0.2.0/pymyenergi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 11:37:56.000000 pymyenergi-0.2.0/pymyenergi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 11:37:56.000000 pymyenergi-0.2.0/pymyenergi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-03 11:37:56.000000 pymyenergi-0.2.0/pymyenergi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-03 11:37:56.000000 pymyenergi-0.2.0/pymyenergi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-06-03 11:37:56.033929 pymyenergi-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 11:37:56.033929 pymyenergi-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/tests/test_eddi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/tests/test_harvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/tests/test_libbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-03 11:37:51.000000 pymyenergi-0.2.0/tests/test_zappi.py
```

### Comparing `pymyenergi-0.1.1/LICENSE` & `pymyenergi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymyenergi-0.1.1/PKG-INFO` & `pymyenergi-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,62 @@
-Metadata-Version: 2.1
-Name: pymyenergi
-Version: 0.1.1
-Summary: Python library and CLI for communicating with myenergi API.
-Home-page: https://github.com/cjne/pymyenergi
-Author: Johan Isaksson
-Author-email: johan@generatorhallen.se
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx
-Requires-Dist: pycognito
-
 # pymyenergi
 
-An async python library for myenergi API
+An async Python library for myenergi API
 
 This is a very early release, things are changing rapidly so use at your own risk!
 
-_NOTE:_ This work is not officially supported by myenergi and functionality can stop working at any time without warning
+> [!IMPORTANT]
+> This work is not officially supported by myenergi and functionality can stop working at any time without warning
 
 ## Installation
 
-The easiest method is to install using pip3/pip (venv is also a good idea)
+The easiest method is to install using pip (`pip`/`pip3`):
 
-```
+```bash
 pip install pymyenergi
 ```
 
-to update to the latest version
+Installing within a [Python virtual environment](https://docs.python.org/3/library/venv.html) is often a good idea:
 
+```bash
+python -m venv .venv
+source .venv/bin/activate
+pip install pymyenergi
 ```
+
+To update to the latest version:
+
+```bash
 pip install pymyenergi -U
 ```
 
-Setup will add a cli under the name myenergicli, see below for usage
+Setup will add a CLI under the name `myenergicli`. See below for usage.
 
 ## CLI
 
-A simple cli is provided with this library.
+A simple CLI is provided with this library.
+
+If no `username`, `password`, `app_email` or `app_password` is supplied as input arguments, and no configuration file is found, you will be prompted for credentials.
 
-If no username, password, app_email or app_password is supplied as input arguments and no configuration file is found you will be prompted.
-Configuration file will be searched for in ./.myenergi.cfg and ~/.myenergi.cfg
+Configuration file will be searched for in `./.myenergi.cfg` and `~/.myenergi.cfg`.
 
 ### Example configuration file
 
-```
+```ini
 [hub]
 serial=12345678
-password=yourpassword
+password=your-password
 app_email=myemail@email.com
-app_password=yourapppassword
+app_password=your-app-password
 ```
 
 ### CLI usage
 
 ```
-usage: myenergi [-h] [-u USERNAME] [-p PASSWORD] [-e APP_EMAIL] [-a APP_PASSWORD] [-d] [-j]
+usage: myenergi [-h] [-u USERNAME] [-p PASSWORD] [-e APP_EMAIL] [-a APP_PASSWORD] [-d] [-j] [--skip-oauth]
                 {list,overview,zappi,eddi,harvi,libbi} ...
 
 myenergi CLI.
 
 positional arguments:
   {list,overview,zappi,eddi,harvi,libbi}
                         sub-command help
@@ -82,112 +75,110 @@
   -a APP_PASSWORD, --app_password APP_PASSWORD
   -d, --debug
   -j, --json
 ```
 
 ## Library usage
 
-Install pymyenergi using pip (requires python > 3.6)
+Install pymyenergi using pip (requires Python > 3.6)
 
-### Example client usage
+### Example library usage
 
-```
+```python
 import asyncio
 from pymyenergi.connection import Connection
 from pymyenergi.client import MyenergiClient
 from sys import argv
 import logging
 
 logging.basicConfig()
 logging.root.setLevel(logging.INFO)
 
-user = argv[1]
-password = argv[2]
+user, password = argv
 
 async def zappis() -> None:
     conn = Connection(user, password)
     client = MyenergiClient(conn)
 
     zappis = await client.getDevices('zappi')
     for zappi in zappis:
         print(f"Zappi {zappi.serial_number} charge mode {zappi.charge_mode}")
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(zappis())
 ```
 
-### Example client usage - Zappi
+### Example library usage - Zappi
 
-```
+```python
 import asyncio
 from pymyenergi.connection import Connection
 from pymyenergi.zappi import Zappi
 from sys import argv
 import logging
 
 logging.basicConfig()
 logging.root.setLevel(logging.INFO)
 
-user = argv[1]
-password = argv[2]
-zappi_serial = argv[3]
+user, password, zappi_serial = argv
 
 
 async def get_data() -> None:
     conn = Connection(user, password)
     zappi = Zappi(conn, zappi_serial)
     await zappi.refresh()
     print(f"Zappi S/N {zappi.serial_number} version {zappi.firmware_version}")
     print(f"Status: {zappi.status} Plug status: {zappi.plug_status} Locked: {zappi.locked}")
     print(f"Priority: {zappi.priority}")
     print(f"Charge mode: {zappi.charge_mode} {zappi.num_phases} phase")
-    print("")
+    print()
     print(f"Lock when plugged in   : {zappi.lock_when_pluggedin}")
     print(f"Lock when unplugged    : {zappi.lock_when_unplugged}")
     print(f"Charge when locked     : {zappi.charge_when_locked}")
     print(f"Charge session allowed : {zappi.charge_session_allowed}")
     print(f"Charge added: {zappi.charge_added}")
-    print("")
+    print()
     print(f"CT 1 {zappi.ct1.name} {zappi.ct1.power}W")
     print(f"CT 2 {zappi.ct2.name} {zappi.ct2.power}W")
     print(f"CT 3 {zappi.ct3.name} {zappi.ct3.power}W")
     print(f"CT 4 {zappi.ct4.name} {zappi.ct4.power}W")
     print(f"CT 5 {zappi.ct5.name} {zappi.ct5.power}W")
     print(f"CT 6 {zappi.ct6.name} {zappi.ct6.power}W")
-    print("")
+    print()
     print(f"Supply voltage: {zappi.supply_voltage}V frequency: {zappi.supply_frequency}Hz")
     print("Power:")
     print(f"  Grid      : {zappi.power_grid}W")
     print(f"  Generated : {zappi.power_generated}W")
-    print("")
-    print(f"      Boost start at {zappi.boost_start_hour}:{zappi.boost_start_minute} add {zappi.boost_amount}kWh")
+    print()
+    # print(f"      Boost start at {zappi.boost_start_hour}:{zappi.boost_start_minute} add {zappi.boost_amount}kWh")
     print(f"Smart Boost start at {zappi.smart_boost_start_hour}:{zappi.smart_boost_start_minute} add {zappi.smart_boost_amount}kWh")
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(get_data())
 ```
 
 ## Libbi support
+
 Currently supported features:
 
 - Reads a few values such as State of Charge, DCPV CT
 - Battery in and out energy
 - Gets and sets the current operating mode (normal/stopped/export)
 - Change priority of Libbi
 - Enable/Disable charging from the grid
 - Set charge target (in Wh)
 
-cli examples:
-```
+
+## CLI examples:
+
+```bash
 myenergi libbi show
 myenergi libbi mode normal
 myenergi libbi priority 1
 myenergi libbi energy
 myenergi libbi chargefromgrid false
 myenergi libbi chargetarget 10200
 ```
 
-
-
 ## Credits
 
 [twonk](https://github.com/twonk/MyEnergi-App-Api) for documenting the unofficial API
```

### Comparing `pymyenergi-0.1.1/README.md` & `pymyenergi-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,79 @@
+Metadata-Version: 2.1
+Name: pymyenergi
+Version: 0.2.0
+Summary: Python library and CLI for communicating with myenergi API.
+Home-page: https://github.com/cjne/pymyenergi
+Author: Johan Isaksson
+Author-email: johan@generatorhallen.se
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: pycognito
+
 # pymyenergi
 
-An async python library for myenergi API
+An async Python library for myenergi API
 
 This is a very early release, things are changing rapidly so use at your own risk!
 
-_NOTE:_ This work is not officially supported by myenergi and functionality can stop working at any time without warning
+> [!IMPORTANT]
+> This work is not officially supported by myenergi and functionality can stop working at any time without warning
 
 ## Installation
 
-The easiest method is to install using pip3/pip (venv is also a good idea)
+The easiest method is to install using pip (`pip`/`pip3`):
 
-```
+```bash
 pip install pymyenergi
 ```
 
-to update to the latest version
+Installing within a [Python virtual environment](https://docs.python.org/3/library/venv.html) is often a good idea:
 
+```bash
+python -m venv .venv
+source .venv/bin/activate
+pip install pymyenergi
 ```
+
+To update to the latest version:
+
+```bash
 pip install pymyenergi -U
 ```
 
-Setup will add a cli under the name myenergicli, see below for usage
+Setup will add a CLI under the name `myenergicli`. See below for usage.
 
 ## CLI
 
-A simple cli is provided with this library.
+A simple CLI is provided with this library.
+
+If no `username`, `password`, `app_email` or `app_password` is supplied as input arguments, and no configuration file is found, you will be prompted for credentials.
 
-If no username, password, app_email or app_password is supplied as input arguments and no configuration file is found you will be prompted.
-Configuration file will be searched for in ./.myenergi.cfg and ~/.myenergi.cfg
+Configuration file will be searched for in `./.myenergi.cfg` and `~/.myenergi.cfg`.
 
 ### Example configuration file
 
-```
+```ini
 [hub]
 serial=12345678
-password=yourpassword
+password=your-password
 app_email=myemail@email.com
-app_password=yourapppassword
+app_password=your-app-password
 ```
 
 ### CLI usage
 
 ```
-usage: myenergi [-h] [-u USERNAME] [-p PASSWORD] [-e APP_EMAIL] [-a APP_PASSWORD] [-d] [-j]
+usage: myenergi [-h] [-u USERNAME] [-p PASSWORD] [-e APP_EMAIL] [-a APP_PASSWORD] [-d] [-j] [--skip-oauth]
                 {list,overview,zappi,eddi,harvi,libbi} ...
 
 myenergi CLI.
 
 positional arguments:
   {list,overview,zappi,eddi,harvi,libbi}
                         sub-command help
@@ -65,112 +92,110 @@
   -a APP_PASSWORD, --app_password APP_PASSWORD
   -d, --debug
   -j, --json
 ```
 
 ## Library usage
 
-Install pymyenergi using pip (requires python > 3.6)
+Install pymyenergi using pip (requires Python > 3.6)
 
-### Example client usage
+### Example library usage
 
-```
+```python
 import asyncio
 from pymyenergi.connection import Connection
 from pymyenergi.client import MyenergiClient
 from sys import argv
 import logging
 
 logging.basicConfig()
 logging.root.setLevel(logging.INFO)
 
-user = argv[1]
-password = argv[2]
+user, password = argv
 
 async def zappis() -> None:
     conn = Connection(user, password)
     client = MyenergiClient(conn)
 
     zappis = await client.getDevices('zappi')
     for zappi in zappis:
         print(f"Zappi {zappi.serial_number} charge mode {zappi.charge_mode}")
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(zappis())
 ```
 
-### Example client usage - Zappi
+### Example library usage - Zappi
 
-```
+```python
 import asyncio
 from pymyenergi.connection import Connection
 from pymyenergi.zappi import Zappi
 from sys import argv
 import logging
 
 logging.basicConfig()
 logging.root.setLevel(logging.INFO)
 
-user = argv[1]
-password = argv[2]
-zappi_serial = argv[3]
+user, password, zappi_serial = argv
 
 
 async def get_data() -> None:
     conn = Connection(user, password)
     zappi = Zappi(conn, zappi_serial)
     await zappi.refresh()
     print(f"Zappi S/N {zappi.serial_number} version {zappi.firmware_version}")
     print(f"Status: {zappi.status} Plug status: {zappi.plug_status} Locked: {zappi.locked}")
     print(f"Priority: {zappi.priority}")
     print(f"Charge mode: {zappi.charge_mode} {zappi.num_phases} phase")
-    print("")
+    print()
     print(f"Lock when plugged in   : {zappi.lock_when_pluggedin}")
     print(f"Lock when unplugged    : {zappi.lock_when_unplugged}")
     print(f"Charge when locked     : {zappi.charge_when_locked}")
     print(f"Charge session allowed : {zappi.charge_session_allowed}")
     print(f"Charge added: {zappi.charge_added}")
-    print("")
+    print()
     print(f"CT 1 {zappi.ct1.name} {zappi.ct1.power}W")
     print(f"CT 2 {zappi.ct2.name} {zappi.ct2.power}W")
     print(f"CT 3 {zappi.ct3.name} {zappi.ct3.power}W")
     print(f"CT 4 {zappi.ct4.name} {zappi.ct4.power}W")
     print(f"CT 5 {zappi.ct5.name} {zappi.ct5.power}W")
     print(f"CT 6 {zappi.ct6.name} {zappi.ct6.power}W")
-    print("")
+    print()
     print(f"Supply voltage: {zappi.supply_voltage}V frequency: {zappi.supply_frequency}Hz")
     print("Power:")
     print(f"  Grid      : {zappi.power_grid}W")
     print(f"  Generated : {zappi.power_generated}W")
-    print("")
-    print(f"      Boost start at {zappi.boost_start_hour}:{zappi.boost_start_minute} add {zappi.boost_amount}kWh")
+    print()
+    # print(f"      Boost start at {zappi.boost_start_hour}:{zappi.boost_start_minute} add {zappi.boost_amount}kWh")
     print(f"Smart Boost start at {zappi.smart_boost_start_hour}:{zappi.smart_boost_start_minute} add {zappi.smart_boost_amount}kWh")
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(get_data())
 ```
 
 ## Libbi support
+
 Currently supported features:
 
 - Reads a few values such as State of Charge, DCPV CT
 - Battery in and out energy
 - Gets and sets the current operating mode (normal/stopped/export)
 - Change priority of Libbi
 - Enable/Disable charging from the grid
 - Set charge target (in Wh)
 
-cli examples:
-```
+
+## CLI examples:
+
+```bash
 myenergi libbi show
 myenergi libbi mode normal
 myenergi libbi priority 1
 myenergi libbi energy
 myenergi libbi chargefromgrid false
 myenergi libbi chargetarget 10200
 ```
 
-
-
 ## Credits
 
 [twonk](https://github.com/twonk/MyEnergi-App-Api) for documenting the unofficial API
```

### Comparing `pymyenergi-0.1.1/pymyenergi/base_device.py` & `pymyenergi-0.2.0/pymyenergi/base_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             "ct4": 0,
             "ct5": 0,
             "ct6": 0,
             "ive1": 0,
             "ivi1": 0,
             "bdp1": 0,
             "bcp1": 0,
-            "pvp1": 0
+            "pvp1": 0,
         }
         if resolution == MINUTE:
             url = f"/cgi-jday-{self.prefix}{self._serialno}-{date_from.year}-{date_from.month}-{date_from.day}-{date_from.hour}-0-{how_long}"
         else:
             url = f"/cgi-jdayhour-{self.prefix}{self._serialno}-{date_from.year}-{date_from.month}-{date_from.day}-{date_from.hour}-{how_long}"
         _LOGGER.debug(f"Fetching {resolution} history data for {self.kind}")
         data = await self._connection.get(url)
@@ -165,19 +165,19 @@
 
         return_data = {
             "generated": round(energy_wh["gep"] / 1000, 2),
             "grid_import": round(energy_wh["imp"] / 1000, 2),
             "grid_export": round(energy_wh["exp"] / 1000, 2),
             "battery_charge": round(energy_wh["bcp1"] / 1000, 2),
             "battery_discharge": round(energy_wh["bdp1"] / 1000, 2),
-            "inverter_export": round(energy_wh["ive1"] /1000, 2),
-            "inverter_import": round(energy_wh["ivi1"] /1000, 2),
+            "inverter_export": round(energy_wh["ive1"] / 1000, 2),
+            "inverter_import": round(energy_wh["ivi1"] / 1000, 2),
             "device_boosted": device_boosted,
             "device_green": device_green,
-            "device_total": device_boosted + device_green
+            "device_total": device_boosted + device_green,
         }
         if resolution == MINUTE:
             return_data["pv_total"] = round(energy_wh["pvp1"] / 1000, 2)
 
         for i in range(6):
             key = f"ct{i+1}"
             if hasattr(self, key):
```

### Comparing `pymyenergi-0.1.1/pymyenergi/cli.py` & `pymyenergi-0.2.0/pymyenergi/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 
 from pymyenergi.client import device_factory
 from pymyenergi.client import MyenergiClient
 from pymyenergi.connection import Connection
 from pymyenergi.eddi import BOOST_TARGETS
 from pymyenergi.eddi import EDDI_MODES
 from pymyenergi.exceptions import WrongCredentials
-from pymyenergi.zappi import CHARGE_MODES
 from pymyenergi.libbi import LIBBI_MODES
+from pymyenergi.zappi import CHARGE_MODES
 
 from . import EDDI
 from . import HARVI
-from . import ZAPPI
 from . import LIBBI
+from . import ZAPPI
 
 logging.basicConfig()
 logging.root.setLevel(logging.WARNING)
 
 
 async def main(args):
     username = args.username or input("Please enter your hub serial number: ")
     password = args.password or getpass(prompt="Password (apikey): ")
-    app_email = args.app_email or input("App email (enter to skip; only needed for libbi): ")
-    if app_email:
-        app_password = args.app_password or getpass(prompt="App password: ")
+    if not args.skip_oauth:
+        app_email = args.app_email or input("App email (enter to skip; only needed for libbi): ")
+        if app_email:
+            app_password = args.app_password or getpass(prompt="App password: ")
+        else:
+            app_password = ""
     else:
-        app_password = ''
+        app_email = ""
+        app_password = ""
     conn = Connection(username, password, app_password, app_email)
     if app_email and app_password:
         await conn.discoverLocations()
     if args.debug:
         logging.root.setLevel(logging.DEBUG)
     client = MyenergiClient(conn)
     try:
@@ -191,14 +195,15 @@
     )
     parser.add_argument(
         "-e",
         "--app_email",
         dest="app_email",
         default=config.get("hub", "app_email").strip('"'),
     )
+    parser.add_argument("--skip-oauth", dest="skip_oauth", action="store_true", default=False)
     parser.add_argument("-d", "--debug", dest="debug", action="store_true")
     parser.add_argument("-j", "--json", dest="json", action="store_true", default=False)
     parser.add_argument("--version", dest="version", action="store_true", default=False)
     subparsers = parser.add_subparsers(dest="command", help="sub-command help")
     subparser_list = subparsers.add_parser("list", help="list devices")
     subparser_list.add_argument("-k", "--kind", dest="kind", default="all")
     subparsers.add_parser("overview", help="show overview")
```

### Comparing `pymyenergi-0.1.1/pymyenergi/client.py` & `pymyenergi-0.2.0/pymyenergi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from . import CT_GENERATION
 from . import CT_GRID
 from . import CT_LOAD
 from . import DEVICE_TYPES
 from . import EDDI
 from . import FREQUENCY_GRID
 from . import HARVI
-from . import LIBBI
 from . import HOUR
+from . import LIBBI
 from . import VOLTAGE_GRID
 from . import ZAPPI
 from .eddi import Eddi
 from .harvi import Harvi
 from .libbi import Libbi
 from .zappi import Zappi
 
@@ -79,15 +79,17 @@
         for device in devices:
             if device.kind == ZAPPI or device.kind == EDDI or device == LIBBI:
                 zappi_or_eddi_or_libbi = device
                 break
         if zappi_or_eddi_or_libbi is not None:
             for key in energy_keys:
                 if self._history_totals[key] == 0:
-                    self._history_totals[key] = zappi_or_eddi_or_libbi.history_data.get(key, 0)
+                    self._history_totals[key] = zappi_or_eddi_or_libbi.history_data.get(
+                        key, 0
+                    )
             self._history_totals["green"] = self._history_totals.get(
                 "green", 0
             ) + zappi_or_eddi_or_libbi.history_data.get("device_green", 0)
 
     def _calculate_totals(self):
         """Calculate current data totals"""
         devices = self.get_devices_sync()
@@ -129,15 +131,18 @@
                         )
 
         if zappi_or_eddi_or_libbi is not None:
             self._totals[FREQUENCY_GRID] = zappi_or_eddi_or_libbi.supply_frequency
             self._totals[VOLTAGE_GRID] = zappi_or_eddi_or_libbi.supply_voltage
         if self._totals.get(CT_GRID, 0) == 0 and zappi_or_eddi_or_libbi is not None:
             self._totals[CT_GRID] = zappi_or_eddi_or_libbi.power_grid
-        if self._totals.get(CT_GENERATION, 0) == 0 and zappi_or_eddi_or_libbi is not None:
+        if (
+            self._totals.get(CT_GENERATION, 0) == 0
+            and zappi_or_eddi_or_libbi is not None
+        ):
             self._totals[CT_GENERATION] = zappi_or_eddi_or_libbi.power_generated
 
     def get_power_totals(self):
         return self._totals
 
     @property
     def consumption_home(self):
@@ -210,26 +215,28 @@
         _LOGGER.debug("Refreshing data for all myenergi devices")
         data = await self.fetch_data()
         self._data = data["devices"]
         self._keys = data["keys"]
         for grp in self._data:
             keys = list(grp.keys())
             key = keys[0]
-            if(len(keys) > 1 and keys[1] == 'fwv'):
-                self._firmware_version = grp['fwv']
+            if len(keys) > 1 and keys[1] == "fwv":
+                self._firmware_version = grp["fwv"]
             if key not in DEVICE_TYPES:
                 if key == "fwv":
                     self._firmware_version = grp[key]
                 else:
                     _LOGGER.debug(f"Unknown device type: {key}")
                 continue
             devices = grp[key]
             for device_data in devices:
                 serial = device_data.get("sno")
-                self._update_available = device_data.get('newBootloaderAvailable', False)
+                self._update_available = device_data.get(
+                    "newBootloaderAvailable", False
+                )
                 existing_device = self.devices.get(serial, None)
                 if existing_device is None:
                     existing_device = device_factory(
                         self._connection, key, serial, device_data
                     )
                     serial_key = existing_device.prefix + str(
                         existing_device.serial_number
```

### Comparing `pymyenergi-0.1.1/pymyenergi/connection.py` & `pymyenergi-0.2.0/pymyenergi/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,48 +4,54 @@
 
 """
 import logging
 import sys
 from typing import Text
 
 import httpx
-
 from pycognito import Cognito
 
 from .exceptions import MyenergiException
 from .exceptions import TimeoutException
 from .exceptions import WrongCredentials
 
 _LOGGER = logging.getLogger(__name__)
-_USER_POOL_ID = 'eu-west-2_E57cCJB20'
-_CLIENT_ID = '2fup0dhufn5vurmprjkj599041'
+_USER_POOL_ID = "eu-west-2_E57cCJB20"
+_CLIENT_ID = "2fup0dhufn5vurmprjkj599041"
+
+
 
 class Connection:
     """Connection to myenergi API."""
 
     def __init__(
-        self, username: Text = None, password: Text = None, app_password: Text = None, app_email: Text = None, timeout: int = 20
+        self,
+        username: Text = None,
+        password: Text = None,
+        app_password: Text = None,
+        app_email: Text = None,
+        timeout: int = 20,
     ) -> None:
         """Initialize connection object."""
         self.timeout = timeout
         self.director_url = "https://director.myenergi.net"
         self.base_url = None
         self.oauth_base_url = "https://myaccount.myenergi.com"
         self.username = username
         self.password = password
         self.app_password = app_password
         self.app_email = app_email
         self.auth = httpx.DigestAuth(self.username, self.password)
         self.headers = {"User-Agent": "Wget/1.14 (linux-gnu)"}
-        if self.app_email and app_password:
+        if self.app_email and self.app_password:
             self.oauth = Cognito(_USER_POOL_ID, _CLIENT_ID, username=self.app_email)
             self.oauth.authenticate(password=self.app_password)
             self.oauth_headers = {"Authorization": f"Bearer {self.oauth.access_token}"}
         self.do_query_asn = True
-        self.invitation_id = ''
+        self.invitation_id = ""
         _LOGGER.debug("New connection created")
 
     def _checkMyenergiServerURL(self, responseHeader):
         if "X_MYENERGI-asn" in responseHeader:
             new_url = "https://" + responseHeader["X_MYENERGI-asn"]
             if new_url != self.base_url:
                 _LOGGER.info(f"Updated myenergi active server to {new_url}")
@@ -53,18 +59,19 @@
         else:
             _LOGGER.debug(
                 "Myenergi ASN not found in Myenergi header, assume auth failure (bad username)"
             )
             raise WrongCredentials()
 
     async def discoverLocations(self):
-        locs = await self.get("/api/Location", oauth=True)
-        # check if guest location - use the first location by default
-        if locs["content"][0]["isGuestLocation"] == True:
-            self.invitation_id = locs["content"][0]["invitationData"]["invitationId"]
+        if self.app_email and self.app_password:
+            locs = await self.get("/api/Location", oauth=True)
+            # check if guest location - use the first location by default
+            if locs["content"][0]["isGuestLocation"] == True:
+                self.invitation_id = locs["content"][0]["invitationData"]["invitationId"]
 
     def checkAndUpdateToken(self):
         # check if we have oauth credentials
         if self.app_email and self.app_password:
             # check if we have to renew out token
             self.oauth.check_token()
             self.oauth_headers = {"Authorization": f"Bearer {self.oauth.access_token}"}
@@ -75,16 +82,16 @@
             # check if we have oauth credentials
             if self.app_email and self.app_password:
                 async with httpx.AsyncClient(
                     headers=self.oauth_headers, timeout=self.timeout
                 ) as httpclient:
                     theUrl = self.oauth_base_url + url
                     # if we have an invitiation id, we need to add that to the query
-                    if (self.invitation_id != ""):
-                        if ("?" in theUrl):
+                    if self.invitation_id != "":
+                        if "?" in theUrl:
                             theUrl = theUrl + "&invitationId=" + self.invitation_id
                         else:
                             theUrl = theUrl + "?invitationId=" + self.invitation_id
                     try:
                         _LOGGER.debug(f"{method} {url} {theUrl}")
                         response = await httpclient.request(method, theUrl, json=json)
                     except httpx.ReadTimeout:
```

### Comparing `pymyenergi-0.1.1/pymyenergi/eddi.py` & `pymyenergi-0.2.0/pymyenergi/eddi.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             if ct.name_as_key == "ct_none":
                 continue
             keys[ct.name_as_key] = keys.get(ct.name_as_key, 0) + 1
         return keys
 
     @property
     def hsk(self):
-        """ Heatsink temperature """
+        """Heatsink temperature"""
         val = self._data.get("hsk", None)
         if val is not None:
             val = val / 10
         return val
 
     @property
     def l1_phase(self):
```

### Comparing `pymyenergi-0.1.1/pymyenergi/exceptions.py` & `pymyenergi-0.2.0/pymyenergi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymyenergi-0.1.1/pymyenergi/harvi.py` & `pymyenergi-0.2.0/pymyenergi/harvi.py`

 * *Files identical despite different names*

### Comparing `pymyenergi-0.1.1/pymyenergi/libbi.py` & `pymyenergi-0.2.0/pymyenergi/libbi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-import logging
-
 from pymyenergi.connection import Connection
 
 from . import LIBBI
 from .base_device import BaseDevice
 
-_LOGGER = logging.getLogger(__name__)
-
 STATES = {
     0: "Off",
     1: "On",
     2: "Battery Full",
     4: "Idle",
     5: "Charging",
     6: "Discharging",
@@ -23,17 +19,19 @@
     11: "Stopped",
     101: "Battery Empty",
     102: "Full",
     104: "Full",
     151: "FW Upgrade (ARM)",
     156: "FW Upgrade (DSP)",
     172: "BMS Charge Temperature Low",
+    176: "BMS Updating",
     234: "Calibration Charge",
     251: "FW Upgrade (DSP)",
     252: "FW Upgrade (ARM)",
+    253: "BMS Upgrading",
 }
 
 LIBBI_MODES = ["Stopped", "Normal", "Export"]
 LIBBI_MODE_CONFIG = {
     "Stopped": {"mode_int": 0, "mode_name": "STOP"},
     "Normal": {"mode_int": 1, "mode_name": "BALANCE"},
     "Export": {"mode_int": 5, "mode_name": "DRAIN"},
@@ -80,18 +78,14 @@
 
     @property
     def local_mode(self):
         """Get current known status"""
         return self._data.get("lmo", 1)
 
     @property
-    def prefix(self):
-        return "E"
-
-    @property
     def ct_keys(self):
         """Return CT key names that are not none"""
         keys = {}
         for i in range(6):
             ct = getattr(self, f"ct{i+1}")
             if ct.name_as_key == "ct_none":
                 continue
@@ -197,20 +191,26 @@
     def generated(self):
         """Solar generation from history data"""
         return self.history_data.get("generated", 0)
 
     @property
     def charge_from_grid(self):
         """Is charging from the grid enabled?"""
-        return self._extra_data.get("charge_from_grid")
+        if self._connection.app_email and self._connection.app_password:
+            return self._extra_data.get("charge_from_grid")
+        else:
+            return None
 
     @property
     def charge_target(self):
         """Libbi charge target"""
-        return self._extra_data.get("charge_target", 0) / 1000
+        if self._connection.app_email and self._connection.app_password:
+            return self._extra_data.get("charge_target", 0) / 1000
+        else:
+            return None
 
     @property
     def prefix(self):
         return "L"
 
     def get_mode_description(self, mode: str):
         """Get the mode name as returned by myenergi API. E.g. Normal mode is BALANCE"""
@@ -227,37 +227,43 @@
             f"/cgi-libbi-mode-{self.prefix}{self._serialno}-{mode_int}"
         )
         self._data["lmo"] = LIBBI_MODE_CONFIG[mode.capitalize()]["mode_name"]
         return True
 
     async def set_charge_from_grid(self, charge_from_grid: bool):
         """Set charge from grid"""
-        await self._connection.put(
-            f"/api/AccountAccess/LibbiMode?chargeFromGrid={charge_from_grid}&serialNo={self._serialno}",
-            oauth=True,
-        )
-        self._extra_data["charge_from_grid"] = charge_from_grid
-        return True
+        if self._connection.app_email and self._connection.app_password:
+            await self._connection.put(
+                f"/api/AccountAccess/LibbiMode?chargeFromGrid={charge_from_grid}&serialNo={self._serialno}",
+                oauth=True,
+            )
+            self._extra_data["charge_from_grid"] = charge_from_grid
+            return True
+        else:
+            return False
 
     async def set_priority(self, priority):
         """Set device priority"""
         await self._connection.get(
             f"/cgi-set-priority-{self.prefix}{self._serialno}-{int(priority)}"
         )
         self._data["pri"] = int(priority)
         return True
 
     async def set_charge_target(self, charge_target: float):
         """Set charge target"""
-        await self._connection.put(
-            f"/api/AccountAccess/{self._serialno}/TargetEnergy?targetEnergy={charge_target}",
-            oauth=True,
-        )
-        self._extra_data["charge_target"] = charge_target
-        return True
+        if self._connection.app_email and self._connection.app_password:
+            await self._connection.put(
+                f"/api/AccountAccess/{self._serialno}/TargetEnergy?targetEnergy={charge_target}",
+                oauth=True,
+            )
+            self._extra_data["charge_target"] = charge_target
+            return True
+        else:
+            return False
 
     def show(self, short_format=False):
         """Returns a string with all data in human readable format"""
         ret = ""
         name = ""
         if self.name:
             name = f" {self.name}"
@@ -271,19 +277,26 @@
         ret = ret + f"Inverter size: {self.inverter_size}kWh\n"
         ret = ret + f"State of Charge: {self.state_of_charge}%\n"
         ret = ret + f"Generating: {self.power_generated}W\n"
         ret = ret + f"Grid: {self.power_grid}W\n"
         ret = ret + f"Status: {self.status}\n"
         ret = ret + "Local Mode: " + self.get_mode_description(self.local_mode) + "\n"
         ret = ret + "Charge from Grid: "
-        if self.charge_from_grid:
-            ret = ret + "Enabled\n"
+        if self.charge_from_grid is not None:
+            if self.charge_from_grid:
+                ret = ret + "Enabled\n"
+            else:
+                ret = ret + "Disabled\n"
+        else:
+            ret = ret + f"<unavailable>\n"
+        ret = ret + f"Charge target: "
+        if self.charge_target is not None:
+            ret = ret + f"{self.charge_target}kWh\n"
         else:
-            ret = ret + "Disabled\n"
-        ret = ret + f"Charge target: {self.charge_target}kWh\n"
+            ret = ret + f"<unavailable>\n"
         ret = ret + f"CT 1 {self.ct1.name} {self.ct1.power}W phase {self.ct1.phase}\n"
         ret = ret + f"CT 2 {self.ct2.name} {self.ct2.power}W phase {self.ct2.phase}\n"
         ret = ret + f"CT 3 {self.ct3.name} {self.ct3.power}W phase {self.ct3.phase}\n"
         ret = ret + f"CT 4 {self.ct4.name} {self.ct4.power}W phase {self.ct4.phase}\n"
         ret = ret + f"CT 5 {self.ct5.name} {self.ct5.power}W phase {self.ct5.phase}\n"
         ret = ret + f"CT 6 {self.ct6.name} {self.ct6.power}W phase {self.ct6.phase}\n"
         for key in self.ct_keys:
```

### Comparing `pymyenergi-0.1.1/pymyenergi/zappi.py` & `pymyenergi-0.2.0/pymyenergi/zappi.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,44 @@
     "B1": "EV Connected",
     "B2": "Waiting for EV",
     "C1": "EV ready to charge",
     "C2": "Charging",
     "F": "Fault",
     "U": "",
 }
-SINGLE_PHASE = "SINGLE_PHASE"
+PHASES_STATES = {
+    "SINGLE_PHASE" : "1",
+    "THREE_PHASE" : "3",
+    "AUTO" : "auto",
+}
+PHASES_STRINGS = {
+    "1" : "SINGLE_PHASE",
+    "3" : "THREE_PHASE",
+    "auto" : "AUTO",
+}
+PHASE_SETTING = {
+    "1" : 0,
+    "3" : 1,
+    "auto" : 2,
+}
+
+
 
 class Zappi(BaseDevice):
     """Zappi Client for myenergi API."""
 
     def __init__(self, connection: Connection, serialno, data=None) -> None:
         self.history_data = {}
         self.boost_data = {}
         super().__init__(connection, serialno, data)
 
     async def refresh(self):
         """Refresh device data"""
         self.data = await self.fetch_data()
+        self.boost_data = await self.fetch_boost_data()
 
     async def fetch_boost_data(self):
         """Fetch data from myenergi"""
         response = await self._connection.get(
             f"/cgi-boost-time-{self.prefix}{self._serialno}"
         )
         data = response
@@ -245,19 +262,15 @@
 
     @property
     def zsl(self):
         return self._data.get("zsl")
 
     @property
     def num_phases(self):
-        phases = self._data.get("phaseSetting", 1)
-        if phases == SINGLE_PHASE:
-            return 1
-        else:
-            return 3
+        return PHASES_STATES.get(self._data.get("phaseSetting", "1"), "")
 
     @property
     def update_available(self):
         return self._data.get("newBootloaderAvailable", False)
 
     @property
     def rdc(self):
@@ -319,15 +332,15 @@
     async def stop_charge(self):
         """Stop charge"""
         await self._connection.get(f"/cgi-zappi-mode-Z{self._serialno}-4-0-0-0000")
         return True
 
     async def stop_boost(self):
         """Stop charge"""
-        await self._connection.get(f"/cgi-zappi-mode-Z{self._serialno}-2-0-0-0000")
+        await self._connection.get(f"/cgi-zappi-mode-Z{self._serialno}-0-2-0-0000")
         return True
 
     async def set_charge_mode(self, mode):
         """Set charge mode, one of Fast, Eco, Eco+ or Stopped"""
         mode_int = CHARGE_MODES.index(mode.capitalize())
         await self._connection.get(
             f"/cgi-zappi-mode-Z{self._serialno}-{mode_int}-0-0-0000"
@@ -339,14 +352,25 @@
     async def set_minimum_green_level(self, level):
         """Set minimum green level 0-100"""
         await self._connection.get(f"/cgi-set-min-green-Z{self._serialno}-{level}")
         # Set local data if successful
         self._data["mgl"] = level
         return True
 
+    async def set_phase_setting(self, phase):
+        """Set phase setting, can be set 1/3/auto"""
+        phasesetting_int = PHASE_SETTING.get(phase)
+        await self._connection.get(
+            f"/cgi-zappi-phase-setting-Z{self._serialno}-{phasesetting_int}"
+        )
+        # Set local data if successful
+        self._data["num_phases"] = PHASES_STRINGS.get(phase)
+        return True
+
+
     async def start_boost(self, amount):
         """Start boost"""
         if self.charge_mode not in ["Eco", "Eco+"]:
             return False
         await self._connection.get(
             f"/cgi-zappi-mode-Z{self._serialno}-0-10-{int(amount)}-0000"
         )
```

### Comparing `pymyenergi-0.1.1/pymyenergi.egg-info/PKG-INFO` & `pymyenergi-0.2.0/pymyenergi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymyenergi
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python library and CLI for communicating with myenergi API.
 Home-page: https://github.com/cjne/pymyenergi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,57 +13,67 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: pycognito
 
 # pymyenergi
 
-An async python library for myenergi API
+An async Python library for myenergi API
 
 This is a very early release, things are changing rapidly so use at your own risk!
 
-_NOTE:_ This work is not officially supported by myenergi and functionality can stop working at any time without warning
+> [!IMPORTANT]
+> This work is not officially supported by myenergi and functionality can stop working at any time without warning
 
 ## Installation
 
-The easiest method is to install using pip3/pip (venv is also a good idea)
+The easiest method is to install using pip (`pip`/`pip3`):
 
-```
+```bash
 pip install pymyenergi
 ```
 
-to update to the latest version
+Installing within a [Python virtual environment](https://docs.python.org/3/library/venv.html) is often a good idea:
 
+```bash
+python -m venv .venv
+source .venv/bin/activate
+pip install pymyenergi
 ```
+
+To update to the latest version:
+
+```bash
 pip install pymyenergi -U
 ```
 
-Setup will add a cli under the name myenergicli, see below for usage
+Setup will add a CLI under the name `myenergicli`. See below for usage.
 
 ## CLI
 
-A simple cli is provided with this library.
+A simple CLI is provided with this library.
 
-If no username, password, app_email or app_password is supplied as input arguments and no configuration file is found you will be prompted.
-Configuration file will be searched for in ./.myenergi.cfg and ~/.myenergi.cfg
+If no `username`, `password`, `app_email` or `app_password` is supplied as input arguments, and no configuration file is found, you will be prompted for credentials.
+
+Configuration file will be searched for in `./.myenergi.cfg` and `~/.myenergi.cfg`.
 
 ### Example configuration file
 
-```
+```ini
 [hub]
 serial=12345678
-password=yourpassword
+password=your-password
 app_email=myemail@email.com
-app_password=yourapppassword
+app_password=your-app-password
 ```
 
 ### CLI usage
 
 ```
-usage: myenergi [-h] [-u USERNAME] [-p PASSWORD] [-e APP_EMAIL] [-a APP_PASSWORD] [-d] [-j]
+usage: myenergi [-h] [-u USERNAME] [-p PASSWORD] [-e APP_EMAIL] [-a APP_PASSWORD] [-d] [-j] [--skip-oauth]
                 {list,overview,zappi,eddi,harvi,libbi} ...
 
 myenergi CLI.
 
 positional arguments:
   {list,overview,zappi,eddi,harvi,libbi}
                         sub-command help
@@ -82,112 +92,110 @@
   -a APP_PASSWORD, --app_password APP_PASSWORD
   -d, --debug
   -j, --json
 ```
 
 ## Library usage
 
-Install pymyenergi using pip (requires python > 3.6)
+Install pymyenergi using pip (requires Python > 3.6)
 
-### Example client usage
+### Example library usage
 
-```
+```python
 import asyncio
 from pymyenergi.connection import Connection
 from pymyenergi.client import MyenergiClient
 from sys import argv
 import logging
 
 logging.basicConfig()
 logging.root.setLevel(logging.INFO)
 
-user = argv[1]
-password = argv[2]
+user, password = argv
 
 async def zappis() -> None:
     conn = Connection(user, password)
     client = MyenergiClient(conn)
 
     zappis = await client.getDevices('zappi')
     for zappi in zappis:
         print(f"Zappi {zappi.serial_number} charge mode {zappi.charge_mode}")
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(zappis())
 ```
 
-### Example client usage - Zappi
+### Example library usage - Zappi
 
-```
+```python
 import asyncio
 from pymyenergi.connection import Connection
 from pymyenergi.zappi import Zappi
 from sys import argv
 import logging
 
 logging.basicConfig()
 logging.root.setLevel(logging.INFO)
 
-user = argv[1]
-password = argv[2]
-zappi_serial = argv[3]
+user, password, zappi_serial = argv
 
 
 async def get_data() -> None:
     conn = Connection(user, password)
     zappi = Zappi(conn, zappi_serial)
     await zappi.refresh()
     print(f"Zappi S/N {zappi.serial_number} version {zappi.firmware_version}")
     print(f"Status: {zappi.status} Plug status: {zappi.plug_status} Locked: {zappi.locked}")
     print(f"Priority: {zappi.priority}")
     print(f"Charge mode: {zappi.charge_mode} {zappi.num_phases} phase")
-    print("")
+    print()
     print(f"Lock when plugged in   : {zappi.lock_when_pluggedin}")
     print(f"Lock when unplugged    : {zappi.lock_when_unplugged}")
     print(f"Charge when locked     : {zappi.charge_when_locked}")
     print(f"Charge session allowed : {zappi.charge_session_allowed}")
     print(f"Charge added: {zappi.charge_added}")
-    print("")
+    print()
     print(f"CT 1 {zappi.ct1.name} {zappi.ct1.power}W")
     print(f"CT 2 {zappi.ct2.name} {zappi.ct2.power}W")
     print(f"CT 3 {zappi.ct3.name} {zappi.ct3.power}W")
     print(f"CT 4 {zappi.ct4.name} {zappi.ct4.power}W")
     print(f"CT 5 {zappi.ct5.name} {zappi.ct5.power}W")
     print(f"CT 6 {zappi.ct6.name} {zappi.ct6.power}W")
-    print("")
+    print()
     print(f"Supply voltage: {zappi.supply_voltage}V frequency: {zappi.supply_frequency}Hz")
     print("Power:")
     print(f"  Grid      : {zappi.power_grid}W")
     print(f"  Generated : {zappi.power_generated}W")
-    print("")
-    print(f"      Boost start at {zappi.boost_start_hour}:{zappi.boost_start_minute} add {zappi.boost_amount}kWh")
+    print()
+    # print(f"      Boost start at {zappi.boost_start_hour}:{zappi.boost_start_minute} add {zappi.boost_amount}kWh")
     print(f"Smart Boost start at {zappi.smart_boost_start_hour}:{zappi.smart_boost_start_minute} add {zappi.smart_boost_amount}kWh")
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(get_data())
 ```
 
 ## Libbi support
+
 Currently supported features:
 
 - Reads a few values such as State of Charge, DCPV CT
 - Battery in and out energy
 - Gets and sets the current operating mode (normal/stopped/export)
 - Change priority of Libbi
 - Enable/Disable charging from the grid
 - Set charge target (in Wh)
 
-cli examples:
-```
+
+## CLI examples:
+
+```bash
 myenergi libbi show
 myenergi libbi mode normal
 myenergi libbi priority 1
 myenergi libbi energy
 myenergi libbi chargefromgrid false
 myenergi libbi chargetarget 10200
 ```
 
-
-
 ## Credits
 
 [twonk](https://github.com/twonk/MyEnergi-App-Api) for documenting the unofficial API
```

### Comparing `pymyenergi-0.1.1/pymyenergi.egg-info/SOURCES.txt` & `pymyenergi-0.2.0/pymyenergi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymyenergi-0.1.1/setup.py` & `pymyenergi-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 setup(
     name="pymyenergi",
     version=version,
     author="Johan Isaksson",
     author_email="johan@generatorhallen.se",
     description="Python library and CLI for communicating with myenergi API.",
-    long_description=open("README.md", 'r').read(),
-    long_description_content_type='text/markdown',
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
     package_data={"pymyenergi": ["VERSION"]},
     include_package_data=True,
     url="https://github.com/cjne/pymyenergi",
     license="MIT",
     packages=["pymyenergi"],
     python_requires=">=3.6",
     install_requires=["httpx", "pycognito"],
```

### Comparing `pymyenergi-0.1.1/tests/test_client.py` & `pymyenergi-0.2.0/tests/test_client.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from pymyenergi.client import MyenergiClient
 from pymyenergi.eddi import Eddi
 from pymyenergi.harvi import Harvi
-from pymyenergi.zappi import Zappi
 from pymyenergi.libbi import Libbi
+from pymyenergi.zappi import Zappi
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 conn = {}
 
 
@@ -65,8 +65,8 @@
     assert client.consumption_home == 16000
 
 
 async def test_get_libbi_devices(client_fetch_data_fixture):
     client = MyenergiClient(conn)
     devices = await client.get_devices("libbi")
     assert len(devices) == 1
-    assert isinstance(devices[0], Libbi)
+    assert isinstance(devices[0], Libbi)
```

### Comparing `pymyenergi-0.1.1/tests/test_eddi.py` & `pymyenergi-0.2.0/tests/test_eddi.py`

 * *Files identical despite different names*

