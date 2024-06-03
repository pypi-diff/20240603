# Comparing `tmp/aixhello-4.7.tar.gz` & `tmp/aixhello-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-4.7.tar", last modified: Mon Jun  3 10:21:16 2024, max compression
+gzip compressed data, was "aixhello-4.9.tar", last modified: Mon Jun  3 10:29:56 2024, max compression
```

## Comparing `aixhello-4.7.tar` & `aixhello-4.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 10:21:16.329091 aixhello-4.7/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.7/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-03 10:21:16.329091 aixhello-4.7/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 10:21:16.299750 aixhello-4.7/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.7/aixhello/__init__.py
--rw-rw-rw-   0        0        0   642328 2024-06-03 10:21:08.000000 aixhello-4.7/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-03 10:21:16.327093 aixhello-4.7/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 10:21:16.000000 aixhello-4.7/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 10:21:16.331093 aixhello-4.7/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-06-03 10:15:05.000000 aixhello-4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 10:29:56.821403 aixhello-4.9/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.9/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-03 10:29:56.821403 aixhello-4.9/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 10:29:56.801396 aixhello-4.9/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.9/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   643520 2024-06-03 10:29:44.000000 aixhello-4.9/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-03 10:29:56.820402 aixhello-4.9/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-03 10:29:56.000000 aixhello-4.9/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-03 10:29:56.000000 aixhello-4.9/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 10:29:56.000000 aixhello-4.9/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-03 10:29:56.000000 aixhello-4.9/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 10:29:56.000000 aixhello-4.9/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 10:29:56.824398 aixhello-4.9/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-06-03 10:25:57.000000 aixhello-4.9/setup.py
```

### Comparing `aixhello-4.7/LICENSE` & `aixhello-4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-4.7/PKG-INFO` & `aixhello-4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.7
+Version: 4.9
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.7/README.md` & `aixhello-4.9/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-4.7/aixhello/xyello.c` & `aixhello-4.9/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -7592,16 +7592,16 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   Py_ssize_t __pyx_t_10;
   PyObject *(*__pyx_t_11)(PyObject *);
   PyObject *__pyx_t_12 = NULL;
-  int __pyx_t_13;
-  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  int __pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_t_16;
   char const *__pyx_t_17;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   PyObject *__pyx_t_21 = NULL;
@@ -7887,73 +7887,98 @@
               break;
             }
             __Pyx_GOTREF(__pyx_t_1);
           }
           __Pyx_XDECREF_SET(__pyx_v_doc, __pyx_t_1);
           __pyx_t_1 = 0;
 
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CipherEncode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CipherEncode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_12 = NULL;
+          __pyx_t_12 = __Pyx_PyObject_Dict_GetItem(__pyx_v_doc, __pyx_n_u_extracted_text); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 234, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_13 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
-          if (likely(PyMethod_Check(__pyx_t_5))) {
-            __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_5);
-            if (likely(__pyx_t_12)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-              __Pyx_INCREF(__pyx_t_12);
+          if (likely(PyMethod_Check(__pyx_t_3))) {
+            __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_3);
+            if (likely(__pyx_t_13)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+              __Pyx_INCREF(__pyx_t_13);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_5, function);
+              __Pyx_DECREF_SET(__pyx_t_3, function);
               __pyx_t_4 = 1;
             }
           }
           #endif
           {
-            PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_3};
-            __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-            __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+            PyObject *__pyx_callargs[2] = {__pyx_t_13, __pyx_t_12};
+            __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+            __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+            if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L4_error)
+            __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          }
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __pyx_t_5 = NULL;
+          __pyx_t_4 = 0;
+          #if CYTHON_UNPACK_METHODS
+          if (likely(PyMethod_Check(__pyx_t_3))) {
+            __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+            if (likely(__pyx_t_5)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+              __Pyx_INCREF(__pyx_t_5);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_3, function);
+              __pyx_t_4 = 1;
+            }
+          }
+          #endif
+          {
+            PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_kp_u_utf_8};
+            __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
             if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L4_error)
             __Pyx_GOTREF(__pyx_t_1);
-            __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           }
           __Pyx_XDECREF_SET(__pyx_v_encodeText, __pyx_t_1);
           __pyx_t_1 = 0;
 
           __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_5) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
           if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_v_encodeText) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
 
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_5) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_3) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_5) < 0) __PYX_ERR(0, 236, __pyx_L4_error)
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 235, __pyx_L4_error)
+          __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 235, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
         __Pyx_XDECREF(__pyx_r);
         __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L4_error)
@@ -7962,43 +7987,44 @@
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_v_results);
         __Pyx_GIVEREF(__pyx_v_results);
         if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 242, __pyx_L4_error);
-        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L4_error)
-        __Pyx_GOTREF(__pyx_t_3);
-        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 242, __pyx_L4_error)
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L4_error)
+        __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 242, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_5);
+        if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 242, __pyx_L4_error)
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 242, __pyx_L4_error)
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
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
       __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_4) {
         __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 243, __pyx_L6_except_error)
-        __Pyx_XGOTREF(__pyx_t_5);
+        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_5, &__pyx_t_2) < 0) __PYX_ERR(0, 243, __pyx_L6_except_error)
         __Pyx_XGOTREF(__pyx_t_3);
+        __Pyx_XGOTREF(__pyx_t_5);
         __Pyx_XGOTREF(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_3);
-        __pyx_v_e = __pyx_t_3;
+        __Pyx_INCREF(__pyx_t_5);
+        __pyx_v_e = __pyx_t_5;
         /*try:*/ {
 
           __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_12 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 244, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -8011,26 +8037,26 @@
           __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 245, __pyx_L18_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_13 = PyTuple_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 245, __pyx_L18_error)
+          __Pyx_GOTREF(__pyx_t_13);
           __Pyx_GIVEREF(__pyx_t_1);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error);
           __pyx_t_1 = 0;
           __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 245, __pyx_L18_error)
-          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 245, __pyx_L18_error)
+          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_13, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 245, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_r = __pyx_t_15;
           __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           goto __pyx_L17_return;
@@ -8040,15 +8066,15 @@
           __pyx_L18_error:;
           /*exception exit:*/{
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
             __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
+            __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
             __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
             if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
             if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20) < 0)) __Pyx_ErrFetch(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
             __Pyx_XGOTREF(__pyx_t_18);
             __Pyx_XGOTREF(__pyx_t_19);
             __Pyx_XGOTREF(__pyx_t_20);
             __Pyx_XGOTREF(__pyx_t_21);
@@ -8105,60 +8131,60 @@
     }
 
   }
 
   /*else*/ {
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 247, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 247, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error);
-    __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
-    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_t_5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error);
+    __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 248, __pyx_L1_error)
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
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_XDECREF(__pyx_t_14);
+  __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_url);
   __Pyx_XDECREF(__pyx_v_headers);
   __Pyx_XDECREF(__pyx_v_pipeline);
```

### Comparing `aixhello-4.7/aixhello.egg-info/PKG-INFO` & `aixhello-4.9/aixhello.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.7
+Version: 4.9
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.7/setup.py` & `aixhello-4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='4.7',  
+    version='4.9',  
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

