# Comparing `tmp/aixhello-4.5.tar.gz` & `tmp/aixhello-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-4.5.tar", last modified: Mon Jun  3 09:07:28 2024, max compression
+gzip compressed data, was "aixhello-4.7.tar", last modified: Mon Jun  3 10:21:16 2024, max compression
```

## Comparing `aixhello-4.5.tar` & `aixhello-4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:28.349137 aixhello-4.5/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.5/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-03 09:07:28.348135 aixhello-4.5/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:28.323150 aixhello-4.5/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.5/aixhello/__init__.py
--rw-rw-rw-   0        0        0   621516 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-03 09:07:28.347136 aixhello-4.5/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 09:07:28.353143 aixhello-4.5/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-06-03 09:06:53.000000 aixhello-4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:21:16.329091 aixhello-4.7/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.7/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-03 10:21:16.329091 aixhello-4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:21:16.299750 aixhello-4.7/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.7/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   642328 2024-06-03 10:21:08.000000 aixhello-4.7/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-03 10:21:16.327093 aixhello-4.7/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 10:21:16.331093 aixhello-4.7/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-06-03 10:15:05.000000 aixhello-4.7/setup.py
```

### Comparing `aixhello-4.5/LICENSE` & `aixhello-4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-4.5/PKG-INFO` & `aixhello-4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.5
+Version: 4.7
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.5/README.md` & `aixhello-4.7/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-4.5/aixhello/xyello.c` & `aixhello-4.7/aixhello/xyello.c`

 * *Files 1% similar despite different names*

```diff
@@ -1938,14 +1938,25 @@
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
+/* DictGetItem.proto */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
+#define __Pyx_PyObject_Dict_GetItem(obj, name)\
+    (likely(PyDict_CheckExact(obj)) ?\
+     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
+#else
+#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
+#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
+#endif
+
 /* PyUnicode_Substring.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Substring(
             PyObject* text, Py_ssize_t start, Py_ssize_t stop);
 
 /* UnicodeConcatInPlace.proto */
 # if CYTHON_COMPILING_IN_CPYTHON && PY_MAJOR_VERSION >= 3
     #if CYTHON_REFNANNY
@@ -1970,25 +1981,14 @@
 #define __Pyx_PyObject_LookupSpecial(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 1)
 static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error);
 #else
 #define __Pyx_PyObject_LookupSpecialNoError(o,n) __Pyx_PyObject_GetAttrStrNoError(o,n)
 #define __Pyx_PyObject_LookupSpecial(o,n) __Pyx_PyObject_GetAttrStr(o,n)
 #endif
 
-/* DictGetItem.proto */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
-#define __Pyx_PyObject_Dict_GetItem(obj, name)\
-    (likely(PyDict_CheckExact(obj)) ?\
-     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
-#else
-#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
-#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
-#endif
-
 /* PyObjectFormatSimple.proto */
 #if CYTHON_COMPILING_IN_PYPY
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #elif PY_MAJOR_VERSION < 3
     #define __Pyx_PyObject_FormatSimple(s, f) (\
@@ -2305,32 +2305,32 @@
 #define __Pyx_MODULE_NAME "aixhello.xyello"
 extern int __pyx_module_is_main_aixhello__xyello;
 int __pyx_module_is_main_aixhello__xyello = 0;
 
 /* Implementation of "aixhello.xyello" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_chr;
-static PyObject *__pyx_builtin_open;
 static PyObject *__pyx_builtin_print;
+static PyObject *__pyx_builtin_open;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "";
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_e[] = "e";
 static const char __pyx_k__6[] = "*";
-static const char __pyx_k__7[] = "...";
+static const char __pyx_k__8[] = "...";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_re[] = "re";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
-static const char __pyx_k__11[] = ".";
-static const char __pyx_k__41[] = "?";
+static const char __pyx_k__12[] = ".";
+static const char __pyx_k__44[] = "?";
 static const char __pyx_k_chr[] = "chr";
 static const char __pyx_k_doc[] = "doc";
 static const char __pyx_k_dot[] = "dot";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_mth[] = "mth";
@@ -2440,33 +2440,34 @@
 static const char __pyx_k_encodeText[] = "encodeText";
 static const char __pyx_k_max_length[] = "max_length";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_text_embed[] = "text_embed";
 static const char __pyx_k_text_query[] = "text_query";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_TrainVector[] = "TrainVector";
 static const char __pyx_k_encoded_url[] = "encoded_url";
 static const char __pyx_k_input_bytes[] = "input_bytes";
 static const char __pyx_k_padded_text[] = "padded_text";
 static const char __pyx_k_params_dict[] = "params_dict";
 static const char __pyx_k_searchScore[] = "searchScore";
 static const char __pyx_k_status_code[] = "status_code";
 static const char __pyx_k_text_chunks[] = "text_chunks";
 static const char __pyx_k_CipherEncode[] = "CipherEncode";
 static const char __pyx_k_Content_Type[] = "Content-Type";
 static const char __pyx_k_GraphFEncode[] = "GraphFEncode";
+static const char __pyx_k_UpdateVector[] = "UpdateVector";
 static const char __pyx_k_file_content[] = "file_content";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_vectorSearch[] = "vectorSearch";
 static const char __pyx_k_vector_query[] = "vector_query";
-static const char __pyx_k_SaveToMongoDb[] = "SaveToMongoDb";
 static const char __pyx_k_decryptedText[] = "decryptedText";
 static const char __pyx_k_decrypted_url[] = "decrypted_url";
 static const char __pyx_k_encoded_bytes[] = "encoded_bytes";
 static const char __pyx_k_encryptedText[] = "encryptedText";
 static const char __pyx_k_query_payload[] = "query_payload";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_response_data[] = "response_data";
@@ -2485,55 +2486,57 @@
 static const char __pyx_k_xyellw_Decenigma[] = "xyellw.Decenigma";
 static const char __pyx_k_xyellw_Decipherx[] = "xyellw.Decipherx";
 static const char __pyx_k_xyellw_Encapseal[] = "xyellw.Encapseal";
 static const char __pyx_k_xyellw_limitText[] = "xyellw.limitText";
 static const char __pyx_k_y1c8_8BxP9XN_VKM[] = "y1c8@8BxP9XN#VKM";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_xyellw_TrainVector[] = "xyellw.TrainVector";
 static const char __pyx_k_AuthenticationError[] = "AuthenticationError";
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
 static const char __pyx_k_xyellw_CipherEncode[] = "xyellw.CipherEncode";
 static const char __pyx_k_xyellw_GraphFEncode[] = "xyellw.GraphFEncode";
+static const char __pyx_k_xyellw_UpdateVector[] = "xyellw.UpdateVector";
 static const char __pyx_k_xyellw_vectorSearch[] = "xyellw.vectorSearch";
-static const char __pyx_k_xyellw_SaveToMongoDb[] = "xyellw.SaveToMongoDb";
 static const char __pyx_k_xyellw_vectorizeText[] = "xyellw.vectorizeText";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
 static const char __pyx_k_xyellw_vectorizeEmbed[] = "xyellw.vectorizeEmbed";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_xyellw_SignalSimilarity[] = "xyellw.SignalSimilarity";
 static const char __pyx_k_Invalid_API_key_provided[] = "Invalid API key provided";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
 static const char __pyx_k_An_unexpected_error_occurred[] = "An unexpected error occurred";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
 static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_Error_processing_response_JSON[] = "Error processing response JSON: ";
+static const char __pyx_k_Successfully_update_the_vector[] = "Successfully update the vector.";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
-static const char __pyx_k_Successfully_save_to_the_databas[] = "Successfully save to the database.";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4AsrMkJF3D7AnEcHok5damnRp1itFTxnx2dNcFig8Q+Zg==";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12limitText(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14GraphFEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_file_path); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16CipherEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18SignalSimilarity(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_20vectorSearch(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, CYTHON_UNUSED PyObject *__pyx_v_vector_query, PyObject *__pyx_v_text_query, int __pyx_v_top_n); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_22__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_24__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10UpdateVector(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12TrainVector(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_filename); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14limitText(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16GraphFEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_file_path); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18CipherEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_20SignalSimilarity(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_22vectorSearch(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, CYTHON_UNUSED PyObject *__pyx_v_vector_query, PyObject *__pyx_v_text_query, int __pyx_v_top_n); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_24__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_26__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
@@ -2578,22 +2581,23 @@
   PyObject *__pyx_kp_u_Error;
   PyObject *__pyx_kp_u_Error_processing_response_JSON;
   PyObject *__pyx_n_s_GraphFEncode;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_u_Invalid_API_key_provided;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
-  PyObject *__pyx_n_s_SaveToMongoDb;
   PyObject *__pyx_n_s_SignalSimilarity;
-  PyObject *__pyx_kp_u_Successfully_save_to_the_databas;
-  PyObject *__pyx_kp_u__11;
-  PyObject *__pyx_n_s__41;
+  PyObject *__pyx_kp_u_Successfully_update_the_vector;
+  PyObject *__pyx_n_s_TrainVector;
+  PyObject *__pyx_n_s_UpdateVector;
+  PyObject *__pyx_kp_u__12;
+  PyObject *__pyx_n_s__44;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_kp_u__6;
-  PyObject *__pyx_kp_u__7;
+  PyObject *__pyx_kp_u__8;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_u_accuracy;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
   PyObject *__pyx_n_s_api_key;
@@ -2656,14 +2660,15 @@
   PyObject *__pyx_n_s_exit;
   PyObject *__pyx_n_u_extracted_text;
   PyObject *__pyx_n_s_file;
   PyObject *__pyx_n_s_file_content;
   PyObject *__pyx_n_u_file_data;
   PyObject *__pyx_n_s_file_path;
   PyObject *__pyx_n_u_file_type;
+  PyObject *__pyx_n_s_filename;
   PyObject *__pyx_n_u_filename;
   PyObject *__pyx_n_u_filter;
   PyObject *__pyx_n_s_finalize;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_headers;
@@ -2762,16 +2767,17 @@
   PyObject *__pyx_n_u_wildcard;
   PyObject *__pyx_n_s_xyellw;
   PyObject *__pyx_n_s_xyellw_CipherEncode;
   PyObject *__pyx_n_s_xyellw_Decenigma;
   PyObject *__pyx_n_s_xyellw_Decipherx;
   PyObject *__pyx_n_s_xyellw_Encapseal;
   PyObject *__pyx_n_s_xyellw_GraphFEncode;
-  PyObject *__pyx_n_s_xyellw_SaveToMongoDb;
   PyObject *__pyx_n_s_xyellw_SignalSimilarity;
+  PyObject *__pyx_n_s_xyellw_TrainVector;
+  PyObject *__pyx_n_s_xyellw_UpdateVector;
   PyObject *__pyx_n_s_xyellw___reduce_cython;
   PyObject *__pyx_n_s_xyellw___setstate_cython;
   PyObject *__pyx_n_s_xyellw_limitText;
   PyObject *__pyx_n_s_xyellw_vectorSearch;
   PyObject *__pyx_n_s_xyellw_vectorizeEmbed;
   PyObject *__pyx_n_s_xyellw_vectorizeText;
   PyObject *__pyx_kp_b_y1c8_8BxP9XN_VKM;
@@ -2779,50 +2785,53 @@
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_4;
   PyObject *__pyx_int_200;
   PyObject *__pyx_int_1000;
   PyObject *__pyx_int_222419149;
   PyObject *__pyx_int_228825662;
   PyObject *__pyx_int_238750788;
+  PyObject *__pyx_slice__7;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__5;
-  PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
   PyObject *__pyx_tuple__10;
-  PyObject *__pyx_tuple__12;
-  PyObject *__pyx_tuple__14;
-  PyObject *__pyx_tuple__16;
-  PyObject *__pyx_tuple__18;
-  PyObject *__pyx_tuple__20;
-  PyObject *__pyx_tuple__22;
-  PyObject *__pyx_tuple__24;
-  PyObject *__pyx_tuple__26;
+  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_tuple__13;
+  PyObject *__pyx_tuple__15;
+  PyObject *__pyx_tuple__17;
+  PyObject *__pyx_tuple__19;
+  PyObject *__pyx_tuple__21;
+  PyObject *__pyx_tuple__23;
+  PyObject *__pyx_tuple__25;
   PyObject *__pyx_tuple__27;
   PyObject *__pyx_tuple__29;
-  PyObject *__pyx_tuple__31;
-  PyObject *__pyx_tuple__33;
-  PyObject *__pyx_tuple__35;
-  PyObject *__pyx_tuple__37;
-  PyObject *__pyx_tuple__39;
-  PyObject *__pyx_codeobj__13;
-  PyObject *__pyx_codeobj__15;
-  PyObject *__pyx_codeobj__17;
-  PyObject *__pyx_codeobj__19;
-  PyObject *__pyx_codeobj__21;
-  PyObject *__pyx_codeobj__23;
-  PyObject *__pyx_codeobj__25;
+  PyObject *__pyx_tuple__30;
+  PyObject *__pyx_tuple__32;
+  PyObject *__pyx_tuple__34;
+  PyObject *__pyx_tuple__36;
+  PyObject *__pyx_tuple__38;
+  PyObject *__pyx_tuple__40;
+  PyObject *__pyx_tuple__42;
+  PyObject *__pyx_codeobj__14;
+  PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__18;
+  PyObject *__pyx_codeobj__20;
+  PyObject *__pyx_codeobj__22;
+  PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__26;
   PyObject *__pyx_codeobj__28;
-  PyObject *__pyx_codeobj__30;
-  PyObject *__pyx_codeobj__32;
-  PyObject *__pyx_codeobj__34;
-  PyObject *__pyx_codeobj__36;
-  PyObject *__pyx_codeobj__38;
-  PyObject *__pyx_codeobj__40;
+  PyObject *__pyx_codeobj__31;
+  PyObject *__pyx_codeobj__33;
+  PyObject *__pyx_codeobj__35;
+  PyObject *__pyx_codeobj__37;
+  PyObject *__pyx_codeobj__39;
+  PyObject *__pyx_codeobj__41;
+  PyObject *__pyx_codeobj__43;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2878,22 +2887,23 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_Error);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Error_processing_response_JSON);
   Py_CLEAR(clear_module_state->__pyx_n_s_GraphFEncode);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
-  Py_CLEAR(clear_module_state->__pyx_n_s_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_n_s_SignalSimilarity);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__11);
-  Py_CLEAR(clear_module_state->__pyx_n_s__41);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_update_the_vector);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TrainVector);
+  Py_CLEAR(clear_module_state->__pyx_n_s_UpdateVector);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__12);
+  Py_CLEAR(clear_module_state->__pyx_n_s__44);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__7);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__8);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_u_accuracy);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
@@ -2956,14 +2966,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_exit);
   Py_CLEAR(clear_module_state->__pyx_n_u_extracted_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_file);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_content);
   Py_CLEAR(clear_module_state->__pyx_n_u_file_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_file_path);
   Py_CLEAR(clear_module_state->__pyx_n_u_file_type);
+  Py_CLEAR(clear_module_state->__pyx_n_s_filename);
   Py_CLEAR(clear_module_state->__pyx_n_u_filename);
   Py_CLEAR(clear_module_state->__pyx_n_u_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_finalize);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_headers);
@@ -3062,16 +3073,17 @@
   Py_CLEAR(clear_module_state->__pyx_n_u_wildcard);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_CipherEncode);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_GraphFEncode);
-  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_SignalSimilarity);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_TrainVector);
+  Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_UpdateVector);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_limitText);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorSearch);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeEmbed);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_CLEAR(clear_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
@@ -3079,50 +3091,53 @@
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_4);
   Py_CLEAR(clear_module_state->__pyx_int_200);
   Py_CLEAR(clear_module_state->__pyx_int_1000);
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
   Py_CLEAR(clear_module_state->__pyx_int_228825662);
   Py_CLEAR(clear_module_state->__pyx_int_238750788);
+  Py_CLEAR(clear_module_state->__pyx_slice__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
-  Py_CLEAR(clear_module_state->__pyx_tuple__12);
-  Py_CLEAR(clear_module_state->__pyx_tuple__14);
-  Py_CLEAR(clear_module_state->__pyx_tuple__16);
-  Py_CLEAR(clear_module_state->__pyx_tuple__18);
-  Py_CLEAR(clear_module_state->__pyx_tuple__20);
-  Py_CLEAR(clear_module_state->__pyx_tuple__22);
-  Py_CLEAR(clear_module_state->__pyx_tuple__24);
-  Py_CLEAR(clear_module_state->__pyx_tuple__26);
+  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_tuple__13);
+  Py_CLEAR(clear_module_state->__pyx_tuple__15);
+  Py_CLEAR(clear_module_state->__pyx_tuple__17);
+  Py_CLEAR(clear_module_state->__pyx_tuple__19);
+  Py_CLEAR(clear_module_state->__pyx_tuple__21);
+  Py_CLEAR(clear_module_state->__pyx_tuple__23);
+  Py_CLEAR(clear_module_state->__pyx_tuple__25);
   Py_CLEAR(clear_module_state->__pyx_tuple__27);
   Py_CLEAR(clear_module_state->__pyx_tuple__29);
-  Py_CLEAR(clear_module_state->__pyx_tuple__31);
-  Py_CLEAR(clear_module_state->__pyx_tuple__33);
-  Py_CLEAR(clear_module_state->__pyx_tuple__35);
-  Py_CLEAR(clear_module_state->__pyx_tuple__37);
-  Py_CLEAR(clear_module_state->__pyx_tuple__39);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__19);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
+  Py_CLEAR(clear_module_state->__pyx_tuple__30);
+  Py_CLEAR(clear_module_state->__pyx_tuple__32);
+  Py_CLEAR(clear_module_state->__pyx_tuple__34);
+  Py_CLEAR(clear_module_state->__pyx_tuple__36);
+  Py_CLEAR(clear_module_state->__pyx_tuple__38);
+  Py_CLEAR(clear_module_state->__pyx_tuple__40);
+  Py_CLEAR(clear_module_state->__pyx_tuple__42);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__18);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__22);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
   Py_CLEAR(clear_module_state->__pyx_codeobj__28);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__30);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__32);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__34);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__36);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__38);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__40);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__31);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__33);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__35);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__37);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__39);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__41);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__43);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3156,22 +3171,23 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_Error);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Error_processing_response_JSON);
   Py_VISIT(traverse_module_state->__pyx_n_s_GraphFEncode);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
-  Py_VISIT(traverse_module_state->__pyx_n_s_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_n_s_SignalSimilarity);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__11);
-  Py_VISIT(traverse_module_state->__pyx_n_s__41);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_update_the_vector);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TrainVector);
+  Py_VISIT(traverse_module_state->__pyx_n_s_UpdateVector);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__12);
+  Py_VISIT(traverse_module_state->__pyx_n_s__44);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__7);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__8);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_u_accuracy);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
@@ -3234,14 +3250,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_exit);
   Py_VISIT(traverse_module_state->__pyx_n_u_extracted_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_file);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_content);
   Py_VISIT(traverse_module_state->__pyx_n_u_file_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_file_path);
   Py_VISIT(traverse_module_state->__pyx_n_u_file_type);
+  Py_VISIT(traverse_module_state->__pyx_n_s_filename);
   Py_VISIT(traverse_module_state->__pyx_n_u_filename);
   Py_VISIT(traverse_module_state->__pyx_n_u_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_finalize);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_headers);
@@ -3340,16 +3357,17 @@
   Py_VISIT(traverse_module_state->__pyx_n_u_wildcard);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_CipherEncode);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decipherx);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Encapseal);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_GraphFEncode);
-  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_SaveToMongoDb);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_SignalSimilarity);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_TrainVector);
+  Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_UpdateVector);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_limitText);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorSearch);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeEmbed);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_vectorizeText);
   Py_VISIT(traverse_module_state->__pyx_kp_b_y1c8_8BxP9XN_VKM);
@@ -3357,50 +3375,53 @@
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_4);
   Py_VISIT(traverse_module_state->__pyx_int_200);
   Py_VISIT(traverse_module_state->__pyx_int_1000);
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
   Py_VISIT(traverse_module_state->__pyx_int_228825662);
   Py_VISIT(traverse_module_state->__pyx_int_238750788);
+  Py_VISIT(traverse_module_state->__pyx_slice__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
-  Py_VISIT(traverse_module_state->__pyx_tuple__12);
-  Py_VISIT(traverse_module_state->__pyx_tuple__14);
-  Py_VISIT(traverse_module_state->__pyx_tuple__16);
-  Py_VISIT(traverse_module_state->__pyx_tuple__18);
-  Py_VISIT(traverse_module_state->__pyx_tuple__20);
-  Py_VISIT(traverse_module_state->__pyx_tuple__22);
-  Py_VISIT(traverse_module_state->__pyx_tuple__24);
-  Py_VISIT(traverse_module_state->__pyx_tuple__26);
+  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_tuple__13);
+  Py_VISIT(traverse_module_state->__pyx_tuple__15);
+  Py_VISIT(traverse_module_state->__pyx_tuple__17);
+  Py_VISIT(traverse_module_state->__pyx_tuple__19);
+  Py_VISIT(traverse_module_state->__pyx_tuple__21);
+  Py_VISIT(traverse_module_state->__pyx_tuple__23);
+  Py_VISIT(traverse_module_state->__pyx_tuple__25);
   Py_VISIT(traverse_module_state->__pyx_tuple__27);
   Py_VISIT(traverse_module_state->__pyx_tuple__29);
-  Py_VISIT(traverse_module_state->__pyx_tuple__31);
-  Py_VISIT(traverse_module_state->__pyx_tuple__33);
-  Py_VISIT(traverse_module_state->__pyx_tuple__35);
-  Py_VISIT(traverse_module_state->__pyx_tuple__37);
-  Py_VISIT(traverse_module_state->__pyx_tuple__39);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__19);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
+  Py_VISIT(traverse_module_state->__pyx_tuple__30);
+  Py_VISIT(traverse_module_state->__pyx_tuple__32);
+  Py_VISIT(traverse_module_state->__pyx_tuple__34);
+  Py_VISIT(traverse_module_state->__pyx_tuple__36);
+  Py_VISIT(traverse_module_state->__pyx_tuple__38);
+  Py_VISIT(traverse_module_state->__pyx_tuple__40);
+  Py_VISIT(traverse_module_state->__pyx_tuple__42);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__18);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__22);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
   Py_VISIT(traverse_module_state->__pyx_codeobj__28);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__30);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__32);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__34);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__36);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__38);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__40);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__31);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__33);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__35);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__37);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__39);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__41);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__43);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3444,22 +3465,23 @@
 #define __pyx_kp_u_Error __pyx_mstate_global->__pyx_kp_u_Error
 #define __pyx_kp_u_Error_processing_response_JSON __pyx_mstate_global->__pyx_kp_u_Error_processing_response_JSON
 #define __pyx_n_s_GraphFEncode __pyx_mstate_global->__pyx_n_s_GraphFEncode
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_u_Invalid_API_key_provided __pyx_mstate_global->__pyx_kp_u_Invalid_API_key_provided
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
-#define __pyx_n_s_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_SaveToMongoDb
 #define __pyx_n_s_SignalSimilarity __pyx_mstate_global->__pyx_n_s_SignalSimilarity
-#define __pyx_kp_u_Successfully_save_to_the_databas __pyx_mstate_global->__pyx_kp_u_Successfully_save_to_the_databas
-#define __pyx_kp_u__11 __pyx_mstate_global->__pyx_kp_u__11
-#define __pyx_n_s__41 __pyx_mstate_global->__pyx_n_s__41
+#define __pyx_kp_u_Successfully_update_the_vector __pyx_mstate_global->__pyx_kp_u_Successfully_update_the_vector
+#define __pyx_n_s_TrainVector __pyx_mstate_global->__pyx_n_s_TrainVector
+#define __pyx_n_s_UpdateVector __pyx_mstate_global->__pyx_n_s_UpdateVector
+#define __pyx_kp_u__12 __pyx_mstate_global->__pyx_kp_u__12
+#define __pyx_n_s__44 __pyx_mstate_global->__pyx_n_s__44
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
-#define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
+#define __pyx_kp_u__8 __pyx_mstate_global->__pyx_kp_u__8
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_u_accuracy __pyx_mstate_global->__pyx_n_u_accuracy
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
 #define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
@@ -3522,14 +3544,15 @@
 #define __pyx_n_s_exit __pyx_mstate_global->__pyx_n_s_exit
 #define __pyx_n_u_extracted_text __pyx_mstate_global->__pyx_n_u_extracted_text
 #define __pyx_n_s_file __pyx_mstate_global->__pyx_n_s_file
 #define __pyx_n_s_file_content __pyx_mstate_global->__pyx_n_s_file_content
 #define __pyx_n_u_file_data __pyx_mstate_global->__pyx_n_u_file_data
 #define __pyx_n_s_file_path __pyx_mstate_global->__pyx_n_s_file_path
 #define __pyx_n_u_file_type __pyx_mstate_global->__pyx_n_u_file_type
+#define __pyx_n_s_filename __pyx_mstate_global->__pyx_n_s_filename
 #define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
 #define __pyx_n_u_filter __pyx_mstate_global->__pyx_n_u_filter
 #define __pyx_n_s_finalize __pyx_mstate_global->__pyx_n_s_finalize
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_headers __pyx_mstate_global->__pyx_n_s_headers
@@ -3628,16 +3651,17 @@
 #define __pyx_n_u_wildcard __pyx_mstate_global->__pyx_n_u_wildcard
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_CipherEncode __pyx_mstate_global->__pyx_n_s_xyellw_CipherEncode
 #define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
 #define __pyx_n_s_xyellw_Decipherx __pyx_mstate_global->__pyx_n_s_xyellw_Decipherx
 #define __pyx_n_s_xyellw_Encapseal __pyx_mstate_global->__pyx_n_s_xyellw_Encapseal
 #define __pyx_n_s_xyellw_GraphFEncode __pyx_mstate_global->__pyx_n_s_xyellw_GraphFEncode
-#define __pyx_n_s_xyellw_SaveToMongoDb __pyx_mstate_global->__pyx_n_s_xyellw_SaveToMongoDb
 #define __pyx_n_s_xyellw_SignalSimilarity __pyx_mstate_global->__pyx_n_s_xyellw_SignalSimilarity
+#define __pyx_n_s_xyellw_TrainVector __pyx_mstate_global->__pyx_n_s_xyellw_TrainVector
+#define __pyx_n_s_xyellw_UpdateVector __pyx_mstate_global->__pyx_n_s_xyellw_UpdateVector
 #define __pyx_n_s_xyellw___reduce_cython __pyx_mstate_global->__pyx_n_s_xyellw___reduce_cython
 #define __pyx_n_s_xyellw___setstate_cython __pyx_mstate_global->__pyx_n_s_xyellw___setstate_cython
 #define __pyx_n_s_xyellw_limitText __pyx_mstate_global->__pyx_n_s_xyellw_limitText
 #define __pyx_n_s_xyellw_vectorSearch __pyx_mstate_global->__pyx_n_s_xyellw_vectorSearch
 #define __pyx_n_s_xyellw_vectorizeEmbed __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeEmbed
 #define __pyx_n_s_xyellw_vectorizeText __pyx_mstate_global->__pyx_n_s_xyellw_vectorizeText
 #define __pyx_kp_b_y1c8_8BxP9XN_VKM __pyx_mstate_global->__pyx_kp_b_y1c8_8BxP9XN_VKM
@@ -3645,50 +3669,53 @@
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_4 __pyx_mstate_global->__pyx_int_4
 #define __pyx_int_200 __pyx_mstate_global->__pyx_int_200
 #define __pyx_int_1000 __pyx_mstate_global->__pyx_int_1000
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
 #define __pyx_int_228825662 __pyx_mstate_global->__pyx_int_228825662
 #define __pyx_int_238750788 __pyx_mstate_global->__pyx_int_238750788
+#define __pyx_slice__7 __pyx_mstate_global->__pyx_slice__7
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
-#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
-#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
-#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
-#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
-#define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
-#define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
-#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
-#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
-#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
+#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
+#define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
+#define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
+#define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
+#define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
+#define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
+#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
 #define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
 #define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
-#define __pyx_tuple__31 __pyx_mstate_global->__pyx_tuple__31
-#define __pyx_tuple__33 __pyx_mstate_global->__pyx_tuple__33
-#define __pyx_tuple__35 __pyx_mstate_global->__pyx_tuple__35
-#define __pyx_tuple__37 __pyx_mstate_global->__pyx_tuple__37
-#define __pyx_tuple__39 __pyx_mstate_global->__pyx_tuple__39
-#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
-#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
-#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
-#define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
-#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
-#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
-#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
+#define __pyx_tuple__30 __pyx_mstate_global->__pyx_tuple__30
+#define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
+#define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
+#define __pyx_tuple__36 __pyx_mstate_global->__pyx_tuple__36
+#define __pyx_tuple__38 __pyx_mstate_global->__pyx_tuple__38
+#define __pyx_tuple__40 __pyx_mstate_global->__pyx_tuple__40
+#define __pyx_tuple__42 __pyx_mstate_global->__pyx_tuple__42
+#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
+#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
+#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
+#define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
 #define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
-#define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
-#define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
-#define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
-#define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
-#define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
-#define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
+#define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
+#define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
+#define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
+#define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
+#define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
+#define __pyx_codeobj__41 __pyx_mstate_global->__pyx_codeobj__41
+#define __pyx_codeobj__43 __pyx_mstate_global->__pyx_codeobj__43
 /* #### Code section: module_code ### */
 
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -5655,23 +5682,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11UpdateVector(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11SaveToMongoDb = {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_11UpdateVector = {"UpdateVector", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11UpdateVector, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_11UpdateVector(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_collection = 0;
@@ -5685,15 +5712,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[5] = {0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("SaveToMongoDb (wrapper)", 0);
+  __Pyx_RefNannySetupContext("UpdateVector (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
@@ -5729,50 +5756,50 @@
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_database)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 1); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("UpdateVector", 1, 5, 5, 1); __PYX_ERR(0, 83, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_datasource)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 2); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("UpdateVector", 1, 5, 5, 2); __PYX_ERR(0, 83, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_enkyc)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 3); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("UpdateVector", 1, 5, 5, 3); __PYX_ERR(0, 83, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_params_dict)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, 4); __PYX_ERR(0, 83, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("UpdateVector", 1, 5, 5, 4); __PYX_ERR(0, 83, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SaveToMongoDb") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "UpdateVector") < 0)) __PYX_ERR(0, 83, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
@@ -5783,33 +5810,33 @@
     __pyx_v_database = ((PyObject*)values[1]);
     __pyx_v_datasource = ((PyObject*)values[2]);
     __pyx_v_enkyc = ((PyObject*)values[3]);
     __pyx_v_params_dict = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("SaveToMongoDb", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 83, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("UpdateVector", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 83, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.SaveToMongoDb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.UpdateVector", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_collection), (&PyUnicode_Type), 1, "collection", 1))) __PYX_ERR(0, 83, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_database), (&PyUnicode_Type), 1, "database", 1))) __PYX_ERR(0, 83, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_datasource), (&PyUnicode_Type), 1, "datasource", 1))) __PYX_ERR(0, 83, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_enkyc), (&PyUnicode_Type), 1, "enkyc", 1))) __PYX_ERR(0, 83, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc, __pyx_v_params_dict);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_10UpdateVector(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_collection, __pyx_v_database, __pyx_v_datasource, __pyx_v_enkyc, __pyx_v_params_dict);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -5818,15 +5845,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10UpdateVector(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict) {
   PyObject *__pyx_v_decrypted_url = NULL;
   PyObject *__pyx_v_payload = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -5835,15 +5862,15 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("SaveToMongoDb", 1);
+  __Pyx_RefNannySetupContext("UpdateVector", 1);
 
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
@@ -5968,16 +5995,16 @@
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_3, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_7) {
 
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_kp_u_Successfully_save_to_the_databas);
-    __pyx_r = __pyx_kp_u_Successfully_save_to_the_databas;
+    __Pyx_INCREF(__pyx_kp_u_Successfully_update_the_vector);
+    __pyx_r = __pyx_kp_u_Successfully_update_the_vector;
     goto __pyx_L0;
 
   }
 
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
@@ -5995,37 +6022,432 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.SaveToMongoDb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.UpdateVector", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_decrypted_url);
   __Pyx_XDECREF(__pyx_v_payload);
   __Pyx_XDECREF(__pyx_v_headers);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13limitText(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13TrainVector(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13limitText = {"limitText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13limitText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13limitText(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_13TrainVector = {"TrainVector", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13TrainVector, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_13TrainVector(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_connParam = 0;
+  PyObject *__pyx_v_filename = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[2] = {0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("TrainVector (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_connParam,&__pyx_n_s_filename,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_connParam)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_filename)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("TrainVector", 1, 2, 2, 1); __PYX_ERR(0, 115, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "TrainVector") < 0)) __PYX_ERR(0, 115, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 2)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+    }
+    __pyx_v_connParam = values[0];
+    __pyx_v_filename = ((PyObject*)values[1]);
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("TrainVector", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 115, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.TrainVector", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_filename), (&PyUnicode_Type), 1, "filename", 1))) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12TrainVector(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_filename);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12TrainVector(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_filename) {
+  PyObject *__pyx_v_url = NULL;
+  PyObject *__pyx_v_headers = NULL;
+  PyObject *__pyx_v_pipeline = NULL;
+  PyObject *__pyx_v_query_payload = NULL;
+  PyObject *__pyx_v_response = NULL;
+  PyObject *__pyx_v_response_data = NULL;
+  PyObject *__pyx_v_documents = NULL;
+  PyObject *__pyx_v_doc = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  PyObject *(*__pyx_t_7)(PyObject *);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("TrainVector", 1);
+
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_v_url = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_enkyc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_t_2) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_headers = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_index, __pyx_t_3) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_v_filename) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_wildcard, __pyx_kp_u__6) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_path, __pyx_t_5) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_3) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_search, __pyx_t_2) < 0) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filename, __pyx_int_1) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_project, __pyx_t_3) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_int_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 2, __pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 0;
+  __pyx_v_pipeline = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
+
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_database, __pyx_t_3) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_v_query_payload = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
+
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_requests); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_post); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_INCREF(__pyx_v_url);
+  __Pyx_GIVEREF(__pyx_v_url);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_url)) __PYX_ERR(0, 155, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_response = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = NULL;
+  __pyx_t_4 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_v_response_data = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_response_data, __pyx_n_u_documents); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_documents = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_documents, 0, 1, NULL, NULL, &__pyx_slice__7, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
+    __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_6 = 0;
+    __pyx_t_7 = NULL;
+  } else {
+    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  for (;;) {
+    if (likely(!__pyx_t_7)) {
+      if (likely(PyList_CheckExact(__pyx_t_2))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_1); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+        #else
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        #endif
+      }
+    } else {
+      __pyx_t_1 = __pyx_t_7(__pyx_t_2);
+      if (unlikely(!__pyx_t_1)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 160, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_1);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_1);
+    __pyx_t_1 = 0;
+
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_v_doc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("aixhello.xyello.xyellw.TrainVector", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_url);
+  __Pyx_XDECREF(__pyx_v_headers);
+  __Pyx_XDECREF(__pyx_v_pipeline);
+  __Pyx_XDECREF(__pyx_v_query_payload);
+  __Pyx_XDECREF(__pyx_v_response);
+  __Pyx_XDECREF(__pyx_v_response_data);
+  __Pyx_XDECREF(__pyx_v_documents);
+  __Pyx_XDECREF(__pyx_v_doc);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15limitText(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_15limitText = {"limitText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15limitText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15limitText(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_text = 0;
@@ -6065,27 +6487,27 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_length);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 115, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "limitText") < 0)) __PYX_ERR(0, 115, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "limitText") < 0)) __PYX_ERR(0, 163, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
@@ -6093,30 +6515,30 @@
       }
     }
     __pyx_v_text = ((PyObject*)values[0]);
     __pyx_v_max_length = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("limitText", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 115, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("limitText", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 163, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.limitText", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 115, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_12limitText(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text, __pyx_v_max_length);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_14limitText(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text, __pyx_v_max_length);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -6125,58 +6547,58 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12limitText(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14limitText(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("limitText", 1);
 
   if (unlikely(__pyx_v_text == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 116, __pyx_L1_error)
+    __PYX_ERR(0, 164, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_text); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 116, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_text); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_v_max_length, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_v_max_length, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_4) {
 
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_text == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 117, __pyx_L1_error)
+      __PYX_ERR(0, 165, __pyx_L1_error)
     }
     __Pyx_INCREF(__pyx_v_max_length);
     __pyx_t_3 = __pyx_v_max_length;
     __pyx_t_4 = (__pyx_t_3 == Py_None);
     if (__pyx_t_4) {
       __pyx_t_1 = PY_SSIZE_T_MAX;
     } else {
-      __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 117, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 165, __pyx_L1_error)
       __pyx_t_1 = __pyx_t_5;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyUnicode_Substring(__pyx_v_text, 0, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Substring(__pyx_v_text, 0, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_3, __pyx_kp_u__7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_3, __pyx_kp_u__8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
   }
@@ -6197,23 +6619,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15GraphFEncode(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17GraphFEncode(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_15GraphFEncode = {"GraphFEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15GraphFEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_15GraphFEncode(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_17GraphFEncode = {"GraphFEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17GraphFEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17GraphFEncode(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_file_path = 0;
@@ -6249,46 +6671,46 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_file_path)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GraphFEncode") < 0)) __PYX_ERR(0, 120, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "GraphFEncode") < 0)) __PYX_ERR(0, 168, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_file_path = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("GraphFEncode", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 120, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("GraphFEncode", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 168, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.GraphFEncode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_file_path), (&PyUnicode_Type), 1, "file_path", 1))) __PYX_ERR(0, 120, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_14GraphFEncode(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_file_path);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_file_path), (&PyUnicode_Type), 1, "file_path", 1))) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_16GraphFEncode(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_file_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -6297,15 +6719,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14GraphFEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_file_path) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16GraphFEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_file_path) {
   PyObject *__pyx_v_file = NULL;
   PyObject *__pyx_v_file_content = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -6320,28 +6742,28 @@
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("GraphFEncode", 1);
 
   /*with:*/ {
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_file_path);
     __Pyx_GIVEREF(__pyx_v_file_path);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_file_path)) __PYX_ERR(0, 121, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_file_path)) __PYX_ERR(0, 169, __pyx_L1_error);
     __Pyx_INCREF(__pyx_n_u_rb);
     __Pyx_GIVEREF(__pyx_n_u_rb);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_rb)) __PYX_ERR(0, 121, __pyx_L1_error);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_n_u_rb)) __PYX_ERR(0, 169, __pyx_L1_error);
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_open, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_exit); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L3_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_2, __pyx_n_s_enter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -6353,15 +6775,15 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L3_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_t_4 = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     /*try:*/ {
@@ -6372,15 +6794,15 @@
         __Pyx_XGOTREF(__pyx_t_7);
         __Pyx_XGOTREF(__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_9);
         /*try:*/ {
           __pyx_v_file = __pyx_t_4;
           __pyx_t_4 = 0;
 
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L7_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_file, __pyx_n_s_read); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_1 = NULL;
           __pyx_t_6 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_2))) {
             __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
             if (likely(__pyx_t_1)) {
@@ -6392,25 +6814,25 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_1, NULL};
             __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L7_error)
+            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 170, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           }
           __pyx_v_file_content = __pyx_t_4;
           __pyx_t_4 = 0;
 
           __Pyx_XDECREF(__pyx_r);
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_base64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L7_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_base64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L7_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 171, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_1 = NULL;
           __pyx_t_6 = 0;
           #if CYTHON_UNPACK_METHODS
           if (unlikely(PyMethod_Check(__pyx_t_5))) {
             __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
@@ -6423,19 +6845,19 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_v_file_content};
             __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L7_error)
+            if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L7_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 171, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_t_2 = NULL;
           __pyx_t_6 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_5))) {
             __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -6448,15 +6870,15 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_u_utf_8};
             __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
             __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L7_error)
+            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_4);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
           __pyx_r = __pyx_t_4;
           __pyx_t_4 = 0;
           goto __pyx_L11_try_return;
 
@@ -6464,36 +6886,36 @@
         __pyx_L7_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("aixhello.xyello.xyellw.GraphFEncode", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_2) < 0) __PYX_ERR(0, 121, __pyx_L9_except_error)
+          if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_2) < 0) __PYX_ERR(0, 169, __pyx_L9_except_error)
           __Pyx_XGOTREF(__pyx_t_4);
           __Pyx_XGOTREF(__pyx_t_5);
           __Pyx_XGOTREF(__pyx_t_2);
-          __pyx_t_1 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L9_except_error)
+          __pyx_t_1 = PyTuple_Pack(3, __pyx_t_4, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 121, __pyx_L9_except_error)
+          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 169, __pyx_L9_except_error)
           __Pyx_GOTREF(__pyx_t_10);
           __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (__pyx_t_11 < 0) __PYX_ERR(0, 121, __pyx_L9_except_error)
+          if (__pyx_t_11 < 0) __PYX_ERR(0, 169, __pyx_L9_except_error)
           __pyx_t_12 = (!__pyx_t_11);
           if (unlikely(__pyx_t_12)) {
             __Pyx_GIVEREF(__pyx_t_4);
             __Pyx_GIVEREF(__pyx_t_5);
             __Pyx_XGIVEREF(__pyx_t_2);
             __Pyx_ErrRestoreWithState(__pyx_t_4, __pyx_t_5, __pyx_t_2);
             __pyx_t_4 = 0; __pyx_t_5 = 0; __pyx_t_2 = 0; 
-            __PYX_ERR(0, 121, __pyx_L9_except_error)
+            __PYX_ERR(0, 169, __pyx_L9_except_error)
           }
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
           goto __pyx_L8_exception_handled;
         }
         __pyx_L9_except_error:;
@@ -6514,29 +6936,29 @@
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
-          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, NULL);
+          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__9, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 121, __pyx_L1_error)
+          if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 169, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L4_return: {
         __pyx_t_9 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_3) {
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, NULL);
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__9, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 121, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 169, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __pyx_r = __pyx_t_9;
         __pyx_t_9 = 0;
         goto __pyx_L0;
       }
@@ -6566,23 +6988,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17CipherEncode(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19CipherEncode(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_17CipherEncode = {"CipherEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17CipherEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_17CipherEncode(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_19CipherEncode = {"CipherEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19CipherEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19CipherEncode(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_text = 0;
@@ -6618,46 +7040,46 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "CipherEncode") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "CipherEncode") < 0)) __PYX_ERR(0, 173, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_text = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("CipherEncode", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 125, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("CipherEncode", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 173, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.CipherEncode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 125, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_16CipherEncode(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text), (&PyUnicode_Type), 1, "text", 1))) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_18CipherEncode(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_text);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -6666,15 +7088,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16CipherEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18CipherEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text) {
   PyObject *__pyx_v_input_bytes = NULL;
   PyObject *__pyx_v_encoded_bytes = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -6682,24 +7104,24 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("CipherEncode", 1);
 
   if (unlikely(__pyx_v_text == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 126, __pyx_L1_error)
+    __PYX_ERR(0, 174, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_text); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_input_bytes = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_base64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_b64encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6712,15 +7134,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_v_input_bytes};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_encoded_bytes = __pyx_t_1;
   __pyx_t_1 = 0;
 
   __Pyx_XDECREF(__pyx_r);
@@ -6742,23 +7164,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19SignalSimilarity(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_21SignalSimilarity(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_19SignalSimilarity = {"SignalSimilarity", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19SignalSimilarity, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_19SignalSimilarity(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_21SignalSimilarity = {"SignalSimilarity", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_21SignalSimilarity, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_21SignalSimilarity(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_a = 0;
@@ -6797,87 +7219,87 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_a)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_b)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 130, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("SignalSimilarity", 1, 2, 2, 1); __PYX_ERR(0, 130, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("SignalSimilarity", 1, 2, 2, 1); __PYX_ERR(0, 178, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SignalSimilarity") < 0)) __PYX_ERR(0, 130, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "SignalSimilarity") < 0)) __PYX_ERR(0, 178, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_a = values[0];
     __pyx_v_b = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("SignalSimilarity", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 130, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("SignalSimilarity", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 178, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.SignalSimilarity", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_18SignalSimilarity(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_20SignalSimilarity(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18SignalSimilarity(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_20SignalSimilarity(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("SignalSimilarity", 1);
 
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dot); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -6890,24 +7312,24 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_2, __pyx_v_a, __pyx_v_b};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_linalg); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_linalg); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_norm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_norm); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
@@ -6920,24 +7342,24 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_a};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_linalg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_linalg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_norm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_norm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -6950,23 +7372,23 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_v_b};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyNumber_Multiply(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Multiply(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
@@ -6984,23 +7406,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_21vectorSearch(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_23vectorSearch(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_21vectorSearch = {"vectorSearch", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_21vectorSearch, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_21vectorSearch(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_23vectorSearch = {"vectorSearch", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_23vectorSearch, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_23vectorSearch(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_connParam = 0;
@@ -7048,94 +7470,94 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_connParam)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_result_length)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 1); __PYX_ERR(0, 133, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 1); __PYX_ERR(0, 181, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vector_query)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 2); __PYX_ERR(0, 133, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 2); __PYX_ERR(0, 181, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_query)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 3); __PYX_ERR(0, 133, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 3); __PYX_ERR(0, 181, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_top_n)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 4); __PYX_ERR(0, 133, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, 4); __PYX_ERR(0, 181, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vectorSearch") < 0)) __PYX_ERR(0, 133, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vectorSearch") < 0)) __PYX_ERR(0, 181, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
     }
     __pyx_v_connParam = values[0];
-    __pyx_v_result_length = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_result_length == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+    __pyx_v_result_length = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_result_length == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
     __pyx_v_vector_query = values[2];
     __pyx_v_text_query = ((PyObject*)values[3]);
-    __pyx_v_top_n = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_top_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L3_error)
+    __pyx_v_top_n = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_top_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 133, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vectorSearch", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 181, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_query), (&PyUnicode_Type), 1, "text_query", 1))) __PYX_ERR(0, 133, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_20vectorSearch(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_result_length, __pyx_v_vector_query, __pyx_v_text_query, __pyx_v_top_n);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_query), (&PyUnicode_Type), 1, "text_query", 1))) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_22vectorSearch(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_result_length, __pyx_v_vector_query, __pyx_v_text_query, __pyx_v_top_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -7144,15 +7566,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_20vectorSearch(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, CYTHON_UNUSED PyObject *__pyx_v_vector_query, PyObject *__pyx_v_text_query, int __pyx_v_top_n) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_22vectorSearch(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, CYTHON_UNUSED PyObject *__pyx_v_vector_query, PyObject *__pyx_v_text_query, int __pyx_v_top_n) {
   PyObject *__pyx_v_url = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_pipeline = NULL;
   PyObject *__pyx_v_query_payload = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_response_data = NULL;
   PyObject *__pyx_v_documents = NULL;
@@ -7186,15 +7608,15 @@
   PyObject *__pyx_t_22 = NULL;
   PyObject *__pyx_t_23 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vectorSearch", 1);
 
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -7206,154 +7628,154 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_url = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Content_Type, __pyx_kp_u_application_json) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_Access_Control_Request_Headers, __pyx_kp_u__6) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
 
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_enkyc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_enkyc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_t_2) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_api_key_2, __pyx_t_2) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_index, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_index, __pyx_t_3) < 0) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_v_text_query) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_v_text_query) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_wildcard, __pyx_kp_u__6) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_path, __pyx_t_5) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_wildcard, __pyx_kp_u__6) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_path, __pyx_t_5) < 0) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_3) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_3) < 0) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_search, __pyx_t_2) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_search, __pyx_t_2) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filename, __pyx_int_1) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_extracted_text, __pyx_int_1) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_text_embeddings, __pyx_int_1) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filename, __pyx_int_1) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_extracted_text, __pyx_int_1) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_text_embeddings, __pyx_int_1) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_meta, __pyx_n_u_searchScore) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_score, __pyx_t_5) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_meta, __pyx_n_u_searchScore) < 0) __PYX_ERR(0, 208, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_score, __pyx_t_5) < 0) __PYX_ERR(0, 205, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_project, __pyx_t_3) < 0) __PYX_ERR(0, 156, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_project, __pyx_t_3) < 0) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_top_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_top_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_t_5) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_t_5) < 0) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 1, __pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 2, __pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 2, __pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_v_pipeline = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_database, __pyx_t_3) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_database, __pyx_t_3) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
   __pyx_v_query_payload = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_requests); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_requests); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_post); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_post); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_url);
   __Pyx_GIVEREF(__pyx_v_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_url)) __PYX_ERR(0, 176, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_url)) __PYX_ERR(0, 224, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_response = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_6) {
 
     {
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_8);
       __Pyx_XGOTREF(__pyx_t_9);
       /*try:*/ {
 
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L4_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 228, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_5 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_5)) {
@@ -7365,24 +7787,24 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L4_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         }
         __pyx_v_response_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L4_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L4_error)
+        __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
         __pyx_t_3 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_3)) {
@@ -7395,87 +7817,87 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_n_u_documents, __pyx_t_5};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L4_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         }
         __pyx_v_documents = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L4_error)
+        __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_results = ((PyObject*)__pyx_t_1);
         __pyx_t_1 = 0;
 
-        __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_documents, 0, __pyx_v_top_n, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_documents, 0, __pyx_v_top_n, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
           __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
           __pyx_t_10 = 0;
           __pyx_t_11 = NULL;
         } else {
-          __pyx_t_10 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L4_error)
+          __pyx_t_10 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 185, __pyx_L4_error)
+          __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 233, __pyx_L4_error)
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         for (;;) {
           if (likely(!__pyx_t_11)) {
             if (likely(PyList_CheckExact(__pyx_t_2))) {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 185, __pyx_L4_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 233, __pyx_L4_error)
                 #endif
                 if (__pyx_t_10 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 185, __pyx_L4_error)
+              __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 233, __pyx_L4_error)
               #else
-              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L4_error)
+              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L4_error)
               __Pyx_GOTREF(__pyx_t_1);
               #endif
             } else {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 185, __pyx_L4_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 233, __pyx_L4_error)
                 #endif
                 if (__pyx_t_10 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 185, __pyx_L4_error)
+              __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 233, __pyx_L4_error)
               #else
-              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L4_error)
+              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L4_error)
               __Pyx_GOTREF(__pyx_t_1);
               #endif
             }
           } else {
             __pyx_t_1 = __pyx_t_11(__pyx_t_2);
             if (unlikely(!__pyx_t_1)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 185, __pyx_L4_error)
+                else __PYX_ERR(0, 233, __pyx_L4_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_1);
           }
           __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CipherEncode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CipherEncode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_12 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_5))) {
             __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_5);
             if (likely(__pyx_t_12)) {
@@ -7488,70 +7910,70 @@
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_3};
             __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L4_error)
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L4_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
           __Pyx_XDECREF_SET(__pyx_v_encodeText, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_v_encodeText) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_v_encodeText) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
 
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_5) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_5) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_3) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_3) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 187, __pyx_L4_error)
+          __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 235, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
         __Pyx_XDECREF(__pyx_r);
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L4_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L4_error)
+        __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_v_results);
         __Pyx_GIVEREF(__pyx_v_results);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 194, __pyx_L4_error);
-        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L4_error)
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 242, __pyx_L4_error);
+        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 194, __pyx_L4_error)
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 194, __pyx_L4_error)
+        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 242, __pyx_L4_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_5;
         __pyx_t_5 = 0;
         goto __pyx_L8_try_return;
@@ -7563,49 +7985,49 @@
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
       __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_4) {
         __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 195, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 243, __pyx_L6_except_error)
         __Pyx_XGOTREF(__pyx_t_5);
         __Pyx_XGOTREF(__pyx_t_3);
         __Pyx_XGOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __pyx_v_e = __pyx_t_3;
         /*try:*/ {
 
-          __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 244, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
           __Pyx_XDECREF(__pyx_r);
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 197, __pyx_L18_error)
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error)
+          __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 197, __pyx_L18_error)
+          __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_14);
           __Pyx_GIVEREF(__pyx_t_1);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error);
           __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 197, __pyx_L18_error)
-          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 197, __pyx_L18_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 245, __pyx_L18_error)
+          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_r = __pyx_t_15;
           __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -7681,44 +8103,44 @@
       __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       goto __pyx_L0;
     }
 
   }
 
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
-    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 200, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_15;
     __pyx_t_15 = 0;
     goto __pyx_L0;
@@ -7751,23 +8173,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_23__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_25__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_23__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_23__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_23__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_25__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_25__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_25__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -7784,22 +8206,22 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_22__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_24__reduce_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_22__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_24__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -7917,23 +8339,23 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_25__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_27__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_25__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_25__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_25__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_8aixhello_6xyello_6xyellw_27__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_27__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_27__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -7999,28 +8421,28 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_24__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_26__setstate_cython__(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_24__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_26__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 1);
@@ -8184,15 +8606,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_xyellw", 1);
 
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__10, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__11, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
@@ -8400,22 +8822,23 @@
 
 static PyMethodDef __pyx_methods_8aixhello_6xyello_xyellw[] = {
   {"Decipherx", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Encapseal", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"Decenigma", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"vectorizeEmbed", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {"vectorizeText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"SaveToMongoDb", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"limitText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13limitText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"GraphFEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15GraphFEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"CipherEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17CipherEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"SignalSimilarity", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19SignalSimilarity, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"vectorSearch", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_21vectorSearch, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_23__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_25__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"UpdateVector", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_11UpdateVector, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"TrainVector", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_13TrainVector, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"limitText", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_15limitText, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"GraphFEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_17GraphFEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"CipherEncode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_19CipherEncode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"SignalSimilarity", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_21SignalSimilarity, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"vectorSearch", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_23vectorSearch, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_25__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8aixhello_6xyello_6xyellw_27__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_8aixhello_6xyello_xyellw_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8aixhello_6xyello_xyellw},
   {Py_tp_methods, (void *)__pyx_methods_8aixhello_6xyello_xyellw},
   {Py_tp_new, (void *)__pyx_tp_new_8aixhello_6xyello_xyellw},
@@ -8543,22 +8966,23 @@
     {&__pyx_kp_u_Error, __pyx_k_Error, sizeof(__pyx_k_Error), 0, 1, 0, 0},
     {&__pyx_kp_u_Error_processing_response_JSON, __pyx_k_Error_processing_response_JSON, sizeof(__pyx_k_Error_processing_response_JSON), 0, 1, 0, 0},
     {&__pyx_n_s_GraphFEncode, __pyx_k_GraphFEncode, sizeof(__pyx_k_GraphFEncode), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_u_Invalid_API_key_provided, __pyx_k_Invalid_API_key_provided, sizeof(__pyx_k_Invalid_API_key_provided), 0, 1, 0, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-    {&__pyx_n_s_SaveToMongoDb, __pyx_k_SaveToMongoDb, sizeof(__pyx_k_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_n_s_SignalSimilarity, __pyx_k_SignalSimilarity, sizeof(__pyx_k_SignalSimilarity), 0, 0, 1, 1},
-    {&__pyx_kp_u_Successfully_save_to_the_databas, __pyx_k_Successfully_save_to_the_databas, sizeof(__pyx_k_Successfully_save_to_the_databas), 0, 1, 0, 0},
-    {&__pyx_kp_u__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 1, 0, 0},
-    {&__pyx_n_s__41, __pyx_k__41, sizeof(__pyx_k__41), 0, 0, 1, 1},
+    {&__pyx_kp_u_Successfully_update_the_vector, __pyx_k_Successfully_update_the_vector, sizeof(__pyx_k_Successfully_update_the_vector), 0, 1, 0, 0},
+    {&__pyx_n_s_TrainVector, __pyx_k_TrainVector, sizeof(__pyx_k_TrainVector), 0, 0, 1, 1},
+    {&__pyx_n_s_UpdateVector, __pyx_k_UpdateVector, sizeof(__pyx_k_UpdateVector), 0, 0, 1, 1},
+    {&__pyx_kp_u__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 1, 0, 0},
+    {&__pyx_n_s__44, __pyx_k__44, sizeof(__pyx_k__44), 0, 0, 1, 1},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
-    {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
+    {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_u_accuracy, __pyx_k_accuracy, sizeof(__pyx_k_accuracy), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
     {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
@@ -8621,14 +9045,15 @@
     {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
     {&__pyx_n_u_extracted_text, __pyx_k_extracted_text, sizeof(__pyx_k_extracted_text), 0, 1, 0, 1},
     {&__pyx_n_s_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 0, 1, 1},
     {&__pyx_n_s_file_content, __pyx_k_file_content, sizeof(__pyx_k_file_content), 0, 0, 1, 1},
     {&__pyx_n_u_file_data, __pyx_k_file_data, sizeof(__pyx_k_file_data), 0, 1, 0, 1},
     {&__pyx_n_s_file_path, __pyx_k_file_path, sizeof(__pyx_k_file_path), 0, 0, 1, 1},
     {&__pyx_n_u_file_type, __pyx_k_file_type, sizeof(__pyx_k_file_type), 0, 1, 0, 1},
+    {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
     {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
     {&__pyx_n_u_filter, __pyx_k_filter, sizeof(__pyx_k_filter), 0, 1, 0, 1},
     {&__pyx_n_s_finalize, __pyx_k_finalize, sizeof(__pyx_k_finalize), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_headers, __pyx_k_headers, sizeof(__pyx_k_headers), 0, 0, 1, 1},
@@ -8727,32 +9152,33 @@
     {&__pyx_n_u_wildcard, __pyx_k_wildcard, sizeof(__pyx_k_wildcard), 0, 1, 0, 1},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_CipherEncode, __pyx_k_xyellw_CipherEncode, sizeof(__pyx_k_xyellw_CipherEncode), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decipherx, __pyx_k_xyellw_Decipherx, sizeof(__pyx_k_xyellw_Decipherx), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Encapseal, __pyx_k_xyellw_Encapseal, sizeof(__pyx_k_xyellw_Encapseal), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_GraphFEncode, __pyx_k_xyellw_GraphFEncode, sizeof(__pyx_k_xyellw_GraphFEncode), 0, 0, 1, 1},
-    {&__pyx_n_s_xyellw_SaveToMongoDb, __pyx_k_xyellw_SaveToMongoDb, sizeof(__pyx_k_xyellw_SaveToMongoDb), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_SignalSimilarity, __pyx_k_xyellw_SignalSimilarity, sizeof(__pyx_k_xyellw_SignalSimilarity), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_TrainVector, __pyx_k_xyellw_TrainVector, sizeof(__pyx_k_xyellw_TrainVector), 0, 0, 1, 1},
+    {&__pyx_n_s_xyellw_UpdateVector, __pyx_k_xyellw_UpdateVector, sizeof(__pyx_k_xyellw_UpdateVector), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___reduce_cython, __pyx_k_xyellw___reduce_cython, sizeof(__pyx_k_xyellw___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw___setstate_cython, __pyx_k_xyellw___setstate_cython, sizeof(__pyx_k_xyellw___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_limitText, __pyx_k_xyellw_limitText, sizeof(__pyx_k_xyellw_limitText), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_vectorSearch, __pyx_k_xyellw_vectorSearch, sizeof(__pyx_k_xyellw_vectorSearch), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_vectorizeEmbed, __pyx_k_xyellw_vectorizeEmbed, sizeof(__pyx_k_xyellw_vectorizeEmbed), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_vectorizeText, __pyx_k_xyellw_vectorizeText, sizeof(__pyx_k_xyellw_vectorizeText), 0, 0, 1, 1},
     {&__pyx_kp_b_y1c8_8BxP9XN_VKM, __pyx_k_y1c8_8BxP9XN_VKM, sizeof(__pyx_k_y1c8_8BxP9XN_VKM), 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 121, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 169, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -8771,98 +9197,107 @@
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  __pyx_tuple__8 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_slice__7 = PySlice_New(Py_None, __pyx_int_1, Py_None); if (unlikely(!__pyx_slice__7)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__7);
+  __Pyx_GIVEREF(__pyx_slice__7);
 
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 239, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 13, __pyx_L1_error)
-
-  __pyx_tuple__14 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 20, __pyx_L1_error)
-
-  __pyx_tuple__16 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 35, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 35, __pyx_L1_error)
-
-  __pyx_tuple__18 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbed, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 52, __pyx_L1_error)
-
-  __pyx_tuple__20 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 69, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 69, __pyx_L1_error)
-
-  __pyx_tuple__22 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 83, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SaveToMongoDb, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 83, __pyx_L1_error)
-
-  __pyx_tuple__24 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_max_length); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_limitText, 115, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_int_1000); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__11 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+
+  __pyx_tuple__13 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 13, __pyx_L1_error)
+
+  __pyx_tuple__15 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 20, __pyx_L1_error)
+
+  __pyx_tuple__17 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 35, __pyx_L1_error)
+
+  __pyx_tuple__19 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbed, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 52, __pyx_L1_error)
+
+  __pyx_tuple__21 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 69, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 69, __pyx_L1_error)
+
+  __pyx_tuple__23 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_UpdateVector, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 83, __pyx_L1_error)
+
+  __pyx_tuple__25 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_filename, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_doc); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_TrainVector, 115, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 115, __pyx_L1_error)
 
-  __pyx_tuple__27 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_file_path, __pyx_n_s_file, __pyx_n_s_file_content); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_max_length); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_GraphFEncode, 120, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 120, __pyx_L1_error)
-
-  __pyx_tuple__29 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_input_bytes, __pyx_n_s_encoded_bytes); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_limitText, 163, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_int_1000); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_CipherEncode, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 125, __pyx_L1_error)
 
-  __pyx_tuple__31 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 130, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SignalSimilarity, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 130, __pyx_L1_error)
-
-  __pyx_tuple__33 = PyTuple_Pack(17, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_vector_query, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_encodeText, __pyx_n_s_e); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorSearch, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 133, __pyx_L1_error)
-
-  __pyx_tuple__35 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 1, __pyx_L1_error)
-
-  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(1, 16, __pyx_L1_error)
-
-  __pyx_tuple__39 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_file_path, __pyx_n_s_file, __pyx_n_s_file_content); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_GraphFEncode, 168, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 168, __pyx_L1_error)
+
+  __pyx_tuple__32 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_input_bytes, __pyx_n_s_encoded_bytes); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_CipherEncode, 173, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 173, __pyx_L1_error)
+
+  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SignalSimilarity, 178, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 178, __pyx_L1_error)
+
+  __pyx_tuple__36 = PyTuple_Pack(17, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_vector_query, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_encodeText, __pyx_n_s_e); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorSearch, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 181, __pyx_L1_error)
+
+  __pyx_tuple__38 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  __pyx_tuple__40 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(1, 16, __pyx_L1_error)
+
+  __pyx_tuple__42 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
+  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -9333,94 +9768,100 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_base64, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_base64, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbed, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbed, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeEmbed, __pyx_t_2) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeText, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11SaveToMongoDb, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SaveToMongoDb, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11UpdateVector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_UpdateVector, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SaveToMongoDb, __pyx_t_2) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_UpdateVector, __pyx_t_2) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13limitText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_limitText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13TrainVector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_TrainVector, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__26);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_limitText, __pyx_t_2) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_TrainVector, __pyx_t_2) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_15GraphFEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_GraphFEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_15limitText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_limitText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_GraphFEncode, __pyx_t_2) < 0) __PYX_ERR(0, 120, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__29);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_limitText, __pyx_t_2) < 0) __PYX_ERR(0, 163, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_17CipherEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_CipherEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_17GraphFEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_GraphFEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_CipherEncode, __pyx_t_2) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_GraphFEncode, __pyx_t_2) < 0) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_19SignalSimilarity, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SignalSimilarity, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_19CipherEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_CipherEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SignalSimilarity, __pyx_t_2) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_CipherEncode, __pyx_t_2) < 0) __PYX_ERR(0, 173, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_21vectorSearch, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorSearch, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_21SignalSimilarity, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SignalSimilarity, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorSearch, __pyx_t_2) < 0) __PYX_ERR(0, 133, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SignalSimilarity, __pyx_t_2) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_23__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_23vectorSearch, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorSearch, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorSearch, __pyx_t_2) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
+
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_25__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_25__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_27__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_xyellw, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -11063,14 +11504,38 @@
 #endif
         return ((double)a == (double)b);
     }
     return __Pyx_PyObject_IsTrueAndDecref(
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
+/* DictGetItem */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
+    PyObject *value;
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (!PyErr_Occurred()) {
+            if (unlikely(PyTuple_Check(key))) {
+                PyObject* args = PyTuple_Pack(1, key);
+                if (likely(args)) {
+                    PyErr_SetObject(PyExc_KeyError, args);
+                    Py_DECREF(args);
+                }
+            } else {
+                PyErr_SetObject(PyExc_KeyError, key);
+            }
+        }
+        return NULL;
+    }
+    Py_INCREF(value);
+    return value;
+}
+#endif
+
 /* PyUnicode_Substring */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Substring(
             PyObject* text, Py_ssize_t start, Py_ssize_t stop) {
     Py_ssize_t length;
     if (unlikely(__Pyx_PyUnicode_READY(text) == -1)) return NULL;
     length = __Pyx_PyUnicode_GET_LENGTH(text);
     if (start < 0) {
@@ -11178,38 +11643,14 @@
     } else if (with_error) {
         PyErr_SetObject(PyExc_AttributeError, attr_name);
     }
     return res;
 }
 #endif
 
-/* DictGetItem */
-#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
-static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
-    PyObject *value;
-    value = PyDict_GetItemWithError(d, key);
-    if (unlikely(!value)) {
-        if (!PyErr_Occurred()) {
-            if (unlikely(PyTuple_Check(key))) {
-                PyObject* args = PyTuple_Pack(1, key);
-                if (likely(args)) {
-                    PyErr_SetObject(PyExc_KeyError, args);
-                    Py_DECREF(args);
-                }
-            } else {
-                PyErr_SetObject(PyExc_KeyError, key);
-            }
-        }
-        return NULL;
-    }
-    Py_INCREF(value);
-    return value;
-}
-#endif
-
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
     PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
@@ -11390,15 +11831,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__11);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__12);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -14468,15 +14909,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__41);
+        name = __Pyx_NewRef(__pyx_n_s__44);
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
 static unsigned long __Pyx_get_runtime_version(void) {
```

### Comparing `aixhello-4.5/aixhello.egg-info/PKG-INFO` & `aixhello-4.7/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.5
+Version: 4.7
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.5/setup.py` & `aixhello-4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='4.5',  
+    version='4.7',  
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

