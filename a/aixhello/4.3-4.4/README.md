# Comparing `tmp/aixhello-4.3.tar.gz` & `tmp/aixhello-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixhello-4.3.tar", last modified: Mon Jun  3 08:22:31 2024, max compression
+gzip compressed data, was "aixhello-4.4.tar", last modified: Mon Jun  3 09:00:34 2024, max compression
```

## Comparing `aixhello-4.3.tar` & `aixhello-4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-06-03 08:22:31.239443 aixhello-4.3/
--rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.3/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1078 2024-06-03 08:22:31.239443 aixhello-4.3/PKG-INFO
--rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-03 08:22:31.219444 aixhello-4.3/aixhello/
--rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.3/aixhello/__init__.py
--rw-rw-rw-   0        0        0   620010 2024-06-03 08:22:20.000000 aixhello-4.3/aixhello/xyello.c
-drwxrwxrwx   0        0        0        0 2024-06-03 08:22:31.237449 aixhello-4.3/aixhello.egg-info/
--rw-rw-rw-   0        0        0     1078 2024-06-03 08:22:31.000000 aixhello-4.3/aixhello.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-06-03 08:22:31.000000 aixhello-4.3/aixhello.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-03 08:22:31.000000 aixhello-4.3/aixhello.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-06-03 08:22:31.000000 aixhello-4.3/aixhello.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-03 08:22:31.000000 aixhello-4.3/aixhello.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-06-03 08:22:31.242447 aixhello-4.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-06-03 08:21:58.000000 aixhello-4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 09:00:34.810120 aixhello-4.4/
+-rw-rw-rw-   0        0        0     1080 2024-05-31 08:14:25.000000 aixhello-4.4/LICENSE
+-rw-rw-rw-   0        0        0       86 2024-05-31 08:50:40.000000 aixhello-4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1078 2024-06-03 09:00:34.809171 aixhello-4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2024-06-01 22:51:13.000000 aixhello-4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 09:00:34.787118 aixhello-4.4/aixhello/
+-rw-rw-rw-   0        0        0       26 2024-05-31 08:07:25.000000 aixhello-4.4/aixhello/__init__.py
+-rw-rw-rw-   0        0        0   621282 2024-06-03 09:00:23.000000 aixhello-4.4/aixhello/xyello.c
+drwxrwxrwx   0        0        0        0 2024-06-03 09:00:34.808119 aixhello-4.4/aixhello.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-03 09:00:34.000000 aixhello-4.4/aixhello.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-06-03 09:00:34.817113 aixhello-4.4/setup.cfg
+-rw-rw-rw-   0        0        0      973 2024-06-03 08:59:56.000000 aixhello-4.4/setup.py
```

### Comparing `aixhello-4.3/LICENSE` & `aixhello-4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aixhello-4.3/PKG-INFO` & `aixhello-4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.3
+Version: 4.4
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.3/README.md` & `aixhello-4.4/README.md`

 * *Files identical despite different names*

### Comparing `aixhello-4.3/aixhello/xyello.c` & `aixhello-4.4/aixhello/xyello.c`

 * *Files 0% similar despite different names*

```diff
@@ -7163,17 +7163,17 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   Py_ssize_t __pyx_t_10;
   PyObject *(*__pyx_t_11)(PyObject *);
-  int __pyx_t_12;
+  PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
-  PyObject *__pyx_t_14 = NULL;
+  int __pyx_t_14;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_t_16;
   char const *__pyx_t_17;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   PyObject *__pyx_t_21 = NULL;
@@ -7469,39 +7469,64 @@
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 187, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_filename, __pyx_t_3) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_CipherEncode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_13 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __Pyx_GOTREF(__pyx_t_13);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_12 = NULL;
+          __pyx_t_4 = 0;
+          #if CYTHON_UNPACK_METHODS
+          if (likely(PyMethod_Check(__pyx_t_5))) {
+            __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_5);
+            if (likely(__pyx_t_12)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+              __Pyx_INCREF(__pyx_t_12);
+              __Pyx_INCREF(function);
+              __Pyx_DECREF_SET(__pyx_t_5, function);
+              __pyx_t_4 = 1;
+            }
+          }
+          #endif
+          {
+            PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_13};
+            __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+            __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 188, __pyx_L4_error)
+            __Pyx_GOTREF(__pyx_t_3);
+            __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+          }
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_t_3) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 188, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_extracted_text, __pyx_t_5) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_5) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L4_error)
+          __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L4_error)
+          __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L4_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_text_embeddings, __pyx_t_3) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_doc, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 190, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 190, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_5);
+          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_3) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_accuracy, __pyx_t_5) < 0) __PYX_ERR(0, 187, __pyx_L4_error)
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          __pyx_t_12 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 186, __pyx_L4_error)
+          __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_results, __pyx_t_1); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 186, __pyx_L4_error)
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
         __Pyx_XDECREF(__pyx_r);
         __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L4_error)
@@ -7510,42 +7535,44 @@
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_v_results);
         __Pyx_GIVEREF(__pyx_v_results);
         if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_results)) __PYX_ERR(0, 193, __pyx_L4_error);
-        __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L4_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 193, __pyx_L4_error)
-        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L4_error)
+        __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_3);
+        if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 193, __pyx_L4_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L4_error)
+        __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_r = __pyx_t_3;
-        __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_r = __pyx_t_5;
+        __pyx_t_5 = 0;
         goto __pyx_L8_try_return;
 
       }
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
       __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_4) {
         __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_5, &__pyx_t_2) < 0) __PYX_ERR(0, 194, __pyx_L6_except_error)
-        __Pyx_XGOTREF(__pyx_t_3);
+        if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_3, &__pyx_t_2) < 0) __PYX_ERR(0, 194, __pyx_L6_except_error)
         __Pyx_XGOTREF(__pyx_t_5);
+        __Pyx_XGOTREF(__pyx_t_3);
         __Pyx_XGOTREF(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
-        __pyx_v_e = __pyx_t_5;
+        __Pyx_INCREF(__pyx_t_3);
+        __pyx_v_e = __pyx_t_3;
         /*try:*/ {
 
           __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error_processing_response_JSON, __pyx_t_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 195, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -7558,26 +7585,26 @@
           __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_json); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_dumps); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 196, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_13);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
-          __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 196, __pyx_L18_error)
-          __Pyx_GOTREF(__pyx_t_14);
+          __pyx_t_12 = PyTuple_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __Pyx_GOTREF(__pyx_t_12);
           __Pyx_GIVEREF(__pyx_t_1);
-          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error);
+          if (__Pyx_PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error);
           __pyx_t_1 = 0;
           __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_1);
           if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 196, __pyx_L18_error)
-          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_14, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 196, __pyx_L18_error)
+          __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_12, __pyx_t_1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 196, __pyx_L18_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __pyx_r = __pyx_t_15;
           __pyx_t_15 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           goto __pyx_L17_return;
@@ -7586,16 +7613,16 @@
         /*finally:*/ {
           __pyx_L18_error:;
           /*exception exit:*/{
             __Pyx_PyThreadState_declare
             __Pyx_PyThreadState_assign
             __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0; __pyx_t_21 = 0; __pyx_t_22 = 0; __pyx_t_23 = 0;
             __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+            __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-            __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
             __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
             if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_21, &__pyx_t_22, &__pyx_t_23);
             if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20) < 0)) __Pyx_ErrFetch(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
             __Pyx_XGOTREF(__pyx_t_18);
             __Pyx_XGOTREF(__pyx_t_19);
             __Pyx_XGOTREF(__pyx_t_20);
             __Pyx_XGOTREF(__pyx_t_21);
@@ -7652,60 +7679,60 @@
     }
 
   }
 
   /*else*/ {
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_response, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_t_2, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Error, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 198, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_json); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_dumps); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_5);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error);
-    __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
-    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_indent, __pyx_int_4) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 199, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
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
+  __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
-  __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_AddTraceback("aixhello.xyello.xyellw.vectorSearch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_url);
   __Pyx_XDECREF(__pyx_v_headers);
   __Pyx_XDECREF(__pyx_v_pipeline);
```

### Comparing `aixhello-4.3/aixhello.egg-info/PKG-INFO` & `aixhello-4.4/aixhello.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixhello
-Version: 4.3
+Version: 4.4
 Summary: AI HRM Package
 Author: SecureAI
 Author-email: package@xerocai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `aixhello-4.3/setup.py` & `aixhello-4.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'language_level': 3,         
         'emit_code_comments': False,  
     }
 }
 
 setup(
     name='aixhello',
-    version='4.3',  # Increment the version number
+    version='4.4',  
     description='AI HRM Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='SecureAI',
     author_email='package@xerocai.com',
     classifiers=[
         'Programming Language :: Python :: 3',
```

