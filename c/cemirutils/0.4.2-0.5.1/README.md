# Comparing `tmp/cemirutils-0.4.2.tar.gz` & `tmp/cemirutils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemirutils-0.4.2.tar", last modified: Mon Jun  3 10:55:44 2024, max compression
+gzip compressed data, was "cemirutils-0.5.1.tar", last modified: Mon Jun  3 14:57:19 2024, max compression
```

## Comparing `cemirutils-0.4.2.tar` & `cemirutils-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:55:44.230614 cemirutils-0.4.2/
--rw-rw-r--   0 muslu     (1000) muslu     (1000)        0 2024-06-03 07:24:46.000000 cemirutils-0.4.2/LICENSE
--rw-r--r--   0 muslu     (1000) muslu     (1000)     5519 2024-06-03 10:55:44.230614 cemirutils-0.4.2/PKG-INFO
--rw-rw-r--   0 muslu     (1000) muslu     (1000)     5055 2024-06-03 10:53:24.000000 cemirutils-0.4.2/README.md
-drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:55:44.230614 cemirutils-0.4.2/cemirutils/
--rw-rw-r--   0 muslu     (1000) muslu     (1000)      140 2024-06-03 07:24:46.000000 cemirutils-0.4.2/cemirutils/__init__.py
--rw-rw-r--   0 muslu     (1000) muslu     (1000)    30488 2024-06-03 10:33:45.000000 cemirutils-0.4.2/cemirutils/utils.py
-drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 10:55:44.230614 cemirutils-0.4.2/cemirutils.egg-info/
--rw-r--r--   0 muslu     (1000) muslu     (1000)     5519 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/PKG-INFO
--rw-rw-r--   0 muslu     (1000) muslu     (1000)      205 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/SOURCES.txt
--rw-rw-r--   0 muslu     (1000) muslu     (1000)        1 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/dependency_links.txt
--rw-rw-r--   0 muslu     (1000) muslu     (1000)       11 2024-06-03 10:55:44.000000 cemirutils-0.4.2/cemirutils.egg-info/top_level.txt
--rw-rw-r--   0 muslu     (1000) muslu     (1000)       38 2024-06-03 10:55:44.230614 cemirutils-0.4.2/setup.cfg
--rw-rw-r--   0 muslu     (1000) muslu     (1000)      677 2024-06-03 10:55:31.000000 cemirutils-0.4.2/setup.py
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 14:57:19.305361 cemirutils-0.5.1/
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)        0 2024-06-03 07:24:46.000000 cemirutils-0.5.1/LICENSE
+-rw-r--r--   0 muslu     (1000) muslu     (1000)     5519 2024-06-03 14:57:19.305361 cemirutils-0.5.1/PKG-INFO
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)     5055 2024-06-03 10:53:24.000000 cemirutils-0.5.1/README.md
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 14:57:19.305361 cemirutils-0.5.1/cemirutils/
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      140 2024-06-03 07:24:46.000000 cemirutils-0.5.1/cemirutils/__init__.py
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)    31980 2024-06-03 14:51:38.000000 cemirutils-0.5.1/cemirutils/utils.py
+drwxrwxr-x   0 muslu     (1000) muslu     (1000)        0 2024-06-03 14:57:19.305361 cemirutils-0.5.1/cemirutils.egg-info/
+-rw-r--r--   0 muslu     (1000) muslu     (1000)     5519 2024-06-03 14:57:19.000000 cemirutils-0.5.1/cemirutils.egg-info/PKG-INFO
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      205 2024-06-03 14:57:19.000000 cemirutils-0.5.1/cemirutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)        1 2024-06-03 14:57:19.000000 cemirutils-0.5.1/cemirutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)       11 2024-06-03 14:57:19.000000 cemirutils-0.5.1/cemirutils.egg-info/top_level.txt
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)       38 2024-06-03 14:57:19.309361 cemirutils-0.5.1/setup.cfg
+-rw-rw-r--   0 muslu     (1000) muslu     (1000)      677 2024-06-03 14:46:33.000000 cemirutils-0.5.1/setup.py
```

### Comparing `cemirutils-0.4.2/PKG-INFO` & `cemirutils-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cemirutils
-Version: 0.4.2
+Version: 0.5.1
 Summary: Basit veri işleme ve SQL yardımcıları
 Home-page: https://github.com/cememir/cemirutils
 Author: Cem Emir / Muslu Yüksektepe
 Author-email: musluyuksektepe@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cemirutils-0.4.2/README.md` & `cemirutils-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cemirutils-0.4.2/cemirutils/utils.py` & `cemirutils-0.5.1/cemirutils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,42 @@
 import subprocess
 from calendar import monthrange
 from datetime import datetime, timedelta
 from http.server import SimpleHTTPRequestHandler, HTTPServer
 from urllib import request, parse
 
 
+class Dict2Dot(dict):
+    def __getattr__(self, key):
+        if key in self:
+            value = self[key]
+            if isinstance(value, dict):
+                return Dict2Dot(value)
+            return value
+        else:
+            raise AttributeError(f"'{self.__class__.__name__}' objesinde '{key}' anahtarı bulunamadı.")
+
+
 class CemirUtils:
-    def __init__(self, data, dbname, dbuser, dbpassword, dbhost='localhost', dbport=5432, dbcreate_db_if_not_exists=False):
+
+    def __init__(self, data=None, dbname=None, dbuser=None, dbpassword=None, dbhost='localhost', dbport=5432, timeout=3, dbcreate_db_if_not_exists=False):
         """
         CemirUtils sınıfının yapıcı fonksiyonu.
         Verilen veriyi sınıfın 'data' değişkenine atar.
 
         Parametre:
         data (list, dict): İşlenecek sayısal veri listesi veya sözlük.
         """
         self.data = data
         self.dbname = dbname
         self.dbuser = dbuser
         self.dbpassword = dbpassword
         self.dbhost = dbhost
         self.dbport = dbport
+        self.timeout = timeout
 
         if dbcreate_db_if_not_exists:
             self.psql_create_database(dbname)
 
     def getmethods(self):
         """
         CemirUtils sınıfının mevcut tüm metodlarının isimlerini yazdırır.
@@ -64,22 +77,30 @@
         Returns:
             str: Sorgu sonucu veya JSON formatında hata bilgisi.
         """
         if dbname is None:
             dbname = self.dbname
 
         command = f'PGPASSWORD={self.dbpassword} psql -h {self.dbhost} -p {self.dbport} -U {self.dbuser} -d {dbname} -c {json.dumps(query, ensure_ascii=False)}'
-        result = subprocess.run(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-        if result.returncode != 0:
+
+        try:
+            result = subprocess.run(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, timeout=self.timeout)
+            if result.returncode != 0:
+                error_info = {
+                    "error": "Query failed",
+                    "message": result.stderr.strip()
+                }
+                return json.dumps(error_info, ensure_ascii=False)
+            return result.stdout.strip()
+        except subprocess.TimeoutExpired as e:
             error_info = {
-                "error": "Query failed",
-                "message": result.stderr.strip()
+                "error": "TimeOut",
+                "message": f"timed out"
             }
             return json.dumps(error_info, ensure_ascii=False)
-        return result.stdout.strip()
 
     def psql_insert(self, table_name, columns, values, get_id=False):
         """
         Veritabanına yeni kayıt ekler.
 
         Args:
             table_name (str): Tablo adı.
@@ -204,15 +225,15 @@
         try:
             result = int(self.psql_execute_query(query).split()[1])
             if result >= 0:
                 return {"error": False}
         except:
             return self.psql_execute_query(query)
 
-    def days_between_dates(self, date1, date2):
+    def time_days_between_dates(self, date1, date2):
         """
         İki tarih arasındaki gün sayısını hesaplar.
 
 
         Args:
             date1 (str): İlk tarih (YYYY-MM-DD formatında).
             date2 (str): İkinci tarih (YYYY-MM-DD formatında).
@@ -223,15 +244,15 @@
         """
         date_format = "%Y-%m-%d"
         d1 = datetime.strptime(date1, date_format)
         d2 = datetime.strptime(date2, date_format)
         delta = d2 - d1
         return delta.days
 
-    def hours_minutes_seconds_between_times(self, time1, time2):
+    def time_hours_minutes_seconds_between_times(self, time1, time2):
         """
         İki zaman arasındaki saat, dakika ve saniye farkını hesaplar.
 
 
         Args:
             time1 (str): İlk zaman (HH:MM:SS formatında).
             time2 (str): İkinci zaman (HH:MM:SS formatında).
@@ -269,15 +290,15 @@
         days = delta.days
         seconds = delta.seconds
         hours = seconds // 3600
         minutes = (seconds % 3600) // 60
         seconds = seconds % 60
         return days, hours, minutes, seconds
 
-    def add_days_to_date(self, date, days):
+    def time_add_days_to_date(self, date, days):
         """
         Belirtilen tarihe gün sayısı ekleyerek yeni bir tarih hesaplar.
 
 
         Args:
             date (str): Başlangıç tarihi (YYYY-MM-DD formatında).
             days (int): Eklenecek gün sayısı.
@@ -287,33 +308,33 @@
             datetime: Yeni tarih.
         """
         date_format = "%Y-%m-%d"
         d = datetime.strptime(date, date_format)
         new_date = d + timedelta(days=days)
         return new_date
 
-    def add_days_and_format(self, date, days):
+    def time_add_days_and_format(self, date, days):
         """
         Belirtilen tarihe gün sayısı ekleyip yeni tarihi istenilen dilde gün adı ile birlikte formatlar.
 
 
         Args:
             date (str): Başlangıç tarihi (YYYY-MM-DD formatında).
             days (int): Eklenecek gün sayısı.
             locale (str): Dil kodu (varsayılan 'en').
 
 
         Returns:
             str: Formatlanmış yeni tarih ve gün adı.
         """
-        new_date = self.add_days_to_date(date, days)
+        new_date = self.time_add_days_to_date(date, days)
         formatted_date = new_date.strftime("%Y-%m-%d")
         return f"{formatted_date} ({new_date})"
 
-    def is_weekend(self, date):
+    def time_is_weekend(self, date):
         """
         Bir tarihin hafta sonu olup olmadığını kontrol eder.
 
 
         Args:
             date (str): Tarih (YYYY-MM-DD formatında).
 
@@ -321,44 +342,44 @@
         Returns:
             bool: Hafta sonu ise True, değilse False.
         """
         date_format = "%Y-%m-%d"
         d = datetime.strptime(date, date_format)
         return d.weekday() >= 5  # 5 = Cumartesi, 6 = Pazar
 
-    def is_leap_year(self, year):
+    def time_is_leap_year(self, year):
         """
         Bir yılın artık yıl olup olmadığını kontrol eder.
 
 
         Args:
             year (int): Yıl.
 
 
         Returns:
             bool: Artık yıl ise True, değilse False.
         """
         return year % 4 == 0 and (year % 100 != 0 or year % 400 == 0)
 
-    def days_in_month(self, year, month):
+    def time_days_in_month(self, year, month):
         """
         Bir ay içindeki gün sayısını döndürür.
 
 
         Args:
             year (int): Yıl.
             month (int): Ay.
 
 
         Returns:
             int: Ay içindeki gün sayısı.
         """
         return monthrange(year, month)[1]
 
-    def next_weekday(self, date, weekday):
+    def time_next_weekday(self, date, weekday):
         """
         Bir tarihten sonraki belirli bir günün tarihini döndürür (örneğin, bir sonraki Pazartesi).
 
 
         Args:
             date (str): Başlangıç tarihi (YYYY-MM-DD formatında).
             weekday (int): Hedef gün (0 = Pazartesi, 1 = Salı, vb.).
@@ -370,31 +391,27 @@
         date_format = "%Y-%m-%d"
         d = datetime.strptime(date, date_format)
         days_ahead = weekday - d.weekday()
         if days_ahead <= 0:  # Hedef gün zaten bu hafta geçmiş
             days_ahead += 7
         return d + timedelta(days=days_ahead)
 
-    def format_date_in_locale(self, date, locale='en', format='full'):
+    @staticmethod
+    def time_todatetime(date):
         """
-        Bir tarihi istenilen dilde ve formatta yazdırır.
-
+        Bir tarihi datetime türüne çevirir
 
         Args:
             date (str): Tarih (YYYY-MM-DD formatında).
-            locale (str): Dil kodu (varsayılan 'en').
-            format (str): Tarih formatı (varsayılan 'full').
-
 
         Returns:
             str: Formatlanmış tarih.
         """
-        date_format = "%Y-%m-%d"
-        d = datetime.strptime(date, date_format)
-        return d
+
+        return datetime.strptime(date, "%Y-%m-%d")
 
     def time_since(self, past_date):
         """
         Belirli bir tarihten geçen yıl, ay, gün, saat, dakika ve saniyeyi hesaplar.
 
         Parametre:
         past_date (str): Geçmiş tarih (yyyy-mm-dd HH:MM:SS formatında)
@@ -423,15 +440,15 @@
             'months': months,
             'days': days,
             'hours': hours,
             'minutes': minutes,
             'seconds': seconds
         }
 
-    def business_days_between_dates(self, date1, date2):
+    def time_business_days_between_dates(self, date1, date2):
         """
         İki tarih arasındaki iş günü sayısını hesaplar.
 
 
         Args:
         date1 (str): İlk tarih (YYYY-MM-DD formatında).
         date2 (str): İkinci tarih (YYYY-MM-DD formatında).
@@ -443,143 +460,152 @@
         date_format = "%Y-%m-%d"
         d1 = datetime.strptime(date1, date_format)
         d2 = datetime.strptime(date2, date_format)
         day_generator = (d1 + timedelta(x) for x in range((d2 - d1).days + 1))
         business_days = sum(1 for day in day_generator if day.weekday() < 5)
         return business_days
 
-    def replace_multiple(self, text, replacements):
+    def str_replace_multiple(self, text, replacements):
         """
         Verilen metinde çoklu değiştirme işlemi yapar.
 
 
         Args:
             text (str): Değiştirilecek metin.
             replacements (dict): Değiştirilecek değer çiftleri (anahtar: eski değer, değer: yeni değer).
 
+        Örnek:
+
+        >>> utils = CemirUtils()
+        >>> print(utils.str_replace_multiple("asd muslu asd", {"asd": "muslu", "muslu": "emir"}))
 
         Returns:
             str: Değiştirilmiş metin.
         """
         for old, new in replacements.items():
             text = text.replace(old, new)
         return text
 
-    def replace_with_last(self, text, values):
+    def str_replace_with_last(self, text, values):
         """
         Verilen metinde belirtilen tüm değerleri son değer ile değiştirir.
 
 
         Args:
             text (str): Değiştirilecek metin.
             values (tuple): Değiştirilecek değerler.
 
+        Örnek:
+
+        >>> utils = CemirUtils()
+        >>> print(utils.str_replace_with_last("asd muslu asd", ("muslu", "emir"}))
+
 
         Returns:
             str: Değiştirilmiş metin.
         """
         if not values:
             return text
         last_value = values[-1]
         for value in values[:-1]:
             text = text.replace(value, last_value)
         return text
 
-    def multiply_by_scalar(self, scalar):
+    def list_multiply_by_scalar(self, scalar):
         """
         Veri listesindeki her bir elemanı verilen skaler değer ile çarpar.
 
         Parametre:
         scalar (int, float): Çarpılacak skaler değer.
 
         Dönüş:
         list: Skaler değer ile çarpılmış veri listesi.
 
         Örnek:
         >>> ceml = CemirUtils([1, 2, 3])
-        >>> ceml.multiply_by_scalar(2)
+        >>> ceml.list_multiply_by_scalar(2)
         [2, 4, 6]
         """
         if isinstance(self.data, list):
             return [x * scalar for x in self.data]
         else:
             raise TypeError("Veri tipi liste olmalıdır.")
 
-    def get_frequency(self, value):
+    def list_get_frequency(self, value):
         """
         Verilen değerin veri listesinde kaç kez geçtiğini sayar.
 
         Parametre:
         value: Sayılacak değer.
 
         Dönüş:
         int: Değerin listede kaç kez geçtiği.
 
         Örnek:
         >>> ceml = CemirUtils([1, 2, 2, 3])
-        >>> ceml.get_frequency(2)
+        >>> ceml.list_get_frequency(2)
         2
         """
         if isinstance(self.data, list):
             return self.data.count(value)
         else:
             raise TypeError("Veri tipi liste olmalıdır.")
 
-    def reverse_list(self):
+    def list_reverse(self):
         """
         Veri listesini tersine çevirir.
 
         Dönüş:
         list: Tersine çevrilmiş veri listesi.
 
         Örnek:
         >>> ceml = CemirUtils([1, 2, 3])
-        >>> ceml.reverse_list()
+        >>> ceml.list_reverse()
         [3, 2, 1]
         """
         if isinstance(self.data, list):
             return self.data[::-1]
         else:
             raise TypeError("Veri tipi liste olmalıdır.")
 
-    def get_max_value(self):
+    def list_get_max_value(self):
         """
         Veri listesindeki en büyük değeri döner.
 
         Dönüş:
         int, float: Veri listesindeki en büyük değer.
 
         Örnek:
         >>> ceml = CemirUtils([1, 2, 3])
-        >>> ceml.get_max_value()
+        >>> ceml.list_get_max_value()
         3
         """
         if isinstance(self.data, list):
             return max(self.data)
         else:
             raise TypeError("Veri tipi liste olmalıdır.")
 
-    def get_min_value(self):
+    def list_get_min_value(self):
         """
         Veri listesindeki en küçük değeri döner.
 
         Dönüş:
         int, float: Veri listesindeki en küçük değer.
 
         Örnek:
         >>> ceml = CemirUtils([1, 2, 3])
-        >>> ceml.get_min_value()
+        >>> ceml.list_get_min_value()
         1
         """
         if isinstance(self.data, list):
             return min(self.data)
         else:
             raise TypeError("Veri tipi liste olmalıdır.")
 
-    def filter_by_key(self, key, value):
+    def dict_filter_by_key(self, key, value):
         """
         Sözlükte veya sözlüklerin bulunduğu listede belirtilen anahtar ve değere sahip elemanları filtreler.
 
         Parametreler:
         key: Filtreleme yapılacak anahtar.
         value: Filtreleme yapılacak değer.
 
@@ -598,55 +624,57 @@
         if isinstance(self.data, dict):
             return {k: v for k, v in self.data.items() if k == key and v == value}
         elif isinstance(self.data, list):
             return [item for item in self.data if isinstance(item, dict) and item.get(key) == value]
         else:
             raise TypeError("Veri tipi sözlük veya sözlük listesi olmalıdır.")
 
-    def get_keys(self):
+    def dict_get_value(self, path):
+        """
+        Verilen yol (path) ifadesine göre sözlük içinde değeri getirir.
+
+        Parametre:
+        path (str): Sözlük içinde istenen değerin yolu (örneğin 'key1.key2.key3').
+
+        Dönüş:
+        Değer (value): Belirtilen yoldaki değer.
+        """
+        keys = path.split('.')
+        value = self.data
+        try:
+            for key in keys:
+                value = value[key]
+        except (TypeError, KeyError):
+            return None
+        return value
+
+    def dict_get_keys(self):
         """
         Sözlükteki veya sözlüklerin bulunduğu listedeki anahtarları döner.
 
         Dönüş:
         list: Anahtarlar listesi.
 
         Örnek:
         >>> cemd = CemirUtils({'a': 1, 'b': 2, 'c': 3})
-        >>> cemd.get_keys()
+        >>> cemd.dict_get_keys()
         ['a', 'b', 'c']
 
         >>> ceml = CemirUtils([{'a': 1}, {'b': 2}, {'a': 3}])
-        >>> ceml.get_keys()
+        >>> ceml.dict_get_keys()
         ['a', 'b', 'a']
         """
         if isinstance(self.data, dict):
             return list(self.data.keys())
         elif isinstance(self.data, list):
             return [key for item in self.data if isinstance(item, dict) for key in item.keys()]
         else:
             raise TypeError("Veri tipi sözlük veya sözlük listesi olmalıdır.")
 
-    def flatten_list(self):
-        """
-        Çok katmanlı listeyi tek katmana indirger.
-
-        Dönüş:
-        list: Tek katmanlı liste.
-
-        Örnek:
-        >>> ceml = CemirUtils([[1, 2], [3, 4], [5]])
-        >>> ceml.flatten_list()
-        [1, 2, 3, 4, 5]
-        """
-        if isinstance(self.data, list) and all(isinstance(i, list) for i in self.data):
-            return [item for sublist in self.data for item in sublist]
-        else:
-            raise TypeError("Veri tipi çok katmanlı liste olmalıdır.")
-
-    def merge_dicts(self, *dicts):
+    def dict_merge(self, *dicts):
         """
         Verilen sözlükleri birleştirir.
 
         Parametreler:
         *dicts (dict): Birleştirilecek sözlükler.
 
         Dönüş:
@@ -661,126 +689,143 @@
             merged = {}
             for d in dicts:
                 merged.update(d)
             return merged
         else:
             raise TypeError("Tüm parametreler sözlük olmalıdır.")
 
-    def filter_greater_than(self, threshold):
+    def list_filter_greater_than(self, threshold):
         """
         Belirtilen eşik değerinden büyük olan öğeleri filtreler.
 
         Parametre:
         threshold (int/float): Eşik değer.
 
         Dönüş:
         list: Eşik değerinden büyük olan öğeleri içeren liste.
 
         Örnek:
         >>> cem = CemirUtils([3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5])
-        >>> cem.filter_greater_than(5)
+        >>> cem.list_filter_greater_than(5)
         [9, 6]
         """
         return [x for x in self.data if x > threshold]
 
-    def filter_less_than(self, threshold):
+    def list_filter_less_than(self, threshold):
         """
         Belirtilen eşik değerinden küçük olan öğeleri filtreler.
 
         Parametre:
         threshold (int/float): Eşik değer.
 
         Dönüş:
         list: Eşik değerinden küçük olan öğeleri içeren liste.
 
         Örnek:
         >>> cem = CemirUtils([3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5])
-        >>> cem.filter_less_than(4)
+        >>> cem.list_filter_less_than(4)
         [3, 1, 1, 2, 3]
         """
         return [x for x in self.data if x < threshold]
 
-    def sum_values(self):
+    def list_flatten(self):
+        """
+        Çok katmanlı listeyi tek katmana indirger.
+
+        Dönüş:
+        list: Tek katmanlı liste.
+
+        Örnek:
+        >>> ceml = CemirUtils([[1, 2], [3, 4], [5]])
+        >>> ceml.flatten_list()
+        [1, 2, 3, 4, 5]
+        """
+        if isinstance(self.data, list) and all(isinstance(i, list) for i in self.data):
+            return [item for sublist in self.data for item in sublist]
+        else:
+            raise TypeError("Veri tipi çok katmanlı liste olmalıdır.")
+
+    def list_sum_values(self):
         """
         Listedeki tüm sayısal değerlerin toplamını hesaplar.
 
         Dönüş:
         int/float: Listedeki sayısal değerlerin toplamı.
 
         Örnek:
         >>> cem = CemirUtils([3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5])
-        >>> cem.sum_values()
+        >>> cem.list_sum_values()
         44
         """
         return sum(self.data)
 
-    def average(self):
+    def list_average(self):
         """
         Listedeki sayısal değerlerin ortalamasını hesaplar.
 
         Dönüş:
         float: Listedeki sayısal değerlerin ortalaması. Liste boşsa 0 döner.
 
         Örnek:
         >>> cem = CemirUtils([3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5])
-        >>> cem.average()
+        >>> cem.list_average()
         4.0
         """
         return sum(self.data) / len(self.data) if self.data else 0
 
-    def head(self, n=5):
+    def list_head(self, n=5):
         """
         Listenin ilk n elemanını döndürür.
         Args:
             n (int): Döndürülecek eleman sayısı (varsayılan 5).
         Returns:
             list: İlk n eleman.
         """
         return self.data[:n]
 
-    def tail(self, n=5):
+    def list_tail(self, n=5):
         """
         Listenin son n elemanını döndürür.
         Args:
             n (int): Döndürülecek eleman sayısı (varsayılan 5).
         Returns:
             list: Son n eleman.
         """
         return self.data[-n:]
 
-    def main(self, n=5):
+    def list_main(self, n=5):
         """
         Listenin ortadaki elemanlarını döndürür.
         Eğer listenin uzunluğu 2n veya daha küçükse tüm listeyi döndürür.
         Args:
             n (int): Kenarlardan kesilecek eleman sayısı (varsayılan 5).
         Returns:
             list: Ortadaki elemanlar.
         """
         if len(self.data) <= 2 * n:
             return self.data
         return self.data[n:-n]
 
-    def unique_values(self):
+    def list_unique_values(self):
         """
         Listenin benzersiz elemanlarını döndürür.
         Returns:
             list: Benzersiz elemanlar.
         """
         return list(set(self.data))
 
-    def sort_asc(self):
+    def list_sort_asc(self):
         """
         Listeyi artan sırada sıralar.
         Returns:
             list: Artan sırada sıralanmış liste.
         """
         return sorted(self.data)
 
-    def sort_desc(self):
+    def list_sort_desc(self):
         """
         Listeyi azalan sırada sıralar.
         Returns:
             list: Azalan sırada sıralanmış liste.
         """
         return sorted(self.data, reverse=True)
```

### Comparing `cemirutils-0.4.2/cemirutils.egg-info/PKG-INFO` & `cemirutils-0.5.1/cemirutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cemirutils
-Version: 0.4.2
+Version: 0.5.1
 Summary: Basit veri işleme ve SQL yardımcıları
 Home-page: https://github.com/cememir/cemirutils
 Author: Cem Emir / Muslu Yüksektepe
 Author-email: musluyuksektepe@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cemirutils-0.4.2/setup.py` & `cemirutils-0.5.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='cemirutils',
-    version='0.4.2',
+    version='0.5.1',
     packages=find_packages(),
     install_requires=[],
     author='Cem Emir / Muslu Yüksektepe',
     author_email='musluyuksektepe@gmail.com',
     description='Basit veri işleme ve SQL yardımcıları',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
```

