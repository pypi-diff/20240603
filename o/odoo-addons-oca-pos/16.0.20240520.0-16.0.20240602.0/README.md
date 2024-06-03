# Comparing `tmp/odoo_addons_oca_pos-16.0.20240520.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_pos-16.0.20240602.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1768 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3654 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 24-May-21 05:55 odoo_addons_oca_pos-16.0.20240520.0.dist-info/RECORD
-4 files, 4132 bytes uncompressed, 1010 bytes compressed:  75.6%
+Zip file size: 1778 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3726 b- defN 24-Jun-03 05:45 odoo_addons_oca_pos-16.0.20240602.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-03 05:45 odoo_addons_oca_pos-16.0.20240602.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Jun-03 05:45 odoo_addons_oca_pos-16.0.20240602.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 24-Jun-03 05:45 odoo_addons_oca_pos-16.0.20240602.0.dist-info/RECORD
+4 files, 4204 bytes uncompressed, 1020 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/METADATA
+Filename: odoo_addons_oca_pos-16.0.20240602.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/WHEEL
+Filename: odoo_addons_oca_pos-16.0.20240602.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_pos-16.0.20240602.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_pos-16.0.20240520.0.dist-info/RECORD
+Filename: odoo_addons_oca_pos-16.0.20240602.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_pos-16.0.20240520.0.dist-info/METADATA` & `odoo_addons_oca_pos-16.0.20240602.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-pos
-Version: 16.0.20240520.0
+Version: 16.0.20240602.0
 Summary: Meta package for oca-pos Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -39,14 +39,15 @@
 Requires-Dist: odoo-addon-pos-payment-change <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-method-cashdro <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-method-change-policy <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-method-image <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-payment-terminal <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-display-default-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-label <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-pos-product-mergeable-line <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-multi-barcode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-container-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-packaging-multi-barcode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-product-quick-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-receipt-hide-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-receipt-hide-price <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-pos-receipt-replace-user-by-trigram <16.1dev,>=16.0dev
```

