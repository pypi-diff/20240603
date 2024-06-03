# Comparing `tmp/cemirutils-0.3.1.tar.gz` & `tmp/cemirutils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemirutils-0.3.1.tar", last modified: Sun May 26 10:12:36 2024, max compression
+gzip compressed data, was "cemirutils-0.4.1.tar", last modified: Mon Jun  3 10:39:12 2024, max compression
```

## Comparing `cemirutils-0.3.1.tar` & `cemirutils-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:12:36.574329 cemirutils-0.3.1/
--rw-rw-rw-   0        0        0        0 2024-05-25 12:03:29.000000 cemirutils-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     4575 2024-05-26 10:12:36.573351 cemirutils-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4103 2024-05-26 10:12:19.000000 cemirutils-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 10:12:36.567494 cemirutils-0.3.1/cemirutils/
--rw-rw-rw-   0        0        0      146 2024-05-25 12:05:50.000000 cemirutils-0.3.1/cemirutils/__init__.py
--rw-rw-rw-   0        0        0    24553 2024-05-26 10:12:19.000000 cemirutils-0.3.1/cemirutils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:12:36.572376 cemirutils-0.3.1/cemirutils.egg-info/
--rw-rw-rw-   0        0        0     4575 2024-05-26 10:12:36.000000 cemirutils-0.3.1/cemirutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-26 10:12:36.000000 cemirutils-0.3.1/cemirutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:12:36.000000 cemirutils-0.3.1/cemirutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-26 10:12:36.000000 cemirutils-0.3.1/cemirutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 10:12:36.574329 cemirutils-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-26 09:55:03.000000 cemirutils-0.3.1/setup.py
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:39:12.734598 cemirutils-0.4.1/
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)        0 2024-06-03 07:24:46.000000 cemirutils-0.4.1/LICENSE
+-rw-r--r--   0 muslu     (1000) muslu     (1000)     5294 2024-06-03 10:39:12.734598 cemirutils-0.4.1/PKG-INFO
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)     4830 2024-06-03 10:36:07.000000 cemirutils-0.4.1/README.md
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:39:12.734598 cemirutils-0.4.1/cemirutils/
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      140 2024-06-03 07:24:46.000000 cemirutils-0.4.1/cemirutils/__init__.py
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)    30488 2024-06-03 10:33:45.000000 cemirutils-0.4.1/cemirutils/utils.py
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:39:12.734598 cemirutils-0.4.1/cemirutils.egg-info/
+-rw-r--r--   0 muslu     (1000) muslu     (1000)     5294 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/PKG-INFO
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      205 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)        1 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)       11 2024-06-03 10:39:12.000000 cemirutils-0.4.1/cemirutils.egg-info/top_level.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)       38 2024-06-03 10:39:12.734598 cemirutils-0.4.1/setup.cfg
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      677 2024-06-03 10:36:54.000000 cemirutils-0.4.1/setup.py
```

### Comparing `cemirutils-0.3.1/PKG-INFO` & `cemirutils-0.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,133 @@
-Metadata-Version: 2.1
-Name: cemirutils
-Version: 0.3.1
-Summary: Basit veri işleme yardımcıları
-Home-page: https://github.com/cememir/cemirutils
-Author: Cem Emir / Muslu Yüksektepe
-Author-email: musluyuksektepe@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<meta charset="UTF-8">
-
-# CemirUtils
-
-CemirUtils, basit veri işleme işlevlerini içeren bir Python yardımcı kütüphanesidir.
-
-## Kurulum
-
-Öncelikle CemirUtils kütüphanesini Python projesine eklemek için aşağıdaki adımları izleyin:
-
-```bash
-pip install cemirutils
-````
-
-
-## Kullanım
-
-Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir. Örneğin:
-
-
-```python
-from cemirutils import CemirUtils
-
-# Mevcut tüm metodların isimlerini yazdır
-cemir_utils = CemirUtils(None)
-print(cemir_utils.getmethods())
-
-
-get_response = cemir_utils.http_get("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
-print("GET Response:", get_response)
-
-# POST isteği
-post_data = {"title": "foo", "body": "bar", "userId": 1}
-post_response = cemir_utils.http_post("https://jsonplaceholder.typicode.com/posts", data=post_data, verify_ssl=True)
-print("POST Response:", post_response)
-
-# PUT isteği
-put_data = {"title": "foo", "body": "bar", "userId": 1}
-put_response = cemir_utils.http_put("https://jsonplaceholder.typicode.com/posts/1", data=put_data, verify_ssl=True)
-print("PUT Response:", put_response)
-
-# DELETE isteği
-delete_response = cemir_utils.http_delete("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
-print("DELETE Response:", delete_response)
-
-# PATCH isteği
-patch_data = {"title": "foo"}
-patch_response = cemir_utils.http_patch("https://jsonplaceholder.typicode.com/posts/1", data=patch_data, verify_ssl=True)
-print("PATCH Response:", patch_response)
-
-
-data_list = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
-cem = CemirUtils(data_list)
-print(data_list)
-print(cem.head(2))  # Listenin ilk 5 elemanını yazdırır.
-print(cem.tail(4))  # Listenin son 5 elemanını yazdırır.
-print(cem.main())  # Listenin ortadaki elemanlarını yazdırır.
-print(cem.unique_values())  # Listenin benzersiz elemanlarını yazdırır.
-print(cem.sort_asc())  # Listenin artan sırada sıralanmış halini yazdırır.
-print(cem.sort_desc())  # Listenin azalan sırada sıralanmış halini yazdırır.
-print(data_list)  # Orijinal veri listesini yazdırır
-print(cem.filter_greater_than(5))  # 5'ten büyük değerleri yazdırır: [9, 6]
-print(cem.filter_less_than(4))  # 4'ten küçük değerleri yazdırır: [3, 1, 1, 2, 3]
-print(cem.sum_values())  # Değerlerin toplamını yazdırır: 44
-print(cem.average())  # Değerlerin ortalamasını yazdırır: 4.0
-
-
-## Zaman işlemleri
-utils = CemirUtils(None)
-print(utils.days_between_dates("2024-05-01", "2024-05-25"))  # 24
-print(utils.hours_minutes_seconds_between_times("08:30:00", "15:45:30"))  # (7, 15, 30)
-print(utils.time_until_date("2024-05-27 23:59:59"))  # Kalan gün, saat, dakika, saniye
-print(utils.add_days_and_format("2024-05-01", 30))  # "2024-05-31 (Cuma)"
-print(utils.is_weekend("2024-05-25"))  # True
-print(utils.is_leap_year(2024))  # True
-print(utils.days_in_month(2024, 2))  # 29
-print(utils.next_weekday("2024-05-25", 0))  # 2024-05-27
-print(utils.time_since("2022-01-01 00:00:00"))  # (2, 4, 24, 14, 30, 15)
-print(utils.business_days_between_dates("2024-05-01", "2024-05-25"))  # 17
-
-
-# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar.
-ceml = CemirUtils([1, 2, 3])
-ceml.multiply_by_scalar(2)  # Output: [2, 4, 6]
-
-
-ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar
-result = ceml.multiply_by_scalar(2)
-print(result)  # Output: [2, 4, 6]
-
-
-ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki en büyük değeri döner.
-ceml.get_max_value()  # Output: 3
-
-
-ceml = CemirUtils([1, 2, 2, 3])
-# Verilen değerin veri listesinde kaç kez geçtiğini sayar.
-result = ceml.get_frequency(2)
-print(result)  # Output: 2
-
-
-cemd = CemirUtils({'a': 1, 'b': 2, 'c': 3})
-# Sözlükteki veya sözlük listesindeki anahtarları döndürür.
-cemd.get_keys()  # Output: ['a', 'b', 'c']
-
-
-ceml = CemirUtils([[1, 2], [3, 4], [5]])
-# Çok katmanlı listeyi tek katmana indirger.
-ceml.flatten_list()  # Output: [1, 2, 3, 4, 5]
-
-````
+<meta charset="UTF-8">
+
+# CemirUtils
+
+CemirUtils, basit veri işleme işlevlerini içeren bir Python yardımcı kütüphanesidir.
+
+## Kurulum
+
+Öncelikle CemirUtils kütüphanesini Python projesine eklemek için aşağıdaki adımları izleyin:
+
+```bash
+pip install cemirutils
+````
+
+
+## Kullanım
+
+
+
+
+* PostgreSQL için CRUD işlemleri.
+```python
+from cemirutils import CemirUtils
+
+# Örnek kullanım
+utils = CemirUtils(data=False, dbname='test_db3', dbuser='postgres', dbpassword='', dbport=5435, dbcreate_db_if_not_exists=True)
+
+print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
+print(utils.psql_insert('test_table', ('id', 'name', 'data'), (3, "emir", {"age": 40, "city": "İzmir"}), get_id=True))
+print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
+print(utils.psql_read('test_table'))
+print(utils.psql_read('test_table_flat'))
+print(utils.psql_update('test_table', {'name': 'MusluY', 'data': '{"age": 40, "city": "Sivas"}'}, 'id = 2', get_id=True))
+print(utils.psql_delete('test_table', 'id = 2'))
+
+```
+
+Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir.
+* Örneğin:
+
+```python
+from cemirutils import CemirUtils
+
+# Mevcut tüm metodların isimlerini yazdır
+cemir_utils = CemirUtils(None)
+print(cemir_utils.getmethods())
+
+
+get_response = cemir_utils.http_get("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
+print("GET Response:", get_response)
+
+# POST isteği
+post_data = {"title": "foo", "body": "bar", "userId": 1}
+post_response = cemir_utils.http_post("https://jsonplaceholder.typicode.com/posts", data=post_data, verify_ssl=True)
+print("POST Response:", post_response)
+
+# PUT isteği
+put_data = {"title": "foo", "body": "bar", "userId": 1}
+put_response = cemir_utils.http_put("https://jsonplaceholder.typicode.com/posts/1", data=put_data, verify_ssl=True)
+print("PUT Response:", put_response)
+
+# DELETE isteği
+delete_response = cemir_utils.http_delete("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
+print("DELETE Response:", delete_response)
+
+# PATCH isteği
+patch_data = {"title": "foo"}
+patch_response = cemir_utils.http_patch("https://jsonplaceholder.typicode.com/posts/1", data=patch_data, verify_ssl=True)
+print("PATCH Response:", patch_response)
+
+
+data_list = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
+cem = CemirUtils(data_list)
+print(data_list)
+print(cem.head(2))  # Listenin ilk 5 elemanını yazdırır.
+print(cem.tail(4))  # Listenin son 5 elemanını yazdırır.
+print(cem.main())  # Listenin ortadaki elemanlarını yazdırır.
+print(cem.unique_values())  # Listenin benzersiz elemanlarını yazdırır.
+print(cem.sort_asc())  # Listenin artan sırada sıralanmış halini yazdırır.
+print(cem.sort_desc())  # Listenin azalan sırada sıralanmış halini yazdırır.
+print(data_list)  # Orijinal veri listesini yazdırır
+print(cem.filter_greater_than(5))  # 5'ten büyük değerleri yazdırır: [9, 6]
+print(cem.filter_less_than(4))  # 4'ten küçük değerleri yazdırır: [3, 1, 1, 2, 3]
+print(cem.sum_values())  # Değerlerin toplamını yazdırır: 44
+print(cem.average())  # Değerlerin ortalamasını yazdırır: 4.0
+
+
+## Zaman işlemleri
+utils = CemirUtils(None)
+print(utils.days_between_dates("2024-05-01", "2024-05-25"))  # 24
+print(utils.hours_minutes_seconds_between_times("08:30:00", "15:45:30"))  # (7, 15, 30)
+print(utils.time_until_date("2024-05-27 23:59:59"))  # Kalan gün, saat, dakika, saniye
+print(utils.add_days_and_format("2024-05-01", 30))  # "2024-05-31 (Cuma)"
+print(utils.is_weekend("2024-05-25"))  # True
+print(utils.is_leap_year(2024))  # True
+print(utils.days_in_month(2024, 2))  # 29
+print(utils.next_weekday("2024-05-25", 0))  # 2024-05-27
+print(utils.time_since("2022-01-01 00:00:00"))  # (2, 4, 24, 14, 30, 15)
+print(utils.business_days_between_dates("2024-05-01", "2024-05-25"))  # 17
+
+
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar.
+ceml = CemirUtils([1, 2, 3])
+ceml.multiply_by_scalar(2)  # Output: [2, 4, 6]
+
+
+ceml = CemirUtils([1, 2, 3])
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar
+result = ceml.multiply_by_scalar(2)
+print(result)  # Output: [2, 4, 6]
+
+
+ceml = CemirUtils([1, 2, 3])
+# Veri listesindeki en büyük değeri döner.
+ceml.get_max_value()  # Output: 3
+
+
+ceml = CemirUtils([1, 2, 2, 3])
+# Verilen değerin veri listesinde kaç kez geçtiğini sayar.
+result = ceml.get_frequency(2)
+print(result)  # Output: 2
+
+
+cemd = CemirUtils({'a': 1, 'b': 2, 'c': 3})
+# Sözlükteki veya sözlük listesindeki anahtarları döndürür.
+cemd.get_keys()  # Output: ['a', 'b', 'c']
+
+
+ceml = CemirUtils([[1, 2], [3, 4], [5]])
+# Çok katmanlı listeyi tek katmana indirger.
+ceml.flatten_list()  # Output: [1, 2, 3, 4, 5]
+
+````
```

### Comparing `cemirutils-0.3.1/cemirutils.egg-info/PKG-INFO` & `cemirutils-0.4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,147 @@
-Metadata-Version: 2.1
-Name: cemirutils
-Version: 0.3.1
-Summary: Basit veri işleme yardımcıları
-Home-page: https://github.com/cememir/cemirutils
-Author: Cem Emir / Muslu Yüksektepe
-Author-email: musluyuksektepe@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<meta charset="UTF-8">
-
-# CemirUtils
-
-CemirUtils, basit veri işleme işlevlerini içeren bir Python yardımcı kütüphanesidir.
-
-## Kurulum
-
-Öncelikle CemirUtils kütüphanesini Python projesine eklemek için aşağıdaki adımları izleyin:
-
-```bash
-pip install cemirutils
-````
-
-
-## Kullanım
-
-Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir. Örneğin:
-
-
-```python
-from cemirutils import CemirUtils
-
-# Mevcut tüm metodların isimlerini yazdır
-cemir_utils = CemirUtils(None)
-print(cemir_utils.getmethods())
-
-
-get_response = cemir_utils.http_get("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
-print("GET Response:", get_response)
-
-# POST isteği
-post_data = {"title": "foo", "body": "bar", "userId": 1}
-post_response = cemir_utils.http_post("https://jsonplaceholder.typicode.com/posts", data=post_data, verify_ssl=True)
-print("POST Response:", post_response)
-
-# PUT isteği
-put_data = {"title": "foo", "body": "bar", "userId": 1}
-put_response = cemir_utils.http_put("https://jsonplaceholder.typicode.com/posts/1", data=put_data, verify_ssl=True)
-print("PUT Response:", put_response)
-
-# DELETE isteği
-delete_response = cemir_utils.http_delete("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
-print("DELETE Response:", delete_response)
-
-# PATCH isteği
-patch_data = {"title": "foo"}
-patch_response = cemir_utils.http_patch("https://jsonplaceholder.typicode.com/posts/1", data=patch_data, verify_ssl=True)
-print("PATCH Response:", patch_response)
-
-
-data_list = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
-cem = CemirUtils(data_list)
-print(data_list)
-print(cem.head(2))  # Listenin ilk 5 elemanını yazdırır.
-print(cem.tail(4))  # Listenin son 5 elemanını yazdırır.
-print(cem.main())  # Listenin ortadaki elemanlarını yazdırır.
-print(cem.unique_values())  # Listenin benzersiz elemanlarını yazdırır.
-print(cem.sort_asc())  # Listenin artan sırada sıralanmış halini yazdırır.
-print(cem.sort_desc())  # Listenin azalan sırada sıralanmış halini yazdırır.
-print(data_list)  # Orijinal veri listesini yazdırır
-print(cem.filter_greater_than(5))  # 5'ten büyük değerleri yazdırır: [9, 6]
-print(cem.filter_less_than(4))  # 4'ten küçük değerleri yazdırır: [3, 1, 1, 2, 3]
-print(cem.sum_values())  # Değerlerin toplamını yazdırır: 44
-print(cem.average())  # Değerlerin ortalamasını yazdırır: 4.0
-
-
-## Zaman işlemleri
-utils = CemirUtils(None)
-print(utils.days_between_dates("2024-05-01", "2024-05-25"))  # 24
-print(utils.hours_minutes_seconds_between_times("08:30:00", "15:45:30"))  # (7, 15, 30)
-print(utils.time_until_date("2024-05-27 23:59:59"))  # Kalan gün, saat, dakika, saniye
-print(utils.add_days_and_format("2024-05-01", 30))  # "2024-05-31 (Cuma)"
-print(utils.is_weekend("2024-05-25"))  # True
-print(utils.is_leap_year(2024))  # True
-print(utils.days_in_month(2024, 2))  # 29
-print(utils.next_weekday("2024-05-25", 0))  # 2024-05-27
-print(utils.time_since("2022-01-01 00:00:00"))  # (2, 4, 24, 14, 30, 15)
-print(utils.business_days_between_dates("2024-05-01", "2024-05-25"))  # 17
-
-
-# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar.
-ceml = CemirUtils([1, 2, 3])
-ceml.multiply_by_scalar(2)  # Output: [2, 4, 6]
-
-
-ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar
-result = ceml.multiply_by_scalar(2)
-print(result)  # Output: [2, 4, 6]
-
-
-ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki en büyük değeri döner.
-ceml.get_max_value()  # Output: 3
-
-
-ceml = CemirUtils([1, 2, 2, 3])
-# Verilen değerin veri listesinde kaç kez geçtiğini sayar.
-result = ceml.get_frequency(2)
-print(result)  # Output: 2
-
-
-cemd = CemirUtils({'a': 1, 'b': 2, 'c': 3})
-# Sözlükteki veya sözlük listesindeki anahtarları döndürür.
-cemd.get_keys()  # Output: ['a', 'b', 'c']
-
-
-ceml = CemirUtils([[1, 2], [3, 4], [5]])
-# Çok katmanlı listeyi tek katmana indirger.
-ceml.flatten_list()  # Output: [1, 2, 3, 4, 5]
-
-````
+Metadata-Version: 2.1
+Name: cemirutils
+Version: 0.4.1
+Summary: Basit veri işleme ve SQL yardımcıları
+Home-page: https://github.com/cememir/cemirutils
+Author: Cem Emir / Muslu Yüksektepe
+Author-email: musluyuksektepe@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<meta charset="UTF-8">
+
+# CemirUtils
+
+CemirUtils, basit veri işleme işlevlerini içeren bir Python yardımcı kütüphanesidir.
+
+## Kurulum
+
+Öncelikle CemirUtils kütüphanesini Python projesine eklemek için aşağıdaki adımları izleyin:
+
+```bash
+pip install cemirutils
+````
+
+
+## Kullanım
+
+
+
+
+* PostgreSQL için CRUD işlemleri.
+```python
+from cemirutils import CemirUtils
+
+# Örnek kullanım
+utils = CemirUtils(data=False, dbname='test_db3', dbuser='postgres', dbpassword='', dbport=5435, dbcreate_db_if_not_exists=True)
+
+print(utils.psql_create_table('test_table_flat', 'id SERIAL PRIMARY KEY, name VARCHAR(100), surname VARCHAR(100)'))
+print(utils.psql_insert('test_table', ('id', 'name', 'data'), (3, "emir", {"age": 40, "city": "İzmir"}), get_id=True))
+print(utils.psql_insert('test_table_flat', ('id', 'name', 'surname'), (3, 'Muslu', 'Yüksektepe'), get_id=True))
+print(utils.psql_read('test_table'))
+print(utils.psql_read('test_table_flat'))
+print(utils.psql_update('test_table', {'name': 'MusluY', 'data': '{"age": 40, "city": "Sivas"}'}, 'id = 2', get_id=True))
+print(utils.psql_delete('test_table', 'id = 2'))
+
+```
+
+Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir.
+* Örneğin:
+
+```python
+from cemirutils import CemirUtils
+
+# Mevcut tüm metodların isimlerini yazdır
+cemir_utils = CemirUtils(None)
+print(cemir_utils.getmethods())
+
+
+get_response = cemir_utils.http_get("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
+print("GET Response:", get_response)
+
+# POST isteği
+post_data = {"title": "foo", "body": "bar", "userId": 1}
+post_response = cemir_utils.http_post("https://jsonplaceholder.typicode.com/posts", data=post_data, verify_ssl=True)
+print("POST Response:", post_response)
+
+# PUT isteği
+put_data = {"title": "foo", "body": "bar", "userId": 1}
+put_response = cemir_utils.http_put("https://jsonplaceholder.typicode.com/posts/1", data=put_data, verify_ssl=True)
+print("PUT Response:", put_response)
+
+# DELETE isteği
+delete_response = cemir_utils.http_delete("https://jsonplaceholder.typicode.com/posts/1", verify_ssl=True)
+print("DELETE Response:", delete_response)
+
+# PATCH isteği
+patch_data = {"title": "foo"}
+patch_response = cemir_utils.http_patch("https://jsonplaceholder.typicode.com/posts/1", data=patch_data, verify_ssl=True)
+print("PATCH Response:", patch_response)
+
+
+data_list = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
+cem = CemirUtils(data_list)
+print(data_list)
+print(cem.head(2))  # Listenin ilk 5 elemanını yazdırır.
+print(cem.tail(4))  # Listenin son 5 elemanını yazdırır.
+print(cem.main())  # Listenin ortadaki elemanlarını yazdırır.
+print(cem.unique_values())  # Listenin benzersiz elemanlarını yazdırır.
+print(cem.sort_asc())  # Listenin artan sırada sıralanmış halini yazdırır.
+print(cem.sort_desc())  # Listenin azalan sırada sıralanmış halini yazdırır.
+print(data_list)  # Orijinal veri listesini yazdırır
+print(cem.filter_greater_than(5))  # 5'ten büyük değerleri yazdırır: [9, 6]
+print(cem.filter_less_than(4))  # 4'ten küçük değerleri yazdırır: [3, 1, 1, 2, 3]
+print(cem.sum_values())  # Değerlerin toplamını yazdırır: 44
+print(cem.average())  # Değerlerin ortalamasını yazdırır: 4.0
+
+
+## Zaman işlemleri
+utils = CemirUtils(None)
+print(utils.days_between_dates("2024-05-01", "2024-05-25"))  # 24
+print(utils.hours_minutes_seconds_between_times("08:30:00", "15:45:30"))  # (7, 15, 30)
+print(utils.time_until_date("2024-05-27 23:59:59"))  # Kalan gün, saat, dakika, saniye
+print(utils.add_days_and_format("2024-05-01", 30))  # "2024-05-31 (Cuma)"
+print(utils.is_weekend("2024-05-25"))  # True
+print(utils.is_leap_year(2024))  # True
+print(utils.days_in_month(2024, 2))  # 29
+print(utils.next_weekday("2024-05-25", 0))  # 2024-05-27
+print(utils.time_since("2022-01-01 00:00:00"))  # (2, 4, 24, 14, 30, 15)
+print(utils.business_days_between_dates("2024-05-01", "2024-05-25"))  # 17
+
+
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar.
+ceml = CemirUtils([1, 2, 3])
+ceml.multiply_by_scalar(2)  # Output: [2, 4, 6]
+
+
+ceml = CemirUtils([1, 2, 3])
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar
+result = ceml.multiply_by_scalar(2)
+print(result)  # Output: [2, 4, 6]
+
+
+ceml = CemirUtils([1, 2, 3])
+# Veri listesindeki en büyük değeri döner.
+ceml.get_max_value()  # Output: 3
+
+
+ceml = CemirUtils([1, 2, 2, 3])
+# Verilen değerin veri listesinde kaç kez geçtiğini sayar.
+result = ceml.get_frequency(2)
+print(result)  # Output: 2
+
+
+cemd = CemirUtils({'a': 1, 'b': 2, 'c': 3})
+# Sözlükteki veya sözlük listesindeki anahtarları döndürür.
+cemd.get_keys()  # Output: ['a', 'b', 'c']
+
+
+ceml = CemirUtils([[1, 2], [3, 4], [5]])
+# Çok katmanlı listeyi tek katmana indirger.
+ceml.flatten_list()  # Output: [1, 2, 3, 4, 5]
+
+````
```

