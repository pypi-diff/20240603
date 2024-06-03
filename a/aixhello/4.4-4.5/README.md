# Comparing `tmp/aixhello-4.4.tar.gz` & `tmp/aixhello-4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-4.4.tar", last modified: Mon Jun  3 09:00:34 2024, max compression
+gzip compressed data, was "aixhello-4.5.tar", last modified: Mon Jun  3 09:07:28 2024, max compression
```

## Comparing `aixhello-4.4.tar` & `aixhello-4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 09:00:34.810120 aixhello-4.4/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.4/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-03 09:00:34.809171 aixhello-4.4/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 09:00:34.787118 aixhello-4.4/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.4/aixhello/__init__.py
--rw-rw-rw-   0        0        0   621282 2024-06-03 09:00:23.000000 aixhello-4.4/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-03 09:00:34.808119 aixhello-4.4/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 09:00:34.817113 aixhello-4.4/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-06-03 08:59:56.000000 aixhello-4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:07:28.349137 aixhello-4.5/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.5/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-03 09:07:28.348135 aixhello-4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 09:07:28.323150 aixhello-4.5/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.5/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   621516 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-03 09:07:28.347136 aixhello-4.5/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 09:07:28.000000 aixhello-4.5/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 09:07:28.353143 aixhello-4.5/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-06-03 09:06:53.000000 aixhello-4.5/setup.py
```

### Comparing `aixhello-4.4/LICENSE` & `aixhello-4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-4.4/PKG-INFO` & `aixhello-4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.4
+Version: 4.5
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.4/README.md` & `aixhello-4.5/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-4.4/aixhello/xyello.c` & `aixhello-4.5/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -2433,14 +2433,15 @@
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_algorithms[] = "algorithms";
 static const char __pyx_k_collection[] = "collection";
 static const char __pyx_k_dataSource[] = "dataSource";
 static const char __pyx_k_datasource[] = "datasource";
 static const char __pyx_k_embeddings[] = "embeddings";
+static const char __pyx_k_encodeText[] = "encodeText";
 static const char __pyx_k_max_length[] = "max_length";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_text_embed[] = "text_embed";
 static const char __pyx_k_text_query[] = "text_query";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_encoded_url[] = "encoded_url";
@@ -2639,14 +2640,15 @@
   PyObject *__pyx_n_s_dot;
   PyObject *__pyx_n_s_dumps;
   PyObject *__pyx_n_s_e;
   PyObject *__pyx_n_s_embedding;
   PyObject *__pyx_n_s_embeddings;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encode;
+  PyObject *__pyx_n_s_encodeText;
   PyObject *__pyx_n_s_encoded_bytes;
   PyObject *__pyx_n_s_encoded_url;
   PyObject *__pyx_n_s_encryptedText;
   PyObject *__pyx_n_s_encryptor;
   PyObject *__pyx_n_s_enkyc;
   PyObject *__pyx_n_u_enkyc;
   PyObject *__pyx_n_s_enter;
@@ -2938,14 +2940,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_dot);
   Py_CLEAR(clear_module_state->__pyx_n_s_dumps);
   Py_CLEAR(clear_module_state->__pyx_n_s_e);
   Py_CLEAR(clear_module_state->__pyx_n_s_embedding);
   Py_CLEAR(clear_module_state->__pyx_n_s_embeddings);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
+  Py_CLEAR(clear_module_state->__pyx_n_s_encodeText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoded_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptedText);
   Py_CLEAR(clear_module_state->__pyx_n_s_encryptor);
   Py_CLEAR(clear_module_state->__pyx_n_s_enkyc);
   Py_CLEAR(clear_module_state->__pyx_n_u_enkyc);
   Py_CLEAR(clear_module_state->__pyx_n_s_enter);
@@ -3215,14 +3218,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_dot);
   Py_VISIT(traverse_module_state->__pyx_n_s_dumps);
   Py_VISIT(traverse_module_state->__pyx_n_s_e);
   Py_VISIT(traverse_module_state->__pyx_n_s_embedding);
   Py_VISIT(traverse_module_state->__pyx_n_s_embeddings);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
+  Py_VISIT(traverse_module_state->__pyx_n_s_encodeText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoded_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptedText);
   Py_VISIT(traverse_module_state->__pyx_n_s_encryptor);
   Py_VISIT(traverse_module_state->__pyx_n_s_enkyc);
   Py_VISIT(traverse_module_state->__pyx_n_u_enkyc);
   Py_VISIT(traverse_module_state->__pyx_n_s_enter);
@@ -3502,14 +3506,15 @@
 #define __pyx_n_s_dot __pyx_mstate_global->__pyx_n_s_dot
 #define __pyx_n_s_dumps __pyx_mstate_global->__pyx_n_s_dumps
 #define __pyx_n_s_e __pyx_mstate_global->__pyx_n_s_e
 #define __pyx_n_s_embedding __pyx_mstate_global->__pyx_n_s_embedding
 #define __pyx_n_s_embeddings __pyx_mstate_global->__pyx_n_s_embeddings
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
+#define __pyx_n_s_encodeText __pyx_mstate_global->__pyx_n_s_encodeText
 #define __pyx_n_s_encoded_bytes __pyx_mstate_global->__pyx_n_s_encoded_bytes
 #define __pyx_n_s_encoded_url __pyx_mstate_global->__pyx_n_s_encoded_url
 #define __pyx_n_s_encryptedText __pyx_mstate_global->__pyx_n_s_encryptedText
 #define __pyx_n_s_encryptor __pyx_mstate_global->__pyx_n_s_encryptor
 #define __pyx_n_s_enkyc __pyx_mstate_global->__pyx_n_s_enkyc
 #define __pyx_n_u_enkyc __pyx_mstate_global->__pyx_n_u_enkyc
 #define __pyx_n_s_enter __pyx_mstate_global->__pyx_n_s_enter
@@ -7149,14 +7154,15 @@
   PyObject *__pyx_v_pipeline = NULL;
   PyObject *__pyx_v_query_payload = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_response_data = NULL;
   PyObject *__pyx_v_documents = NULL;
   PyObject *__pyx_v_results = NULL;
   PyObject *__pyx_v_doc = NULL;
+  PyObject *__pyx_v_encodeText = NULL;
   PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
@@ -7164,16 +7170,16 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   Py_ssize_t __pyx_t_10;
   PyObject *(*__pyx_t_11)(PyObject *);
   PyObject *__pyx_t_12 = NULL;
-  PyObject *__pyx_t_13 = NULL;
-  int __pyx_t_14;
+  int __pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_t_16;
   char const *__pyx_t_17;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   PyObject *__pyx_t_21 = NULL;
@@ -7459,31 +7465,18 @@
               break;
             }
             __Pyx_GOTREF(__pyx_t_1);
           }
           __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 187, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CipherEncode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 186, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CipherEncode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 188, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 188, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __pyx_t_12 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_5))) {
             __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_5);
             if (likely(__pyx_t_12)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -7491,120 +7484,131 @@
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_5, function);
               __pyx_t_4 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_13};
-            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_3};
+            __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L4_error)
-            __Pyx_GOTREF(__pyx_t_3);
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L4_error)
+            __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           }
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_t_3) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
+          __Pyx_XDECREF_SET(__pyx_v_encodeText, __pyx_t_1);
+          __pyx_t_1 = 0;
+
+          __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_1);
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_v_encodeText) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
+
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_5) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_5) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_3) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_3) < 0) __PYX_ERR(0, 188, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 186, __pyx_L4_error)
+          __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 187, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
         __Pyx_XDECREF(__pyx_r);
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L4_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L4_error)
+        __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_v_results);
         __Pyx_GIVEREF(__pyx_v_results);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 193, __pyx_L4_error);
-        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L4_error)
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 194, __pyx_L4_error);
+        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 193, __pyx_L4_error)
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L4_error)
+        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 194, __pyx_L4_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 194, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_5;
         __pyx_t_5 = 0;
         goto __pyx_L8_try_return;
 
       }
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
       __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_4) {
         __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 194, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 195, __pyx_L6_except_error)
         __Pyx_XGOTREF(__pyx_t_5);
         __Pyx_XGOTREF(__pyx_t_3);
         __Pyx_XGOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __pyx_v_e = __pyx_t_3;
         /*try:*/ {
 
-          __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 195, __pyx_L18_error)
-          __Pyx_GOTREF(__pyx_t_13);
+          __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_12); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
           __Pyx_XDECREF(__pyx_r);
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 196, __pyx_L18_error)
-          __Pyx_GOTREF(__pyx_t_13);
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 197, __pyx_L18_error)
+          __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_12 = PyTuple_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 196, __pyx_L18_error)
-          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 197, __pyx_L18_error)
+          __Pyx_GOTREF(__pyx_t_14);
           __Pyx_GIVEREF(__pyx_t_1);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error);
           __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 196, __pyx_L18_error)
-          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_12, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 196, __pyx_L18_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 197, __pyx_L18_error)
+          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 197, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_15);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_r = __pyx_t_15;
           __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           goto __pyx_L17_return;
@@ -7614,15 +7618,15 @@
           __pyx_L18_error:;
           /*exception exit:*/{
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
             __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
             __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
             if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
             if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20) < 0)) __Pyx_ErrFetch(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
             __Pyx_XGOTREF(__pyx_t_18);
             __Pyx_XGOTREF(__pyx_t_19);
             __Pyx_XGOTREF(__pyx_t_20);
             __Pyx_XGOTREF(__pyx_t_21);
@@ -7677,44 +7681,44 @@
       __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       goto __pyx_L0;
     }
 
   }
 
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
-    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 199, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_15;
     __pyx_t_15 = 0;
     goto __pyx_L0;
@@ -7724,28 +7728,29 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_url);
   __Pyx_XDECREF(__pyx_v_headers);
   __Pyx_XDECREF(__pyx_v_pipeline);
   __Pyx_XDECREF(__pyx_v_query_payload);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_response_data);
   __Pyx_XDECREF(__pyx_v_documents);
   __Pyx_XDECREF(__pyx_v_results);
   __Pyx_XDECREF(__pyx_v_doc);
+  __Pyx_XDECREF(__pyx_v_encodeText);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
@@ -8600,14 +8605,15 @@
     {&__pyx_n_s_dot, __pyx_k_dot, sizeof(__pyx_k_dot), 0, 0, 1, 1},
     {&__pyx_n_s_dumps, __pyx_k_dumps, sizeof(__pyx_k_dumps), 0, 0, 1, 1},
     {&__pyx_n_s_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 1, 1},
     {&__pyx_n_s_embedding, __pyx_k_embedding, sizeof(__pyx_k_embedding), 0, 0, 1, 1},
     {&__pyx_n_s_embeddings, __pyx_k_embeddings, sizeof(__pyx_k_embeddings), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
+    {&__pyx_n_s_encodeText, __pyx_k_encodeText, sizeof(__pyx_k_encodeText), 0, 0, 1, 1},
     {&__pyx_n_s_encoded_bytes, __pyx_k_encoded_bytes, sizeof(__pyx_k_encoded_bytes), 0, 0, 1, 1},
     {&__pyx_n_s_encoded_url, __pyx_k_encoded_url, sizeof(__pyx_k_encoded_url), 0, 0, 1, 1},
     {&__pyx_n_s_encryptedText, __pyx_k_encryptedText, sizeof(__pyx_k_encryptedText), 0, 0, 1, 1},
     {&__pyx_n_s_encryptor, __pyx_k_encryptor, sizeof(__pyx_k_encryptor), 0, 0, 1, 1},
     {&__pyx_n_s_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 0, 1, 1},
     {&__pyx_n_u_enkyc, __pyx_k_enkyc, sizeof(__pyx_k_enkyc), 0, 1, 0, 1},
     {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
@@ -8738,15 +8744,15 @@
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 30, __pyx_L1_error)
   __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 121, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 196, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -8769,15 +8775,15 @@
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   __pyx_tuple__8 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
@@ -8830,18 +8836,18 @@
   __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_CipherEncode, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 125, __pyx_L1_error)
 
   __pyx_tuple__31 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
   __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SignalSimilarity, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 130, __pyx_L1_error)
 
-  __pyx_tuple__33 = PyTuple_Pack(16, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_vector_query, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_e); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(17, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_vector_query, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_encodeText, __pyx_n_s_e); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorSearch, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorSearch, 133, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 133, __pyx_L1_error)
 
   __pyx_tuple__35 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
   __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 16, __pyx_L1_error)
```

### Comparing `aixhello-4.4/aixhello.egg-info/PKG-INFO` & `aixhello-4.5/aixhello.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.4
+Version: 4.5
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.4/setup.py` & `aixhello-4.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='4.4',  
+    version='4.5',  
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

