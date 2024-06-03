# Comparing `tmp/bcraapi-0.0.1.tar.gz` & `tmp/bcraapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcraapi-0.0.1.tar", last modified: Fri May  3 00:02:54 2024, max compression
+gzip compressed data, was "bcraapi-0.0.2.tar", last modified: Mon Jun  3 00:52:00 2024, max compression
```

## Comparing `bcraapi-0.0.1.tar` & `bcraapi-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:02:54.061433 bcraapi-0.0.1/
--rw-rw-rw-   0        0        0    35823 2024-04-30 01:20:25.000000 bcraapi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    11646 2024-05-03 00:02:54.061433 bcraapi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10598 2024-05-02 23:48:39.000000 bcraapi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 00:02:54.042852 bcraapi-0.0.1/bcraapi/
--rw-rw-rw-   0        0        0      152 2024-05-02 22:49:31.000000 bcraapi-0.0.1/bcraapi/__init__.py
--rw-rw-rw-   0        0        0     1159 2024-05-02 22:31:07.000000 bcraapi-0.0.1/bcraapi/api_client.py
--rw-rw-rw-   0        0        0     1920 2024-05-02 23:48:14.000000 bcraapi-0.0.1/bcraapi/get_from_bcra.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:02:54.059422 bcraapi-0.0.1/bcraapi.egg-info/
--rw-rw-rw-   0        0        0    11646 2024-05-03 00:02:53.000000 bcraapi-0.0.1/bcraapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-05-03 00:02:53.000000 bcraapi-0.0.1/bcraapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:02:53.000000 bcraapi-0.0.1/bcraapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-03 00:02:53.000000 bcraapi-0.0.1/bcraapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 00:02:53.000000 bcraapi-0.0.1/bcraapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 00:02:54.061433 bcraapi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1382 2024-05-03 00:00:13.000000 bcraapi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:52:00.724558 bcraapi-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-06-03 00:52:00.692731 bcraapi-0.0.2/.github/
+drwxrwxrwx   0        0        0        0 2024-06-03 00:52:00.706310 bcraapi-0.0.2/.github/workflows/
+-rw-rw-rw-   0        0        0     1363 2024-05-01 21:14:40.000000 bcraapi-0.0.2/.github/workflows/python-package.yml
+-rw-rw-rw-   0        0        0        7 2024-06-02 23:53:27.000000 bcraapi-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0    35823 2024-04-30 01:20:25.000000 bcraapi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    11646 2024-06-03 00:52:00.722966 bcraapi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10598 2024-05-02 23:48:39.000000 bcraapi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 00:52:00.710822 bcraapi-0.0.2/bcraapi/
+-rw-rw-rw-   0        0        0      152 2024-06-03 00:42:35.000000 bcraapi-0.0.2/bcraapi/__init__.py
+-rw-rw-rw-   0        0        0     1161 2024-06-03 00:14:49.000000 bcraapi-0.0.2/bcraapi/api_client.py
+-rw-rw-rw-   0        0        0     1858 2024-06-03 00:11:29.000000 bcraapi-0.0.2/bcraapi/get_from_bcra.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:52:00.720969 bcraapi-0.0.2/bcraapi/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:20:25.000000 bcraapi-0.0.2/bcraapi/tests/__init__.py
+-rw-rw-rw-   0        0        0      546 2024-06-03 00:39:17.000000 bcraapi-0.0.2/bcraapi/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-06-03 00:52:00.720969 bcraapi-0.0.2/bcraapi.egg-info/
+-rw-rw-rw-   0        0        0    11646 2024-06-03 00:52:00.000000 bcraapi-0.0.2/bcraapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-06-03 00:52:00.000000 bcraapi-0.0.2/bcraapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 00:52:00.000000 bcraapi-0.0.2/bcraapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-03 00:52:00.000000 bcraapi-0.0.2/bcraapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-03 00:52:00.000000 bcraapi-0.0.2/bcraapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       36 2024-05-01 21:14:00.000000 bcraapi-0.0.2/pytest.ini
+-rw-rw-rw-   0        0        0       66 2024-06-03 00:38:20.000000 bcraapi-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 00:52:00.724745 bcraapi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1398 2024-06-03 00:41:15.000000 bcraapi-0.0.2/setup.py
```

### Comparing `bcraapi-0.0.1/LICENSE` & `bcraapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bcraapi-0.0.1/PKG-INFO` & `bcraapi-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcraapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python API for Banco Central de la República Argentina (BCRA)
 Home-page: https://github.com/Jaldekoa/BCRA-Wrapper
 Author: Jon Aldekoa
 Author-email: jaldekoa@gmail.com
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `bcraapi-0.0.1/README.md` & `bcraapi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bcraapi-0.0.1/bcraapi/api_client.py` & `bcraapi-0.0.2/bcraapi/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         endpoint (str): Endpoint de la API a la que realiza la petición.
         lang (str): Los idiomas configurados actualmente “es-AR” y “en-US”. De no informar dicho parámetro, la respuesta se realizará por defecto en “es-AR”.
 
     Returns:
         dict: JSON de respuesta.
     """
 
-    base_url, header = "https://api.bcra.gob.ar/estadisticas/v1", __check_lang(lang)
+    base_url, header = "https://api.bcra.gob.ar/estadisticas/v2.0", __check_lang(lang)
     res = requests.get(f"{base_url}/{endpoint}", headers=header, verify=False)
     json = res.json()
 
     if res.status_code == 200:
         return json["results"]
     else:
         raise Exception(f"Error {json['status']}. {'.'.join(json['errorMessages'])}")
```

### Comparing `bcraapi-0.0.1/bcraapi/get_from_bcra.py` & `bcraapi-0.0.2/bcraapi/get_from_bcra.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         return pd.DataFrame.from_dict(json["results"])
     else:
         raise Exception(f"Error {json['status']}. {'.'.join(json['errorMessages'])}")
 
 
 def __parse_cols(df: pd.DataFrame) -> pd.DataFrame:
     if "fecha" in df.columns:
-        df["fecha"] = pd.to_datetime(df["fecha"], format="%d/%m/%Y").dt.strftime("%Y-%m-%d")
+        df["fecha"] = pd.to_datetime(df["fecha"], format="%Y-%m-%d")
     if "valor" in df.columns:
-        df["valor"] = df["valor"].str.replace(".", "").str.replace(",", ".").astype(float)
+        df["valor"] = pd.to_numeric(df["valor"])
     return df
 
 
 def datos_variable(id_variable: int, desde: str, hasta: str) -> pd.DataFrame:
     """
     Método para obtener los valores para la variable y el rango de fechas indicadas.
 
@@ -30,22 +30,22 @@
         id_variable (int): ID de la variable deseada, la misma se puede consultar por el endpoint “Obtener principales variables”.
         desde (str): Corresponde a la fecha de inicio del rango a consultar, la misma deberá tener el formato YYYY-MM-DD.
         hasta (str): Corresponde a la fecha de fin del rango a consultar, la misma deberá tener el formato YYYY-MM-DD.
 
     Returns:
         pd.DataFrame: DataFrame de pandas con las columnas idVariable, fecha y valor.
     """
-    df = __connect_to_data(f"{base_url}/estadisticas/v1/DatosVariable/{id_variable}/{desde}/{hasta}")
+    df = __connect_to_data(f"{base_url}/estadisticas/v2.0/DatosVariable/{id_variable}/{desde}/{hasta}")
     df = __parse_cols(df)
     return df
 
 
 def principales_variables() -> pd.DataFrame:
     """
     Método para obtener la lista de todas las variables publicadas por el BCRA.
 
     Returns:
         pd.DataFrame: DataFrame de pandas con las columnas idVariable, cdSerie, fecha y valor.
     """
-    df = __connect_to_data(f"{base_url}/estadisticas/v1/principalesvariables")
+    df = __connect_to_data(f"{base_url}/estadisticas/v2.0/principalesvariables")
     df = __parse_cols(df)
     return df
```

### Comparing `bcraapi-0.0.1/bcraapi.egg-info/PKG-INFO` & `bcraapi-0.0.2/bcraapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcraapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python API for Banco Central de la República Argentina (BCRA)
 Home-page: https://github.com/Jaldekoa/BCRA-Wrapper
 Author: Jon Aldekoa
 Author-email: jaldekoa@gmail.com
 Platform: Any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `bcraapi-0.0.1/setup.py` & `bcraapi-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 THIS_PATH = Path(__file__).parent
 DESCRIPTION = "Python API for Banco Central de la República Argentina (BCRA)"
-LONG_DESCRIPTION = (THIS_PATH / "README.md").read_text()
+LONG_DESCRIPTION = (THIS_PATH / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="bcraapi",
     version=VERSION,
     url="https://github.com/Jaldekoa/BCRA-Wrapper",
     author="Jon Aldekoa",
```

