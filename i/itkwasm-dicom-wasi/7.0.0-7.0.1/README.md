# Comparing `tmp/itkwasm_dicom_wasi-7.0.0.tar.gz` & `tmp/itkwasm_dicom_wasi-7.0.1.tar.gz`

## Comparing `itkwasm_dicom_wasi-7.0.0.tar` & `itkwasm_dicom_wasi-7.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/_version.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/read_image_dicom_file_series.py
--rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/structured_report_to_html.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/structured_report_to_text.py
--rwxr-xr-x   0        0        0 11805531 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
--rwxr-xr-x   0        0        0  8540051 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
--rwxr-xr-x   0        0        0  8358340 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm
--rwxr-xr-x   0        0        0 11204728 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
--rwxr-xr-x   0        0        0 11185242 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/tests/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/tests/common.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/tests/test_apply_presentation_state_to_image.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/tests/test_read_dicom_encapsulated_pdf.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/tests/test_read_image_dicom_file_series.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/tests/test_structured_report_to_html.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/tests/test_structured_report_to_text.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/.gitignore
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/README.md
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/_version.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/read_image_dicom_file_series.py
+-rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/structured_report_to_html.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/structured_report_to_text.py
+-rwxr-xr-x   0        0        0 11805531 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm
+-rwxr-xr-x   0        0        0  8540051 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm
+-rwxr-xr-x   0        0        0  8358340 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm
+-rwxr-xr-x   0        0        0 11204728 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm
+-rwxr-xr-x   0        0        0 11185242 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/tests/common.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/tests/test_apply_presentation_state_to_image.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/tests/test_read_dicom_encapsulated_pdf.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/tests/test_read_image_dicom_file_series.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/tests/test_structured_report_to_html.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/tests/test_structured_report_to_text.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/.gitignore
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/README.md
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 itkwasm_dicom_wasi-7.0.1/PKG-INFO
```

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/apply_presentation_state_to_image.py` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/apply_presentation_state_to_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/read_dicom_encapsulated_pdf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/read_image_dicom_file_series.py` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/read_image_dicom_file_series.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/structured_report_to_html.py` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/structured_report_to_html.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/structured_report_to_text.py` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/structured_report_to_text.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/apply-presentation-state-to-image.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/read-dicom-encapsulated-pdf.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/read-image-dicom-file-series.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-html.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm` & `itkwasm_dicom_wasi-7.0.1/itkwasm_dicom_wasi/wasm_modules/structured-report-to-text.wasi.wasm`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/README.md` & `itkwasm_dicom_wasi-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/pyproject.toml` & `itkwasm_dicom_wasi-7.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_wasi-7.0.0/PKG-INFO` & `itkwasm_dicom_wasi-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-dicom-wasi
-Version: 7.0.0
+Version: 7.0.1
 Dynamic: Summary
 Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
```

