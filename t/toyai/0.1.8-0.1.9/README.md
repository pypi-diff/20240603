# Comparing `tmp/toyai-0.1.8-py3-none-any.whl.zip` & `tmp/toyai-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6838 bytes, number of entries: 13
--rw-r--r--  2.0 unx     4164 b- defN 24-Jun-03 04:22 toyai/ETL.py
+Zip file size: 6855 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     4226 b- defN 24-Jun-03 04:27 toyai/ETL.py
 -rw-r--r--  2.0 unx      725 b- defN 24-Jun-01 16:40 toyai/Trainer.py
 -rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 07:08 toyai/__init__.py
 -rw-r--r--  2.0 unx     2784 b- defN 24-Jun-02 13:01 toyai/cli.py
 -rw-r--r--  2.0 unx     2876 b- defN 24-Jun-01 07:02 toyai/tools/FileText.py
 -rw-r--r--  2.0 unx       68 b- defN 24-Jun-01 06:58 toyai/tools/__init__.py
 -rw-r--r--  2.0 unx      156 b- defN 24-Jun-01 04:04 toyai/tools/os.py
 -rw-r--r--  2.0 unx     1473 b- defN 24-Jun-01 04:04 toyai/tools/txt.py
--rw-r--r--  2.0 unx      360 b- defN 24-Jun-03 04:22 toyai-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 04:22 toyai-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 24-Jun-03 04:22 toyai-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Jun-03 04:22 toyai-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      969 b- defN 24-Jun-03 04:22 toyai-0.1.8.dist-info/RECORD
-13 files, 13806 bytes uncompressed, 5236 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx      360 b- defN 24-Jun-03 04:27 toyai-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 04:27 toyai-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-Jun-03 04:27 toyai-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Jun-03 04:27 toyai-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      969 b- defN 24-Jun-03 04:27 toyai-0.1.9.dist-info/RECORD
+13 files, 13868 bytes uncompressed, 5253 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: toyai/tools/os.py
 Comment: 
 
 Filename: toyai/tools/txt.py
 Comment: 
 
-Filename: toyai-0.1.8.dist-info/METADATA
+Filename: toyai-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: toyai-0.1.8.dist-info/WHEEL
+Filename: toyai-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: toyai-0.1.8.dist-info/entry_points.txt
+Filename: toyai-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: toyai-0.1.8.dist-info/top_level.txt
+Filename: toyai-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: toyai-0.1.8.dist-info/RECORD
+Filename: toyai-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## toyai/ETL.py

```diff
@@ -106,25 +106,27 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if os.path.exists(self.output_dir):
             # เปลี่ยนชื่อโฟลเดอร์
             to_dir = self.output_dir.replace(f"_{self.nameunique}", self.nameunique)
             if os.path.exists(to_dir):
                 tmp_dir = f"{self.root_output_dir}/.tmp/{self.name}/{uuid.uuid4()}"
-                self.logger.log("Move existing file to: {tmp}")
+                self.logger.info("Move existing file to: {tmp}")
                 shutil.move(
                     to_dir,
                     tmp_dir,
                     copy_function=shutil.copy2,
                 )
             shutil.move(
                 self.output_dir,
                 to_dir,
                 copy_function=shutil.copy2,
             )
 
+            self.logger.info("Created : {self.output_dir}")
+
     def get_save_filepath(self, extension):
         filepath = f"{self.output_dir}/{self.name}{extension}"
         if not os.path.exists(self.output_dir):
             return mkdir(filename=filepath)
 
         return filepath
```

## Comparing `toyai-0.1.8.dist-info/RECORD` & `toyai-0.1.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-toyai/ETL.py,sha256=CzAqUwIbxkeZ7USixLh8UfAtLClRqd0esz0IAeX9H70,4164
+toyai/ETL.py,sha256=yOoP0egUeMgafNpqKU-1KEltXiq0O_BKuA3r1qhCEPY,4226
 toyai/Trainer.py,sha256=wBbSCprUUINqhvtHHkIxPkDEyvXKxnic-Hc3W7jFg_E,725
 toyai/__init__.py,sha256=cYh-COdIdSWRhadc5LJIT6-Huf4JFADl0nKwcTLuGQU,92
 toyai/cli.py,sha256=JD8mcD28ziJyoHYSsyUUDXId2BwJPPM2OR5GGsQJdQI,2784
 toyai/tools/FileText.py,sha256=Jvc_D71dUoeepT-aWGvbAvnyd7O2yl_CxkUWBdeL3_Y,2876
 toyai/tools/__init__.py,sha256=hYa5zmDCAaOmjHsbmFJi3wUkE-i3xsTPhGZ2MuOqcRQ,68
 toyai/tools/os.py,sha256=AbSVoJthyWb3yraEcmnbfQ4fKr8Wt0qiFv-uaFZPYRA,156
 toyai/tools/txt.py,sha256=VAZNohxTwGT1fAtI_SUSLNMwjVMHn3VfaQf0mLJ5sQE,1473
-toyai-0.1.8.dist-info/METADATA,sha256=pAgpIhfNK5T8xZhiAZ5c3mAYC6_VqpUlw60BcyjLWOc,360
-toyai-0.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-toyai-0.1.8.dist-info/entry_points.txt,sha256=GhcIoyzdCVpO8zyT2_v7HVy1G9rIk5nBAQ87317B58g,41
-toyai-0.1.8.dist-info/top_level.txt,sha256=k2LxSFWZgS_pbAObmLshiV0RAP0kCuePltZoZg8vhWA,6
-toyai-0.1.8.dist-info/RECORD,,
+toyai-0.1.9.dist-info/METADATA,sha256=NY1-Vw9TjTNKu7wxJ_pWLlNWzDxVGIGiH0wdpdQjz6A,360
+toyai-0.1.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+toyai-0.1.9.dist-info/entry_points.txt,sha256=GhcIoyzdCVpO8zyT2_v7HVy1G9rIk5nBAQ87317B58g,41
+toyai-0.1.9.dist-info/top_level.txt,sha256=k2LxSFWZgS_pbAObmLshiV0RAP0kCuePltZoZg8vhWA,6
+toyai-0.1.9.dist-info/RECORD,,
```

