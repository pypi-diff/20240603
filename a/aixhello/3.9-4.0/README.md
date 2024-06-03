# Comparing `tmp/aixhello-3.9.tar.gz` & `tmp/aixhello-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-3.9.tar", last modified: Sun Jun  2 08:53:42 2024, max compression
+gzip compressed data, was "aixhello-4.0.tar", last modified: Sun Jun  2 09:03:24 2024, max compression
```

## Comparing `aixhello-3.9.tar` & `aixhello-4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-02 08:53:42.603042 aixhello-3.9/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-3.9/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-02 08:53:42.603042 aixhello-3.9/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-06-02 08:53:42.568510 aixhello-3.9/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-3.9/aixhello/__init__.py
--rw-rw-rw-   0        0        0   567258 2024-06-02 08:53:35.000000 aixhello-3.9/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-02 08:53:42.601035 aixhello-3.9/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-02 08:53:42.000000 aixhello-3.9/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-02 08:53:42.000000 aixhello-3.9/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-02 08:53:42.000000 aixhello-3.9/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-02 08:53:42.000000 aixhello-3.9/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-02 08:53:42.000000 aixhello-3.9/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-02 08:53:42.609035 aixhello-3.9/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-02 08:52:02.000000 aixhello-3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 09:03:24.659383 aixhello-4.0/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.0/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-02 09:03:24.658383 aixhello-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 09:03:24.636976 aixhello-4.0/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.0/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   569830 2024-06-02 09:03:15.000000 aixhello-4.0/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-02 09:03:24.656385 aixhello-4.0/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-02 09:03:24.000000 aixhello-4.0/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-02 09:03:24.661383 aixhello-4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-02 09:01:48.000000 aixhello-4.0/setup.py
```

### Comparing `aixhello-3.9/LICENSE` & `aixhello-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-3.9/PKG-INFO` & `aixhello-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.9
+Version: 4.0
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.9/README.md` & `aixhello-4.0/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-3.9/aixhello/xyello.c` & `aixhello-4.0/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -2342,14 +2342,15 @@
 static const char __pyx_k_indent[] = "indent";
 static const char __pyx_k_openai[] = "openai";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_search[] = "$search";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_upsert[] = "upsert";
+static const char __pyx_k_vector[] = "vector";
 static const char __pyx_k_xyellw[] = "xyellw";
 static const char __pyx_k_api_key[] = "api_key";
 static const char __pyx_k_api_url[] = "api_url";
 static const char __pyx_k_backend[] = "backend";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_headers[] = "headers";
 static const char __pyx_k_message[] = "message";
@@ -2388,14 +2389,15 @@
 static const char __pyx_k_collection[] = "collection";
 static const char __pyx_k_dataSource[] = "dataSource";
 static const char __pyx_k_datasource[] = "datasource";
 static const char __pyx_k_embeddings[] = "embeddings";
 static const char __pyx_k_max_length[] = "max_length";
 static const char __pyx_k_pad_length[] = "pad_length";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
+static const char __pyx_k_similarity[] = "similarity";
 static const char __pyx_k_text_embed[] = "text_embed";
 static const char __pyx_k_text_query[] = "text_query";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_encoded_url[] = "encoded_url";
 static const char __pyx_k_padded_text[] = "padded_text";
 static const char __pyx_k_params_dict[] = "params_dict";
 static const char __pyx_k_searchScore[] = "searchScore";
@@ -2405,14 +2407,15 @@
 static const char __pyx_k_Content_Type[] = "Content-Type";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_shorten_text[] = "shorten_text";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
+static const char __pyx_k_vector_query[] = "vector_query";
 static const char __pyx_k_SaveToMongoDb[] = "SaveToMongoDb";
 static const char __pyx_k_decryptedText[] = "decryptedText";
 static const char __pyx_k_decrypted_url[] = "decrypted_url";
 static const char __pyx_k_encryptedText[] = "encryptedText";
 static const char __pyx_k_query_payload[] = "query_payload";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_response_data[] = "response_data";
@@ -2463,15 +2466,15 @@
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10SaveToMongoDb(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12shorten_text(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, PyObject *__pyx_v_text_query, int __pyx_v_top_n); /* proto */
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, CYTHON_UNUSED PyObject *__pyx_v_vector_query, PyObject *__pyx_v_text_query, int __pyx_v_top_n); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -2650,14 +2653,15 @@
   PyObject *__pyx_n_u_searchScore;
   PyObject *__pyx_n_u_searchindex;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_kp_u_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shorten_text;
+  PyObject *__pyx_n_u_similarity;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_state;
   PyObject *__pyx_n_s_status_code;
   PyObject *__pyx_n_s_strText;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_text;
@@ -2671,14 +2675,16 @@
   PyObject *__pyx_n_s_top_n;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_u_update;
   PyObject *__pyx_n_u_upsert;
   PyObject *__pyx_n_s_url;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
+  PyObject *__pyx_n_u_vector;
+  PyObject *__pyx_n_s_vector_query;
   PyObject *__pyx_n_s_vector_search;
   PyObject *__pyx_n_s_vectorizeEmbed;
   PyObject *__pyx_n_s_vectorizeText;
   PyObject *__pyx_n_u_wildcard;
   PyObject *__pyx_n_s_xyellw;
   PyObject *__pyx_n_s_xyellw_Decenigma;
   PyObject *__pyx_n_s_xyellw_Decipherx;
@@ -2919,14 +2925,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_u_searchScore);
   Py_CLEAR(clear_module_state->__pyx_n_u_searchindex);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_kp_u_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shorten_text);
+  Py_CLEAR(clear_module_state->__pyx_n_u_similarity);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_status_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_strText);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_text);
@@ -2940,14 +2947,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_top_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_upsert);
   Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
+  Py_CLEAR(clear_module_state->__pyx_n_u_vector);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vector_query);
   Py_CLEAR(clear_module_state->__pyx_n_s_vector_search);
   Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeEmbed);
   Py_CLEAR(clear_module_state->__pyx_n_s_vectorizeText);
   Py_CLEAR(clear_module_state->__pyx_n_u_wildcard);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_CLEAR(clear_module_state->__pyx_n_s_xyellw_Decipherx);
@@ -3166,14 +3175,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_u_searchScore);
   Py_VISIT(traverse_module_state->__pyx_n_u_searchindex);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_kp_u_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shorten_text);
+  Py_VISIT(traverse_module_state->__pyx_n_u_similarity);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_status_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_strText);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_text);
@@ -3187,14 +3197,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_top_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_upsert);
   Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
+  Py_VISIT(traverse_module_state->__pyx_n_u_vector);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vector_query);
   Py_VISIT(traverse_module_state->__pyx_n_s_vector_search);
   Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeEmbed);
   Py_VISIT(traverse_module_state->__pyx_n_s_vectorizeText);
   Py_VISIT(traverse_module_state->__pyx_n_u_wildcard);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decenigma);
   Py_VISIT(traverse_module_state->__pyx_n_s_xyellw_Decipherx);
@@ -3423,14 +3435,15 @@
 #define __pyx_n_u_searchScore __pyx_mstate_global->__pyx_n_u_searchScore
 #define __pyx_n_u_searchindex __pyx_mstate_global->__pyx_n_u_searchindex
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_kp_u_set __pyx_mstate_global->__pyx_kp_u_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shorten_text __pyx_mstate_global->__pyx_n_s_shorten_text
+#define __pyx_n_u_similarity __pyx_mstate_global->__pyx_n_u_similarity
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
 #define __pyx_n_s_status_code __pyx_mstate_global->__pyx_n_s_status_code
 #define __pyx_n_s_strText __pyx_mstate_global->__pyx_n_s_strText
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_text __pyx_mstate_global->__pyx_n_s_text
@@ -3444,14 +3457,16 @@
 #define __pyx_n_s_top_n __pyx_mstate_global->__pyx_n_s_top_n
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_u_update __pyx_mstate_global->__pyx_n_u_update
 #define __pyx_n_u_upsert __pyx_mstate_global->__pyx_n_u_upsert
 #define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
+#define __pyx_n_u_vector __pyx_mstate_global->__pyx_n_u_vector
+#define __pyx_n_s_vector_query __pyx_mstate_global->__pyx_n_s_vector_query
 #define __pyx_n_s_vector_search __pyx_mstate_global->__pyx_n_s_vector_search
 #define __pyx_n_s_vectorizeEmbed __pyx_mstate_global->__pyx_n_s_vectorizeEmbed
 #define __pyx_n_s_vectorizeText __pyx_mstate_global->__pyx_n_s_vectorizeText
 #define __pyx_n_u_wildcard __pyx_mstate_global->__pyx_n_u_wildcard
 #define __pyx_n_s_xyellw __pyx_mstate_global->__pyx_n_s_xyellw
 #define __pyx_n_s_xyellw_Decenigma __pyx_mstate_global->__pyx_n_s_xyellw_Decenigma
 #define __pyx_n_s_xyellw_Decipherx __pyx_mstate_global->__pyx_n_s_xyellw_Decipherx
@@ -6006,21 +6021,22 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_connParam = 0;
   CYTHON_UNUSED int __pyx_v_result_length;
+  CYTHON_UNUSED PyObject *__pyx_v_vector_query = 0;
   PyObject *__pyx_v_text_query = 0;
   int __pyx_v_top_n;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[4] = {0,0,0,0};
+  PyObject* values[5] = {0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("vector_search (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
@@ -6028,18 +6044,20 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_connParam,&__pyx_n_s_result_length,&__pyx_n_s_text_query,&__pyx_n_s_top_n,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_connParam,&__pyx_n_s_result_length,&__pyx_n_s_vector_query,&__pyx_n_s_text_query,&__pyx_n_s_top_n,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -6060,72 +6078,84 @@
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_result_length)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vector_search", 1, 4, 4, 1); __PYX_ERR(0, 119, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vector_search", 1, 5, 5, 1); __PYX_ERR(0, 119, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_query)) != 0)) {
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vector_query)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vector_search", 1, 4, 4, 2); __PYX_ERR(0, 119, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vector_search", 1, 5, 5, 2); __PYX_ERR(0, 119, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_top_n)) != 0)) {
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_text_query)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vector_search", 1, 4, 4, 3); __PYX_ERR(0, 119, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vector_search", 1, 5, 5, 3); __PYX_ERR(0, 119, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_top_n)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("vector_search", 1, 5, 5, 4); __PYX_ERR(0, 119, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vector_search") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 4)) {
+    } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+      values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
     }
     __pyx_v_connParam = values[0];
     __pyx_v_result_length = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_result_length == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
-    __pyx_v_text_query = ((PyObject*)values[2]);
-    __pyx_v_top_n = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_top_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
+    __pyx_v_vector_query = values[2];
+    __pyx_v_text_query = ((PyObject*)values[3]);
+    __pyx_v_top_n = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_top_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 119, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vector_search", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 119, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vector_search", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 119, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_text_query), (&PyUnicode_Type), 1, "text_query", 1))) __PYX_ERR(0, 119, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_14vector_search(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_result_length, __pyx_v_text_query, __pyx_v_top_n);
+  __pyx_r = __pyx_pf_8aixhello_6xyello_6xyellw_14vector_search(((struct __pyx_obj_8aixhello_6xyello_xyellw *)__pyx_v_self), __pyx_v_connParam, __pyx_v_result_length, __pyx_v_vector_query, __pyx_v_text_query, __pyx_v_top_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -6134,15 +6164,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, PyObject *__pyx_v_text_query, int __pyx_v_top_n) {
+static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14vector_search(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, CYTHON_UNUSED PyObject *__pyx_v_vector_query, PyObject *__pyx_v_text_query, int __pyx_v_top_n) {
   PyObject *__pyx_v_url = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_pipeline = NULL;
   PyObject *__pyx_v_query_payload = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_response_data = NULL;
   PyObject *__pyx_v_documents = NULL;
@@ -6241,32 +6271,33 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_u_search, __pyx_t_2) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filename, __pyx_int_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_extracted_text, __pyx_int_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_text_embeddings, __pyx_int_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_meta, __pyx_n_u_searchScore) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_kp_u_meta, __pyx_n_u_searchScore) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_score, __pyx_t_5) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u_project, __pyx_t_3) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_top_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_top_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_t_5) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_limit, __pyx_t_5) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   __pyx_t_5 = PyList_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
@@ -6275,73 +6306,73 @@
   if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 2, __pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_v_pipeline = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_dataSource); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_dataSource, __pyx_t_3) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_database); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_database, __pyx_t_3) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_database, __pyx_t_3) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 156, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_collection, __pyx_t_3) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_pipeline, __pyx_v_pipeline) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
   __pyx_v_query_payload = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_requests); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_requests); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_post); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_post); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 161, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_url);
   __Pyx_GIVEREF(__pyx_v_url);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_url)) __PYX_ERR(0, 161, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_url)) __PYX_ERR(0, 162, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 161, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_headers, __pyx_v_headers) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_json, __pyx_v_query_payload) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_response = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PyInt_BoolEqObjC(__pyx_t_1, __pyx_int_200, 0xC8, 0)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 164, __pyx_L1_error)
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
 
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L4_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_5 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_5)) {
@@ -6353,24 +6384,24 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_5, NULL};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L4_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         }
         __pyx_v_response_data = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L4_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response_data, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L4_error)
+        __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
         __pyx_t_3 = NULL;
         __pyx_t_4 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_3)) {
@@ -6383,184 +6414,192 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_n_u_documents, __pyx_t_5};
           __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L4_error)
+          if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         }
         __pyx_v_documents = __pyx_t_1;
         __pyx_t_1 = 0;
 
-        __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L4_error)
+        __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_v_results = ((PyObject*)__pyx_t_1);
         __pyx_t_1 = 0;
 
-        __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_documents, 0, __pyx_v_top_n, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_documents, 0, __pyx_v_top_n, NULL, NULL, NULL, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
           __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
           __pyx_t_10 = 0;
           __pyx_t_11 = NULL;
         } else {
-          __pyx_t_10 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L4_error)
+          __pyx_t_10 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 170, __pyx_L4_error)
+          __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 171, __pyx_L4_error)
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         for (;;) {
           if (likely(!__pyx_t_11)) {
             if (likely(PyList_CheckExact(__pyx_t_2))) {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 170, __pyx_L4_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 171, __pyx_L4_error)
                 #endif
                 if (__pyx_t_10 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 170, __pyx_L4_error)
+              __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 171, __pyx_L4_error)
               #else
-              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L4_error)
+              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L4_error)
               __Pyx_GOTREF(__pyx_t_1);
               #endif
             } else {
               {
                 Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
                 #if !CYTHON_ASSUME_SAFE_MACROS
-                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 170, __pyx_L4_error)
+                if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 171, __pyx_L4_error)
                 #endif
                 if (__pyx_t_10 >= __pyx_temp) break;
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 170, __pyx_L4_error)
+              __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_1); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(0, 171, __pyx_L4_error)
               #else
-              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L4_error)
+              __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L4_error)
               __Pyx_GOTREF(__pyx_t_1);
               #endif
             }
           } else {
             __pyx_t_1 = __pyx_t_11(__pyx_t_2);
             if (unlikely(!__pyx_t_1)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 170, __pyx_L4_error)
+                else __PYX_ERR(0, 171, __pyx_L4_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_1);
           }
           __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          __pyx_t_1 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L4_error)
+          __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 172, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 172, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 172, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_t_5) < 0) __PYX_ERR(0, 172, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 174, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 175, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 174, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_score, __pyx_t_3) < 0) __PYX_ERR(0, 172, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_vector, __pyx_t_3) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 171, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_similarity, __pyx_t_5) < 0) __PYX_ERR(0, 173, __pyx_L4_error)
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+          __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 172, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
         __Pyx_XDECREF(__pyx_r);
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L4_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L4_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_dumps); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L4_error)
+        __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_v_results);
         __Pyx_GIVEREF(__pyx_v_results);
-        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 177, __pyx_L4_error);
-        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L4_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 177, __pyx_L4_error)
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 177, __pyx_L4_error)
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 179, __pyx_L4_error);
+        __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
+        if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 179, __pyx_L4_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_r = __pyx_t_5;
-        __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_r = __pyx_t_3;
+        __pyx_t_3 = 0;
         goto __pyx_L8_try_return;
 
       }
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
       __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_4) {
         __Pyx_AddTraceback("aixhello.xyello.xyellw.vector_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 178, __pyx_L6_except_error)
-        __Pyx_XGOTREF(__pyx_t_5);
+        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_5, &__pyx_t_2) < 0) __PYX_ERR(0, 180, __pyx_L6_except_error)
         __Pyx_XGOTREF(__pyx_t_3);
+        __Pyx_XGOTREF(__pyx_t_5);
         __Pyx_XGOTREF(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_3);
-        __pyx_v_e = __pyx_t_3;
+        __Pyx_INCREF(__pyx_t_5);
+        __pyx_v_e = __pyx_t_5;
         /*try:*/ {
 
-          __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 179, __pyx_L18_error)
+          __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 181, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
           __Pyx_XDECREF(__pyx_r);
-          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L18_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 180, __pyx_L18_error)
+          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 182, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-          __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L18_error)
+          __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 180, __pyx_L18_error)
+          __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 182, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_14);
           __Pyx_GIVEREF(__pyx_t_1);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 180, __pyx_L18_error);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 182, __pyx_L18_error);
           __pyx_t_1 = 0;
-          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L18_error)
+          __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 180, __pyx_L18_error)
-          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 180, __pyx_L18_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 182, __pyx_L18_error)
+          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 182, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_r = __pyx_t_15;
           __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -6636,48 +6675,48 @@
       __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       goto __pyx_L0;
     }
 
   }
 
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 182, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error);
-    __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
-    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_t_5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error);
+    __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_15;
     __pyx_t_15 = 0;
     goto __pyx_L0;
   }
 
 
   /* function exit code */
@@ -7626,14 +7665,15 @@
     {&__pyx_n_u_searchScore, __pyx_k_searchScore, sizeof(__pyx_k_searchScore), 0, 1, 0, 1},
     {&__pyx_n_u_searchindex, __pyx_k_searchindex, sizeof(__pyx_k_searchindex), 0, 1, 0, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_kp_u_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 1, 0, 0},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shorten_text, __pyx_k_shorten_text, sizeof(__pyx_k_shorten_text), 0, 0, 1, 1},
+    {&__pyx_n_u_similarity, __pyx_k_similarity, sizeof(__pyx_k_similarity), 0, 1, 0, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
     {&__pyx_n_s_status_code, __pyx_k_status_code, sizeof(__pyx_k_status_code), 0, 0, 1, 1},
     {&__pyx_n_s_strText, __pyx_k_strText, sizeof(__pyx_k_strText), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
@@ -7647,14 +7687,16 @@
     {&__pyx_n_s_top_n, __pyx_k_top_n, sizeof(__pyx_k_top_n), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_u_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 1, 0, 1},
     {&__pyx_n_u_upsert, __pyx_k_upsert, sizeof(__pyx_k_upsert), 0, 1, 0, 1},
     {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
+    {&__pyx_n_u_vector, __pyx_k_vector, sizeof(__pyx_k_vector), 0, 1, 0, 1},
+    {&__pyx_n_s_vector_query, __pyx_k_vector_query, sizeof(__pyx_k_vector_query), 0, 0, 1, 1},
     {&__pyx_n_s_vector_search, __pyx_k_vector_search, sizeof(__pyx_k_vector_search), 0, 0, 1, 1},
     {&__pyx_n_s_vectorizeEmbed, __pyx_k_vectorizeEmbed, sizeof(__pyx_k_vectorizeEmbed), 0, 0, 1, 1},
     {&__pyx_n_s_vectorizeText, __pyx_k_vectorizeText, sizeof(__pyx_k_vectorizeText), 0, 0, 1, 1},
     {&__pyx_n_u_wildcard, __pyx_k_wildcard, sizeof(__pyx_k_wildcard), 0, 1, 0, 1},
     {&__pyx_n_s_xyellw, __pyx_k_xyellw, sizeof(__pyx_k_xyellw), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decenigma, __pyx_k_xyellw_Decenigma, sizeof(__pyx_k_xyellw_Decenigma), 0, 0, 1, 1},
     {&__pyx_n_s_xyellw_Decipherx, __pyx_k_xyellw_Decipherx, sizeof(__pyx_k_xyellw_Decipherx), 0, 0, 1, 1},
@@ -7670,15 +7712,15 @@
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 181, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -7697,15 +7739,15 @@
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
   __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
@@ -7743,18 +7785,18 @@
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
   __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_shorten_text, 114, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 114, __pyx_L1_error)
   __pyx_tuple__25 = PyTuple_Pack(1, __pyx_int_1000); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
 
-  __pyx_tuple__26 = PyTuple_Pack(15, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_e); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(16, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_vector_query, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_e); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vector_search, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vector_search, 119, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 119, __pyx_L1_error)
 
   __pyx_tuple__28 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   __pyx_tuple__30 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 16, __pyx_L1_error)
```

### Comparing `aixhello-3.9/aixhello.egg-info/PKG-INFO` & `aixhello-4.0/aixhello.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 3.9
+Version: 4.0
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-3.9/setup.py` & `aixhello-4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='3.9',  # Increment the version number
+    version='4.0',  # Increment the version number
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

