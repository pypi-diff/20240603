# Comparing `tmp/toyai-0.1.6-py3-none-any.whl.zip` & `tmp/toyai-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6774 bytes, number of entries: 13
--rw-r--r--  2.0 unx     3926 b- defN 24-Jun-03 03:50 toyai/ETL.py
+Zip file size: 6812 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     4066 b- defN 24-Jun-03 03:53 toyai/ETL.py
 -rw-r--r--  2.0 unx      725 b- defN 24-Jun-01 16:40 toyai/Trainer.py
 -rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 07:08 toyai/__init__.py
 -rw-r--r--  2.0 unx     2784 b- defN 24-Jun-02 13:01 toyai/cli.py
 -rw-r--r--  2.0 unx     2876 b- defN 24-Jun-01 07:02 toyai/tools/FileText.py
 -rw-r--r--  2.0 unx       68 b- defN 24-Jun-01 06:58 toyai/tools/__init__.py
 -rw-r--r--  2.0 unx      156 b- defN 24-Jun-01 04:04 toyai/tools/os.py
 -rw-r--r--  2.0 unx     1473 b- defN 24-Jun-01 04:04 toyai/tools/txt.py
--rw-r--r--  2.0 unx      360 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      969 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/RECORD
-13 files, 13568 bytes uncompressed, 5172 bytes compressed:  61.9%
+-rw-r--r--  2.0 unx      360 b- defN 24-Jun-03 03:53 toyai-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 03:53 toyai-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-Jun-03 03:53 toyai-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Jun-03 03:53 toyai-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      969 b- defN 24-Jun-03 03:53 toyai-0.1.7.dist-info/RECORD
+13 files, 13708 bytes uncompressed, 5210 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: toyai/tools/os.py
 Comment: 
 
 Filename: toyai/tools/txt.py
 Comment: 
 
-Filename: toyai-0.1.6.dist-info/METADATA
+Filename: toyai-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: toyai-0.1.6.dist-info/WHEEL
+Filename: toyai-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: toyai-0.1.6.dist-info/entry_points.txt
+Filename: toyai-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: toyai-0.1.6.dist-info/top_level.txt
+Filename: toyai-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: toyai-0.1.6.dist-info/RECORD
+Filename: toyai-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## toyai/ETL.py

```diff
@@ -69,14 +69,18 @@
 
         self.args = UnknownArgs(unknown_args)
 
     def __enter__(self):
         self.nameunique = f"{self.name}"
         self.output_dir = f"{self.output_dir}/_{self.nameunique}"
 
+        # สร้าง logger
+        self.logger = logging.getLogger(f"{self.name}_logger")
+        self.logger.setLevel(logging.INFO)
+
         if not self.logger.hasHandlers():
             # Create handler for console output
             console_handler = logging.StreamHandler()
             console_handler.setLevel(logging.INFO)
 
             # Add the console handler to the logger
             self.logger.addHandler(console_handler)
```

## Comparing `toyai-0.1.6.dist-info/RECORD` & `toyai-0.1.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-toyai/ETL.py,sha256=QUM7kh02V_rvMwnZSyvkZRezaCOkck0BLP4AI4X1RCs,3926
+toyai/ETL.py,sha256=qnNO6Y_Hswxb9AFV6EA7MAMEqE8Dg7O4MeF8opTv7ak,4066
 toyai/Trainer.py,sha256=wBbSCprUUINqhvtHHkIxPkDEyvXKxnic-Hc3W7jFg_E,725
 toyai/__init__.py,sha256=cYh-COdIdSWRhadc5LJIT6-Huf4JFADl0nKwcTLuGQU,92
 toyai/cli.py,sha256=JD8mcD28ziJyoHYSsyUUDXId2BwJPPM2OR5GGsQJdQI,2784
 toyai/tools/FileText.py,sha256=Jvc_D71dUoeepT-aWGvbAvnyd7O2yl_CxkUWBdeL3_Y,2876
 toyai/tools/__init__.py,sha256=hYa5zmDCAaOmjHsbmFJi3wUkE-i3xsTPhGZ2MuOqcRQ,68
 toyai/tools/os.py,sha256=AbSVoJthyWb3yraEcmnbfQ4fKr8Wt0qiFv-uaFZPYRA,156
 toyai/tools/txt.py,sha256=VAZNohxTwGT1fAtI_SUSLNMwjVMHn3VfaQf0mLJ5sQE,1473
-toyai-0.1.6.dist-info/METADATA,sha256=eCxjTV3Oo7HH_m8rTrtdesJwh6OvNs_GAfOfxZNw9gE,360
-toyai-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-toyai-0.1.6.dist-info/entry_points.txt,sha256=GhcIoyzdCVpO8zyT2_v7HVy1G9rIk5nBAQ87317B58g,41
-toyai-0.1.6.dist-info/top_level.txt,sha256=k2LxSFWZgS_pbAObmLshiV0RAP0kCuePltZoZg8vhWA,6
-toyai-0.1.6.dist-info/RECORD,,
+toyai-0.1.7.dist-info/METADATA,sha256=IVOtpgI2TKRqEqgBIhzFF0eV9_Yz7xrH0JTRowy3J-8,360
+toyai-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+toyai-0.1.7.dist-info/entry_points.txt,sha256=GhcIoyzdCVpO8zyT2_v7HVy1G9rIk5nBAQ87317B58g,41
+toyai-0.1.7.dist-info/top_level.txt,sha256=k2LxSFWZgS_pbAObmLshiV0RAP0kCuePltZoZg8vhWA,6
+toyai-0.1.7.dist-info/RECORD,,
```

