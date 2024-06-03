# Comparing `tmp/Jvav-2.0.0.tar.gz` & `tmp/Jvav-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-fezxj5tn/Jvav-2.0.0.tar", last modified: Mon Jun  3 05:35:48 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-xldct1s5/Jvav-2.1.0.tar", last modified: Mon Jun  3 08:10:52 2024, max compression
```

## Comparing `Jvav-2.0.0.tar` & `Jvav-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 05:35:48.000000 Jvav-2.0.0/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-2.0.0/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      579 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-06-03 05:35:48.000000 Jvav-2.0.0/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-2.0.0/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-2.0.0/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-06-03 05:35:48.000000 Jvav-2.0.0/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-2.0.0/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 05:35:48.000000 Jvav-2.0.0/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      455 2024-06-03 05:35:04.000000 Jvav-2.0.0/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-2.0.0/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    77436 2024-06-03 05:34:21.000000 Jvav-2.0.0/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:49:11.000000 Jvav-2.0.0/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-06-03 05:35:48.000000 Jvav-2.0.0/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-06-03 05:35:04.000000 Jvav-2.0.0/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 08:10:52.000000 Jvav-2.1.0/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 08:10:52.000000 Jvav-2.1.0/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4200 2024-06-03 08:10:52.000000 Jvav-2.1.0/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-06-03 08:10:52.000000 Jvav-2.1.0/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-06-03 08:10:52.000000 Jvav-2.1.0/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-06-03 08:10:52.000000 Jvav-2.1.0/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-2.1.0/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-06-03 08:10:52.000000 Jvav-2.1.0/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-06-03 08:10:52.000000 Jvav-2.1.0/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-2.1.0/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-2.1.0/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4200 2024-06-03 08:10:52.000000 Jvav-2.1.0/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3470 2024-06-03 05:36:29.000000 Jvav-2.1.0/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-06-03 08:10:52.000000 Jvav-2.1.0/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      455 2024-06-03 08:10:25.000000 Jvav-2.1.0/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-2.1.0/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    77070 2024-06-03 08:09:40.000000 Jvav-2.1.0/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:49:11.000000 Jvav-2.1.0/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-06-03 08:10:52.000000 Jvav-2.1.0/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-06-03 08:10:25.000000 Jvav-2.1.0/setup.py
```

### Comparing `Jvav-2.0.0/Jvav.egg-info/PKG-INFO` & `Jvav-2.1.0/Jvav.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 2.0.0
+Version: 2.1.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
@@ -36,15 +36,14 @@
 - JavLibUtil
 - JavBusUtil
 - AvgleUtil
 - MagnetUtil
 - SukebeiUtil
 - WikiUtil
 - TransUtil
-- SgpUtil
 - RankUtil
 
 ```py
 # A sample for DmmUtil
 import jvav
 
 util = jvav.DmmUtil()
@@ -107,17 +106,15 @@
 And then you can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~
 
 ## TODO
 
 The following are some functions to be implemented, and I look forward to your contribution~ 
 
-- [ ] fix SgpUtil(currently not work)
 - [ ] support RankUtil in CMD
-- [ ] fix JavLibUtil(currently not work because of cloudflare)
 - [x] cache the successful query results locally (Thanks: [@akynazh](https://github.com/akynazh))
 - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake))
 - [ ] support db.msin.jp
 - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh))
 
 ## Thanks
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: Jvav Version: 2.0.0 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 2.1.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
 :: Indexing/Search Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # Jvav Useful tools for Jav. Supports Python
 library operations and command-line usage, with additional proxy options and
 cache support. ## INSTALL ``` # python >= 3.7 pip install jvav -U ``` ## LIB -
 DmmUtil - JavDbUtil - JavLibUtil - JavBusUtil - AvgleUtil - MagnetUtil -
-SukebeiUtil - WikiUtil - TransUtil - SgpUtil - RankUtil ```py # A sample for
-DmmUtil import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
+SukebeiUtil - WikiUtil - TransUtil - RankUtil ```py # A sample for DmmUtil
+import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
 ('å°åç±è') util.get_score_by_id('cawd-441') util.get_all_top_stars() ```
 ## CMD ```shell usage: cmd.py [-h] [-v] [-av1 AV1] [-av2 AV2] [-av3 AV3] [-sg
 SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn SRN] [-tg TG] [-pv1 PV1] [-pv2 PV2]
 [-tp] [-p PROXY] optional arguments: -h, --help show this help message and exit
 -v, --version Check version -av1 AV1 Followed by a code, search this code on
 JavBus -av2 AV2 Followed by a code, search this code on Sukebei -av3 AV3
 Followed by a code, search this code on JavDb -sg SG Followed by a code, search
@@ -34,15 +34,13 @@
 development, please use python <= 3.7. And it is recommended to use python
 virtual environment to avoid some unnecessary problems. Here is my developing
 steps: ```shell git clone https://github.com/akynazh/jvav.git cd jvav ~/.pyenv/
 versions/3.7.12/bin/python -m venv .venv source ./.venv/bin/activate pip3
 install -r requirements.txt ``` And then you can enjoy coding! Remember to
 write or run test cases in `tests/test.py`. Please make sure the test is okay
 before submitting your code~ ## TODO The following are some functions to be
-implemented, and I look forward to your contribution~ - [ ] fix SgpUtil
-(currently not work) - [ ] support RankUtil in CMD - [ ] fix JavLibUtil
-(currently not work because of cloudflare) - [x] cache the successful query
-results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x] support
-javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) - [ ]
-support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://
-github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains
-for their support to this project!
+implemented, and I look forward to your contribution~ - [ ] support RankUtil in
+CMD - [x] cache the successful query results locally (Thanks: [@akynazh](https:
+//github.com/akynazh)) - [x] support javdb.com (Thanks: [@Steven-Fake](https://
+github.com/Steven-Fake)) - [ ] support db.msin.jp - [x] support JavDbUtil in
+cmd (Thanks: [@akynazh](https://github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ 
+_(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains for their support to this project!
```

### Comparing `Jvav-2.0.0/Jvav.egg-info/requires.txt` & `Jvav-2.1.0/Jvav.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Jvav-2.0.0/LICENSE` & `Jvav-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-2.0.0/PKG-INFO` & `Jvav-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 2.0.0
+Version: 2.1.0
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
@@ -36,15 +36,14 @@
 - JavLibUtil
 - JavBusUtil
 - AvgleUtil
 - MagnetUtil
 - SukebeiUtil
 - WikiUtil
 - TransUtil
-- SgpUtil
 - RankUtil
 
 ```py
 # A sample for DmmUtil
 import jvav
 
 util = jvav.DmmUtil()
@@ -107,17 +106,15 @@
 And then you can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~
 
 ## TODO
 
 The following are some functions to be implemented, and I look forward to your contribution~ 
 
-- [ ] fix SgpUtil(currently not work)
 - [ ] support RankUtil in CMD
-- [ ] fix JavLibUtil(currently not work because of cloudflare)
 - [x] cache the successful query results locally (Thanks: [@akynazh](https://github.com/akynazh))
 - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake))
 - [ ] support db.msin.jp
 - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh))
 
 ## Thanks
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: Jvav Version: 2.0.0 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 2.1.0 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
 :: Indexing/Search Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE # Jvav Useful tools for Jav. Supports Python
 library operations and command-line usage, with additional proxy options and
 cache support. ## INSTALL ``` # python >= 3.7 pip install jvav -U ``` ## LIB -
 DmmUtil - JavDbUtil - JavLibUtil - JavBusUtil - AvgleUtil - MagnetUtil -
-SukebeiUtil - WikiUtil - TransUtil - SgpUtil - RankUtil ```py # A sample for
-DmmUtil import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
+SukebeiUtil - WikiUtil - TransUtil - RankUtil ```py # A sample for DmmUtil
+import jvav util = jvav.DmmUtil() util.get_nice_avs_by_star_name
 ('å°åç±è') util.get_score_by_id('cawd-441') util.get_all_top_stars() ```
 ## CMD ```shell usage: cmd.py [-h] [-v] [-av1 AV1] [-av2 AV2] [-av3 AV3] [-sg
 SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn SRN] [-tg TG] [-pv1 PV1] [-pv2 PV2]
 [-tp] [-p PROXY] optional arguments: -h, --help show this help message and exit
 -v, --version Check version -av1 AV1 Followed by a code, search this code on
 JavBus -av2 AV2 Followed by a code, search this code on Sukebei -av3 AV3
 Followed by a code, search this code on JavDb -sg SG Followed by a code, search
@@ -34,15 +34,13 @@
 development, please use python <= 3.7. And it is recommended to use python
 virtual environment to avoid some unnecessary problems. Here is my developing
 steps: ```shell git clone https://github.com/akynazh/jvav.git cd jvav ~/.pyenv/
 versions/3.7.12/bin/python -m venv .venv source ./.venv/bin/activate pip3
 install -r requirements.txt ``` And then you can enjoy coding! Remember to
 write or run test cases in `tests/test.py`. Please make sure the test is okay
 before submitting your code~ ## TODO The following are some functions to be
-implemented, and I look forward to your contribution~ - [ ] fix SgpUtil
-(currently not work) - [ ] support RankUtil in CMD - [ ] fix JavLibUtil
-(currently not work because of cloudflare) - [x] cache the successful query
-results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x] support
-javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) - [ ]
-support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://
-github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains
-for their support to this project!
+implemented, and I look forward to your contribution~ - [ ] support RankUtil in
+CMD - [x] cache the successful query results locally (Thanks: [@akynazh](https:
+//github.com/akynazh)) - [x] support javdb.com (Thanks: [@Steven-Fake](https://
+github.com/Steven-Fake)) - [ ] support db.msin.jp - [x] support JavDbUtil in
+cmd (Thanks: [@akynazh](https://github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ 
+_(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains for their support to this project!
```

### Comparing `Jvav-2.0.0/README.md` & `Jvav-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 - JavLibUtil
 - JavBusUtil
 - AvgleUtil
 - MagnetUtil
 - SukebeiUtil
 - WikiUtil
 - TransUtil
-- SgpUtil
 - RankUtil
 
 ```py
 # A sample for DmmUtil
 import jvav
 
 util = jvav.DmmUtil()
@@ -87,17 +86,15 @@
 And then you can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~
 
 ## TODO
 
 The following are some functions to be implemented, and I look forward to your contribution~ 
 
-- [ ] fix SgpUtil(currently not work)
 - [ ] support RankUtil in CMD
-- [ ] fix JavLibUtil(currently not work because of cloudflare)
 - [x] cache the successful query results locally (Thanks: [@akynazh](https://github.com/akynazh))
 - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake))
 - [ ] support db.msin.jp
 - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://github.com/akynazh))
 
 ## Thanks
```

#### html2text {}

```diff
@@ -1,38 +1,37 @@
 # Jvav Useful tools for Jav. Supports Python library operations and command-
 line usage, with additional proxy options and cache support. ## INSTALL ``` #
 python >= 3.7 pip install jvav -U ``` ## LIB - DmmUtil - JavDbUtil - JavLibUtil
 - JavBusUtil - AvgleUtil - MagnetUtil - SukebeiUtil - WikiUtil - TransUtil -
-SgpUtil - RankUtil ```py # A sample for DmmUtil import jvav util = jvav.DmmUtil
-() util.get_nice_avs_by_star_name('å°åç±è') util.get_score_by_id('cawd-
-441') util.get_all_top_stars() ``` ## CMD ```shell usage: cmd.py [-h] [-v] [-
-av1 AV1] [-av2 AV2] [-av3 AV3] [-sg SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn
-SRN] [-tg TG] [-pv1 PV1] [-pv2 PV2] [-tp] [-p PROXY] optional arguments: -h, --
-help show this help message and exit -v, --version Check version -av1 AV1
-Followed by a code, search this code on JavBus -av2 AV2 Followed by a code,
-search this code on Sukebei -av3 AV3 Followed by a code, search this code on
-JavDb -sg SG Followed by a code, search the explainer video of this code -auth
-AUTH Followed by a authentication code for JavBus, get it from cookie key:
-bus_auth -nc Filter out high-definition subtitles magnet links -uc Filter out
-uncoded magnet links -sr SR Followed by an actress name, get a list of high-
-rated codes based on the actress name -srn SRN Followed by an actress name, get
-a list of the most recent codes based on the actress name -tg TG Followed by a
-keyword, search for codes based on the keyword -pv1 PV1 Followed by a code, get
-the corresponding preview video of the code on DMM -pv2 PV2 Follow a code, get
-the corresponding preview video of the code on Avgle -tp Get the top 25 ranking
-of DMM actresses -p PROXY, --proxy PROXY Followed by a proxy server address (by
+RankUtil ```py # A sample for DmmUtil import jvav util = jvav.DmmUtil()
+util.get_nice_avs_by_star_name('å°åç±è') util.get_score_by_id('cawd-441')
+util.get_all_top_stars() ``` ## CMD ```shell usage: cmd.py [-h] [-v] [-av1 AV1]
+[-av2 AV2] [-av3 AV3] [-sg SG] [-auth AUTH] [-nc] [-uc] [-sr SR] [-srn SRN] [-
+tg TG] [-pv1 PV1] [-pv2 PV2] [-tp] [-p PROXY] optional arguments: -h, --help
+show this help message and exit -v, --version Check version -av1 AV1 Followed
+by a code, search this code on JavBus -av2 AV2 Followed by a code, search this
+code on Sukebei -av3 AV3 Followed by a code, search this code on JavDb -sg SG
+Followed by a code, search the explainer video of this code -auth AUTH Followed
+by a authentication code for JavBus, get it from cookie key: bus_auth -nc
+Filter out high-definition subtitles magnet links -uc Filter out uncoded magnet
+links -sr SR Followed by an actress name, get a list of high-rated codes based
+on the actress name -srn SRN Followed by an actress name, get a list of the
+most recent codes based on the actress name -tg TG Followed by a keyword,
+search for codes based on the keyword -pv1 PV1 Followed by a code, get the
+corresponding preview video of the code on DMM -pv2 PV2 Follow a code, get the
+corresponding preview video of the code on Avgle -tp Get the top 25 ranking of
+DMM actresses -p PROXY, --proxy PROXY Followed by a proxy server address (by
 default reads the value of the environment variable http_proxy) ``` ## DEV I
 use python-3.7.12 for development, please use python <= 3.7. And it is
 recommended to use python virtual environment to avoid some unnecessary
 problems. Here is my developing steps: ```shell git clone https://github.com/
 akynazh/jvav.git cd jvav ~/.pyenv/versions/3.7.12/bin/python -m venv .venv
 source ./.venv/bin/activate pip3 install -r requirements.txt ``` And then you
 can enjoy coding! Remember to write or run test cases in `tests/test.py`.
 Please make sure the test is okay before submitting your code~ ## TODO The
 following are some functions to be implemented, and I look forward to your
-contribution~ - [ ] fix SgpUtil(currently not work) - [ ] support RankUtil in
-CMD - [ ] fix JavLibUtil(currently not work because of cloudflare) - [x] cache
-the successful query results locally (Thanks: [@akynazh](https://github.com/
-akynazh)) - [x] support javdb.com (Thanks: [@Steven-Fake](https://github.com/
-Steven-Fake)) - [ ] support db.msin.jp - [x] support JavDbUtil in cmd (Thanks:
-[@akynazh](https://github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)
-_l_o_g_o_._]Thanks to JetBrains for their support to this project!
+contribution~ - [ ] support RankUtil in CMD - [x] cache the successful query
+results locally (Thanks: [@akynazh](https://github.com/akynazh)) - [x] support
+javdb.com (Thanks: [@Steven-Fake](https://github.com/Steven-Fake)) - [ ]
+support db.msin.jp - [x] support JavDbUtil in cmd (Thanks: [@akynazh](https://
+github.com/akynazh)) ## Thanks _[_J_e_t_B_r_a_i_n_s_ _L_o_g_o_ _(_M_a_i_n_)_ _l_o_g_o_._]Thanks to JetBrains
+for their support to this project!
```

### Comparing `Jvav-2.0.0/jvav/cmd.py` & `Jvav-2.1.0/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-2.0.0/jvav/utils.py` & `Jvav-2.1.0/jvav/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,20 @@
 from anti_useragent import UserAgent
 from bs4 import BeautifulSoup
 from deep_translator import GoogleTranslator
 
 
 class BaseUtil:
     def __init__(self, proxy_addr="", use_cache=True):
-        """初始化
-
-        :param str proxy_addr: 代理服务器地址, 默认为 ''
-        """
-
         self.log = logging.getLogger(__name__)
-        self.proxy_addr = ""
+        self.proxy_addr = proxy_addr
         self.use_cache = use_cache
-        if proxy_addr != "":
-            self.proxy_addr = proxy_addr
+        self.proxy_json = None
         if self.proxy_addr != "":
             self.proxy_json = {"http": proxy_addr, "https": proxy_addr}
-        else:
-            self.proxy_json = {"http": "", "https": ""}
 
     @staticmethod
     def ua_mobile() -> str:
         """返回手机端 UserAgent
 
         :return str: 手机端 UserAgent
         """
@@ -51,59 +43,59 @@
     def ua() -> str:
         """随机返回 UserAgent
 
         :return str: UserAgent
         """
         return UserAgent().random
 
-    def _inner_send_req(
-            self, url: str, session, headers={}, proxies={}, m=0, **args
-    ) -> Union[Tuple[int, None], Tuple[int, Any]]:
-        if headers == {}:
+    def _inner_send_req(self, url: str, session, headers=None, m=0, **args) -> Union[Tuple[int, None], Tuple[int, Any]]:
+        if not headers:
             headers = {"user-agent": self.ua()}
-        if proxies == {}:
-            proxies = self.proxy_json
         try:
-            if m == 0:
-                resp = session.get(url, proxies=proxies, headers=headers, **args)
-            elif m == 1:
-                resp = session.post(url, proxies=proxies, headers=headers, **args)
-            elif m == 2:
-                resp = session.delete(url, proxies=proxies, headers=headers, **args)
-            elif m == 3:
-                resp = session.put(url, proxies=proxies, headers=headers, **args)
-            if resp.status_code != 200:
-                return 404, None
-            return 200, resp
+            methods = {
+                0: session.get,
+                1: session.post,
+                2: session.delete,
+                3: session.put
+            }
+            if m in methods:
+                if self.proxy_json:
+                    resp = methods[m](url, proxies=self.proxy_json, headers=headers, **args)
+                else:
+                    resp = methods[m](url, headers=headers, **args)
+                if resp.status_code != 200:
+                    return 404, None
+                return 200, resp
+            else:
+                return 502, None
         except Exception as e:
             self.log.error(f"BaseUtil: 访问 {url}: {e}")
             return 502, None
 
     def send_req(
-            self, url: str, headers={}, proxies={}, m=0, **args
+            self, url: str, headers=None, m=0, **args
     ) -> Tuple[int, requests.Response]:
         """发送请求
 
         :param str url: 地址
         :param dict headers: 请求头, 默认使用随机请求头
-        :param dict proxies: 代理字典, 默认使用类初始化时指定的代理进行配置
         :param int m: 请求方法, 默认为 get(0), 其他为 post(1), delete(2), put(3)
         :param dict args: 其他 requests 参数
         :return tuple[int, requests.Response] 状态码和请求返回值
         关于状态码:
         200: 成功
         404: 未找到
-        502: 网络问题
+        502: 后台/网络问题
         """
         if self.use_cache:
             with requests_cache.CachedSession(cache_name=".jvav_cache") as session:
-                return self._inner_send_req(url, session, headers, proxies, m, **args)
+                return self._inner_send_req(url, session, headers, m, **args)
         else:
             with requests.Session() as session:
-                return self._inner_send_req(url, session, headers, proxies, m, **args)
+                return self._inner_send_req(url, session, headers, m, **args)
 
     @staticmethod
     def get_soup(resp: requests.Response) -> BeautifulSoup:
         """从请求结果得到 soup
 
         :param requests.Response resp: 请求结果
         :return BeautifulSoup
```

### Comparing `Jvav-2.0.0/requirements.txt` & `Jvav-2.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `Jvav-2.0.0/setup.py` & `Jvav-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="2.0.0",
+    version="2.1.0",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```

