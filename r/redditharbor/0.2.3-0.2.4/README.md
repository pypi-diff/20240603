# Comparing `tmp/redditharbor-0.2.3.tar.gz` & `tmp/redditharbor-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redditharbor-0.2.3.tar", last modified: Fri Apr 19 05:56:02 2024, max compression
+gzip compressed data, was "redditharbor-0.2.4.tar", last modified: Sun Jun  2 21:27:11 2024, max compression
```

## Comparing `redditharbor-0.2.3.tar` & `redditharbor-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.721027 redditharbor-0.2.3/
--rw-rw-rw-   0        0        0     1084 2023-12-06 15:35:46.000000 redditharbor-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      153 2024-01-09 02:55:52.000000 redditharbor-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      798 2024-04-19 05:56:02.720028 redditharbor-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    10060 2024-04-18 14:29:48.000000 redditharbor-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.617356 redditharbor-0.2.3/redditharbor/
--rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.704586 redditharbor-0.2.3/redditharbor/dock/
--rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/dock/__init__.py
--rw-rw-rw-   0        0        0    52389 2024-04-11 00:15:31.000000 redditharbor-0.2.3/redditharbor/dock/pipeline.py
--rw-rw-rw-   0        0        0     7044 2023-12-22 18:42:34.000000 redditharbor-0.2.3/redditharbor/login.py
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.714068 redditharbor-0.2.3/redditharbor/utils/
--rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/utils/__init__.py
--rw-rw-rw-   0        0        0    43299 2024-03-18 14:45:00.000000 redditharbor-0.2.3/redditharbor/utils/download.py
--rw-rw-rw-   0        0        0     6026 2024-02-16 11:32:00.000000 redditharbor-0.2.3/redditharbor/utils/fetch.py
--rw-rw-rw-   0        0        0     1683 2023-12-18 14:33:43.000000 redditharbor-0.2.3/redditharbor/utils/metrics.py
--rw-rw-rw-   0        0        0     6025 2023-12-21 19:53:08.000000 redditharbor-0.2.3/redditharbor/utils/subreddit_collections.py
-drwxrwxrwx   0        0        0        0 2024-04-19 05:56:02.717660 redditharbor-0.2.3/redditharbor.egg-info/
--rw-rw-rw-   0        0        0      798 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 05:56:02.000000 redditharbor-0.2.3/redditharbor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-19 05:56:02.723318 redditharbor-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      997 2024-04-19 05:55:46.000000 redditharbor-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:27:11.556136 redditharbor-0.2.4/
+-rw-rw-rw-   0        0        0     1084 2023-12-06 15:35:46.000000 redditharbor-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      153 2024-01-09 02:55:52.000000 redditharbor-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      839 2024-06-02 21:27:11.555137 redditharbor-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10060 2024-04-18 14:29:48.000000 redditharbor-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 21:27:11.491841 redditharbor-0.2.4/redditharbor/
+-rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.4/redditharbor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:27:11.533697 redditharbor-0.2.4/redditharbor/dock/
+-rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.4/redditharbor/dock/__init__.py
+-rw-rw-rw-   0        0        0    52389 2024-04-11 00:15:31.000000 redditharbor-0.2.4/redditharbor/dock/pipeline.py
+-rw-rw-rw-   0        0        0     7044 2023-12-22 18:42:34.000000 redditharbor-0.2.4/redditharbor/login.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:27:11.546656 redditharbor-0.2.4/redditharbor/utils/
+-rw-rw-rw-   0        0        0        0 2023-12-18 14:33:43.000000 redditharbor-0.2.4/redditharbor/utils/__init__.py
+-rw-rw-rw-   0        0        0    43621 2024-06-02 21:23:53.000000 redditharbor-0.2.4/redditharbor/utils/download.py
+-rw-rw-rw-   0        0        0     6026 2024-02-16 11:32:00.000000 redditharbor-0.2.4/redditharbor/utils/fetch.py
+-rw-rw-rw-   0        0        0     1683 2023-12-18 14:33:43.000000 redditharbor-0.2.4/redditharbor/utils/metrics.py
+-rw-rw-rw-   0        0        0     6025 2023-12-21 19:53:08.000000 redditharbor-0.2.4/redditharbor/utils/subreddit_collections.py
+drwxrwxrwx   0        0        0        0 2024-06-02 21:27:11.550643 redditharbor-0.2.4/redditharbor.egg-info/
+-rw-rw-rw-   0        0        0      839 2024-06-02 21:27:11.000000 redditharbor-0.2.4/redditharbor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-06-02 21:27:11.000000 redditharbor-0.2.4/redditharbor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 21:27:11.000000 redditharbor-0.2.4/redditharbor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2024-06-02 21:27:11.000000 redditharbor-0.2.4/redditharbor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 21:27:11.000000 redditharbor-0.2.4/redditharbor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 21:27:11.560120 redditharbor-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2024-06-02 21:27:07.000000 redditharbor-0.2.4/setup.py
```

### Comparing `redditharbor-0.2.3/LICENSE` & `redditharbor-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.3/PKG-INFO` & `redditharbor-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: redditharbor
-Version: 0.2.3
+Version: 0.2.4
 Summary: Effortlessly collect and store Reddit data in your database.
 Home-page: https://github.com/socius-org/RedditHarbor/
-Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.3.tar.gz
+Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.4.tar.gz
 Author: Nick S.H Oh
 Author-email: research@socius.org
 License: MIT
 Keywords: Reddit,Supabase,reddit-api,database,reddit-crawler,reddit-scraper
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: praw==7.7.1
 Requires-Dist: supabase==1.0.3
 Requires-Dist: rich==13.4.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: presidio-analyzer==2.2.351
 Requires-Dist: presidio-anonymizer==2.2.351
-Requires-Dist: pillow>=10.2.0
+Requires-Dist: pillow>=10.3.0
 Requires-Dist: requests==2.31.0
 Provides-Extra: pii
 Requires-Dist: spacy[en_core_web_lg]; extra == "pii"
```

### Comparing `redditharbor-0.2.3/README.md` & `redditharbor-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.3/redditharbor/dock/pipeline.py` & `redditharbor-0.2.4/redditharbor/dock/pipeline.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.3/redditharbor/login.py` & `redditharbor-0.2.4/redditharbor/login.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.3/redditharbor/utils/download.py` & `redditharbor-0.2.4/redditharbor/utils/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,17 @@
             else:
                 start_row += self.page_size
                 end_row = self.row_count
             
             paginated_submissions = (
                 self.submission_db.select(*columns).range(start_row, end_row).execute()
             ).model_dump()["data"]
-            with open(f"{save_file_path}\{file_name}_{page}.pickle", "wb") as handle:
+            with open(
+                os.path.join(save_file_path, f"{file_name}_{page}.pickle"), "wb"
+            ) as handle:
                 pickle.dump(
                     paginated_submissions, handle, protocol=pickle.HIGHEST_PROTOCOL
                 )
 
         return console.print(
             f"{self.row_count} rows downloaded and saved in {self.page_numbers - 1} pickle files"
         )
@@ -162,15 +164,16 @@
             ValueError: If the provided columns are not valid or if the input is neither a string nor a list.
 
         Returns:
             None. Prints the number of rows downloaded and the CSV file created.
         """
 
         save_file_path = os.path.join(self.cwd, f"{file_path}")
-        
+        save_file_name = os.path.join(save_file_path, f"{file_name}.csv")
+
         os.makedirs(save_file_path, exist_ok=True)
 
         if isinstance(columns, str):
             if columns.lower() == "all":
                 columns = "*"
             else:
                 raise ValueError(f"Invalid input: {columns}")
@@ -180,15 +183,15 @@
                 raise ValueError(f"Invalid column names provided: {invalid_columns}")
         else:
             raise ValueError("Input is neither a string nor a list.")
 
         start_row, end_row = 0, 1000
 
         with open(
-            f"{save_file_path}\{file_name}.csv", "w", newline="", encoding="utf-8"
+            save_file_name, "w", newline="", encoding="utf-8"
         ) as csvfile:
             writer = csv.writer(csvfile)
             writer.writerow(columns if columns != "*" else self.columns)
 
             for page in track(
                 range(1, self.page_numbers + 1),
                 description=f"Downloading to .csv file in {save_file_path}",
@@ -207,15 +210,15 @@
                     .range(start_row, end_row)
                     .execute()
                 ).model_dump()["data"]
                 for row in paginated_submissions:
                     writer.writerow(list(row.values()))
 
         return console.print(
-            f"{self.row_count} rows downloaded and saved in {save_file_path}\{file_name}.csv"
+            f"{self.row_count} rows downloaded and saved in {save_file_name}"
         )
 
     def to_txt(self, columns: List[str] or str, file_name: str = "submission", file_path: str = "submission_exports"):
         """
         Save Supabase data to a .txt file.
 
         Args:
@@ -227,14 +230,15 @@
             ValueError: If the provided columns are not valid or if the input is neither a string nor a list.
 
         Returns:
             None. Prints the number of rows downloaded and the TXT file created.
         """
 
         save_file_path = os.path.join(self.cwd, f"{file_path}")
+        save_file_name = os.path.join(save_file_path, f"{file_name}.txt")
         
         os.makedirs(save_file_path, exist_ok=True)
 
         if isinstance(columns, str):
             if columns.lower() == "all":
                 columns = "*"
             else:
@@ -244,17 +248,15 @@
             if invalid_columns:
                 raise ValueError(f"Invalid column names provided: {invalid_columns}")
         else:
             raise ValueError("Input is neither a string nor a list.")
 
         start_row, end_row = 0, self.page_size
 
-        with open(
-            f"{save_file_path}\{file_name}.txt", "w", encoding="utf-8"
-        ) as txtfile:
+        with open(save_file_name, "w", encoding="utf-8") as txtfile:
             txtfile.write("\t".join(columns if columns != "*" else self.columns) + "\n")
 
             for page in track(
                 range(1, self.page_numbers + 1),
                 description=f"Downloading to .txt file in {save_file_path}",
             ):
                 if page == 1:
@@ -271,15 +273,15 @@
                     .range(start_row, end_row)
                     .execute()
                 ).model_dump()["data"]
                 for row in paginated_submissions:
                     txtfile.write("\t".join(map(str, row.values())) + "\n")
 
         return console.print(
-            f"{self.row_count} rows downloaded and saved in {save_file_path}\{file_name}.txt"
+            f"{self.row_count} rows downloaded and saved in {save_file_name}"
         )
 
     def to_json(self, columns: List[str] or str, file_name: str = "submission", file_path: str = "submission_exports"):
         """
         Save Supabase data to multiple .json files.
 
         Args:
@@ -325,15 +327,15 @@
                 start_row += self.page_size
                 end_row = self.row_count
             
             paginated_submissions = (
                 self.submission_db.select(*columns).range(start_row, end_row).execute()
             ).model_dump()["data"]
             with open(
-                f"{save_file_path}\{file_name}_{page}.json", "w", encoding="utf-8"
+                os.path.join(save_file_path, f"{file_name}_{page}.json"), "w", encoding="utf-8"
             ) as jsonfile:
                 json.dump(paginated_submissions, jsonfile, ensure_ascii=False, indent=2)
 
         return console.print(
             f"{self.row_count} rows downloaded and saved in {self.page_numbers - 1} json files"
         )
     
@@ -518,15 +520,17 @@
             else:
                 start_row += self.page_size
                 end_row = self.row_count
             
             paginated_comments = (
                 self.comment_db.select(*columns).range(start_row, end_row).execute()
             ).model_dump()["data"]
-            with open(f"{save_file_path}\{file_name}_{page}.pickle", "wb") as handle:
+            with open(
+                os.path.join(save_file_path, f"{file_name}_{page}.pickle"), "wb"
+            ) as handle:
                 pickle.dump(
                     paginated_comments, handle, protocol=pickle.HIGHEST_PROTOCOL
                 )
 
         return console.print(
             f"{self.row_count} rows downloaded and saved in {self.page_numbers - 1} pickle files"
         )
@@ -544,14 +548,15 @@
             ValueError: If the provided columns are not valid or if the input is neither a string nor a list.
 
         Returns:
             None. Prints the number of rows downloaded and the CSV file created.
         """
 
         save_file_path = os.path.join(self.cwd, f"{file_path}")
+        save_file_name = os.path.join(save_file_path, f"{file_name}.csv")
         
         os.makedirs(save_file_path, exist_ok=True)
 
         if isinstance(columns, str):
             if columns.lower() == "all":
                 columns = "*"
             else:
@@ -562,15 +567,15 @@
                 raise ValueError(f"Invalid column names provided: {invalid_columns}")
         else:
             raise ValueError("Input is neither a string nor a list.")
 
         start_row, end_row = 0, self.page_size
 
         with open(
-            f"{save_file_path}\{file_name}.csv", "w", newline="", encoding="utf-8"
+            save_file_name, "w", newline="", encoding="utf-8"
         ) as csvfile:
             writer = csv.writer(csvfile)
             writer.writerow(columns if columns != "*" else self.columns)
 
             for page in track(
                 range(1, self.page_numbers + 1),
                 description=f"Downloading to .csv file in {save_file_path}",
@@ -589,15 +594,15 @@
                     .range(start_row, end_row)
                     .execute()
                 ).model_dump()["data"]
                 for row in paginated_comments:
                     writer.writerow(list(row.values()))
 
         return console.print(
-            f"{self.row_count} rows downloaded and saved in {save_file_path}\{file_name}.csv"
+            f"{self.row_count} rows downloaded and saved in {save_file_name}"
         )
 
     def to_txt(self, columns: List[str] or str, file_name: str = "comment", file_path: str = "comment_exports"):
         """
         Save Supabase data to a .txt file.
 
         Args:
@@ -609,14 +614,15 @@
             ValueError: If the provided columns are not valid or if the input is neither a string nor a list.
 
         Returns:
             None. Prints the number of rows downloaded and the TXT file created.
         """
 
         save_file_path = os.path.join(self.cwd, f"{file_path}")
+        save_file_name = os.path.join(save_file_path, f"{file_name}.txt")
         
         os.makedirs(save_file_path, exist_ok=True)
 
         if isinstance(columns, str):
             if columns.lower() == "all":
                 columns = "*"
             else:
@@ -626,17 +632,15 @@
             if invalid_columns:
                 raise ValueError(f"Invalid column names provided: {invalid_columns}")
         else:
             raise ValueError("Input is neither a string nor a list.")
 
         start_row, end_row = 0, self.page_size
 
-        with open(
-            f"{save_file_path}\{file_name}.txt", "w", encoding="utf-8"
-        ) as txtfile:
+        with open(save_file_name, "w", encoding="utf-8") as txtfile:
             txtfile.write("\t".join(columns if columns != "*" else self.columns) + "\n")
 
             for page in track(
                 range(1, self.page_numbers + 1),
                 description=f"Downloading to .txt file in {save_file_path}",
             ):
                 if page == 1:
@@ -653,15 +657,15 @@
                     .range(start_row, end_row)
                     .execute()
                 ).model_dump()["data"]
                 for row in paginated_comments:
                     txtfile.write("\t".join(map(str, row.values())) + "\n")
 
         return console.print(
-            f"{self.row_count} rows downloaded and saved in {save_file_path}\{file_name}.txt"
+            f"{self.row_count} rows downloaded and saved in {save_file_name}"
         )
 
     def to_json(self, columns: List[str] or str, file_name: str = "comment", file_path: str = "comment_exports"):
         """
         Save Supabase data to multiple .json files.
 
         Args:
@@ -707,15 +711,15 @@
                 start_row += self.page_size
                 end_row = self.row_count
             
             paginated_comments = (
                 self.comment_db.select(*columns).range(start_row, end_row).execute()
             ).model_dump()["data"]
             with open(
-                f"{save_file_path}\{file_name}_{page}.json", "w", encoding="utf-8"
+                os.path.join(save_file_path, f"{file_name}_{page}.json"), "w", encoding="utf-8"
             ) as jsonfile:
                 json.dump(paginated_comments, jsonfile, ensure_ascii=False, indent=2)
 
         return console.print(
             f"{self.row_count} rows downloaded and saved in {self.page_numbers - 1} json files"
         )
 
@@ -829,15 +833,17 @@
             else:
                 start_row += self.page_size
                 end_row = self.row_count
             
             paginated_redditors = (
                 self.redditor_db.select(*columns).range(start_row, end_row).execute()
             ).model_dump()["data"]
-            with open(f"{save_file_path}\{file_name}_{page}.pickle", "wb") as handle:
+            with open(
+                os.path.join(save_file_path, f"{file_name}_{page}.pickle"), "wb"
+            ) as handle:
                 pickle.dump(
                     paginated_redditors, handle, protocol=pickle.HIGHEST_PROTOCOL
                 )
 
         return console.print(
             f"{self.row_count} rows downloaded and saved in {self.page_numbers - 1} pickle files"
         )
@@ -855,14 +861,15 @@
             ValueError: If the provided columns are not valid or if the input is neither a string nor a list.
 
         Returns:
             None. Prints the number of rows downloaded and the CSV file created.
         """
 
         save_file_path = os.path.join(self.cwd, f"{file_path}")
+        save_file_name = os.path.join(save_file_path, f"{file_name}.csv")
         
         os.makedirs(save_file_path, exist_ok=True)
 
         if isinstance(columns, str):
             if columns.lower() == "all":
                 columns = "*"
             else:
@@ -873,15 +880,15 @@
                 raise ValueError(f"Invalid column names provided: {invalid_columns}")
         else:
             raise ValueError("Input is neither a string nor a list.")
 
         start_row, end_row = 0, self.page_size
 
         with open(
-            f"{save_file_path}\{file_name}.csv", "w", newline="", encoding="utf-8"
+            save_file_name, "w", newline="", encoding="utf-8"
         ) as csvfile:
             writer = csv.writer(csvfile)
             writer.writerow(columns if columns != "*" else self.columns)
 
             for page in track(
                 range(1, self.page_numbers + 1),
                 description=f"Downloading to .csv file in {save_file_path}",
@@ -900,15 +907,15 @@
                     .range(start_row, end_row)
                     .execute()
                 ).model_dump()["data"]
                 for row in paginated_redditors:
                     writer.writerow(list(row.values()))
 
         return console.print(
-            f"{self.row_count} rows downloaded and saved in {save_file_path}\{file_name}.csv"
+            f"{self.row_count} rows downloaded and saved in {save_file_name}"
         )
 
     def to_txt(self, columns: List[str] or str, file_name: str = "user", file_path: str = "user_exports"):
         """
         Save Supabase data to a .txt file.
 
         Args:
@@ -920,14 +927,15 @@
             ValueError: If the provided columns are not valid or if the input is neither a string nor a list.
 
         Returns:
             None. Prints the number of rows downloaded and the TXT file created.
         """
 
         save_file_path = os.path.join(self.cwd, f"{file_path}")
+        save_file_name = os.path.join(save_file_path, f"{file_name}.txt")
         
         os.makedirs(save_file_path, exist_ok=True)
 
         if isinstance(columns, str):
             if columns.lower() == "all":
                 columns = "*"
             else:
@@ -937,17 +945,15 @@
             if invalid_columns:
                 raise ValueError(f"Invalid column names provided: {invalid_columns}")
         else:
             raise ValueError("Input is neither a string nor a list.")
 
         start_row, end_row = 0, self.page_size
 
-        with open(
-            f"{save_file_path}\{file_name}.txt", "w", encoding="utf-8"
-        ) as txtfile:
+        with open(save_file_name, "w", encoding="utf-8") as txtfile:
             txtfile.write("\t".join(columns if columns != "*" else self.columns) + "\n")
 
             for page in track(
                 range(1, self.page_numbers + 1),
                 description=f"Downloading to .txt file in {save_file_path}",
             ):
                 if page == 1:
@@ -964,15 +970,15 @@
                     .range(start_row, end_row)
                     .execute()
                 ).model_dump()["data"]
                 for row in paginated_redditors:
                     txtfile.write("\t".join(map(str, row.values())) + "\n")
 
         return console.print(
-            f"{self.row_count} rows downloaded and saved in {save_file_path}\{file_name}.txt"
+            f"{self.row_count} rows downloaded and saved in {save_file_name}"
         )
 
     def to_json(self, columns: List[str] or str, file_name: str = "user", file_path: str = "user_exports"):
         """
         Save Supabase data to multiple .json files.
 
         Args:
@@ -1018,14 +1024,14 @@
                 start_row += self.page_size
                 end_row = self.row_count
             
             paginated_redditors = (
                 self.redditor_db.select(*columns).range(start_row, end_row).execute()
             ).model_dump()["data"]
             with open(
-                f"{save_file_path}\{file_name}_{page}.json", "w", encoding="utf-8"
+                os.path.join(save_file_path, f"{file_name}_{page}.json"), "w", encoding="utf-8"
             ) as jsonfile:
                 json.dump(paginated_redditors, jsonfile, ensure_ascii=False, indent=2)
 
         return console.print(
             f"{self.row_count} rows downloaded and saved in {self.page_numbers} json files"
         )
```

### Comparing `redditharbor-0.2.3/redditharbor/utils/fetch.py` & `redditharbor-0.2.4/redditharbor/utils/fetch.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.3/redditharbor/utils/metrics.py` & `redditharbor-0.2.4/redditharbor/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.3/redditharbor/utils/subreddit_collections.py` & `redditharbor-0.2.4/redditharbor/utils/subreddit_collections.py`

 * *Files identical despite different names*

### Comparing `redditharbor-0.2.3/redditharbor.egg-info/PKG-INFO` & `redditharbor-0.2.4/redditharbor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: redditharbor
-Version: 0.2.3
+Version: 0.2.4
 Summary: Effortlessly collect and store Reddit data in your database.
 Home-page: https://github.com/socius-org/RedditHarbor/
-Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.3.tar.gz
+Download-URL: https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.4.tar.gz
 Author: Nick S.H Oh
 Author-email: research@socius.org
 License: MIT
 Keywords: Reddit,Supabase,reddit-api,database,reddit-crawler,reddit-scraper
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: praw==7.7.1
 Requires-Dist: supabase==1.0.3
 Requires-Dist: rich==13.4.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: presidio-analyzer==2.2.351
 Requires-Dist: presidio-anonymizer==2.2.351
-Requires-Dist: pillow>=10.2.0
+Requires-Dist: pillow>=10.3.0
 Requires-Dist: requests==2.31.0
 Provides-Extra: pii
 Requires-Dist: spacy[en_core_web_lg]; extra == "pii"
```

### Comparing `redditharbor-0.2.3/setup.py` & `redditharbor-0.2.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from setuptools import setup
 
+# with open('README.md') as f:
+#     long_description = f.read()
+
 setup(
   name = 'redditharbor',
   packages = ['redditharbor'],   
-  version = '0.2.3',      
+  version = '0.2.4',      
   license='MIT',        
-  description = 'Effortlessly collect and store Reddit data in your database.',   
+  description = 'Effortlessly collect and store Reddit data in your database.',
+#   long_description=long_description,
+  long_description_content_type='text/markdown',
   author = 'Nick S.H Oh',                   
   author_email = 'research@socius.org',      
   url = 'https://github.com/socius-org/RedditHarbor/',  
-  download_url = 'https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.3.tar.gz', 
+  download_url = 'https://github.com/socius-org/RedditHarbor/archive/refs/tags/0.2.4.tar.gz', 
   keywords = ['Reddit', 'Supabase', 'reddit-api', 'database', 'reddit-crawler', 'reddit-scraper'],
   include_package_data=True,
   install_requires=[
           'praw == 7.7.1',
           'supabase == 1.0.3', 
           'rich == 13.4.2',
           'python-dotenv == 1.0.0',
           'presidio-analyzer == 2.2.351', 
           'presidio-anonymizer == 2.2.351',
-          'pillow >= 10.2.0', 
+          'pillow >= 10.3.0', 
           'requests == 2.31.0'  
       ],
   extras_require={
     'pii': ['spacy[en_core_web_lg]'],
     }
 )
```

