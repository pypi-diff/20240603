# Comparing `tmp/comtypes-1.4.1.zip` & `tmp/comtypes-1.4.2.zip`

## zipinfo {}

```diff
@@ -1,117 +1,118 @@
-Zip file size: 218696 bytes, number of entries: 115
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-10 23:31 comtypes-1.4.1/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-10 23:31 comtypes-1.4.1/comtypes/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-10 23:31 comtypes-1.4.1/comtypes.egg-info/
--rw-rw-rw-  2.0 fat    45715 b- defN 24-Apr-10 23:31 comtypes-1.4.1/CHANGES.txt
--rw-rw-rw-  2.0 fat     1273 b- defN 24-Apr-10 23:31 comtypes-1.4.1/LICENSE.txt
--rw-rw-rw-  2.0 fat       34 b- defN 24-Apr-10 23:31 comtypes-1.4.1/MANIFEST.in
--rw-rw-rw-  2.0 fat     4099 b- defN 24-Apr-10 23:31 comtypes-1.4.1/PKG-INFO
--rw-rw-rw-  2.0 fat     3374 b- defN 24-Apr-10 23:31 comtypes-1.4.1/README.md
--rw-rw-rw-  2.0 fat       42 b- defN 24-Apr-10 23:31 comtypes-1.4.1/setup.cfg
--rw-rw-rw-  2.0 fat     6035 b- defN 24-Apr-10 23:31 comtypes-1.4.1/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-10 23:31 comtypes-1.4.1/comtypes/tools/
--rw-rw-rw-  2.0 fat    33648 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/automation.py
--rw-rw-rw-  2.0 fat     1759 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/clear_cache.py
--rw-rw-rw-  2.0 fat     3388 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/connectionpoints.py
--rw-rw-rw-  2.0 fat     3855 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/errorinfo.py
--rw-rw-rw-  2.0 fat     2730 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/git.py
--rw-rw-rw-  2.0 fat     2539 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/GUID.py
--rw-rw-rw-  2.0 fat     8494 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/hints.pyi
--rw-rw-rw-  2.0 fat     2431 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/hresult.py
--rw-rw-rw-  2.0 fat     1697 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/logutil.py
--rw-rw-rw-  2.0 fat     1311 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/messageloop.py
--rw-rw-rw-  2.0 fat     2046 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/patcher.py
--rw-rw-rw-  2.0 fat     8399 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/persist.py
--rw-rw-rw-  2.0 fat    17259 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/safearray.py
--rw-rw-rw-  2.0 fat     8845 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/shelllink.py
--rw-rw-rw-  2.0 fat    41436 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/typeinfo.py
--rw-rw-rw-  2.0 fat     3005 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/util.py
--rw-rw-rw-  2.0 fat     6601 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/viewobject.py
--rw-rw-rw-  2.0 fat    30619 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/_comobject.py
--rw-rw-rw-  2.0 fat    21786 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/_memberspec.py
--rw-rw-rw-  2.0 fat     2189 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/_meta.py
--rw-rw-rw-  2.0 fat     5244 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/_npsupport.py
--rw-rw-rw-  2.0 fat     4498 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/_safearray.py
--rw-rw-rw-  2.0 fat    42672 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/__init__.py
--rw-rw-rw-  2.0 fat     6032 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/dynamic.py
--rw-rw-rw-  2.0 fat     9230 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/lazybind.py
--rw-rw-rw-  2.0 fat     5803 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/_code_cache.py
--rw-rw-rw-  2.0 fat     4579 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/_constants.py
--rw-rw-rw-  2.0 fat    11198 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/_events.py
--rw-rw-rw-  2.0 fat    11163 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/_generate.py
--rw-rw-rw-  2.0 fat    11958 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/client/__init__.py
--rw-rw-rw-  2.0 fat     2887 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/automation.py
--rw-rw-rw-  2.0 fat     6806 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/connectionpoints.py
--rw-rw-rw-  2.0 fat     4390 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/inprocserver.py
--rw-rw-rw-  2.0 fat     2292 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/localserver.py
--rw-rw-rw-  2.0 fat    15120 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/register.py
--rw-rw-rw-  2.0 fat     2648 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/w_getopt.py
--rw-rw-rw-  2.0 fat     2378 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/server/__init__.py
--rw-rw-rw-  2.0 fat     2342 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/find_memleak.py
--rw-rw-rw-  2.0 fat     1664 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/mylib.idl
--rw-rw-rw-  2.0 fat     2590 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/mytypelib.idl
--rw-rw-rw-  2.0 fat      142 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/runtests.py
--rw-rw-rw-  2.0 fat      170 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/setup.py
--rw-rw-rw-  2.0 fat     2487 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/TestComServer.idl
--rw-rw-rw-  2.0 fat     5150 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/TestComServer.py
--rw-rw-rw-  2.0 fat     3560 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/TestComServer.tlb
--rw-rw-rw-  2.0 fat     1835 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/TestDispServer.idl
--rw-rw-rw-  2.0 fat     3735 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/TestDispServer.py
--rw-rw-rw-  2.0 fat     2992 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/TestDispServer.tlb
--rw-rw-rw-  2.0 fat     4436 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_agilent.py
--rw-rw-rw-  2.0 fat     1370 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_avmc.py
--rw-rw-rw-  2.0 fat     4213 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_basic.py
--rw-rw-rw-  2.0 fat     1565 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_BSTR.py
--rw-rw-rw-  2.0 fat     1404 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_casesensitivity.py
--rw-rw-rw-  2.0 fat      816 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_clear_cache.py
--rw-rw-rw-  2.0 fat    11794 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_client.py
--rw-rw-rw-  2.0 fat     2905 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_client_dynamic.py
--rw-rw-rw-  2.0 fat     5441 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_collections.py
--rw-rw-rw-  2.0 fat     7708 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_comserver.py
--rw-rw-rw-  2.0 fat     4167 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_createwrappers.py
--rw-rw-rw-  2.0 fat     3280 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_dict.py
--rw-rw-rw-  2.0 fat     4824 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_dispinterface.py
--rw-rw-rw-  2.0 fat     1156 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_DISPPARAMS.py
--rw-rw-rw-  2.0 fat     3105 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_dyndispatch.py
--rw-rw-rw-  2.0 fat     4768 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_excel.py
--rw-rw-rw-  2.0 fat     2978 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_findgendir.py
--rw-rw-rw-  2.0 fat     1977 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_getactiveobj.py
--rw-rw-rw-  2.0 fat     1060 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_GUID.py
--rw-rw-rw-  2.0 fat     3384 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_ie.py
--rw-rw-rw-  2.0 fat      887 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_ienum.py
--rw-rw-rw-  2.0 fat     1101 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_imfattributes.py
--rw-rw-rw-  2.0 fat    20881 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_inout_args.py
--rw-rw-rw-  2.0 fat      404 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_jscript.js
--rw-rw-rw-  2.0 fat     2877 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_msscript.py
--rw-rw-rw-  2.0 fat    12209 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_npsupport.py
--rw-rw-rw-  2.0 fat     2573 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_outparam.py
--rw-rw-rw-  2.0 fat     1373 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_propputref.py
--rw-rw-rw-  2.0 fat      379 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_pump_events.py
--rw-rw-rw-  2.0 fat      834 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_QueryService.py
--rw-rw-rw-  2.0 fat    10175 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_safearray.py
--rw-rw-rw-  2.0 fat     1146 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_sapi.py
--rw-rw-rw-  2.0 fat    12147 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_server.py
--rw-rw-rw-  2.0 fat     1512 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_showevents.py
--rw-rw-rw-  2.0 fat      374 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_subinterface.py
--rw-rw-rw-  2.0 fat     3721 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_typeinfo.py
--rw-rw-rw-  2.0 fat     1825 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_urlhistory.py
--rw-rw-rw-  2.0 fat    10871 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_variant.py
--rw-rw-rw-  2.0 fat     4064 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_win32com_interop.py
--rw-rw-rw-  2.0 fat     2500 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_wmi.py
--rw-rw-rw-  2.0 fat     2372 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/test_word.py
--rw-rw-rw-  2.0 fat     8262 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/test/__init__.py
--rw-rw-rw-  2.0 fat    60966 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/tools/codegenerator.py
--rw-rw-rw-  2.0 fat    31261 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/tools/tlbparser.py
--rw-rw-rw-  2.0 fat    12875 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/tools/typeannotator.py
--rw-rw-rw-  2.0 fat     5583 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/tools/typedesc.py
--rw-rw-rw-  2.0 fat     6626 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/tools/typedesc_base.py
--rw-rw-rw-  2.0 fat       30 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       67 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat     4099 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat     2945 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-10 23:31 comtypes-1.4.1/comtypes.egg-info/top_level.txt
-115 files, 739474 bytes uncompressed, 200594 bytes compressed:  72.9%
+Zip file size: 222142 bytes, number of entries: 116
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-06 23:43 comtypes-1.4.2/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-06 23:43 comtypes-1.4.2/comtypes/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-06 23:43 comtypes-1.4.2/comtypes.egg-info/
+-rw-rw-rw-  2.0 fat    46189 b- defN 24-May-06 23:42 comtypes-1.4.2/CHANGES.txt
+-rw-rw-rw-  2.0 fat     1273 b- defN 24-May-06 23:42 comtypes-1.4.2/LICENSE.txt
+-rw-rw-rw-  2.0 fat       34 b- defN 24-May-06 23:42 comtypes-1.4.2/MANIFEST.in
+-rw-rw-rw-  2.0 fat     4099 b- defN 24-May-06 23:43 comtypes-1.4.2/PKG-INFO
+-rw-rw-rw-  2.0 fat     3374 b- defN 24-May-06 23:42 comtypes-1.4.2/README.md
+-rw-rw-rw-  2.0 fat       42 b- defN 24-May-06 23:43 comtypes-1.4.2/setup.cfg
+-rw-rw-rw-  2.0 fat     6035 b- defN 24-May-06 23:42 comtypes-1.4.2/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-06 23:43 comtypes-1.4.2/comtypes/client/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-06 23:43 comtypes-1.4.2/comtypes/server/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-06 23:43 comtypes-1.4.2/comtypes/test/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-06 23:43 comtypes-1.4.2/comtypes/tools/
+-rw-rw-rw-  2.0 fat    33648 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/automation.py
+-rw-rw-rw-  2.0 fat     1759 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/clear_cache.py
+-rw-rw-rw-  2.0 fat     3388 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/connectionpoints.py
+-rw-rw-rw-  2.0 fat     3855 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/errorinfo.py
+-rw-rw-rw-  2.0 fat     2730 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/git.py
+-rw-rw-rw-  2.0 fat     2539 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/GUID.py
+-rw-rw-rw-  2.0 fat     8985 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/hints.pyi
+-rw-rw-rw-  2.0 fat     2431 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/hresult.py
+-rw-rw-rw-  2.0 fat     1697 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/logutil.py
+-rw-rw-rw-  2.0 fat     1311 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/messageloop.py
+-rw-rw-rw-  2.0 fat     2046 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/patcher.py
+-rw-rw-rw-  2.0 fat     8399 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/persist.py
+-rw-rw-rw-  2.0 fat    17259 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/safearray.py
+-rw-rw-rw-  2.0 fat     8845 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/shelllink.py
+-rw-rw-rw-  2.0 fat    41436 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/typeinfo.py
+-rw-rw-rw-  2.0 fat     3005 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/util.py
+-rw-rw-rw-  2.0 fat     6601 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/viewobject.py
+-rw-rw-rw-  2.0 fat    30619 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/_comobject.py
+-rw-rw-rw-  2.0 fat    21786 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/_memberspec.py
+-rw-rw-rw-  2.0 fat     2189 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/_meta.py
+-rw-rw-rw-  2.0 fat     5244 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/_npsupport.py
+-rw-rw-rw-  2.0 fat     4498 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/_safearray.py
+-rw-rw-rw-  2.0 fat    42672 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/__init__.py
+-rw-rw-rw-  2.0 fat     6032 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/client/dynamic.py
+-rw-rw-rw-  2.0 fat     9230 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/client/lazybind.py
+-rw-rw-rw-  2.0 fat     5803 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/client/_code_cache.py
+-rw-rw-rw-  2.0 fat     4579 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/client/_constants.py
+-rw-rw-rw-  2.0 fat    11198 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/client/_events.py
+-rw-rw-rw-  2.0 fat    12034 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/client/_generate.py
+-rw-rw-rw-  2.0 fat    11958 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/client/__init__.py
+-rw-rw-rw-  2.0 fat     2887 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/server/automation.py
+-rw-rw-rw-  2.0 fat     6806 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/server/connectionpoints.py
+-rw-rw-rw-  2.0 fat     4390 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/server/inprocserver.py
+-rw-rw-rw-  2.0 fat     2292 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/server/localserver.py
+-rw-rw-rw-  2.0 fat    15120 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/server/register.py
+-rw-rw-rw-  2.0 fat     2648 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/server/w_getopt.py
+-rw-rw-rw-  2.0 fat     2378 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/server/__init__.py
+-rw-rw-rw-  2.0 fat     2342 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/find_memleak.py
+-rw-rw-rw-  2.0 fat     1664 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/mylib.idl
+-rw-rw-rw-  2.0 fat     2590 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/mytypelib.idl
+-rw-rw-rw-  2.0 fat      142 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/runtests.py
+-rw-rw-rw-  2.0 fat      170 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/setup.py
+-rw-rw-rw-  2.0 fat     2487 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/TestComServer.idl
+-rw-rw-rw-  2.0 fat     5150 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/TestComServer.py
+-rw-rw-rw-  2.0 fat     3560 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/TestComServer.tlb
+-rw-rw-rw-  2.0 fat     1835 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/TestDispServer.idl
+-rw-rw-rw-  2.0 fat     3735 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/TestDispServer.py
+-rw-rw-rw-  2.0 fat     2992 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/TestDispServer.tlb
+-rw-rw-rw-  2.0 fat     4436 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_agilent.py
+-rw-rw-rw-  2.0 fat     1370 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_avmc.py
+-rw-rw-rw-  2.0 fat     4213 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_basic.py
+-rw-rw-rw-  2.0 fat     1565 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_BSTR.py
+-rw-rw-rw-  2.0 fat     1404 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_casesensitivity.py
+-rw-rw-rw-  2.0 fat      816 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_clear_cache.py
+-rw-rw-rw-  2.0 fat    12580 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_client.py
+-rw-rw-rw-  2.0 fat     2905 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_client_dynamic.py
+-rw-rw-rw-  2.0 fat     7515 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_client_regenerate_modules.py
+-rw-rw-rw-  2.0 fat     5441 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_collections.py
+-rw-rw-rw-  2.0 fat     7708 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_comserver.py
+-rw-rw-rw-  2.0 fat     4167 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_createwrappers.py
+-rw-rw-rw-  2.0 fat     3280 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_dict.py
+-rw-rw-rw-  2.0 fat     4824 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_dispinterface.py
+-rw-rw-rw-  2.0 fat     1156 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_DISPPARAMS.py
+-rw-rw-rw-  2.0 fat     3105 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_dyndispatch.py
+-rw-rw-rw-  2.0 fat     4768 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_excel.py
+-rw-rw-rw-  2.0 fat     2978 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_findgendir.py
+-rw-rw-rw-  2.0 fat     1977 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_getactiveobj.py
+-rw-rw-rw-  2.0 fat     1060 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_GUID.py
+-rw-rw-rw-  2.0 fat     3384 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_ie.py
+-rw-rw-rw-  2.0 fat      887 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_ienum.py
+-rw-rw-rw-  2.0 fat     1101 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_imfattributes.py
+-rw-rw-rw-  2.0 fat    20881 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_inout_args.py
+-rw-rw-rw-  2.0 fat      404 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_jscript.js
+-rw-rw-rw-  2.0 fat     2877 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_msscript.py
+-rw-rw-rw-  2.0 fat    12209 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_npsupport.py
+-rw-rw-rw-  2.0 fat     2573 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_outparam.py
+-rw-rw-rw-  2.0 fat     1373 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_propputref.py
+-rw-rw-rw-  2.0 fat      379 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_pump_events.py
+-rw-rw-rw-  2.0 fat      834 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_QueryService.py
+-rw-rw-rw-  2.0 fat    10175 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_safearray.py
+-rw-rw-rw-  2.0 fat     1146 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_sapi.py
+-rw-rw-rw-  2.0 fat    12147 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_server.py
+-rw-rw-rw-  2.0 fat     1512 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_showevents.py
+-rw-rw-rw-  2.0 fat      374 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_subinterface.py
+-rw-rw-rw-  2.0 fat     3721 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_typeinfo.py
+-rw-rw-rw-  2.0 fat     1825 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_urlhistory.py
+-rw-rw-rw-  2.0 fat    10871 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_variant.py
+-rw-rw-rw-  2.0 fat     4064 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_win32com_interop.py
+-rw-rw-rw-  2.0 fat     2500 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_wmi.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/test_word.py
+-rw-rw-rw-  2.0 fat     8262 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/test/__init__.py
+-rw-rw-rw-  2.0 fat    64338 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/tools/codegenerator.py
+-rw-rw-rw-  2.0 fat    31261 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/tools/tlbparser.py
+-rw-rw-rw-  2.0 fat    13096 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/tools/typeannotator.py
+-rw-rw-rw-  2.0 fat     5604 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/tools/typedesc.py
+-rw-rw-rw-  2.0 fat     6626 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/tools/typedesc_base.py
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-06 23:42 comtypes-1.4.2/comtypes/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-06 23:43 comtypes-1.4.2/comtypes.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       67 b- defN 24-May-06 23:43 comtypes-1.4.2/comtypes.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat     4099 b- defN 24-May-06 23:43 comtypes-1.4.2/comtypes.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat     2993 b- defN 24-May-06 23:43 comtypes-1.4.2/comtypes.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-06 23:43 comtypes-1.4.2/comtypes.egg-info/top_level.txt
+116 files, 753273 bytes uncompressed, 203840 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -1,346 +1,349 @@
-Filename: comtypes-1.4.1/
+Filename: comtypes-1.4.2/
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/
+Filename: comtypes-1.4.2/comtypes/
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes.egg-info/
+Filename: comtypes-1.4.2/comtypes.egg-info/
 Comment: 
 
-Filename: comtypes-1.4.1/CHANGES.txt
+Filename: comtypes-1.4.2/CHANGES.txt
 Comment: 
 
-Filename: comtypes-1.4.1/LICENSE.txt
+Filename: comtypes-1.4.2/LICENSE.txt
 Comment: 
 
-Filename: comtypes-1.4.1/MANIFEST.in
+Filename: comtypes-1.4.2/MANIFEST.in
 Comment: 
 
-Filename: comtypes-1.4.1/PKG-INFO
+Filename: comtypes-1.4.2/PKG-INFO
 Comment: 
 
-Filename: comtypes-1.4.1/README.md
+Filename: comtypes-1.4.2/README.md
 Comment: 
 
-Filename: comtypes-1.4.1/setup.cfg
+Filename: comtypes-1.4.2/setup.cfg
 Comment: 
 
-Filename: comtypes-1.4.1/setup.py
+Filename: comtypes-1.4.2/setup.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/
+Filename: comtypes-1.4.2/comtypes/client/
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/
+Filename: comtypes-1.4.2/comtypes/server/
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/
+Filename: comtypes-1.4.2/comtypes/test/
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/tools/
+Filename: comtypes-1.4.2/comtypes/tools/
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/automation.py
+Filename: comtypes-1.4.2/comtypes/automation.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/clear_cache.py
+Filename: comtypes-1.4.2/comtypes/clear_cache.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/connectionpoints.py
+Filename: comtypes-1.4.2/comtypes/connectionpoints.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/errorinfo.py
+Filename: comtypes-1.4.2/comtypes/errorinfo.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/git.py
+Filename: comtypes-1.4.2/comtypes/git.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/GUID.py
+Filename: comtypes-1.4.2/comtypes/GUID.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/hints.pyi
+Filename: comtypes-1.4.2/comtypes/hints.pyi
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/hresult.py
+Filename: comtypes-1.4.2/comtypes/hresult.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/logutil.py
+Filename: comtypes-1.4.2/comtypes/logutil.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/messageloop.py
+Filename: comtypes-1.4.2/comtypes/messageloop.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/patcher.py
+Filename: comtypes-1.4.2/comtypes/patcher.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/persist.py
+Filename: comtypes-1.4.2/comtypes/persist.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/safearray.py
+Filename: comtypes-1.4.2/comtypes/safearray.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/shelllink.py
+Filename: comtypes-1.4.2/comtypes/shelllink.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/typeinfo.py
+Filename: comtypes-1.4.2/comtypes/typeinfo.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/util.py
+Filename: comtypes-1.4.2/comtypes/util.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/viewobject.py
+Filename: comtypes-1.4.2/comtypes/viewobject.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/_comobject.py
+Filename: comtypes-1.4.2/comtypes/_comobject.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/_memberspec.py
+Filename: comtypes-1.4.2/comtypes/_memberspec.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/_meta.py
+Filename: comtypes-1.4.2/comtypes/_meta.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/_npsupport.py
+Filename: comtypes-1.4.2/comtypes/_npsupport.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/_safearray.py
+Filename: comtypes-1.4.2/comtypes/_safearray.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/__init__.py
+Filename: comtypes-1.4.2/comtypes/__init__.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/dynamic.py
+Filename: comtypes-1.4.2/comtypes/client/dynamic.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/lazybind.py
+Filename: comtypes-1.4.2/comtypes/client/lazybind.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/_code_cache.py
+Filename: comtypes-1.4.2/comtypes/client/_code_cache.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/_constants.py
+Filename: comtypes-1.4.2/comtypes/client/_constants.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/_events.py
+Filename: comtypes-1.4.2/comtypes/client/_events.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/_generate.py
+Filename: comtypes-1.4.2/comtypes/client/_generate.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/client/__init__.py
+Filename: comtypes-1.4.2/comtypes/client/__init__.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/automation.py
+Filename: comtypes-1.4.2/comtypes/server/automation.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/connectionpoints.py
+Filename: comtypes-1.4.2/comtypes/server/connectionpoints.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/inprocserver.py
+Filename: comtypes-1.4.2/comtypes/server/inprocserver.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/localserver.py
+Filename: comtypes-1.4.2/comtypes/server/localserver.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/register.py
+Filename: comtypes-1.4.2/comtypes/server/register.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/w_getopt.py
+Filename: comtypes-1.4.2/comtypes/server/w_getopt.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/server/__init__.py
+Filename: comtypes-1.4.2/comtypes/server/__init__.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/find_memleak.py
+Filename: comtypes-1.4.2/comtypes/test/find_memleak.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/mylib.idl
+Filename: comtypes-1.4.2/comtypes/test/mylib.idl
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/mytypelib.idl
+Filename: comtypes-1.4.2/comtypes/test/mytypelib.idl
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/runtests.py
+Filename: comtypes-1.4.2/comtypes/test/runtests.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/setup.py
+Filename: comtypes-1.4.2/comtypes/test/setup.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/TestComServer.idl
+Filename: comtypes-1.4.2/comtypes/test/TestComServer.idl
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/TestComServer.py
+Filename: comtypes-1.4.2/comtypes/test/TestComServer.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/TestComServer.tlb
+Filename: comtypes-1.4.2/comtypes/test/TestComServer.tlb
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/TestDispServer.idl
+Filename: comtypes-1.4.2/comtypes/test/TestDispServer.idl
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/TestDispServer.py
+Filename: comtypes-1.4.2/comtypes/test/TestDispServer.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/TestDispServer.tlb
+Filename: comtypes-1.4.2/comtypes/test/TestDispServer.tlb
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_agilent.py
+Filename: comtypes-1.4.2/comtypes/test/test_agilent.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_avmc.py
+Filename: comtypes-1.4.2/comtypes/test/test_avmc.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_basic.py
+Filename: comtypes-1.4.2/comtypes/test/test_basic.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_BSTR.py
+Filename: comtypes-1.4.2/comtypes/test/test_BSTR.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_casesensitivity.py
+Filename: comtypes-1.4.2/comtypes/test/test_casesensitivity.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_clear_cache.py
+Filename: comtypes-1.4.2/comtypes/test/test_clear_cache.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_client.py
+Filename: comtypes-1.4.2/comtypes/test/test_client.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_client_dynamic.py
+Filename: comtypes-1.4.2/comtypes/test/test_client_dynamic.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_collections.py
+Filename: comtypes-1.4.2/comtypes/test/test_client_regenerate_modules.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_comserver.py
+Filename: comtypes-1.4.2/comtypes/test/test_collections.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_createwrappers.py
+Filename: comtypes-1.4.2/comtypes/test/test_comserver.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_dict.py
+Filename: comtypes-1.4.2/comtypes/test/test_createwrappers.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_dispinterface.py
+Filename: comtypes-1.4.2/comtypes/test/test_dict.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_DISPPARAMS.py
+Filename: comtypes-1.4.2/comtypes/test/test_dispinterface.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_dyndispatch.py
+Filename: comtypes-1.4.2/comtypes/test/test_DISPPARAMS.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_excel.py
+Filename: comtypes-1.4.2/comtypes/test/test_dyndispatch.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_findgendir.py
+Filename: comtypes-1.4.2/comtypes/test/test_excel.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_getactiveobj.py
+Filename: comtypes-1.4.2/comtypes/test/test_findgendir.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_GUID.py
+Filename: comtypes-1.4.2/comtypes/test/test_getactiveobj.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_ie.py
+Filename: comtypes-1.4.2/comtypes/test/test_GUID.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_ienum.py
+Filename: comtypes-1.4.2/comtypes/test/test_ie.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_imfattributes.py
+Filename: comtypes-1.4.2/comtypes/test/test_ienum.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_inout_args.py
+Filename: comtypes-1.4.2/comtypes/test/test_imfattributes.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_jscript.js
+Filename: comtypes-1.4.2/comtypes/test/test_inout_args.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_msscript.py
+Filename: comtypes-1.4.2/comtypes/test/test_jscript.js
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_npsupport.py
+Filename: comtypes-1.4.2/comtypes/test/test_msscript.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_outparam.py
+Filename: comtypes-1.4.2/comtypes/test/test_npsupport.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_propputref.py
+Filename: comtypes-1.4.2/comtypes/test/test_outparam.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_pump_events.py
+Filename: comtypes-1.4.2/comtypes/test/test_propputref.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_QueryService.py
+Filename: comtypes-1.4.2/comtypes/test/test_pump_events.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_safearray.py
+Filename: comtypes-1.4.2/comtypes/test/test_QueryService.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_sapi.py
+Filename: comtypes-1.4.2/comtypes/test/test_safearray.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_server.py
+Filename: comtypes-1.4.2/comtypes/test/test_sapi.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_showevents.py
+Filename: comtypes-1.4.2/comtypes/test/test_server.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_subinterface.py
+Filename: comtypes-1.4.2/comtypes/test/test_showevents.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_typeinfo.py
+Filename: comtypes-1.4.2/comtypes/test/test_subinterface.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_urlhistory.py
+Filename: comtypes-1.4.2/comtypes/test/test_typeinfo.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_variant.py
+Filename: comtypes-1.4.2/comtypes/test/test_urlhistory.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_win32com_interop.py
+Filename: comtypes-1.4.2/comtypes/test/test_variant.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_wmi.py
+Filename: comtypes-1.4.2/comtypes/test/test_win32com_interop.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/test_word.py
+Filename: comtypes-1.4.2/comtypes/test/test_wmi.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/test/__init__.py
+Filename: comtypes-1.4.2/comtypes/test/test_word.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/tools/codegenerator.py
+Filename: comtypes-1.4.2/comtypes/test/__init__.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/tools/tlbparser.py
+Filename: comtypes-1.4.2/comtypes/tools/codegenerator.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/tools/typeannotator.py
+Filename: comtypes-1.4.2/comtypes/tools/tlbparser.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/tools/typedesc.py
+Filename: comtypes-1.4.2/comtypes/tools/typeannotator.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/tools/typedesc_base.py
+Filename: comtypes-1.4.2/comtypes/tools/typedesc.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes/tools/__init__.py
+Filename: comtypes-1.4.2/comtypes/tools/typedesc_base.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes.egg-info/dependency_links.txt
+Filename: comtypes-1.4.2/comtypes/tools/__init__.py
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes.egg-info/entry_points.txt
+Filename: comtypes-1.4.2/comtypes.egg-info/dependency_links.txt
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes.egg-info/PKG-INFO
+Filename: comtypes-1.4.2/comtypes.egg-info/entry_points.txt
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes.egg-info/SOURCES.txt
+Filename: comtypes-1.4.2/comtypes.egg-info/PKG-INFO
 Comment: 
 
-Filename: comtypes-1.4.1/comtypes.egg-info/top_level.txt
+Filename: comtypes-1.4.2/comtypes.egg-info/SOURCES.txt
+Comment: 
+
+Filename: comtypes-1.4.2/comtypes.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `comtypes-1.4.1/CHANGES.txt` & `comtypes-1.4.2/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Comtypes CHANGELOG
 ==================
 
+Release 1.4.2
+--------------
+
+* Improve the stability of module generation by ``GetModule``. By @junkmd.
+* Define ``c_int`` aliases earlier than others in wrapper modules. By @junkmd.
+* Remove trailing newlines generated by ``codegenerator`` and ``typeannotator``. By @junkmd.
+* Determine whether a interface is one of the known symbols not only by its name but also by using its iid. By @junkmd.
+* Add ``Incomplete`` and ``Hresult`` to ``hints.pyi``. By @junkmd.
+
 Release 1.4.1
 --------------
 * Fix `TypeError` when defining enumeration types
 
 Release 1.4.0
 --------------
 * Add enumeration definitions in generated friendly modules. By @junkmd.
```

## Comparing `comtypes-1.4.1/LICENSE.txt` & `comtypes-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/PKG-INFO` & `comtypes-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comtypes
-Version: 1.4.1
+Version: 1.4.2
 Summary: Pure Python COM package
 Home-page: https://github.com/enthought/comtypes
 Download-URL: https://github.com/enthought/comtypes/releases
 Author: Thomas Heller
 Author-email: theller@python.net
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `comtypes-1.4.1/README.md` & `comtypes-1.4.2/README.md`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/setup.py` & `comtypes-1.4.2/setup.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/automation.py` & `comtypes-1.4.2/comtypes/automation.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/clear_cache.py` & `comtypes-1.4.2/comtypes/clear_cache.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/connectionpoints.py` & `comtypes-1.4.2/comtypes/connectionpoints.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/errorinfo.py` & `comtypes-1.4.2/comtypes/errorinfo.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/git.py` & `comtypes-1.4.2/comtypes/git.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/GUID.py` & `comtypes-1.4.2/comtypes/GUID.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/hints.pyi` & `comtypes-1.4.2/comtypes/hints.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,26 +18,38 @@
 )
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
 else:
     from typing_extensions import Protocol
 if sys.version_info >= (3, 10):
-    from typing import Concatenate, ParamSpec
+    from typing import Concatenate, ParamSpec, TypeAlias
+    from typing import TypeGuard as TypeGuard
 else:
-    from typing_extensions import Concatenate, ParamSpec
+    from typing_extensions import Concatenate, ParamSpec, TypeAlias
+    from typing_extensions import TypeGuard as TypeGuard
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 from comtypes.automation import IDispatch as IDispatch, VARIANT as VARIANT
 from comtypes.server import IClassFactory as IClassFactory
 from comtypes.typeinfo import ITypeInfo as ITypeInfo
 
+Incomplete: TypeAlias = Any
+"""The type symbol is used temporarily until the COM library parsers or
+code generators are enhanced to annotate detailed type hints.
+"""
+
+Hresult: TypeAlias = int
+"""The value returned when calling a method with no `[out]` or `[out, retval]`
+arguments and with `HRESULT` as its return type in its COM method definition.
+"""
+
 class _MethodTypeDesc(Protocol):
     arguments: List[Tuple[Any, str, List[str], Optional[Any]]]
     idlflags: List[str]
     name: str
 
 _P_Put = ParamSpec("_P_Put")
 _R_Put = TypeVar("_R_Put")
```

## Comparing `comtypes-1.4.1/comtypes/hresult.py` & `comtypes-1.4.2/comtypes/hresult.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/logutil.py` & `comtypes-1.4.2/comtypes/logutil.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/messageloop.py` & `comtypes-1.4.2/comtypes/messageloop.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/patcher.py` & `comtypes-1.4.2/comtypes/patcher.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/persist.py` & `comtypes-1.4.2/comtypes/persist.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/safearray.py` & `comtypes-1.4.2/comtypes/safearray.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/shelllink.py` & `comtypes-1.4.2/comtypes/shelllink.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/typeinfo.py` & `comtypes-1.4.2/comtypes/typeinfo.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/util.py` & `comtypes-1.4.2/comtypes/util.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/viewobject.py` & `comtypes-1.4.2/comtypes/viewobject.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/_comobject.py` & `comtypes-1.4.2/comtypes/_comobject.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/_memberspec.py` & `comtypes-1.4.2/comtypes/_memberspec.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/_meta.py` & `comtypes-1.4.2/comtypes/_meta.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/_npsupport.py` & `comtypes-1.4.2/comtypes/_npsupport.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/_safearray.py` & `comtypes-1.4.2/comtypes/_safearray.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/__init__.py` & `comtypes-1.4.2/comtypes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # comtypes version numbers follow semver (http://semver.org/) and PEP 440
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 import atexit
 from ctypes import *
 from ctypes import _Pointer, _SimpleCData
 
 try:
     from _ctypes import COMError
```

## Comparing `comtypes-1.4.1/comtypes/client/dynamic.py` & `comtypes-1.4.2/comtypes/client/dynamic.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/client/lazybind.py` & `comtypes-1.4.2/comtypes/client/lazybind.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/client/_code_cache.py` & `comtypes-1.4.2/comtypes/client/_code_cache.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/client/_constants.py` & `comtypes-1.4.2/comtypes/client/_constants.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/client/_events.py` & `comtypes-1.4.2/comtypes/client/_events.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/client/_generate.py` & `comtypes-1.4.2/comtypes/client/_generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import print_function
 import ctypes
 import importlib
+import inspect
 import logging
 import os
 import sys
 import types
-from typing import Any, Tuple, List, Optional, Dict, Union as _UnionT
+from typing import Any, Tuple, List, Mapping, Optional, Dict, Union as _UnionT
 import winreg
 
 from comtypes import GUID, typeinfo
 import comtypes.client
 from comtypes.tools import codegenerator, tlbparser
 
 
@@ -117,15 +118,18 @@
                 pathname = tlib_string
         # if above path torture resulted in an absolute path, then the file exists (at this point)!
         assert not (os.path.isabs(pathname)) or os.path.exists(pathname)
     else:
         pathname = None
         tlib = _load_tlib(tlib)
     logger.debug("GetModule(%s)", tlib.GetLibAttr())
-    return ModuleGenerator().generate(tlib, pathname)
+    mod = _get_existing_module(tlib)
+    if mod is not None:
+        return mod
+    return ModuleGenerator(tlib, pathname).generate()
 
 
 def _load_tlib(obj: Any) -> typeinfo.ITypeLib:
     """Load a pointer of ITypeLib on demand."""
     # obj is a filepath or a ProgID
     if isinstance(obj, str):
         # in any case, attempt to load and if tlib_string is not valid, then raise
@@ -156,118 +160,139 @@
         return typeinfo.LoadRegTypeLib(GUID(obj._reg_libid_), *obj._reg_version_)
     # obj is a pointer of ITypeLib
     elif isinstance(obj, ctypes.POINTER(typeinfo.ITypeLib)):
         return obj  # type: ignore
     raise TypeError("'%r' is not supported type for loading typelib" % obj)
 
 
-def _create_module_in_file(modulename: str, code: str) -> types.ModuleType:
-    """create module in file system, and import it"""
+def _get_existing_module(tlib: typeinfo.ITypeLib) -> Optional[types.ModuleType]:
+    def _get_friendly(name: str) -> Optional[types.ModuleType]:
+        try:
+            mod = _my_import(name)
+        except Exception as details:
+            logger.info("Could not import %s: %s", friendly_name, details)
+        else:
+            return mod
+
+    def _get_wrapper(name: str) -> Optional[types.ModuleType]:
+        if name in sys.modules:
+            return sys.modules[name]
+        try:
+            return _my_import(name)
+        except Exception as details:
+            logger.info("Could not import %s: %s", name, details)
+
+    wrapper_name = codegenerator.name_wrapper_module(tlib)
+    friendly_name = codegenerator.name_friendly_module(tlib)
+    wrapper_module = _get_wrapper(wrapper_name)
+    if wrapper_module is not None:
+        if friendly_name is None:
+            return wrapper_module
+        else:
+            friendly_module = _get_friendly(friendly_name)
+            if friendly_module is not None:
+                return friendly_module
+    return None
+
+
+def _create_module(modulename: str, code: str) -> types.ModuleType:
+    """Creates the module, then imports it."""
     # `modulename` is 'comtypes.gen.xxx'
-    filename = "%s.py" % modulename.split(".")[-1]
-    with open(os.path.join(comtypes.client.gen_dir, filename), "w") as ofi:
+    stem = modulename.split(".")[-1]
+    if comtypes.client.gen_dir is None:
+        # in memory system
+        import comtypes.gen as g
+
+        mod = types.ModuleType(modulename)
+        abs_gen_path = os.path.abspath(g.__path__[0])  # type: ignore
+        mod.__file__ = os.path.join(abs_gen_path, "<memory>")
+        exec(code, mod.__dict__)
+        sys.modules[modulename] = mod
+        setattr(g, stem, mod)
+        return mod
+    # in file system
+    with open(os.path.join(comtypes.client.gen_dir, f"{stem}.py"), "w") as ofi:
         print(code, file=ofi)
     # clear the import cache to make sure Python sees newly created modules
-    if hasattr(importlib, "invalidate_caches"):
-        importlib.invalidate_caches()
+    importlib.invalidate_caches()
     return _my_import(modulename)
 
 
-def _create_module_in_memory(modulename: str, code: str) -> types.ModuleType:
-    """create module in memory system, and import it"""
-    # `modulename` is 'comtypes.gen.xxx'
-    import comtypes.gen as g
-
-    mod = types.ModuleType(modulename)
-    abs_gen_path = os.path.abspath(g.__path__[0])  # type: ignore
-    mod.__file__ = os.path.join(abs_gen_path, "<memory>")
-    exec(code, mod.__dict__)
-    sys.modules[modulename] = mod
-    setattr(g, modulename.split(".")[-1], mod)
-    return mod
-
-
 class ModuleGenerator(object):
-    def __init__(self) -> None:
-        self.codegen = codegenerator.CodeGenerator(_get_known_symbols())
-
-    def generate(
-        self, tlib: typeinfo.ITypeLib, pathname: Optional[str]
-    ) -> types.ModuleType:
-        # create and import the real typelib wrapper module
-        mod = self._create_wrapper_module(tlib, pathname)
-        # try to get the friendly-name, if not, returns the real typelib wrapper module
-        modulename = codegenerator.name_friendly_module(tlib)
-        if modulename is None:
-            return mod
-        # create and import the friendly-named module
-        return self._create_friendly_module(tlib, modulename)
-
-    def _create_friendly_module(
-        self, tlib: typeinfo.ITypeLib, modulename: str
-    ) -> types.ModuleType:
-        """helper which creates and imports the friendly-named module."""
-        try:
-            mod = _my_import(modulename)
-        except Exception as details:
-            logger.info("Could not import %s: %s", modulename, details)
-        else:
-            return mod
-        # the module is always regenerated if the import fails
-        logger.info("# Generating %s", modulename)
-        # determine the Python module name
-        modname = codegenerator.name_wrapper_module(tlib)
-        code = self.codegen.generate_friendly_code(modname)
-        if comtypes.client.gen_dir is None:
-            return _create_module_in_memory(modulename, code)
-        return _create_module_in_file(modulename, code)
-
-    def _create_wrapper_module(
-        self, tlib: typeinfo.ITypeLib, pathname: Optional[str]
-    ) -> types.ModuleType:
-        """helper which creates and imports the real typelib wrapper module."""
-        modulename = codegenerator.name_wrapper_module(tlib)
-        if modulename in sys.modules:
-            return sys.modules[modulename]
-        try:
-            return _my_import(modulename)
-        except Exception as details:
-            logger.info("Could not import %s: %s", modulename, details)
-        # generate the module since it doesn't exist or is out of date
-        logger.info("# Generating %s", modulename)
-        p = tlbparser.TypeLibParser(tlib)
+    def __init__(self, tlib: typeinfo.ITypeLib, pathname: Optional[str]) -> None:
+        self.wrapper_name = codegenerator.name_wrapper_module(tlib)
+        self.friendly_name = codegenerator.name_friendly_module(tlib)
         if pathname is None:
-            pathname = tlbparser.get_tlib_filename(tlib)
-        items = list(p.parse().values())
-        code = self.codegen.generate_wrapper_code(items, filename=pathname)
-        for ext_tlib in self.codegen.externals:  # generates dependency COM-lib modules
+            self.pathname = tlbparser.get_tlib_filename(tlib)
+        else:
+            self.pathname = pathname
+        self.tlib = tlib
+
+    def generate(self) -> types.ModuleType:
+        """Generates wrapper and friendly modules."""
+        known_symbols, known_interfaces = _get_known_namespaces()
+        codegen = codegenerator.CodeGenerator(known_symbols, known_interfaces)
+        codebases: List[Tuple[str, str]] = []
+        logger.info("# Generating %s", self.wrapper_name)
+        items = list(tlbparser.TypeLibParser(self.tlib).parse().values())
+        wrp_code = codegen.generate_wrapper_code(items, filename=self.pathname)
+        codebases.append((self.wrapper_name, wrp_code))
+        if self.friendly_name is not None:
+            logger.info("# Generating %s", self.friendly_name)
+            frd_code = codegen.generate_friendly_code(self.wrapper_name)
+            codebases.append((self.friendly_name, frd_code))
+        for ext_tlib in codegen.externals:  # generates dependency COM-lib modules
             GetModule(ext_tlib)
-        if comtypes.client.gen_dir is None:
-            return _create_module_in_memory(modulename, code)
-        return _create_module_in_file(modulename, code)
+        return [_create_module(name, code) for (name, code) in codebases][-1]
 
 
-def _get_known_symbols() -> Dict[str, str]:
-    known_symbols: Dict[str, str] = {}
+_SymbolName = str
+_ModuleName = str
+_ItfName = str
+_ItfIid = str
+
+
+def _get_known_namespaces() -> Tuple[
+    Mapping[_SymbolName, _ModuleName], Mapping[_ItfName, _ItfIid]
+]:
+    """Returns symbols and interfaces that are already statically defined in `ctypes`
+    and `comtypes`.
+    From `ctypes`, all the names are obtained.
+    From `comtypes`, only the names in each module's `__known_symbols__` are obtained.
+
+    Note:
+        The interfaces that should be included in `__known_symbols__` should be limited
+        to those that can be said to be bound to the design concept of COM, such as
+        `IUnknown`, and those defined in `objidl` and `oaidl`.
+        `comtypes` does NOT aim to statically define all COM object interfaces in
+        its repository.
+    """
+    known_symbols: Dict[_SymbolName, _ModuleName] = {}
+    known_interfaces: Dict[_ItfName, _ItfIid] = {}
     for mod_name in (
         "comtypes.persist",
         "comtypes.typeinfo",
         "comtypes.automation",
         "comtypes",
         "ctypes.wintypes",
         "ctypes",
     ):
         mod = importlib.import_module(mod_name)
         if hasattr(mod, "__known_symbols__"):
             names: List[str] = mod.__known_symbols__
+            for name in names:
+                tgt = getattr(mod, name)
+                if inspect.isclass(tgt) and issubclass(tgt, comtypes.IUnknown):
+                    assert name not in known_interfaces
+                    known_interfaces[name] = str(tgt._iid_)
         else:
             names = list(mod.__dict__)
         for name in names:
             known_symbols[name] = mod.__name__
-    return known_symbols
+    return known_symbols, known_interfaces
 
 
 ################################################################
 
 
 if __name__ == "__main__":
     # When started as script, generate typelib wrapper from .tlb file.
```

## Comparing `comtypes-1.4.1/comtypes/client/__init__.py` & `comtypes-1.4.2/comtypes/client/__init__.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/server/automation.py` & `comtypes-1.4.2/comtypes/server/automation.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/server/connectionpoints.py` & `comtypes-1.4.2/comtypes/server/connectionpoints.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/server/inprocserver.py` & `comtypes-1.4.2/comtypes/server/inprocserver.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/server/localserver.py` & `comtypes-1.4.2/comtypes/server/localserver.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/server/register.py` & `comtypes-1.4.2/comtypes/server/register.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/server/w_getopt.py` & `comtypes-1.4.2/comtypes/server/w_getopt.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/server/__init__.py` & `comtypes-1.4.2/comtypes/server/__init__.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/find_memleak.py` & `comtypes-1.4.2/comtypes/test/find_memleak.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/mylib.idl` & `comtypes-1.4.2/comtypes/test/mylib.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/mytypelib.idl` & `comtypes-1.4.2/comtypes/test/mytypelib.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/TestComServer.idl` & `comtypes-1.4.2/comtypes/test/TestComServer.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/TestComServer.py` & `comtypes-1.4.2/comtypes/test/TestComServer.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/TestComServer.tlb` & `comtypes-1.4.2/comtypes/test/TestComServer.tlb`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/TestDispServer.idl` & `comtypes-1.4.2/comtypes/test/TestDispServer.idl`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/TestDispServer.py` & `comtypes-1.4.2/comtypes/test/TestDispServer.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/TestDispServer.tlb` & `comtypes-1.4.2/comtypes/test/TestDispServer.tlb`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_agilent.py` & `comtypes-1.4.2/comtypes/test/test_agilent.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_avmc.py` & `comtypes-1.4.2/comtypes/test/test_avmc.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_basic.py` & `comtypes-1.4.2/comtypes/test/test_basic.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_BSTR.py` & `comtypes-1.4.2/comtypes/test/test_BSTR.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_casesensitivity.py` & `comtypes-1.4.2/comtypes/test/test_casesensitivity.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_clear_cache.py` & `comtypes-1.4.2/comtypes/test/test_clear_cache.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_client.py` & `comtypes-1.4.2/comtypes/test/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,20 +55,25 @@
 
     def test_ptr_itypelib(self):
         from comtypes import typeinfo
 
         mod = comtypes.client.GetModule(typeinfo.LoadTypeLibEx("scrrun.dll"))
         self.assertIs(mod, Scripting)
 
-    def test_imports_IEnumVARIANT_from_other_generated_modules(self):
+    def test_mscorlib(self):
         # NOTE: `codegenerator` generates code that contains unused imports,
         # but removing them are attracting wierd bugs in library-wrappers
         # which depend on externals.
-        # NOTE: `mscorlib`, which imports `IEnumVARIANT` from `stdole`.
-        comtypes.client.GetModule(("{BED7F4EA-1A96-11D2-8F08-00A0C9A6186D}",))
+        # `mscorlib` imports `stdole` wrapper module and refers`IEnumVARIANT` from it.
+        mod = comtypes.client.GetModule(("{BED7F4EA-1A96-11D2-8F08-00A0C9A6186D}",))
+        # NOTE: `ModuleGenerator` treats the `ctypes._Pointer` base class for pointers
+        # as one of the known symbols, but `mscorlib` has the `_Pointer` com interface.
+        # Even though they have the same name, `codegenerator` generates code to define
+        # the `_Pointer` interface, rather than importing `_Pointer` from `ctypes`.
+        self.assertTrue(issubclass(mod._Pointer, comtypes.IUnknown))
 
     def test_no_replacing_Patch_namespace(self):
         # NOTE: An object named `Patch` is defined in some dll.
         # Depending on how the namespace is defined in the static module,
         # `Patch` in generated modules will be replaced with
         # `comtypes.patcher.Patch`, and generating module will fail.
         # NOTE: `WindowsInstaller`, which has `Patch` definition in dll.
@@ -78,15 +83,20 @@
         # NOTE: In `MSHTML`, the name `htmlInputImage` is used both as a member of
         # the `_htmlInput` enum type and as a CoClass that has `IHTMLElement` and
         # others as interfaces.
         # If a CoClass is assigned where an integer should be assigned, such as in
         # the definition of an enumeration, the generation of the module will fail.
         # See also https://github.com/enthought/comtypes/issues/524
         with contextlib.redirect_stdout(None):  # supress warnings
-            comtypes.client.GetModule("mshtml.tlb")
+            mshtml = comtypes.client.GetModule("mshtml.tlb")
+        # When the member of an enumeration and a CoClass have the same name,
+        # the defined later one is assigned to the name in the module.
+        # By asserting whether the CoClass is assigned to that name, it ensures
+        # that the member of the enumeration is defined earlier.
+        self.assertTrue(issubclass(mshtml.htmlInputImage, comtypes.CoClass))
 
     def test_abstracted_wrapper_module_in_friendly_module(self):
         mod = comtypes.client.GetModule("scrrun.dll")
         self.assertTrue(hasattr(mod, "__wrapper_module__"))
 
     def test_raises_typerror_if_takes_unsupported(self):
         with self.assertRaises(TypeError):
```

## Comparing `comtypes-1.4.1/comtypes/test/test_client_dynamic.py` & `comtypes-1.4.2/comtypes/test/test_client_dynamic.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_collections.py` & `comtypes-1.4.2/comtypes/test/test_collections.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_comserver.py` & `comtypes-1.4.2/comtypes/test/test_comserver.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_createwrappers.py` & `comtypes-1.4.2/comtypes/test/test_createwrappers.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_dict.py` & `comtypes-1.4.2/comtypes/test/test_dict.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_dispinterface.py` & `comtypes-1.4.2/comtypes/test/test_dispinterface.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_DISPPARAMS.py` & `comtypes-1.4.2/comtypes/test/test_DISPPARAMS.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_dyndispatch.py` & `comtypes-1.4.2/comtypes/test/test_dyndispatch.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_excel.py` & `comtypes-1.4.2/comtypes/test/test_excel.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_findgendir.py` & `comtypes-1.4.2/comtypes/test/test_findgendir.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_getactiveobj.py` & `comtypes-1.4.2/comtypes/test/test_getactiveobj.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_GUID.py` & `comtypes-1.4.2/comtypes/test/test_GUID.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_ie.py` & `comtypes-1.4.2/comtypes/test/test_ie.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_ienum.py` & `comtypes-1.4.2/comtypes/test/test_ienum.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_imfattributes.py` & `comtypes-1.4.2/comtypes/test/test_imfattributes.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_inout_args.py` & `comtypes-1.4.2/comtypes/test/test_inout_args.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_msscript.py` & `comtypes-1.4.2/comtypes/test/test_msscript.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_npsupport.py` & `comtypes-1.4.2/comtypes/test/test_npsupport.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_outparam.py` & `comtypes-1.4.2/comtypes/test/test_outparam.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_propputref.py` & `comtypes-1.4.2/comtypes/test/test_propputref.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_QueryService.py` & `comtypes-1.4.2/comtypes/test/test_QueryService.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_safearray.py` & `comtypes-1.4.2/comtypes/test/test_safearray.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_sapi.py` & `comtypes-1.4.2/comtypes/test/test_sapi.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_server.py` & `comtypes-1.4.2/comtypes/test/test_server.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_showevents.py` & `comtypes-1.4.2/comtypes/test/test_showevents.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_typeinfo.py` & `comtypes-1.4.2/comtypes/test/test_typeinfo.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_urlhistory.py` & `comtypes-1.4.2/comtypes/test/test_urlhistory.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_variant.py` & `comtypes-1.4.2/comtypes/test/test_variant.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_win32com_interop.py` & `comtypes-1.4.2/comtypes/test/test_win32com_interop.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_wmi.py` & `comtypes-1.4.2/comtypes/test/test_wmi.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/test_word.py` & `comtypes-1.4.2/comtypes/test/test_word.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/test/__init__.py` & `comtypes-1.4.2/comtypes/test/__init__.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/tools/codegenerator.py` & `comtypes-1.4.2/comtypes/tools/codegenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,87 +204,88 @@
 def _to_arg_definition(
     type_name: str,
     arg_name: str,
     idlflags: List[str],
     default: _DefValType,
 ) -> str:
     if default is not None:
-        elms = (idlflags, type_name, arg_name, default)
-        code = "        (%r, %s, '%s', %r)" % elms
+        code = f"        ({idlflags!r}, {type_name}, '{arg_name}', {default!r})"
         if len(code) > 80:
             code = (
                 "        (\n"
-                "            %r,\n"
-                "            %s,\n"
-                "            '%s',\n"
-                "            %r\n"
+                f"            {idlflags!r},\n"
+                f"            {type_name},\n"
+                f"            '{arg_name}',\n"
+                f"            {default!r}\n"
                 "        )"
-            ) % elms
+            )
     else:
-        elms = (idlflags, type_name, arg_name)
-        code = "        (%r, %s, '%s')" % elms
+        code = f"        ({idlflags!r}, {type_name}, '{arg_name}')"
         if len(code) > 80:
             code = (
                 "        (\n"
-                "            %r,\n"
-                "            %s,\n"
-                "            '%s',\n"
+                f"            {idlflags!r},\n"
+                f"            {type_name},\n"
+                f"            '{arg_name}',\n"
                 "        )"
-            ) % elms
+            )
     return code
 
 
 class ComMethodGenerator(object):
     def __init__(self, m: typedesc.ComMethod, isdual: bool) -> None:
         self._m = m
         self._isdual = isdual
-        self._stream = io.StringIO()
+        self.data: List[str] = []
         self._to_type_name = TypeNamer()
 
-    def generate(self):
-        # () -> str
+    def generate(self) -> str:
         if not self._m.arguments:
             self._make_noargs()
         else:
             self._make_withargs()
-        return self._stream.getvalue()
+        return "\n".join(self.data)
 
     def _get_common_elms(self) -> Tuple[List[_IdlFlagType], str, str]:
         idlflags: List[_IdlFlagType] = []
         if self._isdual:
             idlflags.append(dispid(self._m.memid))
             idlflags.extend(self._m.idlflags)
         else:  # We don't include the dispid for non-dispatch COM interfaces
             idlflags.extend(self._m.idlflags)
         if __debug__ and self._m.doc:
             idlflags.insert(1, helpstring(self._m.doc))
         type_name = self._to_type_name(self._m.returns)
         return (idlflags, type_name, self._m.name)
 
     def _make_noargs(self) -> None:
-        elms = self._get_common_elms()
-        code = "    COMMETHOD(%r, %s, '%s')," % elms
+        flags, type_name, member_name = self._get_common_elms()
+        code = f"    COMMETHOD({flags!r}, {type_name}, '{member_name}'),"
         if len(code) > 80:
             code = (
                 "    COMMETHOD(\n"
-                "        %r,\n"
-                "        %s,\n"
-                "        '%s',\n"
+                f"        {flags!r},\n"
+                f"        {type_name},\n"
+                f"        '{member_name}',\n"
                 "    ),"
-            ) % elms
-        print(code, file=self._stream)
+            )
+        self.data.append(code)
 
     def _make_withargs(self) -> None:
+        flags, type_name, member_name = self._get_common_elms()
         code = (
-            "    COMMETHOD(\n" "        %r,\n" "        %s,\n" "        '%s',"
-        ) % self._get_common_elms()
-        print(code, file=self._stream)
+            "    COMMETHOD(\n"
+            f"        {flags!r},\n"
+            f"        {type_name},\n"
+            f"        '{member_name}',"
+        )
+        self.data.append(code)
         arglist = [_to_arg_definition(*i) for i in self._iter_args()]
-        print(",\n".join(arglist), file=self._stream)
-        print("    ),", file=self._stream)
+        self.data.append(",\n".join(arglist))
+        self.data.append("    ),")
 
     def _iter_args(self) -> Iterator[Tuple[str, str, List[str], _DefValType]]:
         for typ, arg_name, _f, _defval in self._m.arguments:
             ###########################################################
             # IDL files that contain 'open arrays' or 'conformant
             # varying arrays' method parameters are strange.
             # These arrays have both a 'size_is()' and
@@ -337,116 +338,132 @@
                 default = _defval
             yield (type_name, arg_name, idlflags, default)
 
 
 class DispMethodGenerator(object):
     def __init__(self, m: typedesc.DispMethod) -> None:
         self._m = m
-        self._stream = io.StringIO()
+        self.data: List[str] = []
         self._to_type_name = TypeNamer()
 
-    def generate(self):
-        # () -> str
+    def generate(self) -> str:
         if not self._m.arguments:
             self._make_noargs()
         else:
             self._make_withargs()
-        return self._stream.getvalue()
+        return "\n".join(self.data)
 
     def _get_common_elms(self) -> Tuple[List[_IdlFlagType], str, str]:
         idlflags: List[_IdlFlagType] = []
         idlflags.append(dispid(self._m.dispid))
         idlflags.extend(self._m.idlflags)
         if __debug__ and self._m.doc:
             idlflags.insert(1, helpstring(self._m.doc))
         type_name = self._to_type_name(self._m.returns)
         return (idlflags, type_name, self._m.name)
 
     def _make_noargs(self) -> None:
-        elms = self._get_common_elms()
-        code = "    DISPMETHOD(%r, %s, '%s')," % elms
+        flags, type_name, member_name = self._get_common_elms()
+        code = f"    DISPMETHOD({flags!r}, {type_name}, '{member_name}'),"
         if len(code) > 80:
             code = (
                 "    DISPMETHOD(\n"
-                "        %r,\n"
-                "        %s,\n"
-                "        '%s',\n"
+                f"        {flags!r},\n"
+                f"        {type_name},\n"
+                f"        '{member_name}',\n"
                 "    ),"
-            ) % elms
-        print(code, file=self._stream)
+            )
+        self.data.append(code)
 
     def _make_withargs(self) -> None:
+        flags, type_name, member_name = self._get_common_elms()
         code = (
-            "    DISPMETHOD(\n" "        %r,\n" "        %s,\n" "        '%s',"
-        ) % self._get_common_elms()
-        print(code, file=self._stream)
+            "    DISPMETHOD(\n"
+            f"        {flags!r},\n"
+            f"        {type_name},\n"
+            f"        '{member_name}',"
+        )
+        self.data.append(code)
         arglist = [_to_arg_definition(*i) for i in self._iter_args()]
-        print(",\n".join(arglist), file=self._stream)
-        print("    ),", file=self._stream)
+        self.data.append(",\n".join(arglist))
+        self.data.append("    ),")
 
     def _iter_args(self) -> Iterator[Tuple[str, str, List[str], _DefValType]]:
         for typ, arg_name, idlflags, default in self._m.arguments:
             type_name = self._to_type_name(typ)
             yield (type_name, arg_name, idlflags, default)
 
 
 class DispPropertyGenerator(object):
     def __init__(self, m: typedesc.DispProperty) -> None:
         self._m = m
         self._to_type_name = TypeNamer()
 
-    def generate(self):
-        # () -> str
-        elms = self._get_common_elms()
-        code = "    DISPPROPERTY(%r, %s, '%s')," % elms
+    def generate(self) -> str:
+        flags, type_name, member_name = self._get_common_elms()
+        code = f"    DISPPROPERTY({flags!r}, {type_name}, '{member_name}'),"
         if len(code) > 80:
             code = (
                 "    DISPPROPERTY(\n"
-                "        %r,\n"
-                "        %s,\n"
-                "        '%s'\n"
+                f"        {flags!r},\n"
+                f"        {type_name},\n"
+                f"        '{member_name}'\n"
                 "    ),"
-            ) % elms
-        return code + "\n"
+            )
+        return code
 
     def _get_common_elms(self) -> Tuple[List[_IdlFlagType], str, str]:
         idlflags: List[_IdlFlagType] = []
         idlflags.append(dispid(self._m.dispid))
         idlflags.extend(self._m.idlflags)
         if __debug__ and self._m.doc:
             idlflags.insert(1, helpstring(self._m.doc))
         type_name = self._to_type_name(self._m.typ)
         return (idlflags, type_name, self._m.name)
 
 
+_InterfaceTypeDesc = _UnionT[
+    typedesc.ComInterface,
+    typedesc.ComInterfaceHead,
+    typedesc.ComInterfaceBody,
+    typedesc.DispInterface,
+    typedesc.DispInterfaceHead,
+    typedesc.DispInterfaceBody,
+]
+
+
 class CodeGenerator(object):
-    def __init__(self, known_symbols=None):
+    def __init__(self, known_symbols=None, known_interfaces=None) -> None:
         self.stream = io.StringIO()
         self.imports = ImportedNamespaces()
         self.declarations = DeclaredNamespaces()
         self.enums = EnumerationNamespaces()
+        self.unnamed_enum_members: List[Tuple[str, int]] = []
         self._to_type_name = TypeNamer()
         self.known_symbols = known_symbols or {}
+        self.known_interfaces = known_interfaces or {}
 
         self.done = set()  # type descriptions that have been generated
         self.names = set()  # names that have been generated
         self.externals = []  # typelibs imported to generated module
         self.aliases: Dict[str, str] = {}
         self.last_item_class = False
 
     def generate(self, item):
         if item in self.done:
             return
+        if self._is_interface_typedesc(item):
+            self._define_interface(item)
+            return
         if isinstance(item, typedesc.StructureHead):
             name = getattr(item.struct, "name", None)
         else:
             name = getattr(item, "name", None)
         if name in self.known_symbols:
             self.imports.add(name, symbols=self.known_symbols)
-
             self.done.add(item)
             if isinstance(item, typedesc.Structure):
                 self.done.add(item.get_head())
                 self.done.add(item.get_body())
             return
         mth = getattr(self, type(item).__name__)
         # to avoid infinite recursion, we have to mark it as done
@@ -568,14 +585,20 @@
         print("if TYPE_CHECKING:", file=output)
         print("    from typing import Any, Tuple", file=output)
         print("    from comtypes import hints", file=output)
         print(file=output)
         print(file=output)
         print(self.declarations.getvalue(), file=output)
         print(file=output)
+        if self.unnamed_enum_members:
+            print("# values for unnamed enumeration", file=output)
+            for n, v in self.unnamed_enum_members:
+                print(f"{n} = {v}", file=output)
+            print(file=output)
+        print(self.enums.to_constants(), file=output)
         print(self.stream.getvalue(), file=output)
         print(self._make_dunder_all_part(), file=output)
         print(file=output)
         if tlib_mtime is not None:
             print("_check_version(%r, %f)" % (version, tlib_mtime), file=output)
         return output.getvalue()
 
@@ -592,15 +615,15 @@
         output = io.StringIO()
         print("from enum import IntFlag", file=output)
         print(file=output)
         print(f"import {modname} as __wrapper_module__", file=output)
         print(self._make_friendly_module_import_part(modname), file=output)
         print(file=output)
         print(file=output)
-        print(self.enums.getvalue(), file=output)
+        print(self.enums.to_intflags(), file=output)
         print(file=output)
         print(file=output)
         enum_aliases = self.enum_aliases
         if enum_aliases:
             for k, v in enum_aliases.items():
                 print(f"{k} = {v}", file=output)
             print(file=output)
@@ -665,29 +688,25 @@
         self.last_item_class = False
         value = int(tp.value)
         if keyword.iskeyword(tp.name):
             # XXX use logging!
             if __warn_on_munge__:
                 print("# Fixing keyword as EnumValue for %s" % tp.name)
         tp_name = self._to_type_name(tp)
-        print("%s = %d" % (tp_name, value), file=self.stream)
         if tp.enumeration.name:
             self.enums.add(tp.enumeration.name, tp_name, value)
+        else:
+            self.unnamed_enum_members.append((tp_name, value))
         self.names.add(tp_name)
 
     def Enumeration(self, tp: typedesc.Enumeration) -> None:
         self.last_item_class = False
-        if tp.name:
-            print("# values for enumeration '%s'" % tp.name, file=self.stream)
-        else:
-            print("# values for unnamed enumeration", file=self.stream)
         for item in tp.values:
             self.generate(item)
         if tp.name:
-            print("%s = c_int  # enum" % tp.name, file=self.stream)
             self.names.add(tp.name)
 
     def Typedef(self, tp: typedesc.Typedef) -> None:
         if isinstance(tp.typ, (typedesc.Structure, typedesc.Union)):
             self.generate(tp.typ.get_head())
             self.more.add(tp.typ)
         else:
@@ -1062,38 +1081,87 @@
             print(
                 "%s._outgoing_interfaces_ = [%s]" % (coclass.name, ", ".join(sources)),
                 file=self.stream,
             )
 
         self.names.add(coclass.name)
 
+    def _is_interface_typedesc(
+        self, item: Any
+    ) -> "comtypes.hints.TypeGuard[_InterfaceTypeDesc]":
+        return isinstance(
+            item,
+            (
+                typedesc.ComInterface,
+                typedesc.ComInterfaceHead,
+                typedesc.ComInterfaceBody,
+                typedesc.DispInterface,
+                typedesc.DispInterfaceHead,
+                typedesc.DispInterfaceBody,
+            ),
+        )
+
+    def _define_interface(self, item: _InterfaceTypeDesc) -> None:
+        if isinstance(
+            item,
+            (
+                typedesc.ComInterfaceHead,
+                typedesc.ComInterfaceBody,
+                typedesc.DispInterfaceHead,
+                typedesc.DispInterfaceBody,
+            ),
+        ):
+            if self._is_known_interface(item.itf):
+                self.imports.add(item.itf.name, symbols=self.known_symbols)
+                self.done.add(item)
+                return
+        elif isinstance(item, (typedesc.ComInterface, typedesc.DispInterface)):
+            if self._is_known_interface(item):
+                self.imports.add(item.name, symbols=self.known_symbols)
+                self.done.add(item)
+                self.done.add(item.get_head())
+                self.done.add(item.get_body())
+                return
+        else:
+            raise TypeError
+        self.done.add(item)  # to avoid infinite recursion.
+        mth = getattr(self, type(item).__name__)
+        mth(item)
+
     def ComInterface(self, itf: typedesc.ComInterface) -> None:
         self.generate(itf.get_head())
         self.generate(itf.get_body())
         self.names.add(itf.name)
 
+    def _is_known_interface(
+        self, item: _UnionT[typedesc.ComInterface, typedesc.DispInterface]
+    ) -> bool:
+        """Returns whether an interface is statically defined in `comtypes`,
+        based on its name and iid.
+        """
+        if item.name in self.known_interfaces:
+            return self.known_interfaces[item.name] == item.iid
+        return False
+
     def _is_enuminterface(self, itf: typedesc.ComInterface) -> bool:
         # Check if this is an IEnumXXX interface
         if not itf.name.startswith("IEnum"):
             return False
         member_names = [mth.name for mth in itf.members]
         for name in ("Next", "Skip", "Reset", "Clone"):
             if name not in member_names:
                 return False
         return True
 
     def ComInterfaceHead(self, head: typedesc.ComInterfaceHead) -> None:
-        if head.itf.name in self.known_symbols:
-            return
-        base = head.itf.base
         if head.itf.base is None:
             # we don't beed to generate IUnknown
             return
-        self.generate(base.get_head())
-        self.more.add(base)
+        self.generate(head.itf.base.get_head())
+        self.more.add(head.itf.base)
         basename = self._to_type_name(head.itf.base)
 
         self.imports.add("comtypes", "GUID")
 
         if not self.last_item_class:
             print(file=self.stream)
             print(file=self.stream)
@@ -1126,19 +1194,19 @@
             print("        self.Reset()", file=self.stream)
             print("        self.Skip(index)", file=self.stream)
             print("        item, fetched = self.Next(1)", file=self.stream)
             print("        if fetched:", file=self.stream)
             print("            return item", file=self.stream)
             print("        raise IndexError(index)", file=self.stream)
 
-        annotaions = typeannotator.ComInterfaceMembersAnnotator(head.itf).generate()
-        if annotaions:
+        annotations = typeannotator.ComInterfaceMembersAnnotator(head.itf).generate()
+        if annotations:
             print(file=self.stream)
             print("    if TYPE_CHECKING:  # commembers", file=self.stream)
-            print(annotaions, file=self.stream, end="")
+            print(annotations, file=self.stream)
 
         print(file=self.stream)
         print(file=self.stream)
 
     def ComInterfaceBody(self, body: typedesc.ComInterfaceBody) -> None:
         # The base class must be fully generated, including the
         # _methods_ list.
@@ -1254,19 +1322,19 @@
         if doc:
             print(self._to_docstring(doc), file=self.stream)
         print("    _case_insensitive_ = True", file=self.stream)
         print("    _iid_ = GUID(%r)" % head.itf.iid, file=self.stream)
         print("    _idlflags_ = %s" % head.itf.idlflags, file=self.stream)
         print("    _methods_ = []", file=self.stream)
 
-        annotaions = typeannotator.DispInterfaceMembersAnnotator(head.itf).generate()
-        if annotaions:
+        annotations = typeannotator.DispInterfaceMembersAnnotator(head.itf).generate()
+        if annotations:
             print(file=self.stream)
             print("    if TYPE_CHECKING:  # dispmembers", file=self.stream)
-            print(annotaions, file=self.stream, end="")
+            print(annotations, file=self.stream)
 
         print(file=self.stream)
         print(file=self.stream)
 
     def DispInterfaceBody(self, body: typedesc.DispInterfaceBody) -> None:
         # make sure we can generate the body
         for m in body.itf.members:
@@ -1300,15 +1368,15 @@
     def make_ComMethod(self, m: typedesc.ComMethod, isdual: bool) -> None:
         self.imports.add("comtypes", "COMMETHOD")
         if isdual:
             self.imports.add("comtypes", "dispid")
         if __debug__ and m.doc:
             self.imports.add("comtypes", "helpstring")
         gen = ComMethodGenerator(m, isdual)
-        print(gen.generate(), file=self.stream, end="")
+        print(gen.generate(), file=self.stream)
         self.last_item_class = False
         for typ, _, _, default in m.arguments:
             if isinstance(typ, typedesc.ComInterface):
                 self.declarations.add(
                     "OPENARRAY",
                     "POINTER(c_ubyte)",
                     "hack, see comtypes/tools/codegenerator.py",
@@ -1318,27 +1386,27 @@
 
     def make_DispMethod(self, m: typedesc.DispMethod) -> None:
         self.imports.add("comtypes", "DISPMETHOD")
         self.imports.add("comtypes", "dispid")
         if __debug__ and m.doc:
             self.imports.add("comtypes", "helpstring")
         gen = DispMethodGenerator(m)
-        print(gen.generate(), file=self.stream, end="")
+        print(gen.generate(), file=self.stream)
         self.last_item_class = False
         for _, _, _, default in m.arguments:
             if default is not None:
                 self.need_VARIANT_imports(default)
 
     def make_DispProperty(self, prop: typedesc.DispProperty) -> None:
         self.imports.add("comtypes", "DISPPROPERTY")
         self.imports.add("comtypes", "dispid")
         if __debug__ and prop.doc:
             self.imports.add("comtypes", "helpstring")
         gen = DispPropertyGenerator(prop)
-        print(gen.generate(), file=self.stream, end="")
+        print(gen.generate(), file=self.stream)
         self.last_item_class = False
 
 
 class TypeNamer(object):
     def __call__(self, t: Any) -> str:
         # Return a string, containing an expression which can be used
         # to refer to the type. Assumes the 'from ctypes import *'
@@ -1548,38 +1616,59 @@
     def __init__(self):
         self.data: Dict[str, List[Tuple[str, int]]] = {}
 
     def add(self, enum_name: str, member_name: str, value: int) -> None:
         """Adds a namespace will be enumeration and its member.
 
         Examples:
+            <BLANKLINE> is necessary for doctest
             >>> enums = EnumerationNamespaces()
             >>> enums.add('Foo', 'ham', 1)
             >>> enums.add('Foo', 'spam', 2)
             >>> enums.add('Bar', 'bacon', 3)
             >>> assert 'Foo' in enums
             >>> assert 'Baz' not in enums
-            >>> print(enums.getvalue())  # <BLANKLINE> is necessary for doctest
+            >>> print(enums.to_intflags())
             class Foo(IntFlag):
                 ham = 1
                 spam = 2
             <BLANKLINE>
             <BLANKLINE>
             class Bar(IntFlag):
                 bacon = 3
+            >>> print(enums.to_constants())
+            # values for enumeration 'Foo'
+            ham = 1
+            spam = 2
+            Foo = c_int  # enum
+            <BLANKLINE>
+            # values for enumeration 'Bar'
+            bacon = 3
+            Bar = c_int  # enum
         """
         self.data.setdefault(enum_name, []).append((member_name, value))
 
     def __contains__(self, item: str) -> bool:
         return item in self.data
 
     def get_symbols(self) -> Set[str]:
         return set(self.data)
 
-    def getvalue(self) -> str:
+    def to_constants(self) -> str:
+        blocks = []
+        for enum_name, enum_members in self.data.items():
+            lines = []
+            lines.append(f"# values for enumeration '{enum_name}'")
+            for n, v in enum_members:
+                lines.append(f"{n} = {v}")
+            lines.append(f"{enum_name} = c_int  # enum")
+            blocks.append("\n".join(lines))
+        return "\n\n".join(blocks)
+
+    def to_intflags(self) -> str:
         blocks = []
         for enum_name, enum_members in self.data.items():
             lines = []
             lines.append(f"class {enum_name}(IntFlag):")
             for member_name, value in enum_members:
                 lines.append(f"    {member_name} = {value}")
             blocks.append("\n".join(lines))
```

## Comparing `comtypes-1.4.1/comtypes/tools/tlbparser.py` & `comtypes-1.4.2/comtypes/tools/tlbparser.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes/tools/typeannotator.py` & `comtypes-1.4.2/comtypes/tools/typeannotator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import abc
-import io
 import keyword
 from typing import (
     Any,
     Dict,
     Generic,
     Iterable,
     Iterator,
@@ -51,15 +50,15 @@
 _CatMths = Tuple[  # categorized methods
     str, Optional[_T_MTD], Optional[_T_MTD], Optional[_T_MTD], Optional[_T_MTD]
 ]
 
 
 class _MethodsAnnotator(abc.ABC, Generic[_T_MTD]):
     def __init__(self) -> None:
-        self.stream = io.StringIO()
+        self.data: List[str] = []
 
     @abc.abstractmethod
     def to_method_annotator(self, method: _T_MTD) -> _MethodAnnotator[_T_MTD]:
         ...
 
     def _iter_methods(self, members: Iterable[_T_MTD]) -> Iterator[_CatMths[_T_MTD]]:
         methods: Dict[str, List[Optional[_T_MTD]]] = {}
@@ -96,15 +95,15 @@
             elif not fget and not fput and fputref:
                 self._gen_prop_putref(name, fputref)
             elif not fget and fput and fputref:
                 self._gen_prop_put_putref(name, fput, fputref)
             else:
                 self._define_member(f"pass  # what does `{name}` behave?")
             self._patch_dunder(name)
-        return self.stream.getvalue()
+        return "\n".join(f"        {d}" for d in self.data)
 
     def _patch_dunder(self, name: str) -> None:
         if name == "Count":
             self._define_member(f"__len__ = hints.to_dunder_len({name})")
         if name == "Item":
             self._define_member(f"__call__ = hints.to_dunder_call({name})")
             self._define_member(f"__getitem__ = hints.to_dunder_getitem({name})")
@@ -137,15 +136,15 @@
         elif not getter and setter:
             content = f"{mem_name} = hints.normal_property(fset={setter})"
         else:
             return
         self._define_member(content)
 
     def _define_member(self, content: str) -> None:
-        print(f"        {content}", file=self.stream)
+        self.data.append(content)
 
     def _gen_method(self, name: str, mth: _T_MTD) -> None:
         self._define_member(self.to_method_annotator(mth).getvalue(name))
 
     def _gen_prop_get(self, name: str, fget: _T_MTD) -> None:
         getter_anno = self.to_method_annotator(fget)
         self._define_member(getter_anno.getvalue(f"_get_{name}"))
@@ -233,21 +232,21 @@
             if default is None:
                 if has_optional:
                     # probably propput or propputref
                     # HACK: Something that goes into this conditional branch
                     #       should be a special callback.
                     inargs.append("**kwargs: Any")
                     break
-                inargs.append(f"{argname}: Any")
+                inargs.append(f"{argname}: hints.Incomplete")
             else:
-                inargs.append(f"{argname}: Any = ...")
+                inargs.append(f"{argname}: hints.Incomplete = ...")
                 has_optional = True
-        outargs = ["Any" for _ in self._iter_outarg_specs()]
+        outargs = ["hints.Incomplete" for _ in self._iter_outarg_specs()]
         if not outargs:
-            out = "Any"
+            out = "hints.Hresult"
         elif len(outargs) == 1:
             out = outargs[0]
         else:
             out = "Tuple[" + ", ".join(outargs) + "]"
         in_ = ("self, " + ", ".join(inargs)) if inargs else "self"
         return f"def {name}({in_}) -> {out}: ..."
 
@@ -276,32 +275,31 @@
             if default is None:
                 if has_optional:
                     # probably propput or propputref
                     # HACK: Something that goes into this conditional branch
                     #       should be a special callback.
                     inargs.append("**kwargs: Any")
                     break
-                inargs.append(f"{argname}: Any")
+                inargs.append(f"{argname}: hints.Incomplete")
             else:
-                inargs.append(f"{argname}: Any = ...")
+                inargs.append(f"{argname}: hints.Incomplete = ...")
                 has_optional = True
-        out = "Any"
+        out = "hints.Incomplete"
         in_ = ("self, " + ", ".join(inargs)) if inargs else "self"
         return f"def {name}({in_}) -> {out}: ..."
 
 
 class DispMethodsAnnotator(_MethodsAnnotator[typedesc.DispMethod]):
     def to_method_annotator(self, m: typedesc.DispMethod) -> DispMethodAnnotator:
         return DispMethodAnnotator(m)
 
 
 class DispInterfaceMembersAnnotator(object):
     def __init__(self, itf: typedesc.DispInterface):
         self.itf = itf
-        self.stream = io.StringIO()
 
     def _categorize_members(
         self,
     ) -> Tuple[Iterable[typedesc.DispProperty], Iterable[typedesc.DispMethod]]:
         props: List[typedesc.DispProperty] = []
         methods: List[typedesc.DispMethod] = []
         for mem in self.itf.members:
@@ -309,11 +307,15 @@
                 methods.append(mem)
             elif isinstance(mem, typedesc.DispProperty):
                 props.append(mem)
         return props, methods
 
     def generate(self) -> str:
         props, methods = self._categorize_members()
+        property_lines: List[str] = []
         for mem in props:
-            print("        @property  # dispprop", file=self.stream)
-            print(f"        def {mem.name}(self) -> Any: ...", file=self.stream)
-        return self.stream.getvalue() + DispMethodsAnnotator().generate(methods)
+            property_lines.append("@property  # dispprop")
+            out = "hints.Incomplete"
+            property_lines.append(f"def {mem.name}(self) -> {out}: ...")
+        dispprops = "\n".join(f"        {p}" for p in property_lines)
+        dispmethods = DispMethodsAnnotator().generate(methods)
+        return "\n".join(d for d in (dispprops, dispmethods) if d)
```

## Comparing `comtypes-1.4.1/comtypes/tools/typedesc.py` & `comtypes-1.4.2/comtypes/tools/typedesc.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
 
 class ComInterface(object):
     def __init__(
         self,
         name: str,
         members: List[ComMethod],
-        base: Any,
+        base: "Optional[ComInterface]",
         iid: str,
         idlflags: List[str],
     ) -> None:
         self.name = name
         self.members = members
         self.base = base
         self.iid = iid
```

## Comparing `comtypes-1.4.1/comtypes/tools/typedesc_base.py` & `comtypes-1.4.2/comtypes/tools/typedesc_base.py`

 * *Files identical despite different names*

## Comparing `comtypes-1.4.1/comtypes.egg-info/PKG-INFO` & `comtypes-1.4.2/comtypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comtypes
-Version: 1.4.1
+Version: 1.4.2
 Summary: Pure Python COM package
 Home-page: https://github.com/enthought/comtypes
 Download-URL: https://github.com/enthought/comtypes/releases
 Author: Thomas Heller
 Author-email: theller@python.net
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `comtypes-1.4.1/comtypes.egg-info/SOURCES.txt` & `comtypes-1.4.2/comtypes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 comtypes/test/test_agilent.py
 comtypes/test/test_avmc.py
 comtypes/test/test_basic.py
 comtypes/test/test_casesensitivity.py
 comtypes/test/test_clear_cache.py
 comtypes/test/test_client.py
 comtypes/test/test_client_dynamic.py
+comtypes/test/test_client_regenerate_modules.py
 comtypes/test/test_collections.py
 comtypes/test/test_comserver.py
 comtypes/test/test_createwrappers.py
 comtypes/test/test_dict.py
 comtypes/test/test_dispinterface.py
 comtypes/test/test_dyndispatch.py
 comtypes/test/test_excel.py
```

