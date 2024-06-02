# Comparing `tmp/SeqLbToolkit-0.5.0-py3-none-any.whl.zip` & `tmp/SeqLbToolkit-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 31323 bytes, number of entries: 22
+Zip file size: 31365 bytes, number of entries: 22
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-07 15:15 seqlbtoolkit/__init__.py
 -rw-r--r--  2.0 unx    14074 b- defN 24-Jun-01 17:53 seqlbtoolkit/data.py
 -rw-r--r--  2.0 unx     7993 b- defN 24-Jun-01 18:29 seqlbtoolkit/embs.py
--rw-r--r--  2.0 unx     9318 b- defN 24-Jun-01 19:55 seqlbtoolkit/io.py
+-rw-r--r--  2.0 unx     9434 b- defN 24-Jun-02 23:16 seqlbtoolkit/io.py
 -rw-r--r--  2.0 unx     9664 b- defN 24-Jun-01 18:33 seqlbtoolkit/text.py
 -rw-r--r--  2.0 unx     2423 b- defN 24-Jun-01 19:22 seqlbtoolkit/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-07 15:15 seqlbtoolkit/training/__init__.py
 -rw-r--r--  2.0 unx     5511 b- defN 23-Jun-21 15:30 seqlbtoolkit/training/config.py
 -rw-r--r--  2.0 unx     5798 b- defN 23-Jun-21 15:30 seqlbtoolkit/training/eval.py
 -rw-r--r--  2.0 unx     4594 b- defN 23-Jan-07 15:15 seqlbtoolkit/training/output.py
 -rw-r--r--  2.0 unx     4135 b- defN 23-Feb-17 17:51 seqlbtoolkit/training/status.py
 -rw-r--r--  2.0 unx    10455 b- defN 23-Jun-21 15:54 seqlbtoolkit/training/train.py
 -rw-r--r--  2.0 unx      460 b- defN 23-Jun-21 15:30 seqlbtoolkit/training/dataset/__init__.py
 -rw-r--r--  2.0 unx     2176 b- defN 23-Jun-21 15:30 seqlbtoolkit/training/dataset/base_dataset.py
 -rw-r--r--  2.0 unx     1750 b- defN 23-Jun-21 15:30 seqlbtoolkit/training/dataset/batching.py
 -rw-r--r--  2.0 unx     4378 b- defN 23-Jun-21 15:30 seqlbtoolkit/training/dataset/ner_dataset.py
 -rw-r--r--  2.0 unx     7631 b- defN 24-Jun-01 17:53 seqlbtoolkit/training/dataset/utils.py
--rw-r--r--  2.0 unx     1074 b- defN 24-Jun-01 19:58 SeqLbToolkit-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1686 b- defN 24-Jun-01 19:58 SeqLbToolkit-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jun-01 19:58 SeqLbToolkit-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Jun-01 19:58 SeqLbToolkit-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1892 b- defN 24-Jun-01 19:58 SeqLbToolkit-0.5.0.dist-info/RECORD
-22 files, 95117 bytes uncompressed, 28227 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx     1074 b- defN 24-Jun-02 23:18 SeqLbToolkit-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1686 b- defN 24-Jun-02 23:18 SeqLbToolkit-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 23:18 SeqLbToolkit-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Jun-02 23:18 SeqLbToolkit-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1892 b- defN 24-Jun-02 23:18 SeqLbToolkit-0.5.1.dist-info/RECORD
+22 files, 95233 bytes uncompressed, 28269 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: seqlbtoolkit/training/dataset/ner_dataset.py
 Comment: 
 
 Filename: seqlbtoolkit/training/dataset/utils.py
 Comment: 
 
-Filename: SeqLbToolkit-0.5.0.dist-info/LICENSE
+Filename: SeqLbToolkit-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: SeqLbToolkit-0.5.0.dist-info/METADATA
+Filename: SeqLbToolkit-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: SeqLbToolkit-0.5.0.dist-info/WHEEL
+Filename: SeqLbToolkit-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: SeqLbToolkit-0.5.0.dist-info/top_level.txt
+Filename: SeqLbToolkit-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: SeqLbToolkit-0.5.0.dist-info/RECORD
+Filename: SeqLbToolkit-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## seqlbtoolkit/io.py

```diff
@@ -1,24 +1,26 @@
 import os
 import os.path as osp
 import re
 import json
 import yaml
 import shutil
 import logging
+import textwrap
 from pathlib import Path
 from typing import Optional
+from dataclasses import asdict
 
 from rich.logging import RichHandler
 from .utils import deprecated
 
 logger = logging.getLogger(__name__)
 
 
-def set_logging(log_path: Optional[str] = None):
+def set_logging(log_path: Optional[str] = None, level: str = "NOTSET"):
     """Sets up logging format and file handler.
 
     Args:
         log_path (Optional[str]): Path to save the logging file. If None, no log file is saved.
     """
     rh = RichHandler()
     rh.setFormatter(logging.Formatter("%(message)s", datefmt="[%m/%d %X]"))
@@ -30,24 +32,24 @@
         if osp.isfile(log_path):
             os.remove(log_path)
 
         file_handler = logging.FileHandler(filename=log_path)
         file_handler.setLevel(logging.DEBUG)
 
         logging.basicConfig(
-            level="NOTSET",
+            level=level,
             format="%(asctime)s %(levelname)-8s %(message)-80s     @ %(pathname)-s:%(lineno)d",
             datefmt="[%m/%d %X]",
             handlers=[file_handler, rh],
         )
 
     else:
         logging.basicConfig(
             datefmt="[%m/%d %X]",
-            level="NOTSET",
+            level=level,
             handlers=[rh],
         )
 
     return None
 
 
 def logging_args(args):
@@ -60,19 +62,20 @@
 
     Returns
     -------
     None
     """
     arg_elements = {
         attr: getattr(args, attr)
-        for attr in dir(args)
+        for attr in asdict(args)
         if not callable(getattr(args, attr)) and not attr.startswith("_")
     }
     arg_string = yaml.dump(arg_elements, default_flow_style=False, sort_keys=False)
-    logger.info(f"\nConfigurations ({type(args).__name__}):\n{arg_string}")
+    arg_string = textwrap.indent(arg_string, "  ")
+    logger.info(f"Configurations ({type(args).__name__}):\n{arg_string}")
 
     return None
 
 
 def remove_dir(directory: str):
     """
     Remove a directory and its subtree folders/files
```

## Comparing `SeqLbToolkit-0.5.0.dist-info/LICENSE` & `SeqLbToolkit-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SeqLbToolkit-0.5.0.dist-info/METADATA` & `SeqLbToolkit-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeqLbToolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: Commonly-used functions for building sequence labeling models.
 Home-page: https://github.com/Yinghao-Li/seqlbtoolkit
 Author: Yinghao Li
 Author-email: yinghaoli@gatech.edu
 License: MIT
 Keywords: nlp sequence-labeling ml machine-learning natural-language-processing
 Classifier: Intended Audience :: Developers
```

## Comparing `SeqLbToolkit-0.5.0.dist-info/RECORD` & `SeqLbToolkit-0.5.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 seqlbtoolkit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 seqlbtoolkit/data.py,sha256=1pQ6eYDpFmVPeNujq2_KAYn-9kbmMsrijr8obMPpsls,14074
 seqlbtoolkit/embs.py,sha256=JJBJslcqm_cCsfjGXyJTUtBBYqPrJI9n1ZR8f580hYg,7993
-seqlbtoolkit/io.py,sha256=qaoxnwCvfb385cZn5INFkK3v_SSKo8Rih5HZ7hlpu_A,9318
+seqlbtoolkit/io.py,sha256=SFtmkGvVJLuneqFauShI3Ja1K23PKMr8FQk4B21TQ3o,9434
 seqlbtoolkit/text.py,sha256=CFPIQf5XoyT-WSJtyEJ7BuU5NnYLfdXc1L5MTSfhqac,9664
 seqlbtoolkit/utils.py,sha256=bkEupoMl5ZEARBD2bxJg7mfxHvjnOl8Bm8u10UJVCYA,2423
 seqlbtoolkit/training/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 seqlbtoolkit/training/config.py,sha256=5FbZ-otUlcOP-8gdwR6RSmUMkGdZ4m7eOXgOKIUwwh4,5511
 seqlbtoolkit/training/eval.py,sha256=Hl_Rku56xQiUOGqH8AaomlA4NcTN2NLUiOngEA-v8Js,5798
 seqlbtoolkit/training/output.py,sha256=WCLN97N51X696VBnegC-WDTCDdKWx_Tapq1re31OtiI,4594
 seqlbtoolkit/training/status.py,sha256=A3YV1ibNJJzQ5mz3DR2fSxWmQS2KQMaR7y1WsxwAg2w,4135
 seqlbtoolkit/training/train.py,sha256=a4Jfzthbds4tp7VakBEg0RHCe7H1-okU_p_APE6RXa0,10455
 seqlbtoolkit/training/dataset/__init__.py,sha256=052hNzLk4HIVRYt5e2cwvb6jJwWQvKYQj0-eRMPWtbM,460
 seqlbtoolkit/training/dataset/base_dataset.py,sha256=ls2z-XH01KRblCl6ZWJOuGZBdLmS7RfbE5iBjXCeDXs,2176
 seqlbtoolkit/training/dataset/batching.py,sha256=Z-lnE9jJTeasga6BV-JFqkTtKQWhEec6iAvPBKssEoU,1750
 seqlbtoolkit/training/dataset/ner_dataset.py,sha256=jTs_eitAWK2oI-8oLhF7O6IUaC0PkFqWVgSOZraHpnI,4378
 seqlbtoolkit/training/dataset/utils.py,sha256=miuBPHHCK5YZviXAOWyXqCUE-rO9CxE_VotIGcUUChE,7631
-SeqLbToolkit-0.5.0.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-SeqLbToolkit-0.5.0.dist-info/METADATA,sha256=j3l-c5nh6-mbQ8gMHn4xWY2yNNYeDitzeCt8937H-u0,1686
-SeqLbToolkit-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-SeqLbToolkit-0.5.0.dist-info/top_level.txt,sha256=8aU1PwL2imnw9evOIpc_BmleP4C6iquKt6qknMvhB5Q,13
-SeqLbToolkit-0.5.0.dist-info/RECORD,,
+SeqLbToolkit-0.5.1.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+SeqLbToolkit-0.5.1.dist-info/METADATA,sha256=ImLHfhz3lJN0jzo6qFror-sTgVG8ihzJpjJnfWJtpNI,1686
+SeqLbToolkit-0.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+SeqLbToolkit-0.5.1.dist-info/top_level.txt,sha256=8aU1PwL2imnw9evOIpc_BmleP4C6iquKt6qknMvhB5Q,13
+SeqLbToolkit-0.5.1.dist-info/RECORD,,
```

