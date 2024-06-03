# Comparing `tmp/guadania-1.9.2.tar.gz` & `tmp/guadania-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guadania-1.9.2.tar", last modified: Thu Feb 29 12:01:51 2024, max compression
+gzip compressed data, was "guadania-1.9.3.tar", last modified: Mon Jun  3 09:28:36 2024, max compression
```

## Comparing `guadania-1.9.2.tar` & `guadania-1.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 12:01:51.790756 guadania-1.9.2/
--rw-rw-rw-   0        0        0      143 2024-02-29 12:01:51.789756 guadania-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-06-30 09:19:51.000000 guadania-1.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 12:01:51.753160 guadania-1.9.2/guadania/
--rw-rw-rw-   0        0        0       53 2023-06-30 09:19:51.000000 guadania-1.9.2/guadania/__init__.py
--rw-rw-rw-   0        0        0    25092 2024-02-23 12:17:17.000000 guadania-1.9.2/guadania/guadañaFunctions.py
-drwxrwxrwx   0        0        0        0 2024-02-29 12:01:51.787494 guadania-1.9.2/guadania/prisma/
--rw-rw-rw-   0        0        0       30 2023-06-30 09:19:51.000000 guadania-1.9.2/guadania/prisma/__init__.py
--rw-rw-rw-   0        0        0     2498 2023-08-02 07:50:05.000000 guadania-1.9.2/guadania/prisma/prismaEnums.py
--rw-rw-rw-   0        0        0    37509 2023-06-30 09:19:51.000000 guadania-1.9.2/guadania/prisma/prismaFunctions.py
-drwxrwxrwx   0        0        0        0 2024-02-29 12:01:51.764663 guadania-1.9.2/guadania.egg-info/
--rw-rw-rw-   0        0        0      143 2024-02-29 12:01:51.000000 guadania-1.9.2/guadania.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-02-29 12:01:51.000000 guadania-1.9.2/guadania.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 12:01:51.000000 guadania-1.9.2/guadania.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-02-29 12:01:51.000000 guadania-1.9.2/guadania.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-29 12:01:51.000000 guadania-1.9.2/guadania.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 12:01:51.790950 guadania-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0      386 2024-02-29 12:01:41.000000 guadania-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:36.556965 guadania-1.9.3/
+-rw-rw-rw-   0        0        0      143 2024-06-03 09:28:36.555333 guadania-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-30 09:19:51.000000 guadania-1.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:36.499206 guadania-1.9.3/guadania/
+-rw-rw-rw-   0        0        0       53 2023-06-30 09:19:51.000000 guadania-1.9.3/guadania/__init__.py
+-rw-rw-rw-   0        0        0    25172 2024-03-06 11:39:11.000000 guadania-1.9.3/guadania/guadañaFunctions.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:36.553334 guadania-1.9.3/guadania/prisma/
+-rw-rw-rw-   0        0        0       30 2023-06-30 09:19:51.000000 guadania-1.9.3/guadania/prisma/__init__.py
+-rw-rw-rw-   0        0        0     2498 2023-08-02 07:50:05.000000 guadania-1.9.3/guadania/prisma/prismaEnums.py
+-rw-rw-rw-   0        0        0    37546 2024-06-03 09:28:14.000000 guadania-1.9.3/guadania/prisma/prismaFunctions.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:28:36.508728 guadania-1.9.3/guadania.egg-info/
+-rw-rw-rw-   0        0        0      143 2024-06-03 09:28:36.000000 guadania-1.9.3/guadania.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-06-03 09:28:36.000000 guadania-1.9.3/guadania.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:28:36.000000 guadania-1.9.3/guadania.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-06-03 09:28:36.000000 guadania-1.9.3/guadania.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 09:28:36.000000 guadania-1.9.3/guadania.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 09:28:36.556965 guadania-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      386 2024-06-03 09:28:23.000000 guadania-1.9.3/setup.py
```

### Comparing `guadania-1.9.2/README.md` & `guadania-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `guadania-1.9.2/guadania/guadañaFunctions.py` & `guadania-1.9.3/guadania/guadañaFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,16 +221,18 @@
 # Si metes el account id no mete el account group
 def compliance_section_by_policy(prismasession, complianceStandard, accountId = None, accountGroup = None, return_json=False):
     section_summary = compliance_section_summary(prismasession, complianceStandard, return_json=True)
 
 
     all_alerts = alerts(prismasession, policyComplianceStandard=complianceStandard, basic = False, detailed=True, cloudAccountId=accountId, accountGroup=accountGroup)
 
-
-    section_alerts = all_alerts[['id', 'resource.id', 'policy.complianceMetadata']]
+    if not all_alerts.empty:
+        section_alerts = all_alerts[['id', 'resource.id', 'policy.complianceMetadata']]
+    else:
+        section_alerts = all_alerts
     failed_resources = {}
     policies = list_policies(prismasession, complianceStandard)
     section_req = {}
     for section in section_summary:
         failed_resources[section['name']] = {}
         for index, pol in policies.iterrows():
             for comp in pol['complianceMetadata']:
```

### Comparing `guadania-1.9.2/guadania/prisma/prismaEnums.py` & `guadania-1.9.3/guadania/prisma/prismaEnums.py`

 * *Files identical despite different names*

### Comparing `guadania-1.9.2/guadania/prisma/prismaFunctions.py` & `guadania-1.9.3/guadania/prisma/prismaFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -891,20 +891,20 @@
         payload["timerange"] = timerange
 
     headers = {
         "content-type": "application/json; charset=UTF-8",
         'x-redlock-auth': prismaSession.token
     }
 
-    response = requests.request("POST", prismaSession.apiUrl + '/search/config/',
+    response = requests.request("POST", prismaSession.apiUrl + '/search/api/v2/config/',
                                 headers=headers, json=payload)
     try:
         if response.status_code == 200 or response.status_code == 202:
             return json.loads(response.text)
         else:
             raise HTTPError(prismaSession.apiUrl, response.status_code,
                             json.loads(response.text)['message'], response.headers, None)
     except:
-        print("Error en query")
+        print("Error en query: " + str(response.status_code))
```

