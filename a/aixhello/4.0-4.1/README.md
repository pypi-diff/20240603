# Comparing `tmp/aixhello-4.0.tar.gz` & `tmp/aixhello-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-4.0.tar", last modified: Sun Jun  2 09:03:24 2024, max compression
+gzip compressed data, was "aixhello-4.1.tar", last modified: Mon Jun  3 07:25:42 2024, max compression
```

## Comparing `aixhello-4.0.tar` & `aixhello-4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 09:03:24.659383 aixhello-4.0/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.0/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-02 09:03:24.658383 aixhello-4.0/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 09:03:24.636976 aixhello-4.0/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.0/aixhello/__init__.py
--rw-rw-rw-   0        0        0   569830 2024-06-02 09:03:15.000000 aixhello-4.0/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-02 09:03:24.656385 aixhello-4.0/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-02 09:03:24.661383 aixhello-4.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-02 09:01:48.000000 aixhello-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 07:25:42.364810 aixhello-4.1/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.1/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-03 07:25:42.363807 aixhello-4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 07:25:42.329810 aixhello-4.1/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.1/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   569507 2024-06-03 07:25:29.000000 aixhello-4.1/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-03 07:25:42.361808 aixhello-4.1/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-03 07:25:42.000000 aixhello-4.1/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-03 07:25:42.000000 aixhello-4.1/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 07:25:42.000000 aixhello-4.1/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-03 07:25:42.000000 aixhello-4.1/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 07:25:42.000000 aixhello-4.1/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 07:25:42.367808 aixhello-4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-03 07:23:39.000000 aixhello-4.1/setup.py
```

### Comparing `aixhello-4.0/LICENSE` & `aixhello-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-4.0/PKG-INFO` & `aixhello-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.0
+Version: 4.1
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.0/README.md` & `aixhello-4.1/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-4.0/aixhello/xyello.c` & `aixhello-4.1/aixhello/xyello.c`

 * *Files 1% similar despite different names*

```diff
@@ -2342,26 +2342,26 @@
 static const char __pyx_k_indent[] = "indent";
 static const char __pyx_k_openai[] = "openai";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_search[] = "$search";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_upsert[] = "upsert";
-static const char __pyx_k_vector[] = "vector";
 static const char __pyx_k_xyellw[] = "xyellw";
 static const char __pyx_k_api_key[] = "api_key";
 static const char __pyx_k_api_url[] = "api_url";
 static const char __pyx_k_backend[] = "backend";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_headers[] = "headers";
 static const char __pyx_k_message[] = "message";
 static const char __pyx_k_payload[] = "payload";
 static const char __pyx_k_project[] = "$project";
 static const char __pyx_k_results[] = "results";
 static const char __pyx_k_strText[] = "strText";
+static const char __pyx_k_accuracy[] = "accuracy";
 static const char __pyx_k_database[] = "database";
 static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_finalize[] = "finalize";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pipeline[] = "pipeline";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_requests[] = "requests";
@@ -2389,15 +2389,14 @@
 static const char __pyx_k_collection[] = "collection";
 static const char __pyx_k_dataSource[] = "dataSource";
 static const char __pyx_k_datasource[] = "datasource";
 static const char __pyx_k_embeddings[] = "embeddings";
 static const char __pyx_k_max_length[] = "max_length";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
-static const char __pyx_k_similarity[] = "similarity";
 static const char __pyx_k_text_embed[] = "text_embed";
 static const char __pyx_k_text_query[] = "text_query";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_encoded_url[] = "encoded_url";
 static const char __pyx_k_padded_text[] = "padded_text";
 static const char __pyx_k_params_dict[] = "params_dict";
 static const char __pyx_k_searchScore[] = "searchScore";
@@ -2527,14 +2526,15 @@
   PyObject *__pyx_kp_u_Successfully_save_to_the_databas;
   PyObject *__pyx_kp_u__10;
   PyObject *__pyx_n_s__34;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
+  PyObject *__pyx_n_u_accuracy;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
   PyObject *__pyx_n_s_api_key;
   PyObject *__pyx_kp_u_api_key_2;
   PyObject *__pyx_n_s_api_url;
   PyObject *__pyx_kp_u_application_json;
@@ -2653,15 +2653,14 @@
   PyObject *__pyx_n_u_searchScore;
   PyObject *__pyx_n_u_searchindex;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_kp_u_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shorten_text;
-  PyObject *__pyx_n_u_similarity;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_state;
   PyObject *__pyx_n_s_status_code;
   PyObject *__pyx_n_s_strText;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_text;
@@ -2675,15 +2674,14 @@
   PyObject *__pyx_n_s_top_n;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_u_update;
   PyObject *__pyx_n_u_upsert;
   PyObject *__pyx_n_s_url;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
-  PyObject *__pyx_n_u_vector;
   PyObject *__pyx_n_s_vector_query;
   PyObject *__pyx_n_s_vector_search;
   PyObject *__pyx_n_s_vectorizeEmbed;
   PyObject *__pyx_n_s_vectorizeText;
   PyObject *__pyx_n_u_wildcard;
   PyObject *__pyx_n_s_xyellw;
   PyObject *__pyx_n_s_xyellw_Decenigma;
@@ -2799,14 +2797,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_CLEAR(clear_module_state->__pyx_kp_u__10);
   Py_CLEAR(clear_module_state->__pyx_n_s__34);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
+  Py_CLEAR(clear_module_state->__pyx_n_u_accuracy);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
   Py_CLEAR(clear_module_state->__pyx_kp_u_api_key_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_url);
   Py_CLEAR(clear_module_state->__pyx_kp_u_application_json);
@@ -2925,15 +2924,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_u_searchScore);
   Py_CLEAR(clear_module_state->__pyx_n_u_searchindex);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_kp_u_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shorten_text);
-  Py_CLEAR(clear_module_state->__pyx_n_u_similarity);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_status_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_strText);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_text);
@@ -2947,15 +2945,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_top_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_upsert);
   Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
-  Py_CLEAR(clear_module_state->__pyx_n_u_vector);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_query);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_search);
   Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeEmbed);
   Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeText);
   Py_CLEAR(clear_module_state->__pyx_n_u_wildcard);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
@@ -3049,14 +3046,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_save_to_the_databas);
   Py_VISIT(traverse_module_state->__pyx_kp_u__10);
   Py_VISIT(traverse_module_state->__pyx_n_s__34);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
+  Py_VISIT(traverse_module_state->__pyx_n_u_accuracy);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
   Py_VISIT(traverse_module_state->__pyx_kp_u_api_key_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_url);
   Py_VISIT(traverse_module_state->__pyx_kp_u_application_json);
@@ -3175,15 +3173,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_u_searchScore);
   Py_VISIT(traverse_module_state->__pyx_n_u_searchindex);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_kp_u_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shorten_text);
-  Py_VISIT(traverse_module_state->__pyx_n_u_similarity);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_status_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_strText);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_text);
@@ -3197,15 +3194,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_top_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_upsert);
   Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
-  Py_VISIT(traverse_module_state->__pyx_n_u_vector);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_query);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_search);
   Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeEmbed);
   Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeText);
   Py_VISIT(traverse_module_state->__pyx_n_u_wildcard);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
@@ -3309,14 +3305,15 @@
 #define __pyx_kp_u_Successfully_save_to_the_databas __pyx_mstate_global->__pyx_kp_u_Successfully_save_to_the_databas
 #define __pyx_kp_u__10 __pyx_mstate_global->__pyx_kp_u__10
 #define __pyx_n_s__34 __pyx_mstate_global->__pyx_n_s__34
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
+#define __pyx_n_u_accuracy __pyx_mstate_global->__pyx_n_u_accuracy
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
 #define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
 #define __pyx_kp_u_api_key_2 __pyx_mstate_global->__pyx_kp_u_api_key_2
 #define __pyx_n_s_api_url __pyx_mstate_global->__pyx_n_s_api_url
 #define __pyx_kp_u_application_json __pyx_mstate_global->__pyx_kp_u_application_json
@@ -3435,15 +3432,14 @@
 #define __pyx_n_u_searchScore __pyx_mstate_global->__pyx_n_u_searchScore
 #define __pyx_n_u_searchindex __pyx_mstate_global->__pyx_n_u_searchindex
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_kp_u_set __pyx_mstate_global->__pyx_kp_u_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shorten_text __pyx_mstate_global->__pyx_n_s_shorten_text
-#define __pyx_n_u_similarity __pyx_mstate_global->__pyx_n_u_similarity
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
 #define __pyx_n_s_status_code __pyx_mstate_global->__pyx_n_s_status_code
 #define __pyx_n_s_strText __pyx_mstate_global->__pyx_n_s_strText
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_text __pyx_mstate_global->__pyx_n_s_text
@@ -3457,15 +3453,14 @@
 #define __pyx_n_s_top_n __pyx_mstate_global->__pyx_n_s_top_n
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_u_update __pyx_mstate_global->__pyx_n_u_update
 #define __pyx_n_u_upsert __pyx_mstate_global->__pyx_n_u_upsert
 #define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
-#define __pyx_n_u_vector __pyx_mstate_global->__pyx_n_u_vector
 #define __pyx_n_s_vector_query __pyx_mstate_global->__pyx_n_s_vector_query
 #define __pyx_n_s_vector_search __pyx_mstate_global->__pyx_n_s_vector_search
 #define __pyx_n_s_vectorizeEmbed __pyx_mstate_global->__pyx_n_s_vectorizeEmbed
 #define __pyx_n_s_vectorizeText __pyx_mstate_global->__pyx_n_s_vectorizeText
 #define __pyx_n_u_wildcard __pyx_mstate_global->__pyx_n_u_wildcard
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
@@ -6499,31 +6494,31 @@
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
           __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
           __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 175, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_vector, __pyx_t_3) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
           __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_similarity, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
           __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 172, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -7539,14 +7534,15 @@
     {&__pyx_kp_u_Successfully_save_to_the_databas, __pyx_k_Successfully_save_to_the_databas, sizeof(__pyx_k_Successfully_save_to_the_databas), 0, 1, 0, 0},
     {&__pyx_kp_u__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 1, 0, 0},
     {&__pyx_n_s__34, __pyx_k__34, sizeof(__pyx_k__34), 0, 0, 1, 1},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
+    {&__pyx_n_u_accuracy, __pyx_k_accuracy, sizeof(__pyx_k_accuracy), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
     {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
     {&__pyx_kp_u_api_key_2, __pyx_k_api_key_2, sizeof(__pyx_k_api_key_2), 0, 1, 0, 0},
     {&__pyx_n_s_api_url, __pyx_k_api_url, sizeof(__pyx_k_api_url), 0, 0, 1, 1},
     {&__pyx_kp_u_application_json, __pyx_k_application_json, sizeof(__pyx_k_application_json), 0, 1, 0, 0},
@@ -7665,15 +7661,14 @@
     {&__pyx_n_u_searchScore, __pyx_k_searchScore, sizeof(__pyx_k_searchScore), 0, 1, 0, 1},
     {&__pyx_n_u_searchindex, __pyx_k_searchindex, sizeof(__pyx_k_searchindex), 0, 1, 0, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_kp_u_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 1, 0, 0},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shorten_text, __pyx_k_shorten_text, sizeof(__pyx_k_shorten_text), 0, 0, 1, 1},
-    {&__pyx_n_u_similarity, __pyx_k_similarity, sizeof(__pyx_k_similarity), 0, 1, 0, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
     {&__pyx_n_s_status_code, __pyx_k_status_code, sizeof(__pyx_k_status_code), 0, 0, 1, 1},
     {&__pyx_n_s_strText, __pyx_k_strText, sizeof(__pyx_k_strText), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
@@ -7687,15 +7682,14 @@
     {&__pyx_n_s_top_n, __pyx_k_top_n, sizeof(__pyx_k_top_n), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_u_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 1, 0, 1},
     {&__pyx_n_u_upsert, __pyx_k_upsert, sizeof(__pyx_k_upsert), 0, 1, 0, 1},
     {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
-    {&__pyx_n_u_vector, __pyx_k_vector, sizeof(__pyx_k_vector), 0, 1, 0, 1},
     {&__pyx_n_s_vector_query, __pyx_k_vector_query, sizeof(__pyx_k_vector_query), 0, 0, 1, 1},
     {&__pyx_n_s_vector_search, __pyx_k_vector_search, sizeof(__pyx_k_vector_search), 0, 0, 1, 1},
     {&__pyx_n_s_vectorizeEmbed, __pyx_k_vectorizeEmbed, sizeof(__pyx_k_vectorizeEmbed), 0, 0, 1, 1},
     {&__pyx_n_s_vectorizeText, __pyx_k_vectorizeText, sizeof(__pyx_k_vectorizeText), 0, 0, 1, 1},
     {&__pyx_n_u_wildcard, __pyx_k_wildcard, sizeof(__pyx_k_wildcard), 0, 1, 0, 1},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
```

### Comparing `aixhello-4.0/aixhello.egg-info/PKG-INFO` & `aixhello-4.1/aixhello.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.0
+Version: 4.1
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.0/setup.py` & `aixhello-4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='4.0',  # Increment the version number
+    version='4.1',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

