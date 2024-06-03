# Comparing `tmp/ipv4v6-1.0.0.tar.gz` & `tmp/ipv4v6-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipv4v6-1.0.0.tar", last modified: Sat Jun  1 12:52:24 2024, max compression
+gzip compressed data, was "ipv4v6-1.0.1.tar", last modified: Mon Jun  3 11:04:57 2024, max compression
```

## Comparing `ipv4v6-1.0.0.tar` & `ipv4v6-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 12:52:24.530671 ipv4v6-1.0.0/
--rw-rw-rw-   0        0        0     1090 2024-06-01 08:12:14.000000 ipv4v6-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3227 2024-06-01 12:52:24.528143 ipv4v6-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2518 2024-06-01 12:50:07.000000 ipv4v6-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 12:52:24.516112 ipv4v6-1.0.0/ipv4v6/
--rw-rw-rw-   0        0        0       20 2024-06-01 08:56:19.000000 ipv4v6-1.0.0/ipv4v6/__init__.py
--rw-rw-rw-   0        0        0     2362 2024-06-01 09:16:51.000000 ipv4v6-1.0.0/ipv4v6/_core.py
-drwxrwxrwx   0        0        0        0 2024-06-01 12:52:24.526147 ipv4v6-1.0.0/ipv4v6.egg-info/
--rw-rw-rw-   0        0        0     3227 2024-06-01 12:52:24.000000 ipv4v6-1.0.0/ipv4v6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-06-01 12:52:24.000000 ipv4v6-1.0.0/ipv4v6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 12:52:24.000000 ipv4v6-1.0.0/ipv4v6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 12:52:24.000000 ipv4v6-1.0.0/ipv4v6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 12:52:24.530671 ipv4v6-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1067 2024-06-01 12:52:05.000000 ipv4v6-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:04:57.568646 ipv4v6-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2024-06-01 08:12:14.000000 ipv4v6-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1937 2024-06-03 11:04:57.565646 ipv4v6-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-06-03 11:04:25.000000 ipv4v6-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 11:04:57.547372 ipv4v6-1.0.1/ipv4v6/
+-rw-rw-rw-   0        0        0       20 2024-06-01 08:56:19.000000 ipv4v6-1.0.1/ipv4v6/__init__.py
+-rw-rw-rw-   0        0        0     2362 2024-06-01 09:16:51.000000 ipv4v6-1.0.1/ipv4v6/_core.py
+drwxrwxrwx   0        0        0        0 2024-06-03 11:04:57.563634 ipv4v6-1.0.1/ipv4v6.egg-info/
+-rw-rw-rw-   0        0        0     1937 2024-06-03 11:04:56.000000 ipv4v6-1.0.1/ipv4v6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-06-03 11:04:57.000000 ipv4v6-1.0.1/ipv4v6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 11:04:56.000000 ipv4v6-1.0.1/ipv4v6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-03 11:04:56.000000 ipv4v6-1.0.1/ipv4v6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 11:04:57.568646 ipv4v6-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2024-06-03 11:04:45.000000 ipv4v6-1.0.1/setup.py
```

### Comparing `ipv4v6-1.0.0/LICENSE` & `ipv4v6-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipv4v6-1.0.0/PKG-INFO` & `ipv4v6-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipv4v6
-Version: 1.0.0
+Version: 1.0.1
 Summary: A model for get ipv4&ipv6 address
 Home-page: https://github.com/myhldh/GetIP
 Author: OscarMYH(myhldh)
 Author-email: oscarmyh@163.com
 License: MIT
 Keywords: python,computer vision,OscarMYH,myhldh,lightweight,windows,mac,linux
 Classifier: Development Status :: 1 - Planning
@@ -30,45 +30,14 @@
 	```
 
   **(Tips : If you just want to get ipv4 address, *get_ip()* is a better choice because it's faster than *get_ipv4*)**
  * Function *get_ipv6()* is used to get your ipv6 address including only host.
 	 ```
 	 from ipv4v6 import get_ipv6
 	 print(get_ipv6())
-	 #It'll print something like 2409:8a1e:6e81:4280:6456:3051:4f3f:1965
-	 ```
- * Function *ip_tuple()* returns a tuple which contains the host and the port of your ipv4 address.
-   **(Tips : It can be given to *socket.connect()* as parameter)**
-   ```
-   from socket import *
-   from ipv4v6 import ip_tuple
-   sock=socket(AF_INET,SOCK_STREAM)
-   sock.connect(ip_tuple())
-   ```
-* Function *get_ipv4_location()* and *get_ipv6_location* returns the location of your ip address. 
-   ```
-   from ipv4v6 import get_ipv4_location
-   print(get_ipv4_location()) #It'll print the location
-   ```# Thank you for supporting!
-* Function *get_ip()* is used to get your ipv4 address including host and port.
-	```
-	from ipv4v6 import get_ip
-	print(get_ip()) #it'll print something like 117.143.170.80:2653
-	```
-* Function *get_ipv4()* is used to get your ipv4 address including only host.
-	```
-	from ipv4v6 import get_ipv4
-	print(get_ipv4()) #it'll print something like 117.143.170.80
-	```
-
-  **(Tips : If you just want to get ipv4 address, *get_ip()* is a better choice because it's faster than *get_ipv4*)**
- * Function *get_ipv6()* is used to get your ipv6 address including only host.
-	 ```
-	 from ipv4v6 import get_ipv6
-	 print(get_ipv6())
 	 #It'll print something like 2409:8a1e:6e81:4280:6456:3051:4f3f:1965
 	 ```
  * Function *ip_tuple()* returns a tuple which contains the host and the port of your ipv4 address.
    **(Tips : It can be given to *socket.connect()* as parameter)**
    ```
    from socket import *
    from ipv4v6 import ip_tuple
```

### Comparing `ipv4v6-1.0.0/README.md` & `ipv4v6-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,39 +25,8 @@
    sock=socket(AF_INET,SOCK_STREAM)
    sock.connect(ip_tuple())
    ```
 * Function *get_ipv4_location()* and *get_ipv6_location* returns the location of your ip address. 
    ```
    from ipv4v6 import get_ipv4_location
    print(get_ipv4_location()) #It'll print the location
-   ```# Thank you for supporting!
-* Function *get_ip()* is used to get your ipv4 address including host and port.
-	```
-	from ipv4v6 import get_ip
-	print(get_ip()) #it'll print something like 117.143.170.80:2653
-	```
-* Function *get_ipv4()* is used to get your ipv4 address including only host.
-	```
-	from ipv4v6 import get_ipv4
-	print(get_ipv4()) #it'll print something like 117.143.170.80
-	```
-
-  **(Tips : If you just want to get ipv4 address, *get_ip()* is a better choice because it's faster than *get_ipv4*)**
- * Function *get_ipv6()* is used to get your ipv6 address including only host.
-	 ```
-	 from ipv4v6 import get_ipv6
-	 print(get_ipv6())
-	 #It'll print something like 2409:8a1e:6e81:4280:6456:3051:4f3f:1965
-	 ```
- * Function *ip_tuple()* returns a tuple which contains the host and the port of your ipv4 address.
-   **(Tips : It can be given to *socket.connect()* as parameter)**
-   ```
-   from socket import *
-   from ipv4v6 import ip_tuple
-   sock=socket(AF_INET,SOCK_STREAM)
-   sock.connect(ip_tuple())
-   ```
-* Function *get_ipv4_location()* and *get_ipv6_location* returns the location of your ip address. 
-   ```
-   from ipv4v6 import get_ipv4_location
-   print(get_ipv4_location()) #It'll print the location
    ```
```

### Comparing `ipv4v6-1.0.0/ipv4v6/_core.py` & `ipv4v6-1.0.1/ipv4v6/_core.py`

 * *Files identical despite different names*

### Comparing `ipv4v6-1.0.0/ipv4v6.egg-info/PKG-INFO` & `ipv4v6-1.0.1/ipv4v6.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipv4v6
-Version: 1.0.0
+Version: 1.0.1
 Summary: A model for get ipv4&ipv6 address
 Home-page: https://github.com/myhldh/GetIP
 Author: OscarMYH(myhldh)
 Author-email: oscarmyh@163.com
 License: MIT
 Keywords: python,computer vision,OscarMYH,myhldh,lightweight,windows,mac,linux
 Classifier: Development Status :: 1 - Planning
@@ -30,45 +30,14 @@
 	```
 
   **(Tips : If you just want to get ipv4 address, *get_ip()* is a better choice because it's faster than *get_ipv4*)**
  * Function *get_ipv6()* is used to get your ipv6 address including only host.
 	 ```
 	 from ipv4v6 import get_ipv6
 	 print(get_ipv6())
-	 #It'll print something like 2409:8a1e:6e81:4280:6456:3051:4f3f:1965
-	 ```
- * Function *ip_tuple()* returns a tuple which contains the host and the port of your ipv4 address.
-   **(Tips : It can be given to *socket.connect()* as parameter)**
-   ```
-   from socket import *
-   from ipv4v6 import ip_tuple
-   sock=socket(AF_INET,SOCK_STREAM)
-   sock.connect(ip_tuple())
-   ```
-* Function *get_ipv4_location()* and *get_ipv6_location* returns the location of your ip address. 
-   ```
-   from ipv4v6 import get_ipv4_location
-   print(get_ipv4_location()) #It'll print the location
-   ```# Thank you for supporting!
-* Function *get_ip()* is used to get your ipv4 address including host and port.
-	```
-	from ipv4v6 import get_ip
-	print(get_ip()) #it'll print something like 117.143.170.80:2653
-	```
-* Function *get_ipv4()* is used to get your ipv4 address including only host.
-	```
-	from ipv4v6 import get_ipv4
-	print(get_ipv4()) #it'll print something like 117.143.170.80
-	```
-
-  **(Tips : If you just want to get ipv4 address, *get_ip()* is a better choice because it's faster than *get_ipv4*)**
- * Function *get_ipv6()* is used to get your ipv6 address including only host.
-	 ```
-	 from ipv4v6 import get_ipv6
-	 print(get_ipv6())
 	 #It'll print something like 2409:8a1e:6e81:4280:6456:3051:4f3f:1965
 	 ```
  * Function *ip_tuple()* returns a tuple which contains the host and the port of your ipv4 address.
    **(Tips : It can be given to *socket.connect()* as parameter)**
    ```
    from socket import *
    from ipv4v6 import ip_tuple
```

### Comparing `ipv4v6-1.0.0/setup.py` & `ipv4v6-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 here=os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here,"README.md"),encoding="utf-8") as fh:
     long_description="\n"+fh.read()
-VERSION='1.0.0'
+VERSION='1.0.1'
 DESCRIPTION='A model for get ipv4&ipv6 address'
 setup(
     name="ipv4v6",
     version=VERSION,
     author="OscarMYH(myhldh)",
     author_email='oscarmyh@163.com',
     url='https://github.com/myhldh/GetIP',
```

