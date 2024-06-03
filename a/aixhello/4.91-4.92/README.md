# Comparing `tmp/aixhello-4.91.tar.gz` & `tmp/aixhello-4.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-4.91.tar", last modified: Mon Jun  3 10:45:22 2024, max compression
+gzip compressed data, was "aixhello-4.92.tar", last modified: Mon Jun  3 10:48:36 2024, max compression
```

## Comparing `aixhello-4.91.tar` & `aixhello-4.92.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 10:45:21.995746 aixhello-4.91/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.91/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.91/MANIFEST.in
--rw-rw-rw-   0        0        0     1079 2024-06-03 10:45:21.994746 aixhello-4.91/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.91/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 10:45:21.970745 aixhello-4.91/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.91/aixhello/__init__.py
--rw-rw-rw-   0        0        0   715060 2024-06-03 10:45:13.000000 aixhello-4.91/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-03 10:45:21.992744 aixhello-4.91/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1079 2024-06-03 10:45:21.000000 aixhello-4.91/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-03 10:45:21.000000 aixhello-4.91/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 10:45:21.000000 aixhello-4.91/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-03 10:45:21.000000 aixhello-4.91/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 10:45:21.000000 aixhello-4.91/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 10:45:22.001781 aixhello-4.91/setup.cfg
--rw-rw-rw-   0        0        0      974 2024-06-03 10:44:50.000000 aixhello-4.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:36.187527 aixhello-4.92/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.92/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.92/MANIFEST.in
+-rw-rw-rw-   0        0        0     1079 2024-06-03 10:48:36.187527 aixhello-4.92/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.92/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:36.165528 aixhello-4.92/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.92/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   643513 2024-06-03 10:48:29.000000 aixhello-4.92/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-03 10:48:36.185530 aixhello-4.92/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1079 2024-06-03 10:48:36.000000 aixhello-4.92/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-03 10:48:36.000000 aixhello-4.92/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:48:36.000000 aixhello-4.92/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-03 10:48:36.000000 aixhello-4.92/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 10:48:36.000000 aixhello-4.92/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 10:48:36.190538 aixhello-4.92/setup.cfg
+-rw-rw-rw-   0        0        0      974 2024-06-03 10:47:55.000000 aixhello-4.92/setup.py
```

### Comparing `aixhello-4.91/LICENSE` & `aixhello-4.92/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-4.91/PKG-INFO` & `aixhello-4.92/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.91
+Version: 4.92
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.91/README.md` & `aixhello-4.92/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-4.91/aixhello/xyello.c` & `aixhello-4.92/aixhello/xyello.c`

 * *Files 2% similar despite different names*

```diff
@@ -1490,35 +1490,19 @@
 
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8aixhello_6xyello_xyellw;
-struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector;
-struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr;
 
 struct __pyx_obj_8aixhello_6xyello_xyellw {
   PyObject_HEAD
 };
 
-
-struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector {
-  PyObject_HEAD
-  PyObject *__pyx_v_filename;
-};
-
-
-struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr {
-  PyObject_HEAD
-  struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *__pyx_outer_scope;
-  PyObject *__pyx_genexpr_arg_0;
-  PyObject *__pyx_v_doc;
-};
-
 /* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
@@ -1954,23 +1938,14 @@
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* PyIntCompare.proto */
 static CYTHON_INLINE int __Pyx_PyInt_BoolEqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
 
-/* RaiseUnboundLocalError.proto */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
-
-/* RaiseClosureNameError.proto */
-static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname);
-
-/* pep479.proto */
-static void __Pyx_Generator_Replace_StopIteration(int in_async_gen);
-
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
@@ -2310,96 +2285,14 @@
 #else
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
-/* PyObjectCall2Args.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
-/* PyObjectCallMethod1.proto */
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
-
-/* CoroutineBase.proto */
-struct __pyx_CoroutineObject;
-typedef PyObject *(*__pyx_coroutine_body_t)(struct __pyx_CoroutineObject *, PyThreadState *, PyObject *);
-#if CYTHON_USE_EXC_INFO_STACK
-#define __Pyx_ExcInfoStruct  _PyErr_StackItem
-#else
-typedef struct {
-    PyObject *exc_type;
-    PyObject *exc_value;
-    PyObject *exc_traceback;
-} __Pyx_ExcInfoStruct;
-#endif
-typedef struct __pyx_CoroutineObject {
-    PyObject_HEAD
-    __pyx_coroutine_body_t body;
-    PyObject *closure;
-    __Pyx_ExcInfoStruct gi_exc_state;
-    PyObject *gi_weakreflist;
-    PyObject *classobj;
-    PyObject *yieldfrom;
-    PyObject *gi_name;
-    PyObject *gi_qualname;
-    PyObject *gi_modulename;
-    PyObject *gi_code;
-    PyObject *gi_frame;
-    int resume_label;
-    char is_running;
-} __pyx_CoroutineObject;
-static __pyx_CoroutineObject *__Pyx__Coroutine_New(
-    PyTypeObject *type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-    PyObject *name, PyObject *qualname, PyObject *module_name);
-static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
-            __pyx_CoroutineObject *gen, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-            PyObject *name, PyObject *qualname, PyObject *module_name);
-static CYTHON_INLINE void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *self);
-static int __Pyx_Coroutine_clear(PyObject *self);
-static PyObject *__Pyx_Coroutine_Send(PyObject *self, PyObject *value);
-static PyObject *__Pyx_Coroutine_Close(PyObject *self);
-static PyObject *__Pyx_Coroutine_Throw(PyObject *gen, PyObject *args);
-#if CYTHON_USE_EXC_INFO_STACK
-#define __Pyx_Coroutine_SwapException(self)
-#define __Pyx_Coroutine_ResetAndClearException(self)  __Pyx_Coroutine_ExceptionClear(&(self)->gi_exc_state)
-#else
-#define __Pyx_Coroutine_SwapException(self) {\
-    __Pyx_ExceptionSwap(&(self)->gi_exc_state.exc_type, &(self)->gi_exc_state.exc_value, &(self)->gi_exc_state.exc_traceback);\
-    __Pyx_Coroutine_ResetFrameBackpointer(&(self)->gi_exc_state);\
-    }
-#define __Pyx_Coroutine_ResetAndClearException(self) {\
-    __Pyx_ExceptionReset((self)->gi_exc_state.exc_type, (self)->gi_exc_state.exc_value, (self)->gi_exc_state.exc_traceback);\
-    (self)->gi_exc_state.exc_type = (self)->gi_exc_state.exc_value = (self)->gi_exc_state.exc_traceback = NULL;\
-    }
-#endif
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyGen_FetchStopIterationValue(pvalue)\
-    __Pyx_PyGen__FetchStopIterationValue(__pyx_tstate, pvalue)
-#else
-#define __Pyx_PyGen_FetchStopIterationValue(pvalue)\
-    __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, pvalue)
-#endif
-static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *tstate, PyObject **pvalue);
-static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state);
-
-/* PatchModuleWithCoroutine.proto */
-static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code);
-
-/* PatchGeneratorABC.proto */
-static int __Pyx_patch_abc(void);
-
-/* Generator.proto */
-#define __Pyx_Generator_USED
-#define __Pyx_Generator_CheckExact(obj) __Pyx_IS_TYPE(obj, __pyx_GeneratorType)
-#define __Pyx_Generator_New(body, code, closure, name, qualname, module_name)\
-    __Pyx__Coroutine_New(__pyx_GeneratorType, body, code, closure, name, qualname, module_name)
-static PyObject *__Pyx_Generator_Next(PyObject *self);
-static int __pyx_Generator_init(PyObject *module);
-
 /* CheckBinaryVersion.proto */
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
@@ -2412,80 +2305,76 @@
 #define __Pyx_MODULE_NAME "aixhello.xyello"
 extern int __pyx_module_is_main_aixhello__xyello;
 int __pyx_module_is_main_aixhello__xyello = 0;
 
 /* Implementation of "aixhello.xyello" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_chr;
-static PyObject *__pyx_builtin_print;
 static PyObject *__pyx_builtin_open;
+static PyObject *__pyx_builtin_print;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "";
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_e[] = "e";
 static const char __pyx_k__6[] = "*";
-static const char __pyx_k__9[] = "...";
+static const char __pyx_k__7[] = "...";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_iv[] = "iv";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_rb[] = "rb";
 static const char __pyx_k_re[] = "re";
 static const char __pyx_k_AES[] = "AES";
 static const char __pyx_k_CBC[] = "CBC";
-static const char __pyx_k__13[] = ".";
-static const char __pyx_k__45[] = "?";
+static const char __pyx_k__11[] = ".";
+static const char __pyx_k__43[] = "?";
 static const char __pyx_k_chr[] = "chr";
 static const char __pyx_k_doc[] = "doc";
 static const char __pyx_k_dot[] = "dot";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_msg[] = "msg";
 static const char __pyx_k_mth[] = "mth";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_set[] = "$set";
 static const char __pyx_k_url[] = "url";
-static const char __pyx_k_args[] = "args";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_file[] = "file";
 static const char __pyx_k_json[] = "json";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_meta[] = "$meta";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_norm[] = "norm";
 static const char __pyx_k_open[] = "open";
 static const char __pyx_k_path[] = "path";
 static const char __pyx_k_post[] = "post";
 static const char __pyx_k_read[] = "read";
 static const char __pyx_k_self[] = "self";
-static const char __pyx_k_send[] = "send";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_text[] = "text";
 static const char __pyx_k_type[] = "type";
 static const char __pyx_k_Error[] = "Error: ";
 static const char __pyx_k_chunk[] = "chunk";
-static const char __pyx_k_close[] = "close";
 static const char __pyx_k_dumps[] = "dumps";
 static const char __pyx_k_enkyc[] = "enkyc";
 static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_input[] = "input";
 static const char __pyx_k_limit[] = "$limit";
 static const char __pyx_k_model[] = "model";
 static const char __pyx_k_modes[] = "modes";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_query[] = "query";
 static const char __pyx_k_score[] = "score";
 static const char __pyx_k_state[] = "state";
-static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_top_n[] = "top_n";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_Cipher[] = "Cipher";
 static const char __pyx_k_base64[] = "base64";
 static const char __pyx_k_cipher[] = "cipher";
 static const char __pyx_k_create[] = "create";
 static const char __pyx_k_decode[] = "decode";
@@ -2503,15 +2392,14 @@
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_upsert[] = "upsert";
 static const char __pyx_k_xyellw[] = "xyellw";
 static const char __pyx_k_api_key[] = "api_key";
 static const char __pyx_k_api_url[] = "api_url";
 static const char __pyx_k_backend[] = "backend";
 static const char __pyx_k_disable[] = "disable";
-static const char __pyx_k_genexpr[] = "genexpr";
 static const char __pyx_k_headers[] = "headers";
 static const char __pyx_k_message[] = "message";
 static const char __pyx_k_payload[] = "payload";
 static const char __pyx_k_project[] = "$project";
 static const char __pyx_k_results[] = "results";
 static const char __pyx_k_strText[] = "strText";
 static const char __pyx_k_accuracy[] = "accuracy";
@@ -2607,56 +2495,52 @@
 static const char __pyx_k_aixhello_xyello_pyx[] = "aixhello\\xyello.pyx";
 static const char __pyx_k_pyx_unpickle_xyellw[] = "__pyx_unpickle_xyellw";
 static const char __pyx_k_xyellw_CipherEncode[] = "xyellw.CipherEncode";
 static const char __pyx_k_xyellw_GraphFEncode[] = "xyellw.GraphFEncode";
 static const char __pyx_k_xyellw_UpdateVector[] = "xyellw.UpdateVector";
 static const char __pyx_k_xyellw_vectorSearch[] = "xyellw.vectorSearch";
 static const char __pyx_k_xyellw_vectorizeText[] = "xyellw.vectorizeText";
-static const char __pyx_k_Train_vector_complete[] = "Train vector complete";
 static const char __pyx_k_decoded_encryptedText[] = "decoded_encryptedText";
 static const char __pyx_k_decrypted_padded_text[] = "decrypted_padded_text";
 static const char __pyx_k_xyellw_vectorizeEmbed[] = "xyellw.vectorizeEmbed";
 static const char __pyx_k_text_embedding_ada_002[] = "text-embedding-ada-002";
 static const char __pyx_k_xyellw___reduce_cython[] = "xyellw.__reduce_cython__";
 static const char __pyx_k_xyellw_SignalSimilarity[] = "xyellw.SignalSimilarity";
 static const char __pyx_k_Invalid_API_key_provided[] = "Invalid API key provided";
+static const char __pyx_k_Vector_training_complete[] = "Vector training complete.";
 static const char __pyx_k_xyellw___setstate_cython[] = "xyellw.__setstate_cython__";
-static const char __pyx_k_TrainVector_locals_genexpr[] = "TrainVector.<locals>.genexpr";
 static const char __pyx_k_An_unexpected_error_occurred[] = "An unexpected error occurred";
 static const char __pyx_k_cryptography_hazmat_backends[] = "cryptography.hazmat.backends";
 static const char __pyx_k_Access_Control_Request_Headers[] = "Access-Control-Request-Headers";
 static const char __pyx_k_Error_processing_response_JSON[] = "Error processing response JSON: ";
 static const char __pyx_k_Successfully_update_the_vector[] = "Successfully update the vector.";
 static const char __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN[] = "M#rztXq3z@U8rS5jN@PvE4W7F&J(#DhN";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4BFhKWk32xGPxL9k3jhhHkDqcCQrX37yfmobUNPTXxEGQ==";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe3b0c44, 0xda39a3e, 0xd41d8cd) = ())";
-static const char __pyx_k_Training_in_progress_It_will_tak[] = "Training in progress. It will take some time for the train vector to complete.";
+static const char __pyx_k_Training_in_progress_It_will_tak[] = "Training in progress. It will take some time for the vector training to complete.";
 static const char __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1[] = "aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1cmUvc0xwaG9RdURybDZv";
 static const char __pyx_k_cryptography_hazmat_primitives_c[] = "cryptography.hazmat.primitives.ciphers";
 static const char __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2[] = "+bhrKIrE96DyuGeXRfLhHfJ8EJJ3DkvnNAjy1BEETsxAW4fiCkX5oNaIbdYnWEoLv6rO9XYXsjGFum6Uqbj0rw1BCeo6uGrpHTR3rBufk4AsrMkJF3D7AnEcHok5damnRp1itFTxnx2dNcFig8Q+Zg==";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_Decipherx(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_msg); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_2Encapseal(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_strText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_4Decenigma(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_encryptedText); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_6vectorizeEmbed(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_chunks, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_8vectorizeText(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text_embed, PyObject *__pyx_v_text_key); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_10UpdateVector(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_database, PyObject *__pyx_v_datasource, PyObject *__pyx_v_enkyc, PyObject *__pyx_v_params_dict); /* proto */
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_11TrainVector_genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12TrainVector(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_filename); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_14limitText(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text, PyObject *__pyx_v_max_length); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_16GraphFEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_file_path); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_18CipherEncode(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_text); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_20SignalSimilarity(CYTHON_UNUSED struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_22vectorSearch(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, CYTHON_UNUSED int __pyx_v_result_length, CYTHON_UNUSED PyObject *__pyx_v_vector_query, PyObject *__pyx_v_text_query, int __pyx_v_top_n); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_24__reduce_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_26__setstate_cython__(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_8aixhello_6xyello___pyx_unpickle_xyellw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_8aixhello_6xyello_xyellw(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct__TrainVector(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
@@ -2678,20 +2562,16 @@
   PyTypeObject *__pyx_CoroutineAwaitType;
   #endif
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   PyObject *__pyx_type_8aixhello_6xyello_xyellw;
-  PyObject *__pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector;
-  PyObject *__pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr;
   #endif
   PyTypeObject *__pyx_ptype_8aixhello_6xyello_xyellw;
-  PyTypeObject *__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector;
-  PyTypeObject *__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr;
   PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_s_AES;
   PyObject *__pyx_kp_u_Access_Control_Request_Headers;
   PyObject *__pyx_kp_u_An_unexpected_error_occurred;
   PyObject *__pyx_n_s_AuthenticationError;
   PyObject *__pyx_n_s_CBC;
   PyObject *__pyx_n_s_Cipher;
@@ -2706,48 +2586,45 @@
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_u_Invalid_API_key_provided;
   PyObject *__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_SignalSimilarity;
   PyObject *__pyx_kp_u_Successfully_update_the_vector;
   PyObject *__pyx_n_s_TrainVector;
-  PyObject *__pyx_n_s_TrainVector_locals_genexpr;
-  PyObject *__pyx_kp_u_Train_vector_complete;
   PyObject *__pyx_kp_u_Training_in_progress_It_will_tak;
   PyObject *__pyx_n_s_UpdateVector;
-  PyObject *__pyx_kp_u__13;
-  PyObject *__pyx_n_s__45;
+  PyObject *__pyx_kp_u_Vector_training_complete;
+  PyObject *__pyx_kp_u__11;
+  PyObject *__pyx_n_s__43;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_kp_u__6;
-  PyObject *__pyx_kp_u__9;
+  PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1;
   PyObject *__pyx_n_u_accuracy;
   PyObject *__pyx_n_s_aixhello_xyello;
   PyObject *__pyx_kp_s_aixhello_xyello_pyx;
   PyObject *__pyx_n_s_algorithms;
   PyObject *__pyx_n_s_api_key;
   PyObject *__pyx_kp_u_api_key_2;
   PyObject *__pyx_n_s_api_url;
   PyObject *__pyx_kp_u_application_json;
   PyObject *__pyx_kp_u_application_pdf;
-  PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b;
   PyObject *__pyx_n_s_b64decode;
   PyObject *__pyx_n_s_b64encode;
   PyObject *__pyx_n_s_backend;
   PyObject *__pyx_n_s_base64;
   PyObject *__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn;
   PyObject *__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2;
   PyObject *__pyx_n_s_chr;
   PyObject *__pyx_n_s_chunk;
   PyObject *__pyx_n_s_cipher;
   PyObject *__pyx_n_s_cline_in_traceback;
-  PyObject *__pyx_n_s_close;
   PyObject *__pyx_n_s_collection;
   PyObject *__pyx_n_u_collection;
   PyObject *__pyx_n_s_connParam;
   PyObject *__pyx_n_s_create;
   PyObject *__pyx_n_s_cryptography_hazmat_backends;
   PyObject *__pyx_n_s_cryptography_hazmat_primitives_c;
   PyObject *__pyx_n_s_data;
@@ -2792,15 +2669,14 @@
   PyObject *__pyx_n_s_file_path;
   PyObject *__pyx_n_u_file_type;
   PyObject *__pyx_n_s_filename;
   PyObject *__pyx_n_u_filename;
   PyObject *__pyx_n_u_filter;
   PyObject *__pyx_n_s_finalize;
   PyObject *__pyx_kp_u_gc;
-  PyObject *__pyx_n_s_genexpr;
   PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_headers;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_indent;
   PyObject *__pyx_n_u_index;
   PyObject *__pyx_n_s_initializing;
@@ -2859,15 +2735,14 @@
   PyObject *__pyx_n_s_response_data;
   PyObject *__pyx_n_s_result_length;
   PyObject *__pyx_n_s_results;
   PyObject *__pyx_n_u_score;
   PyObject *__pyx_kp_u_search;
   PyObject *__pyx_n_u_searchScore;
   PyObject *__pyx_n_s_self;
-  PyObject *__pyx_n_s_send;
   PyObject *__pyx_kp_u_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_state;
   PyObject *__pyx_n_s_status_code;
   PyObject *__pyx_n_s_strText;
@@ -2877,15 +2752,14 @@
   PyObject *__pyx_n_u_text;
   PyObject *__pyx_n_s_text_chunks;
   PyObject *__pyx_n_s_text_embed;
   PyObject *__pyx_kp_u_text_embedding_ada_002;
   PyObject *__pyx_n_u_text_embeddings;
   PyObject *__pyx_n_s_text_key;
   PyObject *__pyx_n_s_text_query;
-  PyObject *__pyx_n_s_throw;
   PyObject *__pyx_n_s_top_n;
   PyObject *__pyx_n_u_type;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_u_update;
   PyObject *__pyx_n_u_upsert;
   PyObject *__pyx_n_s_url;
   PyObject *__pyx_n_s_use_setstate;
@@ -2919,50 +2793,48 @@
   PyObject *__pyx_int_222419149;
   PyObject *__pyx_int_228825662;
   PyObject *__pyx_int_238750788;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__3;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__5;
-  PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__9;
   PyObject *__pyx_tuple__10;
-  PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__12;
   PyObject *__pyx_tuple__14;
   PyObject *__pyx_tuple__16;
   PyObject *__pyx_tuple__18;
   PyObject *__pyx_tuple__20;
   PyObject *__pyx_tuple__22;
   PyObject *__pyx_tuple__24;
   PyObject *__pyx_tuple__26;
   PyObject *__pyx_tuple__28;
-  PyObject *__pyx_tuple__30;
+  PyObject *__pyx_tuple__29;
   PyObject *__pyx_tuple__31;
   PyObject *__pyx_tuple__33;
   PyObject *__pyx_tuple__35;
   PyObject *__pyx_tuple__37;
   PyObject *__pyx_tuple__39;
   PyObject *__pyx_tuple__41;
-  PyObject *__pyx_tuple__43;
+  PyObject *__pyx_codeobj__13;
   PyObject *__pyx_codeobj__15;
   PyObject *__pyx_codeobj__17;
   PyObject *__pyx_codeobj__19;
   PyObject *__pyx_codeobj__21;
   PyObject *__pyx_codeobj__23;
   PyObject *__pyx_codeobj__25;
   PyObject *__pyx_codeobj__27;
-  PyObject *__pyx_codeobj__29;
+  PyObject *__pyx_codeobj__30;
   PyObject *__pyx_codeobj__32;
   PyObject *__pyx_codeobj__34;
   PyObject *__pyx_codeobj__36;
   PyObject *__pyx_codeobj__38;
   PyObject *__pyx_codeobj__40;
   PyObject *__pyx_codeobj__42;
-  PyObject *__pyx_codeobj__44;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2999,18 +2871,14 @@
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_CLEAR(clear_module_state->__pyx_type_8aixhello_6xyello_xyellw);
-  Py_CLEAR(clear_module_state->__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector);
-  Py_CLEAR(clear_module_state->__pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector);
-  Py_CLEAR(clear_module_state->__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr);
-  Py_CLEAR(clear_module_state->__pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr);
   Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AES);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Access_Control_Request_Headers);
   Py_CLEAR(clear_module_state->__pyx_kp_u_An_unexpected_error_occurred);
   Py_CLEAR(clear_module_state->__pyx_n_s_AuthenticationError);
   Py_CLEAR(clear_module_state->__pyx_n_s_CBC);
   Py_CLEAR(clear_module_state->__pyx_n_s_Cipher);
@@ -3025,48 +2893,45 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_CLEAR(clear_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_SignalSimilarity);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Successfully_update_the_vector);
   Py_CLEAR(clear_module_state->__pyx_n_s_TrainVector);
-  Py_CLEAR(clear_module_state->__pyx_n_s_TrainVector_locals_genexpr);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Train_vector_complete);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Training_in_progress_It_will_tak);
   Py_CLEAR(clear_module_state->__pyx_n_s_UpdateVector);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__13);
-  Py_CLEAR(clear_module_state->__pyx_n_s__45);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Vector_training_complete);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__11);
+  Py_CLEAR(clear_module_state->__pyx_n_s__43);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__9);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_CLEAR(clear_module_state->__pyx_n_u_accuracy);
   Py_CLEAR(clear_module_state->__pyx_n_s_aixhello_xyello);
   Py_CLEAR(clear_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_algorithms);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_key);
   Py_CLEAR(clear_module_state->__pyx_kp_u_api_key_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_api_url);
   Py_CLEAR(clear_module_state->__pyx_kp_u_application_json);
   Py_CLEAR(clear_module_state->__pyx_kp_u_application_pdf);
-  Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64decode);
   Py_CLEAR(clear_module_state->__pyx_n_s_b64encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_backend);
   Py_CLEAR(clear_module_state->__pyx_n_s_base64);
   Py_CLEAR(clear_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
   Py_CLEAR(clear_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_chr);
   Py_CLEAR(clear_module_state->__pyx_n_s_chunk);
   Py_CLEAR(clear_module_state->__pyx_n_s_cipher);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
-  Py_CLEAR(clear_module_state->__pyx_n_s_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_collection);
   Py_CLEAR(clear_module_state->__pyx_n_u_collection);
   Py_CLEAR(clear_module_state->__pyx_n_s_connParam);
   Py_CLEAR(clear_module_state->__pyx_n_s_create);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_CLEAR(clear_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
@@ -3111,15 +2976,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_file_path);
   Py_CLEAR(clear_module_state->__pyx_n_u_file_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_filename);
   Py_CLEAR(clear_module_state->__pyx_n_u_filename);
   Py_CLEAR(clear_module_state->__pyx_n_u_filter);
   Py_CLEAR(clear_module_state->__pyx_n_s_finalize);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
-  Py_CLEAR(clear_module_state->__pyx_n_s_genexpr);
   Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_headers);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_indent);
   Py_CLEAR(clear_module_state->__pyx_n_u_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
@@ -3178,15 +3042,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_response_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_result_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_results);
   Py_CLEAR(clear_module_state->__pyx_n_u_score);
   Py_CLEAR(clear_module_state->__pyx_kp_u_search);
   Py_CLEAR(clear_module_state->__pyx_n_u_searchScore);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
-  Py_CLEAR(clear_module_state->__pyx_n_s_send);
   Py_CLEAR(clear_module_state->__pyx_kp_u_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_status_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_strText);
@@ -3196,15 +3059,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_u_text);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_chunks);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_embed);
   Py_CLEAR(clear_module_state->__pyx_kp_u_text_embedding_ada_002);
   Py_CLEAR(clear_module_state->__pyx_n_u_text_embeddings);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_text_query);
-  Py_CLEAR(clear_module_state->__pyx_n_s_throw);
   Py_CLEAR(clear_module_state->__pyx_n_s_top_n);
   Py_CLEAR(clear_module_state->__pyx_n_u_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_update);
   Py_CLEAR(clear_module_state->__pyx_n_u_upsert);
   Py_CLEAR(clear_module_state->__pyx_n_s_url);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
@@ -3238,50 +3100,48 @@
   Py_CLEAR(clear_module_state->__pyx_int_222419149);
   Py_CLEAR(clear_module_state->__pyx_int_228825662);
   Py_CLEAR(clear_module_state->__pyx_int_238750788);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__3);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
-  Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__12);
   Py_CLEAR(clear_module_state->__pyx_tuple__14);
   Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
   Py_CLEAR(clear_module_state->__pyx_tuple__20);
   Py_CLEAR(clear_module_state->__pyx_tuple__22);
   Py_CLEAR(clear_module_state->__pyx_tuple__24);
   Py_CLEAR(clear_module_state->__pyx_tuple__26);
   Py_CLEAR(clear_module_state->__pyx_tuple__28);
-  Py_CLEAR(clear_module_state->__pyx_tuple__30);
+  Py_CLEAR(clear_module_state->__pyx_tuple__29);
   Py_CLEAR(clear_module_state->__pyx_tuple__31);
   Py_CLEAR(clear_module_state->__pyx_tuple__33);
   Py_CLEAR(clear_module_state->__pyx_tuple__35);
   Py_CLEAR(clear_module_state->__pyx_tuple__37);
   Py_CLEAR(clear_module_state->__pyx_tuple__39);
   Py_CLEAR(clear_module_state->__pyx_tuple__41);
-  Py_CLEAR(clear_module_state->__pyx_tuple__43);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
   Py_CLEAR(clear_module_state->__pyx_codeobj__17);
   Py_CLEAR(clear_module_state->__pyx_codeobj__19);
   Py_CLEAR(clear_module_state->__pyx_codeobj__21);
   Py_CLEAR(clear_module_state->__pyx_codeobj__23);
   Py_CLEAR(clear_module_state->__pyx_codeobj__25);
   Py_CLEAR(clear_module_state->__pyx_codeobj__27);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__30);
   Py_CLEAR(clear_module_state->__pyx_codeobj__32);
   Py_CLEAR(clear_module_state->__pyx_codeobj__34);
   Py_CLEAR(clear_module_state->__pyx_codeobj__36);
   Py_CLEAR(clear_module_state->__pyx_codeobj__38);
   Py_CLEAR(clear_module_state->__pyx_codeobj__40);
   Py_CLEAR(clear_module_state->__pyx_codeobj__42);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__44);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3296,18 +3156,14 @@
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_8aixhello_6xyello_xyellw);
   Py_VISIT(traverse_module_state->__pyx_type_8aixhello_6xyello_xyellw);
-  Py_VISIT(traverse_module_state->__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector);
-  Py_VISIT(traverse_module_state->__pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector);
-  Py_VISIT(traverse_module_state->__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr);
-  Py_VISIT(traverse_module_state->__pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr);
   Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AES);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Access_Control_Request_Headers);
   Py_VISIT(traverse_module_state->__pyx_kp_u_An_unexpected_error_occurred);
   Py_VISIT(traverse_module_state->__pyx_n_s_AuthenticationError);
   Py_VISIT(traverse_module_state->__pyx_n_s_CBC);
   Py_VISIT(traverse_module_state->__pyx_n_s_Cipher);
@@ -3322,48 +3178,45 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_API_key_provided);
   Py_VISIT(traverse_module_state->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_SignalSimilarity);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Successfully_update_the_vector);
   Py_VISIT(traverse_module_state->__pyx_n_s_TrainVector);
-  Py_VISIT(traverse_module_state->__pyx_n_s_TrainVector_locals_genexpr);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Train_vector_complete);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Training_in_progress_It_will_tak);
   Py_VISIT(traverse_module_state->__pyx_n_s_UpdateVector);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__13);
-  Py_VISIT(traverse_module_state->__pyx_n_s__45);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Vector_training_complete);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__11);
+  Py_VISIT(traverse_module_state->__pyx_n_s__43);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__9);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1);
   Py_VISIT(traverse_module_state->__pyx_n_u_accuracy);
   Py_VISIT(traverse_module_state->__pyx_n_s_aixhello_xyello);
   Py_VISIT(traverse_module_state->__pyx_kp_s_aixhello_xyello_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_algorithms);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_key);
   Py_VISIT(traverse_module_state->__pyx_kp_u_api_key_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_api_url);
   Py_VISIT(traverse_module_state->__pyx_kp_u_application_json);
   Py_VISIT(traverse_module_state->__pyx_kp_u_application_pdf);
-  Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64decode);
   Py_VISIT(traverse_module_state->__pyx_n_s_b64encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_backend);
   Py_VISIT(traverse_module_state->__pyx_n_s_base64);
   Py_VISIT(traverse_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn);
   Py_VISIT(traverse_module_state->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_chr);
   Py_VISIT(traverse_module_state->__pyx_n_s_chunk);
   Py_VISIT(traverse_module_state->__pyx_n_s_cipher);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
-  Py_VISIT(traverse_module_state->__pyx_n_s_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_collection);
   Py_VISIT(traverse_module_state->__pyx_n_u_collection);
   Py_VISIT(traverse_module_state->__pyx_n_s_connParam);
   Py_VISIT(traverse_module_state->__pyx_n_s_create);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_backends);
   Py_VISIT(traverse_module_state->__pyx_n_s_cryptography_hazmat_primitives_c);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
@@ -3408,15 +3261,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_file_path);
   Py_VISIT(traverse_module_state->__pyx_n_u_file_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_filename);
   Py_VISIT(traverse_module_state->__pyx_n_u_filename);
   Py_VISIT(traverse_module_state->__pyx_n_u_filter);
   Py_VISIT(traverse_module_state->__pyx_n_s_finalize);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
-  Py_VISIT(traverse_module_state->__pyx_n_s_genexpr);
   Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_headers);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_indent);
   Py_VISIT(traverse_module_state->__pyx_n_u_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
@@ -3475,15 +3327,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_response_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_result_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_results);
   Py_VISIT(traverse_module_state->__pyx_n_u_score);
   Py_VISIT(traverse_module_state->__pyx_kp_u_search);
   Py_VISIT(traverse_module_state->__pyx_n_u_searchScore);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
-  Py_VISIT(traverse_module_state->__pyx_n_s_send);
   Py_VISIT(traverse_module_state->__pyx_kp_u_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_status_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_strText);
@@ -3493,15 +3344,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_u_text);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_chunks);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_embed);
   Py_VISIT(traverse_module_state->__pyx_kp_u_text_embedding_ada_002);
   Py_VISIT(traverse_module_state->__pyx_n_u_text_embeddings);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_text_query);
-  Py_VISIT(traverse_module_state->__pyx_n_s_throw);
   Py_VISIT(traverse_module_state->__pyx_n_s_top_n);
   Py_VISIT(traverse_module_state->__pyx_n_u_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_update);
   Py_VISIT(traverse_module_state->__pyx_n_u_upsert);
   Py_VISIT(traverse_module_state->__pyx_n_s_url);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
@@ -3535,50 +3385,48 @@
   Py_VISIT(traverse_module_state->__pyx_int_222419149);
   Py_VISIT(traverse_module_state->__pyx_int_228825662);
   Py_VISIT(traverse_module_state->__pyx_int_238750788);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__3);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
-  Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__12);
   Py_VISIT(traverse_module_state->__pyx_tuple__14);
   Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
   Py_VISIT(traverse_module_state->__pyx_tuple__20);
   Py_VISIT(traverse_module_state->__pyx_tuple__22);
   Py_VISIT(traverse_module_state->__pyx_tuple__24);
   Py_VISIT(traverse_module_state->__pyx_tuple__26);
   Py_VISIT(traverse_module_state->__pyx_tuple__28);
-  Py_VISIT(traverse_module_state->__pyx_tuple__30);
+  Py_VISIT(traverse_module_state->__pyx_tuple__29);
   Py_VISIT(traverse_module_state->__pyx_tuple__31);
   Py_VISIT(traverse_module_state->__pyx_tuple__33);
   Py_VISIT(traverse_module_state->__pyx_tuple__35);
   Py_VISIT(traverse_module_state->__pyx_tuple__37);
   Py_VISIT(traverse_module_state->__pyx_tuple__39);
   Py_VISIT(traverse_module_state->__pyx_tuple__41);
-  Py_VISIT(traverse_module_state->__pyx_tuple__43);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
   Py_VISIT(traverse_module_state->__pyx_codeobj__17);
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
   Py_VISIT(traverse_module_state->__pyx_codeobj__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__23);
   Py_VISIT(traverse_module_state->__pyx_codeobj__25);
   Py_VISIT(traverse_module_state->__pyx_codeobj__27);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__30);
   Py_VISIT(traverse_module_state->__pyx_codeobj__32);
   Py_VISIT(traverse_module_state->__pyx_codeobj__34);
   Py_VISIT(traverse_module_state->__pyx_codeobj__36);
   Py_VISIT(traverse_module_state->__pyx_codeobj__38);
   Py_VISIT(traverse_module_state->__pyx_codeobj__40);
   Py_VISIT(traverse_module_state->__pyx_codeobj__42);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__44);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3601,20 +3449,16 @@
 #define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
 #endif
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #define __pyx_type_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_type_8aixhello_6xyello_xyellw
-#define __pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector __pyx_mstate_global->__pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector
-#define __pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr __pyx_mstate_global->__pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr
 #endif
 #define __pyx_ptype_8aixhello_6xyello_xyellw __pyx_mstate_global->__pyx_ptype_8aixhello_6xyello_xyellw
-#define __pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector __pyx_mstate_global->__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector
-#define __pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr __pyx_mstate_global->__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr
 #define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_s_AES __pyx_mstate_global->__pyx_n_s_AES
 #define __pyx_kp_u_Access_Control_Request_Headers __pyx_mstate_global->__pyx_kp_u_Access_Control_Request_Headers
 #define __pyx_kp_u_An_unexpected_error_occurred __pyx_mstate_global->__pyx_kp_u_An_unexpected_error_occurred
 #define __pyx_n_s_AuthenticationError __pyx_mstate_global->__pyx_n_s_AuthenticationError
 #define __pyx_n_s_CBC __pyx_mstate_global->__pyx_n_s_CBC
 #define __pyx_n_s_Cipher __pyx_mstate_global->__pyx_n_s_Cipher
@@ -3629,48 +3473,45 @@
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_u_Invalid_API_key_provided __pyx_mstate_global->__pyx_kp_u_Invalid_API_key_provided
 #define __pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN __pyx_mstate_global->__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_SignalSimilarity __pyx_mstate_global->__pyx_n_s_SignalSimilarity
 #define __pyx_kp_u_Successfully_update_the_vector __pyx_mstate_global->__pyx_kp_u_Successfully_update_the_vector
 #define __pyx_n_s_TrainVector __pyx_mstate_global->__pyx_n_s_TrainVector
-#define __pyx_n_s_TrainVector_locals_genexpr __pyx_mstate_global->__pyx_n_s_TrainVector_locals_genexpr
-#define __pyx_kp_u_Train_vector_complete __pyx_mstate_global->__pyx_kp_u_Train_vector_complete
 #define __pyx_kp_u_Training_in_progress_It_will_tak __pyx_mstate_global->__pyx_kp_u_Training_in_progress_It_will_tak
 #define __pyx_n_s_UpdateVector __pyx_mstate_global->__pyx_n_s_UpdateVector
-#define __pyx_kp_u__13 __pyx_mstate_global->__pyx_kp_u__13
-#define __pyx_n_s__45 __pyx_mstate_global->__pyx_n_s__45
+#define __pyx_kp_u_Vector_training_complete __pyx_mstate_global->__pyx_kp_u_Vector_training_complete
+#define __pyx_kp_u__11 __pyx_mstate_global->__pyx_kp_u__11
+#define __pyx_n_s__43 __pyx_mstate_global->__pyx_n_s__43
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
-#define __pyx_kp_u__9 __pyx_mstate_global->__pyx_kp_u__9
+#define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1 __pyx_mstate_global->__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1
 #define __pyx_n_u_accuracy __pyx_mstate_global->__pyx_n_u_accuracy
 #define __pyx_n_s_aixhello_xyello __pyx_mstate_global->__pyx_n_s_aixhello_xyello
 #define __pyx_kp_s_aixhello_xyello_pyx __pyx_mstate_global->__pyx_kp_s_aixhello_xyello_pyx
 #define __pyx_n_s_algorithms __pyx_mstate_global->__pyx_n_s_algorithms
 #define __pyx_n_s_api_key __pyx_mstate_global->__pyx_n_s_api_key
 #define __pyx_kp_u_api_key_2 __pyx_mstate_global->__pyx_kp_u_api_key_2
 #define __pyx_n_s_api_url __pyx_mstate_global->__pyx_n_s_api_url
 #define __pyx_kp_u_application_json __pyx_mstate_global->__pyx_kp_u_application_json
 #define __pyx_kp_u_application_pdf __pyx_mstate_global->__pyx_kp_u_application_pdf
-#define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b __pyx_mstate_global->__pyx_n_s_b
 #define __pyx_n_s_b64decode __pyx_mstate_global->__pyx_n_s_b64decode
 #define __pyx_n_s_b64encode __pyx_mstate_global->__pyx_n_s_b64encode
 #define __pyx_n_s_backend __pyx_mstate_global->__pyx_n_s_backend
 #define __pyx_n_s_base64 __pyx_mstate_global->__pyx_n_s_base64
 #define __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn __pyx_mstate_global->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn
 #define __pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2 __pyx_mstate_global->__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2
 #define __pyx_n_s_chr __pyx_mstate_global->__pyx_n_s_chr
 #define __pyx_n_s_chunk __pyx_mstate_global->__pyx_n_s_chunk
 #define __pyx_n_s_cipher __pyx_mstate_global->__pyx_n_s_cipher
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
-#define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
 #define __pyx_n_s_collection __pyx_mstate_global->__pyx_n_s_collection
 #define __pyx_n_u_collection __pyx_mstate_global->__pyx_n_u_collection
 #define __pyx_n_s_connParam __pyx_mstate_global->__pyx_n_s_connParam
 #define __pyx_n_s_create __pyx_mstate_global->__pyx_n_s_create
 #define __pyx_n_s_cryptography_hazmat_backends __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_backends
 #define __pyx_n_s_cryptography_hazmat_primitives_c __pyx_mstate_global->__pyx_n_s_cryptography_hazmat_primitives_c
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
@@ -3715,15 +3556,14 @@
 #define __pyx_n_s_file_path __pyx_mstate_global->__pyx_n_s_file_path
 #define __pyx_n_u_file_type __pyx_mstate_global->__pyx_n_u_file_type
 #define __pyx_n_s_filename __pyx_mstate_global->__pyx_n_s_filename
 #define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
 #define __pyx_n_u_filter __pyx_mstate_global->__pyx_n_u_filter
 #define __pyx_n_s_finalize __pyx_mstate_global->__pyx_n_s_finalize
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
-#define __pyx_n_s_genexpr __pyx_mstate_global->__pyx_n_s_genexpr
 #define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_headers __pyx_mstate_global->__pyx_n_s_headers
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_indent __pyx_mstate_global->__pyx_n_s_indent
 #define __pyx_n_u_index __pyx_mstate_global->__pyx_n_u_index
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
@@ -3782,15 +3622,14 @@
 #define __pyx_n_s_response_data __pyx_mstate_global->__pyx_n_s_response_data
 #define __pyx_n_s_result_length __pyx_mstate_global->__pyx_n_s_result_length
 #define __pyx_n_s_results __pyx_mstate_global->__pyx_n_s_results
 #define __pyx_n_u_score __pyx_mstate_global->__pyx_n_u_score
 #define __pyx_kp_u_search __pyx_mstate_global->__pyx_kp_u_search
 #define __pyx_n_u_searchScore __pyx_mstate_global->__pyx_n_u_searchScore
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
-#define __pyx_n_s_send __pyx_mstate_global->__pyx_n_s_send
 #define __pyx_kp_u_set __pyx_mstate_global->__pyx_kp_u_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
 #define __pyx_n_s_status_code __pyx_mstate_global->__pyx_n_s_status_code
 #define __pyx_n_s_strText __pyx_mstate_global->__pyx_n_s_strText
@@ -3800,15 +3639,14 @@
 #define __pyx_n_u_text __pyx_mstate_global->__pyx_n_u_text
 #define __pyx_n_s_text_chunks __pyx_mstate_global->__pyx_n_s_text_chunks
 #define __pyx_n_s_text_embed __pyx_mstate_global->__pyx_n_s_text_embed
 #define __pyx_kp_u_text_embedding_ada_002 __pyx_mstate_global->__pyx_kp_u_text_embedding_ada_002
 #define __pyx_n_u_text_embeddings __pyx_mstate_global->__pyx_n_u_text_embeddings
 #define __pyx_n_s_text_key __pyx_mstate_global->__pyx_n_s_text_key
 #define __pyx_n_s_text_query __pyx_mstate_global->__pyx_n_s_text_query
-#define __pyx_n_s_throw __pyx_mstate_global->__pyx_n_s_throw
 #define __pyx_n_s_top_n __pyx_mstate_global->__pyx_n_s_top_n
 #define __pyx_n_u_type __pyx_mstate_global->__pyx_n_u_type
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_u_update __pyx_mstate_global->__pyx_n_u_update
 #define __pyx_n_u_upsert __pyx_mstate_global->__pyx_n_u_upsert
 #define __pyx_n_s_url __pyx_mstate_global->__pyx_n_s_url
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
@@ -3842,50 +3680,48 @@
 #define __pyx_int_222419149 __pyx_mstate_global->__pyx_int_222419149
 #define __pyx_int_228825662 __pyx_mstate_global->__pyx_int_228825662
 #define __pyx_int_238750788 __pyx_mstate_global->__pyx_int_238750788
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
-#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
-#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
 #define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
 #define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
 #define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
 #define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
 #define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
-#define __pyx_tuple__30 __pyx_mstate_global->__pyx_tuple__30
+#define __pyx_tuple__29 __pyx_mstate_global->__pyx_tuple__29
 #define __pyx_tuple__31 __pyx_mstate_global->__pyx_tuple__31
 #define __pyx_tuple__33 __pyx_mstate_global->__pyx_tuple__33
 #define __pyx_tuple__35 __pyx_mstate_global->__pyx_tuple__35
 #define __pyx_tuple__37 __pyx_mstate_global->__pyx_tuple__37
 #define __pyx_tuple__39 __pyx_mstate_global->__pyx_tuple__39
 #define __pyx_tuple__41 __pyx_mstate_global->__pyx_tuple__41
-#define __pyx_tuple__43 __pyx_mstate_global->__pyx_tuple__43
+#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
 #define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
-#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
+#define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
 #define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
 #define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 #define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
 #define __pyx_codeobj__38 __pyx_mstate_global->__pyx_codeobj__38
 #define __pyx_codeobj__40 __pyx_mstate_global->__pyx_codeobj__40
 #define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
-#define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
 /* #### Code section: module_code ### */
 
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8aixhello_6xyello_6xyellw_1Decipherx(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -6320,214 +6156,36 @@
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_8aixhello_6xyello_6xyellw_11TrainVector_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
-
-
-static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_11TrainVector_genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0) {
-  struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *__pyx_cur_scope;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("genexpr", 0);
-  __pyx_cur_scope = (struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *)__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct_1_genexpr(__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
-  if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *)Py_None);
-    __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 160, __pyx_L1_error)
-  } else {
-    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
-  }
-  __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *) __pyx_self;
-  __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
-  __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
-  __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
-  {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8aixhello_6xyello_6xyellw_11TrainVector_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_TrainVector_locals_genexpr, __pyx_n_s_aixhello_xyello); if (unlikely(!gen)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_cur_scope);
-    __Pyx_RefNannyFinishContext();
-    return (PyObject *) gen;
-  }
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("aixhello.xyello.xyellw.TrainVector.genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_gb_8aixhello_6xyello_6xyellw_11TrainVector_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
-{
-  struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *__pyx_cur_scope = ((struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *)__pyx_generator->closure);
-  PyObject *__pyx_r = NULL;
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("genexpr", 0);
-  switch (__pyx_generator->resume_label) {
-    case 0: goto __pyx_L3_first_run;
-    default: /* CPython raises the right error here */
-    __Pyx_RefNannyFinishContext();
-    return NULL;
-  }
-  __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 160, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 160, __pyx_L1_error) }
-  if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
-    __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        {
-          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
-          #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
-          #endif
-          if (__pyx_t_2 >= __pyx_temp) break;
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
-        #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        {
-          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
-          #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
-          #endif
-          if (__pyx_t_2 >= __pyx_temp) break;
-        }
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
-        #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 160, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_doc);
-    __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_doc, __pyx_t_4);
-    __Pyx_GIVEREF(__pyx_t_4);
-    __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename)) { __Pyx_RaiseClosureNameError("filename"); __PYX_ERR(0, 160, __pyx_L1_error) }
-    __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (__pyx_t_6) {
-      __Pyx_XDECREF(__pyx_r);
-      __Pyx_INCREF(Py_True);
-      __pyx_r = Py_True;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      goto __pyx_L0;
-    }
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(Py_False);
-    __pyx_r = Py_False;
-    goto __pyx_L0;
-  }
-  CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_Generator_Replace_StopIteration(0);
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("genexpr", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  #if !CYTHON_USE_EXC_INFO_STACK
-  __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
-  #endif
-  __pyx_generator->resume_label = -1;
-  __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 
 static PyObject *__pyx_pf_8aixhello_6xyello_6xyellw_12TrainVector(struct __pyx_obj_8aixhello_6xyello_xyellw *__pyx_v_self, PyObject *__pyx_v_connParam, PyObject *__pyx_v_filename) {
-  struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *__pyx_cur_scope;
   PyObject *__pyx_v_url = NULL;
   PyObject *__pyx_v_headers = NULL;
   PyObject *__pyx_v_pipeline = NULL;
   PyObject *__pyx_v_query_payload = NULL;
   PyObject *__pyx_v_response = NULL;
   PyObject *__pyx_v_response_data = NULL;
   PyObject *__pyx_v_documents = NULL;
-  PyObject *__pyx_gb_8aixhello_6xyello_6xyellw_11TrainVector_2generator = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
+  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("TrainVector", 0);
-  __pyx_cur_scope = (struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *)__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct__TrainVector(__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector, __pyx_empty_tuple, NULL);
-  if (unlikely(!__pyx_cur_scope)) {
-    __pyx_cur_scope = ((struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *)Py_None);
-    __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 115, __pyx_L1_error)
-  } else {
-    __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
-  }
-  __pyx_cur_scope->__pyx_v_filename = __pyx_v_filename;
-  __Pyx_INCREF(__pyx_cur_scope->__pyx_v_filename);
-  __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_filename);
+  __Pyx_RefNannySetupContext("TrainVector", 1);
 
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_Decenigma); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
@@ -6572,15 +6230,15 @@
   __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_connParam, __pyx_n_u_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_index, __pyx_t_3) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_cur_scope->__pyx_v_filename) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_query, __pyx_v_filename) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
 
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_wildcard, __pyx_kp_u__6) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_path, __pyx_t_5) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_text, __pyx_t_3) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
@@ -6711,41 +6369,50 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_documents = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  __pyx_t_1 = __pyx_pf_8aixhello_6xyello_6xyellw_11TrainVector_genexpr(((PyObject*)__pyx_cur_scope), __pyx_v_documents); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_documents); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+  if (__pyx_t_7) {
+  } else {
+    __pyx_t_6 = __pyx_t_7;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_documents, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_7 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_v_filename, Py_EQ)); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 160, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_6 = __pyx_t_7;
+  __pyx_L4_bool_binop_done:;
   if (__pyx_t_6) {
 
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_kp_u_Vector_training_complete);
+    __pyx_r = __pyx_kp_u_Vector_training_complete;
+    goto __pyx_L0;
 
-    goto __pyx_L3;
   }
 
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_kp_u_Training_in_progress_It_will_tak);
+    __pyx_r = __pyx_kp_u_Training_in_progress_It_will_tak;
+    goto __pyx_L0;
   }
-  __pyx_L3:;
 
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.TrainVector", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
@@ -6753,16 +6420,14 @@
   __Pyx_XDECREF(__pyx_v_url);
   __Pyx_XDECREF(__pyx_v_headers);
   __Pyx_XDECREF(__pyx_v_pipeline);
   __Pyx_XDECREF(__pyx_v_query_payload);
   __Pyx_XDECREF(__pyx_v_response);
   __Pyx_XDECREF(__pyx_v_response_data);
   __Pyx_XDECREF(__pyx_v_documents);
-  __Pyx_XDECREF(__pyx_gb_8aixhello_6xyello_6xyellw_11TrainVector_2generator);
-  __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 
 /* Python wrapper */
@@ -6921,15 +6586,15 @@
     } else {
       __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 167, __pyx_L1_error)
       __pyx_t_1 = __pyx_t_5;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyUnicode_Substring(__pyx_v_text, 0, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_3, __pyx_kp_u__9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_3, __pyx_kp_u__7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
   }
@@ -7267,27 +6932,27 @@
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_3) {
-          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__10, NULL);
+          __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 171, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L4_return: {
         __pyx_t_9 = __pyx_r;
         __pyx_r = 0;
         if (__pyx_t_3) {
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__10, NULL);
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__8, NULL);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 171, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __pyx_r = __pyx_t_9;
         __pyx_t_9 = 0;
@@ -8295,15 +7960,15 @@
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 238, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
           __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 241, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 241, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_5) < 0) __PYX_ERR(0, 238, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
           __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 237, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -8963,15 +8628,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_xyellw", 1);
 
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__12, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__10, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
@@ -9288,332 +8953,14 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
-#if CYTHON_USE_FREELISTS
-static struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *__pyx_freelist_8aixhello_6xyello___pyx_scope_struct__TrainVector[8];
-static int __pyx_freecount_8aixhello_6xyello___pyx_scope_struct__TrainVector = 0;
-#endif
-
-static PyObject *__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct__TrainVector(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  PyObject *o;
-  #if CYTHON_COMPILING_IN_LIMITED_API
-  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
-  o = alloc_func(t, 0);
-  #else
-  #if CYTHON_USE_FREELISTS
-  if (likely((int)(__pyx_freecount_8aixhello_6xyello___pyx_scope_struct__TrainVector > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector)))) {
-    o = (PyObject*)__pyx_freelist_8aixhello_6xyello___pyx_scope_struct__TrainVector[--__pyx_freecount_8aixhello_6xyello___pyx_scope_struct__TrainVector];
-    memset(o, 0, sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector));
-    (void) PyObject_INIT(o, t);
-  } else
-  #endif
-  {
-    o = (*t->tp_alloc)(t, 0);
-    if (unlikely(!o)) return 0;
-  }
-  #endif
-  return o;
-}
-
-static void __pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct__TrainVector(PyObject *o) {
-  struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *p = (struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *)o;
-  #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct__TrainVector) {
-      if (PyObject_CallFinalizerFromDealloc(o)) return;
-    }
-  }
-  #endif
-  Py_CLEAR(p->__pyx_v_filename);
-  #if CYTHON_USE_FREELISTS
-  if (((int)(__pyx_freecount_8aixhello_6xyello___pyx_scope_struct__TrainVector < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector)))) {
-    __pyx_freelist_8aixhello_6xyello___pyx_scope_struct__TrainVector[__pyx_freecount_8aixhello_6xyello___pyx_scope_struct__TrainVector++] = ((struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector *)o);
-  } else
-  #endif
-  {
-    #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
-    (*Py_TYPE(o)->tp_free)(o);
-    #else
-    {
-      freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
-      if (tp_free) tp_free(o);
-    }
-    #endif
-  }
-}
-#if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct__TrainVector},
-  {Py_tp_new, (void *)__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct__TrainVector},
-  {0, 0},
-};
-static PyType_Spec __pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector_spec = {
-  "aixhello.xyello.__pyx_scope_struct__TrainVector",
-  sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector),
-  0,
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector_slots,
-};
-#else
-
-static PyTypeObject __pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector = {
-  PyVarObject_HEAD_INIT(0, 0)
-  "aixhello.xyello.""__pyx_scope_struct__TrainVector", /*tp_name*/
-  sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct__TrainVector), /*tp_basicsize*/
-  0, /*tp_itemsize*/
-  __pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct__TrainVector, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
-  0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
-  0, /*tp_getattr*/
-  0, /*tp_setattr*/
-  #if PY_MAJOR_VERSION < 3
-  0, /*tp_compare*/
-  #endif
-  #if PY_MAJOR_VERSION >= 3
-  0, /*tp_as_async*/
-  #endif
-  0, /*tp_repr*/
-  0, /*tp_as_number*/
-  0, /*tp_as_sequence*/
-  0, /*tp_as_mapping*/
-  0, /*tp_hash*/
-  0, /*tp_call*/
-  0, /*tp_str*/
-  0, /*tp_getattro*/
-  0, /*tp_setattro*/
-  0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
-  0, /*tp_doc*/
-  0, /*tp_traverse*/
-  0, /*tp_clear*/
-  0, /*tp_richcompare*/
-  0, /*tp_weaklistoffset*/
-  0, /*tp_iter*/
-  0, /*tp_iternext*/
-  0, /*tp_methods*/
-  0, /*tp_members*/
-  0, /*tp_getset*/
-  0, /*tp_base*/
-  0, /*tp_dict*/
-  0, /*tp_descr_get*/
-  0, /*tp_descr_set*/
-  #if !CYTHON_USE_TYPE_SPECS
-  0, /*tp_dictoffset*/
-  #endif
-  0, /*tp_init*/
-  0, /*tp_alloc*/
-  __pyx_tp_new_8aixhello_6xyello___pyx_scope_struct__TrainVector, /*tp_new*/
-  0, /*tp_free*/
-  0, /*tp_is_gc*/
-  0, /*tp_bases*/
-  0, /*tp_mro*/
-  0, /*tp_cache*/
-  0, /*tp_subclasses*/
-  0, /*tp_weaklist*/
-  0, /*tp_del*/
-  0, /*tp_version_tag*/
-  #if PY_VERSION_HEX >= 0x030400a1
-  #if CYTHON_USE_TP_FINALIZE
-  0, /*tp_finalize*/
-  #else
-  NULL, /*tp_finalize*/
-  #endif
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if __PYX_NEED_TP_PRINT_SLOT == 1
-  0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030C0000
-  0, /*tp_watched*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
-};
-#endif
-
-#if CYTHON_USE_FREELISTS
-static struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *__pyx_freelist_8aixhello_6xyello___pyx_scope_struct_1_genexpr[8];
-static int __pyx_freecount_8aixhello_6xyello___pyx_scope_struct_1_genexpr = 0;
-#endif
-
-static PyObject *__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  PyObject *o;
-  #if CYTHON_COMPILING_IN_LIMITED_API
-  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
-  o = alloc_func(t, 0);
-  #else
-  #if CYTHON_USE_FREELISTS
-  if (likely((int)(__pyx_freecount_8aixhello_6xyello___pyx_scope_struct_1_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr)))) {
-    o = (PyObject*)__pyx_freelist_8aixhello_6xyello___pyx_scope_struct_1_genexpr[--__pyx_freecount_8aixhello_6xyello___pyx_scope_struct_1_genexpr];
-    memset(o, 0, sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr));
-    (void) PyObject_INIT(o, t);
-    PyObject_GC_Track(o);
-  } else
-  #endif
-  {
-    o = (*t->tp_alloc)(t, 0);
-    if (unlikely(!o)) return 0;
-  }
-  #endif
-  return o;
-}
-
-static void __pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct_1_genexpr(PyObject *o) {
-  struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *)o;
-  #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct_1_genexpr) {
-      if (PyObject_CallFinalizerFromDealloc(o)) return;
-    }
-  }
-  #endif
-  PyObject_GC_UnTrack(o);
-  Py_CLEAR(p->__pyx_outer_scope);
-  Py_CLEAR(p->__pyx_genexpr_arg_0);
-  Py_CLEAR(p->__pyx_v_doc);
-  #if CYTHON_USE_FREELISTS
-  if (((int)(__pyx_freecount_8aixhello_6xyello___pyx_scope_struct_1_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr)))) {
-    __pyx_freelist_8aixhello_6xyello___pyx_scope_struct_1_genexpr[__pyx_freecount_8aixhello_6xyello___pyx_scope_struct_1_genexpr++] = ((struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *)o);
-  } else
-  #endif
-  {
-    #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
-    (*Py_TYPE(o)->tp_free)(o);
-    #else
-    {
-      freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
-      if (tp_free) tp_free(o);
-    }
-    #endif
-  }
-}
-
-static int __pyx_tp_traverse_8aixhello_6xyello___pyx_scope_struct_1_genexpr(PyObject *o, visitproc v, void *a) {
-  int e;
-  struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *p = (struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr *)o;
-  if (p->__pyx_outer_scope) {
-    e = (*v)(((PyObject *)p->__pyx_outer_scope), a); if (e) return e;
-  }
-  if (p->__pyx_genexpr_arg_0) {
-    e = (*v)(p->__pyx_genexpr_arg_0, a); if (e) return e;
-  }
-  if (p->__pyx_v_doc) {
-    e = (*v)(p->__pyx_v_doc, a); if (e) return e;
-  }
-  return 0;
-}
-#if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct_1_genexpr},
-  {Py_tp_traverse, (void *)__pyx_tp_traverse_8aixhello_6xyello___pyx_scope_struct_1_genexpr},
-  {Py_tp_new, (void *)__pyx_tp_new_8aixhello_6xyello___pyx_scope_struct_1_genexpr},
-  {0, 0},
-};
-static PyType_Spec __pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr_spec = {
-  "aixhello.xyello.__pyx_scope_struct_1_genexpr",
-  sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr),
-  0,
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE,
-  __pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr_slots,
-};
-#else
-
-static PyTypeObject __pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr = {
-  PyVarObject_HEAD_INIT(0, 0)
-  "aixhello.xyello.""__pyx_scope_struct_1_genexpr", /*tp_name*/
-  sizeof(struct __pyx_obj_8aixhello_6xyello___pyx_scope_struct_1_genexpr), /*tp_basicsize*/
-  0, /*tp_itemsize*/
-  __pyx_tp_dealloc_8aixhello_6xyello___pyx_scope_struct_1_genexpr, /*tp_dealloc*/
-  #if PY_VERSION_HEX < 0x030800b4
-  0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b4
-  0, /*tp_vectorcall_offset*/
-  #endif
-  0, /*tp_getattr*/
-  0, /*tp_setattr*/
-  #if PY_MAJOR_VERSION < 3
-  0, /*tp_compare*/
-  #endif
-  #if PY_MAJOR_VERSION >= 3
-  0, /*tp_as_async*/
-  #endif
-  0, /*tp_repr*/
-  0, /*tp_as_number*/
-  0, /*tp_as_sequence*/
-  0, /*tp_as_mapping*/
-  0, /*tp_hash*/
-  0, /*tp_call*/
-  0, /*tp_str*/
-  0, /*tp_getattro*/
-  0, /*tp_setattro*/
-  0, /*tp_as_buffer*/
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_HAVE_GC|Py_TPFLAGS_HAVE_FINALIZE, /*tp_flags*/
-  0, /*tp_doc*/
-  __pyx_tp_traverse_8aixhello_6xyello___pyx_scope_struct_1_genexpr, /*tp_traverse*/
-  0, /*tp_clear*/
-  0, /*tp_richcompare*/
-  0, /*tp_weaklistoffset*/
-  0, /*tp_iter*/
-  0, /*tp_iternext*/
-  0, /*tp_methods*/
-  0, /*tp_members*/
-  0, /*tp_getset*/
-  0, /*tp_base*/
-  0, /*tp_dict*/
-  0, /*tp_descr_get*/
-  0, /*tp_descr_set*/
-  #if !CYTHON_USE_TYPE_SPECS
-  0, /*tp_dictoffset*/
-  #endif
-  0, /*tp_init*/
-  0, /*tp_alloc*/
-  __pyx_tp_new_8aixhello_6xyello___pyx_scope_struct_1_genexpr, /*tp_new*/
-  0, /*tp_free*/
-  0, /*tp_is_gc*/
-  0, /*tp_bases*/
-  0, /*tp_mro*/
-  0, /*tp_cache*/
-  0, /*tp_subclasses*/
-  0, /*tp_weaklist*/
-  0, /*tp_del*/
-  0, /*tp_version_tag*/
-  #if PY_VERSION_HEX >= 0x030400a1
-  #if CYTHON_USE_TP_FINALIZE
-  0, /*tp_finalize*/
-  #else
-  NULL, /*tp_finalize*/
-  #endif
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-  0, /*tp_vectorcall*/
-  #endif
-  #if __PYX_NEED_TP_PRINT_SLOT == 1
-  0, /*tp_print*/
-  #endif
-  #if PY_VERSION_HEX >= 0x030C0000
-  0, /*tp_watched*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
-};
-#endif
-
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
@@ -9644,48 +8991,45 @@
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_u_Invalid_API_key_provided, __pyx_k_Invalid_API_key_provided, sizeof(__pyx_k_Invalid_API_key_provided), 0, 1, 0, 0},
     {&__pyx_kp_b_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, __pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN, sizeof(__pyx_k_M_rztXq3z_U8rS5jN_PvE4W7F_J_DhN), 0, 0, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_SignalSimilarity, __pyx_k_SignalSimilarity, sizeof(__pyx_k_SignalSimilarity), 0, 0, 1, 1},
     {&__pyx_kp_u_Successfully_update_the_vector, __pyx_k_Successfully_update_the_vector, sizeof(__pyx_k_Successfully_update_the_vector), 0, 1, 0, 0},
     {&__pyx_n_s_TrainVector, __pyx_k_TrainVector, sizeof(__pyx_k_TrainVector), 0, 0, 1, 1},
-    {&__pyx_n_s_TrainVector_locals_genexpr, __pyx_k_TrainVector_locals_genexpr, sizeof(__pyx_k_TrainVector_locals_genexpr), 0, 0, 1, 1},
-    {&__pyx_kp_u_Train_vector_complete, __pyx_k_Train_vector_complete, sizeof(__pyx_k_Train_vector_complete), 0, 1, 0, 0},
     {&__pyx_kp_u_Training_in_progress_It_will_tak, __pyx_k_Training_in_progress_It_will_tak, sizeof(__pyx_k_Training_in_progress_It_will_tak), 0, 1, 0, 0},
     {&__pyx_n_s_UpdateVector, __pyx_k_UpdateVector, sizeof(__pyx_k_UpdateVector), 0, 0, 1, 1},
-    {&__pyx_kp_u__13, __pyx_k__13, sizeof(__pyx_k__13), 0, 1, 0, 0},
-    {&__pyx_n_s__45, __pyx_k__45, sizeof(__pyx_k__45), 0, 0, 1, 1},
+    {&__pyx_kp_u_Vector_training_complete, __pyx_k_Vector_training_complete, sizeof(__pyx_k_Vector_training_complete), 0, 1, 0, 0},
+    {&__pyx_kp_u__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 1, 0, 0},
+    {&__pyx_n_s__43, __pyx_k__43, sizeof(__pyx_k__43), 0, 0, 1, 1},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
-    {&__pyx_kp_u__9, __pyx_k__9, sizeof(__pyx_k__9), 0, 1, 0, 0},
+    {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_u_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, __pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1, sizeof(__pyx_k_aHR0cHM6Ly94ZXJvY2FpLmNvbS9zZWN1), 0, 1, 0, 1},
     {&__pyx_n_u_accuracy, __pyx_k_accuracy, sizeof(__pyx_k_accuracy), 0, 1, 0, 1},
     {&__pyx_n_s_aixhello_xyello, __pyx_k_aixhello_xyello, sizeof(__pyx_k_aixhello_xyello), 0, 0, 1, 1},
     {&__pyx_kp_s_aixhello_xyello_pyx, __pyx_k_aixhello_xyello_pyx, sizeof(__pyx_k_aixhello_xyello_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_algorithms, __pyx_k_algorithms, sizeof(__pyx_k_algorithms), 0, 0, 1, 1},
     {&__pyx_n_s_api_key, __pyx_k_api_key, sizeof(__pyx_k_api_key), 0, 0, 1, 1},
     {&__pyx_kp_u_api_key_2, __pyx_k_api_key_2, sizeof(__pyx_k_api_key_2), 0, 1, 0, 0},
     {&__pyx_n_s_api_url, __pyx_k_api_url, sizeof(__pyx_k_api_url), 0, 0, 1, 1},
     {&__pyx_kp_u_application_json, __pyx_k_application_json, sizeof(__pyx_k_application_json), 0, 1, 0, 0},
     {&__pyx_kp_u_application_pdf, __pyx_k_application_pdf, sizeof(__pyx_k_application_pdf), 0, 1, 0, 0},
-    {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
     {&__pyx_n_s_b64decode, __pyx_k_b64decode, sizeof(__pyx_k_b64decode), 0, 0, 1, 1},
     {&__pyx_n_s_b64encode, __pyx_k_b64encode, sizeof(__pyx_k_b64encode), 0, 0, 1, 1},
     {&__pyx_n_s_backend, __pyx_k_backend, sizeof(__pyx_k_backend), 0, 0, 1, 1},
     {&__pyx_n_s_base64, __pyx_k_base64, sizeof(__pyx_k_base64), 0, 0, 1, 1},
     {&__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn, sizeof(__pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn), 0, 1, 0, 0},
     {&__pyx_kp_u_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2, __pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2, sizeof(__pyx_k_bhrKIrE96DyuGeXRfLhHfJ8EJJ3Dkvn_2), 0, 1, 0, 0},
     {&__pyx_n_s_chr, __pyx_k_chr, sizeof(__pyx_k_chr), 0, 0, 1, 1},
     {&__pyx_n_s_chunk, __pyx_k_chunk, sizeof(__pyx_k_chunk), 0, 0, 1, 1},
     {&__pyx_n_s_cipher, __pyx_k_cipher, sizeof(__pyx_k_cipher), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-    {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
     {&__pyx_n_s_collection, __pyx_k_collection, sizeof(__pyx_k_collection), 0, 0, 1, 1},
     {&__pyx_n_u_collection, __pyx_k_collection, sizeof(__pyx_k_collection), 0, 1, 0, 1},
     {&__pyx_n_s_connParam, __pyx_k_connParam, sizeof(__pyx_k_connParam), 0, 0, 1, 1},
     {&__pyx_n_s_create, __pyx_k_create, sizeof(__pyx_k_create), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_backends, __pyx_k_cryptography_hazmat_backends, sizeof(__pyx_k_cryptography_hazmat_backends), 0, 0, 1, 1},
     {&__pyx_n_s_cryptography_hazmat_primitives_c, __pyx_k_cryptography_hazmat_primitives_c, sizeof(__pyx_k_cryptography_hazmat_primitives_c), 0, 0, 1, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
@@ -9730,15 +9074,14 @@
     {&__pyx_n_s_file_path, __pyx_k_file_path, sizeof(__pyx_k_file_path), 0, 0, 1, 1},
     {&__pyx_n_u_file_type, __pyx_k_file_type, sizeof(__pyx_k_file_type), 0, 1, 0, 1},
     {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
     {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
     {&__pyx_n_u_filter, __pyx_k_filter, sizeof(__pyx_k_filter), 0, 1, 0, 1},
     {&__pyx_n_s_finalize, __pyx_k_finalize, sizeof(__pyx_k_finalize), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
-    {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
     {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_headers, __pyx_k_headers, sizeof(__pyx_k_headers), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_indent, __pyx_k_indent, sizeof(__pyx_k_indent), 0, 0, 1, 1},
     {&__pyx_n_u_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 1, 0, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
@@ -9797,15 +9140,14 @@
     {&__pyx_n_s_response_data, __pyx_k_response_data, sizeof(__pyx_k_response_data), 0, 0, 1, 1},
     {&__pyx_n_s_result_length, __pyx_k_result_length, sizeof(__pyx_k_result_length), 0, 0, 1, 1},
     {&__pyx_n_s_results, __pyx_k_results, sizeof(__pyx_k_results), 0, 0, 1, 1},
     {&__pyx_n_u_score, __pyx_k_score, sizeof(__pyx_k_score), 0, 1, 0, 1},
     {&__pyx_kp_u_search, __pyx_k_search, sizeof(__pyx_k_search), 0, 1, 0, 0},
     {&__pyx_n_u_searchScore, __pyx_k_searchScore, sizeof(__pyx_k_searchScore), 0, 1, 0, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
-    {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
     {&__pyx_kp_u_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 1, 0, 0},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
     {&__pyx_n_s_status_code, __pyx_k_status_code, sizeof(__pyx_k_status_code), 0, 0, 1, 1},
     {&__pyx_n_s_strText, __pyx_k_strText, sizeof(__pyx_k_strText), 0, 0, 1, 1},
@@ -9815,15 +9157,14 @@
     {&__pyx_n_u_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 1, 0, 1},
     {&__pyx_n_s_text_chunks, __pyx_k_text_chunks, sizeof(__pyx_k_text_chunks), 0, 0, 1, 1},
     {&__pyx_n_s_text_embed, __pyx_k_text_embed, sizeof(__pyx_k_text_embed), 0, 0, 1, 1},
     {&__pyx_kp_u_text_embedding_ada_002, __pyx_k_text_embedding_ada_002, sizeof(__pyx_k_text_embedding_ada_002), 0, 1, 0, 0},
     {&__pyx_n_u_text_embeddings, __pyx_k_text_embeddings, sizeof(__pyx_k_text_embeddings), 0, 1, 0, 1},
     {&__pyx_n_s_text_key, __pyx_k_text_key, sizeof(__pyx_k_text_key), 0, 0, 1, 1},
     {&__pyx_n_s_text_query, __pyx_k_text_query, sizeof(__pyx_k_text_query), 0, 0, 1, 1},
-    {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
     {&__pyx_n_s_top_n, __pyx_k_top_n, sizeof(__pyx_k_top_n), 0, 0, 1, 1},
     {&__pyx_n_u_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 1, 0, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_u_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 1, 0, 1},
     {&__pyx_n_u_upsert, __pyx_k_upsert, sizeof(__pyx_k_upsert), 0, 1, 0, 1},
     {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
@@ -9852,16 +9193,16 @@
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 30, __pyx_L1_error)
-  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 161, __pyx_L1_error)
   __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_builtin_print = __Pyx_GetBuiltinName(__pyx_n_s_print); if (!__pyx_builtin_print) __PYX_ERR(0, 246, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -9880,111 +9221,103 @@
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_u_text_embeddings, __pyx_kp_u_); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Train_vector_complete); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 161, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Training_in_progress_It_will_tak); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  __pyx_tuple__10 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+
+  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_u_score, __pyx_int_0); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 241, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-
-  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_238750788, __pyx_int_228825662, __pyx_int_222419149); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 13, __pyx_L1_error)
 
-  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_encoded_url, __pyx_n_s_api_url, __pyx_n_s_response); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decipherx, 13, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 20, __pyx_L1_error)
 
-  __pyx_tuple__16 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_strText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_encryptor, __pyx_n_s_pad_length, __pyx_n_s_padded_text, __pyx_n_s_encryptedText); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Encapseal, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 35, __pyx_L1_error)
 
-  __pyx_tuple__18 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_encryptedText, __pyx_n_s_key, __pyx_n_s_iv, __pyx_n_s_mth, __pyx_n_s_backend, __pyx_n_s_cipher, __pyx_n_s_decryptor, __pyx_n_s_decoded_encryptedText, __pyx_n_s_decrypted_padded_text, __pyx_n_s_pad_length, __pyx_n_s_decryptedText); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_Decenigma, 35, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbed, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 52, __pyx_L1_error)
 
-  __pyx_tuple__20 = PyTuple_Pack(8, __pyx_n_s_self, __pyx_n_s_text_chunks, __pyx_n_s_text_key, __pyx_n_s_embeddings, __pyx_n_s_chunk, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeEmbed, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 69, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 69, __pyx_L1_error)
 
-  __pyx_tuple__22 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_text_embed, __pyx_n_s_text_key, __pyx_n_s_response, __pyx_n_s_embedding, __pyx_n_s_e); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorizeText, 69, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_UpdateVector, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 83, __pyx_L1_error)
 
-  __pyx_tuple__24 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_database, __pyx_n_s_datasource, __pyx_n_s_enkyc, __pyx_n_s_params_dict, __pyx_n_s_decrypted_url, __pyx_n_s_payload, __pyx_n_s_headers, __pyx_n_s_response); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_filename, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_UpdateVector, 83, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_TrainVector, 115, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 115, __pyx_L1_error)
 
-  __pyx_tuple__26 = PyTuple_Pack(12, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_filename, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_max_length); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_TrainVector, 115, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 115, __pyx_L1_error)
-
-  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_max_length); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_limitText, 165, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_int_1000); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_limitText, 165, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 165, __pyx_L1_error)
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_int_1000); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 165, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
 
-  __pyx_tuple__31 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_file_path, __pyx_n_s_file, __pyx_n_s_file_content); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_file_path, __pyx_n_s_file, __pyx_n_s_file_content); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_GraphFEncode, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 170, __pyx_L1_error)
+
+  __pyx_tuple__31 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_input_bytes, __pyx_n_s_encoded_bytes); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_GraphFEncode, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_CipherEncode, 175, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 175, __pyx_L1_error)
 
-  __pyx_tuple__33 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_text, __pyx_n_s_input_bytes, __pyx_n_s_encoded_bytes); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_CipherEncode, 175, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SignalSimilarity, 180, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 180, __pyx_L1_error)
 
-  __pyx_tuple__35 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(17, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_vector_query, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_encodeText, __pyx_n_s_e); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_SignalSimilarity, 180, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorSearch, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 183, __pyx_L1_error)
 
-  __pyx_tuple__37 = PyTuple_Pack(17, __pyx_n_s_self, __pyx_n_s_connParam, __pyx_n_s_result_length, __pyx_n_s_vector_query, __pyx_n_s_text_query, __pyx_n_s_top_n, __pyx_n_s_url, __pyx_n_s_headers, __pyx_n_s_pipeline, __pyx_n_s_query_payload, __pyx_n_s_response, __pyx_n_s_response_data, __pyx_n_s_documents, __pyx_n_s_results, __pyx_n_s_doc, __pyx_n_s_encodeText, __pyx_n_s_e); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 17, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aixhello_xyello_pyx, __pyx_n_s_vectorSearch, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  __pyx_tuple__39 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(1, 16, __pyx_L1_error)
 
-  __pyx_tuple__41 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 16, __pyx_L1_error)
-
-  __pyx_tuple__43 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_xyellw, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -10068,52 +9401,14 @@
     __pyx_ptype_8aixhello_6xyello_xyellw->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_xyellw, (PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8aixhello_6xyello_xyellw) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   #endif
-  #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector_spec, NULL); if (unlikely(!__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector)) __PYX_ERR(0, 115, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector_spec, __pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
-  #else
-  __pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector = &__pyx_type_8aixhello_6xyello___pyx_scope_struct__TrainVector;
-  #endif
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  #endif
-  #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
-  #endif
-  #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector->tp_print = 0;
-  #endif
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector->tp_dictoffset && __pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_8aixhello_6xyello___pyx_scope_struct__TrainVector->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-  }
-  #endif
-  #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 160, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
-  #else
-  __pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr = &__pyx_type_8aixhello_6xyello___pyx_scope_struct_1_genexpr;
-  #endif
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  #endif
-  #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
-  #endif
-  #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr->tp_print = 0;
-  #endif
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr->tp_dictoffset && __pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_8aixhello_6xyello___pyx_scope_struct_1_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-  }
-  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -10493,100 +9788,100 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_base64, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_base64, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_1Decipherx, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decipherx, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decipherx, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_3Encapseal, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Encapseal, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Encapseal, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_5Decenigma, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_Decenigma, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_Decenigma, __pyx_t_2) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbed, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_7vectorizeEmbed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeEmbed, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeEmbed, __pyx_t_2) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_9vectorizeText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorizeText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorizeText, __pyx_t_2) < 0) __PYX_ERR(0, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11UpdateVector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_UpdateVector, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_11UpdateVector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_UpdateVector, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_UpdateVector, __pyx_t_2) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13TrainVector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_TrainVector, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_13TrainVector, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_TrainVector, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_TrainVector, __pyx_t_2) < 0) __PYX_ERR(0, 115, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_15limitText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_limitText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_15limitText, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_limitText, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__30);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__28);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_limitText, __pyx_t_2) < 0) __PYX_ERR(0, 165, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_17GraphFEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_GraphFEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_17GraphFEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_GraphFEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_GraphFEncode, __pyx_t_2) < 0) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_19CipherEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_CipherEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_19CipherEncode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_CipherEncode, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_CipherEncode, __pyx_t_2) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_21SignalSimilarity, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SignalSimilarity, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_21SignalSimilarity, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_SignalSimilarity, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_SignalSimilarity, __pyx_t_2) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_23vectorSearch, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorSearch, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_23vectorSearch, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw_vectorSearch, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_vectorSearch, __pyx_t_2) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_25__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_25__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___reduce_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_27__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_6xyellw_27__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_xyellw___setstate_cython, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__40)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8aixhello_6xyello_xyellw, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8aixhello_6xyello_xyellw);
 
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8aixhello_6xyello_1__pyx_unpickle_xyellw, 0, __pyx_n_s_pyx_unpickle_xyellw, NULL, __pyx_n_s_aixhello_xyello, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_xyellw, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -12229,54 +11524,14 @@
 #endif
         return ((double)a == (double)b);
     }
     return __Pyx_PyObject_IsTrueAndDecref(
         PyObject_RichCompare(op1, op2, Py_EQ));
 }
 
-/* RaiseUnboundLocalError */
-static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
-    PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
-}
-
-/* RaiseClosureNameError */
-static CYTHON_INLINE void __Pyx_RaiseClosureNameError(const char *varname) {
-    PyErr_Format(PyExc_NameError, "free variable '%s' referenced before assignment in enclosing scope", varname);
-}
-
-/* pep479 */
-static void __Pyx_Generator_Replace_StopIteration(int in_async_gen) {
-    PyObject *exc, *val, *tb, *cur_exc;
-    __Pyx_PyThreadState_declare
-    #ifdef __Pyx_StopAsyncIteration_USED
-    int is_async_stopiteration = 0;
-    #endif
-    CYTHON_MAYBE_UNUSED_VAR(in_async_gen);
-    cur_exc = PyErr_Occurred();
-    if (likely(!__Pyx_PyErr_GivenExceptionMatches(cur_exc, PyExc_StopIteration))) {
-        #ifdef __Pyx_StopAsyncIteration_USED
-        if (in_async_gen && unlikely(__Pyx_PyErr_GivenExceptionMatches(cur_exc, __Pyx_PyExc_StopAsyncIteration))) {
-            is_async_stopiteration = 1;
-        } else
-        #endif
-            return;
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_GetException(&exc, &val, &tb);
-    Py_XDECREF(exc);
-    Py_XDECREF(val);
-    Py_XDECREF(tb);
-    PyErr_SetString(PyExc_RuntimeError,
-        #ifdef __Pyx_StopAsyncIteration_USED
-        is_async_stopiteration ? "async generator raised StopAsyncIteration" :
-        in_async_gen ? "async generator raised StopIteration" :
-        #endif
-        "generator raised StopIteration");
-}
-
 /* DictGetItem */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
     PyObject *value;
     value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
         if (!PyErr_Occurred()) {
@@ -12596,15 +11851,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__13);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__11);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -15674,1134 +14929,20 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__45);
+        name = __Pyx_NewRef(__pyx_n_s__43);
     }
     return name;
 }
 #endif
 
-/* PyObjectCall2Args */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args[3] = {NULL, arg1, arg2};
-    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
-/* PyObjectCallMethod1 */
-#if !(CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2)
-static PyObject* __Pyx__PyObject_CallMethod1(PyObject* method, PyObject* arg) {
-    PyObject *result = __Pyx_PyObject_CallOneArg(method, arg);
-    Py_DECREF(method);
-    return result;
-}
-#endif
-static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg) {
-#if CYTHON_VECTORCALL && __PYX_LIMITED_VERSION_HEX >= 0x030C00A2
-    PyObject *args[2] = {obj, arg};
-    (void) __Pyx_PyObject_GetMethod;
-    (void) __Pyx_PyObject_CallOneArg;
-    (void) __Pyx_PyObject_Call2Args;
-    return PyObject_VectorcallMethod(method_name, args, 2 | PY_VECTORCALL_ARGUMENTS_OFFSET, NULL);
-#else
-    PyObject *method = NULL, *result;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_Call2Args(method, obj, arg);
-        Py_DECREF(method);
-        return result;
-    }
-    if (unlikely(!method)) return NULL;
-    return __Pyx__PyObject_CallMethod1(method, arg);
-#endif
-}
-
-/* CoroutineBase */
-#include <frameobject.h>
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-#define __Pyx_Coroutine_Undelegate(gen) Py_CLEAR((gen)->yieldfrom)
-static int __Pyx_PyGen__FetchStopIterationValue(PyThreadState *__pyx_tstate, PyObject **pvalue) {
-    PyObject *et, *ev, *tb;
-    PyObject *value = NULL;
-    CYTHON_UNUSED_VAR(__pyx_tstate);
-    __Pyx_ErrFetch(&et, &ev, &tb);
-    if (!et) {
-        Py_XDECREF(tb);
-        Py_XDECREF(ev);
-        Py_INCREF(Py_None);
-        *pvalue = Py_None;
-        return 0;
-    }
-    if (likely(et == PyExc_StopIteration)) {
-        if (!ev) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#if PY_VERSION_HEX >= 0x030300A0
-        else if (likely(__Pyx_IS_TYPE(ev, (PyTypeObject*)PyExc_StopIteration))) {
-            value = ((PyStopIterationObject *)ev)->value;
-            Py_INCREF(value);
-            Py_DECREF(ev);
-        }
-#endif
-        else if (unlikely(PyTuple_Check(ev))) {
-            if (PyTuple_GET_SIZE(ev) >= 1) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                value = PyTuple_GET_ITEM(ev, 0);
-                Py_INCREF(value);
-#else
-                value = PySequence_ITEM(ev, 0);
-#endif
-            } else {
-                Py_INCREF(Py_None);
-                value = Py_None;
-            }
-            Py_DECREF(ev);
-        }
-        else if (!__Pyx_TypeCheck(ev, (PyTypeObject*)PyExc_StopIteration)) {
-            value = ev;
-        }
-        if (likely(value)) {
-            Py_XDECREF(tb);
-            Py_DECREF(et);
-            *pvalue = value;
-            return 0;
-        }
-    } else if (!__Pyx_PyErr_GivenExceptionMatches(et, PyExc_StopIteration)) {
-        __Pyx_ErrRestore(et, ev, tb);
-        return -1;
-    }
-    PyErr_NormalizeException(&et, &ev, &tb);
-    if (unlikely(!PyObject_TypeCheck(ev, (PyTypeObject*)PyExc_StopIteration))) {
-        __Pyx_ErrRestore(et, ev, tb);
-        return -1;
-    }
-    Py_XDECREF(tb);
-    Py_DECREF(et);
-#if PY_VERSION_HEX >= 0x030300A0
-    value = ((PyStopIterationObject *)ev)->value;
-    Py_INCREF(value);
-    Py_DECREF(ev);
-#else
-    {
-        PyObject* args = __Pyx_PyObject_GetAttrStr(ev, __pyx_n_s_args);
-        Py_DECREF(ev);
-        if (likely(args)) {
-            value = PySequence_GetItem(args, 0);
-            Py_DECREF(args);
-        }
-        if (unlikely(!value)) {
-            __Pyx_ErrRestore(NULL, NULL, NULL);
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-    }
-#endif
-    *pvalue = value;
-    return 0;
-}
-static CYTHON_INLINE
-void __Pyx_Coroutine_ExceptionClear(__Pyx_ExcInfoStruct *exc_state) {
-#if PY_VERSION_HEX >= 0x030B00a4
-    Py_CLEAR(exc_state->exc_value);
-#else
-    PyObject *t, *v, *tb;
-    t = exc_state->exc_type;
-    v = exc_state->exc_value;
-    tb = exc_state->exc_traceback;
-    exc_state->exc_type = NULL;
-    exc_state->exc_value = NULL;
-    exc_state->exc_traceback = NULL;
-    Py_XDECREF(t);
-    Py_XDECREF(v);
-    Py_XDECREF(tb);
-#endif
-}
-#define __Pyx_Coroutine_AlreadyRunningError(gen)  (__Pyx__Coroutine_AlreadyRunningError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyRunningError(__pyx_CoroutineObject *gen) {
-    const char *msg;
-    CYTHON_MAYBE_UNUSED_VAR(gen);
-    if ((0)) {
-    #ifdef __Pyx_Coroutine_USED
-    } else if (__Pyx_Coroutine_Check((PyObject*)gen)) {
-        msg = "coroutine already executing";
-    #endif
-    #ifdef __Pyx_AsyncGen_USED
-    } else if (__Pyx_AsyncGen_CheckExact((PyObject*)gen)) {
-        msg = "async generator already executing";
-    #endif
-    } else {
-        msg = "generator already executing";
-    }
-    PyErr_SetString(PyExc_ValueError, msg);
-}
-#define __Pyx_Coroutine_NotStartedError(gen)  (__Pyx__Coroutine_NotStartedError(gen), (PyObject*)NULL)
-static void __Pyx__Coroutine_NotStartedError(PyObject *gen) {
-    const char *msg;
-    CYTHON_MAYBE_UNUSED_VAR(gen);
-    if ((0)) {
-    #ifdef __Pyx_Coroutine_USED
-    } else if (__Pyx_Coroutine_Check(gen)) {
-        msg = "can't send non-None value to a just-started coroutine";
-    #endif
-    #ifdef __Pyx_AsyncGen_USED
-    } else if (__Pyx_AsyncGen_CheckExact(gen)) {
-        msg = "can't send non-None value to a just-started async generator";
-    #endif
-    } else {
-        msg = "can't send non-None value to a just-started generator";
-    }
-    PyErr_SetString(PyExc_TypeError, msg);
-}
-#define __Pyx_Coroutine_AlreadyTerminatedError(gen, value, closing)  (__Pyx__Coroutine_AlreadyTerminatedError(gen, value, closing), (PyObject*)NULL)
-static void __Pyx__Coroutine_AlreadyTerminatedError(PyObject *gen, PyObject *value, int closing) {
-    CYTHON_MAYBE_UNUSED_VAR(gen);
-    CYTHON_MAYBE_UNUSED_VAR(closing);
-    #ifdef __Pyx_Coroutine_USED
-    if (!closing && __Pyx_Coroutine_Check(gen)) {
-        PyErr_SetString(PyExc_RuntimeError, "cannot reuse already awaited coroutine");
-    } else
-    #endif
-    if (value) {
-        #ifdef __Pyx_AsyncGen_USED
-        if (__Pyx_AsyncGen_CheckExact(gen))
-            PyErr_SetNone(__Pyx_PyExc_StopAsyncIteration);
-        else
-        #endif
-        PyErr_SetNone(PyExc_StopIteration);
-    }
-}
-static
-PyObject *__Pyx_Coroutine_SendEx(__pyx_CoroutineObject *self, PyObject *value, int closing) {
-    __Pyx_PyThreadState_declare
-    PyThreadState *tstate;
-    __Pyx_ExcInfoStruct *exc_state;
-    PyObject *retval;
-    assert(!self->is_running);
-    if (unlikely(self->resume_label == 0)) {
-        if (unlikely(value && value != Py_None)) {
-            return __Pyx_Coroutine_NotStartedError((PyObject*)self);
-        }
-    }
-    if (unlikely(self->resume_label == -1)) {
-        return __Pyx_Coroutine_AlreadyTerminatedError((PyObject*)self, value, closing);
-    }
-#if CYTHON_FAST_THREAD_STATE
-    __Pyx_PyThreadState_assign
-    tstate = __pyx_tstate;
-#else
-    tstate = __Pyx_PyThreadState_Current;
-#endif
-    exc_state = &self->gi_exc_state;
-    if (exc_state->exc_value) {
-        #if CYTHON_COMPILING_IN_PYPY
-        #else
-        PyObject *exc_tb;
-        #if PY_VERSION_HEX >= 0x030B00a4 && !CYTHON_COMPILING_IN_CPYTHON
-        exc_tb = PyException_GetTraceback(exc_state->exc_value);
-        #elif PY_VERSION_HEX >= 0x030B00a4
-        exc_tb = ((PyBaseExceptionObject*) exc_state->exc_value)->traceback;
-        #else
-        exc_tb = exc_state->exc_traceback;
-        #endif
-        if (exc_tb) {
-            PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
-            PyFrameObject *f = tb->tb_frame;
-            assert(f->f_back == NULL);
-            #if PY_VERSION_HEX >= 0x030B00A1
-            f->f_back = PyThreadState_GetFrame(tstate);
-            #else
-            Py_XINCREF(tstate->frame);
-            f->f_back = tstate->frame;
-            #endif
-            #if PY_VERSION_HEX >= 0x030B00a4 && !CYTHON_COMPILING_IN_CPYTHON
-            Py_DECREF(exc_tb);
-            #endif
-        }
-        #endif
-    }
-#if CYTHON_USE_EXC_INFO_STACK
-    exc_state->previous_item = tstate->exc_info;
-    tstate->exc_info = exc_state;
-#else
-    if (exc_state->exc_type) {
-        __Pyx_ExceptionSwap(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
-    } else {
-        __Pyx_Coroutine_ExceptionClear(exc_state);
-        __Pyx_ExceptionSave(&exc_state->exc_type, &exc_state->exc_value, &exc_state->exc_traceback);
-    }
-#endif
-    self->is_running = 1;
-    retval = self->body(self, tstate, value);
-    self->is_running = 0;
-#if CYTHON_USE_EXC_INFO_STACK
-    exc_state = &self->gi_exc_state;
-    tstate->exc_info = exc_state->previous_item;
-    exc_state->previous_item = NULL;
-    __Pyx_Coroutine_ResetFrameBackpointer(exc_state);
-#endif
-    return retval;
-}
-static CYTHON_INLINE void __Pyx_Coroutine_ResetFrameBackpointer(__Pyx_ExcInfoStruct *exc_state) {
-#if CYTHON_COMPILING_IN_PYPY
-    CYTHON_UNUSED_VAR(exc_state);
-#else
-    PyObject *exc_tb;
-    #if PY_VERSION_HEX >= 0x030B00a4
-    if (!exc_state->exc_value) return;
-    exc_tb = PyException_GetTraceback(exc_state->exc_value);
-    #else
-    exc_tb = exc_state->exc_traceback;
-    #endif
-    if (likely(exc_tb)) {
-        PyTracebackObject *tb = (PyTracebackObject *) exc_tb;
-        PyFrameObject *f = tb->tb_frame;
-        Py_CLEAR(f->f_back);
-        #if PY_VERSION_HEX >= 0x030B00a4
-        Py_DECREF(exc_tb);
-        #endif
-    }
-#endif
-}
-static CYTHON_INLINE
-PyObject *__Pyx_Coroutine_MethodReturn(PyObject* gen, PyObject *retval) {
-    CYTHON_MAYBE_UNUSED_VAR(gen);
-    if (unlikely(!retval)) {
-        __Pyx_PyThreadState_declare
-        __Pyx_PyThreadState_assign
-        if (!__Pyx_PyErr_Occurred()) {
-            PyObject *exc = PyExc_StopIteration;
-            #ifdef __Pyx_AsyncGen_USED
-            if (__Pyx_AsyncGen_CheckExact(gen))
-                exc = __Pyx_PyExc_StopAsyncIteration;
-            #endif
-            __Pyx_PyErr_SetNone(exc);
-        }
-    }
-    return retval;
-}
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-static CYTHON_INLINE
-PyObject *__Pyx_PyGen_Send(PyGenObject *gen, PyObject *arg) {
-#if PY_VERSION_HEX <= 0x030A00A1
-    return _PyGen_Send(gen, arg);
-#else
-    PyObject *result;
-    if (PyIter_Send((PyObject*)gen, arg ? arg : Py_None, &result) == PYGEN_RETURN) {
-        if (PyAsyncGen_CheckExact(gen)) {
-            assert(result == Py_None);
-            PyErr_SetNone(PyExc_StopAsyncIteration);
-        }
-        else if (result == Py_None) {
-            PyErr_SetNone(PyExc_StopIteration);
-        }
-        else {
-#if PY_VERSION_HEX < 0x030d00A1
-            _PyGen_SetStopIterationValue(result);
-#else
-            if (!PyTuple_Check(result) && !PyExceptionInstance_Check(result)) {
-                PyErr_SetObject(PyExc_StopIteration, result);
-            } else {
-                PyObject *exc = __Pyx_PyObject_CallOneArg(PyExc_StopIteration, result);
-                if (likely(exc != NULL)) {
-                    PyErr_SetObject(PyExc_StopIteration, exc);
-                    Py_DECREF(exc);
-                }
-            }
-#endif
-        }
-        Py_DECREF(result);
-        result = NULL;
-    }
-    return result;
-#endif
-}
-#endif
-static CYTHON_INLINE
-PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
-    PyObject *ret;
-    PyObject *val = NULL;
-    __Pyx_Coroutine_Undelegate(gen);
-    __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, &val);
-    ret = __Pyx_Coroutine_SendEx(gen, val, 0);
-    Py_XDECREF(val);
-    return ret;
-}
-static PyObject *__Pyx_Coroutine_Send(PyObject *self, PyObject *value) {
-    PyObject *retval;
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject*) self;
-    PyObject *yf = gen->yieldfrom;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        PyObject *ret;
-        gen->is_running = 1;
-        #ifdef __Pyx_Generator_USED
-        if (__Pyx_Generator_CheckExact(yf)) {
-            ret = __Pyx_Coroutine_Send(yf, value);
-        } else
-        #endif
-        #ifdef __Pyx_Coroutine_USED
-        if (__Pyx_Coroutine_Check(yf)) {
-            ret = __Pyx_Coroutine_Send(yf, value);
-        } else
-        #endif
-        #ifdef __Pyx_AsyncGen_USED
-        if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
-            ret = __Pyx_async_gen_asend_send(yf, value);
-        } else
-        #endif
-        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-        if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
-        } else
-        #endif
-        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-        if (PyCoro_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
-        } else
-        #endif
-        {
-            if (value == Py_None)
-                ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
-            else
-                ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
-        }
-        gen->is_running = 0;
-        if (likely(ret)) {
-            return ret;
-        }
-        retval = __Pyx_Coroutine_FinishDelegation(gen);
-    } else {
-        retval = __Pyx_Coroutine_SendEx(gen, value, 0);
-    }
-    return __Pyx_Coroutine_MethodReturn(self, retval);
-}
-static int __Pyx_Coroutine_CloseIter(__pyx_CoroutineObject *gen, PyObject *yf) {
-    PyObject *retval = NULL;
-    int err = 0;
-    #ifdef __Pyx_Generator_USED
-    if (__Pyx_Generator_CheckExact(yf)) {
-        retval = __Pyx_Coroutine_Close(yf);
-        if (!retval)
-            return -1;
-    } else
-    #endif
-    #ifdef __Pyx_Coroutine_USED
-    if (__Pyx_Coroutine_Check(yf)) {
-        retval = __Pyx_Coroutine_Close(yf);
-        if (!retval)
-            return -1;
-    } else
-    if (__Pyx_CoroutineAwait_CheckExact(yf)) {
-        retval = __Pyx_CoroutineAwait_Close((__pyx_CoroutineAwaitObject*)yf, NULL);
-        if (!retval)
-            return -1;
-    } else
-    #endif
-    #ifdef __Pyx_AsyncGen_USED
-    if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
-        retval = __Pyx_async_gen_asend_close(yf, NULL);
-    } else
-    if (__pyx_PyAsyncGenAThrow_CheckExact(yf)) {
-        retval = __Pyx_async_gen_athrow_close(yf, NULL);
-    } else
-    #endif
-    {
-        PyObject *meth;
-        gen->is_running = 1;
-        meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_close);
-        if (unlikely(!meth)) {
-            if (unlikely(PyErr_Occurred())) {
-                PyErr_WriteUnraisable(yf);
-            }
-        } else {
-            retval = __Pyx_PyObject_CallNoArg(meth);
-            Py_DECREF(meth);
-            if (unlikely(!retval))
-                err = -1;
-        }
-        gen->is_running = 0;
-    }
-    Py_XDECREF(retval);
-    return err;
-}
-static PyObject *__Pyx_Generator_Next(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject*) self;
-    PyObject *yf = gen->yieldfrom;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        PyObject *ret;
-        gen->is_running = 1;
-        #ifdef __Pyx_Generator_USED
-        if (__Pyx_Generator_CheckExact(yf)) {
-            ret = __Pyx_Generator_Next(yf);
-        } else
-        #endif
-        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-        if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, NULL);
-        } else
-        #endif
-        #ifdef __Pyx_Coroutine_USED
-        if (__Pyx_Coroutine_Check(yf)) {
-            ret = __Pyx_Coroutine_Send(yf, Py_None);
-        } else
-        #endif
-            ret = __Pyx_PyObject_GetIterNextFunc(yf)(yf);
-        gen->is_running = 0;
-        if (likely(ret)) {
-            return ret;
-        }
-        return __Pyx_Coroutine_FinishDelegation(gen);
-    }
-    return __Pyx_Coroutine_SendEx(gen, Py_None, 0);
-}
-static PyObject *__Pyx_Coroutine_Close_Method(PyObject *self, PyObject *arg) {
-    CYTHON_UNUSED_VAR(arg);
-    return __Pyx_Coroutine_Close(self);
-}
-static PyObject *__Pyx_Coroutine_Close(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    PyObject *retval, *raised_exception;
-    PyObject *yf = gen->yieldfrom;
-    int err = 0;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        Py_INCREF(yf);
-        err = __Pyx_Coroutine_CloseIter(gen, yf);
-        __Pyx_Coroutine_Undelegate(gen);
-        Py_DECREF(yf);
-    }
-    if (err == 0)
-        PyErr_SetNone(PyExc_GeneratorExit);
-    retval = __Pyx_Coroutine_SendEx(gen, NULL, 1);
-    if (unlikely(retval)) {
-        const char *msg;
-        Py_DECREF(retval);
-        if ((0)) {
-        #ifdef __Pyx_Coroutine_USED
-        } else if (__Pyx_Coroutine_Check(self)) {
-            msg = "coroutine ignored GeneratorExit";
-        #endif
-        #ifdef __Pyx_AsyncGen_USED
-        } else if (__Pyx_AsyncGen_CheckExact(self)) {
-#if PY_VERSION_HEX < 0x03060000
-            msg = "async generator ignored GeneratorExit - might require Python 3.6+ finalisation (PEP 525)";
-#else
-            msg = "async generator ignored GeneratorExit";
-#endif
-        #endif
-        } else {
-            msg = "generator ignored GeneratorExit";
-        }
-        PyErr_SetString(PyExc_RuntimeError, msg);
-        return NULL;
-    }
-    raised_exception = PyErr_Occurred();
-    if (likely(!raised_exception || __Pyx_PyErr_GivenExceptionMatches2(raised_exception, PyExc_GeneratorExit, PyExc_StopIteration))) {
-        if (raised_exception) PyErr_Clear();
-        Py_INCREF(Py_None);
-        return Py_None;
-    }
-    return NULL;
-}
-static PyObject *__Pyx__Coroutine_Throw(PyObject *self, PyObject *typ, PyObject *val, PyObject *tb,
-                                        PyObject *args, int close_on_genexit) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    PyObject *yf = gen->yieldfrom;
-    if (unlikely(gen->is_running))
-        return __Pyx_Coroutine_AlreadyRunningError(gen);
-    if (yf) {
-        PyObject *ret;
-        Py_INCREF(yf);
-        if (__Pyx_PyErr_GivenExceptionMatches(typ, PyExc_GeneratorExit) && close_on_genexit) {
-            int err = __Pyx_Coroutine_CloseIter(gen, yf);
-            Py_DECREF(yf);
-            __Pyx_Coroutine_Undelegate(gen);
-            if (err < 0)
-                return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
-            goto throw_here;
-        }
-        gen->is_running = 1;
-        if (0
-        #ifdef __Pyx_Generator_USED
-            || __Pyx_Generator_CheckExact(yf)
-        #endif
-        #ifdef __Pyx_Coroutine_USED
-            || __Pyx_Coroutine_Check(yf)
-        #endif
-            ) {
-            ret = __Pyx__Coroutine_Throw(yf, typ, val, tb, args, close_on_genexit);
-        #ifdef __Pyx_Coroutine_USED
-        } else if (__Pyx_CoroutineAwait_CheckExact(yf)) {
-            ret = __Pyx__Coroutine_Throw(((__pyx_CoroutineAwaitObject*)yf)->coroutine, typ, val, tb, args, close_on_genexit);
-        #endif
-        } else {
-            PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(yf, __pyx_n_s_throw);
-            if (unlikely(!meth)) {
-                Py_DECREF(yf);
-                if (unlikely(PyErr_Occurred())) {
-                    gen->is_running = 0;
-                    return NULL;
-                }
-                __Pyx_Coroutine_Undelegate(gen);
-                gen->is_running = 0;
-                goto throw_here;
-            }
-            if (likely(args)) {
-                ret = __Pyx_PyObject_Call(meth, args, NULL);
-            } else {
-                PyObject *cargs[4] = {NULL, typ, val, tb};
-                ret = __Pyx_PyObject_FastCall(meth, cargs+1, 3 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-            }
-            Py_DECREF(meth);
-        }
-        gen->is_running = 0;
-        Py_DECREF(yf);
-        if (!ret) {
-            ret = __Pyx_Coroutine_FinishDelegation(gen);
-        }
-        return __Pyx_Coroutine_MethodReturn(self, ret);
-    }
-throw_here:
-    __Pyx_Raise(typ, val, tb, NULL);
-    return __Pyx_Coroutine_MethodReturn(self, __Pyx_Coroutine_SendEx(gen, NULL, 0));
-}
-static PyObject *__Pyx_Coroutine_Throw(PyObject *self, PyObject *args) {
-    PyObject *typ;
-    PyObject *val = NULL;
-    PyObject *tb = NULL;
-    if (unlikely(!PyArg_UnpackTuple(args, (char *)"throw", 1, 3, &typ, &val, &tb)))
-        return NULL;
-    return __Pyx__Coroutine_Throw(self, typ, val, tb, args, 1);
-}
-static CYTHON_INLINE int __Pyx_Coroutine_traverse_excstate(__Pyx_ExcInfoStruct *exc_state, visitproc visit, void *arg) {
-#if PY_VERSION_HEX >= 0x030B00a4
-    Py_VISIT(exc_state->exc_value);
-#else
-    Py_VISIT(exc_state->exc_type);
-    Py_VISIT(exc_state->exc_value);
-    Py_VISIT(exc_state->exc_traceback);
-#endif
-    return 0;
-}
-static int __Pyx_Coroutine_traverse(__pyx_CoroutineObject *gen, visitproc visit, void *arg) {
-    Py_VISIT(gen->closure);
-    Py_VISIT(gen->classobj);
-    Py_VISIT(gen->yieldfrom);
-    return __Pyx_Coroutine_traverse_excstate(&gen->gi_exc_state, visit, arg);
-}
-static int __Pyx_Coroutine_clear(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    Py_CLEAR(gen->closure);
-    Py_CLEAR(gen->classobj);
-    Py_CLEAR(gen->yieldfrom);
-    __Pyx_Coroutine_ExceptionClear(&gen->gi_exc_state);
-#ifdef __Pyx_AsyncGen_USED
-    if (__Pyx_AsyncGen_CheckExact(self)) {
-        Py_CLEAR(((__pyx_PyAsyncGenObject*)gen)->ag_finalizer);
-    }
-#endif
-    Py_CLEAR(gen->gi_code);
-    Py_CLEAR(gen->gi_frame);
-    Py_CLEAR(gen->gi_name);
-    Py_CLEAR(gen->gi_qualname);
-    Py_CLEAR(gen->gi_modulename);
-    return 0;
-}
-static void __Pyx_Coroutine_dealloc(PyObject *self) {
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    PyObject_GC_UnTrack(gen);
-    if (gen->gi_weakreflist != NULL)
-        PyObject_ClearWeakRefs(self);
-    if (gen->resume_label >= 0) {
-        PyObject_GC_Track(self);
-#if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
-        if (unlikely(PyObject_CallFinalizerFromDealloc(self)))
-#else
-        Py_TYPE(gen)->tp_del(self);
-        if (unlikely(Py_REFCNT(self) > 0))
-#endif
-        {
-            return;
-        }
-        PyObject_GC_UnTrack(self);
-    }
-#ifdef __Pyx_AsyncGen_USED
-    if (__Pyx_AsyncGen_CheckExact(self)) {
-        /* We have to handle this case for asynchronous generators
-           right here, because this code has to be between UNTRACK
-           and GC_Del. */
-        Py_CLEAR(((__pyx_PyAsyncGenObject*)self)->ag_finalizer);
-    }
-#endif
-    __Pyx_Coroutine_clear(self);
-    __Pyx_PyHeapTypeObject_GC_Del(gen);
-}
-static void __Pyx_Coroutine_del(PyObject *self) {
-    PyObject *error_type, *error_value, *error_traceback;
-    __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
-    __Pyx_PyThreadState_declare
-    if (gen->resume_label < 0) {
-        return;
-    }
-#if !CYTHON_USE_TP_FINALIZE
-    assert(self->ob_refcnt == 0);
-    __Pyx_SET_REFCNT(self, 1);
-#endif
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&error_type, &error_value, &error_traceback);
-#ifdef __Pyx_AsyncGen_USED
-    if (__Pyx_AsyncGen_CheckExact(self)) {
-        __pyx_PyAsyncGenObject *agen = (__pyx_PyAsyncGenObject*)self;
-        PyObject *finalizer = agen->ag_finalizer;
-        if (finalizer && !agen->ag_closed) {
-            PyObject *res = __Pyx_PyObject_CallOneArg(finalizer, self);
-            if (unlikely(!res)) {
-                PyErr_WriteUnraisable(self);
-            } else {
-                Py_DECREF(res);
-            }
-            __Pyx_ErrRestore(error_type, error_value, error_traceback);
-            return;
-        }
-    }
-#endif
-    if (unlikely(gen->resume_label == 0 && !error_value)) {
-#ifdef __Pyx_Coroutine_USED
-#ifdef __Pyx_Generator_USED
-    if (!__Pyx_Generator_CheckExact(self))
-#endif
-        {
-        PyObject_GC_UnTrack(self);
-#if PY_MAJOR_VERSION >= 3  || defined(PyErr_WarnFormat)
-        if (unlikely(PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "coroutine '%.50S' was never awaited", gen->gi_qualname) < 0))
-            PyErr_WriteUnraisable(self);
-#else
-        {PyObject *msg;
-        char *cmsg;
-        #if CYTHON_COMPILING_IN_PYPY
-        msg = NULL;
-        cmsg = (char*) "coroutine was never awaited";
-        #else
-        char *cname;
-        PyObject *qualname;
-        qualname = gen->gi_qualname;
-        cname = PyString_AS_STRING(qualname);
-        msg = PyString_FromFormat("coroutine '%.50s' was never awaited", cname);
-        if (unlikely(!msg)) {
-            PyErr_Clear();
-            cmsg = (char*) "coroutine was never awaited";
-        } else {
-            cmsg = PyString_AS_STRING(msg);
-        }
-        #endif
-        if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, cmsg, 1) < 0))
-            PyErr_WriteUnraisable(self);
-        Py_XDECREF(msg);}
-#endif
-        PyObject_GC_Track(self);
-        }
-#endif
-    } else {
-        PyObject *res = __Pyx_Coroutine_Close(self);
-        if (unlikely(!res)) {
-            if (PyErr_Occurred())
-                PyErr_WriteUnraisable(self);
-        } else {
-            Py_DECREF(res);
-        }
-    }
-    __Pyx_ErrRestore(error_type, error_value, error_traceback);
-#if !CYTHON_USE_TP_FINALIZE
-    assert(Py_REFCNT(self) > 0);
-    if (likely(--self->ob_refcnt == 0)) {
-        return;
-    }
-    {
-        Py_ssize_t refcnt = Py_REFCNT(self);
-        _Py_NewReference(self);
-        __Pyx_SET_REFCNT(self, refcnt);
-    }
-#if CYTHON_COMPILING_IN_CPYTHON
-    assert(PyType_IS_GC(Py_TYPE(self)) &&
-           _Py_AS_GC(self)->gc.gc_refs != _PyGC_REFS_UNTRACKED);
-    _Py_DEC_REFTOTAL;
-#endif
-#ifdef COUNT_ALLOCS
-    --Py_TYPE(self)->tp_frees;
-    --Py_TYPE(self)->tp_allocs;
-#endif
-#endif
-}
-static PyObject *
-__Pyx_Coroutine_get_name(__pyx_CoroutineObject *self, void *context)
-{
-    PyObject *name = self->gi_name;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!name)) name = Py_None;
-    Py_INCREF(name);
-    return name;
-}
-static int
-__Pyx_Coroutine_set_name(__pyx_CoroutineObject *self, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__name__ must be set to a string object");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(self->gi_name, value);
-    return 0;
-}
-static PyObject *
-__Pyx_Coroutine_get_qualname(__pyx_CoroutineObject *self, void *context)
-{
-    PyObject *name = self->gi_qualname;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!name)) name = Py_None;
-    Py_INCREF(name);
-    return name;
-}
-static int
-__Pyx_Coroutine_set_qualname(__pyx_CoroutineObject *self, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__qualname__ must be set to a string object");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(self->gi_qualname, value);
-    return 0;
-}
-static PyObject *
-__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, void *context)
-{
-    PyObject *frame = self->gi_frame;
-    CYTHON_UNUSED_VAR(context);
-    if (!frame) {
-        if (unlikely(!self->gi_code)) {
-            Py_RETURN_NONE;
-        }
-        frame = (PyObject *) PyFrame_New(
-            PyThreadState_Get(),            /*PyThreadState *tstate,*/
-            (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
-            __pyx_d,                 /*PyObject *globals,*/
-            0                               /*PyObject *locals*/
-        );
-        if (unlikely(!frame))
-            return NULL;
-        self->gi_frame = frame;
-    }
-    Py_INCREF(frame);
-    return frame;
-}
-static __pyx_CoroutineObject *__Pyx__Coroutine_New(
-            PyTypeObject* type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-            PyObject *name, PyObject *qualname, PyObject *module_name) {
-    __pyx_CoroutineObject *gen = PyObject_GC_New(__pyx_CoroutineObject, type);
-    if (unlikely(!gen))
-        return NULL;
-    return __Pyx__Coroutine_NewInit(gen, body, code, closure, name, qualname, module_name);
-}
-static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
-            __pyx_CoroutineObject *gen, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
-            PyObject *name, PyObject *qualname, PyObject *module_name) {
-    gen->body = body;
-    gen->closure = closure;
-    Py_XINCREF(closure);
-    gen->is_running = 0;
-    gen->resume_label = 0;
-    gen->classobj = NULL;
-    gen->yieldfrom = NULL;
-    #if PY_VERSION_HEX >= 0x030B00a4
-    gen->gi_exc_state.exc_value = NULL;
-    #else
-    gen->gi_exc_state.exc_type = NULL;
-    gen->gi_exc_state.exc_value = NULL;
-    gen->gi_exc_state.exc_traceback = NULL;
-    #endif
-#if CYTHON_USE_EXC_INFO_STACK
-    gen->gi_exc_state.previous_item = NULL;
-#endif
-    gen->gi_weakreflist = NULL;
-    Py_XINCREF(qualname);
-    gen->gi_qualname = qualname;
-    Py_XINCREF(name);
-    gen->gi_name = name;
-    Py_XINCREF(module_name);
-    gen->gi_modulename = module_name;
-    Py_XINCREF(code);
-    gen->gi_code = code;
-    gen->gi_frame = NULL;
-    PyObject_GC_Track(gen);
-    return gen;
-}
-
-/* PatchModuleWithCoroutine */
-static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
-#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-    int result;
-    PyObject *globals, *result_obj;
-    globals = PyDict_New();  if (unlikely(!globals)) goto ignore;
-    result = PyDict_SetItemString(globals, "_cython_coroutine_type",
-    #ifdef __Pyx_Coroutine_USED
-        (PyObject*)__pyx_CoroutineType);
-    #else
-        Py_None);
-    #endif
-    if (unlikely(result < 0)) goto ignore;
-    result = PyDict_SetItemString(globals, "_cython_generator_type",
-    #ifdef __Pyx_Generator_USED
-        (PyObject*)__pyx_GeneratorType);
-    #else
-        Py_None);
-    #endif
-    if (unlikely(result < 0)) goto ignore;
-    if (unlikely(PyDict_SetItemString(globals, "_module", module) < 0)) goto ignore;
-    if (unlikely(PyDict_SetItemString(globals, "__builtins__", __pyx_b) < 0)) goto ignore;
-    result_obj = PyRun_String(py_code, Py_file_input, globals, globals);
-    if (unlikely(!result_obj)) goto ignore;
-    Py_DECREF(result_obj);
-    Py_DECREF(globals);
-    return module;
-ignore:
-    Py_XDECREF(globals);
-    PyErr_WriteUnraisable(module);
-    if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning, "Cython module failed to patch module with custom type", 1) < 0)) {
-        Py_DECREF(module);
-        module = NULL;
-    }
-#else
-    py_code++;
-#endif
-    return module;
-}
-
-/* PatchGeneratorABC */
-#ifndef CYTHON_REGISTER_ABCS
-#define CYTHON_REGISTER_ABCS 1
-#endif
-#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-static PyObject* __Pyx_patch_abc_module(PyObject *module);
-static PyObject* __Pyx_patch_abc_module(PyObject *module) {
-    module = __Pyx_Coroutine_patch_module(
-        module, ""
-"if _cython_generator_type is not None:\n"
-"    try: Generator = _module.Generator\n"
-"    except AttributeError: pass\n"
-"    else: Generator.register(_cython_generator_type)\n"
-"if _cython_coroutine_type is not None:\n"
-"    try: Coroutine = _module.Coroutine\n"
-"    except AttributeError: pass\n"
-"    else: Coroutine.register(_cython_coroutine_type)\n"
-    );
-    return module;
-}
-#endif
-static int __Pyx_patch_abc(void) {
-#if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
-    static int abc_patched = 0;
-    if (CYTHON_REGISTER_ABCS && !abc_patched) {
-        PyObject *module;
-        module = PyImport_ImportModule((PY_MAJOR_VERSION >= 3) ? "collections.abc" : "collections");
-        if (unlikely(!module)) {
-            PyErr_WriteUnraisable(NULL);
-            if (unlikely(PyErr_WarnEx(PyExc_RuntimeWarning,
-                    ((PY_MAJOR_VERSION >= 3) ?
-                        "Cython module failed to register with collections.abc module" :
-                        "Cython module failed to register with collections module"), 1) < 0)) {
-                return -1;
-            }
-        } else {
-            module = __Pyx_patch_abc_module(module);
-            abc_patched = 1;
-            if (unlikely(!module))
-                return -1;
-            Py_DECREF(module);
-        }
-        module = PyImport_ImportModule("backports_abc");
-        if (module) {
-            module = __Pyx_patch_abc_module(module);
-            Py_XDECREF(module);
-        }
-        if (!module) {
-            PyErr_Clear();
-        }
-    }
-#else
-    if ((0)) __Pyx_Coroutine_patch_module(NULL, NULL);
-#endif
-    return 0;
-}
-
-/* Generator */
-static PyMethodDef __pyx_Generator_methods[] = {
-    {"send", (PyCFunction) __Pyx_Coroutine_Send, METH_O,
-     (char*) PyDoc_STR("send(arg) -> send 'arg' into generator,\nreturn next yielded value or raise StopIteration.")},
-    {"throw", (PyCFunction) __Pyx_Coroutine_Throw, METH_VARARGS,
-     (char*) PyDoc_STR("throw(typ[,val[,tb]]) -> raise exception in generator,\nreturn next yielded value or raise StopIteration.")},
-    {"close", (PyCFunction) __Pyx_Coroutine_Close_Method, METH_NOARGS,
-     (char*) PyDoc_STR("close() -> raise GeneratorExit inside generator.")},
-    {0, 0, 0, 0}
-};
-static PyMemberDef __pyx_Generator_memberlist[] = {
-    {(char *) "gi_running", T_BOOL, offsetof(__pyx_CoroutineObject, is_running), READONLY, NULL},
-    {(char*) "gi_yieldfrom", T_OBJECT, offsetof(__pyx_CoroutineObject, yieldfrom), READONLY,
-     (char*) PyDoc_STR("object being iterated by 'yield from', or None")},
-    {(char*) "gi_code", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_code), READONLY, NULL},
-    {(char *) "__module__", T_OBJECT, offsetof(__pyx_CoroutineObject, gi_modulename), 0, 0},
-#if CYTHON_USE_TYPE_SPECS
-    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CoroutineObject, gi_weakreflist), READONLY, 0},
-#endif
-    {0, 0, 0, 0, 0}
-};
-static PyGetSetDef __pyx_Generator_getsets[] = {
-    {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
-     (char*) PyDoc_STR("name of the generator"), 0},
-    {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
-     (char*) PyDoc_STR("qualified name of the generator"), 0},
-    {(char *) "gi_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
-     (char*) PyDoc_STR("Frame of the generator"), 0},
-    {0, 0, 0, 0, 0}
-};
-#if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_GeneratorType_slots[] = {
-    {Py_tp_dealloc, (void *)__Pyx_Coroutine_dealloc},
-    {Py_tp_traverse, (void *)__Pyx_Coroutine_traverse},
-    {Py_tp_iter, (void *)PyObject_SelfIter},
-    {Py_tp_iternext, (void *)__Pyx_Generator_Next},
-    {Py_tp_methods, (void *)__pyx_Generator_methods},
-    {Py_tp_members, (void *)__pyx_Generator_memberlist},
-    {Py_tp_getset, (void *)__pyx_Generator_getsets},
-    {Py_tp_getattro, (void *) __Pyx_PyObject_GenericGetAttrNoDict},
-#if CYTHON_USE_TP_FINALIZE
-    {Py_tp_finalize, (void *)__Pyx_Coroutine_del},
-#endif
-    {0, 0},
-};
-static PyType_Spec __pyx_GeneratorType_spec = {
-    __PYX_TYPE_MODULE_PREFIX "generator",
-    sizeof(__pyx_CoroutineObject),
-    0,
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
-    __pyx_GeneratorType_slots
-};
-#else
-static PyTypeObject __pyx_GeneratorType_type = {
-    PyVarObject_HEAD_INIT(0, 0)
-    __PYX_TYPE_MODULE_PREFIX "generator",
-    sizeof(__pyx_CoroutineObject),
-    0,
-    (destructor) __Pyx_Coroutine_dealloc,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_HAVE_FINALIZE,
-    0,
-    (traverseproc) __Pyx_Coroutine_traverse,
-    0,
-    0,
-    offsetof(__pyx_CoroutineObject, gi_weakreflist),
-    0,
-    (iternextfunc) __Pyx_Generator_Next,
-    __pyx_Generator_methods,
-    __pyx_Generator_memberlist,
-    __pyx_Generator_getsets,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-#if CYTHON_USE_TP_FINALIZE
-    0,
-#else
-    __Pyx_Coroutine_del,
-#endif
-    0,
-#if CYTHON_USE_TP_FINALIZE
-    __Pyx_Coroutine_del,
-#elif PY_VERSION_HEX >= 0x030400a1
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-    0,
-#endif
-#if __PYX_NEED_TP_PRINT_SLOT
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-    0,
-#endif
-};
-#endif
-static int __pyx_Generator_init(PyObject *module) {
-#if CYTHON_USE_TYPE_SPECS
-    __pyx_GeneratorType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_GeneratorType_spec, NULL);
-#else
-    CYTHON_UNUSED_VAR(module);
-    __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
-    __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
-    __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
-#endif
-    if (unlikely(!__pyx_GeneratorType)) {
-        return -1;
-    }
-    return 0;
-}
-
 /* CheckBinaryVersion */
 static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
```

### Comparing `aixhello-4.91/aixhello.egg-info/PKG-INFO` & `aixhello-4.92/aixhello.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.91
+Version: 4.92
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.91/setup.py` & `aixhello-4.92/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='4.91',  
+    version='4.92',  
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

