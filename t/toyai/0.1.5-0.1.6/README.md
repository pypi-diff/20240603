# Comparing `tmp/toyai-0.1.5-py3-none-any.whl.zip` & `tmp/toyai-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6872 bytes, number of entries: 13
--rw-r--r--  2.0 unx     4156 b- defN 24-Jun-02 15:57 toyai/ETL.py
+Zip file size: 6774 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     3926 b- defN 24-Jun-03 03:50 toyai/ETL.py
 -rw-r--r--  2.0 unx      725 b- defN 24-Jun-01 16:40 toyai/Trainer.py
 -rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 07:08 toyai/__init__.py
 -rw-r--r--  2.0 unx     2784 b- defN 24-Jun-02 13:01 toyai/cli.py
 -rw-r--r--  2.0 unx     2876 b- defN 24-Jun-01 07:02 toyai/tools/FileText.py
 -rw-r--r--  2.0 unx       68 b- defN 24-Jun-01 06:58 toyai/tools/__init__.py
 -rw-r--r--  2.0 unx      156 b- defN 24-Jun-01 04:04 toyai/tools/os.py
 -rw-r--r--  2.0 unx     1473 b- defN 24-Jun-01 04:04 toyai/tools/txt.py
--rw-r--r--  2.0 unx      360 b- defN 24-Jun-02 15:57 toyai-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 15:57 toyai-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 24-Jun-02 15:57 toyai-0.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-Jun-02 15:57 toyai-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      969 b- defN 24-Jun-02 15:57 toyai-0.1.5.dist-info/RECORD
-13 files, 13798 bytes uncompressed, 5270 bytes compressed:  61.8%
+-rw-r--r--  2.0 unx      360 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      969 b- defN 24-Jun-03 03:50 toyai-0.1.6.dist-info/RECORD
+13 files, 13568 bytes uncompressed, 5172 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: toyai/tools/os.py
 Comment: 
 
 Filename: toyai/tools/txt.py
 Comment: 
 
-Filename: toyai-0.1.5.dist-info/METADATA
+Filename: toyai-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: toyai-0.1.5.dist-info/WHEEL
+Filename: toyai-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: toyai-0.1.5.dist-info/entry_points.txt
+Filename: toyai-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: toyai-0.1.5.dist-info/top_level.txt
+Filename: toyai-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: toyai-0.1.5.dist-info/RECORD
+Filename: toyai-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## toyai/ETL.py

```diff
@@ -69,40 +69,38 @@
 
         self.args = UnknownArgs(unknown_args)
 
     def __enter__(self):
         self.nameunique = f"{self.name}"
         self.output_dir = f"{self.output_dir}/_{self.nameunique}"
 
-        # สร้าง logger
-        self.logger = logging.getLogger(f"{self.name}_logger")
-        self.logger.setLevel(logging.INFO)
-
-        # สร้าง handler สำหรับแสดงใน console
-        console_handler = logging.StreamHandler()
-        console_handler.setLevel(logging.INFO)
-
-        self.logger.addHandler(console_handler)
-        # ตรวจสอบว่า logger ไม่มี handler ซ้ำซ้อน
-        if self.isLogs and self.name is not None:
-            # สร้าง handler สำหรับเขียนลงไฟล์
-            file_handler = logging.FileHandler(
-                mkdir(f"{self.output_dir}/{self.name}.log")
-            )
-            file_handler.setLevel(logging.INFO)
-
-            # สร้าง formatter และกำหนดให้กับทั้งสอง handler
-            formatter = logging.Formatter(
-                "%(asctime)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
-            )
-            file_handler.setFormatter(formatter)
-            console_handler.setFormatter(formatter)
+        if not self.logger.hasHandlers():
+            # Create handler for console output
+            console_handler = logging.StreamHandler()
+            console_handler.setLevel(logging.INFO)
+
+            # Add the console handler to the logger
+            self.logger.addHandler(console_handler)
+
+            if self.isLogs and self.name is not None:
+                # Create handler for logging to a file
+                file_handler = logging.FileHandler(
+                    mkdir(f"{self.output_dir}/{self.name}.log")
+                )
+                file_handler.setLevel(logging.INFO)
+
+                # Create formatter and add it to both handlers
+                formatter = logging.Formatter(
+                    "%(asctime)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
+                )
+                file_handler.setFormatter(formatter)
+                console_handler.setFormatter(formatter)
 
-            # เพิ่ม handler ทั้งสองให้กับ logger
-            self.logger.addHandler(file_handler)
+                # Add the file handler to the logger
+                self.logger.addHandler(file_handler)
 
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if os.path.exists(self.output_dir):
             # เปลี่ยนชื่อโฟลเดอร์
             to_dir = self.output_dir.replace(f"_{self.nameunique}", self.nameunique)
```

