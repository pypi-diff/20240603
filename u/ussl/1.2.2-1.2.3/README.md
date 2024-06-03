# Comparing `tmp/ussl-1.2.2.tar.gz` & `tmp/ussl-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ussl-1.2.2.tar", last modified: Fri May 31 09:34:45 2024, max compression
+gzip compressed data, was "dist\ussl-1.2.3.tar", last modified: Mon Jun  3 10:24:42 2024, max compression
```

## Comparing `ussl-1.2.2.tar` & `ussl-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.290774 ussl-1.2.2/
--rw-rw-rw-   0        0        0    12117 2024-05-31 09:34:45.286154 ussl-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    11465 2024-05-31 09:32:58.000000 ussl-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 09:34:45.290774 ussl-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2233 2024-05-31 09:34:43.000000 ussl-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.239961 ussl-1.2.2/ussl/
--rw-rw-rw-   0        0        0      133 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.258977 ussl-1.2.2/ussl/exceptions/
--rw-rw-rw-   0        0        0      305 2024-05-29 08:59:11.000000 ussl-1.2.2/ussl/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1369 2024-05-22 08:57:11.000000 ussl-1.2.2/ussl/exceptions/main.py
--rw-rw-rw-   0        0        0     1126 2024-05-29 09:16:44.000000 ussl-1.2.2/ussl/exceptions/protocol_exc.py
--rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.2.2/ussl/exceptions/validation_exc.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.261976 ussl-1.2.2/ussl/model/
--rw-rw-rw-   0        0        0     4405 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.266344 ussl-1.2.2/ussl/postprocessing/
--rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.2.2/ussl/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     7341 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/postprocessing/base.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.280865 ussl-1.2.2/ussl/protocol/
--rw-rw-rw-   0        0        0      798 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/__init__.py
--rw-rw-rw-   0        0        0      711 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/base.py
--rw-rw-rw-   0        0        0     1534 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/ldap.py
--rw-rw-rw-   0        0        0     4617 2024-05-31 09:34:43.000000 ussl-1.2.2/ussl/protocol/ssh.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.2.2/ussl/protocol/winexe.py
--rw-rw-rw-   0        0        0     8202 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/winrm.py
--rw-rw-rw-   0        0        0      303 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/wmi.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.283139 ussl-1.2.2/ussl/transport/
--rw-rw-rw-   0        0        0     1508 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.284139 ussl-1.2.2/ussl/utils/
--rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.2.2/ussl/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.249733 ussl-1.2.2/ussl.egg-info/
--rw-rw-rw-   0        0        0    12117 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.493909 ussl-1.2.3/
+-rw-rw-rw-   0        0        0    12117 2024-06-03 10:24:42.490799 ussl-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11465 2024-06-03 10:05:23.000000 ussl-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 10:24:42.493909 ussl-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2233 2024-06-03 10:24:39.000000 ussl-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.430807 ussl-1.2.3/ussl/
+-rw-rw-rw-   0        0        0      133 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.455112 ussl-1.2.3/ussl/exceptions/
+-rw-rw-rw-   0        0        0      305 2024-05-29 08:59:11.000000 ussl-1.2.3/ussl/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1369 2024-05-31 10:42:58.000000 ussl-1.2.3/ussl/exceptions/main.py
+-rw-rw-rw-   0        0        0     1126 2024-05-29 09:16:44.000000 ussl-1.2.3/ussl/exceptions/protocol_exc.py
+-rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.2.3/ussl/exceptions/validation_exc.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.458166 ussl-1.2.3/ussl/model/
+-rw-rw-rw-   0        0        0     4405 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.462973 ussl-1.2.3/ussl/postprocessing/
+-rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.2.3/ussl/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     7341 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/postprocessing/base.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.479134 ussl-1.2.3/ussl/protocol/
+-rw-rw-rw-   0        0        0      798 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/protocol/__init__.py
+-rw-rw-rw-   0        0        0      711 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/protocol/base.py
+-rw-rw-rw-   0        0        0     1534 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/protocol/ldap.py
+-rw-rw-rw-   0        0        0     4617 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/protocol/ssh.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.2.3/ussl/protocol/winexe.py
+-rw-rw-rw-   0        0        0     8268 2024-06-03 10:24:39.000000 ussl-1.2.3/ussl/protocol/winrm.py
+-rw-rw-rw-   0        0        0      303 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/protocol/wmi.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.482437 ussl-1.2.3/ussl/transport/
+-rw-rw-rw-   0        0        0     1508 2024-06-03 10:05:23.000000 ussl-1.2.3/ussl/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.485657 ussl-1.2.3/ussl/utils/
+-rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.2.3/ussl/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:24:42.444568 ussl-1.2.3/ussl.egg-info/
+-rw-rw-rw-   0        0        0    12117 2024-06-03 10:24:42.000000 ussl-1.2.3/ussl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2024-06-03 10:24:42.000000 ussl-1.2.3/ussl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:24:42.000000 ussl-1.2.3/ussl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-06-03 10:24:42.000000 ussl-1.2.3/ussl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-03 10:24:42.000000 ussl-1.2.3/ussl.egg-info/top_level.txt
```

### Comparing `ussl-1.2.2/PKG-INFO` & `ussl-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.2.2
+Version: 1.2.3
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `ussl-1.2.2/README.md` & `ussl-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/setup.py` & `ussl-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 setup(
     name='ussl',
     author='ussc soc dev team',
     author_email='iushangaraev@ussc.ru, pbikkuzhina@ussc.ru',
     description='Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.2',
+    version='1.2.3',
     python_requires='>=3.8.0',
     packages=[
         'ussl',
         'ussl.model',
         'ussl.postprocessing',
         'ussl.protocol',
         'ussl.transport',
```

### Comparing `ussl-1.2.2/ussl/exceptions/main.py` & `ussl-1.2.3/ussl/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/exceptions/protocol_exc.py` & `ussl-1.2.3/ussl/exceptions/protocol_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/exceptions/validation_exc.py` & `ussl-1.2.3/ussl/exceptions/validation_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/model/__init__.py` & `ussl-1.2.3/ussl/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/postprocessing/base.py` & `ussl-1.2.3/ussl/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/protocol/__init__.py` & `ussl-1.2.3/ussl/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/protocol/base.py` & `ussl-1.2.3/ussl/protocol/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/protocol/ldap.py` & `ussl-1.2.3/ussl/protocol/ldap.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/protocol/ssh.py` & `ussl-1.2.3/ussl/protocol/ssh.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/protocol/winrm.py` & `ussl-1.2.3/ussl/protocol/winrm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, Optional, Tuple
 
 import winrm.exceptions
-from requests.exceptions import ReadTimeout, ConnectTimeout
+from requests.exceptions import ReadTimeout, ConnectTimeout, ConnectionError as RequestsConnectionError
 from ussl.exceptions import SOARException
 from winrm import Session
 from winrm.exceptions import (
     AuthenticationError,
     WinRMError,
     WinRMOperationTimeoutError,
     WinRMTransportError,
@@ -25,15 +25,14 @@
     Для управления задержками используется READ_TIMEOUT, OPERATION_TIMEOUT и IDLE_TIMEOUT.
     """
     name = 'winrm'
     WINRM_PORT = 5985
     WINRM_SSL_PORT = 5986
     READ_TIMEOUT = 5
     OPERATION_TIMEOUT = 2
-    IDLE_TIMEOUT = 1
     VALID_TRANSPORT = {'plaintext', 'ntlm'}
 
     def __init__(self, protocol: Optional[Protocol] = None) -> None:
         super().__init__(protocol)
         self._session: Union[Session, None] = None
 
     def connect(self) -> None:
@@ -73,42 +72,41 @@
             raise ConnectionFailed(status)
 
         try:
             self.execute(Query(command=f'mode con:cols={window_width}', timeout=10))
         except Exception as e:
             raise ExecutionError(e)
 
-    def _try_connect(self,
-                     host: str,
+    def _try_connect(self, host: str,
                      credentials: Tuple[str, str],
                      transport: str,
                      scheme: str = None,
                      path: str = 'wsman') -> Tuple[Optional[Session], str]:
         if scheme is not None:
             try:
                 session = self._create_health_check_session(host,
                                                             credentials,
                                                             transport,
                                                             scheme,
                                                             path)
                 return session, ""
-            except ConnectTimeout:
+            except (ConnectTimeout, ConnectionError, RequestsConnectionError):
                 return None, 'Timeout'
             except WinRMError as e:
                 return None, str(e)
         result = ""
         for scheme in ('http', 'https'):
             try:
                 session = self._create_health_check_session(host,
                                                             credentials,
                                                             transport,
                                                             scheme,
                                                             path)
                 return session, ""
-            except ConnectTimeout:
+            except (ConnectTimeout, ConnectionError, RequestsConnectionError):
                 pass
             except winrm.exceptions.WinRMError as e:
                 result += str(e)
         return None, result if result else 'Timeout'
 
     def _create_health_check_session(self,
                                      host: str,
@@ -120,19 +118,19 @@
         session = Session(f'{scheme}://{host}:{port}/{path}',
                           auth=credentials,
                           server_cert_validation='ignore',
                           transport=transport,
                           read_timeout_sec=self.READ_TIMEOUT,
                           operation_timeout_sec=self.OPERATION_TIMEOUT)
         # Проверка соединения с удаленным хостом
-        session.protocol.open_shell(idle_timeout=self.IDLE_TIMEOUT)
+        session.protocol.open_shell()
         return session
 
     def close(self) -> None:
-        # Закрытие сессии не требуется. После выполнения запросов сессия сама вызывает protocol.close_shell()
+        # Закрытие сессии не требуется. После выполнения запросов сессия сама вызывает session.protocol.close_shell()
         self._session = None
 
     def execute(
             self,
             query: Union[Query, str]
     ) -> Response:
         if isinstance(query, str):
```

### Comparing `ussl-1.2.2/ussl/transport/__init__.py` & `ussl-1.2.3/ussl/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl/utils/__init__.py` & `ussl-1.2.3/ussl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.2/ussl.egg-info/PKG-INFO` & `ussl-1.2.3/ussl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.2.2
+Version: 1.2.3
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `ussl-1.2.2/ussl.egg-info/SOURCES.txt` & `ussl-1.2.3/ussl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

