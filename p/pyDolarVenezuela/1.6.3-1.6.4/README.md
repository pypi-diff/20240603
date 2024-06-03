# Comparing `tmp/pydolarvenezuela-1.6.3.tar.gz` & `tmp/pydolarvenezuela-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.6.3.tar", last modified: Sat Jun  1 19:12:24 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.6.4.tar", last modified: Mon Jun  3 04:18:29 2024, max compression
```

## Comparing `pydolarvenezuela-1.6.3.tar` & `pydolarvenezuela-1.6.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 19:12:24.504247 pydolarvenezuela-1.6.3/
--rw-rw-rw-   0        0        0    11547 2024-05-26 02:00:20.000000 pydolarvenezuela-1.6.3/LICENSE
--rw-rw-rw-   0        0        0    19254 2024-06-01 19:12:24.496248 pydolarvenezuela-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     4970 2024-06-01 18:11:34.000000 pydolarvenezuela-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 19:12:24.302253 pydolarvenezuela-1.6.3/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2285 2024-06-01 18:18:48.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 19:12:24.352248 pydolarvenezuela-1.6.3/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-06-01 19:12:24.416248 pydolarvenezuela-1.6.3/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/models/images.py
--rw-rw-rw-   0        0        0      770 2024-05-30 04:34:11.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/models/monitor.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0     1708 2024-06-01 18:19:28.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      860 2024-05-30 03:24:32.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-06-01 19:12:24.472250 pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     6768 2024-06-01 19:02:33.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2689 2024-05-30 04:30:30.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/alcambio.py
--rw-rw-rw-   0        0        0     2335 2024-05-25 22:27:08.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2088 2024-05-25 17:55:45.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2648 2024-05-30 03:43:00.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1289 2024-05-25 17:56:00.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-06-01 19:12:24.489250 pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/calculator.py
--rw-rw-rw-   0        0        0    12770 2024-05-30 04:23:51.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/extras.py
--rw-rw-rw-   0        0        0     2457 2024-05-30 03:31:36.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/time.py
--rw-rw-rw-   0        0        0      824 2024-06-01 19:11:25.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela/version.py
-drwxrwxrwx   0        0        0        0 2024-06-01 19:12:24.492246 pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0    19254 2024-06-01 19:12:24.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2024-06-01 19:12:24.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 19:12:24.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-06-01 19:12:24.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-06-01 19:12:24.000000 pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-06-01 19:11:36.000000 pydolarvenezuela-1.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 19:12:24.505247 pydolarvenezuela-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-06-01 19:11:33.000000 pydolarvenezuela-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:18:29.958292 pydolarvenezuela-1.6.4/
+-rw-rw-rw-   0        0        0    11547 2024-05-26 02:00:20.000000 pydolarvenezuela-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0    19372 2024-06-03 04:18:29.911417 pydolarvenezuela-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4970 2024-06-01 18:11:34.000000 pydolarvenezuela-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 04:18:29.723911 pydolarvenezuela-1.6.4/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2285 2024-06-01 18:18:48.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:18:29.786417 pydolarvenezuela-1.6.4/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:18:29.817662 pydolarvenezuela-1.6.4/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      301 2024-05-19 05:41:42.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/models/images.py
+-rw-rw-rw-   0        0        0      770 2024-05-30 04:34:11.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/models/monitor.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0     1708 2024-06-01 18:19:28.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      860 2024-05-30 03:24:32.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:18:29.864538 pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     6840 2024-06-03 03:42:23.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2689 2024-05-30 04:30:30.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/alcambio.py
+-rw-rw-rw-   0        0        0     2335 2024-05-25 22:27:08.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2088 2024-05-25 17:55:45.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2648 2024-05-30 03:43:00.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1289 2024-05-25 17:56:00.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:18:29.895787 pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/calculator.py
+-rw-rw-rw-   0        0        0    12994 2024-06-02 04:04:29.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/extras.py
+-rw-rw-rw-   0        0        0     2457 2024-05-30 03:31:36.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/time.py
+-rw-rw-rw-   0        0        0      824 2024-06-03 04:02:42.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela/version.py
+drwxrwxrwx   0        0        0        0 2024-06-03 04:18:29.911417 pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0    19372 2024-06-03 04:18:29.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2024-06-03 04:18:29.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 04:18:29.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-06-03 04:18:29.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-06-03 04:18:29.000000 pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1206 2024-06-03 04:17:11.000000 pydolarvenezuela-1.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-03 04:18:29.958292 pydolarvenezuela-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1518 2024-06-03 04:17:25.000000 pydolarvenezuela-1.6.4/setup.py
```

### Comparing `pydolarvenezuela-1.6.3/LICENSE` & `pydolarvenezuela-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/PKG-INFO` & `pydolarvenezuela-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.6.3
+Version: 1.6.4
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -206,16 +206,18 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/fcoagz/pydolarvenezuela
 Project-URL: Bug Tracker, https://github.com/fcoagz/pydolarvenezuela/issues
 Keywords: dolarmonitor,dolartoday,enparalelovzla,bcv,venezuela,dolarparalelo,dolarcambio,dolarvenezuela,dolartodayvenezuela,dolaroficial,dolarlibre,dolarinformal,dolarparalelovzla,dolarbcv,dolarenvenezuela
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: curl_cffi
 Requires-Dist: beautifulsoup4
```

### Comparing `pydolarvenezuela-1.6.3/README.md` & `pydolarvenezuela-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/models/monitor.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/models/monitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/network.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/network.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 if property not in ('banks', 'last_update'):
                     try:
                         self._update_item(old_data, values, property)
                     except KeyError:
                         pass
                 elif property == 'banks': # Comparación de propiedades de los datos BCV
                     banks = values[property]
-                    for i, _ in enumerate(banks):
+                    for i in range(len(banks)):
                         self._update_item(old_data[property], banks, i)
                 elif property == 'last_update':
                     old_data[property] = values[property]
 
             self._redis.set_data(key, json.dumps(old_data), self.db.ttl)
             values = json.loads(self._redis.get_data(key))
             
@@ -111,27 +111,27 @@
             percent: Optional[float] = 0.0
             change: Optional[float] = 0.0  
             color: Optional[str] = "neutral" 
             symbol: Optional[str] = "" 
         ```
         """
         
-        if isinstance(i, str) or isinstance(i, int) and i < len(old_data):
+        if isinstance(i, str) or (isinstance(i, int) and i <= len(old_data) - 1):
             structure_monitor = asdict(Monitor(**old_data[i]))
             for key in list(structure_monitor.keys()):
                 if structure_monitor[key] is None:
                     del structure_monitor[key]
             old_data[i] = structure_monitor
 
         # Ambos consultan si el precio es diferente para realizar cambios.
         # Hay diferentes datos que se distribuyeron como list, {str: dict}.
         if isinstance(i, int): # Actualiza los datos de 'old_data' con los datos de 'new_data' basándose en el título del item.
             title_items = [item['title'] for item in old_data]
             if new_data[i]['title'] in title_items:
-                index_old_data = title_items.index(new_data[i]['title'])
+                index_old_data = title_items.index(new_data[i]['title']) # Encuentra la posición donde se almacena el elemento en la lista
                 if old_data[index_old_data]['price'] != new_data[i]['price']:
                     self._update_price(old_data, new_data, index_old_data)
             else:
                 old_data.append(new_data[i])
         else: # Actualiza los datos de 'old_data' con los datos de 'new_data' basándose en el key del item.
             if i in old_data: 
                 if old_data[i]['price'] != new_data[i]['price']:
```

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/alcambio.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/alcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/provider/italcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/calculator.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/extras.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,19 @@
     },
     {
         "title": "monitor_dolar_vzla",
         "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1716093852/exchangemonitor/qwydse1rhwqyzh4vzmyj.webp",
         "provider": "exchangemonitor"
     },
     {
+        "title": "monitor_dolar_venezuela",
+        "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1716093852/exchangemonitor/kih3nvrygbratbtzvvew.webp",
+        "provider": "exchangemonitor"
+    },
+    {
         "title": "monitor_dolar",
         "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1716093852/exchangemonitor/kih3nvrygbratbtzvvew.webp",
         "provider": "exchangemonitor"
     },
     {
         "title": "enparalelovzla",
         "image": "https://res.cloudinary.com/dcpyfqx87/image/upload/v1716093852/exchangemonitor/kih3nvrygbratbtzvvew.webp",
```

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/utils/time.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/utils/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela/version.py` & `pydolarvenezuela-1.6.4/pyDolarVenezuela/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from colorama import Fore
 from . import network
 
-__version__ = '1.6.3'
+__version__ = '1.6.4'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca
```

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.6.3
+Version: 1.6.4
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -206,16 +206,18 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/fcoagz/pydolarvenezuela
 Project-URL: Bug Tracker, https://github.com/fcoagz/pydolarvenezuela/issues
 Keywords: dolarmonitor,dolartoday,enparalelovzla,bcv,venezuela,dolarparalelo,dolarcambio,dolarvenezuela,dolartodayvenezuela,dolaroficial,dolarlibre,dolarinformal,dolarparalelovzla,dolarbcv,dolarenvenezuela
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: curl_cffi
 Requires-Dist: beautifulsoup4
```

### Comparing `pydolarvenezuela-1.6.3/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.6.4/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.6.3/pyproject.toml` & `pydolarvenezuela-1.6.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.6.3"
+version = "1.6.4"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
@@ -31,14 +31,16 @@
   "dolarlibre",
   "dolarinformal",
   "dolarparalelovzla",
   "dolarbcv",
   "dolarenvenezuela"
 ]
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 "Homepage" = "https://github.com/fcoagz/pydolarvenezuela"
 "Bug Tracker" = "https://github.com/fcoagz/pydolarvenezuela/issues"
```

### Comparing `pydolarvenezuela-1.6.3/setup.py` & `pydolarvenezuela-1.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.6.3'
+VERSION = '1.6.4'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
-LICENSE = 'MIT'
-DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
+LICENSE = 'Apache-2.0 license'
+DESCRIPTION = 'Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.'
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
 LONG_DESC_TYPE = "text/markdown"
 
 INSTALL_REQUIRES = [
       'requests',
       'curl_cffi',
       'beautifulsoup4',
@@ -22,15 +22,15 @@
       'colorama',
       'pytz',
       'redis'
       ]
 
 CLASSIFIERS = [
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ]
```

